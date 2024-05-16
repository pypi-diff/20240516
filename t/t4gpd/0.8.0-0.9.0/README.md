# Comparing `tmp/t4gpd-0.8.0.tar.gz` & `tmp/t4gpd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4gpd-0.8.0.tar", last modified: Fri Oct 13 09:39:30 2023, max compression
+gzip compressed data, was "t4gpd-0.9.0.tar", last modified: Mon Apr 15 13:22:43 2024, max compression
```

## Comparing `t4gpd-0.8.0.tar` & `t4gpd-0.9.0.tar`

### file list

```diff
@@ -1,399 +1,434 @@
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    35149 2020-06-13 17:54:58.000000 t4gpd-0.8.0/LICENSE.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2782 2023-10-13 09:39:30.590844 t4gpd-0.8.0/PKG-INFO
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1490 2023-07-28 09:15:27.000000 t4gpd-0.8.0/README.md
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      107 2023-10-13 09:39:30.590844 t4gpd-0.8.0/setup.cfg
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2141 2022-08-24 08:30:43.000000 t4gpd-0.8.0/setup.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.550845 t4gpd-0.8.0/t4gpd/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      739 2020-11-20 20:32:18.000000 t4gpd-0.8.0/t4gpd/__init__.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      804 2023-10-13 09:29:54.000000 t4gpd-0.8.0/t4gpd/_version.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.550845 t4gpd-0.8.0/t4gpd/avidon/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1671 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2482 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2544 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3769 2021-12-09 09:18:21.000000 t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4490 2022-03-10 16:50:36.000000 t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5774 2022-03-28 12:53:44.000000 t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels3.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-27 19:26:48.000000 t4gpd-0.8.0/t4gpd/avidon/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.554844 t4gpd-0.8.0/t4gpd/avidon/commons/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    10094 2022-03-28 15:25:46.000000 t4gpd-0.8.0/t4gpd/avidon/commons/AbstractEnergyDemand.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1662 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/commons/EnergyDemandCalculator.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1907 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1517 2021-07-01 18:48:52.000000 t4gpd-0.8.0/t4gpd/avidon/commons/Wh.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-27 19:24:53.000000 t4gpd-0.8.0/t4gpd/avidon/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.554844 t4gpd-0.8.0/t4gpd/avidon/scenarios/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      973 2021-06-25 08:28:23.000000 t4gpd-0.8.0/t4gpd/avidon/scenarios/AbstractScenario.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3045 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/scenarios/CredocBasedScenario.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2016 2023-10-06 16:06:25.000000 t4gpd-0.8.0/t4gpd/avidon/scenarios/FullLockdown.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-27 19:26:14.000000 t4gpd-0.8.0/t4gpd/avidon/scenarios/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.554844 t4gpd-0.8.0/t4gpd/comfort/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1492 2022-10-14 15:48:15.000000 t4gpd-0.8.0/t4gpd/comfort/EmpiricalThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-17 12:41:51.000000 t4gpd-0.8.0/t4gpd/comfort/LinearThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2478 2022-10-14 15:47:50.000000 t4gpd-0.8.0/t4gpd/comfort/UniversalThermalIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-02 17:38:35.000000 t4gpd-0.8.0/t4gpd/comfort/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.554844 t4gpd-0.8.0/t4gpd/comfort/algo/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5931 2021-05-12 17:04:21.000000 t4gpd-0.8.0/t4gpd/comfort/algo/CommonsLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4716 2021-05-12 16:38:39.000000 t4gpd-0.8.0/t4gpd/comfort/algo/ConstantsLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7079 2021-05-17 12:10:26.000000 t4gpd-0.8.0/t4gpd/comfort/algo/ETULib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1432 2021-05-12 16:42:17.000000 t4gpd-0.8.0/t4gpd/comfort/algo/PETLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1874 2021-09-02 09:59:31.000000 t4gpd-0.8.0/t4gpd/comfort/algo/PMVLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1714 2021-05-17 13:02:49.000000 t4gpd-0.8.0/t4gpd/comfort/algo/PTLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2066 2021-09-02 10:00:06.000000 t4gpd-0.8.0/t4gpd/comfort/algo/SETLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8302 2021-12-10 17:18:50.000000 t4gpd-0.8.0/t4gpd/comfort/algo/SET_mist.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1380 2021-05-12 08:12:54.000000 t4gpd-0.8.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1877 2021-05-12 18:58:48.000000 t4gpd-0.8.0/t4gpd/comfort/algo/TmrtOutLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    17227 2022-10-24 09:23:00.000000 t4gpd-0.8.0/t4gpd/comfort/algo/UTCILib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13633 2021-02-04 21:08:03.000000 t4gpd-0.8.0/t4gpd/comfort/algo/VDI_PET_corrected.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1284 2022-10-24 09:21:44.000000 t4gpd-0.8.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-02-04 21:08:03.000000 t4gpd-0.8.0/t4gpd/comfort/algo/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.558845 t4gpd-0.8.0/t4gpd/comfort/indices/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2650 2022-10-14 15:46:56.000000 t4gpd-0.8.0/t4gpd/comfort/indices/ASV.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      876 2021-05-12 06:43:03.000000 t4gpd-0.8.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1980 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/DI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3216 2022-10-14 15:46:30.000000 t4gpd-0.8.0/t4gpd/comfort/indices/ETU.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2004 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/H.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2396 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/HI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2202 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/NET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2331 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/OUTSET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2037 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/PE.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3956 2023-09-14 08:19:02.000000 t4gpd-0.8.0/t4gpd/comfort/indices/PET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3088 2022-10-24 15:23:58.000000 t4gpd-0.8.0/t4gpd/comfort/indices/PMV.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2232 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/PT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2801 2022-10-24 15:23:09.000000 t4gpd-0.8.0/t4gpd/comfort/indices/SET.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3026 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/SETmist.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/THI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2223 2021-05-12 19:36:36.000000 t4gpd-0.8.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2178 2022-10-14 15:45:34.000000 t4gpd-0.8.0/t4gpd/comfort/indices/TmrtOut.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5838 2022-10-14 15:44:45.000000 t4gpd-0.8.0/t4gpd/comfort/indices/TmrtRadiometer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4014 2023-09-14 08:19:25.000000 t4gpd-0.8.0/t4gpd/comfort/indices/UTCI.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2660 2022-10-14 14:25:47.000000 t4gpd-0.8.0/t4gpd/comfort/indices/WCT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-05-11 16:27:08.000000 t4gpd-0.8.0/t4gpd/comfort/indices/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1608 2020-10-07 15:28:18.000000 t4gpd-0.8.0/t4gpd/commons/AngleLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1189 2021-01-07 07:59:17.000000 t4gpd-0.8.0/t4gpd/commons/ArrayCoding.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2308 2020-06-19 14:10:50.000000 t4gpd-0.8.0/t4gpd/commons/BoundingBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2366 2020-12-16 13:15:18.000000 t4gpd-0.8.0/t4gpd/commons/CSVLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1675 2021-07-01 09:32:35.000000 t4gpd-0.8.0/t4gpd/commons/CalendarLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7227 2021-06-16 14:25:07.000000 t4gpd-0.8.0/t4gpd/commons/CaliperLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      959 2020-10-02 12:26:10.000000 t4gpd-0.8.0/t4gpd/commons/Checksum.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4541 2020-12-15 16:02:11.000000 t4gpd-0.8.0/t4gpd/commons/ChrystalAlgorithm.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2163 2023-06-24 06:23:57.000000 t4gpd-0.8.0/t4gpd/commons/ColorTemperature.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1637 2022-10-26 07:58:39.000000 t4gpd-0.8.0/t4gpd/commons/DataFrameLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2271 2022-08-24 10:23:43.000000 t4gpd-0.8.0/t4gpd/commons/DateRangeLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4956 2022-05-18 15:38:27.000000 t4gpd-0.8.0/t4gpd/commons/DatetimeLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1770 2022-09-05 10:36:15.000000 t4gpd-0.8.0/t4gpd/commons/DiameterLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5876 2020-06-22 09:32:49.000000 t4gpd-0.8.0/t4gpd/commons/Distances.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2831 2022-01-18 19:42:17.000000 t4gpd-0.8.0/t4gpd/commons/Entropy.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2832 2020-09-11 17:04:11.000000 t4gpd-0.8.0/t4gpd/commons/Epsilon.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1357 2022-10-25 14:40:11.000000 t4gpd-0.8.0/t4gpd/commons/GeoDataFrameLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1907 2021-05-18 08:44:20.000000 t4gpd-0.8.0/t4gpd/commons/GeoProcess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    26169 2023-09-07 14:37:42.000000 t4gpd-0.8.0/t4gpd/commons/GeomLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5407 2022-09-07 15:04:19.000000 t4gpd-0.8.0/t4gpd/commons/GeomLib3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4427 2022-03-28 12:35:37.000000 t4gpd-0.8.0/t4gpd/commons/GridFaceLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1149 2020-06-19 13:58:19.000000 t4gpd-0.8.0/t4gpd/commons/IllegalArgumentTypeException.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5933 2022-11-08 14:40:17.000000 t4gpd-0.8.0/t4gpd/commons/KernelLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3784 2020-10-24 09:49:18.000000 t4gpd-0.8.0/t4gpd/commons/LandoltRingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2718 2023-09-20 16:14:18.000000 t4gpd-0.8.0/t4gpd/commons/LatLonLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2291 2021-04-12 07:38:42.000000 t4gpd-0.8.0/t4gpd/commons/LineStringCuttingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1989 2020-10-11 20:51:06.000000 t4gpd-0.8.0/t4gpd/commons/ListUtilities.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5301 2023-09-13 13:41:25.000000 t4gpd-0.8.0/t4gpd/commons/Logos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2108 2020-06-17 18:58:12.000000 t4gpd-0.8.0/t4gpd/commons/MyEdge.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2709 2020-09-24 09:53:56.000000 t4gpd-0.8.0/t4gpd/commons/MyNode.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8008 2022-06-13 13:36:47.000000 t4gpd-0.8.0/t4gpd/commons/PointsDensifierLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3137 2022-09-20 15:59:32.000000 t4gpd-0.8.0/t4gpd/commons/PointsDensifierLib3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2833 2020-06-22 09:34:45.000000 t4gpd-0.8.0/t4gpd/commons/PolarCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13455 2023-01-30 13:37:02.000000 t4gpd-0.8.0/t4gpd/commons/RayCasting2Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    13317 2023-02-16 10:09:06.000000 t4gpd-0.8.0/t4gpd/commons/RayCasting3Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    14307 2023-10-09 17:26:23.000000 t4gpd-0.8.0/t4gpd/commons/RayCasting4Lib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11700 2023-02-20 09:15:16.000000 t4gpd-0.8.0/t4gpd/commons/RayCastingLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5638 2022-07-20 08:24:45.000000 t4gpd-0.8.0/t4gpd/commons/RotationLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2201 2022-04-08 14:27:04.000000 t4gpd-0.8.0/t4gpd/commons/SVFLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2307 2023-07-28 09:19:12.000000 t4gpd-0.8.0/t4gpd/commons/ShannonEntropy.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1308 2022-07-19 14:44:29.000000 t4gpd-0.8.0/t4gpd/commons/SphericalCartesianCoordinates.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4937 2022-09-20 16:03:36.000000 t4gpd-0.8.0/t4gpd/commons/SphericalProjectionLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1404 2021-06-08 21:34:17.000000 t4gpd-0.8.0/t4gpd/commons/TestUtils.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1502 2023-05-24 21:14:34.000000 t4gpd-0.8.0/t4gpd/commons/WarnUtils.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 09:59:56.000000 t4gpd-0.8.0/t4gpd/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/crossroads_generation/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5464 2023-05-24 14:00:40.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_generation/Sequence.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2722 2023-05-23 14:00:27.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3626 2022-11-07 10:44:48.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 10:44:48.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_generation/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1860 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3791 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1070 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/FFTMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3228 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/FWTMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2953 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1160 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-11-07 14:02:08.000000 t4gpd-0.8.0/t4gpd/commons/crossroads_identification/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/ellipse/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2020-08-31 08:21:22.000000 t4gpd-0.8.0/t4gpd/commons/ellipse/EllipseLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25237 2020-06-23 22:05:17.000000 t4gpd-0.8.0/t4gpd/commons/ellipse/EllipticHullLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-23 22:04:55.000000 t4gpd-0.8.0/t4gpd/commons/ellipse/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/graph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6382 2021-03-24 08:57:48.000000 t4gpd-0.8.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4942 2023-01-27 17:52:06.000000 t4gpd-0.8.0/t4gpd/commons/graph/MCALib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4987 2020-11-23 09:56:15.000000 t4gpd-0.8.0/t4gpd/commons/graph/NeighborhoodLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2883 2020-11-23 09:55:51.000000 t4gpd-0.8.0/t4gpd/commons/graph/ShortestPathLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4289 2020-11-23 10:13:17.000000 t4gpd-0.8.0/t4gpd/commons/graph/UrbanGraphLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6322 2021-06-25 08:43:27.000000 t4gpd-0.8.0/t4gpd/commons/graph/UrbanGraphLibOld.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-21 18:40:43.000000 t4gpd-0.8.0/t4gpd/commons/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/grid/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2938 2023-10-09 09:13:06.000000 t4gpd-0.8.0/t4gpd/commons/grid/AbstractGridLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12292 2023-10-13 08:44:55.000000 t4gpd-0.8.0/t4gpd/commons/grid/GridLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-04-09 08:07:33.000000 t4gpd-0.8.0/t4gpd/commons/grid/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/isovists/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-11-25 21:42:21.000000 t4gpd-0.8.0/t4gpd/commons/isovists/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/rnd/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4458 2023-05-23 15:30:11.000000 t4gpd-0.8.0/t4gpd/commons/rnd/RandomPointPicking.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2023-01-09 09:57:47.000000 t4gpd-0.8.0/t4gpd/commons/rnd/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.562845 t4gpd-0.8.0/t4gpd/commons/sun/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2774 2021-04-21 15:35:41.000000 t4gpd-0.8.0/t4gpd/commons/sun/AbstractSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1441 2022-12-08 17:43:59.000000 t4gpd-0.8.0/t4gpd/commons/sun/DaylightLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1897 2021-06-01 20:45:53.000000 t4gpd-0.8.0/t4gpd/commons/sun/PySolarSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7584 2021-04-22 16:07:47.000000 t4gpd-0.8.0/t4gpd/commons/sun/ShadowLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6719 2021-04-21 15:36:33.000000 t4gpd-0.8.0/t4gpd/commons/sun/SoleneSunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2429 2022-05-18 15:30:31.000000 t4gpd-0.8.0/t4gpd/commons/sun/SunBeamLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8335 2021-12-10 17:17:50.000000 t4gpd-0.8.0/t4gpd/commons/sun/SunLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-21 13:30:14.000000 t4gpd-0.8.0/t4gpd/commons/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.570845 t4gpd-0.8.0/t4gpd/demos/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1113 2023-06-08 13:02:08.000000 t4gpd-0.8.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    65273 2023-10-09 07:13:33.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11796 2023-09-06 17:34:11.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   453528 2022-10-25 15:00:19.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos3.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8790 2023-09-06 17:34:29.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos4.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   745426 2022-07-18 15:50:21.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos5.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435846 2022-10-26 14:52:50.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos6.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    25686 2022-10-31 17:23:24.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos7.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   435537 2022-10-31 17:22:15.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos8.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    87842 2023-09-06 17:48:27.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos9.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   295105 2023-10-11 16:13:19.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosA.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   165363 2023-09-06 17:49:02.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosB.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)   193794 2023-06-08 13:03:08.000000 t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosC.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)  5706650 2023-09-07 15:28:30.000000 t4gpd-0.8.0/t4gpd/demos/NantesBDT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-01-26 22:34:45.000000 t4gpd-0.8.0/t4gpd/demos/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.574844 t4gpd-0.8.0/t4gpd/energy/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2456 2023-10-03 13:36:08.000000 t4gpd-0.8.0/t4gpd/energy/Angstrom.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7953 2023-09-22 08:31:50.000000 t4gpd-0.8.0/t4gpd/energy/DirectSolarIrradianceLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3194 2022-07-22 08:39:12.000000 t4gpd-0.8.0/t4gpd/energy/Dogniaux.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8738 2023-09-22 09:49:35.000000 t4gpd-0.8.0/t4gpd/energy/FelixMarboutin.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3035 2022-07-22 08:20:11.000000 t4gpd-0.8.0/t4gpd/energy/Perez.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1107 2022-07-22 08:20:39.000000 t4gpd-0.8.0/t4gpd/energy/Perraudeau.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3305 2022-07-22 08:21:55.000000 t4gpd-0.8.0/t4gpd/energy/PerrinDeBrichambaut.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3748 2022-07-22 08:40:41.000000 t4gpd-0.8.0/t4gpd/energy/PlotDirectNormalIrradiance.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5427 2023-10-03 13:36:47.000000 t4gpd-0.8.0/t4gpd/energy/PlotIrradiances.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3989 2023-09-22 09:49:53.000000 t4gpd-0.8.0/t4gpd/energy/WilliamAtkinson.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:57:12.000000 t4gpd-0.8.0/t4gpd/energy/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.574844 t4gpd-0.8.0/t4gpd/energy/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4517 2022-05-18 17:36:24.000000 t4gpd-0.8.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-28 20:49:22.000000 t4gpd-0.8.0/t4gpd/energy/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.574844 t4gpd-0.8.0/t4gpd/graph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1047 2020-12-31 14:32:10.000000 t4gpd-0.8.0/t4gpd/graph/STBetweennessCentrality.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1043 2020-12-19 20:28:37.000000 t4gpd-0.8.0/t4gpd/graph/STClosenessCentrality.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2657 2020-11-23 10:00:25.000000 t4gpd-0.8.0/t4gpd/graph/STRoadNeighborhood.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2459 2020-11-21 19:04:19.000000 t4gpd-0.8.0/t4gpd/graph/STShortestPath.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1644 2020-11-23 10:45:34.000000 t4gpd-0.8.0/t4gpd/graph/STToRoadsSections.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1474 2020-11-23 10:45:52.000000 t4gpd-0.8.0/t4gpd/graph/STToRoadsSectionsNodes.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 07:51:42.000000 t4gpd-0.8.0/t4gpd/graph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.574844 t4gpd-0.8.0/t4gpd/io/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1120 2023-04-29 15:30:18.000000 t4gpd-0.8.0/t4gpd/io/AbstractReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4231 2020-09-24 09:56:55.000000 t4gpd-0.8.0/t4gpd/io/CSVInertialSensorReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1889 2020-09-24 09:57:20.000000 t4gpd-0.8.0/t4gpd/io/CSVReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1884 2021-03-10 14:24:32.000000 t4gpd-0.8.0/t4gpd/io/CSVWKTReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2317 2021-03-10 14:24:47.000000 t4gpd-0.8.0/t4gpd/io/CSVWKTWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3373 2022-07-25 09:09:50.000000 t4gpd-0.8.0/t4gpd/io/CirReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1314 2022-07-25 09:34:22.000000 t4gpd-0.8.0/t4gpd/io/CirValReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3331 2021-03-10 21:07:26.000000 t4gpd-0.8.0/t4gpd/io/CirWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5578 2020-10-22 16:39:22.000000 t4gpd-0.8.0/t4gpd/io/CityGMLReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7156 2022-06-24 16:06:01.000000 t4gpd-0.8.0/t4gpd/io/GeoWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1829 2022-11-09 15:42:30.000000 t4gpd-0.8.0/t4gpd/io/GpkgLoader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1818 2022-11-09 15:42:30.000000 t4gpd-0.8.0/t4gpd/io/GpkgWriter.py
--rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)     1879 2023-09-27 14:33:47.000000 t4gpd-0.8.0/t4gpd/io/MedReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12097 2021-06-25 08:29:09.000000 t4gpd-0.8.0/t4gpd/io/MshReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3750 2020-08-25 16:50:36.000000 t4gpd-0.8.0/t4gpd/io/ObjReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3541 2021-02-01 10:43:14.000000 t4gpd-0.8.0/t4gpd/io/ObjWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1430 2021-07-19 15:31:30.000000 t4gpd-0.8.0/t4gpd/io/Reloading.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1152 2022-04-26 12:38:58.000000 t4gpd-0.8.0/t4gpd/io/STLoadAndClip.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3086 2020-06-19 14:12:42.000000 t4gpd-0.8.0/t4gpd/io/SVGWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5130 2022-07-26 12:53:22.000000 t4gpd-0.8.0/t4gpd/io/SalomeWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5030 2022-07-26 12:53:22.000000 t4gpd-0.8.0/t4gpd/io/SalomeWriterAndExtruder.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6490 2021-03-10 14:25:07.000000 t4gpd-0.8.0/t4gpd/io/VTUWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2492 2022-07-25 09:33:33.000000 t4gpd-0.8.0/t4gpd/io/ValReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2806 2021-11-08 15:20:17.000000 t4gpd-0.8.0/t4gpd/io/ZipLoader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3559 2021-10-18 16:00:12.000000 t4gpd-0.8.0/t4gpd/io/ZipWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 18:59:50.000000 t4gpd-0.8.0/t4gpd/io/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.578844 t4gpd-0.8.0/t4gpd/isovist/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4347 2022-07-27 15:30:51.000000 t4gpd-0.8.0/t4gpd/isovist/STIsovistField2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2243 2023-07-28 15:39:06.000000 t4gpd-0.8.0/t4gpd/isovist/STIsovistField2D_new.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-17 09:56:41.000000 t4gpd-0.8.0/t4gpd/isovist/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.578844 t4gpd-0.8.0/t4gpd/misc/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4972 2021-07-20 15:59:02.000000 t4gpd-0.8.0/t4gpd/misc/FrequencyHistogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5748 2023-03-23 17:02:07.000000 t4gpd-0.8.0/t4gpd/misc/OptimalNumberOfClusters.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5344 2021-11-14 15:44:04.000000 t4gpd-0.8.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2960 2021-10-01 15:35:34.000000 t4gpd-0.8.0/t4gpd/misc/PopulationPyramid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5500 2023-01-19 10:23:40.000000 t4gpd-0.8.0/t4gpd/misc/RoseMappingTool.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3038 2022-03-15 16:20:31.000000 t4gpd-0.8.0/t4gpd/misc/STCompass.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2311 2023-03-23 14:05:55.000000 t4gpd-0.8.0/t4gpd/misc/STDendrogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2023-03-23 16:15:02.000000 t4gpd-0.8.0/t4gpd/misc/STKMeans.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4364 2021-01-25 16:17:15.000000 t4gpd-0.8.0/t4gpd/misc/StreetOrientationHistogram.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4386 2022-12-13 18:08:58.000000 t4gpd-0.8.0/t4gpd/misc/TimelineTool.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2824 2021-03-15 16:13:35.000000 t4gpd-0.8.0/t4gpd/misc/WindRose.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-09-29 10:07:30.000000 t4gpd-0.8.0/t4gpd/misc/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.582844 t4gpd-0.8.0/t4gpd/morph/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2873 2021-08-25 16:19:57.000000 t4gpd-0.8.0/t4gpd/morph/GmshTriangulator.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2867 2023-10-13 09:27:02.000000 t4gpd-0.8.0/t4gpd/morph/STAdaptativeGrid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1413 2023-02-17 18:32:38.000000 t4gpd-0.8.0/t4gpd/morph/STBBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1793 2020-06-30 09:46:17.000000 t4gpd-0.8.0/t4gpd/morph/STClip.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4603 2022-08-24 09:39:40.000000 t4gpd-0.8.0/t4gpd/morph/STCoolscapesTessellation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2723 2023-05-23 14:01:31.000000 t4gpd-0.8.0/t4gpd/morph/STCrossroadsGeneration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2853 2023-02-14 11:31:50.000000 t4gpd-0.8.0/t4gpd/morph/STDilationErosion.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2103 2020-12-14 16:55:46.000000 t4gpd-0.8.0/t4gpd/morph/STExtractOpenSpaces.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3726 2021-04-02 09:43:35.000000 t4gpd-0.8.0/t4gpd/morph/STFacadesAnalysis.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8594 2023-02-20 08:30:55.000000 t4gpd-0.8.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2219 2023-10-13 08:46:55.000000 t4gpd-0.8.0/t4gpd/morph/STGrid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3323 2023-09-06 12:40:52.000000 t4gpd-0.8.0/t4gpd/morph/STHeightOfRoughness.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3688 2020-09-17 11:02:43.000000 t4gpd-0.8.0/t4gpd/morph/STIdentifyRowOfTrees.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4480 2021-12-09 14:49:10.000000 t4gpd-0.8.0/t4gpd/morph/STMakeBlocks.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1701 2023-06-07 10:51:36.000000 t4gpd-0.8.0/t4gpd/morph/STMakeGroundSurface.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2812 2020-09-21 14:15:12.000000 t4gpd-0.8.0/t4gpd/morph/STMultipleOverlaps.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4550 2023-02-20 08:36:37.000000 t4gpd-0.8.0/t4gpd/morph/STMultipleOverlaps2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3134 2022-06-13 13:37:40.000000 t4gpd-0.8.0/t4gpd/morph/STPointsDensifier.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2118 2022-06-13 13:11:05.000000 t4gpd-0.8.0/t4gpd/morph/STPointsDensifier2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1717 2020-12-31 16:03:16.000000 t4gpd-0.8.0/t4gpd/morph/STPolygonize.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3105 2023-02-15 17:59:34.000000 t4gpd-0.8.0/t4gpd/morph/STSkeletonize.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2294 2023-02-15 20:25:15.000000 t4gpd-0.8.0/t4gpd/morph/STSkeletonizeTheVoid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6229 2023-10-09 08:09:41.000000 t4gpd-0.8.0/t4gpd/morph/STSkyMap25D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3196 2020-09-24 10:27:56.000000 t4gpd-0.8.0/t4gpd/morph/STSnappingPointsOnLines.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6567 2022-08-24 09:55:25.000000 t4gpd-0.8.0/t4gpd/morph/STSnappingPointsOnLines2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3217 2021-05-18 08:45:03.000000 t4gpd-0.8.0/t4gpd/morph/STSpatialJoin.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1568 2022-10-14 10:00:03.000000 t4gpd-0.8.0/t4gpd/morph/STSquaredBBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2747 2023-09-06 10:08:54.000000 t4gpd-0.8.0/t4gpd/morph/STSurfaceFraction.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2628 2023-01-31 10:54:56.000000 t4gpd-0.8.0/t4gpd/morph/STVariableWidthBuffer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3729 2020-09-25 16:31:01.000000 t4gpd-0.8.0/t4gpd/morph/STVoronoiPartition.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-31 10:00:08.000000 t4gpd-0.8.0/t4gpd/morph/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.586844 t4gpd-0.8.0/t4gpd/morph/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      941 2020-06-18 08:03:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2895 2020-06-19 14:16:30.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1132 2020-06-18 08:03:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4153 2023-01-30 15:34:51.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/AspectRatio.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1003 2020-06-18 08:03:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/BBox.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1813 2023-02-14 11:19:09.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1996 2020-10-07 15:31:07.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1851 2020-12-18 22:37:53.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/CircularityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      946 2020-06-18 08:03:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/ConvexHull.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1917 2020-12-18 22:29:45.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1903 2022-11-07 14:15:37.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4022 2022-11-08 14:46:29.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5107 2023-02-20 08:57:36.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1136 2020-06-19 14:45:22.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/Diameter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2106 2020-12-30 20:08:51.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3512 2022-07-22 14:38:29.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1100 2021-06-21 13:53:15.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1227 2022-03-28 12:36:54.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/GridFace.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2283 2023-01-30 16:12:41.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/HMean.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2179 2023-01-30 14:29:24.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2481 2021-02-14 18:01:56.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1564 2023-01-30 13:38:38.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2342 2020-06-23 22:09:00.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABE.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)      954 2020-06-18 08:03:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABR.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1067 2021-01-10 10:06:31.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABR2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1094 2020-12-15 16:02:50.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/MBC.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1065 2020-12-15 20:28:55.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/MPBR.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1600 2020-12-30 20:09:13.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1374 2022-11-08 14:46:29.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1749 2022-11-08 14:46:29.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1018 2020-06-19 07:17:45.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/RemoveHoles.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1628 2022-06-24 16:06:35.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1235 2021-04-26 14:02:10.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/Rotation2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3611 2023-03-15 18:24:43.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/STGeoProcess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3590 2023-09-12 16:06:46.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyMap2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2996 2023-01-30 15:49:55.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3657 2021-03-03 16:15:56.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1687 2022-01-18 09:14:29.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1898 2023-01-30 14:30:54.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1978 2021-04-26 13:48:42.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/Translation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1792 2023-01-30 16:09:52.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/WMean.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-06-16 15:16:57.000000 t4gpd-0.8.0/t4gpd/morph/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.586844 t4gpd-0.8.0/t4gpd/picoclim/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5476 2023-06-11 13:49:34.000000 t4gpd-0.8.0/t4gpd/picoclim/CampbellSciReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2312 2023-06-11 16:53:22.000000 t4gpd-0.8.0/t4gpd/picoclim/ExtraProcessing.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7497 2023-05-08 20:58:34.000000 t4gpd-0.8.0/t4gpd/picoclim/InertialMeasureReWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5574 2023-06-09 07:25:25.000000 t4gpd-0.8.0/t4gpd/picoclim/InertialMeasureReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3624 2023-03-22 16:43:01.000000 t4gpd-0.8.0/t4gpd/picoclim/JoinByTimeDistance.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6343 2023-06-09 07:11:48.000000 t4gpd-0.8.0/t4gpd/picoclim/KestrelReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2305 2022-10-26 10:49:53.000000 t4gpd-0.8.0/t4gpd/picoclim/MeteoFranceReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15062 2023-03-22 14:23:02.000000 t4gpd-0.8.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8963 2023-06-15 07:06:57.000000 t4gpd-0.8.0/t4gpd/picoclim/MetrologicalCampaignReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3314 2023-06-09 07:21:40.000000 t4gpd-0.8.0/t4gpd/picoclim/SensirionReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6589 2023-05-16 06:56:35.000000 t4gpd-0.8.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7288 2023-06-13 09:00:04.000000 t4gpd-0.8.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3531 2023-05-16 07:41:21.000000 t4gpd-0.8.0/t4gpd/picoclim/TracksWaypointsReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    15960 2023-06-13 08:00:50.000000 t4gpd-0.8.0/t4gpd/picoclim/UClimGuidingReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2860 2023-06-13 08:14:48.000000 t4gpd-0.8.0/t4gpd/picoclim/UClimTrackWaypointsReader.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-09-15 08:50:25.000000 t4gpd-0.8.0/t4gpd/picoclim/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.586844 t4gpd-0.8.0/t4gpd/pyplot/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4516 2022-11-07 14:14:25.000000 t4gpd-0.8.0/t4gpd/pyplot/MultipleMarkerStyles.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-01-31 17:29:02.000000 t4gpd-0.8.0/t4gpd/pyplot/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.586844 t4gpd-0.8.0/t4gpd/pyqgis/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3438 2022-07-29 07:32:07.000000 t4gpd-0.8.0/t4gpd/pyqgis/AddMemoryLayer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1629 2022-07-27 20:17:41.000000 t4gpd-0.8.0/t4gpd/pyqgis/Emphasizer.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8447 2022-07-10 14:41:36.000000 t4gpd-0.8.0/t4gpd/pyqgis/MapPrinter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5785 2023-07-28 09:19:12.000000 t4gpd-0.8.0/t4gpd/pyqgis/PdfMapWriter.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    10441 2023-04-14 15:51:46.000000 t4gpd-0.8.0/t4gpd/pyqgis/SetSymbolLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1323 2021-09-10 16:28:27.000000 t4gpd-0.8.0/t4gpd/pyqgis/ShowFeatureCount.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1746 2021-09-24 09:47:44.000000 t4gpd-0.8.0/t4gpd/pyqgis/ZoomLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-09-09 16:49:22.000000 t4gpd-0.8.0/t4gpd/pyqgis/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.586844 t4gpd-0.8.0/t4gpd/pyvista/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3711 2022-09-02 07:34:06.000000 t4gpd-0.8.0/t4gpd/pyvista/GeodeCiel.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4689 2022-09-01 16:13:45.000000 t4gpd-0.8.0/t4gpd/pyvista/Icosahedron.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    11484 2023-09-27 14:32:53.000000 t4gpd-0.8.0/t4gpd/pyvista/Plotter3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2043 2022-06-22 15:52:10.000000 t4gpd-0.8.0/t4gpd/pyvista/STRaysToViewFactors.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3916 2022-06-05 15:29:14.000000 t4gpd-0.8.0/t4gpd/pyvista/ToPolyData.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4642 2022-09-25 09:28:13.000000 t4gpd-0.8.0/t4gpd/pyvista/ToUnstructuredGrid.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-04-05 17:09:50.000000 t4gpd-0.8.0/t4gpd/pyvista/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/t4gpd/pyvista/commons/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1805 2022-09-05 12:42:46.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/Diameter3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8778 2022-09-01 16:15:11.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/RayCasting3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     7389 2022-09-05 16:44:01.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     8995 2022-09-07 10:57:40.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/SVF3DLib.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3683 2022-08-23 11:33:51.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/Triangle3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-05 21:07:30.000000 t4gpd-0.8.0/t4gpd/pyvista/commons/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3127 2022-07-18 15:37:08.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1398 2022-07-18 07:24:52.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1686 2022-06-22 16:23:38.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4679 2022-08-22 15:26:00.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4542 2022-08-24 08:46:07.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     6047 2022-09-05 16:44:47.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3951 2022-09-05 16:45:02.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/SVF3D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2022-06-09 11:51:20.000000 t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/t4gpd/raster/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1887 2023-10-05 15:57:41.000000 t4gpd-0.8.0/t4gpd/raster/AbstractRasterGeoProcess.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2453 2023-10-05 15:58:49.000000 t4gpd-0.8.0/t4gpd/raster/RTClip.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     5819 2023-10-05 15:59:45.000000 t4gpd-0.8.0/t4gpd/raster/RTFromArrayToRaster.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2762 2023-10-05 16:07:22.000000 t4gpd-0.8.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     1339 2023-08-22 14:37:41.000000 t4gpd-0.8.0/t4gpd/raster/RTLoad.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3037 2023-10-05 16:00:29.000000 t4gpd-0.8.0/t4gpd/raster/RTNdvi.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2445 2023-08-22 14:38:30.000000 t4gpd-0.8.0/t4gpd/raster/RTToFile.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2665 2023-10-05 16:02:43.000000 t4gpd-0.8.0/t4gpd/raster/RTVectorize.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3965 2023-10-05 16:02:00.000000 t4gpd-0.8.0/t4gpd/raster/STRasterize.py
--rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)     2916 2022-06-01 18:54:37.000000 t4gpd-0.8.0/t4gpd/raster/STToRaster.py
--rwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2022-06-01 12:59:39.000000 t4gpd-0.8.0/t4gpd/raster/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/t4gpd/sun/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2041 2021-04-22 15:43:22.000000 t4gpd-0.8.0/t4gpd/sun/AbstractHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3176 2022-05-18 15:39:03.000000 t4gpd-0.8.0/t4gpd/sun/STHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4002 2022-05-18 15:39:34.000000 t4gpd-0.8.0/t4gpd/sun/STSunMap2D.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     3423 2022-05-18 15:44:21.000000 t4gpd-0.8.0/t4gpd/sun/STTreeHardShadow.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4353 2022-05-18 15:44:39.000000 t4gpd-0.8.0/t4gpd/sun/STTreeHardShadow2.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2020-08-25 13:41:14.000000 t4gpd-0.8.0/t4gpd/sun/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.590844 t4gpd-0.8.0/t4gpd/sun/geoProcesses/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2489 2021-04-21 16:17:23.000000 t4gpd-0.8.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2218 2021-04-21 16:17:37.000000 t4gpd-0.8.0/t4gpd/sun/geoProcesses/SunshineDuration.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     4779 2021-04-21 16:17:58.000000 t4gpd-0.8.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        0 2021-03-03 15:05:24.000000 t4gpd-0.8.0/t4gpd/sun/geoProcesses/__init__.py
-drwxrwxr-x   0 tleduc    (1001) tleduc    (1001)        0 2023-10-13 09:39:30.550845 t4gpd-0.8.0/t4gpd.egg-info/
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)     2782 2023-10-13 09:39:30.000000 t4gpd-0.8.0/t4gpd.egg-info/PKG-INFO
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)    12385 2023-10-13 09:39:30.000000 t4gpd-0.8.0/t4gpd.egg-info/SOURCES.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        1 2023-10-13 09:39:30.000000 t4gpd-0.8.0/t4gpd.egg-info/dependency_links.txt
--rw-rw-r--   0 tleduc    (1001) tleduc    (1001)        6 2023-10-13 09:39:30.000000 t4gpd-0.8.0/t4gpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 13:22:39.000000 t4gpd-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 13:22:43.727097 t4gpd-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 13:22:43.731097 t4gpd-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-15 13:22:39.000000 t4gpd-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.659097 t4gpd-0.9.0/t4gpd/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels3.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/AbstractEnergyDemand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/Wh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/AbstractScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/CredocBasedScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/FullLockdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/comfort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/EmpiricalThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/LinearThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/UniversalThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.667096 t4gpd-0.9.0/t4gpd/comfort/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/CommonsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/ConstantsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/ETULib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PETLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PMVLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PTLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/SETLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/SET_mist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/TmrtOutLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/UTCILib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/VDI_PET_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.667096 t4gpd-0.9.0/t4gpd/comfort/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/ASV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/DI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/ETU.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/H.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/HI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/NET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/OUTSET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/SET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/SETmist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/THI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtRadiometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/UTCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/WCT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.675097 t4gpd-0.9.0/t4gpd/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/AngleLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ArrayCoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CSVLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CalendarLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CaliperLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CartesianProductLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ChrystalAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ColorTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ConcaveLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DataFrameLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DateRangeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DatetimeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DiameterLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeoDataFrameLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeomLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeomLib3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GridFaceLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/IllegalArgumentTypeException.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/KernelLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LandoltRingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LatLonLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LineStringCuttingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ListUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/MyEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/MyNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PolarCartesianCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting2Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting3Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting4Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCastingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RotationLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SVFLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ShannonEntropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SphericalCartesianCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SphericalProjectionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/TypeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/WarnUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.675097 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/Sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FFTMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FWTMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/ellipse/
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/EllipseLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/EllipticHullLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/MCALib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/NeighborhoodLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/ShortestPathLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLibOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphVertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/AbstractGridLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/GridLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/isovists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/isovists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/moon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/moon/MoonLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/moon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/proj/
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfPointsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfWallsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/raycasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/PanopticRaysLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/PrepareMasksLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting25DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting2DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/rnd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/rnd/RandomPointPicking.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/rnd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/AbstractSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/DaylightLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/PySolarSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/ShadowLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SoleneSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SunBeamLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.695097 t4gpd-0.9.0/t4gpd/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66648 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   453528 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   745426 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos5.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435846 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos7.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435537 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87828 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos9.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosA.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165363 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosB.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220246 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosC.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5706650 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/NantesBDT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Angstrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/DirectSolarIrradianceLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Dogniaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/FelixMarboutin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Perez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Perraudeau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PerrinDeBrichambaut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PlotDirectNormalIrradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PlotIrradiances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/WilliamAtkinson.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/energy/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STBetweennessCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STClosenessCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STDegreeCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STDelaunayGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STMinimumSpanningTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STRoadNeighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STShortestPath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STToRoadsSections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STToRoadsSectionsNodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.703096 t4gpd-0.9.0/t4gpd/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/AbstractReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVInertialSensorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVWKTReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVWKTWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirValReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CityGMLReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GeoWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GpkgLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GpkgWriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/MedReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/MshReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ObjReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ObjWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/Reloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/STLoadAndClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SVGWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SalomeWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SalomeWriterAndExtruder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/VTUWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ValReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ZipLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ZipWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.703096 t4gpd-0.9.0/t4gpd/isovist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.707096 t4gpd-0.9.0/t4gpd/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/FrequencyHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/OptimalNumberOfClusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/PopulationPyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/RoseMappingTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STCompass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STDendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STKMeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/StreetOrientationHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/TimelineTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/WindRose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.711097 t4gpd-0.9.0/t4gpd/morph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/GmshTriangulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STAdaptativeGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STBBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STCoolscapesTessellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STCrossroadsGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STDilationErosion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STExtractOpenSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STFacadesAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STHeightOfRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STIdentifyRowOfTrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMakeBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMakeGroundSurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPointsDensifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPointsDensifier2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPolygonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkeletonizeTheVoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkyMap25D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSpatialJoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSquaredBBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSurfaceFraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STVariableWidthBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STVoronoiPartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.715097 t4gpd-0.9.0/t4gpd/morph/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AspectRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/BBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CircularityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexHull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Diameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/GridFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/HMean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MBC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MPBR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RemoveHoles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Rotation2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/STGeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyMap2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/WMean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/picoclim/
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/CampbellSciReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/ExtraProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/JoinByTimeDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/KestrelReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MeteoFranceReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SensirionReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/TracksWaypointsReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/UClimGuidingReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/UClimTrackWaypointsReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/pyplot/
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyplot/MultipleMarkerStyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/pyqgis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/AddMemoryLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/Emphasizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/MapPrinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/PdfMapWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/SetSymbolLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/ShowFeatureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/ZoomLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/GeodeCiel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/Icosahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/Plotter3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/STRaysToViewFactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/ToPolyData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/ToUnstructuredGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/Diameter3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/RayCasting3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/SVF3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/Triangle3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/SVF3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/AbstractRasterGeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTFromArrayToRaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTNdvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTToFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTVectorize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4110 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STFromGridToRaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STRasterize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2916 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STToRaster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/AbstractHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STSunMap2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/sun/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/wrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFranceAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFrancePredictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFranceReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/ws/BDTopoWFSReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/ws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/top_level.txt
```

### Comparing `t4gpd-0.8.0/LICENSE.txt` & `t4gpd-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/PKG-INFO` & `t4gpd-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.8.0
+Version: 0.9.0
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
+Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
-Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
-Description: # t4gpd
-        Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
-        
-        ## Pre-requisites
-        To be able to use the **t4gpd** plugin, perform geoprocessing and display your own maps, you need a Python3 interpreter and recent versions of the geopandas, matplotlib, numpy, and shapely libraries. One possibility is to install a [Miniconda3](https://docs.conda.io/en/latest/miniconda.html) environment, in which you will first create and then configure a new environment (we will call it gpd):
-        > conda create -n gpd
-        
-        > conda activate gpd
-        
-        > conda config --env --add channels conda-forge
-        
-        > conda config --env --set channel_priority strict
-        
-        > conda install python=3.10 geopandas=0.12.2 jupyterlab matplotlib notebook scikit-learn xlrd openpyxl imageio rasterio networkx PyWavelets pysolar windrose geocube mapclassify seaborn plotly matplotlib-scalebar pyvista contextily xlwt
-        
-        > pip install Dijkstar suntimes pythermalcomfort
-        
-        ## Installation instructions
-        As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
-        > pip install t4gpd
-        
-        Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-        > pip install t4gpd-0.7.1.tar.gz
-        
-        ## Read the documentation
-        Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
-        
-        
-        
-        
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# t4gpd
+Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
+
+## Pre-requisites
+To be able to use the **t4gpd** plugin, perform geoprocessing and display your own maps, you need a Python3 interpreter and recent versions of the geopandas, matplotlib, numpy, and shapely libraries. One possibility is to install a [Miniconda3](https://docs.conda.io/en/latest/miniconda.html) environment, in which you will first create and then configure a new environment (we will call it gpd):
+> conda create -n gpd
+
+> conda activate gpd
+
+> conda config --env --add channels conda-forge
+
+> conda config --env --set channel_priority strict
+
+> conda install python=3.10 geopandas=0.12.2 contextily geocube imageio jupyterlab mapclassify matplotlib matplotlib-scalebar meshio networkx notebook openpyxl plotly pvlib Pyarrow pysolar pyvista pywavelets rasterio scikit-learn scipy seaborn windrose xlrd xlwt
+
+> pip install dijkstar pythermalcomfort suntimes
+
+## Installation instructions
+As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
+> pip install t4gpd
+
+Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
+> pip install t4gpd-0.9.0.tar.gz
+
+## Read the documentation
+Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
+
+
+
```

### Comparing `t4gpd-0.8.0/README.md` & `t4gpd-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 > conda activate gpd
 
 > conda config --env --add channels conda-forge
 
 > conda config --env --set channel_priority strict
 
-> conda install python=3.10 geopandas=0.12.2 jupyterlab matplotlib notebook scikit-learn xlrd openpyxl imageio rasterio networkx PyWavelets pysolar windrose geocube mapclassify seaborn plotly matplotlib-scalebar pyvista contextily xlwt
+> conda install python=3.10 geopandas=0.12.2 contextily geocube imageio jupyterlab mapclassify matplotlib matplotlib-scalebar meshio networkx notebook openpyxl plotly pvlib Pyarrow pysolar pyvista pywavelets rasterio scikit-learn scipy seaborn windrose xlrd xlwt
 
-> pip install Dijkstar suntimes pythermalcomfort
+> pip install dijkstar pythermalcomfort suntimes
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.7.1.tar.gz
+> pip install t4gpd-0.9.0.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.8.0/setup.py` & `t4gpd-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/__init__.py` & `t4gpd-0.9.0/t4gpd/__init__.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/_version.py` & `t4gpd-0.9.0/t4gpd/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 20 nov. 2020
 
 @author: tleduc
 
-Copyright 2020-2023 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -17,8 +17,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 # The following line *must* be the last in the module, exactly as formatted:
-__version__ = '0.8.0'
+__version__ = '0.9.0'
```

### Comparing `t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment.py` & `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py` & `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py` & `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels.py` & `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels2.py` & `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/STDeploymentOfPVPanels3.py` & `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/commons/AbstractEnergyDemand.py` & `t4gpd-0.9.0/t4gpd/avidon/commons/AbstractEnergyDemand.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/commons/EnergyDemandCalculator.py` & `t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py` & `t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/commons/Wh.py` & `t4gpd-0.9.0/t4gpd/avidon/commons/Wh.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/scenarios/AbstractScenario.py` & `t4gpd-0.9.0/t4gpd/avidon/scenarios/AbstractScenario.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/scenarios/CredocBasedScenario.py` & `t4gpd-0.9.0/t4gpd/avidon/scenarios/CredocBasedScenario.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/avidon/scenarios/FullLockdown.py` & `t4gpd-0.9.0/t4gpd/avidon/scenarios/FullLockdown.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/EmpiricalThermalIndices.py` & `t4gpd-0.9.0/t4gpd/comfort/EmpiricalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/LinearThermalIndices.py` & `t4gpd-0.9.0/t4gpd/comfort/LinearThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/UniversalThermalIndices.py` & `t4gpd-0.9.0/t4gpd/comfort/UniversalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/CommonsLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/CommonsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/ConstantsLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/ConstantsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/ETULib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/ETULib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/PETLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/PETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/PMVLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/PMVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/PTLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/PTLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/SETLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/SETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/SET_mist.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/SET_mist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/TmrtOutLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/TmrtOutLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/UTCILib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/UTCILib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/VDI_PET_corrected.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/VDI_PET_corrected.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py` & `t4gpd-0.9.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/ASV.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/ASV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/DI.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/DI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/ETU.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/ETU.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/H.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/H.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/HI.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/HI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/NET.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/NET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/OUTSET.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/OUTSET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/PE.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/PE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/PET.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/PET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/PMV.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/PMV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/PT.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/PT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/SET.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/SET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/SETmist.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/SETmist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/THI.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/THI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/TmrtOut.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtOut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/TmrtRadiometer.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtRadiometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,17 @@
         _IRback = (ConstantsLib.alpha_l * ConstantsLib.F_lat * IRback)
         _SRlat = (ConstantsLib.alpha_k * ConstantsLib.F_lat * (SRright + SRleft + SRfront + SRback))
         _IRlat = (ConstantsLib.alpha_l * ConstantsLib.F_lat * (IRright + IRleft + IRfront + IRback))
 
         # calculation of the mean radiant temperature [C]
         T_mrt = ((S_rad / (ConstantsLib.epsi_p * ConstantsLib.sigma_B)) ** (0.25) - ConstantsLib.T_kel)
 
-        # T_mrt splitted in up, down and lateral IR and SR according to Middel and Krayenhoff (2019) and Kantor et al. (2016)
+        # T_mrt splitted in up, down and lateral IR and SR according to Middel and 
+        # Krayenhoff (2019, https://doi.org/10.1016/j.scitotenv.2019.06.085) and
+        # Kantor et al. (2016, https://doi.org/10.1515/geo-2016-0021)
         _ratio = T_mrt / S_rad
 
         T_mrt_SRUp = _ratio * _SRUp
         T_mrt_SRDn = _ratio * _SRDn
         T_mrt_IRUp = _ratio * _IRUp
         T_mrt_IRDn = _ratio * _IRDn
         T_mrt_SRright = _ratio * _SRright
```

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/UTCI.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/UTCI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/comfort/indices/WCT.py` & `t4gpd-0.9.0/t4gpd/comfort/indices/WCT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/AngleLib.py` & `t4gpd-0.9.0/t4gpd/commons/AngleLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/ArrayCoding.py` & `t4gpd-0.9.0/t4gpd/commons/ArrayCoding.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/BoundingBox.py` & `t4gpd-0.9.0/t4gpd/commons/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/CSVLib.py` & `t4gpd-0.9.0/t4gpd/commons/CSVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/CalendarLib.py` & `t4gpd-0.9.0/t4gpd/commons/CalendarLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/CaliperLib.py` & `t4gpd-0.9.0/t4gpd/commons/CaliperLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/Checksum.py` & `t4gpd-0.9.0/t4gpd/commons/Checksum.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/ChrystalAlgorithm.py` & `t4gpd-0.9.0/t4gpd/commons/ChrystalAlgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 15 dec. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -38,26 +38,27 @@
         '''
         Constructor
         '''
         self.coords = list(geom.convex_hull.exterior.coords)[:-1]
         self.ncoords = len(self.coords)
 
     def __angleBetweenNodes(self, i, j, k):
-        result = AngleLib.angleBetweenNodes(self.coords[i], self.coords[j], self.coords[k])
+        result = AngleLib.angleBetweenNodes(
+            self.coords[i], self.coords[j], self.coords[k])
         return result if (result <= pi) else self.DPI - result
 
     def __getThirdNodeWithLowestAngleValue(self, idA, idB):
         minAngle, idC = inf, None
         for i in range(self.ncoords):
             if i not in (idA, idB):
                 tmp = self.__angleBetweenNodes(idA, i, idB)
                 if tmp < minAngle:
                     minAngle, idC = tmp, i
 
-        return [ idC, minAngle ]
+        return [idC, minAngle]
 
     def __getCircleViaCenterRadius(self, center, radius):
         center = Point(center)
         circle = center.buffer(radius)
         return [circle, center, radius]
 
     def __getCircleViaDiameter(self, diameter):
@@ -74,15 +75,16 @@
         else:
             abc_angle = self.__angleBetweenNodes(idA, idB, idC)
             cab_angle = self.__angleBetweenNodes(idC, idA, idB)
             maxAngle = max([abc_angle, bca_angle, cab_angle])
 
             if self.PI_DIV_2 > maxAngle:
                 # Un triangle acutangle est un triangle dont tous les angles sont aigus
-                center, radius = GeomLib.getCircumcircle(self.coords[idA], self.coords[idB], self.coords[idC])
+                center, radius = GeomLib.getCircumcircle(
+                    self.coords[idA], self.coords[idB], self.coords[idC])
                 return self.__getCircleViaCenterRadius(center, radius)
 
             elif self.PI_DIV_2 <= abc_angle:
                 # Un triangle obtusangle est un triangle qui a un angle obtus
                 return self.__aux(idA, idC)
 
             else:  # elif self.PI_DIV_2 <= cab_angle:
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/ColorTemperature.py` & `t4gpd-0.9.0/t4gpd/commons/ColorTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/DataFrameLib.py` & `t4gpd-0.9.0/t4gpd/commons/DataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/DateRangeLib.py` & `t4gpd-0.9.0/t4gpd/commons/DateRangeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/DatetimeLib.py` & `t4gpd-0.9.0/t4gpd/commons/DatetimeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/DiameterLib.py` & `t4gpd-0.9.0/t4gpd/commons/DiameterLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/Distances.py` & `t4gpd-0.9.0/t4gpd/commons/Distances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/Entropy.py` & `t4gpd-0.9.0/t4gpd/commons/Entropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/Epsilon.py` & `t4gpd-0.9.0/t4gpd/commons/Epsilon.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/GeoDataFrameLib.py` & `t4gpd-0.9.0/t4gpd/commons/GeoDataFrameLib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 13 mai 2022
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -18,28 +18,42 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas import GeoDataFrame
 from pandas import read_csv
+from shapely import LineString
 from shapely.wkt import loads
 
 
 class GeoDataFrameLib(object):
     '''
     classdocs
     '''
 
     @staticmethod
-    def read_csv(inputFile, decimal='.', sep=';', crs='epsg:2154'):
+    def isAGeoDataFrameOfBipoints(gdf):
+        return (isinstance(gdf, GeoDataFrame) and
+                all(gdf.geometry.apply(lambda g: isinstance(g, LineString))) and
+                all(gdf.geometry.apply(lambda g: 2 == len(g.coords)))
+                )
+
+    @staticmethod
+    def read_csv(inputFile, decimal=".", sep=";", crs="epsg:2154"):
         df = read_csv(inputFile, decimal=decimal, sep=sep)
         df.geometry = df.geometry.apply(lambda g: loads(g))
         return GeoDataFrame(df, crs=crs)
 
     @staticmethod
     def shareTheSameCrs(*gdfs):
-        return ((0 == len(gdfs)) or
-                all([
-                    (isinstance(gdf, GeoDataFrame) and (gdfs[0].crs == gdf.crs))
-                    for gdf in gdfs
-                    ]))
+        return (
+            (0 == len(gdfs)) or
+            all([
+                (isinstance(gdf, GeoDataFrame) and (gdfs[0].crs == gdf.crs))
+                for gdf in gdfs
+            ]) or
+            all([
+                (isinstance(gdf, GeoDataFrame) and (gdf.crs is None))
+                for gdf in gdfs
+            ])
+        )
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/GeoProcess.py` & `t4gpd-0.9.0/t4gpd/commons/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/GeomLib.py` & `t4gpd-0.9.0/t4gpd/commons/GeomLib.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from functools import reduce
 
+from geopandas import GeoDataFrame, overlay, sjoin_nearest
 from numpy import cos, sin, sqrt, pi
 from pandas.core.common import flatten
 from shapely.geometry import CAP_STYLE, GeometryCollection, LinearRing, LineString, MultiLineString, MultiPoint, MultiPolygon, Point, Polygon
 from shapely.ops import nearest_points, transform, unary_union
 from shapely.prepared import prep
 from t4gpd.commons.AngleLib import AngleLib
 from t4gpd.commons.Epsilon import Epsilon
@@ -173,23 +174,19 @@
                     n = n - 1
 
                 i += 1
 
         return result
 
     @staticmethod
-    def getEnclosingFeatures(inputGdf, inputSpatialIndex, point):
-        result = []
-        ids = list(inputSpatialIndex.intersection(point.bounds))
-        for _id in ids:
-            _feature = inputGdf.loc[_id]
-            _geom = _feature.geometry
-            if point.within(_geom):
-                result.append(_feature)
-        return result
+    def getEnclosingFeatures(inputGdf, point):
+        otherGdf = GeoDataFrame({"geometry": [point]}, crs=inputGdf.crs)
+        result = overlay(inputGdf, otherGdf,
+                         how="intersection", keep_geom_type=False)
+        return result.to_dict("records")
 
     @staticmethod
     def getCircumcircle(a, b, c):
         if GeomLib.areAligned(a, b, c):
             ab = GeomLib.distFromTo(a, b)
             bc = GeomLib.distFromTo(b, c)
             ca = GeomLib.distFromTo(c, a)
@@ -274,34 +271,23 @@
         raise IllegalArgumentTypeException(obj, 'Shapely geometry')
 
     @staticmethod
     def getMidPoint(a, b):
         return [(a[0] + b[0]) / 2.0, (a[1] + b[1]) / 2.0]
 
     @staticmethod
-    def getNearestFeature(inputGdf, inputSpatialIndex, point, buffDist, incScale=sqrt(2)):
+    def getNearestFeature(inputGdf, point):
         if not isinstance(point, Point):
-            raise IllegalArgumentTypeException(point, 'Point')
-
-        minDist, nearestPoint, nearestRow = float('inf'), None, None
+            raise IllegalArgumentTypeException(point, "Point")
 
-        ids = []
-        while (0 == len(ids)):
-            ids = list(inputSpatialIndex.intersection(
-                point.buffer(buffDist, -1).bounds))
-            buffDist *= incScale
-
-        for _id in ids:
-            row = inputGdf.loc[_id]
-            rowGeom = row.geometry
-            dist = point.distance(rowGeom)
-            if (dist < minDist):
-                minDist = dist
-                _, nearestPoint = nearest_points(point, rowGeom)
-                nearestRow = row
+        otherGdf = GeoDataFrame({"geometry": [point]}, crs=inputGdf.crs)
+        tmp = sjoin_nearest(inputGdf, otherGdf, distance_col="dist_to_pt")
+        nearestRow = tmp.loc[tmp.dist_to_pt.idxmin()]
+        minDist = nearestRow.dist_to_pt
+        nearestPoint = nearest_points(point, nearestRow.geometry)[1]
 
         return [minDist, nearestPoint, nearestRow]
 
     @staticmethod
     def getNearestFeature3(gdf, point, buffDist, incScale=sqrt(2)):
         if not isinstance(point, Point):
             raise IllegalArgumentTypeException(point, 'Point')
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/GeomLib3D.py` & `t4gpd-0.9.0/t4gpd/commons/GeomLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/GridFaceLib.py` & `t4gpd-0.9.0/t4gpd/commons/GridFaceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/IllegalArgumentTypeException.py` & `t4gpd-0.9.0/t4gpd/commons/IllegalArgumentTypeException.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/KernelLib.py` & `t4gpd-0.9.0/t4gpd/commons/KernelLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/LandoltRingLib.py` & `t4gpd-0.9.0/t4gpd/commons/LandoltRingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/LatLonLib.py` & `t4gpd-0.9.0/t4gpd/commons/LatLonLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/LineStringCuttingLib.py` & `t4gpd-0.9.0/t4gpd/commons/LineStringCuttingLib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 10 avr. 2021
 
 @author: tleduc
 
-Copyright 2020-2021 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,16 +16,17 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from shapely.geometry.linestring import LineString
+from geopandas import GeoDataFrame
+from shapely import LineString
+from shapely.ops import substring
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
 class LineStringCuttingLib(object):
     '''
     classdocs
@@ -55,9 +56,17 @@
     @staticmethod
     def cuttingIntoSegments(gdf, cuttingDist):
         result = []
         for _, row in gdf.iterrows():
             _geom = row.geometry
             _segms = GeomLib.toListOfBipointsAsLineStrings(_geom)
             for _segm in _segms:
-                result += LineStringCuttingLib.__fromLineStringToSegments(_segm, cuttingDist)
+                result += LineStringCuttingLib.__fromLineStringToSegments(
+                    _segm, cuttingDist)
         return GeoDataFrame([{'gid': i, 'geometry': g} for i, g in enumerate(result)], crs=gdf.crs)
+
+    @staticmethod
+    def lineStringShortener(gdf, start_dist, end_dist, normalized):
+        result = gdf.copy(deep=True)
+        result.geometry = result.geometry.apply(
+            lambda geom: substring(geom, start_dist, end_dist, normalized))
+        return result
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/ListUtilities.py` & `t4gpd-0.9.0/t4gpd/commons/ListUtilities.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/Logos.py` & `t4gpd-0.9.0/t4gpd/commons/Logos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/MyEdge.py` & `t4gpd-0.9.0/t4gpd/commons/MyEdge.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/MyNode.py` & `t4gpd-0.9.0/t4gpd/commons/MyNode.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/PointsDensifierLib.py` & `t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/PointsDensifierLib3D.py` & `t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/PolarCartesianCoordinates.py` & `t4gpd-0.9.0/t4gpd/commons/PolarCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/RayCasting2Lib.py` & `t4gpd-0.9.0/t4gpd/commons/RayCasting2Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/RayCasting3Lib.py` & `t4gpd-0.9.0/t4gpd/commons/RayCasting3Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/RayCasting4Lib.py` & `t4gpd-0.9.0/t4gpd/commons/RayCasting4Lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         if not GeomLib.isMultipart(mls):
             return Polygon([])
 
         _ctrPts1 = [ls.coords[-1] for ls in mls.geoms]
         if (nRays == len(_ctrPts1)):
             return Polygon(_ctrPts1)
 
-        viewpoint = viewpoint.coords[0][0:2]
+        viewpoint = viewpoint.centroid.coords[0][0:2]
         assert len(ray_ids) == len(_ctrPts1)
         assert ray_ids == sorted(ray_ids)
         _ctrPts2 = []
         for i, ray_id in enumerate(ray_ids):
             if (0 == i):
                 if (0 != ray_id):
                     _ctrPts2.append(viewpoint)
@@ -180,15 +180,15 @@
             isovRaysField, precision, base)
 
         isovRaysField["__ISOV_CENTRE__"] = isovRaysField.__ISOV_GEOM__.apply(
             lambda geom: geom.centroid)
 
         isovRaysField["vect_drift"] = isovRaysField.apply(
             lambda row: None if row.__ISOV_CENTRE__.is_empty else LineString([
-                row.viewpoint.coords[0][0:2], row.__ISOV_CENTRE__.coords[0]]), axis=1)
+                row.viewpoint.centroid.coords[0][0:2], row.__ISOV_CENTRE__.coords[0]]), axis=1)
         isovRaysField["drift"] = isovRaysField.vect_drift.apply(
             lambda v: None if v is None else v.length)
 
         isovRaysField.drop(
             columns=["__RAY_LEN__", "__ISOV_CENTRE__"], inplace=True)
         return isovRaysField
 
@@ -273,33 +273,41 @@
             raise Exception(
                 "Illegal argument: buildings and rays must share shames CRS!")
         rays.geometry = rays.geometry.apply(lambda geom: GeomLib.forceZCoordinateToZ0(
             geom, z0=geom.coords[0][2] if geom.has_z else h0))
 
         smapRaysField = overlay(rays, buildings.geometry.to_frame(
         ), how="intersection", keep_geom_type=True)
-        smapRaysField = smapRaysField.dissolve(by=["__VPT_ID__", "__RAY_ID__"], as_index=False, aggfunc={
-                                               "gid": "first", "viewpoint": "first"})
-        smapRaysField.geometry = smapRaysField.apply(lambda row: RayCasting4Lib.__keepTheLargestSolidAngle(
-            row.viewpoint, row.geometry), axis=1)
-        # smapRaysField.to_csv("/tmp/a.csv", index=False, sep=";")
-
-        left = rays.set_index(["__VPT_ID__", "__RAY_ID__"], drop=False)
-        left.drop(columns=["__VPT_ID__"], inplace=True)
-        right = smapRaysField.set_index(
-            ["__VPT_ID__", "__RAY_ID__"]).geometry.to_frame()
-        smapRaysField = left.merge(
-            right, how="outer", left_index=True, right_index=True)
-
-        smapRaysField["geometry"] = smapRaysField.apply(
-            lambda row: row.geometry_x if row.geometry_y is None else row.geometry_y, axis=1)
-        smapRaysField.drop(columns=["geometry_x", "geometry_y"], inplace=True)
-        smapRaysField = GeoDataFrame(smapRaysField, crs=buildings.crs)
-        smapRaysField = smapRaysField.loc[smapRaysField[~smapRaysField.geometry.apply(
-            lambda geom: geom.is_empty)].index, :]
+
+        if (0 == len(smapRaysField)):
+            smapRaysField = rays.set_index("__VPT_ID__", drop=True).set_index(
+                "__RAY_ID__", append=True, drop=False)
+        else:
+            smapRaysField = smapRaysField.dissolve(by=["__VPT_ID__", "__RAY_ID__"], as_index=False, aggfunc={
+                "gid": "first", "viewpoint": "first"})
+            smapRaysField.geometry = smapRaysField.apply(lambda row: RayCasting4Lib.__keepTheLargestSolidAngle(
+                row.viewpoint, row.geometry), axis=1)
+
+            left = rays.set_index(["__VPT_ID__", "__RAY_ID__"], drop=False)
+            left.drop(columns=["__VPT_ID__"], inplace=True)
+            right = smapRaysField.set_index(
+                ["__VPT_ID__", "__RAY_ID__"]).geometry.to_frame()
+            smapRaysField = left.merge(
+                right, how="outer", left_index=True, right_index=True)
+
+            smapRaysField["geometry"] = smapRaysField.apply(
+                lambda row: row.geometry_x if row.geometry_y is None else row.geometry_y, axis=1)
+            smapRaysField.drop(
+                columns=["geometry_x", "geometry_y"], inplace=True)
+            smapRaysField = GeoDataFrame(smapRaysField, crs=buildings.crs)
+            smapRaysField = smapRaysField.loc[smapRaysField[~smapRaysField.geometry.apply(
+                lambda geom: geom.is_empty)].index, :]
+            # smapRaysField.drop(
+            #     columns=["__RAY_ID__", "viewpoint"]).to_file("/tmp/6.shp")
+
         smapRaysField = smapRaysField.dissolve(
             by="__VPT_ID__", as_index=False, aggfunc=list)
         smapRaysField.drop(columns=["__VPT_ID__"], inplace=True)
         for fieldname in smapRaysField.columns:
             if fieldname not in ["geometry", "__RAY_ID__"]:
                 smapRaysField[fieldname] = smapRaysField[fieldname].apply(
                     lambda t: t[0])
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/RayCastingLib.py` & `t4gpd-0.9.0/t4gpd/commons/RayCastingLib.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,53 +19,57 @@
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas.geodataframe import GeoDataFrame
 from geopandas.sindex import PyGEOSSTRTreeIndex, SpatialIndex
 from numpy import cos, pi, sin
-from rtree.index import Index 
+from rtree.index import Index
 from shapely.geometry import LineString, MultiLineString, Point
 from shapely.ops import nearest_points, linemerge
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
 class RayCastingLib(object):
     '''
     classdocs
     '''
 
     @staticmethod
     def prepareOrientedRays(masksGdf, masksSIdx, viewPoint):
-        _, nearestPoint, _ = GeomLib.getNearestFeature(
-            masksGdf, masksSIdx, viewPoint, buffDist=40.0)
-        u = GeomLib.unitVector([viewPoint.x, viewPoint.y], [nearestPoint.x, nearestPoint.y])
+        _, nearestPoint, _ = GeomLib.getNearestFeature(masksGdf, viewPoint)
+        u = GeomLib.unitVector([viewPoint.x, viewPoint.y], [
+                               nearestPoint.x, nearestPoint.y])
         return [u, [-u[0], -u[1]]]
 
     @staticmethod
     def preparePanopticRays(nRays=64):
         angularOffset = (2.0 * pi) / nRays
-        shootingDirs = [[float(cos(angularOffset * i)), float(sin(angularOffset * i))] for i in range(nRays)]
+        shootingDirs = [[float(cos(angularOffset * i)),
+                         float(sin(angularOffset * i))] for i in range(nRays)]
         return shootingDirs
 
     @staticmethod
     def singleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength=100.0):
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
 
         # TL. 23.02.2021
         # To avoid: "Inconsistent coordinate dimensionality"
         viewPoint = Point((viewPoint.x, viewPoint.y))
-        remotePoint = Point((viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
-        ray = LineString([(viewPoint.x, viewPoint.y), (remotePoint.x, remotePoint.y)])
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
 
         hitPoint, hitDist, hitMask = [None, rayLength, None]
 
         masksIds = list(masksSIdx.intersection(ray.bounds))
         for maskId in masksIds:
             mask = masksGdf.loc[maskId]
             maskGeom = mask.geometry
@@ -73,37 +77,42 @@
                 _tmp = maskGeom.intersection(ray)
                 _, rp = nearest_points(viewPoint, _tmp)
                 dist = viewPoint.distance(rp)
                 if (dist < hitDist):
                     hitPoint, hitDist, hitMask = rp, dist, mask
 
         if hitPoint is not None:
-            ray = LineString([(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
         else:
             hitPoint = remotePoint
 
         return [ray, hitPoint, hitDist, hitMask]
 
     @staticmethod
     def singleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
                          elevationFieldName, background, h0=0.0):
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
         if elevationFieldName not in masksGdf:
-            raise Exception('%s is not a relevant field name!' % (elevationFieldName))
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
         # TL. 23.02.2021
         # To avoid: "Inconsistent coordinate dimensionality"
         viewPoint = Point((viewPoint.x, viewPoint.y, h0))
-        remotePoint = Point((viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength, h0))
-        ray = LineString([(viewPoint.x, viewPoint.y), (remotePoint.x, remotePoint.y)])
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength, h0))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
 
         hitPoint, hitDist, hitMask, hitHW = [None, rayLength, None, 0]
 
         masksIds = list(masksSIdx.intersection(ray.bounds))
         for maskId in masksIds:
             mask = masksGdf.loc[maskId]
             maskGeom = mask.geometry
@@ -114,38 +123,43 @@
                 hw = height / dist
                 if background and (hitHW < hw):
                     hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
                 elif (not background) and (dist < hitDist):
                     hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
 
         if hitPoint is not None:
-            ray = LineString([(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
         else:
             hitPoint = remotePoint
 
         return [ray, hitPoint, hitDist, hitMask, hitHW]
 
     @staticmethod
     def singleRayCastOnTopOfRoof(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
                                  h0, elevationFieldName, background):
-        
+
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
         if elevationFieldName not in masksGdf:
-            raise Exception('%s is not a relevant field name!' % (elevationFieldName))
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
         # TL. 23.02.2021
         # To avoid: "Inconsistent coordinate dimensionality"
         viewPoint = Point((viewPoint.x, viewPoint.y))
-        remotePoint = Point((viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
-        ray = LineString([(viewPoint.x, viewPoint.y), (remotePoint.x, remotePoint.y)])
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
 
         hitPoint, hitDist, hitMask, hitHW = [None, rayLength, None, 0]
 
         masksIds = list(masksSIdx.intersection(ray.bounds))
         for maskId in masksIds:
             mask = masksGdf.loc[maskId]
             maskGeom = mask.geometry
@@ -156,51 +170,56 @@
                 hw = (height - h0) / dist
                 if background and (hitHW < hw):
                     hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
                 elif (not background) and (dist < hitDist) and (0 < hw):
                     hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
 
         if hitPoint is not None:
-            ray = LineString([(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
         else:
             hitPoint = remotePoint
 
         return [ray, hitPoint, hitDist, hitMask, hitHW]
 
     @staticmethod
     def multipleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength=100.0):
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
 
         rays, hitPoints, hitDists, hitMasks = [[], [], [], []]
 
         for shootingDir in shootingDirs:
-            ray, hitPoint, hitDist, hitMask = RayCastingLib.singleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength)
+            ray, hitPoint, hitDist, hitMask = RayCastingLib.singleRayCast2D(
+                masksGdf, masksSIdx, viewPoint, shootingDir, rayLength)
             rays.append(ray)
             hitPoints.append(hitPoint)
             hitDists.append(hitDist)
             hitMasks.append(hitMask)
 
         return [MultiLineString(rays), hitPoints, hitDists, hitMasks]
 
     @staticmethod
     def multipleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength,
                            elevationFieldName, background, h0=0.0):
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
         if elevationFieldName not in masksGdf:
-            raise Exception('%s is not a relevant field name!' % (elevationFieldName))
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
         rays, hitPoints, hitDists, hitMasks, hitHWs = [[], [], [], [], []]
 
         for shootingDir in shootingDirs:
             ray, hitPoint, hitDist, hitMask, hitHW = RayCastingLib.singleRayCast25D(
                 masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
                 elevationFieldName, background, h0)
@@ -215,19 +234,21 @@
     @staticmethod
     def multipleRayCastOnTopOfRoof(masksGdf, masksSIdx, viewPoint, shootingDirs,
                                    rayLength, enclosingFeatures, elevationFieldName,
                                    background):
         if not isinstance(masksGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
         if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
-            raise IllegalArgumentTypeException(masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
         if not isinstance(viewPoint, Point):
             raise IllegalArgumentTypeException(viewPoint, 'Point')
         if elevationFieldName not in masksGdf:
-            raise Exception('%s is not a relevant field name!' % (elevationFieldName))
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
         rays, hitPoints, hitDists, hitMasks, hitHWs = [[], [], [], [], []]
         h0 = min([f[elevationFieldName] for f in enclosingFeatures])
 
         for shootingDir in shootingDirs:
             ray, hitPoint, hitDist, hitMask, hitHW = RayCastingLib.singleRayCastOnTopOfRoof(
                 masksGdf, masksSIdx, viewPoint, shootingDir, rayLength, h0,
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/RotationLib.py` & `t4gpd-0.9.0/t4gpd/commons/RotationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/SVFLib.py` & `t4gpd-0.9.0/t4gpd/commons/SVFLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/ShannonEntropy.py` & `t4gpd-0.9.0/t4gpd/commons/ShannonEntropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/SphericalCartesianCoordinates.py` & `t4gpd-0.9.0/t4gpd/commons/SphericalCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/SphericalProjectionLib.py` & `t4gpd-0.9.0/t4gpd/commons/SphericalProjectionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/TestUtils.py` & `t4gpd-0.9.0/t4gpd/commons/TestUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/WarnUtils.py` & `t4gpd-0.9.0/t4gpd/commons/WarnUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_generation/Sequence.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/Sequence.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_generation/SequenceRadii.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequenceRadii.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/AbstractMethod.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/AbstractMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/FFTMethod.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FFTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/FWTMethod.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FWTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py` & `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/ellipse/EllipseLib.py` & `t4gpd-0.9.0/t4gpd/commons/ellipse/EllipseLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/ellipse/EllipticHullLib.py` & `t4gpd-0.9.0/t4gpd/commons/ellipse/EllipticHullLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py` & `t4gpd-0.9.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/graph/MCALib.py` & `t4gpd-0.9.0/t4gpd/commons/graph/MCALib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/graph/ShortestPathLib.py` & `t4gpd-0.9.0/t4gpd/commons/graph/ShortestPathLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/graph/UrbanGraphLib.py` & `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/graph/UrbanGraphLibOld.py` & `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLibOld.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/grid/AbstractGridLib.py` & `t4gpd-0.9.0/t4gpd/commons/grid/AbstractGridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/grid/GridLib.py` & `t4gpd-0.9.0/t4gpd/commons/grid/GridLib.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,24 +104,24 @@
         yOffset = ((nrows * dy) - (maxy - miny)) / 2.0
 
         x0, y0 = minx - xOffset, miny - yOffset
 
         rows = []
         for c, x in enumerate(linspace(x0, x0 + ncols * dx, ncols, endpoint=False)):
             xpp = x+dx
-            for r, y in enumerate(linspace(y0, y0 + nrows * dx, nrows, endpoint=False)):
+            for r, y in enumerate(linspace(y0, y0 + nrows * dy, nrows, endpoint=False)):
                 ypp = y+dy
                 rows.append({
                     "gid": r * ncols + c,
                     "dx": dx,
                     "dy": dy,
                     "geometry": box(x, y, xpp, ypp)
                 })
         grid = GeoDataFrame(rows, crs=gdf.crs)
-        grid2 = GridLib.distanceToNearestContour(gdf, grid)
+        grid2 = GridLib.getDistanceToNearestContour(gdf, grid)
         return grid2
 
     @staticmethod
     def __neighbors_4_8(nrows, ncols, r, c):
         e = r * ncols + (c + 1)
         ne = (r + 1) * ncols + (c + 1)
         n = (r + 1) * ncols + c
@@ -154,15 +154,15 @@
         yOffset = ((nrows * dy) - (maxy - miny)) / 2.0
 
         x0, y0 = minx - xOffset, miny - yOffset
 
         rows = []
         for c, x in enumerate(linspace(x0, x0 + ncols * dx, ncols, endpoint=False)):
             xpp = x+dx
-            for r, y in enumerate(linspace(y0, y0 + nrows * dx, nrows, endpoint=False)):
+            for r, y in enumerate(linspace(y0, y0 + nrows * dy, nrows, endpoint=False)):
                 ypp = y+dy
                 neighbors4, neighbors8 = GridLib.__neighbors_4_8(
                     nrows, ncols, r, c)
                 if encode:
                     neighbors4, neighbors8 = (ArrayCoding.encode(neighbors4),
                                               ArrayCoding.encode(neighbors8))
                 rows.append({
@@ -172,25 +172,26 @@
                     "neighbors4": neighbors4,
                     "neighbors8": neighbors8,
                     # "dx": dx,
                     # "dy": dy,
                     "geometry": box(x, y, xpp, ypp)
                 })
         grid = GeoDataFrame(rows, crs=gdf.crs)
-        grid2 = GridLib.distanceToNearestContour(gdf, grid)
-        return grid2
+        return grid
 
     @staticmethod
-    def distanceToNearestContour(gdf, grid):
-        gdf = gdf.copy(deep=True)
-        gdf.geometry = gdf.geometry.apply(
+    def getDistanceToNearestContour(gdf, grid):
+        gdf2 = gdf.copy(deep=True)
+        gdf2.geometry = gdf2.geometry.apply(
             lambda geom: MultiLineString(GeomLib.toListOfLineStrings(geom)))
+        if "dist_to_ctr" in grid:
+            grid.drop(columns="dist_to_ctr", inplace=True)
         grid2 = sjoin_nearest(
-            grid, gdf[["geometry"]], how="inner", distance_col="dist_to_ctr", max_distance=None)
-        if ("index_right" not in gdf) and ("index_right" in grid2):
+            grid, gdf2[["geometry"]], how="inner", distance_col="dist_to_ctr", max_distance=None)
+        if ("index_right" not in gdf2) and ("index_right" in grid2):
             grid2.drop(columns="index_right", inplace=True)
         grid2.drop_duplicates(
             subset=["gid"], keep="first", ignore_index=True, inplace=True)
         return grid2
 
     @staticmethod
     def fromGridToNumpyArray(gdf, fieldvalue, rowFieldname="row", colFieldname="column"):
@@ -321,9 +322,9 @@
                         gid += 1
                         rows.append({
                             "gid": gid,
                             "dx": dx,
                             "geometry": box(x, y, xpp, ypp)
                         })
         grid2 = GeoDataFrame(rows, crs=gdf.crs)
-        grid3 = GridLib.distanceToNearestContour(gdf, grid2)
+        grid3 = GridLib.getDistanceToNearestContour(gdf, grid2)
         return grid3
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/rnd/RandomPointPicking.py` & `t4gpd-0.9.0/t4gpd/commons/rnd/RandomPointPicking.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/AbstractSunLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/AbstractSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/DaylightLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/DaylightLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/PySolarSunLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/PySolarSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/ShadowLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/ShadowLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/SoleneSunLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/SoleneSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/SunBeamLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/SunBeamLib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 28 avr. 2022
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -54,9 +54,8 @@
         ptA = position if GeomLib.is3D(position) else GeomLib.forceZCoordinateToZ0(position, z0=0.0)
         maxElevation = max(masks[maskElevationFieldname])
         sunModel = SunLib(masks, model)
         alti, azim = sunModel.getSolarAnglesInRadians(dt)
         R = (maxElevation - ptA.z) / tan(alti)
         ptB = Point([ptA.x + R * cos(azim), ptA.y + R * sin(azim), ptA.z + R * sin(alti)])
 
-        # return RayCasting2Lib.areCovisible(ptA, ptB, masks, maskElevationFieldname, masksSIdx)
         return RayCasting3Lib.areCovisibleIn3D(ptA, ptB, masks, maskElevationFieldname, masksSIdx)
```

### Comparing `t4gpd-0.8.0/t4gpd/commons/sun/SunLib.py` & `t4gpd-0.9.0/t4gpd/commons/sun/SunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/AbstractGeoDataFrameDemos.py` & `t4gpd-0.9.0/t4gpd/demos/AbstractGeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from io import StringIO
 
 from geopandas import clip, GeoDataFrame
+from shapely import union_all
 from shapely.affinity import rotate, translate
 from shapely.geometry import box, CAP_STYLE, MultiPolygon, Point, Polygon
 from shapely.wkt import loads
 from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.demos.AbstractGeoDataFrameDemos import AbstractGeoDataFrameDemos
@@ -464,14 +465,55 @@
     @staticmethod
     def theChineseCharacterForReach():
         # The Chinese character for "reach" mentioned in (Avis and Toussaint, 1981)
         wkt = 'POLYGON ((62 92, 65 80, 46 77, 33 64, 52 66, 50 73, 66 71, 70 52, 52 56, 45 44, 60 42, 64 35, 42 29, 40 15, 70 18, 80 8, 7 0, 0 9, 25 14, 28 29, 17 28, 14 39, 28 38, 35 53, 17 48, 9 56, 24 64, 31 76, 17 75, 16 84, 62 92))'
         return GeoDataFrame(data=[{'geometry': loads(wkt)}])
 
     @staticmethod
+    def simpleUrbanGraph(choice=1):
+        if (1 == choice):
+            _sio = StringIO("""gid;geometry
+1;LINESTRING(0 0, 0 3, 1 3, 1 2)
+2;LINESTRING(1 3, 3 3, 3 1)
+3;LINESTRING(1 3, 1 2, 2 2, 3 3)
+4;LINESTRING(1 2, 1 1, 3 1, 2 2)
+5;LINESTRING(0 0, 4 0, 4 4, 2 4, 1 3)
+6;LINESTRING(1 3, 1 5, 3 5)
+7;LINESTRING(1 3, 0 4, 1 6, 3 5, 3 6)
+""")
+            return GeoDataFrameLib.read_csv(_sio)
+
+        elif (2 == choice):
+            _sio = StringIO("""gid;geometry
+1;LINESTRING(0 0, 0 3, 1 3)
+2;LINESTRING(0 0, 0 3, 1 3, 1 2)
+3;LINESTRING(0 0, 0 3, 1 3, 1 2, 1 1, 3 1)
+4;LINESTRING(0 0, 0 3, 1 3, 1 2, 2 2)
+5;LINESTRING(0 0, 0 3, 1 3, 3 3)
+6;LINESTRING(0 0, 4 0, 4 4, 2 4)
+7;LINESTRING(0 0, 0 3, 1 3, 1 5, 3 5)
+8;LINESTRING(0 0, 4 0, 4 4, 2 4, 1 3)
+9;LINESTRING(2 2, 3 1, 3 3, 2 2)
+10;LINESTRING(0 0, 0 3, 1 3, 0 4, 1 6, 3 5, 3 6)
+""")
+            return GeoDataFrameLib.read_csv(_sio)
+
+        elif (3 == choice):
+            gdf = GeoDataFrameDemos.simpleUrbanGraph(choice=1)
+            return GeoDataFrame([{"geometry": union_all(gdf.geometry)}])
+
+        elif (4 == choice):
+            gdf = GeoDataFrameDemos.simpleUrbanGraph(choice=3)
+            gdf = gdf.explode(ignore_index=True).reset_index().rename(
+                columns={"index": "gid"})
+            return gdf
+
+        return GeoDataFrameLib.read_csv(_sio)
+
+    @staticmethod
     def plot(sector="Royale2", oFile=None):
         paths, roads, trees, squares = None, None, None, None
 
         if sector == "Royale":
             buildings = GeoDataFrameDemos.districtRoyaleInNantesBuildings()
             paths = GeoDataFrameDemos.districtRoyaleInNantesPaths()
             roads = GeoDataFrameDemos.districtRoyaleInNantesRoads()
```

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos2.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos3.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos5.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos5.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos6.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos6.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos7.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos7.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos8.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos8.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemos9.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos9.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 ;;;;;;;;;Voyage à Nantes;Sentier de découverte;;la Loire à Vélo/la Vélodyssée;;;;;;ITI_AUT_0000002285710202;ROUTNOMM0000000325297519/ROUTNOMM0000000325617764;44109#0RO;44109#0RO;;;;44109;44109;;;;;Non;;;;;;;;;;;;;Restreint aux ayants droit;0;Non;;Double sens;Non;Non;4.0;2.0;9999.0;Pas de Z;3.0;Orthophotographie;;;;;2022-05-13 20:06:25;2014-02-25 17:13:51;En service;0;Non;5;ESP DES TRACEURS DE COQUE;ESP DES TRACEURS DE COQUE;Route à 1 chaussée;TRONROUT0000000332255657;LINESTRING Z (354579.1723472669 6688409 -1000, 354488.2 6688354.8 -1000)
 ;commune;commune;Rue La Tour d'Auvergne;Rue La Tour d'Auvergne;;;44109_4812;44109_4812;;;;;;;;;;;;441094812;441094812;;;;44109;44109;47;42;47;42;Non;;;;;;;;;;;;;Libre;35;Non;;Double sens;Non;Non;4.0;2.0;1.5;Photogrammétrie;2.5;Photogrammétrie;;;2017-07-01;;2022-12-10 14:57:12;2007-07-12 11:22:41;En service;0;Non;5;R LA TOUR D'AUVERGNE;R LA TOUR D'AUVERGNE;Route à 1 chaussée;TRONROUT0000000084093559;LINESTRING Z (354868.6 6688361.8 6.6, 354872.8 6688362.2 6.6, 354896 6688364.087884268 6.977576853526454)
 ;commune;commune;Rue Arthur III;Rue Arthur III;;;44109_0408;44109_0408;;;;;;;;;;;;44109#0EA;44109#0EA;;;;44109;44109;;;;;Non;;;;;;;;;;;;;Libre;35;Non;;Double sens;Non;Non;4.0;2.0;1.5;Photogrammétrie;2.5;Photogrammétrie;;;2017-07-01;;2022-12-10 14:57:12;2016-12-19 12:06:24;En service;0;Non;5;R ARTHUR III;R ARTHUR III;Route à 1 chaussée;TRONROUT0000002000615688;LINESTRING Z (354868.6 6688361.8 6.6, 354864.8 6688397.3 6.8)
 ;;;;;;;;;;;;;;;;;;;;44109#0QW;44109#0QW;;;;44109;44109;;;;;Non;;;;;;;;;;;;;Restreint aux ayants droit;0;Non;;Double sens;Non;Non;5.0;2.0;2.5;Z corrigé;3.0;Orthophotographie;;;;;2017-11-30 19:26:50;2017-06-01 17:22:06;En service;0;Non;5;ALL NIKI DE SAINT-PHALLE;ALL NIKI DE SAINT-PHALLE;Route à 1 chaussée;TRONROUT0000002003976220;LINESTRING Z (354864.8 6688397.3 9.5, 354896 6688400.301749271 9.090670553935745)
 ;commune;commune;Rue Arthur III;Rue Arthur III;;;44109_0408;44109_0408;;;;;;;;;;;;44109#0EA;44109#0EA;;;;44109;44109;5;;9;;Non;;;;;;;;;;;;;Libre;35;Non;;Double sens;Non;Non;4.0;2.0;1.5;Photogrammétrie;2.5;Photogrammétrie;;;2017-07-01;;2022-12-10 14:57:12;2009-09-09 16:24:10;En service;0;Non;5;R ARTHUR III;R ARTHUR III;Route à 1 chaussée;TRONROUT0000000224176726;LINESTRING Z (354864.8 6688397.3 6.8, 354863.79649122804 6688409 6.959649122810142)
 """)
         return GeoDataFrameLib.read_csv(_sio)
-       
+
     @staticmethod
     def prairieAuDucInNantesPath1():
         _sio = StringIO("""geometry
 LINESTRING (354648.14260727953 6688211.714330149, 354647.98951279157 6688211.700557634, 354637.0486024345 6688210.774508305, 354608.84270565317 6688208.035683066, 354607.23398820555 6688207.891409829, 354603.7878139746 6688215.314824239, 354596.12449331133 6688214.60645006, 354582.21460034273 6688213.12530405, 354561.6951105398 6688211.187280567, 354557.2851932434 6688210.806176603, 354535.6419351096 6688309.2769515505, 354535.2429963443 6688309.182155434, 354556.5590431452 6688210.639357932, 354548.6296467959 6688203.631769472, 354531.07009532617 6688201.426221944, 354529.5855921826 6688202.528995708, 354498.11401195574 6688199.51979617, 354469.57980941766 6688198.36201807, 354437.6913605514 6688195.395514355, 354421.1730309755 6688193.736811619, 354415.3960465532 6688193.18902414, 354400.47970195283 6688191.887598102, 354391.73722885555 6688190.755842207, 354384.02804173384 6688188.514798805, 354319.8235337814 6688181.57152045, 354301.9931839867 6688182.598759329, 354272.3427244896 6688180.052884458, 354256.62933774316 6688177.917788565, 354257.7399293631 6688160.703618456, 354274.0732028209 6688162.185869786, 354302.6872480606 6688160.435389245, 354353.66166452534 6688165.808973411, 354361.91342331434 6688168.14458231, 354422.1271878291 6688173.645538298, 354431.51965424535 6688173.712997138, 354490.2935181291 6688179.267759969, 354491.81261139293 6688179.365765986, 354494.1825415612 6688153.873190666, 354505.8896226801 6688154.891197719, 354510.1935504898 6688117.591178974, 354510.5008961229 6688115.365209089, 354536.31791394326 6688117.691902807, 354533.75295199157 6688144.012572044, 354520.33814017085 6688142.567301788, 354516.5292664833 6688180.769991856, 354518.724669209 6688181.053308609, 354573.889699626 6688186.344854437, 354580.85283508507 6688183.947709443, 354612.44760676724 6688186.7815402225, 354622.50627731724 6688195.284220334, 354625.85076048446 6688197.246368688, 354649.16882604925 6688199.280476171, 354668.7956855427 6688201.109139725, 354771.0482473519 6688210.732207292, 354776.2318187611 6688211.299160414, 354779.3095642853 6688210.813200595, 354789.0099146984 6688208.157929713, 354791.71021843486 6688207.897659474, 354796.08260541165 6688208.036073784)
 """)
         return GeoDataFrameLib.read_csv(_sio)
 
@@ -275,15 +275,15 @@
 212;POINT (354510.1935504898 6688117.591178974)
 213;POINT (354518.724669209 6688181.053308609)
 214;POINT (354612.44760676724 6688186.7815402225)
 215;POINT (354649.1688260489 6688199.280476169)
 216;POINT (354796.08260541165 6688208.036073784)
 """)
         return GeoDataFrameLib.read_csv(_sio)
-       
+
     @staticmethod
     def plot(oFile=None):
         roi = GeoDataFrameDemos9.prairieAuDucInNantesRoi()
         buildings = GeoDataFrameDemos9.prairieAuDucInNantesBuildings()
         roads = GeoDataFrameDemos9.prairieAuDucInNantesRoads()
         path1 = GeoDataFrameDemos9.prairieAuDucInNantesPath1()
         waypoints1 = GeoDataFrameDemos9.prairieAuDucInNantesWaypoints1()
```

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosA.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosA.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosB.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosB.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/demos/GeoDataFrameDemosC.py` & `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosC.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 7 juin 2023
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -61,402 +61,403 @@
         return GeoDataFrameLib.read_csv(_sio)
         
     @staticmethod
     def irisTastavinBuildings():
         '''
         # SOURCE:
         # https://geoservices.ign.fr/bdtopo
-        from geopandas import clip
+        from geopandas import clip, read_file
 
         iris = GeoDataFrameDemosC.irisTastavin()
-        buildings = read_file("/home/tleduc/data/bdtopo/BDTOPO_3-0_TOUSTHEMES_SHP_LAMB93_D034_2022-03-15/\
-BDTOPO/1_DONNEES_LIVRAISON_2022-03-00081/BDT_3-0_SHP_LAMB93_D034-ED2022-03-15/BATI/BATIMENT.shp", mask=iris)
+        buildings = read_file("/home/tleduc/data/bdtopo/\
+BDTOPO_3-3_TOUSTHEMES_SHP_LAMB93_D034_2023-09-15/BDTOPO/\
+1_DONNEES_LIVRAISON_2023-09-00196/BDT_3-3_SHP_LAMB93_D034-ED2023-09-15/\
+BATI/BATIMENT.shp", mask=iris)
         buildings = clip(buildings, iris, keep_geom_type=True)
         buildings.to_csv('/tmp/tastavin.csv', sep=';', index=False)
         '''
-        _sio = StringIO("""ID;NATURE;USAGE1;USAGE2;LEGER;ETAT;DATE_CREAT;DATE_MAJ;DATE_APP;DATE_CONF;SOURCE;ID_SOURCE;PREC_PLANI;PREC_ALTI;NB_LOGTS;NB_ETAGES;MAT_MURS;MAT_TOITS;HAUTEUR;Z_MIN_SOL;Z_MIN_TOIT;Z_MAX_TOIT;Z_MAX_SOL;ORIGIN_BAT;APP_FF;geometry
-BATIMENT0000000211120434;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;1.0;0.0;1.0;;;5.9;19.7;25.6;26.2;20.5;Cadastre;C 0.3;POLYGON Z ((770762.1 6277456.6 25.5, 770733 6277467.8 25.5, 770736.3 6277476.4 25.5, 770765.2 6277465 25.5, 770762.1 6277456.6 25.5))
-BATIMENT0000000211120410;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1974-01-01;;;;3.0;2.5;2.0;2.0;49;10;6.6;21.5;28.1;;;Cadastre;A 1.0;POLYGON Z ((770723 6277498.8 28.1, 770719.7 6277490.4 28.1, 770711.5 6277493.7 28.1, 770711.9 6277494.7 28.1, 770704.7 6277497.5 28.1, 770707.7 6277504.9 28.1, 770710.3 6277503.9 28.1, 770723 6277498.8 28.1))
-BATIMENT0000000044598816;Indifférenciée;Annexe;;Non;En service;2006-12-12 11:20:44;2019-04-08 10:00:52;1967-01-01;;;;2.5;1.5;0.0;1.0;00;00;2.4;22.0;;;;Imagerie aérienne;C 0.2;POLYGON Z ((770735.4 6277500.4 24.3, 770734.6 6277498 24.3, 770740.8 6277495.8 24.3, 770739.7 6277492.8 24.3, 770725.8 6277498.1 24.4, 770727.6 6277502.9 24.2, 770735.4 6277500.4 24.3))
-BATIMENT0000000211120356;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;10;10;5.6;21.5;27.1;27.2;;Cadastre;A 1.0;POLYGON Z ((770703.2 6277501.2 27.1, 770699.4 6277502.6 27.1, 770698.1 6277499.4 27.1, 770685.9 6277504 27.1, 770689.2 6277512.1 27.1, 770705.1 6277505.9 27.1, 770703.2 6277501.2 27.1))
-BATIMENT0000000211120375;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;30;10;5.0;22.0;27.0;28.0;;Cadastre;A 1.0;POLYGON Z ((770652.8 6277513 27, 770647 6277506.4 27, 770639.6 6277513.3 27, 770645.4 6277519.8 27, 770652.8 6277513 27))
-BATIMENT0000000211120357;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;;;6.0;21.3;27.3;28.8;;Cadastre;C 0.5;POLYGON Z ((770710.3 6277503.9 27.3, 770707.7 6277504.9 27.3, 770705.1 6277505.9 27.3, 770689.2 6277512.1 27.3, 770693.6 6277523.3 27.3, 770714.7 6277515 27.3, 770710.3 6277503.9 27.3))
-BATIMENT0000002275536127;Indifférenciée;Résidentiel;;Oui;En service;2021-12-17 15:40:19;;;;DGFiP;;5.0;9999.0;;;;;;;;;;Cadastre;;POLYGON Z ((770650.6 6277519.7 -1000, 770642.7 6277526.7 -1000, 770643.7 6277527.7 -1000, 770645.6 6277526.1 -1000, 770646.9 6277527.5 -1000, 770652.7 6277521.9 -1000, 770650.6 6277519.7 -1000))
-BATIMENT0000000211120432;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1987-01-01;;;;3.0;2.5;1.0;1.0;;;6.5;21.0;27.5;;;Cadastre;A 1.0;POLYGON Z ((770717.9 6277528.5 27.5, 770714.7 6277520 27.5, 770698.7 6277525.8 27.5, 770697.4 6277528.8 27.5, 770700 6277535.5 27.5, 770717.9 6277528.5 27.5))
-BATIMENT0000000211120368;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;3.0;2.5;1.0;2.0;20;10;6.5;21.2;27.7;;;Cadastre;A 1.0;POLYGON Z ((770656.2 6277522.9 27.7, 770655.2 6277523.9 27.7, 770653.1 6277521.7 27.7, 770652.7 6277521.9 27.7, 770646.9 6277527.5 27.7, 770652.6 6277533.8 27.7, 770660.1 6277527 27.7, 770656.2 6277522.9 27.7))
-BATIMENT0000000211120367;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;3.0;2.5;1.0;2.0;50;10;6.4;21.3;27.7;28.0;;Cadastre;A 1.0;POLYGON Z ((770664.9 6277534.6 27.7, 770662.9 6277532.4 27.7, 770664.1 6277531.3 27.7, 770660.1 6277527 27.7, 770652.6 6277533.8 27.7, 770658.6 6277540.4 27.7, 770664.9 6277534.6 27.7))
-BATIMENT0000000211120374;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;40;10;4.9;22.0;26.9;28.0;;Cadastre;C 0.7;POLYGON Z ((770647 6277506.4 26.9, 770643.4 6277502.4 26.9, 770642.2 6277503.3 26.9, 770640.3 6277501.2 26.9, 770633.9 6277507.1 26.9, 770639.6 6277513.3 26.9, 770647 6277506.4 26.9))
-BATIMENT0000000211120387;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;45;10;5.2;21.4;26.6;28.2;21.4;Cadastre;A 1.0;POLYGON Z ((770623.3 6277526.5 26.6, 770629.9 6277520.6 26.6, 770624.5 6277514.3 26.6, 770622.1 6277516.5 26.6, 770621.2 6277515.5 26.6, 770616.9 6277519.3 26.6, 770623.3 6277526.5 26.6))
-BATIMENT0000000211120386;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;34;10;6.2;20.5;26.7;28.4;20.7;Cadastre;A 1.0;POLYGON Z ((770623.3 6277526.5 26.7, 770616.9 6277519.3 26.7, 770612.7 6277523.1 26.7, 770613.6 6277524.1 26.7, 770611.5 6277526.1 26.7, 770616.8 6277532.3 26.7, 770623.3 6277526.5 26.7))
-BATIMENT0000000211120385;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.0;20.7;26.7;28.4;20.7;Cadastre;A 1.0;POLYGON Z ((770616.8 6277532.3 26.7, 770611.5 6277526.1 26.7, 770609.1 6277528.2 26.7, 770608.2 6277527.2 26.7, 770603.8 6277531 26.7, 770610.1 6277538.2 26.7, 770611.8 6277540.1 26.7, 770615.6 6277536.7 26.7, 770613.9 6277534.9 26.7, 770616.8 6277532.3 26.7))
-BATIMENT0000000211120384;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;46;10;6.0;20.7;26.7;28.2;20.7;Cadastre;A 1.0;POLYGON Z ((770612.5 6277540.9 26.7, 770611.8 6277540.1 26.7, 770610.1 6277538.2 26.7, 770603.8 6277531 26.7, 770599.5 6277535 26.7, 770600.5 6277536 26.7, 770598.4 6277537.9 26.7, 770603.8 6277544 26.7, 770606.1 6277546.6 26.7, 770612.5 6277540.9 26.7))
-BATIMENT0000000211120383;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.4;20.6;Cadastre;A 1.0;POLYGON Z ((770597.3 6277549.7 26.7, 770603.8 6277544 26.7, 770598.4 6277537.9 26.7, 770596.1 6277539.9 26.7, 770595.1 6277538.9 26.7, 770591.1 6277542.6 26.7, 770597.3 6277549.7 26.7))
-BATIMENT0000000211120382;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.3;20.6;Cadastre;A 1.0;POLYGON Z ((770597.3 6277549.7 26.7, 770591.1 6277542.6 26.7, 770586.6 6277546.6 26.7, 770587.5 6277547.5 26.7, 770585.2 6277549.5 26.7, 770590.6 6277555.7 26.7, 770597.3 6277549.7 26.7))
-BATIMENT0000000211120286;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;3.2;20.3;23.5;24.2;20.3;Cadastre;;POLYGON Z ((770622.4 6277554.7 23.4, 770624.6 6277557.2 23.4, 770626.2 6277555.9 23.4, 770627.5 6277554.8 23.4, 770625.2 6277552.2 23.4, 770623.6 6277553.7 23.4, 770622.4 6277554.7 23.4))
-BATIMENT0000000211120288;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.2;20.2;27.4;28.4;20.3;Cadastre;C 0.2;POLYGON Z ((770640.5 6277554.6 27.4, 770634.6 6277548.2 27.4, 770628.4 6277554.1 27.4, 770630.4 6277556.3 27.4, 770629.2 6277557.4 27.4, 770633 6277561.5 27.4, 770640.5 6277554.6 27.4))
-BATIMENT0000000211120381;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.6;20.7;Cadastre;A 1.0;POLYGON Z ((770585.2 6277549.5 26.7, 770582.9 6277551.6 26.7, 770582.1 6277550.6 26.7, 770578 6277554.2 26.7, 770584.2 6277561.4 26.7, 770590.6 6277555.7 26.7, 770585.2 6277549.5 26.7))
-BATIMENT0000000211120433;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;1.0;2.0;;;7.2;21.0;28.2;;;Cadastre;A 1.0;POLYGON Z ((770724.2 6277535.1 28.2, 770722.6 6277531 28.2, 770725.3 6277530 28.2, 770724 6277526.1 28.2, 770717.9 6277528.5 28.2, 770700 6277535.5 28.2, 770702.4 6277541.6 28.2, 770705.2 6277543.2 28.2, 770721.1 6277536.8 28.2, 770720.9 6277536.3 28.2, 770724.2 6277535.1 28.2))
-BATIMENT0000000211120366;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;6.4;21.3;27.7;27.8;;Cadastre;A 1.0;POLYGON Z ((770672 6277540.1 27.7, 770668.2 6277535.9 27.7, 770667 6277536.8 27.7, 770664.9 6277534.6 27.7, 770658.6 6277540.4 27.7, 770664.6 6277546.9 27.7, 770672 6277540.1 27.7))
-BATIMENT0000000211120365;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;3.0;2.5;1.0;2.0;50;10;6.4;21.3;27.7;27.8;;Cadastre;A 1.0;POLYGON Z ((770670.7 6277553.5 27.7, 770676.9 6277547.8 27.7, 770674.8 6277545.3 27.7, 770675.9 6277544.4 27.7, 770672 6277540.1 27.7, 770664.6 6277546.9 27.7, 770670.7 6277553.5 27.7))
-BATIMENT0000000211120412;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1981-01-01;;;;3.0;2.5;1.0;1.0;50;10;3.9;21.3;25.2;;;Cadastre;B 0.4;POLYGON Z ((770748.6 6277552.3 25.2, 770748.8 6277553.8 25.2, 770753.7 6277553.1 25.2, 770752.9 6277547.8 25.2, 770754.1 6277547.6 25.2, 770753 6277539.6 25.2, 770748.7 6277540.2 25.2, 770749.1 6277543.4 25.2, 770737.7 6277544.9 25.2, 770739.1 6277554.9 25.2, 770742.8 6277554.4 25.2, 770742.6 6277553.1 25.2, 770746.3 6277552.6 25.2, 770746.2 6277551.6 25.2, 770748.4 6277551.3 25.2, 770748.6 6277552.3 25.2))
-BATIMENT0000000211120414;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;5.2;20.1;25.3;27.2;20.2;Cadastre;;POLYGON Z ((770709.4 6277547.2 25.2, 770710.3 6277549.5 25.2, 770714.7 6277547.9 25.2, 770713.7 6277545.6 25.2, 770709.4 6277547.2 25.2))
-BATIMENT0000000211120395;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.8;20.2;23.0;23.4;20.2;Cadastre;;POLYGON Z ((770654.8 6277548.6 23, 770652.8 6277546.5 23, 770650.7 6277548.5 23, 770652.6 6277550.5 23, 770654.8 6277548.6 23))
-BATIMENT0000000211120411;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;3.0;2.5;;;;;4.1;21.3;25.4;;;Cadastre;;POLYGON Z ((770748.4 6277551.3 25.4, 770746.2 6277551.6 25.4, 770746.3 6277552.6 25.4, 770748.6 6277552.3 25.4, 770748.4 6277551.3 25.4))
-BATIMENT0000000211120396;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.3;20.2;22.5;22.6;20.2;Cadastre;;POLYGON Z ((770653.4 6277553.2 22.4, 770651.6 6277551.3 22.4, 770650.1 6277552.8 22.4, 770651.8 6277554.6 22.4, 770653.4 6277553.2 22.4))
-BATIMENT0000000211120415;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1900-01-01;;;;3.0;2.5;1.0;2.0;20;10;6.2;21.0;27.2;28.0;21.0;Cadastre;B 0.6;POLYGON Z ((770707.1 6277550.9 27.2, 770710.6 6277559.5 27.2, 770718.1 6277556.7 27.2, 770714.7 6277547.9 27.2, 770710.3 6277549.5 27.2, 770707.1 6277550.9 27.2))
-BATIMENT0000000211120394;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.3;20.2;22.5;23.0;20.2;Cadastre;;POLYGON Z ((770656.5 6277560.1 22.5, 770654 6277557.4 22.5, 770651.6 6277559.5 22.5, 770654.1 6277562.3 22.5, 770656.5 6277560.1 22.5))
-BATIMENT0000000211120287;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;3.0;2.5;;;;;4.4;21.0;25.4;27.0;21.0;Cadastre;;POLYGON Z ((770633 6277561.5 25.4, 770629.2 6277557.4 25.4, 770630.4 6277556.3 25.4, 770628.4 6277554.1 25.4, 770627.5 6277554.8 25.4, 770626.2 6277555.9 25.4, 770632.2 6277562.3 25.4, 770633 6277561.5 25.4))
-BATIMENT0000000211120289;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;4.5;21.1;25.6;28.2;21.1;Cadastre;C 0.6;POLYGON Z ((770636.9 6277565.6 25.6, 770638 6277564.7 25.6, 770640 6277566.9 25.6, 770646.4 6277561 25.6, 770640.5 6277554.6 25.6, 770633 6277561.5 25.6, 770636.9 6277565.6 25.6))
-BATIMENT0000000211120380;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.7;20.7;Cadastre;A 1.0;POLYGON Z ((770578 6277554.2 26.7, 770573.3 6277558.3 26.7, 770574.2 6277559.3 26.7, 770572 6277561.3 26.7, 770577.5 6277567.4 26.7, 770584.2 6277561.4 26.7, 770578 6277554.2 26.7))
-BATIMENT0000000211120378;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.8;21.0;26.8;28.7;21.0;Cadastre;A 1.0;POLYGON Z ((770570.9 6277573.4 26.8, 770577.5 6277567.4 26.8, 770572 6277561.3 26.8, 770569.8 6277563.3 26.8, 770569 6277562.4 26.8, 770564.7 6277566.3 26.8, 770570.9 6277573.4 26.8))
-BATIMENT0000000211120301;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.2;20.4;Cadastre;C 1.0;POLYGON Z ((770612.4 6277574.2 27.5, 770611.2 6277575.2 27.5, 770609.3 6277573.2 27.5, 770603.2 6277578.8 27.5, 770608.7 6277584.7 27.5, 770616 6277578 27.5, 770612.4 6277574.2 27.5))
-BATIMENT0000000211120299;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.5;20.4;Cadastre;C 1.0;POLYGON Z ((770620.9 6277585.7 27.5, 770618.9 6277583.4 27.5, 770620.1 6277582.3 27.5, 770616 6277578 27.5, 770608.7 6277584.7 27.5, 770614.9 6277591.3 27.5, 770620.9 6277585.7 27.5))
-BATIMENT0000000211120297;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.4;20.4;Cadastre;C 1.0;POLYGON Z ((770620.9 6277597.7 27.4, 770628.2 6277591.1 27.4, 770624.2 6277587 27.4, 770623 6277587.9 27.4, 770620.9 6277585.7 27.4, 770614.9 6277591.3 27.4, 770620.9 6277597.7 27.4))
-BATIMENT0000000211120390;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;6.7;20.6;27.3;29.5;20.7;Cadastre;;POLYGON Z ((770585.2 6277592 27.2, 770582.7 6277589.2 27.2, 770580.3 6277591.5 27.2, 770582.8 6277594.2 27.2, 770585.2 6277592 27.2))
-BATIMENT0000000211120393;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;1.9;20.4;22.3;23.0;20.4;Cadastre;;POLYGON Z ((770609.2 6277593.8 22.2, 770607.1 6277591.6 22.2, 770605.5 6277593.1 22.2, 770607.8 6277595.4 22.2, 770609.2 6277593.8 22.2))
-BATIMENT0000000211120391;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;4.4;20.6;25.0;27.3;20.7;Cadastre;;POLYGON Z ((770582 6277595.1 25, 770579.7 6277592.7 25, 770577.6 6277594.6 25, 770579.8 6277597.2 25, 770582 6277595.1 25))
-BATIMENT0000000211120295;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1961-01-01;;;;3.0;2.5;1.0;2.0;30;10;5.9;21.0;26.9;27.8;21.0;Cadastre;A 1.0;POLYGON Z ((770681.1 6277565.3 26.9, 770682.6 6277563.9 26.9, 770678.5 6277559.6 26.9, 770677.5 6277560.6 26.9, 770675.1 6277558.2 26.9, 770673.6 6277559.6 26.9, 770667.3 6277565.7 26.9, 770673.7 6277572.3 26.9, 770681.1 6277565.3 26.9))
-BATIMENT0000000211120290;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;4.7;21.0;25.7;28.1;21.0;Cadastre;C 0.7;POLYGON Z ((770654 6277565.4 25.7, 770648.4 6277559.2 25.7, 770646.4 6277561 25.7, 770640 6277566.9 25.7, 770642.1 6277569.2 25.7, 770641 6277570.1 25.7, 770644.6 6277574 25.7, 770652 6277567.2 25.7, 770654 6277565.4 25.7))
-BATIMENT0000000211120294;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;30;10;5.9;21.0;26.9;27.8;21.0;Cadastre;A 1.0;POLYGON Z ((770680.1 6277578.8 26.9, 770686.2 6277572.8 26.9, 770684.3 6277570.8 26.9, 770685.3 6277569.8 26.9, 770681.1 6277565.3 26.9, 770673.7 6277572.3 26.9, 770680.1 6277578.8 26.9))
-BATIMENT0000000211120291;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;5.2;21.0;26.2;28.2;21.0;Cadastre;C 0.2;POLYGON Z ((770648.6 6277578.5 26.2, 770649.9 6277577.5 26.2, 770651.8 6277579.6 26.2, 770655.2 6277576.5 26.2, 770658.1 6277573.9 26.2, 770652 6277567.2 26.2, 770644.6 6277574 26.2, 770648.6 6277578.5 26.2))
-BATIMENT0000002000330691;Indifférenciée;Résidentiel;Annexe;Non;En service;2016-11-10 15:17:04;2019-04-08 10:00:52;2014-01-01;2015-07-01;;;2.5;1.5;34.0;6.0;00;00;19.1;18.9;;;;Imagerie aérienne;A 1.0;POLYGON Z ((770724 6277585.2 37.1, 770733.8 6277585.2 37.1, 770733.7 6277587.5 34.8, 770737.9 6277587.5 34.8, 770737.7 6277585.2 38, 770737.7 6277583.6 38, 770742.6 6277583.4 38, 770742.6 6277585.3 38, 770744.4 6277585.3 38, 770744.4 6277587.4 36.9, 770756.4 6277587.3 36.9, 770756.3 6277585.2 37.9, 770756.2 6277569.6 37.9, 770756 6277567.4 36.4, 770740.3 6277567.3 36.4, 770740.3 6277569.3 37.2, 770723.8 6277569.3 37, 770724 6277585.2 37.1))
-BATIMENT0000000211120292;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;5.4;21.0;26.4;28.2;21.0;Cadastre;C 0.6;POLYGON Z ((770661.2 6277582.9 26.4, 770655.2 6277576.5 26.4, 770651.8 6277579.6 26.4, 770649 6277582.3 26.4, 770651.2 6277584.4 26.4, 770650.1 6277585.3 26.4, 770654 6277589.6 26.4, 770661.2 6277582.9 26.4))
-BATIMENT0000000211120293;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;4.9;21.0;25.9;28.2;21.0;Cadastre;C 0.5;POLYGON Z ((770658 6277594 25.9, 770659 6277593 25.9, 770661.1 6277595.2 25.9, 770667.2 6277589.4 25.9, 770661.2 6277582.9 25.9, 770654 6277589.6 25.9, 770658 6277594 25.9))
-BATIMENT0000000211120420;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;25.0;4.0;34;49;13.8;21.0;34.8;;;Cadastre;A 1.0;POLYGON Z ((770762 6277609.6 34.8, 770733.3 6277609.5 34.8, 770733.4 6277621.6 34.8, 770762 6277621.7 34.8, 770762 6277609.6 34.8))
-BATIMENT0000000211120284;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;58.0;6.0;00;00;19.0;21.2;40.2;41.9;21.5;Cadastre;A 1.0;POLYGON Z ((770620 6277667.2 40.2, 770624.7 6277663 40.2, 770625.3 6277663.6 40.2, 770630.7 6277658.7 40.2, 770630.2 6277658.1 40.2, 770640.1 6277649 40.2, 770640.7 6277649.6 40.2, 770646 6277644.6 40.2, 770645.5 6277644 40.2, 770654.8 6277635.2 40.2, 770655.4 6277635.8 40.2, 770660.6 6277631 40.2, 770660.2 6277630.4 40.2, 770669.7 6277621.6 40.2, 770670.2 6277622.1 40.2, 770675.7 6277617.3 40.2, 770675.3 6277616.6 40.2, 770684.7 6277607.8 40.2, 770685.4 6277608.4 40.2, 770690.4 6277603.7 40.2, 770689.9 6277602.9 40.2, 770694.6 6277598.6 40.2, 770688.6 6277592.2 40.2, 770614.1 6277660.7 40.2, 770620 6277667.2 40.2))
-BATIMENT0000000211120419;Indifférenciée;Indifférencié;;Non;En construction;2008-11-18 15:28:19;2020-11-10 17:38:02;1870-01-01;2018-07-08;;;2.5;1.5;1.0;2.0;;;5.9;22.9;;30.9;22.2;Imagerie aérienne;A 1.0;POLYGON Z ((770758.5 6277675.4 28.8, 770760.9 6277679.7 28.8, 770766.3 6277676.8 28.8, 770767.5 6277672.6 28.8, 770766.6 6277655.1 28.8, 770756.6 6277640.1 28.8, 770751.1 6277643.5 28.8, 770745 6277643.6 28.8, 770739.3 6277646.8 28.8, 770756.1 6277676.6 28.8, 770758.5 6277675.4 28.8))
-BATIMENT0000000211120296;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;34;10;7.2;20.3;27.5;28.4;20.4;Cadastre;C 1.0;POLYGON Z ((770633.2 6277598.8 27.4, 770630.8 6277596.3 27.4, 770632 6277595.2 27.4, 770628.2 6277591.1 27.4, 770620.9 6277597.7 27.4, 770627.1 6277604.3 27.4, 770633.2 6277598.8 27.4))
-BATIMENT0000000211120298;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;1.0;1.0;2.0;24;10;7.3;20.3;27.6;28.4;20.5;Cadastre;C 1.0;POLYGON Z ((770640.3 6277604 27.5, 770636.2 6277599.7 27.5, 770635 6277600.8 27.5, 770633.2 6277598.8 27.5, 770627.1 6277604.3 27.5, 770633.1 6277610.6 27.5, 770640.3 6277604 27.5))
-BATIMENT0000000211120300;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.0;20.4;27.4;28.2;20.6;Cadastre;C 0.7;POLYGON Z ((770638.5 6277616.4 27.4, 770644.3 6277611 27.4, 770642.2 6277608.6 27.4, 770643.5 6277607.4 27.4, 770640.3 6277604 27.4, 770633.1 6277610.6 27.4, 770638.5 6277616.4 27.4))
-BATIMENT0000000211120334;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;1.0;1.0;2.0;50;10;6.9;20.6;27.5;28.2;20.7;Cadastre;C 1.0;POLYGON Z ((770626.1 6277623.5 27.4, 770625.5 6277622.5 27.4, 770627.3 6277620.8 27.4, 770621.6 6277614.5 27.4, 770615.1 6277620.6 27.4, 770621.7 6277627.6 27.4, 770626.1 6277623.5 27.4))
-BATIMENT0000000211120333;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;4.4;21.4;25.8;28.2;21.4;Cadastre;C 0.8;POLYGON Z ((770615.1 6277620.6 25.8, 770608.5 6277626.7 25.8, 770614.2 6277632.7 25.8, 770616.4 6277630.7 25.8, 770617.2 6277631.7 25.8, 770621.7 6277627.6 25.8, 770615.1 6277620.6 25.8))
-BATIMENT0000000211120331;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;50;10;7.0;20.7;27.7;28.7;20.9;Cadastre;C 0.4;POLYGON Z ((770608.5 6277626.7 27.7, 770606.6 6277628.5 27.7, 770604.7 6277630.3 27.7, 770602 6277632.8 27.7, 770608.5 6277639.8 27.7, 770612.5 6277636 27.7, 770611.8 6277635.1 27.7, 770614.2 6277632.7 27.7, 770608.5 6277626.7 27.7))
-BATIMENT0000000211120332;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;50;10;4.8;21.4;26.2;28.5;21.4;Cadastre;C 0.2;POLYGON Z ((770595.8 6277638.6 26.2, 770601.5 6277644.6 26.2, 770603.3 6277642.8 26.2, 770604.4 6277643.7 26.2, 770608.5 6277639.8 26.2, 770602 6277632.8 26.2, 770595.8 6277638.6 26.2))
-BATIMENT0000000211120326;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;3.3;21.0;24.3;27.3;21.3;Cadastre;;POLYGON Z ((770592.1 6277643.7 24.2, 770597.6 6277649.8 24.2, 770600.1 6277647.5 24.2, 770594.5 6277641.6 24.2, 770592.1 6277643.7 24.2))
-BATIMENT0000000211120324;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.6;21.4;28.0;29.0;21.5;Cadastre;A 1.0;POLYGON Z ((770598.5 6277650.7 28, 770597.6 6277649.8 28, 770592.1 6277643.7 28, 770590.6 6277641.8 28, 770584 6277648 28, 770585.6 6277649.7 28, 770592.1 6277656.7 28, 770598.5 6277650.7 28))
-BATIMENT0000000211120320;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;4.2;21.3;25.5;26.8;21.4;Cadastre;;POLYGON Z ((770581.6 6277653.4 25.5, 770579.8 6277651.4 25.5, 770577.4 6277653.8 25.5, 770579.2 6277655.7 25.5, 770581.6 6277653.4 25.5))
-BATIMENT0000000211120319;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;20.0;5.0;40;40;17.2;21.8;39.0;;;Cadastre;C 0.4;POLYGON Z ((770645.8 6277685 39, 770648 6277687.2 39, 770654.7 6277680.8 39, 770655.1 6277681.2 39, 770657.6 6277678.9 39, 770657.3 6277678.3 39, 770670.9 6277665.4 39, 770671.4 6277665.8 39, 770673.9 6277663.6 39, 770673.5 6277663.1 39, 770687.1 6277650.1 39, 770687.6 6277650.7 39, 770689.8 6277648.5 39, 770689.4 6277648 39, 770696.5 6277641.4 39, 770700 6277645 39, 770699.5 6277645.5 39, 770701.8 6277647.7 39, 770702.4 6277647.2 39, 770706.3 6277651.4 39, 770712.6 6277645.4 39, 770701.3 6277633.4 39, 770694.9 6277639.4 39, 770690.6 6277634.9 39, 770639.8 6277682.8 39, 770643.8 6277687 39, 770645.8 6277685 39))
-BATIMENT0000000211120336;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;0.0;1.0;00;00;1.9;21.9;23.8;;;Cadastre;C 0.4;POLYGON Z ((770709.8 6277671.6 23.8, 770696.6 6277657.7 23.8, 770644.3 6277707.9 23.8, 770657 6277721.8 23.8, 770709.8 6277671.6 23.8))
-BATIMENT0000000211120317;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;20.0;5.0;40;40;17.2;22.4;39.6;39.6;23.2;Cadastre;C 0.7;POLYGON Z ((770624 6277706.9 39.6, 770623.6 6277707.4 39.6, 770625.6 6277709.4 39.6, 770626 6277708.9 39.6, 770635.7 6277719.4 39.6, 770635.2 6277719.8 39.6, 770637.1 6277721.8 39.6, 770637.6 6277721.3 39.6, 770647.5 6277731.8 39.6, 770647 6277732.3 39.6, 770648.7 6277733.9 39.6, 770649 6277733.5 39.6, 770654.4 6277739.1 39.6, 770661.3 6277732.5 39.6, 770667 6277738.5 39.6, 770672.1 6277733.7 39.6, 770672.7 6277734.4 39.6, 770674.4 6277732.7 39.6, 770673.9 6277732.2 39.6, 770684.6 6277722.1 39.6, 770685.1 6277722.6 39.6, 770686.9 6277721 39.6, 770686.5 6277720.3 39.6, 770697 6277710.4 39.6, 770697.5 6277711 39.6, 770699.7 6277709 39.6, 770699.2 6277708.4 39.6, 770704.6 6277703.3 39.6, 770698.2 6277696.7 39.6, 770661 6277731.9 39.6, 770626.5 6277695.1 39.6, 770619.4 6277701.7 39.6, 770624 6277706.9 39.6))
-BATIMENT0000000211120339;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.4;22.0;Cadastre;A 1.0;POLYGON Z ((770542.7 6277676.8 29.3, 770548.4 6277683.2 29.3, 770550.6 6277681.2 29.3, 770551.7 6277682.2 29.3, 770556.1 6277678.1 29.3, 770549.3 6277670.6 29.3, 770542.7 6277676.8 29.3))
-BATIMENT0000000211120338;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;10;10;7.3;22.0;29.3;29.7;22.0;Cadastre;B 0.6;POLYGON Z ((770539.8 6277679.5 29.3, 770536.4 6277682.7 29.3, 770543.2 6277690.1 29.3, 770547.1 6277686.4 29.3, 770546.1 6277685.2 29.3, 770548.4 6277683.2 29.3, 770542.7 6277676.8 29.3, 770539.8 6277679.5 29.3))
-BATIMENT0000000211120340;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.9;22.1;Cadastre;A 1.0;POLYGON Z ((770536.4 6277682.7 29.3, 770530 6277688.6 29.3, 770535.7 6277694.9 29.3, 770537.9 6277692.9 29.3, 770539 6277694 29.3, 770543.2 6277690.1 29.3, 770536.4 6277682.7 29.3))
-BATIMENT0000000211120342;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.8;22.3;Cadastre;A 1.0;POLYGON Z ((770534.2 6277698 29.3, 770533.4 6277697 29.3, 770535.7 6277694.9 29.3, 770530 6277688.6 29.3, 770523.3 6277694.8 29.3, 770530 6277702.1 29.3, 770534.2 6277698 29.3))
-BATIMENT0000000211120344;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;1.0;0.0;1.0;;;2.1;22.0;24.1;25.3;22.2;Cadastre;A 0.2;POLYGON Z ((770517.6 6277698.8 24, 770515.3 6277696.4 24, 770515.8 6277696.1 24, 770514.5 6277694.9 24, 770512.9 6277696.5 24, 770516.2 6277700.1 24, 770517.6 6277698.8 24))
-BATIMENT0000000211120343;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;34;10;7.2;22.0;29.2;29.9;22.5;Cadastre;A 0.5;POLYGON Z ((770522.4 6277707 29.2, 770524.8 6277705 29.2, 770525.8 6277706 29.2, 770530 6277702.1 29.2, 770523.3 6277694.8 29.2, 770516.8 6277700.8 29.2, 770521.4 6277706 29.2, 770522.4 6277707 29.2))
-BATIMENT0000000211120401;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1970-01-01;;;;5.0;1.0;0.0;1.0;;;7.3;22.0;29.3;34.3;22.2;Cadastre;C 0.2;POLYGON Z ((770571.2 6277707.7 29.2, 770568.3 6277704.4 29.2, 770564.9 6277707.7 29.2, 770567.8 6277710.8 29.2, 770571.2 6277707.7 29.2))
-BATIMENT0000000211120348;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.9;23.1;29.0;30.4;23.1;Cadastre;A 1.0;POLYGON Z ((770515 6277728.7 29, 770521.2 6277723.1 29, 770519.1 6277720.9 29, 770520.3 6277719.6 29, 770516.5 6277715.5 29, 770509.2 6277722.3 29, 770515 6277728.7 29))
-BATIMENT0000000211120347;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;34;10;5.8;23.3;29.1;30.5;23.3;Cadastre;A 1.0;POLYGON Z ((770528.5 6277728.5 29.1, 770524.4 6277724.1 29.1, 770523.2 6277725.3 29.1, 770521.2 6277723.1 29.1, 770515 6277728.7 29.1, 770521.1 6277735.3 29.1, 770528.5 6277728.5 29.1))
-BATIMENT0000000211120345;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;5.5;22.5;28.0;28.9;22.6;Cadastre;;POLYGON Z ((770521.1 6277735.3 28, 770515 6277728.7 28, 770513.7 6277730 28, 770519.6 6277736.6 28, 770521.1 6277735.3 28))
-BATIMENT0000000211120322;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;45;10;6.6;21.4;28.0;28.9;21.5;Cadastre;A 1.0;POLYGON Z ((770581.6 6277653.4 28, 770579.2 6277655.7 28, 770584.7 6277661.8 28, 770586.9 6277659.7 28, 770587.9 6277660.7 28, 770592.1 6277656.8 28, 770592.1 6277656.7 28, 770585.6 6277649.7 28, 770581.6 6277653.4 28))
-BATIMENT0000000211120321;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.5;21.4;27.9;28.9;21.5;Cadastre;A 1.0;POLYGON Z ((770572.7 6277661.7 27.9, 770579.1 6277668.7 27.9, 770583.6 6277664.6 27.9, 770582.7 6277663.6 27.9, 770584.7 6277661.8 27.9, 770579.2 6277655.7 27.9, 770572.7 6277661.7 27.9))
-BATIMENT0000000211120323;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.5;21.4;27.9;29.0;21.6;Cadastre;A 0.9;POLYGON Z ((770572.7 6277661.7 27.9, 770566.1 6277667.9 27.9, 770571.6 6277673.9 27.9, 770573.9 6277671.8 27.9, 770574.7 6277672.7 27.9, 770579.1 6277668.7 27.9, 770572.7 6277661.7 27.9))
-BATIMENT0000000211120325;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;0.0;2.0;40;10;6.3;21.4;27.7;;;Cadastre;A 0.9;POLYGON Z ((770574.7 6277672.7 27.7, 770573.9 6277671.8 27.7, 770571.6 6277673.9 27.7, 770572.4 6277674.8 27.7, 770574.7 6277672.7 27.7))
-BATIMENT0000000211120285;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;40.0;10.0;00;00;23.2;21.0;44.2;53.3;23.2;Cadastre;C 0.5;POLYGON Z ((770605.2 6277736.1 44.2, 770600.6 6277731.3 44.2, 770601.5 6277730.6 44.2, 770596.9 6277725.8 44.2, 770596.1 6277726.4 44.2, 770586 6277715.9 44.2, 770586.8 6277715.1 44.2, 770582.6 6277710.7 44.2, 770581.8 6277711.3 44.2, 770577 6277706.4 44.2, 770580.2 6277703.5 44.2, 770580.8 6277703.9 44.2, 770585.8 6277699.3 44.2, 770585.4 6277698.7 44.2, 770589.9 6277694.5 44.2, 770590.2 6277694.8 44.2, 770595.2 6277690.1 44.2, 770595.9 6277690.6 44.2, 770600.7 6277686.1 44.2, 770600.2 6277685.6 44.2, 770609.8 6277676.6 44.2, 770610.5 6277677.2 44.2, 770615.6 6277672.6 44.2, 770614.8 6277671.9 44.2, 770620 6277667.2 44.2, 770614.1 6277660.7 44.2, 770569.7 6277701.5 44.2, 770575.6 6277707.9 44.2, 770570.1 6277713.2 44.2, 770598.2 6277742.7 44.2, 770605.2 6277736.1 44.2))
-BATIMENT0000000211120282;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;53.0;7.0;10;10;22.3;24.7;47.0;;;Cadastre;C 0.6;POLYGON Z ((770541.6 6277843.5 47, 770547.4 6277849.5 47, 770576.8 6277822.1 47, 770575.2 6277820.3 47, 770616.8 6277781.2 47, 770616.2 6277780.3 47, 770617.3 6277779.2 47, 770616.1 6277777.8 47, 770614.7 6277778.9 47, 770612.2 6277776.2 47, 770637.1 6277753.1 47, 770628.9 6277744.2 47, 770603.9 6277767.3 47, 770608.9 6277772.7 47, 770567.1 6277811.9 47, 770568.7 6277813.7 47, 770539.5 6277841.2 47, 770533.7 6277835.3 47, 770513.2 6277855 47, 770520.9 6277863.2 47, 770541.6 6277843.5 47))
-BATIMENT0000000211120346;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;2.5;1.0;2.0;34;10;5.8;23.3;29.1;30.3;23.3;Cadastre;A 1.0;POLYGON Z ((770527.1 6277741.9 29.1, 770533.3 6277736.2 29.1, 770531.5 6277734.2 29.1, 770532.6 6277733 29.1, 770528.5 6277728.5 29.1, 770521.1 6277735.3 29.1, 770527.1 6277741.9 29.1))
-BATIMENT0000000211120349;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.1;23.1;29.2;30.4;23.1;Cadastre;A 1.0;POLYGON Z ((770540.8 6277741.9 29.2, 770536.5 6277737.2 29.2, 770535.2 6277738.3 29.2, 770533.3 6277736.2 29.2, 770527.1 6277741.9 29.2, 770533.3 6277748.6 29.2, 770540.8 6277741.9 29.2))
-BATIMENT0000000211120351;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;34;10;6.3;23.0;29.3;30.4;23.0;Cadastre;A 1.0;POLYGON Z ((770546.6 6277748.2 29.3, 770544.3 6277745.7 29.3, 770540.8 6277741.9 29.3, 770533.3 6277748.6 29.3, 770532.1 6277749.8 29.3, 770537.9 6277756.2 29.3, 770546.6 6277748.2 29.3))
-BATIMENT0000000211120327;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1975-01-01;;;;3.0;2.5;23.0;6.0;50;10;17.9;24.0;41.9;;;Cadastre;C 0.9;POLYGON Z ((770579.2 6277769.6 41.9, 770563.8 6277753.8 41.9, 770555.2 6277762 41.9, 770554.1 6277760.7 41.9, 770554.6 6277760.3 41.9, 770552.6 6277758.1 41.9, 770544.9 6277765.6 41.9, 770548 6277768.7 41.9, 770551 6277765.8 41.9, 770566.6 6277781.7 41.9, 770579.2 6277769.6 41.9))
-BATIMENT0000000211120318;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1975-01-01;;;;3.0;2.5;23.0;6.0;50;10;16.7;25.2;41.9;;;Cadastre;C 0.6;POLYGON Z ((770546.9 6277800.2 41.9, 770531.8 6277784.4 41.9, 770519.2 6277796.4 41.9, 770534.5 6277812.3 41.9, 770546.9 6277800.2 41.9))
-BATIMENT0000000211120515;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1972-01-01;;;;3.0;1.0;0.0;7.0;;;7.5;25.8;33.3;43.5;26.1;Cadastre;C 0.2;POLYGON Z ((770519.7 6277863.6 33.2, 770515.9 6277859.6 33.2, 770513.8 6277861.7 33.2, 770517.5 6277865.6 33.2, 770519.7 6277863.6 33.2))
-BATIMENT0000000211120376;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;43;14;5.7;21.2;26.9;28.7;21.2;Cadastre;A 1.0;POLYGON Z ((770560.1 6277570.4 26.9, 770560.9 6277571.3 26.9, 770558.9 6277573.2 26.9, 770564.3 6277579.3 26.9, 770570.9 6277573.4 26.9, 770564.7 6277566.3 26.9, 770560.1 6277570.4 26.9))
-BATIMENT0000000211120377;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.5;21.5;27.0;28.7;21.5;Cadastre;A 1.0;POLYGON Z ((770557.6 6277585.2 27, 770564.3 6277579.3 27, 770558.9 6277573.2 27, 770556.6 6277575.2 27, 770555.8 6277574.3 27, 770551.5 6277578.2 27, 770557.6 6277585.2 27))
-BATIMENT0000000211120379;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;2.5;1.0;2.0;45;10;5.3;21.8;27.1;28.7;21.8;Cadastre;A 1.0;POLYGON Z ((770557.6 6277591.8 27.1, 770554.4 6277588.1 27.1, 770557.6 6277585.2 27.1, 770551.5 6277578.2 27.1, 770546.8 6277582.4 27.1, 770547.6 6277583.3 27.1, 770545.2 6277585.3 27.1, 770554 6277595 27.1, 770557.6 6277591.8 27.1))
-BATIMENT0000000211120316;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;1.0;1.0;2.0;45;10;6.8;21.1;27.9;28.8;21.3;Cadastre;A 1.0;POLYGON Z ((770539.4 6277601.5 27.9, 770546.2 6277595.4 27.9, 770540.8 6277589.4 27.9, 770538.1 6277591.7 27.9, 770537.3 6277590.8 27.9, 770533.2 6277594.5 27.9, 770539.4 6277601.5 27.9))
-BATIMENT0000000211120315;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;3.0;1.0;1.0;1.0;40;10;7.0;21.2;28.2;28.9;21.4;Cadastre;A 1.0;POLYGON Z ((770539.4 6277601.5 28.1, 770533.2 6277594.5 28.1, 770528.5 6277598.6 28.1, 770525.5 6277595.3 28.1, 770523.3 6277597.1 28.1, 770532.6 6277607.7 28.1, 770539.4 6277601.5 28.1))
-BATIMENT0000000211120311;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;3.0;2.5;;;;;4.3;22.0;26.3;27.0;22.0;Cadastre;;POLYGON Z ((770524 6277602.7 26.3, 770523 6277601.7 26.3, 770518.7 6277605.7 26.3, 770519.6 6277606.6 26.3, 770524 6277602.7 26.3))
-BATIMENT0000000211120314;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;3.0;1.0;1.0;2.0;04;01;6.9;21.3;28.2;28.9;21.5;Cadastre;C 0.6;POLYGON Z ((770523.3 6277597.1 28.1, 770520.8 6277599.3 28.1, 770523 6277601.7 28.1, 770524 6277602.7 28.1, 770519.6 6277606.6 28.1, 770525.9 6277613.7 28.1, 770526.3 6277613.4 28.1, 770532.6 6277607.7 28.1, 770523.3 6277597.1 28.1))
-BATIMENT0000000211120312;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;3.0;2.5;;;;;4.5;22.0;26.5;;;Cadastre;;POLYGON Z ((770519.6 6277606.6 26.5, 770518.7 6277605.7 26.5, 770514.4 6277609.6 26.5, 770515.2 6277610.5 26.5, 770519.6 6277606.6 26.5))
-BATIMENT0000000231251240;Indifférenciée;Indifférencié;;Non;En service;2010-04-30 12:01:24;2018-02-20 09:16:47;;2009-07-01;;;2.5;1.5;;;;;3.2;22.2;;;;Imagerie aérienne;;POLYGON Z ((770526.3 6277613.4 25.4, 770528 6277615.6 24.6, 770534.7 6277610.5 24.9, 770532.6 6277607.7 25.4, 770526.3 6277613.4 25.4))
-BATIMENT0000000211120310;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;1.0;1.0;2.0;40;10;6.7;21.4;28.1;28.8;21.5;Cadastre;A 0.7;POLYGON Z ((770525.9 6277613.7 28, 770519.6 6277606.6 28, 770515.2 6277610.5 28, 770514.4 6277609.6 28, 770511.7 6277606.4 28, 770509.1 6277608.6 28, 770513.5 6277613.7 28, 770519 6277619.9 28, 770525.9 6277613.7 28))
-BATIMENT0000000211120392;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;3.6;21.1;24.7;26.5;21.2;Cadastre;;POLYGON Z ((770558.3 6277616 24.6, 770555.3 6277613.1 24.6, 770552.4 6277616.2 24.6, 770555.3 6277619.1 24.6, 770558.3 6277616 24.6))
-BATIMENT0000000211120276;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;5.0;1.0;0.0;1.0;;;2.1;21.4;23.5;24.0;21.5;Cadastre;A 0.1;POLYGON Z ((770529.3 6277624.2 23.5, 770527.9 6277622.6 23.5, 770524.9 6277625.2 23.5, 770526.3 6277626.9 23.5, 770529.3 6277624.2 23.5))
-BATIMENT0000000211120277;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.9;21.4;24.3;24.4;21.5;Cadastre;;POLYGON Z ((770530 6277625 24.2, 770529.3 6277624.2 24.2, 770526.3 6277626.9 24.2, 770526.9 6277627.6 24.2, 770530 6277625 24.2))
-BATIMENT0000000211120306;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.7;22.0;27.7;29.3;22.0;Cadastre;C 0.3;POLYGON Z ((770540.8 6277646 27.7, 770535.2 6277639.9 27.7, 770532.8 6277642.1 27.7, 770531.9 6277641 27.7, 770527.4 6277644.9 27.7, 770533.9 6277652.3 27.7, 770540.8 6277646 27.7))
-BATIMENT0000000211120304;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.2;22.0;Cadastre;C 0.3;POLYGON Z ((770533.9 6277652.3 27.8, 770527.4 6277644.9 27.8, 770523.2 6277648.8 27.8, 770524.3 6277649.9 27.8, 770521.7 6277652.2 27.8, 770526.9 6277658.5 27.8, 770529.8 6277655.9 27.8, 770533.9 6277652.3 27.8))
-BATIMENT0000000211120307;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;3.6;21.5;25.1;26.6;21.6;Cadastre;;POLYGON Z ((770531.7 6277658 25, 770535.7 6277654.4 25, 770533.9 6277652.3 25, 770529.8 6277655.9 25, 770531.7 6277658 25))
-BATIMENT0000000211120302;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;43;10;5.8;22.0;27.8;29.3;22.0;Cadastre;C 0.2;POLYGON Z ((770526.9 6277658.5 27.8, 770521.7 6277652.2 27.8, 770519.3 6277654.4 27.8, 770518.2 6277653.1 27.8, 770513.8 6277657.2 27.8, 770520.3 6277664.6 27.8, 770526.9 6277658.5 27.8))
-BATIMENT0000000211120397;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.9;21.6;24.5;26.8;21.7;Cadastre;;POLYGON Z ((770546.5 6277669.3 24.5, 770544.6 6277667 24.5, 770542.4 6277669 24.5, 770544.5 6277671.1 24.5, 770546.5 6277669.3 24.5))
-BATIMENT0000000211120341;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.5;22.0;Cadastre;A 1.0;POLYGON Z ((770556.1 6277678.1 29.3, 770560.1 6277674.4 29.3, 770559 6277673.3 29.3, 770561.3 6277671.1 29.3, 770555.5 6277664.9 29.3, 770549.3 6277670.6 29.3, 770556.1 6277678.1 29.3))
-BATIMENT0000000211120337;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;1.0;0.0;1.0;;;4.4;21.7;26.1;26.5;21.8;Cadastre;B 0.4;POLYGON Z ((770538.5 6277672.2 26.1, 770535.7 6277674.8 26.1, 770539.8 6277679.5 26.1, 770542.7 6277676.8 26.1, 770538.5 6277672.2 26.1))
-BATIMENT0000000211120313;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;2.0;21.5;23.5;24.9;21.5;Cadastre;;POLYGON Z ((770511.7 6277606.4 23.5, 770507.5 6277601.7 23.5, 770505 6277603.8 23.5, 770509.1 6277608.6 23.5, 770511.7 6277606.4 23.5))
-BATIMENT0000000211120245;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1968-01-01;;;;3.0;1.0;39.0;5.0;30;40;16.3;21.4;37.7;38.0;21.7;Cadastre;A 1.0;POLYGON Z ((770502.1 6277605 37.6, 770498 6277608.3 37.6, 770499 6277609.6 37.6, 770490.8 6277616 37.6, 770492.9 6277618.6 37.6, 770487.1 6277623.3 37.6, 770491.7 6277628.9 37.6, 770479.2 6277638.8 37.6, 770474.6 6277633.3 37.6, 770417.5 6277678.9 37.6, 770424.7 6277687.1 37.6, 770422.5 6277689.2 37.6, 770424.1 6277691.1 37.6, 770424 6277691.3 37.6, 770428.3 6277696.5 37.6, 770430.9 6277694.4 37.6, 770432.3 6277695.8 37.6, 770509.8 6277628 37.6, 770502.3 6277619.2 37.6, 770505.3 6277616.8 37.6, 770508.4 6277620.4 37.6, 770512.4 6277617 37.6, 770505.1 6277608.5 37.6, 770502.1 6277605 37.6))
-BATIMENT0000000211120303;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.0;22.0;Cadastre;C 0.1;POLYGON Z ((770520.3 6277664.6 27.8, 770513.8 6277657.2 27.8, 770509.1 6277661.3 27.8, 770510.2 6277662.5 27.8, 770507.8 6277664.7 27.8, 770513.2 6277670.9 27.8, 770520.3 6277664.6 27.8))
-BATIMENT0000000211120308;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;3.8;21.5;25.3;26.5;21.6;Cadastre;;POLYGON Z ((770502.8 6277667.2 25.3, 770501.4 6277665.5 25.3, 770498.7 6277667.8 25.3, 770500.3 6277669.4 25.3, 770502.8 6277667.2 25.3))
-BATIMENT0000000211120305;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.2;22.0;Cadastre;C 0.3;POLYGON Z ((770506.5 6277676.8 27.8, 770510.1 6277673.6 27.8, 770516.7 6277680.8 27.8, 770519.6 6277678 27.8, 770513.2 6277670.9 27.8, 770507.8 6277664.7 27.8, 770506.8 6277663.7 27.8, 770502.8 6277667.2 27.8, 770500.3 6277669.4 27.8, 770506.5 6277676.8 27.8))
-BATIMENT0000000211120309;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.6;22.0;27.6;28.9;22.0;Cadastre;C 0.1;POLYGON Z ((770506.5 6277676.8 27.6, 770500.3 6277669.4 27.6, 770495.5 6277673.7 27.6, 770496.6 6277674.9 27.6, 770494.4 6277676.9 27.6, 770499.8 6277683 27.6, 770500.8 6277682.1 27.6, 770502.5 6277683.9 27.6, 770505.5 6277681.1 27.6, 770503.7 6277679.3 27.6, 770506.5 6277676.8 27.6))
-BATIMENT0000000211120399;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;1.5;21.7;23.2;24.3;21.8;Cadastre;;POLYGON Z ((770513.8 6277679.1 23.1, 770511.9 6277676.7 23.1, 770510.9 6277677.5 23.1, 770513 6277679.9 23.1, 770513.8 6277679.1 23.1))
-BATIMENT0000000211120402;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;4.7;21.6;26.3;27.2;21.7;Cadastre;;POLYGON Z ((770494.8 6277682.3 26.2, 770492.6 6277680.1 26.2, 770491.8 6277680.9 26.2, 770494 6277683.1 26.2, 770494.8 6277682.3 26.2))
-BATIMENT0000000211120255;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;0.0;2.0;;;5.4;22.7;28.1;29.2;22.7;Cadastre;C 0.3;POLYGON Z ((770493.4 6277687.7 28.1, 770487.8 6277681.4 28.1, 770485.6 6277683.4 28.1, 770484.7 6277682.2 28.1, 770480.3 6277686.1 28.1, 770486.8 6277693.6 28.1, 770493.4 6277687.7 28.1))
-BATIMENT0000000211120398;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.1;21.8;23.9;24.2;21.9;Cadastre;;POLYGON Z ((770503.8 6277688.3 23.8, 770501.7 6277686 23.8, 770500.6 6277687.1 23.8, 770502.7 6277689.4 23.8, 770503.8 6277688.3 23.8))
-BATIMENT0000000211120256;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.4;22.7;28.1;29.3;22.7;Cadastre;C 0.3;POLYGON Z ((770480 6277699.8 28.1, 770486.8 6277693.6 28.1, 770480.3 6277686.1 28.1, 770475.6 6277690.3 28.1, 770476.6 6277691.4 28.1, 770474.3 6277693.4 28.1, 770480 6277699.8 28.1))
-BATIMENT0000000211120400;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.0;21.8;23.8;24.2;22.0;Cadastre;;POLYGON Z ((770492.6 6277699.5 23.8, 770490.4 6277697 23.8, 770489.2 6277698.1 23.8, 770491.4 6277700.6 23.8, 770492.6 6277699.5 23.8))
-BATIMENT0000000211120257;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.5;22.7;28.2;29.3;22.7;Cadastre;C 0.3;POLYGON Z ((770480 6277699.8 28.2, 770474.3 6277693.4 28.2, 770472.2 6277695.4 28.2, 770471.1 6277694.3 28.2, 770466.8 6277698.2 28.2, 770473.3 6277705.8 28.2, 770480 6277699.8 28.2))
-BATIMENT0000000211120258;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;5.5;22.7;28.2;29.4;22.7;Cadastre;C 0.3;POLYGON Z ((770466.8 6277698.2 28.2, 770462 6277702.4 28.2, 770463.1 6277703.6 28.2, 770461 6277705.2 28.2, 770466.7 6277711.7 28.2, 770473.3 6277705.8 28.2, 770466.8 6277698.2 28.2))
-BATIMENT0000000211120251;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;22.9;29.1;30.0;;Cadastre;C 0.3;POLYGON Z ((770454.8 6277712.7 29.1, 770449.1 6277706.2 29.1, 770442.8 6277711.8 29.1, 770444.8 6277714 29.1, 770443.9 6277714.8 29.1, 770447.7 6277719.2 29.1, 770454.8 6277712.7 29.1))
-BATIMENT0000000211120350;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;1.0;2.0;50;10;6.0;23.0;29.0;30.4;23.0;Cadastre;A 1.0;POLYGON Z ((770516.5 6277715.5 29, 770512.7 6277711.5 29, 770511.6 6277712.7 29, 770509.3 6277710.3 29, 770503.1 6277715.8 29, 770509.2 6277722.3 29, 770516.5 6277715.5 29))
-BATIMENT0000000211120273;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2020-05-29 12:14:55;;;;;5.0;1.0;;;;;2.0;21.8;23.8;23.8;21.9;Cadastre;;POLYGON Z ((770465.2 6277716.5 23.7, 770464.4 6277715.6 23.7, 770462.9 6277717 23.7, 770463.7 6277717.9 23.7, 770465.2 6277716.5 23.7))
-BATIMENT0000000211120252;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.2;22.9;29.1;30.3;;Cadastre;C 0.3;POLYGON Z ((770461 6277719.5 29.1, 770454.8 6277712.7 29.1, 770447.7 6277719.2 29.1, 770451.4 6277723.3 29.1, 770452.3 6277722.6 29.1, 770454.6 6277725.2 29.1, 770461 6277719.5 29.1))
-BATIMENT0000000211120272;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.8;21.9;24.7;24.7;22.1;Cadastre;;POLYGON Z ((770472.3 6277724.6 24.6, 770470.3 6277722.3 24.6, 770468.8 6277723.6 24.6, 770470.8 6277725.9 24.6, 770472.3 6277724.6 24.6))
-BATIMENT0000000211120253;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.3;22.9;29.2;30.3;22.9;Cadastre;C 0.3;POLYGON Z ((770461 6277719.5 29.2, 770454.6 6277725.2 29.2, 770456.6 6277727.7 29.2, 770455.8 6277728.5 29.2, 770459.6 6277732.6 29.2, 770466.7 6277726.2 29.2, 770461 6277719.5 29.2))
-BATIMENT0000000211120259;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;24.0;6.0;40;40;13.0;22.7;35.7;;;Cadastre;C 0.1;POLYGON Z ((770440.4 6277739.7 35.7, 770400.7 6277694.1 35.7, 770394 6277700 35.7, 770398.6 6277705.2 35.7, 770397.9 6277706 35.7, 770402.4 6277711.1 35.7, 770403.1 6277710.5 35.7, 770411.8 6277720.4 35.7, 770411 6277721 35.7, 770415.8 6277726.3 35.7, 770416.4 6277725.7 35.7, 770424.7 6277735.3 35.7, 770424 6277735.9 35.7, 770428.8 6277741.3 35.7, 770429.3 6277740.8 35.7, 770433.7 6277745.7 35.7, 770440.4 6277739.7 35.7))
-BATIMENT0000000211120208;Eglise;Religieux;;Oui;En service;2008-11-18 15:28:19;;;;;;3.0;2.5;;;;;6.2;23.0;29.2;;;Cadastre;;POLYGON Z ((770290.2 6277720.8 29.2, 770289.8 6277718.4 29.2, 770264.1 6277723.2 29.2, 770264.6 6277725.6 29.2, 770290.2 6277720.8 29.2))
-BATIMENT0000000211120207;Eglise;Religieux;;Non;En service;2008-11-18 15:28:19;;;;;;3.0;2.5;;;;;5.9;23.0;28.9;;;Cadastre;;POLYGON Z ((770289.4 6277714.6 28.9, 770289.8 6277718.4 28.9, 770290.2 6277720.8 28.9, 770264.6 6277725.6 28.9, 770260.1 6277726.4 28.9, 770261.6 6277734.4 28.9, 770265.8 6277733.6 28.9, 770292.7 6277728.9 28.9, 770293.1 6277731.4 28.9, 770293.5 6277733.3 28.9, 770302.7 6277725.5 28.9, 770302.1 6277714 28.9, 770289.4 6277714.6 28.9))
-BATIMENT0000000211120206;Eglise;Religieux;;Oui;En service;2008-11-18 15:28:19;;;;;;3.0;2.5;;;;;5.9;23.0;28.9;;;Cadastre;;POLYGON Z ((770292.7 6277728.9 28.9, 770265.8 6277733.6 28.9, 770266.2 6277735.9 28.9, 770293.1 6277731.4 28.9, 770292.7 6277728.9 28.9))
-BATIMENT0000000211120179;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;5.0;1.0;1.0;1.0;00;00;3.4;22.7;26.1;26.4;22.8;Cadastre;C 1.0;POLYGON Z ((770275.8 6277747.4 26, 770272.8 6277743.9 26, 770270.6 6277746 26, 770273.6 6277749.4 26, 770275.8 6277747.4 26))
-BATIMENT0000000211120241;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;3.0;2.5;;;;;7.3;22.9;30.2;30.6;23.2;Cadastre;;POLYGON Z ((770396.5 6277742.1 30.2, 770395.6 6277742.8 30.2, 770393.5 6277740.3 30.2, 770394.4 6277739.5 30.2, 770390.7 6277735.2 30.2, 770389.8 6277736 30.2, 770387.5 6277733.5 30.2, 770388.4 6277732.7 30.2, 770384.8 6277728.6 30.2, 770383.9 6277729.2 30.2, 770381.8 6277726.8 30.2, 770382.7 6277726 30.2, 770378.9 6277721.7 30.2, 770376.6 6277723.7 30.2, 770375.4 6277722.3 30.2, 770370 6277726.9 30.2, 770367.7 6277724.2 30.2, 770363.4 6277728 30.2, 770364.5 6277729.3 30.2, 770363.1 6277730.7 30.2, 770364.1 6277732 30.2, 770362.8 6277733.1 30.2, 770365.5 6277736.3 30.2, 770370.8 6277731.5 30.2, 770382.6 6277744.8 30.2, 770380 6277747 30.2, 770382.4 6277749.7 30.2, 770374.1 6277757 30.2, 770374 6277760.2 30.2, 770374.6 6277760.8 30.2, 770372 6277763 30.2, 770329 6277714.3 30.2, 770320.6 6277721.8 30.2, 770319.6 6277720.7 30.2, 770319.8 6277720.3 30.2, 770317 6277717 30.2, 770313.1 6277720.4 30.2, 770365.4 6277780.4 30.2, 770377.9 6277769.6 30.2, 770377 6277768.5 30.2, 770375.2 6277766.5 30.2, 770377.9 6277764.2 30.2, 770379.7 6277766.2 30.2, 770381.1 6277765.1 30.2, 770381.8 6277766.1 30.2, 770386.4 6277762 30.2, 770385.7 6277761.1 30.2, 770387.9 6277759.2 30.2, 770388.8 6277760.1 30.2, 770393.1 6277756.2 30.2, 770392.4 6277755.2 30.2, 770395 6277753 30.2, 770395.8 6277754 30.2, 770400 6277750.4 30.2, 770399 6277749.2 30.2, 770400.1 6277748.3 30.2, 770399 6277747 30.2, 770400.2 6277746.1 30.2, 770396.5 6277742.1 30.2))
-BATIMENT0000000211120240;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;3.0;1.0;;;;;12.9;22.6;35.5;38.8;22.7;Cadastre;;POLYGON Z ((770399 6277747 35.5, 770400.1 6277748.3 35.5, 770399 6277749.2 35.5, 770400 6277750.4 35.5, 770402.1 6277748.5 35.5, 770400.2 6277746.1 35.5, 770399 6277747 35.5))
-BATIMENT0000000211120270;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;5.0;1.0;;;;;2.0;23.0;25.0;25.7;23.1;Cadastre;;POLYGON Z ((770339.4 6277758.6 24.9, 770337.8 6277756.8 24.9, 770331.7 6277762 24.9, 770333.3 6277763.9 24.9, 770339.4 6277758.6 24.9))
-BATIMENT0000000211120242;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;3.0;1.0;;;;;3.3;23.0;26.3;28.5;23.1;Cadastre;;POLYGON Z ((770379.7 6277766.2 26.2, 770377.9 6277764.2 26.2, 770375.2 6277766.5 26.2, 770377 6277768.5 26.2, 770379.7 6277766.2 26.2))
-BATIMENT0000000211120269;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;5.0;1.0;;;;;2.4;23.0;25.4;26.0;23.2;Cadastre;;POLYGON Z ((770346.3 6277766.6 25.4, 770344.7 6277764.7 25.4, 770338.7 6277770 25.4, 770340.4 6277771.8 25.4, 770346.3 6277766.6 25.4))
-BATIMENT0000000211120254;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1965-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.3;23.0;29.3;29.9;23.0;Cadastre;C 0.3;POLYGON Z ((770459.6 6277732.6 29.3, 770463.7 6277737.2 29.3, 770464.4 6277736.4 29.3, 770466.4 6277738.6 29.3, 770472.7 6277733 29.3, 770466.7 6277726.2 29.3, 770459.6 6277732.6 29.3))
-BATIMENT0000000211120231;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;4.1;22.2;26.3;27.7;22.5;Cadastre;;POLYGON Z ((770443.7 6277746 26.3, 770441 6277742.9 26.3, 770437.8 6277745.8 26.3, 770440.5 6277748.9 26.3, 770443.7 6277746 26.3))
-BATIMENT0000000211120248;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.0;23.6;30.6;31.0;23.6;Cadastre;C 0.3;POLYGON Z ((770487.1 6277749.3 30.6, 770481.4 6277742.8 30.6, 770474.9 6277748.6 30.6, 770477.1 6277750.9 30.6, 770476 6277751.8 30.6, 770479.8 6277756 30.6, 770487.1 6277749.3 30.6))
-BATIMENT0000000211120249;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;40;10;7.0;23.6;30.6;30.8;23.6;Cadastre;C 0.3;POLYGON Z ((770483.6 6277760.3 30.6, 770484.5 6277759.5 30.6, 770486.7 6277761.9 30.6, 770493.1 6277756.2 30.6, 770487.1 6277749.3 30.6, 770479.8 6277756 30.6, 770483.6 6277760.3 30.6))
-BATIMENT0000000211120328;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;3.0;2.5;1.0;2.0;45;13;6.2;24.3;30.5;31.2;;Cadastre;C 0.2;POLYGON Z ((770497.6 6277762 30.5, 770491.2 6277767.7 30.5, 770493.2 6277769.9 30.5, 770492.2 6277770.7 30.5, 770496.1 6277775.1 30.5, 770503.6 6277768.6 30.5, 770497.6 6277762 30.5))
-BATIMENT0000000211120329;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;1.0;2.0;40;10;6.1;24.3;30.4;31.3;24.3;Cadastre;C 0.3;POLYGON Z ((770496.1 6277775.1 30.4, 770499.9 6277779.5 30.4, 770500.9 6277778.8 30.4, 770502.8 6277781.1 30.4, 770509.3 6277775.3 30.4, 770503.6 6277768.6 30.4, 770496.1 6277775.1 30.4))
-BATIMENT0000000211120250;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1965-01-01;;;;3.0;2.5;55.0;4.0;40;40;12.9;24.3;37.2;38.1;25.4;Cadastre;A 1.0;POLYGON Z ((770438.3 6277841.6 37.2, 770413.1 6277812.4 37.2, 770417.9 6277808.1 37.2, 770418.4 6277808.7 37.2, 770423.7 6277804 37.2, 770423.3 6277803.3 37.2, 770432.9 6277794.8 37.2, 770433.5 6277795.5 37.2, 770438.8 6277790.6 37.2, 770438.4 6277790 37.2, 770447.9 6277781.6 37.2, 770448.3 6277782.3 37.2, 770454.2 6277777.2 37.2, 770453.6 6277776.6 37.2, 770458.4 6277772.5 37.2, 770460.6 6277775 37.2, 770459.9 6277775.6 37.2, 770465.7 6277782 37.2, 770466.4 6277781.5 37.2, 770474.4 6277790.6 37.2, 770473.6 6277791.2 37.2, 770479.2 6277797.6 37.2, 770479.9 6277796.9 37.2, 770483.5 6277801 37.2, 770490.1 6277794.8 37.2, 770463.5 6277764.5 37.2, 770456.7 6277770.4 37.2, 770452.5 6277765.5 37.2, 770406.9 6277805.6 37.2, 770411 6277810.3 37.2, 770404.2 6277816.3 37.2, 770408 6277820.8 37.2, 770407.2 6277821.5 37.2, 770413 6277828.1 37.2, 770413.9 6277827.3 37.2, 770421.8 6277836.5 37.2, 770421.1 6277837.3 37.2, 770426.7 6277843.7 37.2, 770427.5 6277842.9 37.2, 770431.5 6277847.6 37.2, 770438.3 6277841.6 37.2))
-BATIMENT0000000211120246;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;22.0;6.0;00;00;16.0;25.6;41.6;42.2;25.6;Cadastre;A 1.0;POLYGON Z ((770510.8 6277827.6 41.6, 770495.9 6277811.8 41.6, 770483.1 6277823.9 41.6, 770498.4 6277839.6 41.6, 770510.8 6277827.6 41.6))
-BATIMENT0000000211120508;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;48.0;6.0;40;40;18.9;26.0;44.9;46.9;26.2;Cadastre;A 1.0;POLYGON Z ((770413 6277896.7 44.9, 770417.6 6277892.3 44.9, 770418.4 6277893 44.9, 770423.2 6277888.5 44.9, 770422.4 6277887.7 44.9, 770432.2 6277878.5 44.9, 770433 6277879.3 44.9, 770437.8 6277874.7 44.9, 770437 6277873.9 44.9, 770446.8 6277864.6 44.9, 770447.5 6277865.5 44.9, 770452.5 6277860.8 44.9, 770451.6 6277860.1 44.9, 770461.2 6277851 44.9, 770462 6277851.8 44.9, 770467 6277847.1 44.9, 770466.3 6277846.2 44.9, 770471.4 6277841.4 44.9, 770465.3 6277835 44.9, 770452.1 6277847 44.9, 770436.6 6277861.5 44.9, 770419.8 6277877.6 44.9, 770406.6 6277890.1 44.9, 770413 6277896.7 44.9))
-BATIMENT0000000211120504;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;2.5;4.0;2.0;15;10;6.8;27.0;33.8;34.0;27.0;Cadastre;C 0.2;POLYGON Z ((770442.6 6277891.6 33.8, 770451.9 6277901.6 33.8, 770459.2 6277894.7 33.8, 770454.1 6277889 33.8, 770467.8 6277876 33.8, 770461.2 6277868.9 33.8, 770442.7 6277886.2 33.8, 770442.6 6277891.6 33.8))
-BATIMENT0000000211120203;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;2.5;;;;;15.9;23.5;39.4;41.3;23.9;Cadastre;;POLYGON Z ((770213.4 6277782.5 39.4, 770215.1 6277784.3 39.4, 770239.1 6277764 39.4, 770240.3 6277765.3 39.4, 770246.6 6277760.1 39.4, 770235.6 6277747.6 39.4, 770229.3 6277752.9 39.4, 770230.8 6277754.5 39.4, 770206.9 6277774.9 39.4, 770205.2 6277773 39.4, 770190.6 6277785.4 39.4, 770198.9 6277794.6 39.4, 770213.4 6277782.5 39.4))
-BATIMENT0000000211120271;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;5.0;1.0;;;;;3.2;23.0;26.2;26.5;23.2;Cadastre;;POLYGON Z ((770339.7 6277772 26.1, 770335.6 6277767.3 26.1, 770331.5 6277762.6 26.1, 770326.7 6277766.7 26.1, 770322.1 6277770.8 26.1, 770326 6277775.5 26.1, 770330.2 6277780.3 26.1, 770335.1 6277776.1 26.1, 770339.7 6277772 26.1))
-BATIMENT0000000211120260;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;3.0;1.0;43.0;9.0;40;40;21.9;22.7;44.6;51.8;24.3;Cadastre;C 0.7;POLYGON Z ((770353.9 6277828.3 44.5, 770354.4 6277828.9 44.5, 770360.6 6277823.5 44.5, 770360.2 6277822.8 44.5, 770369.3 6277814.7 44.5, 770369.9 6277815.5 44.5, 770376.2 6277809.8 44.5, 770375.6 6277809.2 44.5, 770380 6277805.5 44.5, 770379.7 6277805.2 44.5, 770383.7 6277801.6 44.5, 770384.4 6277802.4 44.5, 770390.8 6277796.7 44.5, 770390.2 6277795.8 44.5, 770398.8 6277788.5 44.5, 770399.4 6277789.2 44.5, 770405.9 6277783.6 44.5, 770405.3 6277782.9 44.5, 770414.3 6277775.1 44.5, 770415 6277775.8 44.5, 770421.1 6277770.4 44.5, 770420.4 6277769.7 44.5, 770424.4 6277766.2 44.5, 770424.7 6277766.4 44.5, 770429.1 6277762.5 44.5, 770429.6 6277763.2 44.5, 770435.9 6277757.6 44.5, 770435.3 6277757 44.5, 770440 6277753 44.5, 770434 6277746.1 44.5, 770342.9 6277825.1 44.5, 770349.3 6277832.4 44.5, 770353.9 6277828.3 44.5))
-BATIMENT0000000211120219;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1978-01-01;;;;3.0;2.5;0.0;1.0;;;17.0;23.6;40.6;40.8;24.1;Cadastre;C 0.2;POLYGON Z ((770264.2 6277770.9 40.6, 770259.7 6277774.5 40.6, 770271.1 6277787.9 40.6, 770270.1 6277788.9 40.6, 770271.6 6277790.6 40.6, 770260.3 6277800.3 40.6, 770259.2 6277799 40.6, 770232.5 6277822.3 40.6, 770232.4 6277822.8 40.6, 770229.7 6277825.4 40.6, 770232.5 6277828.4 40.6, 770235.4 6277826 40.6, 770240.5 6277832 40.6, 770267.3 6277808.5 40.6, 770268.3 6277809.6 40.6, 770279.9 6277799.5 40.6, 770281.2 6277801.1 40.6, 770287.6 6277795.5 40.6, 770276 6277782.2 40.6, 770279.8 6277778.9 40.6, 770269.1 6277766.7 40.6, 770264.2 6277770.9 40.6))
-BATIMENT0000000211120464;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;3.0;2.5;;;;;7.1;25.0;32.1;32.7;25.0;Cadastre;;POLYGON Z ((770267.4 6277853.2 32.1, 770265.6 6277854.8 32.1, 770268.3 6277857.8 32.1, 770270 6277856.3 32.1, 770267.4 6277853.2 32.1))
-BATIMENT0000000211120465;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;2007-01-01;;;;3.0;2.5;0.0;1.0;;;3.7;25.0;28.7;32.4;25.2;Cadastre;C 0.5;POLYGON Z ((770301.2 6277869.1 28.7, 770300.2 6277868 28.7, 770301.1 6277867 28.7, 770301.1 6277865 28.7, 770298.4 6277861.9 28.7, 770301.9 6277859 28.7, 770299.7 6277856.4 28.7, 770299.8 6277854.6 28.7, 770298 6277854.5 28.7, 770295.7 6277852 28.7, 770296.1 6277850.4 28.7, 770294.4 6277850.4 28.7, 770292.1 6277847.8 28.7, 770292.3 6277846.1 28.7, 770290.6 6277846.1 28.7, 770288.2 6277843.3 28.7, 770288.4 6277841.6 28.7, 770286.7 6277841.6 28.7, 770282.6 6277837.1 28.7, 770264.1 6277853.3 28.7, 770265.6 6277854.8 28.7, 770267.4 6277853.2 28.7, 770270 6277856.3 28.7, 770274 6277860.8 28.7, 770278.7 6277856.6 28.7, 770285.9 6277864.9 28.7, 770280.2 6277870.1 28.7, 770272.7 6277861.6 28.7, 770270.4 6277861.2 28.7, 770268.4 6277863 28.7, 770268.4 6277864.5 28.7, 770266.2 6277866.4 28.7, 770264.7 6277866.3 28.7, 770262.1 6277868.6 28.7, 770262 6277870 28.7, 770264 6277872.2 28.7, 770265.4 6277872.1 28.7, 770267.6 6277874.6 28.7, 770267.4 6277876 28.7, 770269.4 6277878.3 28.7, 770271.1 6277878.2 28.7, 770273.9 6277875.7 28.7, 770274.8 6277876.8 28.7, 770273.1 6277878.4 28.7, 770274.2 6277879.6 28.7, 770275.9 6277877.9 28.7, 770276.2 6277878.3 28.7, 770279.3 6277878.6 28.7, 770281.5 6277876.6 28.7, 770283.7 6277878.9 28.7, 770287.6 6277878.9 28.7, 770289.6 6277877.3 28.7, 770290.8 6277878.4 28.7, 770288.7 6277880.3 28.7, 770288.4 6277884.1 28.7, 770289.9 6277885.8 28.7, 770288.3 6277887.2 28.7, 770288.1 6277891.9 28.7, 770293.2 6277897.9 28.7, 770305.9 6277887 28.7, 770302.4 6277882.8 28.7, 770310.5 6277875.5 28.7, 770304.3 6277868.6 28.7, 770301.8 6277868.6 28.7, 770301.2 6277869.1 28.7))
-BATIMENT0000000211120488;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;3.0;2.5;;;;;3.5;25.0;28.5;28.5;25.0;Cadastre;;POLYGON Z ((770303.1 6277867.4 28.5, 770302.1 6277866.1 28.5, 770301.1 6277867 28.5, 770300.2 6277868 28.5, 770301.2 6277869.1 28.5, 770301.8 6277868.6 28.5, 770303.1 6277867.4 28.5))
-BATIMENT0000000211120487;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;2.5;;;;;3.5;25.0;28.5;28.9;25.0;Cadastre;;POLYGON Z ((770290.8 6277878.4 28.5, 770289.6 6277877.3 28.5, 770287.6 6277878.9 28.5, 770288.7 6277880.3 28.5, 770290.8 6277878.4 28.5))
-BATIMENT0000002275435066;Indifférenciée;Résidentiel;;Oui;En service;2021-12-09 16:30:40;;;;DGFiP;;5.0;9999.0;;;;;;;;;;Cadastre;;POLYGON Z ((770281.6 6277879.6 -1000, 770276.1 6277879.4 -1000, 770274.6 6277880.8 -1000, 770277 6277883.4 -1000, 770278.9 6277881.7 -1000, 770284 6277887.4 -1000, 770286.6 6277885.1 -1000, 770281.6 6277879.6 -1000))
-BATIMENT0000000211120511;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;3.0;2.5;40.0;4.0;40;40;13.3;25.9;39.2;40.0;26.0;Cadastre;A 1.0;POLYGON Z ((770335.3 6277930.4 39.2, 770336 6277930.9 39.2, 770341.2 6277926.4 39.2, 770340.7 6277925.8 39.2, 770350.8 6277917 39.2, 770351.3 6277917.7 39.2, 770356.3 6277913.2 39.2, 770355.8 6277912.6 39.2, 770365.7 6277903.8 39.2, 770366.4 6277904.6 39.2, 770371.2 6277900.3 39.2, 770370.6 6277899.7 39.2, 770380.4 6277891 39.2, 770381.1 6277891.7 39.2, 770386.5 6277887 39.2, 770385.9 6277886.3 39.2, 770396 6277877.7 39.2, 770396.6 6277878.4 39.2, 770402 6277873.7 39.2, 770401.4 6277873 39.2, 770406.4 6277868.7 39.2, 770400.8 6277862.1 39.2, 770324.3 6277928.5 39.2, 770329.8 6277935.1 39.2, 770335.3 6277930.4 39.2))
-BATIMENT0000000211120486;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;5.0;1.0;;;;;2.6;26.2;28.8;29.0;26.6;Cadastre;;POLYGON Z ((770478.1 6277882.4 28.8, 770469.8 6277890.4 28.8, 770470.9 6277891.6 28.8, 770479.4 6277883.8 28.8, 770478.1 6277882.4 28.8))
-BATIMENT0000000211120522;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1957-01-01;;;;3.0;1.0;2.0;2.0;15;10;7.6;26.4;34.0;34.8;27.0;Cadastre;A 1.0;POLYGON Z ((770506.4 6277891.3 34, 770499.5 6277884 34, 770492.3 6277890.9 34, 770499.2 6277898.4 34, 770506.4 6277891.3 34))
-BATIMENT0000000211120502;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1957-01-01;;;;3.0;2.5;2.0;2.0;50;10;5.9;27.9;33.8;35.4;27.9;Cadastre;A 1.0;POLYGON Z ((770494.6 6277904.4 33.8, 770484 6277893 33.8, 770476.8 6277899.8 33.8, 770487.4 6277911.2 33.8, 770494.6 6277904.4 33.8))
-BATIMENT0000000211120505;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1958-01-01;;;;3.0;2.5;6.0;3.0;15;10;10.3;27.8;38.1;39.8;27.9;Cadastre;A 1.0;POLYGON Z ((770480.4 6277917.9 38.1, 770473.7 6277910.8 38.1, 770475.8 6277908.7 38.1, 770471.2 6277904 38.1, 770469.3 6277905.7 38.1, 770462.3 6277898.2 38.1, 770454.7 6277905.5 38.1, 770472.9 6277925.1 38.1, 770480.4 6277917.9 38.1))
-BATIMENT0000000211120506;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1972-01-01;;;;3.0;2.5;1.0;2.0;50;10;5.8;28.0;33.8;35.0;28.0;Cadastre;A 1.0;POLYGON Z ((770436.5 6277913.2 33.8, 770428.1 6277904.4 33.8, 770420.3 6277911.7 33.8, 770428.7 6277920.7 33.8, 770436.5 6277913.2 33.8))
-BATIMENT0000000211120503;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1953-01-01;;;;3.0;1.0;3.0;2.0;10;10;9.2;27.6;36.8;38.0;28.4;Cadastre;A 1.0;POLYGON Z ((770452.5 6277936.1 36.8, 770447.9 6277931.2 36.8, 770447 6277932 36.8, 770444.9 6277929.7 36.8, 770436.8 6277937.1 36.8, 770443.6 6277944.2 36.8, 770452.5 6277936.1 36.8))
-BATIMENT0000000211120510;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1982-01-01;;;;3.0;2.5;3.0;2.0;10;10;7.4;26.6;34.0;35.2;;Cadastre;A 1.0;POLYGON Z ((770313.5 6277912.6 34, 770314.5 6277913.7 34, 770327.3 6277902.4 34, 770320.2 6277893.9 34, 770304.1 6277908 34, 770310.5 6277915.2 34, 770313.5 6277912.6 34))
-BATIMENT0000000211120477;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;2007-01-01;;;;3.0;1.0;0.0;1.0;;;12.8;25.1;37.9;44.5;25.7;Cadastre;C 0.4;POLYGON Z ((770282.2 6277918 37.9, 770270 6277904.1 37.9, 770256.3 6277916.2 37.9, 770268.5 6277930 37.9, 770282.2 6277918 37.9))
-BATIMENT0000000211120509;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;54.0;9.0;00;00;21.3;26.9;48.2;54.4;26.9;Cadastre;A 1.0;POLYGON Z ((770362.9 6277931 48.2, 770361.9 6277929.9 48.2, 770347 6277944.2 48.2, 770353.5 6277951.2 48.2, 770358.2 6277946.8 48.2, 770359.1 6277947.3 48.2, 770363.8 6277942.7 48.2, 770363.3 6277942.1 48.2, 770373.2 6277932.8 48.2, 770373.8 6277933.5 48.2, 770378.7 6277929 48.2, 770378 6277928.4 48.2, 770387.8 6277919.4 48.2, 770388.5 6277920 48.2, 770393.4 6277915.3 48.2, 770392.9 6277914.7 48.2, 770397.5 6277910.4 48.2, 770398 6277910.9 48.2, 770402.7 6277906.4 48.2, 770403.5 6277907.2 48.2, 770408.9 6277902 48.2, 770408.2 6277901.4 48.2, 770413 6277896.7 48.2, 770406.6 6277890.1 48.2, 770362.9 6277931 48.2))
-BATIMENT0000000211120507;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1850-01-01;;;;3.0;1.0;1.0;2.0;10;10;6.9;25.5;32.4;32.9;25.9;Cadastre;A 1.0;POLYGON Z ((770317.4 6277922.2 32.3, 770313.3 6277917.5 32.3, 770303.2 6277926.4 32.3, 770303.7 6277927.1 32.3, 770301.8 6277928.8 32.3, 770305.1 6277932.9 32.3, 770317.4 6277922.2 32.3))
-BATIMENT0000000231251324;Indifférenciée;Annexe;;Non;En service;2010-04-30 12:01:24;2019-04-08 10:00:52;1999-01-01;2009-07-01;;;2.5;1.5;0.0;1.0;00;00;4.6;26.5;;39.0;28.1;Imagerie aérienne;C 0.3;POLYGON Z ((770411.8 6277932.9 30.6, 770404.3 6277925.1 30.9, 770398.5 6277931.1 30.9, 770405.9 6277938.6 31, 770411.8 6277932.9 30.6))
-BATIMENT0000000211120491;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;3.0;2.5;;;;;4.6;28.2;32.8;;;Cadastre;;POLYGON Z ((770408.7 6277947.4 32.8, 770405.5 6277943.9 32.8, 770404.8 6277944.8 32.8, 770407.9 6277948.2 32.8, 770408.7 6277947.4 32.8))
-BATIMENT0000000211120482;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;12.1;25.9;38.0;43.0;26.1;Cadastre;;POLYGON Z ((770274.9 6277951 38, 770280 6277946.7 38, 770275.6 6277941.4 38, 770269.6 6277946.5 38, 770274.9 6277951 38))
-BATIMENT0000000211120492;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1986-01-01;;;;3.0;2.5;1.0;2.0;23;10;4.6;28.2;32.8;35.2;28.8;Cadastre;A 1.0;POLYGON Z ((770404.8 6277944.8 32.8, 770405.5 6277943.9 32.8, 770400.6 6277938.4 32.8, 770394.2 6277944.6 32.8, 770399.1 6277949.8 32.8, 770398.3 6277950.6 32.8, 770401.6 6277954 32.8, 770407.9 6277948.2 32.8, 770404.8 6277944.8 32.8))
-BATIMENT0000000211120497;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1954-01-01;;;;3.0;2.5;2.0;2.0;00;00;6.9;28.3;35.2;37.4;29.0;Cadastre;C 0.7;POLYGON Z ((770437.2 6277949.5 35.2, 770424.6 6277936.1 35.2, 770416.3 6277943.9 35.2, 770428.8 6277957.4 35.2, 770437.2 6277949.5 35.2))
-BATIMENT0000000211120483;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;10.8;26.0;36.8;43.3;26.2;Cadastre;;POLYGON Z ((770284.1 6277951.2 36.7, 770280 6277946.7 36.7, 770274.9 6277951 36.7, 770279.2 6277955.2 36.7, 770284.1 6277951.2 36.7))
-BATIMENT0000000211120484;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-07-29 11:03:18;;;;;3.0;1.0;9.0;5.0;01;01;9.6;26.1;35.7;38.3;26.5;Cadastre;C 0.1;POLYGON Z ((770290.8 6277966.9 35.6, 770296.2 6277961.9 35.6, 770286.2 6277949.4 35.6, 770284.1 6277951.2 35.6, 770279.2 6277955.2 35.6, 770278.2 6277956.2 35.6, 770288.5 6277967.3 35.6, 770290.8 6277966.9 35.6))
-BATIMENT0000000211120496;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;3.0;2.5;2.0;2.0;00;00;7.2;28.9;36.1;37.6;29.5;Cadastre;A 1.0;POLYGON Z ((770413.7 6277969 36.1, 770416.4 6277971.7 36.1, 770422.5 6277965.6 36.1, 770416 6277958.3 36.1, 770407 6277967 36.1, 770407.2 6277967.2 36.1, 770409.2 6277969.4 36.1, 770411.2 6277971.5 36.1, 770413.7 6277969 36.1))
-BATIMENT0000000211120494;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;3.0;1.0;;;;;2.9;29.2;32.1;32.3;29.5;Cadastre;;POLYGON Z ((770405.4 6277968.8 32, 770407.5 6277971 32, 770409.2 6277969.4 32, 770407.2 6277967.2 32, 770405.4 6277968.8 32))
-BATIMENT0000000211120495;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1952-01-01;;;;3.0;2.5;3.0;2.0;10;10;6.3;28.9;35.2;37.7;29.7;Cadastre;A 1.0;POLYGON Z ((770411 6277976.4 35.2, 770404.3 6277968.9 35.2, 770391.3 6277981.4 35.2, 770398 6277988.7 35.2, 770411 6277976.4 35.2))
-BATIMENT0000000211120498;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1956-01-01;;;;3.0;2.5;1.0;1.0;50;10;7.2;28.6;35.8;;;Cadastre;A 1.0;POLYGON Z ((770392.4 6277992 35.8, 770378.6 6277977.2 35.8, 770370.8 6277984.4 35.8, 770384.7 6277999.2 35.8, 770392.4 6277992 35.8))
-BATIMENT0000000211117722;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:26:42;2019-04-08 10:00:52;1973-01-01;;;;3.0;2.5;1.0;1.0;40;10;8.4;28.6;37.0;38.7;29.4;Cadastre;A 1.0;POLYGON Z ((770378.3 6278003.2 37, 770376.9 6278001.6 37, 770380.4 6277998.5 37, 770370.9 6277988.2 37, 770363.6 6277995 37, 770374.5 6278006.7 37, 770378.3 6278003.2 37))
+        _sio = StringIO("""ID;NATURE;USAGE1;USAGE2;LEGER;ETAT;DATE_CREAT;DATE_MAJ;DATE_APP;DATE_CONF;SOURCE;ID_SOURCE;ACQU_PLANI;PREC_PLANI;ACQU_ALTI;PREC_ALTI;NB_LOGTS;NB_ETAGES;MAT_MURS;MAT_TOITS;HAUTEUR;Z_MIN_SOL;Z_MIN_TOIT;Z_MAX_TOIT;Z_MAX_SOL;ORIGIN_BAT;APP_FF;geometry
+BATIMENT0000000211120434;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;1.0;;;5.9;19.7;25.6;26.2;20.5;Cadastre;C 0.3;POLYGON Z ((770762.1 6277456.6 25.5, 770733 6277467.8 25.5, 770736.3 6277476.4 25.5, 770765.2 6277465 25.5, 770762.1 6277456.6 25.5))
+BATIMENT0000000211120410;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1974-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;2.0;2.0;49;10;6.6;21.5;28.1;;;Cadastre;A 1.0;POLYGON Z ((770723 6277498.8 28.1, 770719.7 6277490.4 28.1, 770711.5 6277493.7 28.1, 770711.9 6277494.7 28.1, 770704.7 6277497.5 28.1, 770707.7 6277504.9 28.1, 770710.3 6277503.9 28.1, 770723 6277498.8 28.1))
+BATIMENT0000000044598816;Indifférenciée;Annexe;;Non;En service;2006-12-12 11:20:44;2019-04-08 10:00:52;1967-01-01;;;;BDTopo;2.5;BDTopo;1.5;0.0;1.0;00;00;2.4;22.0;;;;Imagerie aérienne;C 0.2;POLYGON Z ((770735.4 6277500.4 24.3, 770734.6 6277498 24.3, 770740.8 6277495.8 24.3, 770739.7 6277492.8 24.3, 770725.8 6277498.1 24.4, 770727.6 6277502.9 24.2, 770735.4 6277500.4 24.3))
+BATIMENT0000000211120356;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;10;10;5.6;21.5;27.1;27.2;;Cadastre;A 1.0;POLYGON Z ((770703.2 6277501.2 27.1, 770699.4 6277502.6 27.1, 770698.1 6277499.4 27.1, 770685.9 6277504 27.1, 770689.2 6277512.1 27.1, 770705.1 6277505.9 27.1, 770703.2 6277501.2 27.1))
+BATIMENT0000000211120375;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;30;10;5.0;22.0;27.0;28.0;;Cadastre;A 1.0;POLYGON Z ((770652.8 6277513 27, 770647 6277506.4 27, 770639.6 6277513.3 27, 770645.4 6277519.8 27, 770652.8 6277513 27))
+BATIMENT0000000211120357;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;;;6.0;21.3;27.3;28.8;;Cadastre;C 0.5;POLYGON Z ((770710.3 6277503.9 27.3, 770707.7 6277504.9 27.3, 770705.1 6277505.9 27.3, 770689.2 6277512.1 27.3, 770693.6 6277523.3 27.3, 770714.7 6277515 27.3, 770710.3 6277503.9 27.3))
+BATIMENT0000002275536127;Indifférenciée;Résidentiel;;Oui;En service;2021-12-17 15:40:19;2023-03-22 21:39:05;;;DGFiP;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.0;20.5;22.5;23.5;21.0;Cadastre;;POLYGON Z ((770650.6 6277519.7 22.5, 770642.7 6277526.7 22.5, 770643.7 6277527.7 22.5, 770645.6 6277526.1 22.5, 770646.9 6277527.5 22.5, 770652.7 6277521.9 22.5, 770650.6 6277519.7 22.5))
+BATIMENT0000000211120432;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1987-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;1.0;;;6.5;21.0;27.5;;;Cadastre;A 1.0;POLYGON Z ((770717.9 6277528.5 27.5, 770714.7 6277520 27.5, 770698.7 6277525.8 27.5, 770697.4 6277528.8 27.5, 770700 6277535.5 27.5, 770717.9 6277528.5 27.5))
+BATIMENT0000000211120368;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;20;10;6.5;21.2;27.7;;;Cadastre;A 1.0;POLYGON Z ((770656.2 6277522.9 27.7, 770655.2 6277523.9 27.7, 770653.1 6277521.7 27.7, 770652.7 6277521.9 27.7, 770646.9 6277527.5 27.7, 770652.6 6277533.8 27.7, 770660.1 6277527 27.7, 770656.2 6277522.9 27.7))
+BATIMENT0000000211120367;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;6.4;21.3;27.7;28.0;;Cadastre;A 1.0;POLYGON Z ((770664.9 6277534.6 27.7, 770662.9 6277532.4 27.7, 770664.1 6277531.3 27.7, 770660.1 6277527 27.7, 770652.6 6277533.8 27.7, 770658.6 6277540.4 27.7, 770664.9 6277534.6 27.7))
+BATIMENT0000000211120374;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;4.9;22.0;26.9;28.0;;Cadastre;C 0.7;POLYGON Z ((770647 6277506.4 26.9, 770643.4 6277502.4 26.9, 770642.2 6277503.3 26.9, 770640.3 6277501.2 26.9, 770633.9 6277507.1 26.9, 770639.6 6277513.3 26.9, 770647 6277506.4 26.9))
+BATIMENT0000000211120387;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;45;10;5.2;21.4;26.6;28.2;21.4;Cadastre;A 1.0;POLYGON Z ((770623.3 6277526.5 26.6, 770629.9 6277520.6 26.6, 770624.5 6277514.3 26.6, 770622.1 6277516.5 26.6, 770621.2 6277515.5 26.6, 770616.9 6277519.3 26.6, 770623.3 6277526.5 26.6))
+BATIMENT0000000211120386;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;34;10;6.2;20.5;26.7;28.4;20.7;Cadastre;A 1.0;POLYGON Z ((770623.3 6277526.5 26.7, 770616.9 6277519.3 26.7, 770612.7 6277523.1 26.7, 770613.6 6277524.1 26.7, 770611.5 6277526.1 26.7, 770616.8 6277532.3 26.7, 770623.3 6277526.5 26.7))
+BATIMENT0000000211120385;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.0;20.7;26.7;28.4;20.7;Cadastre;A 1.0;POLYGON Z ((770616.8 6277532.3 26.7, 770611.5 6277526.1 26.7, 770609.1 6277528.2 26.7, 770608.2 6277527.2 26.7, 770603.8 6277531 26.7, 770610.1 6277538.2 26.7, 770611.8 6277540.1 26.7, 770615.6 6277536.7 26.7, 770613.9 6277534.9 26.7, 770616.8 6277532.3 26.7))
+BATIMENT0000000211120384;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;46;10;6.0;20.7;26.7;28.2;20.7;Cadastre;A 1.0;POLYGON Z ((770612.5 6277540.9 26.7, 770611.8 6277540.1 26.7, 770610.1 6277538.2 26.7, 770603.8 6277531 26.7, 770599.5 6277535 26.7, 770600.5 6277536 26.7, 770598.4 6277537.9 26.7, 770603.8 6277544 26.7, 770606.1 6277546.6 26.7, 770612.5 6277540.9 26.7))
+BATIMENT0000000211120383;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.4;20.6;Cadastre;A 1.0;POLYGON Z ((770597.3 6277549.7 26.7, 770603.8 6277544 26.7, 770598.4 6277537.9 26.7, 770596.1 6277539.9 26.7, 770595.1 6277538.9 26.7, 770591.1 6277542.6 26.7, 770597.3 6277549.7 26.7))
+BATIMENT0000000211120382;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.3;20.6;Cadastre;A 1.0;POLYGON Z ((770597.3 6277549.7 26.7, 770591.1 6277542.6 26.7, 770586.6 6277546.6 26.7, 770587.5 6277547.5 26.7, 770585.2 6277549.5 26.7, 770590.6 6277555.7 26.7, 770597.3 6277549.7 26.7))
+BATIMENT0000000211120286;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;3.2;20.3;23.5;24.2;20.3;Cadastre;;POLYGON Z ((770622.4 6277554.7 23.4, 770624.6 6277557.2 23.4, 770626.2 6277555.9 23.4, 770627.5 6277554.8 23.4, 770625.2 6277552.2 23.4, 770623.6 6277553.7 23.4, 770622.4 6277554.7 23.4))
+BATIMENT0000000211120288;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.2;20.2;27.4;28.4;20.3;Cadastre;C 0.2;POLYGON Z ((770640.5 6277554.6 27.4, 770634.6 6277548.2 27.4, 770628.4 6277554.1 27.4, 770630.4 6277556.3 27.4, 770629.2 6277557.4 27.4, 770633 6277561.5 27.4, 770640.5 6277554.6 27.4))
+BATIMENT0000000211120381;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.6;20.7;Cadastre;A 1.0;POLYGON Z ((770585.2 6277549.5 26.7, 770582.9 6277551.6 26.7, 770582.1 6277550.6 26.7, 770578 6277554.2 26.7, 770584.2 6277561.4 26.7, 770590.6 6277555.7 26.7, 770585.2 6277549.5 26.7))
+BATIMENT0000000211120433;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;;;7.2;21.0;28.2;;;Cadastre;A 1.0;POLYGON Z ((770724.2 6277535.1 28.2, 770722.6 6277531 28.2, 770725.3 6277530 28.2, 770724 6277526.1 28.2, 770717.9 6277528.5 28.2, 770700 6277535.5 28.2, 770702.4 6277541.6 28.2, 770705.2 6277543.2 28.2, 770721.1 6277536.8 28.2, 770720.9 6277536.3 28.2, 770724.2 6277535.1 28.2))
+BATIMENT0000000211120366;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;6.4;21.3;27.7;27.8;;Cadastre;A 1.0;POLYGON Z ((770672 6277540.1 27.7, 770668.2 6277535.9 27.7, 770667 6277536.8 27.7, 770664.9 6277534.6 27.7, 770658.6 6277540.4 27.7, 770664.6 6277546.9 27.7, 770672 6277540.1 27.7))
+BATIMENT0000000211120365;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2021-12-17 15:40:19;1961-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;6.4;21.3;27.7;27.8;;Cadastre;A 1.0;POLYGON Z ((770670.7 6277553.5 27.7, 770676.9 6277547.8 27.7, 770674.8 6277545.3 27.7, 770675.9 6277544.4 27.7, 770672 6277540.1 27.7, 770664.6 6277546.9 27.7, 770670.7 6277553.5 27.7))
+BATIMENT0000000211120412;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1981-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;1.0;50;10;3.9;21.3;25.2;;;Cadastre;B 0.4;POLYGON Z ((770748.6 6277552.3 25.2, 770748.8 6277553.8 25.2, 770753.7 6277553.1 25.2, 770752.9 6277547.8 25.2, 770754.1 6277547.6 25.2, 770753 6277539.6 25.2, 770748.7 6277540.2 25.2, 770749.1 6277543.4 25.2, 770737.7 6277544.9 25.2, 770739.1 6277554.9 25.2, 770742.8 6277554.4 25.2, 770742.6 6277553.1 25.2, 770746.3 6277552.6 25.2, 770746.2 6277551.6 25.2, 770748.4 6277551.3 25.2, 770748.6 6277552.3 25.2))
+BATIMENT0000000211120414;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;5.2;20.1;25.3;27.2;20.2;Cadastre;;POLYGON Z ((770709.4 6277547.2 25.2, 770710.3 6277549.5 25.2, 770714.7 6277547.9 25.2, 770713.7 6277545.6 25.2, 770709.4 6277547.2 25.2))
+BATIMENT0000000211120395;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.8;20.2;23.0;23.4;20.2;Cadastre;;POLYGON Z ((770654.8 6277548.6 23, 770652.8 6277546.5 23, 770650.7 6277548.5 23, 770652.6 6277550.5 23, 770654.8 6277548.6 23))
+BATIMENT0000000211120411;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;4.1;21.3;25.4;;;Cadastre;;POLYGON Z ((770748.4 6277551.3 25.4, 770746.2 6277551.6 25.4, 770746.3 6277552.6 25.4, 770748.6 6277552.3 25.4, 770748.4 6277551.3 25.4))
+BATIMENT0000000211120396;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.3;20.2;22.5;22.6;20.2;Cadastre;;POLYGON Z ((770653.4 6277553.2 22.4, 770651.6 6277551.3 22.4, 770650.1 6277552.8 22.4, 770651.8 6277554.6 22.4, 770653.4 6277553.2 22.4))
+BATIMENT0000000211120415;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1900-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;20;10;6.2;21.0;27.2;28.0;21.0;Cadastre;B 0.6;POLYGON Z ((770707.1 6277550.9 27.2, 770710.6 6277559.5 27.2, 770718.1 6277556.7 27.2, 770714.7 6277547.9 27.2, 770710.3 6277549.5 27.2, 770707.1 6277550.9 27.2))
+BATIMENT0000000211120394;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.3;20.2;22.5;23.0;20.2;Cadastre;;POLYGON Z ((770656.5 6277560.1 22.5, 770654 6277557.4 22.5, 770651.6 6277559.5 22.5, 770654.1 6277562.3 22.5, 770656.5 6277560.1 22.5))
+BATIMENT0000000211120287;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;4.4;21.0;25.4;27.0;21.0;Cadastre;;POLYGON Z ((770633 6277561.5 25.4, 770629.2 6277557.4 25.4, 770630.4 6277556.3 25.4, 770628.4 6277554.1 25.4, 770627.5 6277554.8 25.4, 770626.2 6277555.9 25.4, 770632.2 6277562.3 25.4, 770633 6277561.5 25.4))
+BATIMENT0000000211120289;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;4.5;21.1;25.6;28.2;21.1;Cadastre;C 0.6;POLYGON Z ((770636.9 6277565.6 25.6, 770638 6277564.7 25.6, 770640 6277566.9 25.6, 770646.4 6277561 25.6, 770640.5 6277554.6 25.6, 770633 6277561.5 25.6, 770636.9 6277565.6 25.6))
+BATIMENT0000000211120380;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;20.5;26.7;28.7;20.7;Cadastre;A 1.0;POLYGON Z ((770578 6277554.2 26.7, 770573.3 6277558.3 26.7, 770574.2 6277559.3 26.7, 770572 6277561.3 26.7, 770577.5 6277567.4 26.7, 770584.2 6277561.4 26.7, 770578 6277554.2 26.7))
+BATIMENT0000000211120378;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.8;21.0;26.8;28.7;21.0;Cadastre;A 1.0;POLYGON Z ((770570.9 6277573.4 26.8, 770577.5 6277567.4 26.8, 770572 6277561.3 26.8, 770569.8 6277563.3 26.8, 770569 6277562.4 26.8, 770564.7 6277566.3 26.8, 770570.9 6277573.4 26.8))
+BATIMENT0000000211120301;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.2;20.4;Cadastre;C 1.0;POLYGON Z ((770612.4 6277574.2 27.5, 770611.2 6277575.2 27.5, 770609.3 6277573.2 27.5, 770603.2 6277578.8 27.5, 770608.7 6277584.7 27.5, 770616 6277578 27.5, 770612.4 6277574.2 27.5))
+BATIMENT0000000211120299;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.5;20.4;Cadastre;C 1.0;POLYGON Z ((770620.9 6277585.7 27.5, 770618.9 6277583.4 27.5, 770620.1 6277582.3 27.5, 770616 6277578 27.5, 770608.7 6277584.7 27.5, 770614.9 6277591.3 27.5, 770620.9 6277585.7 27.5))
+BATIMENT0000000211120297;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.2;20.3;27.5;28.4;20.4;Cadastre;C 1.0;POLYGON Z ((770620.9 6277597.7 27.4, 770628.2 6277591.1 27.4, 770624.2 6277587 27.4, 770623 6277587.9 27.4, 770620.9 6277585.7 27.4, 770614.9 6277591.3 27.4, 770620.9 6277597.7 27.4))
+BATIMENT0000000211120390;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;6.7;20.6;27.3;29.5;20.7;Cadastre;;POLYGON Z ((770585.2 6277592 27.2, 770582.7 6277589.2 27.2, 770580.3 6277591.5 27.2, 770582.8 6277594.2 27.2, 770585.2 6277592 27.2))
+BATIMENT0000000211120393;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;1.9;20.4;22.3;23.0;20.4;Cadastre;;POLYGON Z ((770609.2 6277593.8 22.2, 770607.1 6277591.6 22.2, 770605.5 6277593.1 22.2, 770607.8 6277595.4 22.2, 770609.2 6277593.8 22.2))
+BATIMENT0000000211120391;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;4.4;20.6;25.0;27.3;20.7;Cadastre;;POLYGON Z ((770582 6277595.1 25, 770579.7 6277592.7 25, 770577.6 6277594.6 25, 770579.8 6277597.2 25, 770582 6277595.1 25))
+BATIMENT0000000211120295;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1961-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;30;10;5.9;21.0;26.9;27.8;21.0;Cadastre;A 1.0;POLYGON Z ((770681.1 6277565.3 26.9, 770682.6 6277563.9 26.9, 770678.5 6277559.6 26.9, 770677.5 6277560.6 26.9, 770675.1 6277558.2 26.9, 770673.6 6277559.6 26.9, 770667.3 6277565.7 26.9, 770673.7 6277572.3 26.9, 770681.1 6277565.3 26.9))
+BATIMENT0000000211120290;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;4.7;21.0;25.7;28.1;21.0;Cadastre;C 0.7;POLYGON Z ((770654 6277565.4 25.7, 770648.4 6277559.2 25.7, 770646.4 6277561 25.7, 770640 6277566.9 25.7, 770642.1 6277569.2 25.7, 770641 6277570.1 25.7, 770644.6 6277574 25.7, 770652 6277567.2 25.7, 770654 6277565.4 25.7))
+BATIMENT0000000211120294;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;30;10;5.9;21.0;26.9;27.8;21.0;Cadastre;A 1.0;POLYGON Z ((770680.1 6277578.8 26.9, 770686.2 6277572.8 26.9, 770684.3 6277570.8 26.9, 770685.3 6277569.8 26.9, 770681.1 6277565.3 26.9, 770673.7 6277572.3 26.9, 770680.1 6277578.8 26.9))
+BATIMENT0000000211120291;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;5.2;21.0;26.2;28.2;21.0;Cadastre;C 0.2;POLYGON Z ((770648.6 6277578.5 26.2, 770649.9 6277577.5 26.2, 770651.8 6277579.6 26.2, 770655.2 6277576.5 26.2, 770658.1 6277573.9 26.2, 770652 6277567.2 26.2, 770644.6 6277574 26.2, 770648.6 6277578.5 26.2))
+BATIMENT0000002000330691;Indifférenciée;Résidentiel;Annexe;Non;En service;2016-11-10 15:17:04;2019-04-08 10:00:52;2014-01-01;2015-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;34.0;6.0;00;00;19.1;18.9;;;;Imagerie aérienne;A 1.0;POLYGON Z ((770724 6277585.2 37.1, 770733.8 6277585.2 37.1, 770733.7 6277587.5 34.8, 770737.9 6277587.5 34.8, 770737.7 6277585.2 38, 770737.7 6277583.6 38, 770742.6 6277583.4 38, 770742.6 6277585.3 38, 770744.4 6277585.3 38, 770744.4 6277587.4 36.9, 770756.4 6277587.3 36.9, 770756.3 6277585.2 37.9, 770756.2 6277569.6 37.9, 770756 6277567.4 36.4, 770740.3 6277567.3 36.4, 770740.3 6277569.3 37.2, 770723.8 6277569.3 37, 770724 6277585.2 37.1))
+BATIMENT0000000211120292;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;5.4;21.0;26.4;28.2;21.0;Cadastre;C 0.6;POLYGON Z ((770661.2 6277582.9 26.4, 770655.2 6277576.5 26.4, 770651.8 6277579.6 26.4, 770649 6277582.3 26.4, 770651.2 6277584.4 26.4, 770650.1 6277585.3 26.4, 770654 6277589.6 26.4, 770661.2 6277582.9 26.4))
+BATIMENT0000000211120293;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;4.9;21.0;25.9;28.2;21.0;Cadastre;C 0.5;POLYGON Z ((770658 6277594 25.9, 770659 6277593 25.9, 770661.1 6277595.2 25.9, 770667.2 6277589.4 25.9, 770661.2 6277582.9 25.9, 770654 6277589.6 25.9, 770658 6277594 25.9))
+BATIMENT0000000211120420;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;25.0;4.0;34;49;13.8;21.0;34.8;;;Cadastre;A 1.0;POLYGON Z ((770762 6277609.6 34.8, 770733.3 6277609.5 34.8, 770733.4 6277621.6 34.8, 770762 6277621.7 34.8, 770762 6277609.6 34.8))
+BATIMENT0000000211120284;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;58.0;6.0;00;00;19.0;21.2;40.2;41.9;21.5;Cadastre;A 1.0;POLYGON Z ((770620 6277667.2 40.2, 770624.7 6277663 40.2, 770625.3 6277663.6 40.2, 770630.7 6277658.7 40.2, 770630.2 6277658.1 40.2, 770640.1 6277649 40.2, 770640.7 6277649.6 40.2, 770646 6277644.6 40.2, 770645.5 6277644 40.2, 770654.8 6277635.2 40.2, 770655.4 6277635.8 40.2, 770660.6 6277631 40.2, 770660.2 6277630.4 40.2, 770669.7 6277621.6 40.2, 770670.2 6277622.1 40.2, 770675.7 6277617.3 40.2, 770675.3 6277616.6 40.2, 770684.7 6277607.8 40.2, 770685.4 6277608.4 40.2, 770690.4 6277603.7 40.2, 770689.9 6277602.9 40.2, 770694.6 6277598.6 40.2, 770688.6 6277592.2 40.2, 770614.1 6277660.7 40.2, 770620 6277667.2 40.2))
+BATIMENT0000000211120319;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;20.0;5.0;40;40;17.2;21.8;39.0;;;Cadastre;C 0.4;POLYGON Z ((770645.8 6277685 39, 770648 6277687.2 39, 770654.7 6277680.8 39, 770655.1 6277681.2 39, 770657.6 6277678.9 39, 770657.3 6277678.3 39, 770670.9 6277665.4 39, 770671.4 6277665.8 39, 770673.9 6277663.6 39, 770673.5 6277663.1 39, 770687.1 6277650.1 39, 770687.6 6277650.7 39, 770689.8 6277648.5 39, 770689.4 6277648 39, 770696.5 6277641.4 39, 770700 6277645 39, 770699.5 6277645.5 39, 770701.8 6277647.7 39, 770702.4 6277647.2 39, 770706.3 6277651.4 39, 770712.6 6277645.4 39, 770701.3 6277633.4 39, 770694.9 6277639.4 39, 770690.6 6277634.9 39, 770639.8 6277682.8 39, 770643.8 6277687 39, 770645.8 6277685 39))
+BATIMENT0000000211120296;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;34;10;7.2;20.3;27.5;28.4;20.4;Cadastre;C 1.0;POLYGON Z ((770633.2 6277598.8 27.4, 770630.8 6277596.3 27.4, 770632 6277595.2 27.4, 770628.2 6277591.1 27.4, 770620.9 6277597.7 27.4, 770627.1 6277604.3 27.4, 770633.2 6277598.8 27.4))
+BATIMENT0000000211120298;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;24;10;7.3;20.3;27.6;28.4;20.5;Cadastre;C 1.0;POLYGON Z ((770640.3 6277604 27.5, 770636.2 6277599.7 27.5, 770635 6277600.8 27.5, 770633.2 6277598.8 27.5, 770627.1 6277604.3 27.5, 770633.1 6277610.6 27.5, 770640.3 6277604 27.5))
+BATIMENT0000000211120300;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.0;20.4;27.4;28.2;20.6;Cadastre;C 0.7;POLYGON Z ((770638.5 6277616.4 27.4, 770644.3 6277611 27.4, 770642.2 6277608.6 27.4, 770643.5 6277607.4 27.4, 770640.3 6277604 27.4, 770633.1 6277610.6 27.4, 770638.5 6277616.4 27.4))
+BATIMENT0000000211120334;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;6.9;20.6;27.5;28.2;20.7;Cadastre;C 1.0;POLYGON Z ((770626.1 6277623.5 27.4, 770625.5 6277622.5 27.4, 770627.3 6277620.8 27.4, 770621.6 6277614.5 27.4, 770615.1 6277620.6 27.4, 770621.7 6277627.6 27.4, 770626.1 6277623.5 27.4))
+BATIMENT0000000211120333;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;4.4;21.4;25.8;28.2;21.4;Cadastre;C 0.8;POLYGON Z ((770615.1 6277620.6 25.8, 770608.5 6277626.7 25.8, 770614.2 6277632.7 25.8, 770616.4 6277630.7 25.8, 770617.2 6277631.7 25.8, 770621.7 6277627.6 25.8, 770615.1 6277620.6 25.8))
+BATIMENT0000000211120331;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;50;10;7.0;20.7;27.7;28.7;20.9;Cadastre;C 0.4;POLYGON Z ((770608.5 6277626.7 27.7, 770606.6 6277628.5 27.7, 770604.7 6277630.3 27.7, 770602 6277632.8 27.7, 770608.5 6277639.8 27.7, 770612.5 6277636 27.7, 770611.8 6277635.1 27.7, 770614.2 6277632.7 27.7, 770608.5 6277626.7 27.7))
+BATIMENT0000000211120332;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;4.8;21.4;26.2;28.5;21.4;Cadastre;C 0.2;POLYGON Z ((770595.8 6277638.6 26.2, 770601.5 6277644.6 26.2, 770603.3 6277642.8 26.2, 770604.4 6277643.7 26.2, 770608.5 6277639.8 26.2, 770602 6277632.8 26.2, 770595.8 6277638.6 26.2))
+BATIMENT0000000211120326;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;3.3;21.0;24.3;27.3;21.3;Cadastre;;POLYGON Z ((770592.1 6277643.7 24.2, 770597.6 6277649.8 24.2, 770600.1 6277647.5 24.2, 770594.5 6277641.6 24.2, 770592.1 6277643.7 24.2))
+BATIMENT0000000211120324;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.6;21.4;28.0;29.0;21.5;Cadastre;A 1.0;POLYGON Z ((770598.5 6277650.7 28, 770597.6 6277649.8 28, 770592.1 6277643.7 28, 770590.6 6277641.8 28, 770584 6277648 28, 770585.6 6277649.7 28, 770592.1 6277656.7 28, 770598.5 6277650.7 28))
+BATIMENT0000000211120320;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;4.2;21.3;25.5;26.8;21.4;Cadastre;;POLYGON Z ((770581.6 6277653.4 25.5, 770579.8 6277651.4 25.5, 770577.4 6277653.8 25.5, 770579.2 6277655.7 25.5, 770581.6 6277653.4 25.5))
+BATIMENT0000000211120419;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2022-09-29 16:55:19;1870-01-01;2021-08-11;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;2.0;;;18.8;22.0;;30.9;22.2;Imagerie aérienne;A 1.0;POLYGON Z ((770760.9 6277673.1 40.8, 770760.1 6277649.4 40.8, 770757.6 6277645.4 40.8, 770745.4 6277645.7 40.8, 770740.1 6277649.1 40.8, 770755.8 6277676 40.8, 770760.9 6277673.1 40.8))
+BATIMENT0000000211120336;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2023-03-22 21:39:07;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;0.0;1.0;00;00;1.9;21.9;23.8;25.8;23.2;Cadastre;C 0.4;POLYGON Z ((770709.8 6277671.6 23.8, 770696.6 6277657.7 23.8, 770644.3 6277707.9 23.8, 770657 6277721.8 23.8, 770709.8 6277671.6 23.8))
+BATIMENT0000000211120317;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;20.0;5.0;40;40;17.2;22.4;39.6;39.6;23.2;Cadastre;C 0.7;POLYGON Z ((770624 6277706.9 39.6, 770623.6 6277707.4 39.6, 770625.6 6277709.4 39.6, 770626 6277708.9 39.6, 770635.7 6277719.4 39.6, 770635.2 6277719.8 39.6, 770637.1 6277721.8 39.6, 770637.6 6277721.3 39.6, 770647.5 6277731.8 39.6, 770647 6277732.3 39.6, 770648.7 6277733.9 39.6, 770649 6277733.5 39.6, 770654.4 6277739.1 39.6, 770661.3 6277732.5 39.6, 770667 6277738.5 39.6, 770672.1 6277733.7 39.6, 770672.7 6277734.4 39.6, 770674.4 6277732.7 39.6, 770673.9 6277732.2 39.6, 770684.6 6277722.1 39.6, 770685.1 6277722.6 39.6, 770686.9 6277721 39.6, 770686.5 6277720.3 39.6, 770697 6277710.4 39.6, 770697.5 6277711 39.6, 770699.7 6277709 39.6, 770699.2 6277708.4 39.6, 770704.6 6277703.3 39.6, 770698.2 6277696.7 39.6, 770661 6277731.9 39.6, 770626.5 6277695.1 39.6, 770619.4 6277701.7 39.6, 770624 6277706.9 39.6))
+BATIMENT0000000211120339;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.4;22.0;Cadastre;A 1.0;POLYGON Z ((770542.7 6277676.8 29.3, 770548.4 6277683.2 29.3, 770550.6 6277681.2 29.3, 770551.7 6277682.2 29.3, 770556.1 6277678.1 29.3, 770549.3 6277670.6 29.3, 770542.7 6277676.8 29.3))
+BATIMENT0000000211120338;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;10;10;7.3;22.0;29.3;29.7;22.0;Cadastre;B 0.6;POLYGON Z ((770539.8 6277679.5 29.3, 770536.4 6277682.7 29.3, 770543.2 6277690.1 29.3, 770547.1 6277686.4 29.3, 770546.1 6277685.2 29.3, 770548.4 6277683.2 29.3, 770542.7 6277676.8 29.3, 770539.8 6277679.5 29.3))
+BATIMENT0000000211120340;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.9;22.1;Cadastre;A 1.0;POLYGON Z ((770536.4 6277682.7 29.3, 770530 6277688.6 29.3, 770535.7 6277694.9 29.3, 770537.9 6277692.9 29.3, 770539 6277694 29.3, 770543.2 6277690.1 29.3, 770536.4 6277682.7 29.3))
+BATIMENT0000000211120342;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.8;22.3;Cadastre;A 1.0;POLYGON Z ((770534.2 6277698 29.3, 770533.4 6277697 29.3, 770535.7 6277694.9 29.3, 770530 6277688.6 29.3, 770523.3 6277694.8 29.3, 770530 6277702.1 29.3, 770534.2 6277698 29.3))
+BATIMENT0000000211120344;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;1.0;;;2.1;22.0;24.1;25.3;22.2;Cadastre;A 0.2;POLYGON Z ((770517.6 6277698.8 24, 770515.3 6277696.4 24, 770515.8 6277696.1 24, 770514.5 6277694.9 24, 770512.9 6277696.5 24, 770516.2 6277700.1 24, 770517.6 6277698.8 24))
+BATIMENT0000000211120343;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;34;10;7.2;22.0;29.2;29.9;22.5;Cadastre;A 0.5;POLYGON Z ((770522.4 6277707 29.2, 770524.8 6277705 29.2, 770525.8 6277706 29.2, 770530 6277702.1 29.2, 770523.3 6277694.8 29.2, 770516.8 6277700.8 29.2, 770521.4 6277706 29.2, 770522.4 6277707 29.2))
+BATIMENT0000000211120401;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1970-01-01;;;;BDParcellaire;5.0;Corrélation;1.0;0.0;1.0;;;7.3;22.0;29.3;34.3;22.2;Cadastre;C 0.2;POLYGON Z ((770571.2 6277707.7 29.2, 770568.3 6277704.4 29.2, 770564.9 6277707.7 29.2, 770567.8 6277710.8 29.2, 770571.2 6277707.7 29.2))
+BATIMENT0000000211120348;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.9;23.1;29.0;30.4;23.1;Cadastre;A 1.0;POLYGON Z ((770515 6277728.7 29, 770521.2 6277723.1 29, 770519.1 6277720.9 29, 770520.3 6277719.6 29, 770516.5 6277715.5 29, 770509.2 6277722.3 29, 770515 6277728.7 29))
+BATIMENT0000000211120347;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;34;10;5.8;23.3;29.1;30.5;23.3;Cadastre;A 1.0;POLYGON Z ((770528.5 6277728.5 29.1, 770524.4 6277724.1 29.1, 770523.2 6277725.3 29.1, 770521.2 6277723.1 29.1, 770515 6277728.7 29.1, 770521.1 6277735.3 29.1, 770528.5 6277728.5 29.1))
+BATIMENT0000000211120345;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;5.5;22.5;28.0;28.9;22.6;Cadastre;;POLYGON Z ((770521.1 6277735.3 28, 770515 6277728.7 28, 770513.7 6277730 28, 770519.6 6277736.6 28, 770521.1 6277735.3 28))
+BATIMENT0000000211120322;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;45;10;6.6;21.4;28.0;28.9;21.5;Cadastre;A 1.0;POLYGON Z ((770581.6 6277653.4 28, 770579.2 6277655.7 28, 770584.7 6277661.8 28, 770586.9 6277659.7 28, 770587.9 6277660.7 28, 770592.1 6277656.8 28, 770592.1 6277656.7 28, 770585.6 6277649.7 28, 770581.6 6277653.4 28))
+BATIMENT0000000211120321;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.5;21.4;27.9;28.9;21.5;Cadastre;A 1.0;POLYGON Z ((770572.7 6277661.7 27.9, 770579.1 6277668.7 27.9, 770583.6 6277664.6 27.9, 770582.7 6277663.6 27.9, 770584.7 6277661.8 27.9, 770579.2 6277655.7 27.9, 770572.7 6277661.7 27.9))
+BATIMENT0000000211120323;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.5;21.4;27.9;29.0;21.6;Cadastre;A 0.9;POLYGON Z ((770572.7 6277661.7 27.9, 770566.1 6277667.9 27.9, 770571.6 6277673.9 27.9, 770573.9 6277671.8 27.9, 770574.7 6277672.7 27.9, 770579.1 6277668.7 27.9, 770572.7 6277661.7 27.9))
+BATIMENT0000000211120325;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2023-03-22 21:39:05;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;2.0;40;10;2.6;21.8;24.5;24.8;22.0;Cadastre;A 0.9;POLYGON Z ((770574.7 6277672.7 24.5, 770573.9 6277671.8 24.5, 770571.6 6277673.9 24.5, 770572.4 6277674.8 24.5, 770574.7 6277672.7 24.5))
+BATIMENT0000000211120285;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;40.0;10.0;00;00;23.2;21.0;44.2;53.3;23.2;Cadastre;C 0.5;POLYGON Z ((770605.2 6277736.1 44.2, 770600.6 6277731.3 44.2, 770601.5 6277730.6 44.2, 770596.9 6277725.8 44.2, 770596.1 6277726.4 44.2, 770586 6277715.9 44.2, 770586.8 6277715.1 44.2, 770582.6 6277710.7 44.2, 770581.8 6277711.3 44.2, 770577 6277706.4 44.2, 770580.2 6277703.5 44.2, 770580.8 6277703.9 44.2, 770585.8 6277699.3 44.2, 770585.4 6277698.7 44.2, 770589.9 6277694.5 44.2, 770590.2 6277694.8 44.2, 770595.2 6277690.1 44.2, 770595.9 6277690.6 44.2, 770600.7 6277686.1 44.2, 770600.2 6277685.6 44.2, 770609.8 6277676.6 44.2, 770610.5 6277677.2 44.2, 770615.6 6277672.6 44.2, 770614.8 6277671.9 44.2, 770620 6277667.2 44.2, 770614.1 6277660.7 44.2, 770569.7 6277701.5 44.2, 770575.6 6277707.9 44.2, 770570.1 6277713.2 44.2, 770598.2 6277742.7 44.2, 770605.2 6277736.1 44.2))
+BATIMENT0000000211120282;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2023-03-22 21:39:07;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;53.0;7.0;10;10;22.3;24.7;47.0;47.0;26.3;Cadastre;C 0.6;POLYGON Z ((770541.6 6277843.5 47, 770547.4 6277849.5 47, 770576.8 6277822.1 47, 770575.2 6277820.3 47, 770616.8 6277781.2 47, 770616.2 6277780.3 47, 770617.3 6277779.2 47, 770616.1 6277777.8 47, 770614.7 6277778.9 47, 770612.2 6277776.2 47, 770637.1 6277753.1 47, 770628.9 6277744.2 47, 770603.9 6277767.3 47, 770608.9 6277772.7 47, 770567.1 6277811.9 47, 770568.7 6277813.7 47, 770539.5 6277841.2 47, 770533.7 6277835.3 47, 770513.2 6277855 47, 770520.9 6277863.2 47, 770541.6 6277843.5 47))
+BATIMENT0000000211120346;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;34;10;5.8;23.3;29.1;30.3;23.3;Cadastre;A 1.0;POLYGON Z ((770527.1 6277741.9 29.1, 770533.3 6277736.2 29.1, 770531.5 6277734.2 29.1, 770532.6 6277733 29.1, 770528.5 6277728.5 29.1, 770521.1 6277735.3 29.1, 770527.1 6277741.9 29.1))
+BATIMENT0000000211120349;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.1;23.1;29.2;30.4;23.1;Cadastre;A 1.0;POLYGON Z ((770540.8 6277741.9 29.2, 770536.5 6277737.2 29.2, 770535.2 6277738.3 29.2, 770533.3 6277736.2 29.2, 770527.1 6277741.9 29.2, 770533.3 6277748.6 29.2, 770540.8 6277741.9 29.2))
+BATIMENT0000000211120351;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;34;10;6.3;23.0;29.3;30.4;23.0;Cadastre;A 1.0;POLYGON Z ((770546.6 6277748.2 29.3, 770544.3 6277745.7 29.3, 770540.8 6277741.9 29.3, 770533.3 6277748.6 29.3, 770532.1 6277749.8 29.3, 770537.9 6277756.2 29.3, 770546.6 6277748.2 29.3))
+BATIMENT0000000211120327;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1975-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;23.0;6.0;50;10;17.9;24.0;41.9;;;Cadastre;C 0.9;POLYGON Z ((770579.2 6277769.6 41.9, 770563.8 6277753.8 41.9, 770555.2 6277762 41.9, 770554.1 6277760.7 41.9, 770554.6 6277760.3 41.9, 770552.6 6277758.1 41.9, 770544.9 6277765.6 41.9, 770548 6277768.7 41.9, 770551 6277765.8 41.9, 770566.6 6277781.7 41.9, 770579.2 6277769.6 41.9))
+BATIMENT0000000211120318;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1975-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;23.0;6.0;50;10;16.7;25.2;41.9;;;Cadastre;C 0.6;POLYGON Z ((770546.9 6277800.2 41.9, 770531.8 6277784.4 41.9, 770519.2 6277796.4 41.9, 770534.5 6277812.3 41.9, 770546.9 6277800.2 41.9))
+BATIMENT0000000211120515;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1972-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;7.0;;;7.5;25.8;33.3;43.5;26.1;Cadastre;C 0.2;POLYGON Z ((770519.7 6277863.6 33.2, 770515.9 6277859.6 33.2, 770513.8 6277861.7 33.2, 770517.5 6277865.6 33.2, 770519.7 6277863.6 33.2))
+BATIMENT0000000211120376;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;43;14;5.7;21.2;26.9;28.7;21.2;Cadastre;A 1.0;POLYGON Z ((770560.1 6277570.4 26.9, 770560.9 6277571.3 26.9, 770558.9 6277573.2 26.9, 770564.3 6277579.3 26.9, 770570.9 6277573.4 26.9, 770564.7 6277566.3 26.9, 770560.1 6277570.4 26.9))
+BATIMENT0000000211120377;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.5;21.5;27.0;28.7;21.5;Cadastre;A 1.0;POLYGON Z ((770557.6 6277585.2 27, 770564.3 6277579.3 27, 770558.9 6277573.2 27, 770556.6 6277575.2 27, 770555.8 6277574.3 27, 770551.5 6277578.2 27, 770557.6 6277585.2 27))
+BATIMENT0000000211120379;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;45;10;5.3;21.8;27.1;28.7;21.8;Cadastre;A 1.0;POLYGON Z ((770557.6 6277591.8 27.1, 770554.4 6277588.1 27.1, 770557.6 6277585.2 27.1, 770551.5 6277578.2 27.1, 770546.8 6277582.4 27.1, 770547.6 6277583.3 27.1, 770545.2 6277585.3 27.1, 770554 6277595 27.1, 770557.6 6277591.8 27.1))
+BATIMENT0000000211120316;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;45;10;6.8;21.1;27.9;28.8;21.3;Cadastre;A 1.0;POLYGON Z ((770539.4 6277601.5 27.9, 770546.2 6277595.4 27.9, 770540.8 6277589.4 27.9, 770538.1 6277591.7 27.9, 770537.3 6277590.8 27.9, 770533.2 6277594.5 27.9, 770539.4 6277601.5 27.9))
+BATIMENT0000000211120315;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1964-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;1.0;40;10;7.0;21.2;28.2;28.9;21.4;Cadastre;A 1.0;POLYGON Z ((770539.4 6277601.5 28.1, 770533.2 6277594.5 28.1, 770528.5 6277598.6 28.1, 770525.5 6277595.3 28.1, 770523.3 6277597.1 28.1, 770532.6 6277607.7 28.1, 770539.4 6277601.5 28.1))
+BATIMENT0000000211120311;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;4.3;22.0;26.3;27.0;22.0;Cadastre;;POLYGON Z ((770524 6277602.7 26.3, 770523 6277601.7 26.3, 770518.7 6277605.7 26.3, 770519.6 6277606.6 26.3, 770524 6277602.7 26.3))
+BATIMENT0000000211120314;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1962-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;04;01;6.9;21.3;28.2;28.9;21.5;Cadastre;C 0.6;POLYGON Z ((770523.3 6277597.1 28.1, 770520.8 6277599.3 28.1, 770523 6277601.7 28.1, 770524 6277602.7 28.1, 770519.6 6277606.6 28.1, 770525.9 6277613.7 28.1, 770526.3 6277613.4 28.1, 770532.6 6277607.7 28.1, 770523.3 6277597.1 28.1))
+BATIMENT0000000211120312;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;4.5;22.0;26.5;;;Cadastre;;POLYGON Z ((770519.6 6277606.6 26.5, 770518.7 6277605.7 26.5, 770514.4 6277609.6 26.5, 770515.2 6277610.5 26.5, 770519.6 6277606.6 26.5))
+BATIMENT0000000231251240;Indifférenciée;Indifférencié;;Non;En service;2010-04-30 12:01:24;2018-02-20 09:16:47;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;;;;;3.2;22.2;;;;Imagerie aérienne;;POLYGON Z ((770526.3 6277613.4 25.4, 770528 6277615.6 24.6, 770534.7 6277610.5 24.9, 770532.6 6277607.7 25.4, 770526.3 6277613.4 25.4))
+BATIMENT0000000211120310;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;40;10;6.7;21.4;28.1;28.8;21.5;Cadastre;A 0.7;POLYGON Z ((770525.9 6277613.7 28, 770519.6 6277606.6 28, 770515.2 6277610.5 28, 770514.4 6277609.6 28, 770511.7 6277606.4 28, 770509.1 6277608.6 28, 770513.5 6277613.7 28, 770519 6277619.9 28, 770525.9 6277613.7 28))
+BATIMENT0000000211120392;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;3.6;21.1;24.7;26.5;21.2;Cadastre;;POLYGON Z ((770558.3 6277616 24.6, 770555.3 6277613.1 24.6, 770552.4 6277616.2 24.6, 770555.3 6277619.1 24.6, 770558.3 6277616 24.6))
+BATIMENT0000000211120276;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire;5.0;Corrélation;1.0;0.0;1.0;;;2.1;21.4;23.5;24.0;21.5;Cadastre;A 0.1;POLYGON Z ((770529.3 6277624.2 23.5, 770527.9 6277622.6 23.5, 770524.9 6277625.2 23.5, 770526.3 6277626.9 23.5, 770529.3 6277624.2 23.5))
+BATIMENT0000000211120277;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.9;21.4;24.3;24.4;21.5;Cadastre;;POLYGON Z ((770530 6277625 24.2, 770529.3 6277624.2 24.2, 770526.3 6277626.9 24.2, 770526.9 6277627.6 24.2, 770530 6277625 24.2))
+BATIMENT0000000211120306;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.7;22.0;27.7;29.3;22.0;Cadastre;C 0.3;POLYGON Z ((770540.8 6277646 27.7, 770535.2 6277639.9 27.7, 770532.8 6277642.1 27.7, 770531.9 6277641 27.7, 770527.4 6277644.9 27.7, 770533.9 6277652.3 27.7, 770540.8 6277646 27.7))
+BATIMENT0000000211120304;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.2;22.0;Cadastre;C 0.3;POLYGON Z ((770533.9 6277652.3 27.8, 770527.4 6277644.9 27.8, 770523.2 6277648.8 27.8, 770524.3 6277649.9 27.8, 770521.7 6277652.2 27.8, 770526.9 6277658.5 27.8, 770529.8 6277655.9 27.8, 770533.9 6277652.3 27.8))
+BATIMENT0000000211120307;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;3.6;21.5;25.1;26.6;21.6;Cadastre;;POLYGON Z ((770531.7 6277658 25, 770535.7 6277654.4 25, 770533.9 6277652.3 25, 770529.8 6277655.9 25, 770531.7 6277658 25))
+BATIMENT0000000211120302;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;43;10;5.8;22.0;27.8;29.3;22.0;Cadastre;C 0.2;POLYGON Z ((770526.9 6277658.5 27.8, 770521.7 6277652.2 27.8, 770519.3 6277654.4 27.8, 770518.2 6277653.1 27.8, 770513.8 6277657.2 27.8, 770520.3 6277664.6 27.8, 770526.9 6277658.5 27.8))
+BATIMENT0000000211120397;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.9;21.6;24.5;26.8;21.7;Cadastre;;POLYGON Z ((770546.5 6277669.3 24.5, 770544.6 6277667 24.5, 770542.4 6277669 24.5, 770544.5 6277671.1 24.5, 770546.5 6277669.3 24.5))
+BATIMENT0000000211120341;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.3;22.0;29.3;29.5;22.0;Cadastre;A 1.0;POLYGON Z ((770556.1 6277678.1 29.3, 770560.1 6277674.4 29.3, 770559 6277673.3 29.3, 770561.3 6277671.1 29.3, 770555.5 6277664.9 29.3, 770549.3 6277670.6 29.3, 770556.1 6277678.1 29.3))
+BATIMENT0000000211120337;Indifférenciée;Annexe;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;1.0;;;4.4;21.7;26.1;26.5;21.8;Cadastre;B 0.4;POLYGON Z ((770538.5 6277672.2 26.1, 770535.7 6277674.8 26.1, 770539.8 6277679.5 26.1, 770542.7 6277676.8 26.1, 770538.5 6277672.2 26.1))
+BATIMENT0000000211120313;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;2.0;21.5;23.5;24.9;21.5;Cadastre;;POLYGON Z ((770511.7 6277606.4 23.5, 770507.5 6277601.7 23.5, 770505 6277603.8 23.5, 770509.1 6277608.6 23.5, 770511.7 6277606.4 23.5))
+BATIMENT0000000211120245;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1968-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;39.0;5.0;30;40;16.3;21.4;37.7;38.0;21.7;Cadastre;A 1.0;POLYGON Z ((770502.1 6277605 37.6, 770498 6277608.3 37.6, 770499 6277609.6 37.6, 770490.8 6277616 37.6, 770492.9 6277618.6 37.6, 770487.1 6277623.3 37.6, 770491.7 6277628.9 37.6, 770479.2 6277638.8 37.6, 770474.6 6277633.3 37.6, 770417.5 6277678.9 37.6, 770424.7 6277687.1 37.6, 770422.5 6277689.2 37.6, 770424.1 6277691.1 37.6, 770424 6277691.3 37.6, 770428.3 6277696.5 37.6, 770430.9 6277694.4 37.6, 770432.3 6277695.8 37.6, 770509.8 6277628 37.6, 770502.3 6277619.2 37.6, 770505.3 6277616.8 37.6, 770508.4 6277620.4 37.6, 770512.4 6277617 37.6, 770505.1 6277608.5 37.6, 770502.1 6277605 37.6))
+BATIMENT0000000211120303;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.0;22.0;Cadastre;C 0.1;POLYGON Z ((770520.3 6277664.6 27.8, 770513.8 6277657.2 27.8, 770509.1 6277661.3 27.8, 770510.2 6277662.5 27.8, 770507.8 6277664.7 27.8, 770513.2 6277670.9 27.8, 770520.3 6277664.6 27.8))
+BATIMENT0000000211120308;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;3.8;21.5;25.3;26.5;21.6;Cadastre;;POLYGON Z ((770502.8 6277667.2 25.3, 770501.4 6277665.5 25.3, 770498.7 6277667.8 25.3, 770500.3 6277669.4 25.3, 770502.8 6277667.2 25.3))
+BATIMENT0000000211120305;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.8;22.0;27.8;29.2;22.0;Cadastre;C 0.3;POLYGON Z ((770506.5 6277676.8 27.8, 770510.1 6277673.6 27.8, 770516.7 6277680.8 27.8, 770519.6 6277678 27.8, 770513.2 6277670.9 27.8, 770507.8 6277664.7 27.8, 770506.8 6277663.7 27.8, 770502.8 6277667.2 27.8, 770500.3 6277669.4 27.8, 770506.5 6277676.8 27.8))
+BATIMENT0000000211120309;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.6;22.0;27.6;28.9;22.0;Cadastre;C 0.1;POLYGON Z ((770506.5 6277676.8 27.6, 770500.3 6277669.4 27.6, 770495.5 6277673.7 27.6, 770496.6 6277674.9 27.6, 770494.4 6277676.9 27.6, 770499.8 6277683 27.6, 770500.8 6277682.1 27.6, 770502.5 6277683.9 27.6, 770505.5 6277681.1 27.6, 770503.7 6277679.3 27.6, 770506.5 6277676.8 27.6))
+BATIMENT0000000211120399;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;1.5;21.7;23.2;24.3;21.8;Cadastre;;POLYGON Z ((770513.8 6277679.1 23.1, 770511.9 6277676.7 23.1, 770510.9 6277677.5 23.1, 770513 6277679.9 23.1, 770513.8 6277679.1 23.1))
+BATIMENT0000000211120402;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;4.7;21.6;26.3;27.2;21.7;Cadastre;;POLYGON Z ((770494.8 6277682.3 26.2, 770492.6 6277680.1 26.2, 770491.8 6277680.9 26.2, 770494 6277683.1 26.2, 770494.8 6277682.3 26.2))
+BATIMENT0000000211120255;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;0.0;2.0;;;5.4;22.7;28.1;29.2;22.7;Cadastre;C 0.3;POLYGON Z ((770493.4 6277687.7 28.1, 770487.8 6277681.4 28.1, 770485.6 6277683.4 28.1, 770484.7 6277682.2 28.1, 770480.3 6277686.1 28.1, 770486.8 6277693.6 28.1, 770493.4 6277687.7 28.1))
+BATIMENT0000000211120398;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.1;21.8;23.9;24.2;21.9;Cadastre;;POLYGON Z ((770503.8 6277688.3 23.8, 770501.7 6277686 23.8, 770500.6 6277687.1 23.8, 770502.7 6277689.4 23.8, 770503.8 6277688.3 23.8))
+BATIMENT0000000211120256;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.4;22.7;28.1;29.3;22.7;Cadastre;C 0.3;POLYGON Z ((770480 6277699.8 28.1, 770486.8 6277693.6 28.1, 770480.3 6277686.1 28.1, 770475.6 6277690.3 28.1, 770476.6 6277691.4 28.1, 770474.3 6277693.4 28.1, 770480 6277699.8 28.1))
+BATIMENT0000000211120400;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.0;21.8;23.8;24.2;22.0;Cadastre;;POLYGON Z ((770492.6 6277699.5 23.8, 770490.4 6277697 23.8, 770489.2 6277698.1 23.8, 770491.4 6277700.6 23.8, 770492.6 6277699.5 23.8))
+BATIMENT0000000211120257;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.5;22.7;28.2;29.3;22.7;Cadastre;C 0.3;POLYGON Z ((770480 6277699.8 28.2, 770474.3 6277693.4 28.2, 770472.2 6277695.4 28.2, 770471.1 6277694.3 28.2, 770466.8 6277698.2 28.2, 770473.3 6277705.8 28.2, 770480 6277699.8 28.2))
+BATIMENT0000000211120258;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;5.5;22.7;28.2;29.4;22.7;Cadastre;C 0.3;POLYGON Z ((770466.8 6277698.2 28.2, 770462 6277702.4 28.2, 770463.1 6277703.6 28.2, 770461 6277705.2 28.2, 770466.7 6277711.7 28.2, 770473.3 6277705.8 28.2, 770466.8 6277698.2 28.2))
+BATIMENT0000000211120251;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;22.9;29.1;30.0;;Cadastre;C 0.3;POLYGON Z ((770454.8 6277712.7 29.1, 770449.1 6277706.2 29.1, 770442.8 6277711.8 29.1, 770444.8 6277714 29.1, 770443.9 6277714.8 29.1, 770447.7 6277719.2 29.1, 770454.8 6277712.7 29.1))
+BATIMENT0000000211120350;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;6.0;23.0;29.0;30.4;23.0;Cadastre;A 1.0;POLYGON Z ((770516.5 6277715.5 29, 770512.7 6277711.5 29, 770511.6 6277712.7 29, 770509.3 6277710.3 29, 770503.1 6277715.8 29, 770509.2 6277722.3 29, 770516.5 6277715.5 29))
+BATIMENT0000000211120273;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2020-05-29 12:14:55;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.0;21.8;23.8;23.8;21.9;Cadastre;;POLYGON Z ((770465.2 6277716.5 23.7, 770464.4 6277715.6 23.7, 770462.9 6277717 23.7, 770463.7 6277717.9 23.7, 770465.2 6277716.5 23.7))
+BATIMENT0000000211120252;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.2;22.9;29.1;30.3;;Cadastre;C 0.3;POLYGON Z ((770461 6277719.5 29.1, 770454.8 6277712.7 29.1, 770447.7 6277719.2 29.1, 770451.4 6277723.3 29.1, 770452.3 6277722.6 29.1, 770454.6 6277725.2 29.1, 770461 6277719.5 29.1))
+BATIMENT0000000211120272;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.8;21.9;24.7;24.7;22.1;Cadastre;;POLYGON Z ((770472.3 6277724.6 24.6, 770470.3 6277722.3 24.6, 770468.8 6277723.6 24.6, 770470.8 6277725.9 24.6, 770472.3 6277724.6 24.6))
+BATIMENT0000000211120253;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.3;22.9;29.2;30.3;22.9;Cadastre;C 0.3;POLYGON Z ((770461 6277719.5 29.2, 770454.6 6277725.2 29.2, 770456.6 6277727.7 29.2, 770455.8 6277728.5 29.2, 770459.6 6277732.6 29.2, 770466.7 6277726.2 29.2, 770461 6277719.5 29.2))
+BATIMENT0000000211120259;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;24.0;6.0;40;40;13.0;22.7;35.7;;;Cadastre;C 0.1;POLYGON Z ((770440.4 6277739.7 35.7, 770400.7 6277694.1 35.7, 770394 6277700 35.7, 770398.6 6277705.2 35.7, 770397.9 6277706 35.7, 770402.4 6277711.1 35.7, 770403.1 6277710.5 35.7, 770411.8 6277720.4 35.7, 770411 6277721 35.7, 770415.8 6277726.3 35.7, 770416.4 6277725.7 35.7, 770424.7 6277735.3 35.7, 770424 6277735.9 35.7, 770428.8 6277741.3 35.7, 770429.3 6277740.8 35.7, 770433.7 6277745.7 35.7, 770440.4 6277739.7 35.7))
+BATIMENT0000000211120208;Eglise;Religieux;;Oui;En service;2008-11-18 15:28:19;;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;6.2;23.0;29.2;;;Cadastre;;POLYGON Z ((770290.2 6277720.8 29.2, 770289.8 6277718.4 29.2, 770264.1 6277723.2 29.2, 770264.6 6277725.6 29.2, 770290.2 6277720.8 29.2))
+BATIMENT0000000211120207;Eglise;Religieux;;Non;En service;2008-11-18 15:28:19;;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;5.9;23.0;28.9;;;Cadastre;;POLYGON Z ((770289.4 6277714.6 28.9, 770289.8 6277718.4 28.9, 770290.2 6277720.8 28.9, 770264.6 6277725.6 28.9, 770260.1 6277726.4 28.9, 770261.6 6277734.4 28.9, 770265.8 6277733.6 28.9, 770292.7 6277728.9 28.9, 770293.1 6277731.4 28.9, 770293.5 6277733.3 28.9, 770302.7 6277725.5 28.9, 770302.1 6277714 28.9, 770289.4 6277714.6 28.9))
+BATIMENT0000000211120206;Eglise;Religieux;;Oui;En service;2008-11-18 15:28:19;;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;5.9;23.0;28.9;;;Cadastre;;POLYGON Z ((770292.7 6277728.9 28.9, 770265.8 6277733.6 28.9, 770266.2 6277735.9 28.9, 770293.1 6277731.4 28.9, 770292.7 6277728.9 28.9))
+BATIMENT0000000211120179;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire;5.0;Corrélation;1.0;1.0;1.0;00;00;3.4;22.7;26.1;26.4;22.8;Cadastre;C 1.0;POLYGON Z ((770275.8 6277747.4 26, 770272.8 6277743.9 26, 770270.6 6277746 26, 770273.6 6277749.4 26, 770275.8 6277747.4 26))
+BATIMENT0000000211120241;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;7.3;22.9;30.2;30.6;23.2;Cadastre;;POLYGON Z ((770396.5 6277742.1 30.2, 770395.6 6277742.8 30.2, 770393.5 6277740.3 30.2, 770394.4 6277739.5 30.2, 770390.7 6277735.2 30.2, 770389.8 6277736 30.2, 770387.5 6277733.5 30.2, 770388.4 6277732.7 30.2, 770384.8 6277728.6 30.2, 770383.9 6277729.2 30.2, 770381.8 6277726.8 30.2, 770382.7 6277726 30.2, 770378.9 6277721.7 30.2, 770376.6 6277723.7 30.2, 770375.4 6277722.3 30.2, 770370 6277726.9 30.2, 770367.7 6277724.2 30.2, 770363.4 6277728 30.2, 770364.5 6277729.3 30.2, 770363.1 6277730.7 30.2, 770364.1 6277732 30.2, 770362.8 6277733.1 30.2, 770365.5 6277736.3 30.2, 770370.8 6277731.5 30.2, 770382.6 6277744.8 30.2, 770380 6277747 30.2, 770382.4 6277749.7 30.2, 770374.1 6277757 30.2, 770374 6277760.2 30.2, 770374.6 6277760.8 30.2, 770372 6277763 30.2, 770329 6277714.3 30.2, 770320.6 6277721.8 30.2, 770319.6 6277720.7 30.2, 770319.8 6277720.3 30.2, 770317 6277717 30.2, 770313.1 6277720.4 30.2, 770365.4 6277780.4 30.2, 770377.9 6277769.6 30.2, 770377 6277768.5 30.2, 770375.2 6277766.5 30.2, 770377.9 6277764.2 30.2, 770379.7 6277766.2 30.2, 770381.1 6277765.1 30.2, 770381.8 6277766.1 30.2, 770386.4 6277762 30.2, 770385.7 6277761.1 30.2, 770387.9 6277759.2 30.2, 770388.8 6277760.1 30.2, 770393.1 6277756.2 30.2, 770392.4 6277755.2 30.2, 770395 6277753 30.2, 770395.8 6277754 30.2, 770400 6277750.4 30.2, 770399 6277749.2 30.2, 770400.1 6277748.3 30.2, 770399 6277747 30.2, 770400.2 6277746.1 30.2, 770396.5 6277742.1 30.2))
+BATIMENT0000000211120240;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;12.9;22.6;35.5;38.8;22.7;Cadastre;;POLYGON Z ((770399 6277747 35.5, 770400.1 6277748.3 35.5, 770399 6277749.2 35.5, 770400 6277750.4 35.5, 770402.1 6277748.5 35.5, 770400.2 6277746.1 35.5, 770399 6277747 35.5))
+BATIMENT0000000211120270;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.0;23.0;25.0;25.7;23.1;Cadastre;;POLYGON Z ((770339.4 6277758.6 24.9, 770337.8 6277756.8 24.9, 770331.7 6277762 24.9, 770333.3 6277763.9 24.9, 770339.4 6277758.6 24.9))
+BATIMENT0000000211120242;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;3.3;23.0;26.3;28.5;23.1;Cadastre;;POLYGON Z ((770379.7 6277766.2 26.2, 770377.9 6277764.2 26.2, 770375.2 6277766.5 26.2, 770377 6277768.5 26.2, 770379.7 6277766.2 26.2))
+BATIMENT0000000211120269;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.4;23.0;25.4;26.0;23.2;Cadastre;;POLYGON Z ((770346.3 6277766.6 25.4, 770344.7 6277764.7 25.4, 770338.7 6277770 25.4, 770340.4 6277771.8 25.4, 770346.3 6277766.6 25.4))
+BATIMENT0000000211120254;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1965-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.3;23.0;29.3;29.9;23.0;Cadastre;C 0.3;POLYGON Z ((770459.6 6277732.6 29.3, 770463.7 6277737.2 29.3, 770464.4 6277736.4 29.3, 770466.4 6277738.6 29.3, 770472.7 6277733 29.3, 770466.7 6277726.2 29.3, 770459.6 6277732.6 29.3))
+BATIMENT0000000211120231;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;4.1;22.2;26.3;27.7;22.5;Cadastre;;POLYGON Z ((770443.7 6277746 26.3, 770441 6277742.9 26.3, 770437.8 6277745.8 26.3, 770440.5 6277748.9 26.3, 770443.7 6277746 26.3))
+BATIMENT0000000211120248;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.0;23.6;30.6;31.0;23.6;Cadastre;C 0.3;POLYGON Z ((770487.1 6277749.3 30.6, 770481.4 6277742.8 30.6, 770474.9 6277748.6 30.6, 770477.1 6277750.9 30.6, 770476 6277751.8 30.6, 770479.8 6277756 30.6, 770487.1 6277749.3 30.6))
+BATIMENT0000000211120249;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;7.0;23.6;30.6;30.8;23.6;Cadastre;C 0.3;POLYGON Z ((770483.6 6277760.3 30.6, 770484.5 6277759.5 30.6, 770486.7 6277761.9 30.6, 770493.1 6277756.2 30.6, 770487.1 6277749.3 30.6, 770479.8 6277756 30.6, 770483.6 6277760.3 30.6))
+BATIMENT0000000211120328;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1967-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;45;13;6.2;24.3;30.5;31.2;;Cadastre;C 0.2;POLYGON Z ((770497.6 6277762 30.5, 770491.2 6277767.7 30.5, 770493.2 6277769.9 30.5, 770492.2 6277770.7 30.5, 770496.1 6277775.1 30.5, 770503.6 6277768.6 30.5, 770497.6 6277762 30.5))
+BATIMENT0000000211120329;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;40;10;6.1;24.3;30.4;31.3;24.3;Cadastre;C 0.3;POLYGON Z ((770496.1 6277775.1 30.4, 770499.9 6277779.5 30.4, 770500.9 6277778.8 30.4, 770502.8 6277781.1 30.4, 770509.3 6277775.3 30.4, 770503.6 6277768.6 30.4, 770496.1 6277775.1 30.4))
+BATIMENT0000000211120250;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1965-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;55.0;4.0;40;40;12.9;24.3;37.2;38.1;25.4;Cadastre;A 1.0;POLYGON Z ((770438.3 6277841.6 37.2, 770413.1 6277812.4 37.2, 770417.9 6277808.1 37.2, 770418.4 6277808.7 37.2, 770423.7 6277804 37.2, 770423.3 6277803.3 37.2, 770432.9 6277794.8 37.2, 770433.5 6277795.5 37.2, 770438.8 6277790.6 37.2, 770438.4 6277790 37.2, 770447.9 6277781.6 37.2, 770448.3 6277782.3 37.2, 770454.2 6277777.2 37.2, 770453.6 6277776.6 37.2, 770458.4 6277772.5 37.2, 770460.6 6277775 37.2, 770459.9 6277775.6 37.2, 770465.7 6277782 37.2, 770466.4 6277781.5 37.2, 770474.4 6277790.6 37.2, 770473.6 6277791.2 37.2, 770479.2 6277797.6 37.2, 770479.9 6277796.9 37.2, 770483.5 6277801 37.2, 770490.1 6277794.8 37.2, 770463.5 6277764.5 37.2, 770456.7 6277770.4 37.2, 770452.5 6277765.5 37.2, 770406.9 6277805.6 37.2, 770411 6277810.3 37.2, 770404.2 6277816.3 37.2, 770408 6277820.8 37.2, 770407.2 6277821.5 37.2, 770413 6277828.1 37.2, 770413.9 6277827.3 37.2, 770421.8 6277836.5 37.2, 770421.1 6277837.3 37.2, 770426.7 6277843.7 37.2, 770427.5 6277842.9 37.2, 770431.5 6277847.6 37.2, 770438.3 6277841.6 37.2))
+BATIMENT0000000211120246;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;22.0;6.0;00;00;16.0;25.6;41.6;42.2;25.6;Cadastre;A 1.0;POLYGON Z ((770510.8 6277827.6 41.6, 770495.9 6277811.8 41.6, 770483.1 6277823.9 41.6, 770498.4 6277839.6 41.6, 770510.8 6277827.6 41.6))
+BATIMENT0000000211120508;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;48.0;6.0;40;40;18.9;26.0;44.9;46.9;26.2;Cadastre;A 1.0;POLYGON Z ((770413 6277896.7 44.9, 770417.6 6277892.3 44.9, 770418.4 6277893 44.9, 770423.2 6277888.5 44.9, 770422.4 6277887.7 44.9, 770432.2 6277878.5 44.9, 770433 6277879.3 44.9, 770437.8 6277874.7 44.9, 770437 6277873.9 44.9, 770446.8 6277864.6 44.9, 770447.5 6277865.5 44.9, 770452.5 6277860.8 44.9, 770451.6 6277860.1 44.9, 770461.2 6277851 44.9, 770462 6277851.8 44.9, 770467 6277847.1 44.9, 770466.3 6277846.2 44.9, 770471.4 6277841.4 44.9, 770465.3 6277835 44.9, 770452.1 6277847 44.9, 770436.6 6277861.5 44.9, 770419.8 6277877.6 44.9, 770406.6 6277890.1 44.9, 770413 6277896.7 44.9))
+BATIMENT0000000211120504;Indifférenciée;Résidentiel;Commercial et services;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;4.0;2.0;15;10;6.8;27.0;33.8;34.0;27.0;Cadastre;C 0.2;POLYGON Z ((770442.6 6277891.6 33.8, 770451.9 6277901.6 33.8, 770459.2 6277894.7 33.8, 770454.1 6277889 33.8, 770467.8 6277876 33.8, 770461.2 6277868.9 33.8, 770442.7 6277886.2 33.8, 770442.6 6277891.6 33.8))
+BATIMENT0000000211120203;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;15.9;23.5;39.4;41.3;23.9;Cadastre;;POLYGON Z ((770213.4 6277782.5 39.4, 770215.1 6277784.3 39.4, 770239.1 6277764 39.4, 770240.3 6277765.3 39.4, 770246.6 6277760.1 39.4, 770235.6 6277747.6 39.4, 770229.3 6277752.9 39.4, 770230.8 6277754.5 39.4, 770206.9 6277774.9 39.4, 770205.2 6277773 39.4, 770190.6 6277785.4 39.4, 770198.9 6277794.6 39.4, 770213.4 6277782.5 39.4))
+BATIMENT0000000211120271;Indifférenciée;Commercial et services;;Oui;En service;2008-11-18 15:28:19;2019-07-29 11:03:24;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;3.2;23.0;26.2;26.5;23.2;Cadastre;;POLYGON Z ((770339.7 6277772 26.1, 770335.6 6277767.3 26.1, 770331.5 6277762.6 26.1, 770326.7 6277766.7 26.1, 770322.1 6277770.8 26.1, 770326 6277775.5 26.1, 770330.2 6277780.3 26.1, 770335.1 6277776.1 26.1, 770339.7 6277772 26.1))
+BATIMENT0000000211120260;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1966-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;43.0;9.0;40;40;21.9;22.7;44.6;51.8;24.3;Cadastre;C 0.7;POLYGON Z ((770353.9 6277828.3 44.5, 770354.4 6277828.9 44.5, 770360.6 6277823.5 44.5, 770360.2 6277822.8 44.5, 770369.3 6277814.7 44.5, 770369.9 6277815.5 44.5, 770376.2 6277809.8 44.5, 770375.6 6277809.2 44.5, 770380 6277805.5 44.5, 770379.7 6277805.2 44.5, 770383.7 6277801.6 44.5, 770384.4 6277802.4 44.5, 770390.8 6277796.7 44.5, 770390.2 6277795.8 44.5, 770398.8 6277788.5 44.5, 770399.4 6277789.2 44.5, 770405.9 6277783.6 44.5, 770405.3 6277782.9 44.5, 770414.3 6277775.1 44.5, 770415 6277775.8 44.5, 770421.1 6277770.4 44.5, 770420.4 6277769.7 44.5, 770424.4 6277766.2 44.5, 770424.7 6277766.4 44.5, 770429.1 6277762.5 44.5, 770429.6 6277763.2 44.5, 770435.9 6277757.6 44.5, 770435.3 6277757 44.5, 770440 6277753 44.5, 770434 6277746.1 44.5, 770342.9 6277825.1 44.5, 770349.3 6277832.4 44.5, 770353.9 6277828.3 44.5))
+BATIMENT0000000211120219;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1978-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;0.0;1.0;;;17.0;23.6;40.6;40.8;24.1;Cadastre;C 0.2;POLYGON Z ((770264.2 6277770.9 40.6, 770259.7 6277774.5 40.6, 770271.1 6277787.9 40.6, 770270.1 6277788.9 40.6, 770271.6 6277790.6 40.6, 770260.3 6277800.3 40.6, 770259.2 6277799 40.6, 770232.5 6277822.3 40.6, 770232.4 6277822.8 40.6, 770229.7 6277825.4 40.6, 770232.5 6277828.4 40.6, 770235.4 6277826 40.6, 770240.5 6277832 40.6, 770267.3 6277808.5 40.6, 770268.3 6277809.6 40.6, 770279.9 6277799.5 40.6, 770281.2 6277801.1 40.6, 770287.6 6277795.5 40.6, 770276 6277782.2 40.6, 770279.8 6277778.9 40.6, 770269.1 6277766.7 40.6, 770264.2 6277770.9 40.6))
+BATIMENT0000000211120464;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;7.1;25.0;32.1;32.7;25.0;Cadastre;;POLYGON Z ((770267.4 6277853.2 32.1, 770265.6 6277854.8 32.1, 770268.3 6277857.8 32.1, 770270 6277856.3 32.1, 770267.4 6277853.2 32.1))
+BATIMENT0000000211120465;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;2007-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;0.0;1.0;;;3.7;25.0;28.7;32.4;25.2;Cadastre;C 0.5;POLYGON Z ((770301.2 6277869.1 28.7, 770300.2 6277868 28.7, 770301.1 6277867 28.7, 770301.1 6277865 28.7, 770298.4 6277861.9 28.7, 770301.9 6277859 28.7, 770299.7 6277856.4 28.7, 770299.8 6277854.6 28.7, 770298 6277854.5 28.7, 770295.7 6277852 28.7, 770296.1 6277850.4 28.7, 770294.4 6277850.4 28.7, 770292.1 6277847.8 28.7, 770292.3 6277846.1 28.7, 770290.6 6277846.1 28.7, 770288.2 6277843.3 28.7, 770288.4 6277841.6 28.7, 770286.7 6277841.6 28.7, 770282.6 6277837.1 28.7, 770264.1 6277853.3 28.7, 770265.6 6277854.8 28.7, 770267.4 6277853.2 28.7, 770270 6277856.3 28.7, 770274 6277860.8 28.7, 770278.7 6277856.6 28.7, 770285.9 6277864.9 28.7, 770280.2 6277870.1 28.7, 770272.7 6277861.6 28.7, 770270.4 6277861.2 28.7, 770268.4 6277863 28.7, 770268.4 6277864.5 28.7, 770266.2 6277866.4 28.7, 770264.7 6277866.3 28.7, 770262.1 6277868.6 28.7, 770262 6277870 28.7, 770264 6277872.2 28.7, 770265.4 6277872.1 28.7, 770267.6 6277874.6 28.7, 770267.4 6277876 28.7, 770269.4 6277878.3 28.7, 770271.1 6277878.2 28.7, 770273.9 6277875.7 28.7, 770274.8 6277876.8 28.7, 770273.1 6277878.4 28.7, 770274.2 6277879.6 28.7, 770275.9 6277877.9 28.7, 770276.2 6277878.3 28.7, 770279.3 6277878.6 28.7, 770281.5 6277876.6 28.7, 770283.7 6277878.9 28.7, 770287.6 6277878.9 28.7, 770289.6 6277877.3 28.7, 770290.8 6277878.4 28.7, 770288.7 6277880.3 28.7, 770288.4 6277884.1 28.7, 770289.9 6277885.8 28.7, 770288.3 6277887.2 28.7, 770288.1 6277891.9 28.7, 770293.2 6277897.9 28.7, 770305.9 6277887 28.7, 770302.4 6277882.8 28.7, 770310.5 6277875.5 28.7, 770304.3 6277868.6 28.7, 770301.8 6277868.6 28.7, 770301.2 6277869.1 28.7))
+BATIMENT0000000211120488;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 11:33:35;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;3.5;25.0;28.5;28.5;25.0;Cadastre;;POLYGON Z ((770303.1 6277867.4 28.5, 770302.1 6277866.1 28.5, 770301.1 6277867 28.5, 770300.2 6277868 28.5, 770301.2 6277869.1 28.5, 770301.8 6277868.6 28.5, 770303.1 6277867.4 28.5))
+BATIMENT0000000211120487;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;3.5;25.0;28.5;28.9;25.0;Cadastre;;POLYGON Z ((770290.8 6277878.4 28.5, 770289.6 6277877.3 28.5, 770287.6 6277878.9 28.5, 770288.7 6277880.3 28.5, 770290.8 6277878.4 28.5))
+BATIMENT0000002275435066;Indifférenciée;Résidentiel;;Oui;En service;2021-12-09 16:30:40;2023-03-22 21:39:05;;;DGFiP;;BDParcellaire;5.0;Corrélation;1.0;;;;;3.2;24.9;28.1;30.6;25.2;Cadastre;;POLYGON Z ((770281.6 6277879.6 28.1, 770276.1 6277879.4 28.1, 770274.6 6277880.8 28.1, 770277 6277883.4 28.1, 770278.9 6277881.7 28.1, 770284 6277887.4 28.1, 770286.6 6277885.1 28.1, 770281.6 6277879.6 28.1))
+BATIMENT0000000211120511;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1963-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;40.0;4.0;40;40;13.3;25.9;39.2;40.0;26.0;Cadastre;A 1.0;POLYGON Z ((770335.3 6277930.4 39.2, 770336 6277930.9 39.2, 770341.2 6277926.4 39.2, 770340.7 6277925.8 39.2, 770350.8 6277917 39.2, 770351.3 6277917.7 39.2, 770356.3 6277913.2 39.2, 770355.8 6277912.6 39.2, 770365.7 6277903.8 39.2, 770366.4 6277904.6 39.2, 770371.2 6277900.3 39.2, 770370.6 6277899.7 39.2, 770380.4 6277891 39.2, 770381.1 6277891.7 39.2, 770386.5 6277887 39.2, 770385.9 6277886.3 39.2, 770396 6277877.7 39.2, 770396.6 6277878.4 39.2, 770402 6277873.7 39.2, 770401.4 6277873 39.2, 770406.4 6277868.7 39.2, 770400.8 6277862.1 39.2, 770324.3 6277928.5 39.2, 770329.8 6277935.1 39.2, 770335.3 6277930.4 39.2))
+BATIMENT0000000211120486;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire;5.0;Corrélation;1.0;;;;;2.6;26.2;28.8;29.0;26.6;Cadastre;;POLYGON Z ((770478.1 6277882.4 28.8, 770469.8 6277890.4 28.8, 770470.9 6277891.6 28.8, 770479.4 6277883.8 28.8, 770478.1 6277882.4 28.8))
+BATIMENT0000000211120522;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1957-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;2.0;2.0;15;10;7.6;26.4;34.0;34.8;27.0;Cadastre;A 1.0;POLYGON Z ((770506.4 6277891.3 34, 770499.5 6277884 34, 770492.3 6277890.9 34, 770499.2 6277898.4 34, 770506.4 6277891.3 34))
+BATIMENT0000000211120502;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1957-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;2.0;2.0;50;10;5.9;27.9;33.8;35.4;27.9;Cadastre;A 1.0;POLYGON Z ((770494.6 6277904.4 33.8, 770484 6277893 33.8, 770476.8 6277899.8 33.8, 770487.4 6277911.2 33.8, 770494.6 6277904.4 33.8))
+BATIMENT0000000211120505;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1958-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;6.0;3.0;15;10;10.3;27.8;38.1;39.8;27.9;Cadastre;A 1.0;POLYGON Z ((770480.4 6277917.9 38.1, 770473.7 6277910.8 38.1, 770475.8 6277908.7 38.1, 770471.2 6277904 38.1, 770469.3 6277905.7 38.1, 770462.3 6277898.2 38.1, 770454.7 6277905.5 38.1, 770472.9 6277925.1 38.1, 770480.4 6277917.9 38.1))
+BATIMENT0000000211120506;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1972-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;2.0;50;10;5.8;28.0;33.8;35.0;28.0;Cadastre;A 1.0;POLYGON Z ((770436.5 6277913.2 33.8, 770428.1 6277904.4 33.8, 770420.3 6277911.7 33.8, 770428.7 6277920.7 33.8, 770436.5 6277913.2 33.8))
+BATIMENT0000000211120503;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1953-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;3.0;2.0;10;10;9.2;27.6;36.8;38.0;28.4;Cadastre;A 1.0;POLYGON Z ((770452.5 6277936.1 36.8, 770447.9 6277931.2 36.8, 770447 6277932 36.8, 770444.9 6277929.7 36.8, 770436.8 6277937.1 36.8, 770443.6 6277944.2 36.8, 770452.5 6277936.1 36.8))
+BATIMENT0000000211120510;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1982-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;3.0;2.0;10;10;7.4;26.6;34.0;35.2;;Cadastre;A 1.0;POLYGON Z ((770313.5 6277912.6 34, 770314.5 6277913.7 34, 770327.3 6277902.4 34, 770320.2 6277893.9 34, 770304.1 6277908 34, 770310.5 6277915.2 34, 770313.5 6277912.6 34))
+BATIMENT0000000211120477;Indifférenciée;Commercial et services;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;2007-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;0.0;1.0;;;12.8;25.1;37.9;44.5;25.7;Cadastre;C 0.4;POLYGON Z ((770282.2 6277918 37.9, 770270 6277904.1 37.9, 770256.3 6277916.2 37.9, 770268.5 6277930 37.9, 770282.2 6277918 37.9))
+BATIMENT0000000211120509;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;54.0;9.0;00;00;21.3;26.9;48.2;54.4;26.9;Cadastre;A 1.0;POLYGON Z ((770362.9 6277931 48.2, 770361.9 6277929.9 48.2, 770347 6277944.2 48.2, 770353.5 6277951.2 48.2, 770358.2 6277946.8 48.2, 770359.1 6277947.3 48.2, 770363.8 6277942.7 48.2, 770363.3 6277942.1 48.2, 770373.2 6277932.8 48.2, 770373.8 6277933.5 48.2, 770378.7 6277929 48.2, 770378 6277928.4 48.2, 770387.8 6277919.4 48.2, 770388.5 6277920 48.2, 770393.4 6277915.3 48.2, 770392.9 6277914.7 48.2, 770397.5 6277910.4 48.2, 770398 6277910.9 48.2, 770402.7 6277906.4 48.2, 770403.5 6277907.2 48.2, 770408.9 6277902 48.2, 770408.2 6277901.4 48.2, 770413 6277896.7 48.2, 770406.6 6277890.1 48.2, 770362.9 6277931 48.2))
+BATIMENT0000000211120507;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1850-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;10;10;6.9;25.5;32.4;32.9;25.9;Cadastre;A 1.0;POLYGON Z ((770317.4 6277922.2 32.3, 770313.3 6277917.5 32.3, 770303.2 6277926.4 32.3, 770303.7 6277927.1 32.3, 770301.8 6277928.8 32.3, 770305.1 6277932.9 32.3, 770317.4 6277922.2 32.3))
+BATIMENT0000000231251324;Indifférenciée;Annexe;;Non;En service;2010-04-30 12:01:24;2019-04-08 10:00:52;1999-01-01;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;0.0;1.0;00;00;4.6;26.5;;39.0;28.1;Imagerie aérienne;C 0.3;POLYGON Z ((770411.8 6277932.9 30.6, 770404.3 6277925.1 30.9, 770398.5 6277931.1 30.9, 770405.9 6277938.6 31, 770411.8 6277932.9 30.6))
+BATIMENT0000000211120491;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2018-02-20 09:16:47;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;;;;;4.6;28.2;32.8;;;Cadastre;;POLYGON Z ((770408.7 6277947.4 32.8, 770405.5 6277943.9 32.8, 770404.8 6277944.8 32.8, 770407.9 6277948.2 32.8, 770408.7 6277947.4 32.8))
+BATIMENT0000000211120482;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;12.1;25.9;38.0;43.0;26.1;Cadastre;;POLYGON Z ((770274.9 6277951 38, 770280 6277946.7 38, 770275.6 6277941.4 38, 770269.6 6277946.5 38, 770274.9 6277951 38))
+BATIMENT0000000211120492;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2023-03-22 21:39:05;1986-01-01;;;;BDParcellaire recalée;3.0;Corrélation;1.0;1.0;2.0;23;10;7.4;26.6;34.0;35.1;28.1;Cadastre;A 1.0;POLYGON Z ((770404.8 6277944.8 34, 770405.5 6277943.9 34, 770400.6 6277938.4 34, 770394.2 6277944.6 34, 770399.1 6277949.8 34, 770398.3 6277950.6 34, 770401.6 6277954 34, 770407.9 6277948.2 34, 770404.8 6277944.8 34))
+BATIMENT0000000211120497;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1954-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;2.0;2.0;00;00;6.9;28.3;35.2;37.4;29.0;Cadastre;C 0.7;POLYGON Z ((770437.2 6277949.5 35.2, 770424.6 6277936.1 35.2, 770416.3 6277943.9 35.2, 770428.8 6277957.4 35.2, 770437.2 6277949.5 35.2))
+BATIMENT0000000211120483;Indifférenciée;Indifférencié;;Non;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;10.8;26.0;36.8;43.3;26.2;Cadastre;;POLYGON Z ((770284.1 6277951.2 36.7, 770280 6277946.7 36.7, 770274.9 6277951 36.7, 770279.2 6277955.2 36.7, 770284.1 6277951.2 36.7))
+BATIMENT0000000211120484;Indifférenciée;Commercial et services;Résidentiel;Non;En service;2008-11-18 15:28:19;2019-07-29 11:03:18;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;9.0;5.0;01;01;9.6;26.1;35.7;38.3;26.5;Cadastre;C 0.1;POLYGON Z ((770290.8 6277966.9 35.6, 770296.2 6277961.9 35.6, 770286.2 6277949.4 35.6, 770284.1 6277951.2 35.6, 770279.2 6277955.2 35.6, 770278.2 6277956.2 35.6, 770288.5 6277967.3 35.6, 770290.8 6277966.9 35.6))
+BATIMENT0000000211120496;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;2.0;2.0;00;00;7.2;28.9;36.1;37.6;29.5;Cadastre;A 1.0;POLYGON Z ((770413.7 6277969 36.1, 770416.4 6277971.7 36.1, 770422.5 6277965.6 36.1, 770416 6277958.3 36.1, 770407 6277967 36.1, 770407.2 6277967.2 36.1, 770409.2 6277969.4 36.1, 770411.2 6277971.5 36.1, 770413.7 6277969 36.1))
+BATIMENT0000000211120494;Indifférenciée;Indifférencié;;Oui;En service;2008-11-18 15:28:19;2017-03-30 10:33:07;;;;;BDParcellaire recalée;3.0;Corrélation;1.0;;;;;2.9;29.2;32.1;32.3;29.5;Cadastre;;POLYGON Z ((770405.4 6277968.8 32, 770407.5 6277971 32, 770409.2 6277969.4 32, 770407.2 6277967.2 32, 770405.4 6277968.8 32))
+BATIMENT0000000211120495;Indifférenciée;Résidentiel;Annexe;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1952-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;3.0;2.0;10;10;6.3;28.9;35.2;37.7;29.7;Cadastre;A 1.0;POLYGON Z ((770411 6277976.4 35.2, 770404.3 6277968.9 35.2, 770391.3 6277981.4 35.2, 770398 6277988.7 35.2, 770411 6277976.4 35.2))
+BATIMENT0000000211120498;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:28:19;2019-04-08 10:00:52;1956-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;1.0;50;10;7.2;28.6;35.8;;;Cadastre;A 1.0;POLYGON Z ((770392.4 6277992 35.8, 770378.6 6277977.2 35.8, 770370.8 6277984.4 35.8, 770384.7 6277999.2 35.8, 770392.4 6277992 35.8))
+BATIMENT0000000211117722;Indifférenciée;Résidentiel;;Non;En service;2008-11-18 15:26:42;2019-04-08 10:00:52;1973-01-01;;;;BDParcellaire recalée;3.0;Interpolation bâti BDTopo;2.5;1.0;1.0;40;10;8.4;28.6;37.0;38.7;29.4;Cadastre;A 1.0;POLYGON Z ((770378.3 6278003.2 37, 770376.9 6278001.6 37, 770380.4 6277998.5 37, 770370.9 6277988.2 37, 770363.6 6277995 37, 770374.5 6278006.7 37, 770378.3 6278003.2 37))
 """)
         return GeoDataFrameLib.read_csv(_sio)
 
     @staticmethod
     def irisTastavinRoads():
         '''
         # SOURCE:
         # https://geoservices.ign.fr/bdtopo
-        from geopandas import clip
+        from geopandas import clip, read_file
 
         iris = GeoDataFrameDemosC.irisTastavin()
-        roads = read_file("/home/tleduc/data/bdtopo/BDTOPO_3-0_TOUSTHEMES_SHP_LAMB93_D034_2022-03-15/\
-BDTOPO/1_DONNEES_LIVRAISON_2022-03-00081/BDT_3-0_SHP_LAMB93_D034-ED2022-03-15/TRANSPORT/TRONCON_DE_ROUTE.shp", mask=iris)
+        roads = read_file("/home/tleduc/data/bdtopo/\
+BDTOPO_3-3_TOUSTHEMES_SHP_LAMB93_D034_2023-09-15/BDTOPO/\
+1_DONNEES_LIVRAISON_2023-09-00196/BDT_3-3_SHP_LAMB93_D034-ED2023-09-15/\
+TRANSPORT/TRONCON_DE_ROUTE.shp", mask=iris)
         roads = clip(roads, iris, keep_geom_type=True)
         roads.to_csv('/tmp/tastavin.csv', sep=';', index=False)
         '''
-        _sio = StringIO("""ID;NATURE;NOM_1_G;NOM_1_D;NOM_2_G;NOM_2_D;IMPORTANCE;FICTIF;POS_SOL;ETAT;DATE_CREAT;DATE_MAJ;DATE_APP;DATE_CONF;SOURCE;ID_SOURCE;PREC_PLANI;PREC_ALTI;NB_VOIES;LARGEUR;IT_VERT;PRIVE;SENS;CYCLABLE;BUS;URBAIN;VIT_MOY_VL;ACCES_VL;ACCES_PED;FERMETURE;NAT_RESTR;RESTR_H;RESTR_P;RESTR_PPE;RESTR_LAR;RESTR_LON;RESTR_MAT;BORNEDEB_G;BORNEDEB_D;BORNEFIN_G;BORNEFIN_D;INSEECOM_G;INSEECOM_D;TYP_ADRES;ALIAS_G;ALIAS_D;C_POSTAL_G;C_POSTAL_D;DATE_SERV;ID_VOIE_G;ID_VOIE_D;ID_RN;ID_ITI;NUMERO;NUM_EUROP;CL_ADMIN;GESTION;TOPONYME;ITI_CYCL;VOIE_VERTE;NATURE_ITI;NOM_ITI;geometry
-TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;Métrique;;;34070;34070;;341720797;341720797;;;;;;;;;;;;LINESTRING Z (770660.7 6277485.2 20.4, 770668 6277478.8 20)
-TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;Métrique;;;34070;34070;;341720797;341720797;;;;;;;;;;;;LINESTRING Z (770668 6277478.8 20, 770674.8 6277475.7 19.3)
-TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;Métrique;;;34070;34070;;341720797;341720797;;;;;;;;;;;;LINESTRING Z (770674.8 6277475.7 19.3, 770691 6277470.2 19)
-TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;Métrique;;;34070;34070;;341720797;341720797;;;;;;;;;;;;LINESTRING Z (770691 6277470.2 19, 770691.9 6277470.5 19)
-TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;Métrique;;;34070;34070;;341720797;341720797;;;;;;;;;;;;LINESTRING Z (770691.9 6277470.5 19, 770692.6 6277472.4 19, 770698.8 6277490.2 19.9, 770699.7 6277491.3 19.9, 770702.3 6277491.6 19.9, 770760.1 6277469.4 19.9)
-TRONROUT0000000240978829;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-03 16:10:28;;2009-07-01;;;2.5;1.5;1.0;4.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1392;;1356;;34172;34172;Classique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770651.3720822622 6277488.083804627 20.3, 770657.1 6277499.8 20.3)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770563.5 6277547.7 20.9, 770565.8 6277545.8 20.7)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770565.8 6277545.8 20.7, 770596.3 6277521.8 20.4)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770596.3 6277521.8 20.4, 770620.1 6277502.4 20.4)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770620.1 6277502.4 20.4, 770625.6 6277499 20)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770625.6 6277499 20, 770630.9 6277496.6 20)
-TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770630.9 6277496.6 20, 770636.6 6277495.3 20, 770641.5 6277494.8 20, 770647.6 6277495 20, 770652.5 6277496.8 20.2, 770657.1 6277499.8 20.3)
-TRONROUT0000000240978882;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1356;;1278;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770657.1 6277499.8 20.3, 770657.8 6277500.3 20.3, 770661 6277504.3 20.5, 770668.2 6277515.5 20.8, 770689.1 6277557.1 20.9, 770695 6277572.2 20.9)
-TRONROUT0000000240978676;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2012-01-10 08:59:00;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;1285;1376;1285;1182;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770660.7 6277485.2 20.4, 770663 6277486.5 20.4, 770670 6277492.2 20.5, 770674.4 6277496.7 20.5, 770677.4 6277501.2 20.5, 770678.5 6277502.8 20.5, 770681.1 6277508.2 20.4, 770685.3 6277518.3 20.1, 770688.8 6277527.4 20.1, 770698.1 6277550.8 20.1, 770706 6277571.8 20.3, 770714.4 6277597.3 20.7, 770724.9 6277629.8 20.9, 770729.6 6277641.6 21.1, 770733.7 6277650.4 21.3, 770737.9 6277659 21.4, 770741.6 6277665.2 21.4)
-TRONROUT0000000044845894;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;1;;1;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770686.4 6277580.7 20.7, 770695 6277572.2 20.9)
-TRONROUT0000000240978838;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;1268;;1278;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770699.6 6277584.1 20.9, 770696.2 6277575.3 20.9, 770695 6277572.2 20.9)
-TRONROUT0000000240978103;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770695.6 6277583 20.7, 770690.9 6277581.4 20.7, 770686.4 6277580.7 20.7)
-TRONROUT0000000044845857;Route à 1 chaussée;IMP JULES VERNE;IMP JULES VERNE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;12;11;2;1;34172;34172;Classique;;;34070;34070;;341723097;341723097;;;;;;;;;;;;LINESTRING Z (770620.4 6277569.7 23, 770655 6277609.9 21.8)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770447 6277630.6 22.5, 770455 6277627 22.5)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770455 6277627 22.5, 770459.4 6277626.2 21.5)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770459.4 6277626.2 21.5, 770465.2 6277624 21.5)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770465.2 6277624 21.5, 770470.4 6277621.3 21.6)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770470.4 6277621.3 21.6, 770475.5 6277617.9 21.6)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770475.5 6277617.9 21.6, 770482.2 6277612.5 21.7)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770482.2 6277612.5 21.7, 770509.4 6277591.1 21.8)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770509.4 6277591.1 21.8, 770556.7 6277553.7 21.4)
-TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2006-12-12 11:20:44;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770556.7 6277553.7 21.4, 770563.5 6277547.7 20.9)
-TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2007-12-13 12:17:21;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;30;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770420.2 6277653.1 22.5)
-TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2007-12-13 12:17:21;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;30;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770420.2 6277653.1 22.5, 770442.6 6277635.1 22.5)
-TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2007-12-13 12:17:21;2011-11-29 13:48:16;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;30;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770442.6 6277635.1 22.5, 770447 6277630.6 22.5)
-TRONROUT0000000044845873;Route à 1 chaussée;R DE CAMARGUE;R DE CAMARGUE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;19;10;34172;34172;Classique;;;34070;34070;;341720933;341720933;;;;;;;;;;;;LINESTRING Z (770426.4 6277714.1 22.6, 770467.4 6277677.1 22.1, 770521.1 6277629 22.3)
-TRONROUT0000000044845823;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:04:00;;;;;20.0;2.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;12;;8;;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770522 6277709.8 23.3, 770534.9 6277723.6 23.3)
-TRONROUT0000000240977666;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;31;;33;;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770546 6277713.1 23.1, 770534.9 6277723.6 23.3)
-TRONROUT0000000044845917;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:04:00;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;8;;2;;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770546 6277713.1 23.1, 770556.5 6277728 23.6, 770557 6277730.3 23.1, 770555.1 6277733.3 22.5, 770551.6 6277735.8 22.5, 770548.9 6277735.6 22.5, 770546.3 6277734.8 22.5, 770534.9 6277723.6 23.3)
-TRONROUT0000000044845915;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2006-12-12 11:20:44;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;45;44;95;94;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770426.4 6277714.1 22.6, 770455.2 6277747.4 23)
-TRONROUT0000000240978819;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;3;;3;34172;34172;Classique;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770655 6277609.9 21.8, 770685.7 6277581.4 20.7, 770686.4 6277580.7 20.7)
-TRONROUT0000000044845900;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1266;;1246;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770706.2 6277605.4 20.9)
-TRONROUT0000000201934075;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2008-07-30 13:46:27;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1246;;1182;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770706.2 6277605.4 20.9, 770707 6277607.9 20.9, 770716.8 6277638.1 20.9, 770721.5 6277652 21.4, 770723.9 6277658.6 21.6, 770725.4 6277664.6 21.6, 770725.7 6277668.6 21.6, 770725.6 6277669.6 21.6)
-TRONROUT0000000044845937;Route à 1 chaussée;R MONGE;R MONGE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;6;13;2;1;34172;34172;Classique;;;34070;34070;;341723782;341723782;;;;;;;;;;;;LINESTRING Z (770604.3 6277698.1 23.4, 770634.4 6277671.1 21, 770688.6 6277620.4 20.4, 770701.7 6277609.7 20.6, 770706.2 6277605.4 20.9)
-TRONROUT0000000240977790;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-05-18 13:10:15;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770781.0810751509 6277670.824410313 24.003784969834356, 770781.6 6277663.3 23.9)
-TRONROUT0000000240977790;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-05-18 13:10:15;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770781.6 6277663.3 23.9, 770782.2 6277618.8 24.1)
-TRONROUT0000000240977790;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-05-18 13:10:15;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770782.2 6277618.8 24.1, 770781.4 6277587 24.1, 770781.5 6277586.8 24.1)
-TRONROUT0000000044845902;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;5;;29;;34172;34172;Linéaire;;;34070;34070;;341724123;341724123;;;;;;;;;;;;LINESTRING Z (770655 6277609.9 21.8, 770546 6277713.1 23.1)
-TRONROUT0000000201934073;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2008-07-30 13:46:27;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770741.6 6277665.2 21.4, 770734.2 6277666.6 21.5, 770728.4 6277667.7 21.5, 770725.6 6277669.6 21.6)
-TRONROUT0000000240977939;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1138;;1183;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770721.3573665497 6277698.415444838 21.772811387814933, 770724.9 6277694.7 21.6, 770728 6277689.4 21.4, 770730.3 6277683.3 21.5, 770732.3 6277678 21.6, 770734.9 6277673.2 21.5, 770741.6 6277665.2 21.4)
-TRONROUT0000000044845890;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;1182;;1138;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770725.6 6277669.6 21.6, 770725 6277674 21.7, 770723.3 6277681.5 21.7, 770720.1 6277690.7 21.9, 770717.1 6277696.6 22.1, 770713.7 6277702 22.3, 770709.7 6277706.8 22.5, 770704.3 6277712.2 23.2)
-TRONROUT0000000044845909;Route à 1 chaussée;R JOSEPH CUGNOT;R JOSEPH CUGNOT;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341723061;341723061;;;;;;;;;;;;LINESTRING Z (770741.6 6277665.2 21.4, 770745.5 6277670.5 21.4, 770748.9 6277675.4 21.8, 770749.0770886724 6277675.71875961 21.81416709377949)
-TRONROUT0000000240978879;Route à 1 chaussée;R MONGE;R MONGE;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;8;17;8;15;34172;34172;Classique;;;34070;34070;;341723782;341723782;;;;;;;;;;;;LINESTRING Z (770610.6 6277723.7 23.9, 770597.6 6277711.6 22.9, 770596.4 6277708.9 22.9, 770596.3 6277706.5 22.9, 770597.6 6277703.5 22.9, 770604.3 6277698.1 23.4)
-TRONROUT0000000240978477;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-10-05 19:17:23;;2009-07-01;;;2.5;1.5;2.0;5.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770630.8 6277726.6 22.8, 770613 6277707.5 22.6, 770604.3 6277698.1 23.4)
-TRONROUT0000000240977856;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-10-05 19:17:23;;2009-07-01;;;2.5;1.5;2.0;5.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770622 6277735.1 23.1, 770630.8 6277726.6 22.8)
-TRONROUT0000000240978941;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2012-01-10 13:27:39;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;1138;1139;1062;1063;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770704.3 6277712.2 23.2, 770694.9 6277721.9 24.3)
-TRONROUT0000000240978941;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2012-01-10 13:27:39;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;1138;1139;1062;1063;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770694.9 6277721.9 24.3, 770661.1 6277755.6 24.8)
-TRONROUT0000000044845832;Route à 1 chaussée;R MONGE;R MONGE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;14;;12;;34172;34172;Classique;;;34070;34070;;341723782;341723782;;;;;;;;;;;;LINESTRING Z (770661.1 6277755.6 24.8, 770634 6277730.1 22.8, 770630.8 6277726.6 22.8)
-TRONROUT0000000240977948;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2010-07-16 14:01:58;2012-01-10 11:17:24;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770661.1 6277755.6 24.8, 770657.3 6277759.3 24.9)
-TRONROUT0000000044845860;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:17:24;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;989;990;1063;1062;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770613.2 6277802.6 25.5, 770657.3 6277759.3 24.9)
-TRONROUT0000000044845868;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:17:24;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;990;989;938;937;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770613.2 6277802.6 25.5, 770567.4 6277845.2 27.3)
-TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770590.5 6277857.2 26.6, 770592.7 6277838.7 27)
-TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770592.7 6277838.7 27, 770598.6 6277821.6 26.4)
-TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770598.6 6277821.6 26.4, 770604.9 6277810.8 26.1)
-TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770604.9 6277810.8 26.1, 770613.2 6277802.6 25.5)
-TRONROUT0000000044845908;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2006-12-12 11:20:44;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;95;94;151;150;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770455.2 6277747.4 23, 770503 6277802.8 24.6)
-TRONROUT0000000044845889;Route à 1 chaussée;R LAVOISIER;R LAVOISIER;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;4;;6;34172;34172;Classique;;;34070;34070;;341723202;341723202;;;;;;;;;;;;LINESTRING Z (770527.6 6277831.3 24.4, 770596.3 6277766.3 24.2, 770597.9 6277764 24.2, 770598.2 6277760.8 23.9, 770598.9 6277757.6 23.8, 770622 6277735.1 23.1)
-TRONROUT0000000044845907;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2006-12-12 11:20:44;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;159;160;199;200;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770503 6277802.8 24.5, 770521.1 6277823.3 25.3, 770525.4 6277828.6 25.2, 770527.6 6277831.3 24.4)
-TRONROUT0000000044845896;Route à 1 chaussée;R LAVOISIER;R LAVOISIER;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;2;;2;;34172;34172;Classique;;;34070;34070;;341723202;341723202;;;;;;;;;;;;LINESTRING Z (770527.6 6277831.3 24.4, 770496 6277864.5 26)
-TRONROUT0000000044845879;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770567.4 6277845.2 27.3, 770565.9 6277852.4 26.6)
-TRONROUT0000000044845811;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:05:14;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;938;937;924;925;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770567.4 6277845.2 27.3, 770558.7 6277853.7 26.9)
-TRONROUT0000000044845920;Route à 1 chaussée;;;;;4;Non;0;En service;2006-12-12 11:20:44;;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770565.9 6277852.4 26.6, 770571 6277852.2 27)
-TRONROUT0000000044845920;Route à 1 chaussée;;;;;4;Non;0;En service;2006-12-12 11:20:44;;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770571 6277852.2 27, 770579.2 6277854 27)
-TRONROUT0000000044845920;Route à 1 chaussée;;;;;4;Non;0;En service;2006-12-12 11:20:44;;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770579.2 6277854 27, 770588.8 6277857.2 27.8)
-TRONROUT0000000044845920;Route à 1 chaussée;;;;;4;Non;0;En service;2006-12-12 11:20:44;;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770588.8 6277857.2 27.8, 770590.5 6277857.2 26.6)
-TRONROUT0000000044845888;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:05:14;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;924;925;886;887;34172;34172;Métrique;;;34000;34000;;341723665;341723665;;;;;;;;;;;;LINESTRING Z (770558.7 6277853.7 26.9, 770531.7 6277882.3 27.3)
-TRONROUT0000000044845837;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;37;38;117;118;34172;34172;Métrique;;;34070;34070;;341725252;341725252;;;;;;;;;;;;LINESTRING Z (770496 6277864.5 26.1, 770492.6 6277866.7 26.8, 770489.7 6277867.9 26.8, 770486.7 6277868.3 26.8, 770482.7 6277867.4 26.8, 770475.2 6277862.9 26.8, 770470.7 6277861.4 26.8, 770468.5 6277860.9 26.8, 770466.2 6277861.4 26.8, 770464.1 6277862.8 26.8, 770432.7 6277891.8 27.2)
-TRONROUT0000000044845826;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;38;37;2;1;34172;34172;Métrique;;;34070;34070;;341725252;341725252;;;;;;;;;;;;LINESTRING Z (770496 6277864.5 26.1, 770523 6277891.6 27.8)
-TRONROUT0000000044845940;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:05:14;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;;55A;;55;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770531.7 6277882.3 27.3, 770523 6277891.6 27.8)
-TRONROUT0000000044845916;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 12:06:40;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;55;34;55;38;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770523 6277891.6 27.8)
-TRONROUT0000000044845891;Route à 1 chaussée;R SAINTE-MONIQUE;R SAINTE-MONIQUE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;5;2;34172;34172;Classique;;;34070;34070;;341725248;341725248;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770432.7 6277891.8 27.2)
-TRONROUT0000000044843639;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 12:06:40;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770465.6 6277945.3 28.8)
-TRONROUT0000000044843690;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:08:40;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;32;53;26B;51;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770465.6 6277945.3 28.8, 770417.4 6277990.6 29)
-TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770394.3 6277674.2 22.8)
-TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770394.3 6277674.2 22.8, 770392 6277676.3 22.8)
-TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770392 6277676.3 22.8, 770388.2 6277679.9 22.9)
-TRONROUT0000000044845895;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2006-12-12 11:20:44;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770396.9 6277676.3 23, 770396.8 6277680.8 22.8)
-TRONROUT0000000240978435;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2010-07-16 14:01:58;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770396.8 6277680.8 22.8, 770392.8 6277680.6 22.9, 770388.2 6277679.9 22.9)
-TRONROUT0000000240978812;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;30;Libre;;;;;;;;;Non;283;284;297;296;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770379.9 6277682.4 22.5, 770384.7 6277681.3 22.9)
-TRONROUT0000000240978812;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;30;Libre;;;;;;;;;Non;283;284;297;296;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770384.7 6277681.3 22.9, 770388.1 6277680 22.9, 770388.2 6277679.9 22.9)
-TRONROUT0000000109698644;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2007-12-13 12:17:21;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;269;268;283;284;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770367.7 6277691.9 22.7, 770379.9 6277682.4 22.5)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770343.3 6277697.3 22.3, 770346.6 6277697.1 22.2)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770346.6 6277697.1 22.2, 770354.1 6277696.4 22)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770354.1 6277696.4 22, 770358.4 6277695.9 22.7)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770358.4 6277695.9 22.7, 770361.1 6277695.5 22.7)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770361.1 6277695.5 22.7, 770365.3 6277693.2 22.7)
-TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770365.3 6277693.2 22.7, 770367.7 6277691.9 22.7)
-TRONROUT0000000240978935;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;;;5;Non;0;En service;2010-07-16 14:01:58;2013-12-04 12:46:34;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;45;44;34172;34172;Métrique;;;34070;34070;;341722579;341722579;;;;;;;;;;;;LINESTRING Z (770396.8 6277680.8 22.8, 770425 6277712.5 22.6, 770426.4 6277714.1 22.6)
-TRONROUT0000000044845871;Route à 1 chaussée;R SAINT-JACQUES;R SAINT-JACQUES;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;94;93;2;1;34172;34172;Métrique;;;34070;34070;;341725126;341725126;;;;;;;;;;;;LINESTRING Z (770384.3 6277810.1 24.3, 770399.8 6277797.1 23.7, 770442.3 6277758.6 23.4, 770453.9 6277748.4 23.2, 770455.2 6277747.4 23)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770243 6277721.5 22.4, 770247 6277717.6 22.4)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770247 6277717.6 22.4, 770259 6277707.7 22.1)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770259 6277707.7 22.1, 770272.5 6277701.8 22)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770272.5 6277701.8 22, 770287.9 6277699.7 22)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770287.9 6277699.7 22, 770304.6 6277699 21.9)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770304.6 6277699 21.9, 770330.3 6277697.9 22.3)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770330.3 6277697.9 22.3, 770338.6 6277697.6 22.5)
-TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770338.6 6277697.6 22.5, 770343.3 6277697.3 22.3)
-TRONROUT0000000201979444;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;123;122;135;136;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770233.1 6277731 22.4, 770243 6277721.5 22.4)
-TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770216 6277746.4 22.1, 770222.5 6277740.9 22.1)
-TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770222.5 6277740.9 22.1, 770228.9 6277735 22.4)
-TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770228.9 6277735 22.4, 770233.1 6277731 22.4)
-TRONROUT0000000240978930;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;63;64;99;100;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770187.9 6277771.8 23.1, 770205.4 6277756.6 23.1)
-TRONROUT0000000240978930;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;63;64;99;100;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770205.4 6277756.6 23.1, 770216 6277746.4 22.1)
-TRONROUT0000000044845846;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;2;103;104;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770243 6277721.5 23.5, 770276.5 6277759.2 20.4, 770315.6 6277804 16.3)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770139.6 6277792.9 24.5, 770145.1 6277791.3 24.1)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770145.1 6277791.3 24.1, 770153.7 6277786.7 23.5)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770153.7 6277786.7 23.5, 770166.2 6277780.4 23.5)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770166.2 6277780.4 23.5, 770168.2 6277779.5 23.5)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770168.2 6277779.5 23.5, 770174 6277776.9 23.5)
-TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;2;;62;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770174 6277776.9 23.5, 770187.9 6277771.8 23.1)
-TRONROUT0000000201979451;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;61;;1;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770187.9 6277771.8 23.1, 770187.1 6277772.4 23.1, 770180.1 6277777.8 23.2, 770171.6 6277783.7 23.4, 770171.4 6277783.9 23.4, 770156.3 6277792.2 23.4, 770146.1 6277798.5 23.5, 770140.1 6277800.9 23.2, 770135.2 6277802.7 24.7)
-TRONROUT0000000240978464;Route à 1 chaussée;;;;;5;Non;0;En service;2010-07-16 14:01:58;2015-10-05 19:17:23;;2009-07-01;;;2.5;1.5;2.0;5.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770387.4 6277814.2 24.7, 770384.3 6277810.1 24.3)
-TRONROUT0000000115739992;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2008-02-08 11:05:31;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770387.4 6277814.2 24.7, 770396.3 6277825.7 24.8)
-TRONROUT0000000044845899;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;103;104;159;158;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770315.6 6277804 24.6, 770348.4 6277840.6 25.3)
-TRONROUT0000000044845821;Route à 1 chaussée;R SAINT-JACQUES;R SAINT-JACQUES;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;140;141;94;93;34172;34172;Métrique;;;34070;34070;;341725126;341725126;;;;;;;;;;;;LINESTRING Z (770348.4 6277840.6 25.3, 770375.9 6277817 24.6, 770384.3 6277810.1 24.3)
-TRONROUT0000000044845912;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;3;;1;34172;34172;Linéaire;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770396.3 6277825.7 24.8, 770407.7 6277840.4 24.9)
-TRONROUT0000000115739993;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2008-02-08 11:05:31;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770396.3 6277825.7 24.8, 770361 6277854.7 25.4)
-TRONROUT0000000240977397;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770348.4 6277840.6 25.3, 770352.4 6277845 25.4)
-TRONROUT0000000115739991;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2008-02-08 11:05:31;2012-01-10 15:17:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;;1;;34172;34172;Classique;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770398.6 6277848.6 25, 770407.7 6277840.4 24.9)
-TRONROUT0000000044845822;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;172;171;158;159;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770361 6277854.7 25.4, 770357.6 6277850.9 25.4, 770352.4 6277845 25.4)
-TRONROUT0000000115739990;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2008-02-08 11:05:31;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770407.7 6277840.4 24.9, 770408.9 6277842 24.9, 770423.3 6277860 25.1)
-TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770124.6 6277788.2 25.3, 770131.4 6277791.3 24.1)
-TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770131.4 6277791.3 24.1, 770136.8 6277792.7 24.1)
-TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770136.8 6277792.7 24.1, 770139.6 6277792.9 24.5)
-TRONROUT0000000201979450;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2012-02-13 09:03:26;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;618;619;600;601;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770124.6 6277788.2 25.3, 770131 6277797.1 25.5)
-TRONROUT0000000201979450;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2012-02-13 09:03:26;;;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;618;619;600;601;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770131 6277797.1 25.5, 770135.2 6277802.7 24.7)
-TRONROUT0000000240979102;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;;;5;Non;0;En service;2010-07-16 14:01:58;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341724240;341724240;;;;;;;;;;;;LINESTRING Z (770135.2 6277802.7 24.7, 770139.6 6277792.9 24.5)
-TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;601;;553;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770135.2 6277802.7 24.7, 770142 6277809.5 24.9)
-TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;601;;553;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770142 6277809.5 24.9, 770154 6277828.2 24.6)
-TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;601;;553;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770154 6277828.2 24.6, 770157.4 6277834.7 24.6)
-TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;601;;553;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770157.4 6277834.7 24.6, 770158.5 6277837.4 25.2)
-TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-07-31 11:14:36;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;1.0;3.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;601;;553;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770158.5 6277837.4 25.2, 770159.4 6277843.5 25.2)
-TRONROUT0000000044845854;Route à 1 chaussée;PL DU CARDINAL VERDIER;PL DU CARDINAL VERDIER;;;5;Non;0;En service;2006-12-12 11:20:44;2012-08-10 15:40:49;;;;;2.5;1.5;2.0;5.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;82;;82;;34172;34172;Classique;;;34070;34070;;341721028;341721028;;;;;;;;;;;;LINESTRING Z (770194.3 6277798.2 25.8, 770247 6277860.6 25.3, 770315.6 6277804 24.6)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770165 6277907.9 25.3, 770163.4 6277904.6 24.9)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770163.4 6277904.6 24.9, 770162.3 6277901.2 24.9)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770162.3 6277901.2 24.9, 770161.9 6277897.5 24.9)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770161.9 6277897.5 24.9, 770162.7 6277881.3 25.4)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770162.7 6277881.3 25.4, 770163.2 6277869.2 25.4)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770163.2 6277869.2 25.4, 770162.8 6277863.6 25.4)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770162.8 6277863.6 25.4, 770162.6 6277857.5 25.3)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770162.6 6277857.5 25.3, 770162.4 6277852 25.3)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770162.4 6277852 25.3, 770161.7 6277848.2 25.3)
-TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2010-07-16 14:01:58;2012-02-13 09:14:16;;2009-07-01;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770161.7 6277848.2 25.3, 770159.4 6277843.5 25.2)
-TRONROUT0000000116207180;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770165 6277907.9 25.3, 770171 6277914.5 25.5, 770178.8 6277920.7 25.6, 770183.4 6277923.8 25.6, 770188.3 6277925.9 25.3)
-TRONROUT0000000116207179;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;455;454;487;488;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770181.8 6277936.8 25.3, 770173.7 6277925.2 25.3)
-TRONROUT0000000116207179;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;455;454;487;488;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770173.7 6277925.2 25.3, 770169.4 6277918.3 25.2)
-TRONROUT0000000116207179;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2011-09-09 10:59:41;;;;;2.5;1.5;1.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;455;454;487;488;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770169.4 6277918.3 25.2, 770165 6277907.9 25.3)
-TRONROUT0000000116207183;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770188.3 6277925.9 25.3, 770191.4 6277926.3 25.3, 770192.4 6277927.2 25.3)
-TRONROUT0000000116207185;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770220.4 6277928.8 25.7, 770211.5 6277927.7 25.3, 770205.1 6277927.7 25.3, 770199.2 6277927.9 25.3, 770192.4 6277927.2 25.3)
-TRONROUT0000000116207188;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770181.8 6277936.8 25.3, 770181.1 6277933.6 25.3, 770181.6 6277930.6 25.3, 770183.2 6277927.9 25.3, 770185.5 6277926.4 25.3, 770188.3 6277925.9 25.3)
-TRONROUT0000000116207186;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770192.4 6277927.2 25.3, 770193.5 6277928 25.3, 770195 6277930.4 25.3, 770195.7 6277933.6 25.3, 770195.4 6277937 25.3, 770193.9 6277939.4 25.3)
-TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2018-09-04 13:53:19;;;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770220.4 6277928.8 25.7, 770212.1 6277930.6 25.8)
-TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2018-09-04 13:53:19;;;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770212.1 6277930.6 25.8, 770205 6277933.1 25.7)
-TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2018-09-04 13:53:19;;;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770205 6277933.1 25.7, 770199.7 6277935.8 25.7)
-TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2008-02-15 13:40:18;2018-09-04 13:53:19;;;;;2.5;1.5;2.0;4.0;Non;Non;Sens direct;;;Oui;40;Libre;;;;;;;;;Non;;;;;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770199.7 6277935.8 25.7, 770193.9 6277939.4 25.3)
-TRONROUT0000000116207182;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770185.5 6277940 25.3, 770183.4 6277938.9 25.3)
-TRONROUT0000000116207182;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770183.4 6277938.9 25.3, 770181.8 6277936.8 25.3)
-TRONROUT0000000116207181;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770193.9 6277939.4 25.3, 770191.3 6277940.6 25.3)
-TRONROUT0000000116207181;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770191.3 6277940.6 25.3, 770188.4 6277940.9 25.3)
-TRONROUT0000000116207181;Rond-point;;;;;4;Non;0;En service;2008-02-15 13:40:18;2017-10-26 14:33:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens direct;;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770188.4 6277940.9 25.3, 770185.5 6277940 25.3)
-TRONROUT0000000294020592;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;;;5;Non;0;En service;2012-01-10 15:17:41;;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;1;;1;;34172;34172;Classique;;;34070;34070;;341724933;341724933;;;;;;;;;;;;LINESTRING Z (770374.5 6277870 25.6, 770398.6 6277848.6 25)
-TRONROUT0000000115739995;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2008-02-08 11:05:31;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;192;191;172;171;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770374.5 6277870 25.6, 770361 6277854.7 25.4)
-TRONROUT0000000115739994;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;;;5;Non;0;En service;2008-02-08 11:05:31;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;198;197;192;191;34172;34172;Métrique;;;34070;34070;;341720134;341720134;;;;;;;;;;;;LINESTRING Z (770378.3 6277874.3 25.6, 770374.5 6277870 25.6)
-TRONROUT0000000294020591;Route à 1 chaussée;;;;;5;Non;0;En service;2012-01-10 15:17:41;2018-04-27 03:14:23;;;;;3.0;0.5;1.0;3.0;Non;Non;Sens direct;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;;;;;;;;;;;;;;LINESTRING Z (770398.6 6277848.6 25.1, 770413.5 6277867.8 25.7, 770340.7 6277935 26.5, 770326.2 6277940.2 26.7, 770314.1 6277935 26.6, 770312.1 6277933.1 26.6)
-TRONROUT0000000044845877;Route à 1 chaussée;LES ORMEAUX 2;LES ORMEAUX 2;;;5;Non;0;En service;2006-12-12 11:20:44;2012-06-08 17:25:28;;;;;2.5;1.5;2.0;4.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;Classique;;;;;;34172#03X;34172#03X;;;;;;;;;;;;LINESTRING Z (770312.1 6277933.1 27.1, 770378.5 6277874.6 25.6, 770378.3 6277874.3 25.6)
-TRONROUT0000000044845858;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;;;;2.5;1.5;2.0;7.0;Non;Non;Double sens;;;Oui;30;Libre;;;;;;;;;Non;117;118;219;218;34172;34172;Métrique;;;34070;34070;;341725252;341725252;;;;;;;;;;;;LINESTRING Z (770432.7 6277891.8 27.2, 770354.3 6277964 27.8, 770351.2 6277966.4 27.8, 770341.5 6277969.7 27.4)
-TRONROUT0000000044845878;Route empierrée;ALL MAURICE BONAFOS;ALL MAURICE BONAFOS;;;5;Non;0;En service;2006-12-12 11:20:44;2011-09-09 10:59:41;;2009-07-01;;;2.5;1.5;;;Non;Non;Double sens;;;Oui;0;Restreint aux ayants droit;;;;;;;;;Non;;135;;135;34172;34172;Classique;;;34070;34070;;341723668;341723668;;;;;;;;;;;;LINESTRING Z (770305.9 6277957.2 26.7, 770375.7 6278029.7 29.3)
-TRONROUT0000000044843696;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:08:40;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;45;20;49;26B;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770375.7 6278029.7 29.3, 770417.4 6277990.6 29)
-TRONROUT0000000044843668;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;;;4;Non;0;En service;2006-12-12 11:20:44;2012-01-10 11:08:40;;;;;2.5;1.5;2.0;6.0;Non;Non;Double sens;;;Oui;40;Libre;;;;;;;;;Non;45;;45;;34172;34172;Classique;;;34070;34070;;341725055;341725055;;;;;;;;;;;;LINESTRING Z (770364.7 6278040.1 29.5, 770375.7 6278029.7 29.3)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770364.7 6278040.1 29.5, 770350.1 6278030.6 29.6)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770350.1 6278030.6 29.6, 770321.9 6278006.7 28.1)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770321.9 6278006.7 28.1, 770307.5 6277994.6 27.9)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770307.5 6277994.6 27.9, 770295.5 6277983 27)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770295.5 6277983 27, 770265.8 6277950.8 26.2)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770265.8 6277950.8 26.2, 770258.3 6277943.6 26.2)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770258.3 6277943.6 26.2, 770250.8 6277938 26.2)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770250.8 6277938 26.2, 770243.4 6277933.9 26.2)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770243.4 6277933.9 26.2, 770236.9 6277931.3 26.1)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770236.9 6277931.3 26.1, 770228.5 6277929.7 25.8)
-TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;;;4;Non;0;En service;2006-12-12 11:20:44;2012-02-13 09:17:20;;;;;2.5;1.5;2.0;5.0;Non;Non;Sens inverse;;;Oui;40;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;Métrique;;;34070;34070;;341725850;341725850;;;;;;;;;;;;LINESTRING Z (770228.5 6277929.7 25.8, 770220.4 6277928.8 25.7)
+        _sio = StringIO("""ID;NATURE;NOM_COLL_G;NOM_COLL_D;IMPORTANCE;FICTIF;POS_SOL;ETAT;DATE_CREAT;DATE_MAJ;DATE_APP;DATE_CONF;SOURCE;ID_SOURCE;ACQU_PLANI;PREC_PLANI;ACQU_ALTI;PREC_ALTI;NB_VOIES;LARGEUR;IT_VERT;PRIVE;SENS;BUS;URBAIN;VIT_MOY_VL;ACCES_VL;ACCES_PED;FERMETURE;NAT_RESTR;RESTR_H;RESTR_P;RESTR_PPE;RESTR_LAR;RESTR_LON;RESTR_MAT;BORNEDEB_G;BORNEDEB_D;BORNEFIN_G;BORNEFIN_D;INSEECOM_G;INSEECOM_D;ALIAS_G;ALIAS_D;DATE_SERV;ID_VOIE_G;ID_VOIE_D;ID_RN;ID_ITI;NUMERO;NUM_EUROP;CL_ADMIN;GESTION;TOPONYME;ITI_CYCL;VOIE_VERTE;NATURE_ITI;NOM_ITI;DELESTAGE;SRC_BAN_G;SRC_BAN_D;NOM_BAN_G;NOM_BAN_D;LD_BAN_G;LD_BAN_D;ID_BAN_G;ID_BAN_D;SENS_CYC_G;SENS_CYC_D;CYCLABLE_G;CYCLABLE_D;RETOURDFCI;GAB_DFCI;IMPAS_DFCI;NDET_DFCI;OALIM_DFCI;PTMAX_DFCI;PISTE_DFCI;DFCI_DEBRO;DFCI_FOSSE;SENS_DFCI;TERR_DFCI;VIT_DFCI;CROIS_DFCI;geometry
+TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;;;;341720797;341720797;;;;;;;;;;;;;commune;commune;Allée du Boulingrin;Allée du Boulingrin;;;34172_0797;34172_0797;;;;;;;;;;;;;;;;;;LINESTRING Z (770660.7 6277485.2 20.4, 770668 6277478.8 20)
+TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;;;;341720797;341720797;;;;;;;;;;;;;commune;commune;Allée du Boulingrin;Allée du Boulingrin;;;34172_0797;34172_0797;;;;;;;;;;;;;;;;;;LINESTRING Z (770668 6277478.8 20, 770674.8 6277475.7 19.3)
+TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;;;;341720797;341720797;;;;;;;;;;;;;commune;commune;Allée du Boulingrin;Allée du Boulingrin;;;34172_0797;34172_0797;;;;;;;;;;;;;;;;;;LINESTRING Z (770674.8 6277475.7 19.3, 770691 6277470.2 19)
+TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;;;;341720797;341720797;;;;;;;;;;;;;commune;commune;Allée du Boulingrin;Allée du Boulingrin;;;34172_0797;34172_0797;;;;;;;;;;;;;;;;;;LINESTRING Z (770691 6277470.2 19, 770691.9 6277470.5 19)
+TRONROUT0000000044847977;Route à 1 chaussée;ALL DU BOULINGRIN;ALL DU BOULINGRIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;141;140;34172;34172;;;;341720797;341720797;;;;;;;;;;;;;commune;commune;Allée du Boulingrin;Allée du Boulingrin;;;34172_0797;34172_0797;;;;;;;;;;;;;;;;;;LINESTRING Z (770691.9 6277470.5 19, 770692.6 6277472.4 19, 770698.8 6277490.2 19.9, 770699.7 6277491.3 19.9, 770702.3 6277491.6 19.9, 770760.1 6277469.4 19.9)
+TRONROUT0000000240978829;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;4.0;Non;Non;Sens inverse;;Oui;30;Libre;;;;;;;;;Non;1392;;1356;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770651.3720822622 6277488.083804627 20.3, 770657.1 6277499.8 20.3)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770563.5 6277547.7 20.9, 770565.8 6277545.8 20.7)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770565.8 6277545.8 20.7, 770596.3 6277521.8 20.4)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770596.3 6277521.8 20.4, 770620.1 6277502.4 20.4)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770620.1 6277502.4 20.4, 770625.6 6277499 20)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770625.6 6277499 20, 770630.9 6277496.6 20)
+TRONROUT0000000044848012;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;515;516;631;630;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770630.9 6277496.6 20, 770636.6 6277495.3 20, 770641.5 6277494.8 20, 770647.6 6277495 20, 770652.5 6277496.8 20.2, 770657.1 6277499.8 20.3)
+TRONROUT0000000240978882;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;35;Libre;;;;;;;;;Non;1356;;1278;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770657.1 6277499.8 20.3, 770657.8 6277500.3 20.3, 770661 6277504.3 20.5, 770668.2 6277515.5 20.8, 770689.1 6277557.1 20.9, 770695 6277572.2 20.9)
+TRONROUT0000000240978676;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;35;Libre;;;;;;;;;Non;1285;1376;1285;1182;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770660.7 6277485.2 20.4, 770663 6277486.5 20.4, 770670 6277492.2 20.5, 770674.4 6277496.7 20.5, 770677.4 6277501.2 20.5, 770678.5 6277502.8 20.5, 770681.1 6277508.2 20.4, 770685.3 6277518.3 20.1, 770688.8 6277527.4 20.1, 770698.1 6277550.8 20.1, 770706 6277571.8 20.3, 770714.4 6277597.3 20.7, 770724.9 6277629.8 20.9, 770729.6 6277641.6 21.1, 770733.7 6277650.4 21.3, 770737.9 6277659 21.4, 770741.6 6277665.2 21.4)
+TRONROUT0000000044845894;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;1;;1;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770686.4 6277580.7 20.7, 770695 6277572.2 20.9)
+TRONROUT0000000240978838;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;1268;;1278;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770699.6 6277584.1 20.9, 770696.2 6277575.3 20.9, 770695 6277572.2 20.9)
+TRONROUT0000000240978103;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770695.6 6277583 20.7, 770690.9 6277581.4 20.7, 770686.4 6277580.7 20.7)
+TRONROUT0000000044845857;Route à 1 chaussée;IMP JULES VERNE;IMP JULES VERNE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;12;11;2;1;34172;34172;;;;341723097;341723097;;;;;;;;;;;;;commune;commune;Impasse Jules Verne;Impasse Jules Verne;;;34172_3097;34172_3097;;;;;;;;;;;;;;;;;;LINESTRING Z (770620.4 6277569.7 23, 770655 6277609.9 21.8)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770447 6277630.6 22.5, 770455 6277627 22.5)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770455 6277627 22.5, 770459.4 6277626.2 21.5)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770459.4 6277626.2 21.5, 770465.2 6277624 21.5)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770465.2 6277624 21.5, 770470.4 6277621.3 21.6)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770470.4 6277621.3 21.6, 770475.5 6277617.9 21.6)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770475.5 6277617.9 21.6, 770482.2 6277612.5 21.7)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770482.2 6277612.5 21.7, 770509.4 6277591.1 21.8)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770509.4 6277591.1 21.8, 770556.7 6277553.7 21.4)
+TRONROUT0000000044845913;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;369;370;515;516;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770556.7 6277553.7 21.4, 770563.5 6277547.7 20.9)
+TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2007-12-13 12:17:21;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;20;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770420.2 6277653.1 22.5)
+TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2007-12-13 12:17:21;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;20;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770420.2 6277653.1 22.5, 770442.6 6277635.1 22.5)
+TRONROUT0000000109698649;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2007-12-13 12:17:21;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;20;Libre;;;;;;;;;Non;297;296;369;368;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770442.6 6277635.1 22.5, 770447 6277630.6 22.5)
+TRONROUT0000000044845873;Route à 1 chaussée;R DE CAMARGUE;R DE CAMARGUE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;19;10;34172;34172;;;;341720933;341720933;;;;;;;;;;;;;commune;commune;Rue de Camargue;Rue de Camargue;;;34172_0933;34172_0933;;;;;;;;;;;;;;;;;;LINESTRING Z (770426.4 6277714.1 22.6, 770467.4 6277677.1 22.1, 770521.1 6277629 22.3)
+TRONROUT0000000044845823;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Géoroute;20.0;Z corrigé;2.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;12;;8;;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770522 6277709.8 23.3, 770534.9 6277723.6 23.3)
+TRONROUT0000000240977666;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;31;;33;;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770546 6277713.1 23.1, 770534.9 6277723.6 23.3)
+TRONROUT0000000044845917;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;10;Libre;;;;;;;;;Non;8;;2;;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770546 6277713.1 23.1, 770556.5 6277728 23.6, 770557 6277730.3 23.1, 770555.1 6277733.3 22.5, 770551.6 6277735.8 22.5, 770548.9 6277735.6 22.5, 770546.3 6277734.8 22.5, 770534.9 6277723.6 23.3)
+TRONROUT0000000044845915;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;45;44;95;94;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770426.4 6277714.1 22.6, 770455.2 6277747.4 23)
+TRONROUT0000000240978819;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;3;;3;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770655 6277609.9 21.8, 770685.7 6277581.4 20.7, 770686.4 6277580.7 20.7)
+TRONROUT0000000044845900;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;1266;;1246;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770700 6277585.3 20.9, 770706.2 6277605.4 20.9)
+TRONROUT0000000201934075;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2008-07-30 13:46:27;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;35;Libre;;;;;;;;;Non;1246;;1182;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770706.2 6277605.4 20.9, 770707 6277607.9 20.9, 770716.8 6277638.1 20.9, 770721.5 6277652 21.4, 770723.9 6277658.6 21.6, 770725.4 6277664.6 21.6, 770725.7 6277668.6 21.6, 770725.6 6277669.6 21.6)
+TRONROUT0000000044845937;Route à 1 chaussée;R MONGE;R MONGE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;10;Libre;;;;;;;;;Non;6;13;2;1;34172;34172;;;;341723782;341723782;;;;;;;;;;;;;commune;commune;Rue Monge;Rue Monge;;;34172_3782;34172_3782;;;;;;;;;;;;;;;;;;LINESTRING Z (770604.3 6277698.1 23.4, 770634.4 6277671.1 21, 770688.6 6277620.4 20.4, 770701.7 6277609.7 20.6, 770706.2 6277605.4 20.9)
+TRONROUT0000000240977790;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770781.0810751509 6277670.824410313 24.003784969834356, 770781.6 6277663.3 23.9)
+TRONROUT0000000240977790;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770781.6 6277663.3 23.9, 770782.2 6277618.8 24.1)
+TRONROUT0000000240977790;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770782.2 6277618.8 24.1, 770781.4 6277587 24.1, 770781.5 6277586.8 24.1)
+TRONROUT0000000044845902;Route à 1 chaussée;ALL DU PARC TASTAVIN;ALL DU PARC TASTAVIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;5;;29;;34172;34172;;;;341724123;341724123;;;;;;;;;;;;;commune;commune;Allée du Parc Tastavin;Allée du Parc Tastavin;;;34172_4123;34172_4123;;;;;;;;;;;;;;;;;;LINESTRING Z (770655 6277609.9 21.8, 770546 6277713.1 23.1)
+TRONROUT0000000201934073;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2008-07-30 13:46:27;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770741.6 6277665.2 21.4, 770734.2 6277666.6 21.5, 770728.4 6277667.7 21.5, 770725.6 6277669.6 21.6)
+TRONROUT0000000240977939;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;30;Libre;;;;;;;;;Non;1138;;1183;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770721.3573665497 6277698.415444838 21.772811387814933, 770724.9 6277694.7 21.6, 770728 6277689.4 21.4, 770730.3 6277683.3 21.5, 770732.3 6277678 21.6, 770734.9 6277673.2 21.5, 770741.6 6277665.2 21.4)
+TRONROUT0000000044845890;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;30;Libre;;;;;;;;;Non;1182;;1138;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770725.6 6277669.6 21.6, 770725 6277674 21.7, 770723.3 6277681.5 21.7, 770720.1 6277690.7 21.9, 770717.1 6277696.6 22.1, 770713.7 6277702 22.3, 770709.7 6277706.8 22.5, 770704.3 6277712.2 23.2)
+TRONROUT0000000044845909;Route à 1 chaussée;R JOSEPH CUGNOT;R JOSEPH CUGNOT;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;35;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723061;341723061;;;;;;;;;;;;;commune;commune;Rue Joseph Cugnot;Rue Joseph Cugnot;;;34172_3061;34172_3061;;;;;;;;;;;;;;;;;;LINESTRING Z (770741.6 6277665.2 21.4, 770745.5 6277670.5 21.4, 770748.9 6277675.4 21.8, 770749.0770886724 6277675.71875961 21.81416709377949)
+TRONROUT0000000240978879;Route à 1 chaussée;R MONGE;R MONGE;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;8;17;8;15;34172;34172;;;;341723782;341723782;;;;;;;;;;;;;commune;commune;Rue Monge;Rue Monge;;;34172_3782;34172_3782;;;;;;;;;;;;;;;;;;LINESTRING Z (770610.6 6277723.7 23.9, 770597.6 6277711.6 22.9, 770596.4 6277708.9 22.9, 770596.3 6277706.5 22.9, 770597.6 6277703.5 22.9, 770604.3 6277698.1 23.4)
+TRONROUT0000000240978477;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770630.8 6277726.6 22.8, 770613 6277707.5 22.6, 770604.3 6277698.1 23.4)
+TRONROUT0000000240977856;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770622 6277735.1 23.1, 770630.8 6277726.6 22.8)
+TRONROUT0000000240978941;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;25;Libre;;;;;;;;;Non;1138;1139;1062;1063;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770704.3 6277712.2 23.2, 770694.9 6277721.9 24.3)
+TRONROUT0000000240978941;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;25;Libre;;;;;;;;;Non;1138;1139;1062;1063;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770694.9 6277721.9 24.3, 770661.1 6277755.6 24.8)
+TRONROUT0000000044845832;Route à 1 chaussée;R MONGE;R MONGE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;14;;12;;34172;34172;;;;341723782;341723782;;;;;;;;;;;;;commune;commune;Rue Monge;Rue Monge;;;34172_3782;34172_3782;;;;;;;;;;;;;;;;;;LINESTRING Z (770661.1 6277755.6 24.8, 770634 6277730.1 22.8, 770630.8 6277726.6 22.8)
+TRONROUT0000000240977948;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;30;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770661.1 6277755.6 24.8, 770657.3 6277759.3 24.9)
+TRONROUT0000000044845860;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;30;Libre;;;;;;;;;Non;989;990;1063;1062;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770613.2 6277802.6 25.5, 770657.3 6277759.3 24.9)
+TRONROUT0000000044845868;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;30;Libre;;;;;;;;;Non;990;989;938;937;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770613.2 6277802.6 25.5, 770567.4 6277845.2 27.3)
+TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770590.5 6277857.2 26.6, 770592.7 6277838.7 27)
+TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770592.7 6277838.7 27, 770598.6 6277821.6 26.4)
+TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770598.6 6277821.6 26.4, 770604.9 6277810.8 26.1)
+TRONROUT0000000044845928;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770604.9 6277810.8 26.1, 770613.2 6277802.6 25.5)
+TRONROUT0000000044845908;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;95;94;151;150;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770455.2 6277747.4 23, 770503 6277802.8 24.6)
+TRONROUT0000000044845889;Route à 1 chaussée;R LAVOISIER;R LAVOISIER;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;4;;6;34172;34172;;;;341723202;341723202;;;;;;;;;;;;;commune;commune;Rue Lavoisier;Rue Lavoisier;;;34172_3202;34172_3202;;;;;;;;;;;;;;;;;;LINESTRING Z (770527.6 6277831.3 24.4, 770596.3 6277766.3 24.2, 770597.9 6277764 24.2, 770598.2 6277760.8 23.9, 770598.9 6277757.6 23.8, 770622 6277735.1 23.1)
+TRONROUT0000000044845907;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;159;160;199;200;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770503 6277802.8 24.5, 770521.1 6277823.3 25.3, 770525.4 6277828.6 25.2, 770527.6 6277831.3 24.4)
+TRONROUT0000000044845896;Route à 1 chaussée;R LAVOISIER;R LAVOISIER;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;2;;2;;34172;34172;;;;341723202;341723202;;;;;;;;;;;;;commune;commune;Rue Lavoisier;Rue Lavoisier;;;34172_3202;34172_3202;;;;;;;;;;;;;;;;;;LINESTRING Z (770527.6 6277831.3 24.4, 770496 6277864.5 26)
+TRONROUT0000000044845879;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens inverse;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770567.4 6277845.2 27.3, 770565.9 6277852.4 26.6)
+TRONROUT0000000044845811;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;938;937;924;925;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770567.4 6277845.2 27.3, 770558.7 6277853.7 26.9)
+TRONROUT0000000044845920;Route à 1 chaussée;;;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770565.9 6277852.4 26.6, 770571 6277852.2 27)
+TRONROUT0000000044845920;Route à 1 chaussée;;;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770571 6277852.2 27, 770579.2 6277854 27)
+TRONROUT0000000044845920;Route à 1 chaussée;;;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770579.2 6277854 27, 770588.8 6277857.2 27.8)
+TRONROUT0000000044845920;Route à 1 chaussée;;;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770588.8 6277857.2 27.8, 770590.5 6277857.2 26.6)
+TRONROUT0000000044845888;Route à 1 chaussée;AV DE MAURIN;AV DE MAURIN;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;25;Libre;;;;;;;;;Non;924;925;886;887;34172;34172;;;;341723665;341723665;;;;;;;;;;;;;commune;commune;Avenue de Maurin;Avenue de Maurin;;;34172_3665;34172_3665;;;;;;;;;;;;;;;;;;LINESTRING Z (770558.7 6277853.7 26.9, 770531.7 6277882.3 27.3)
+TRONROUT0000000044845837;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;37;38;117;118;34172;34172;;;;341725252;341725252;;;;;;;;;;;;;commune;commune;Rue Sainte Véronique;Rue Sainte Véronique;;;34172_5252;34172_5252;;;;;;;;;;;;;;;;;;LINESTRING Z (770496 6277864.5 26.1, 770492.6 6277866.7 26.8, 770489.7 6277867.9 26.8, 770486.7 6277868.3 26.8, 770482.7 6277867.4 26.8, 770475.2 6277862.9 26.8, 770470.7 6277861.4 26.8, 770468.5 6277860.9 26.8, 770466.2 6277861.4 26.8, 770464.1 6277862.8 26.8, 770432.7 6277891.8 27.2)
+TRONROUT0000000044845826;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;38;37;2;1;34172;34172;;;;341725252;341725252;;;;;;;;;;;;;commune;commune;Rue Sainte Véronique;Rue Sainte Véronique;;;34172_5252;34172_5252;;;;;;;;;;;;;;;;;;LINESTRING Z (770496 6277864.5 26.1, 770523 6277891.6 27.8)
+TRONROUT0000000044845940;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;55A;;55;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770531.7 6277882.3 27.3, 770523 6277891.6 27.8)
+TRONROUT0000000044845916;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;30;Libre;;;;;;;;;Non;55;34;55;38;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770523 6277891.6 27.8)
+TRONROUT0000000044845891;Route à 1 chaussée;R SAINTE-MONIQUE;R SAINTE-MONIQUE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;1;2;5;2;34172;34172;;;;341725248;341725248;;;;;;;;;;;;;commune;commune;Rue Sainte Monique;Rue Sainte Monique;;;34172_5248;34172_5248;;;;;;;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770432.7 6277891.8 27.2)
+TRONROUT0000000044843639;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770474.6 6277936.9 28.8, 770465.6 6277945.3 28.8)
+TRONROUT0000000044843690;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;30;Libre;;;;;;;;;Non;32;53;26B;51;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770465.6 6277945.3 28.8, 770417.4 6277990.6 29)
+TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770394.3 6277674.2 22.8)
+TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770394.3 6277674.2 22.8, 770392 6277676.3 22.8)
+TRONROUT0000000240978890;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770392 6277676.3 22.8, 770388.2 6277679.9 22.9)
+TRONROUT0000000044845895;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770397.2 6277671.9 22.8, 770396.9 6277676.3 23, 770396.8 6277680.8 22.8)
+TRONROUT0000000240978435;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770396.8 6277680.8 22.8, 770392.8 6277680.6 22.9, 770388.2 6277679.9 22.9)
+TRONROUT0000000240978812;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;283;284;297;296;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770379.9 6277682.4 22.5, 770384.7 6277681.3 22.9)
+TRONROUT0000000240978812;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;283;284;297;296;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770384.7 6277681.3 22.9, 770388.1 6277680 22.9, 770388.2 6277679.9 22.9)
+TRONROUT0000000109698644;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2007-12-13 12:17:21;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;269;268;283;284;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770367.7 6277691.9 22.7, 770379.9 6277682.4 22.5)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770343.3 6277697.3 22.3, 770346.6 6277697.1 22.2)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770346.6 6277697.1 22.2, 770354.1 6277696.4 22)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770354.1 6277696.4 22, 770358.4 6277695.9 22.7)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770358.4 6277695.9 22.7, 770361.1 6277695.5 22.7)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770361.1 6277695.5 22.7, 770365.3 6277693.2 22.7)
+TRONROUT0000000201979442;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;243;242;269;268;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770365.3 6277693.2 22.7, 770367.7 6277691.9 22.7)
+TRONROUT0000000240978935;Route à 1 chaussée;R VINCENT EUVRARD;R VINCENT EUVRARD;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;45;44;34172;34172;;;;341722579;341722579;;;;;;;;;;;;;commune;commune;Rue Vincent Euvrard;Rue Vincent Euvrard;;;34172_2579;34172_2579;;;;;;;;;;;;;;;;;;LINESTRING Z (770396.8 6277680.8 22.8, 770425 6277712.5 22.6, 770426.4 6277714.1 22.6)
+TRONROUT0000000044845871;Route à 1 chaussée;R SAINT-JACQUES;R SAINT-JACQUES;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;94;93;2;1;34172;34172;;;;341725126;341725126;;;;;;;;;;;;;commune;commune;Rue Saint Jacques;Rue Saint Jacques;;;34172_5126;34172_5126;;;;;;;;;;;;;;;;;;LINESTRING Z (770384.3 6277810.1 24.3, 770399.8 6277797.1 23.7, 770442.3 6277758.6 23.4, 770453.9 6277748.4 23.2, 770455.2 6277747.4 23)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770243 6277721.5 22.4, 770247 6277717.6 22.4)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770247 6277717.6 22.4, 770259 6277707.7 22.1)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770259 6277707.7 22.1, 770272.5 6277701.8 22)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770272.5 6277701.8 22, 770287.9 6277699.7 22)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770287.9 6277699.7 22, 770304.6 6277699 21.9)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770304.6 6277699 21.9, 770330.3 6277697.9 22.3)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770330.3 6277697.9 22.3, 770338.6 6277697.6 22.5)
+TRONROUT0000000201979445;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;135;136;243;242;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770338.6 6277697.6 22.5, 770343.3 6277697.3 22.3)
+TRONROUT0000000201979444;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;123;122;135;136;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770233.1 6277731 22.4, 770243 6277721.5 22.4)
+TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770216 6277746.4 22.1, 770222.5 6277740.9 22.1)
+TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770222.5 6277740.9 22.1, 770228.9 6277735 22.4)
+TRONROUT0000000201979447;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;99;100;123;122;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770228.9 6277735 22.4, 770233.1 6277731 22.4)
+TRONROUT0000000240978930;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;63;64;99;100;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770187.9 6277771.8 23.1, 770205.4 6277756.6 23.1)
+TRONROUT0000000240978930;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;63;64;99;100;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770205.4 6277756.6 23.1, 770216 6277746.4 22.1)
+TRONROUT0000000044845846;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;1;2;103;104;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770243 6277721.5 23.5, 770276.5 6277759.2 20.4, 770315.6 6277804 16.3)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770139.6 6277792.9 24.5, 770145.1 6277791.3 24.1)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770145.1 6277791.3 24.1, 770153.7 6277786.7 23.5)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770153.7 6277786.7 23.5, 770166.2 6277780.4 23.5)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770166.2 6277780.4 23.5, 770168.2 6277779.5 23.5)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770168.2 6277779.5 23.5, 770174 6277776.9 23.5)
+TRONROUT0000000240978265;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;2;;62;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770174 6277776.9 23.5, 770187.9 6277771.8 23.1)
+TRONROUT0000000201979451;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;61;;1;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770187.9 6277771.8 23.1, 770187.1 6277772.4 23.1, 770180.1 6277777.8 23.2, 770171.6 6277783.7 23.4, 770171.4 6277783.9 23.4, 770156.3 6277792.2 23.4, 770146.1 6277798.5 23.5, 770140.1 6277800.9 23.2, 770135.2 6277802.7 24.7)
+TRONROUT0000000240978464;Route à 1 chaussée;;;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770387.4 6277814.2 24.7, 770384.3 6277810.1 24.3)
+TRONROUT0000000115739992;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770387.4 6277814.2 24.7, 770396.3 6277825.7 24.8)
+TRONROUT0000000044845899;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;103;104;159;158;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770315.6 6277804 24.6, 770348.4 6277840.6 25.3)
+TRONROUT0000000044845821;Route à 1 chaussée;R SAINT-JACQUES;R SAINT-JACQUES;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;140;141;94;93;34172;34172;;;;341725126;341725126;;;;;;;;;;;;;commune;commune;Rue Saint Jacques;Rue Saint Jacques;;;34172_5126;34172_5126;;;;;;;;;;;;;;;;;;LINESTRING Z (770348.4 6277840.6 25.3, 770375.9 6277817 24.6, 770384.3 6277810.1 24.3)
+TRONROUT0000000044845912;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;;3;;1;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770396.3 6277825.7 24.8, 770407.7 6277840.4 24.9)
+TRONROUT0000000115739993;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770396.3 6277825.7 24.8, 770361 6277854.7 25.4)
+TRONROUT0000000240977397;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770348.4 6277840.6 25.3, 770352.4 6277845 25.4)
+TRONROUT0000000115739991;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;1;;1;;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770398.6 6277848.6 25, 770407.7 6277840.4 24.9)
+TRONROUT0000000044845822;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;172;171;158;159;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770361 6277854.7 25.4, 770357.6 6277850.9 25.4, 770352.4 6277845 25.4)
+TRONROUT0000000115739990;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770407.7 6277840.4 24.9, 770408.9 6277842 24.9, 770423.3 6277860 25.1)
+TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770124.6 6277788.2 25.3, 770131.4 6277791.3 24.1)
+TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770131.4 6277791.3 24.1, 770136.8 6277792.7 24.1)
+TRONROUT0000000240979105;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770136.8 6277792.7 24.1, 770139.6 6277792.9 24.5)
+TRONROUT0000000201979450;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;618;619;600;601;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770124.6 6277788.2 25.3, 770131 6277797.1 25.5)
+TRONROUT0000000201979450;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;;;;Levé GPS;2.5;Levé GPS;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;618;619;600;601;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770131 6277797.1 25.5, 770135.2 6277802.7 24.7)
+TRONROUT0000000240979102;Route à 1 chaussée;BD PEDRO DE LUNA;BD PEDRO DE LUNA;5;Non;0;En service;2010-07-16 14:01:58;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341724240;341724240;;;;;;;;;;;;;commune;commune;Boulevard Pedro de Luna;Boulevard Pedro de Luna;;;34172_4240;34172_4240;;;;;;;;;;;;;;;;;;LINESTRING Z (770135.2 6277802.7 24.7, 770139.6 6277792.9 24.5)
+TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;601;;553;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770135.2 6277802.7 24.7, 770142 6277809.5 24.9)
+TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;601;;553;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770142 6277809.5 24.9, 770154 6277828.2 24.6)
+TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;601;;553;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770154 6277828.2 24.6, 770157.4 6277834.7 24.6)
+TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;601;;553;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770157.4 6277834.7 24.6, 770158.5 6277837.4 25.2)
+TRONROUT0000000201979448;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-07-31 11:14:36;2023-08-26 17:45:08;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;3.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;601;;553;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770158.5 6277837.4 25.2, 770159.4 6277843.5 25.2)
+TRONROUT0000000044845854;Route à 1 chaussée;PL DU CARDINAL VERDIER;PL DU CARDINAL VERDIER;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;82;;82;;34172;34172;;;;341721028;341721028;;;;;;;;;;;;;non commune;non commune;Place Cardinal Verdier;Place Cardinal Verdier;;;34172_1028;34172_1028;;;;;;;;;;;;;;;;;;LINESTRING Z (770194.3 6277798.2 25.8, 770247 6277860.6 25.3, 770315.6 6277804 24.6)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770166.4 6277909.1 25.3, 770163.4 6277904.6 24.9)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770163.4 6277904.6 24.9, 770162.3 6277901.2 24.9)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770162.3 6277901.2 24.9, 770161.9 6277897.5 24.9)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770161.9 6277897.5 24.9, 770162.7 6277881.3 25.4)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770162.7 6277881.3 25.4, 770163.2 6277869.2 25.4)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770163.2 6277869.2 25.4, 770162.8 6277863.6 25.4)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770162.8 6277863.6 25.4, 770162.6 6277857.5 25.3)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770162.6 6277857.5 25.3, 770162.4 6277852 25.3)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770162.4 6277852 25.3, 770161.7 6277848.2 25.3)
+TRONROUT0000000240978905;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2010-07-16 14:01:58;2023-09-08 09:28:10;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;487;488;551;552;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770161.7 6277848.2 25.3, 770159.4 6277843.5 25.2)
+TRONROUT0000000116207180;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;4.0;Non;Non;Sens direct;;Oui;25;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770166.4 6277909.1 25.3, 770171.4 6277913.8 25.5, 770175.4 6277917.4 25.5, 770178.9 6277920.1 25.6, 770183.5 6277923.3 25.6, 770186.9 6277925.6 25.3)
+TRONROUT0000000116207179;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;1.0;4.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;455;454;487;488;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770180.9 6277932.9 25.3, 770178.5 6277930.3 25.3, 770175.7 6277926.9 25.3, 770173.5 6277924.2 25.2, 770171.3 6277921.3 25.2, 770169.5 6277918.1 25.2, 770168.3 6277915.4 25.2, 770167.4 6277913 25.2, 770166.4 6277909.1 25.3)
+TRONROUT0000000116207183;Rond-point;;;4;Non;0;En service;2008-02-15 13:40:18;2023-09-13 10:06:32;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens direct;;Oui;15;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770186.9 6277925.6 25.3, 770188.3 6277925.5 25.3, 770189.7 6277925.6 25.3, 770191.1 6277926 25.3, 770192.4 6277926.7 25.3)
+TRONROUT0000000116207185;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens inverse;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770220.4 6277928.8 25.7, 770211.6 6277928 25.3, 770205.1 6277927.7 25.3, 770199.1 6277927.3 25.3, 770194.9 6277927 25.3, 770192.4 6277926.7 25.3)
+TRONROUT0000000116207182;Rond-point;;;4;Non;0;En service;2008-02-15 13:40:18;2023-09-07 13:30:06;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770180.9 6277932.9 25.3, 770181 6277931.5 25.3, 770181.4 6277930.1 25.3, 770182.1 6277928.8 25.3, 770183 6277927.6 25.3, 770184.2 6277926.7 25.3, 770185.5 6277926 25.3, 770186.9 6277925.6 25.3)
+TRONROUT0000000116207186;Rond-point;;;4;Non;0;En service;2008-02-15 13:40:18;2023-09-07 13:30:06;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770192.4 6277926.7 25.3, 770194.5 6277928.8 25.3, 770195.2 6277930.1 25.3, 770195.6 6277931.5 25.3, 770195.7 6277932.9 25.3, 770195.6 6277934.3 25.3, 770195.2 6277935.7 25.3, 770194.5 6277937 25.3, 770193.6 6277938.2 25.3, 770192.4 6277939.1 25.3)
+TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770220.4 6277928.8 25.7, 770212.1 6277930.6 25.8)
+TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770212.1 6277930.6 25.8, 770205 6277933.1 25.7)
+TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770205 6277933.1 25.7, 770199.7 6277935.8 25.7)
+TRONROUT0000000116207184;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770199.7 6277935.8 25.7, 770192.4 6277939.1 25.3)
+TRONROUT0000002334351182;Rond-point;;;4;Non;0;En service;2023-09-07 13:30:06;;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770185.5 6277939.8 25.3, 770184.2 6277939.1 25.3, 770183 6277938.2 25.3, 770182.1 6277937 25.3, 770181.4 6277935.7 25.3, 770181 6277934.3 25.3, 770180.9 6277932.9 25.3)
+TRONROUT0000000116207181;Rond-point;;;4;Non;0;En service;2008-02-15 13:40:18;2023-09-07 13:30:06;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens direct;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770192.4 6277939.1 25.3, 770191.1 6277939.8 25.3, 770189.7 6277940.2 25.3, 770188.3 6277940.3 25.3, 770186.9 6277940.2 25.3, 770185.5 6277939.8 25.3)
+TRONROUT0000000116207189;Route à 1 chaussée;;;5;Non;0;En service;2008-02-15 13:40:18;2023-09-07 13:30:06;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;4.0;Non;Non;Double sens;;Oui;5;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770192.9652061858 6277939.831443299 25.344329896912157, 770192.4 6277939.1 25.3)
+TRONROUT0000000116207187;Route à 1 chaussée;R DU MAS DE LEMASSON;R DU MAS DE LEMASSON;4;Non;0;En service;2008-02-15 13:40:18;2023-09-08 09:28:10;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;6.0;Non;Non;Sens inverse;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;341723595;341723595;;;;;;;;;;;;;commune;commune;Rue du Mas de Lemasson;Rue du Mas de Lemasson;;;34172_3595;34172_3595;;;;;;;;;;;;;;;;;;LINESTRING Z (770185.5 6277939.8 25.3, 770185.4679389313 6277939.983206107 25.3)
+TRONROUT0000000294020592;Route à 1 chaussée;PL ROMAIN ROLLAND;PL ROMAIN ROLLAND;5;Non;0;En service;2012-01-10 15:17:41;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;1;;1;;34172;34172;;;;341724933;341724933;;;;;;;;;;;;;commune;commune;Place Romain Rolland;Place Romain Rolland;;;34172_4933;34172_4933;;;;;;;;;;;;;;;;;;LINESTRING Z (770374.5 6277870 25.6, 770398.6 6277848.6 25)
+TRONROUT0000000115739995;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;15;Libre;;;;;;;;;Non;192;191;172;171;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770374.5 6277870 25.6, 770361 6277854.7 25.4)
+TRONROUT0000000115739994;Route à 1 chaussée;R EMILE CHARTIER DIT ALAIN;R EMILE CHARTIER DIT ALAIN;5;Non;0;En service;2008-02-08 11:05:31;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;198;197;192;191;34172;34172;;;;341720134;341720134;;;;;;;;;;;;;commune;commune;Rue Emile Chartier dit Alain;Rue Emile Chartier dit Alain;;;34172_0134;34172_0134;;;;;;;;;;;;;;;;;;LINESTRING Z (770378.3 6277874.3 25.6, 770374.5 6277870 25.6)
+TRONROUT0000000294020591;Route à 1 chaussée;;;5;Non;0;En service;2012-01-10 15:17:41;2023-08-26 17:45:08;;;;;Orthophotographie;3.0;Lidar;0.5;1.0;3.0;Non;Non;Sens direct;;Oui;10;Libre;;;;;;;;;Non;;;;;34172;34172;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770398.6 6277848.6 25.1, 770413.5 6277867.8 25.7, 770340.7 6277935 26.5, 770326.2 6277940.2 26.7, 770314.1 6277935 26.6, 770312.1 6277933.1 26.6)
+TRONROUT0000000044845877;Route à 1 chaussée;LES ORMEAUX 2;LES ORMEAUX 2;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;4.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;;;;;34172;34172;;;;34172#03X;34172#03X;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;LINESTRING Z (770312.1 6277933.1 27.1, 770378.5 6277874.6 25.6, 770378.3 6277874.3 25.6)
+TRONROUT0000000044845858;Route à 1 chaussée;R SAINTE-VERONIQUE;R SAINTE-VERONIQUE;5;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;7.0;Non;Non;Double sens;;Oui;20;Libre;;;;;;;;;Non;117;118;219;218;34172;34172;;;;341725252;341725252;;;;;;;;;;;;;commune;commune;Rue Sainte Véronique;Rue Sainte Véronique;;;34172_5252;34172_5252;;;;;;;;;;;;;;;;;;LINESTRING Z (770432.7 6277891.8 27.2, 770354.3 6277964 27.8, 770351.2 6277966.4 27.8, 770341.5 6277969.7 27.4)
+TRONROUT0000000044845878;Route empierrée;ALL MAURICE BONAFOS;ALL MAURICE BONAFOS;5;Non;0;En service;2006-12-12 11:20:44;2022-12-10 12:02:02;;2009-07-01;;;Photogrammétrie;2.5;Photogrammétrie;1.5;;;Non;Non;Double sens;;Oui;0;Restreint aux ayants droit;;;;;;;;;Non;;135;;135;34172;34172;;;;341723668;341723668;;;;;;;;;;;;;commune;commune;Allées Maurice Bonafos;Allées Maurice Bonafos;;;34172_3668;34172_3668;;;;;;;;;;;;;;;;;;LINESTRING Z (770305.9 6277957.2 26.7, 770375.7 6278029.7 29.3)
+TRONROUT0000000044843696;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;35;Libre;;;;;;;;;Non;45;20;49;26B;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770375.7 6278029.7 29.3, 770417.4 6277990.6 29)
+TRONROUT0000000044843668;Route à 1 chaussée;R SAINT-CLEOPHAS;R SAINT-CLEOPHAS;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;BDTopo;2.5;BDTopo;1.5;2.0;6.0;Non;Non;Double sens;;Oui;10;Libre;;;;;;;;;Non;45;;45;;34172;34172;;;;341725055;341725055;;;;;;;;;;;;;commune;commune;Rue Saint Cléophas;Rue Saint Cléophas;;;34172_5055;34172_5055;;;;;;;;;;;;;;;;;;LINESTRING Z (770364.7 6278040.1 29.5, 770375.7 6278029.7 29.3)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770364.7 6278040.1 29.5, 770350.1 6278030.6 29.6)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770350.1 6278030.6 29.6, 770321.9 6278006.7 28.1)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770321.9 6278006.7 28.1, 770307.5 6277994.6 27.9)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770307.5 6277994.6 27.9, 770295.5 6277983 27)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770295.5 6277983 27, 770265.8 6277950.8 26.2)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770265.8 6277950.8 26.2, 770258.3 6277943.6 26.2)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770258.3 6277943.6 26.2, 770250.8 6277938 26.2)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770250.8 6277938 26.2, 770243.4 6277933.9 26.2)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770243.4 6277933.9 26.2, 770236.9 6277931.3 26.1)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770236.9 6277931.3 26.1, 770228.5 6277929.7 25.8)
+TRONROUT0000000044845892;Route à 1 chaussée;AV DE VILLENEUVE ANGOULEME;AV DE VILLENEUVE ANGOULEME;4;Non;0;En service;2006-12-12 11:20:44;2023-08-26 17:45:08;;;;;Photogrammétrie;2.5;Photogrammétrie;1.5;2.0;5.0;Non;Non;Sens inverse;;Oui;15;Libre;;;;;;;;;Non;267;266;453;454;34172;34172;;;;341725850;341725850;;;;;;;;;;;;;commune;commune;Avenue de Villeneuve-Angoulème;Avenue de Villeneuve-Angoulème;;;34172_5850;34172_5850;;;;;;;;;;;;;;;;;;LINESTRING Z (770228.5 6277929.7 25.8, 770220.4 6277928.8 25.7)
 """)
         return GeoDataFrameLib.read_csv(_sio)
 
     @staticmethod
     def irisTastavinStreetlights():
         '''
         # SOURCE:
```

### Comparing `t4gpd-0.8.0/t4gpd/demos/NantesBDT.py` & `t4gpd-0.9.0/t4gpd/demos/NantesBDT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/Angstrom.py` & `t4gpd-0.9.0/t4gpd/energy/Angstrom.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/DirectSolarIrradianceLib.py` & `t4gpd-0.9.0/t4gpd/energy/DirectSolarIrradianceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/Dogniaux.py` & `t4gpd-0.9.0/t4gpd/energy/Dogniaux.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/FelixMarboutin.py` & `t4gpd-0.9.0/t4gpd/energy/FelixMarboutin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/Perez.py` & `t4gpd-0.9.0/t4gpd/energy/Perez.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/Perraudeau.py` & `t4gpd-0.9.0/t4gpd/energy/Perraudeau.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/PerrinDeBrichambaut.py` & `t4gpd-0.9.0/t4gpd/energy/PerrinDeBrichambaut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/PlotDirectNormalIrradiance.py` & `t4gpd-0.9.0/t4gpd/energy/PlotDirectNormalIrradiance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/PlotIrradiances.py` & `t4gpd-0.9.0/t4gpd/energy/PlotIrradiances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/WilliamAtkinson.py` & `t4gpd-0.9.0/t4gpd/energy/WilliamAtkinson.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py` & `t4gpd-0.9.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/graph/STBetweennessCentrality.py` & `t4gpd-0.9.0/t4gpd/io/STLoadAndClip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 31 dec. 2020
+Created on 18 juin 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,24 +16,26 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from geopandas import clip, read_file
+from t4gpd.commons.BoundingBox import BoundingBox
 from t4gpd.commons.GeoProcess import GeoProcess
-from t4gpd.commons.graph.MCALib import MCALib
 
 
-class STBetweennessCentrality(GeoProcess):
+class STLoadAndClip(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, roads):
+    def __init__(self, filename, roi):
         '''
         Constructor
         '''
-        self.mca = MCALib(roads)
+        self.inputGdf = read_file(filename, bbox=roi)
+        self.roi = BoundingBox(roi).asPolygon()
 
     def run(self):
-        return self.mca.betweenness_centrality()
+        return clip(self.inputGdf, self.roi)
```

### Comparing `t4gpd-0.8.0/t4gpd/graph/STClosenessCentrality.py` & `t4gpd-0.9.0/t4gpd/graph/STClosenessCentrality.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 19 dec. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,24 +16,29 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from geopandas import GeoDataFrame
 from t4gpd.commons.GeoProcess import GeoProcess
-from t4gpd.commons.graph.MCALib import MCALib
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
 
 class STClosenessCentrality(GeoProcess):
     '''
     classdocs
     '''
 
     def __init__(self, roads):
         '''
         Constructor
         '''
-        self.mca = MCALib(roads)
+        if not isinstance(roads, GeoDataFrame):
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
+        self.roads = roads
 
     def run(self):
-        return self.mca.closeness_centrality()
+        ug = UrbanGraphFactory.create(self.roads, method="networkx")
+        return ug.closeness_centrality()
```

### Comparing `t4gpd-0.8.0/t4gpd/graph/STRoadNeighborhood.py` & `t4gpd-0.9.0/t4gpd/graph/STRoadNeighborhood.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 16 nov. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,16 +16,16 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from shapely.geometry import MultiLineString, Point
+from geopandas import GeoDataFrame
+from shapely import Point
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.commons.graph.NeighborhoodLib import NeighborhoodLib
 
 
 class STRoadNeighborhood(GeoProcess):
     '''
@@ -33,35 +33,42 @@
     '''
 
     def __init__(self, roads, fromPoints, maxDists):
         '''
         Constructor
         '''
         if not isinstance(roads, GeoDataFrame):
-            raise IllegalArgumentTypeException(roads, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
         if not isinstance(fromPoints, (GeoDataFrame, Point)):
-            raise IllegalArgumentTypeException(fromPoints, 'GeoDataFrame or single Point')
+            raise IllegalArgumentTypeException(
+                fromPoints, "GeoDataFrame or single Point")
         if not isinstance(maxDists, (str, float, int)):
-            raise IllegalArgumentTypeException(maxDists, 'String fieldname, float or int values')
+            raise IllegalArgumentTypeException(
+                maxDists, "String fieldname, float or int values")
 
         self.roads = roads
 
         if isinstance(fromPoints, GeoDataFrame):
             if maxDists in fromPoints:
-                self.fromPointsAndMaxDists = list(zip(fromPoints.centroid, fromPoints[maxDists]))
+                self.fromPointsAndMaxDists = list(
+                    zip(fromPoints.centroid, fromPoints[maxDists]))
             elif isinstance(maxDists, (float, int)):
-                self.fromPointsAndMaxDists = list(zip(fromPoints.centroid, [maxDists] * len(fromPoints)))
+                self.fromPointsAndMaxDists = list(
+                    zip(fromPoints.centroid, [maxDists] * len(fromPoints)))
         elif isinstance(maxDists, (float, int)):
             self.fromPointsAndMaxDists = [fromPoints, maxDists]
         else:
-            raise Exception('%s is neither a float value nor a fromPoints fieldname!' % maxDists)
+            raise Exception(
+                "{maxDists} is neither a float value nor a fromPoints fieldname!")
 
     def run(self):
         rows = []
         for gid, (fromPoint, maxDist) in enumerate(self.fromPointsAndMaxDists):
             gdf = NeighborhoodLib.neighborhood(self.roads, fromPoint, maxDist)
             rows.append({
-                'gid':gid, 'fromPoint': fromPoint.wkt, 'maxDist': maxDist,
-                'geometry': MultiLineString([geom for geom in gdf.geometry])
-                })
+                "gid": gid,
+                "fromPoint": fromPoint.wkt,
+                "maxDist": maxDist,
+                "geometry": gdf.geometry.squeeze()
+            })
             gid += 1
         return GeoDataFrame(rows, crs=self.roads.crs)
```

### Comparing `t4gpd-0.8.0/t4gpd/graph/STShortestPath.py` & `t4gpd-0.9.0/t4gpd/graph/STShortestPath.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,55 +16,56 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
+from geopandas import GeoDataFrame
+from pandas import concat
 from shapely.geometry import Point
-
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.graph.ShortestPathLib import ShortestPathLib
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
 
 class STShortestPath(GeoProcess):
     '''
     classdocs
     '''
 
     def __init__(self, roads, fromPoints, toPoints):
         '''
         Constructor
         '''
         if not isinstance(roads, GeoDataFrame):
-            raise IllegalArgumentTypeException(roads, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
         if not isinstance(fromPoints, (GeoDataFrame, Point)):
-            raise IllegalArgumentTypeException(fromPoints, 'GeoDataFrame or single Point')
+            raise IllegalArgumentTypeException(
+                fromPoints, "GeoDataFrame or single Point")
         if not isinstance(toPoints, (GeoDataFrame, Point)):
-            raise IllegalArgumentTypeException(toPoints, 'GeoDataFrame or single Point')
+            raise IllegalArgumentTypeException(
+                toPoints, "GeoDataFrame or single Point")
+
+        self.graph = UrbanGraphFactory.create(roads, method="networkx")
 
-        self.graph = ShortestPathLib(roads)
         self.roads = roads
 
         if isinstance(fromPoints, GeoDataFrame):
             self.fromPoints = list(fromPoints.centroid)
         else:
             self.fromPoints = [fromPoints]
 
         if isinstance(toPoints, GeoDataFrame):
             self.toPoints = list(toPoints.centroid)
         else:
             self.toPoints = [toPoints]
 
     def run(self):
-        gid, rows = 0, []
+        gdfs = []
         for fromPoint in self.fromPoints:
             for toPoint in self.toPoints:
-                pathGeom, pathLen = self.graph.shortestPath(fromPoint, toPoint)
-                if not pathGeom is None:
-                    rows.append({'gid':gid, 'pathLen': pathLen, 'fromPoint': fromPoint.wkt,
-                                 'toPoint': toPoint.wkt, 'geometry': pathGeom})
-                    gid += 1
+                gdfs.append(self.graph.shortest_path(fromPoint, toPoint))
 
-        return GeoDataFrame(rows, crs=self.roads.crs)
+        result = GeoDataFrame(concat(gdfs), crs=self.roads.crs)
+        result["gid"] = range(len(result))
+        return result
```

### Comparing `t4gpd-0.8.0/t4gpd/graph/STToRoadsSections.py` & `t4gpd-0.9.0/t4gpd/graph/STMinimumSpanningTree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 17 juin 2020
+Created on 26 oct. 2023
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,38 +16,29 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-
+from geopandas import GeoDataFrame
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.graph.UrbanGraphLibOld import UrbanGraphLibOld
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
 
-class STToRoadsSections(GeoProcess):
+class STMinimumSpanningTree(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, inputGdf, withoutCulDeSac=False):
+    def __init__(self, roads):
         '''
         Constructor
         '''
-        if not isinstance(inputGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(inputGdf, 'GeoDataFrame')
-        self.inputGdf = inputGdf
-        self.withoutCulDeSac = withoutCulDeSac
+        if not isinstance(roads, GeoDataFrame):
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
+        self.roads = roads
 
     def run(self):
-        ga = UrbanGraphLibOld()
-        ga.add([row for _, row in self.inputGdf.iterrows()])
-
-        if self.withoutCulDeSac:
-            rs = ga.getUniqueRoadsSectionsWithoutCulDeSac()
-        else:
-            rs = ga.getUniqueRoadsSections()
-
-        return GeoDataFrame(rs, crs=self.inputGdf.crs)
+        ug = UrbanGraphFactory.create(self.roads, method="networkx")
+        return ug.minimum_spanning_tree()
```

### Comparing `t4gpd-0.8.0/t4gpd/graph/STToRoadsSectionsNodes.py` & `t4gpd-0.9.0/t4gpd/graph/STToRoadsSectionsNodes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 17 juin 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,33 +16,29 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-
+from geopandas import GeoDataFrame
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.graph.UrbanGraphLibOld import UrbanGraphLibOld
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
 
 class STToRoadsSectionsNodes(GeoProcess):
     '''
     classdocs
     '''
 
     def __init__(self, inputGdf):
         '''
         Constructor
         '''
         if not isinstance(inputGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(inputGdf, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(inputGdf, "GeoDataFrame")
         self.inputGdf = inputGdf
 
     def run(self):
-        ga = UrbanGraphLibOld()
-        ga.add([row for _, row in self.inputGdf.iterrows()])
-
-        rsn = ga.getUniqueRoadsSectionsNodes()
-        return GeoDataFrame(rsn, crs=self.inputGdf.crs)
+        ug = UrbanGraphFactory.create(self.inputGdf, method=None)
+        return ug.getUniqueRoadsSectionsNodes()
```

### Comparing `t4gpd-0.8.0/t4gpd/io/AbstractReader.py` & `t4gpd-0.9.0/t4gpd/io/AbstractReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CSVInertialSensorReader.py` & `t4gpd-0.9.0/t4gpd/io/CSVInertialSensorReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CSVReader.py` & `t4gpd-0.9.0/t4gpd/io/CSVReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CSVWKTReader.py` & `t4gpd-0.9.0/t4gpd/io/CSVWKTReader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 31 aug. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,15 +16,16 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
+from geopandas import GeoDataFrame
+from pandas import read_csv
 from shapely.wkt import loads
 from t4gpd.commons.CSVLib import CSVLib
 from t4gpd.commons.GeoProcess import GeoProcess
 
 
 class CSVWKTReader(GeoProcess):
     '''
@@ -38,23 +39,19 @@
         '''
         self.inputFile = inputFile
         self.geomFieldName = geomFieldName
         self.fieldSep = fieldSep
         self.crs = srcEpsgCode
         self.dstEpsgCode = dstEpsgCode
         self.decimalSep = decimalSep
-        
-    def run(self):
-        _rows = CSVLib.read(self.inputFile, self.fieldSep, self.decimalSep)
-
-        rows = []
-        for row in _rows:
-            row['geometry'] = loads(row[self.geomFieldName])
-            rows.append(row)
-
-        outputGdf = GeoDataFrame(rows, crs=self.crs)
-        if 'geometry' != self.geomFieldName:
-            outputGdf = outputGdf.drop(self.geomFieldName, axis=1)
 
+    def run(self):
+        df = read_csv(self.inputFile, sep=self.fieldSep,
+                      decimal=self.decimalSep)
+        df.rename(columns={fieldname: fieldname.strip()
+                  for fieldname in df.columns}, inplace=True)
+        df.rename(columns={self.geomFieldName: "geometry"}, inplace=True)
+        df.geometry = df.geometry.apply(lambda v: loads(v))
+        gdf = GeoDataFrame(df, crs=self.crs)
         if not self.dstEpsgCode is None:
-            outputGdf = outputGdf.to_crs(self.dstEpsgCode)
-        return outputGdf
+            return gdf.to_crs(self.dstEpsgCode)
+        return gdf
```

### Comparing `t4gpd-0.8.0/t4gpd/io/CSVWKTWriter.py` & `t4gpd-0.9.0/t4gpd/io/CSVWKTWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CirReader.py` & `t4gpd-0.9.0/t4gpd/io/CirReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CirValReader.py` & `t4gpd-0.9.0/t4gpd/io/CirValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CirWriter.py` & `t4gpd-0.9.0/t4gpd/io/CirWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/CityGMLReader.py` & `t4gpd-0.9.0/t4gpd/io/CityGMLReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/GeoWriter.py` & `t4gpd-0.9.0/t4gpd/io/GeoWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/GpkgLoader.py` & `t4gpd-0.9.0/t4gpd/io/GpkgLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/GpkgWriter.py` & `t4gpd-0.9.0/t4gpd/io/GpkgWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/MedReader.py` & `t4gpd-0.9.0/t4gpd/io/MedReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/MshReader.py` & `t4gpd-0.9.0/t4gpd/io/MshReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/ObjReader.py` & `t4gpd-0.9.0/t4gpd/io/ObjReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/ObjWriter.py` & `t4gpd-0.9.0/t4gpd/io/ObjWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/Reloading.py` & `t4gpd-0.9.0/t4gpd/io/Reloading.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/STLoadAndClip.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/BBox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 18 juin 2020
+Created on 16 juin 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,26 +16,19 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas import clip, read_file
 from t4gpd.commons.BoundingBox import BoundingBox
-from t4gpd.commons.GeoProcess import GeoProcess
+from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class STLoadAndClip(GeoProcess):
+class BBox(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, filename, roi):
-        '''
-        Constructor
-        '''
-        self.inputGdf = read_file(filename, bbox=roi)
-        self.roi = BoundingBox(roi).asPolygon()
-
-    def run(self):
-        return clip(self.inputGdf, self.roi)
+    @staticmethod
+    def runWithArgs(row):
+        return { 'geometry': BoundingBox(row.geometry).asPolygon() }
```

### Comparing `t4gpd-0.8.0/t4gpd/io/SVGWriter.py` & `t4gpd-0.9.0/t4gpd/io/SVGWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/SalomeWriter.py` & `t4gpd-0.9.0/t4gpd/io/SalomeWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/SalomeWriterAndExtruder.py` & `t4gpd-0.9.0/t4gpd/io/SalomeWriterAndExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/VTUWriter.py` & `t4gpd-0.9.0/t4gpd/io/VTUWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/ValReader.py` & `t4gpd-0.9.0/t4gpd/io/ValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/ZipLoader.py` & `t4gpd-0.9.0/t4gpd/io/ZipLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/io/ZipWriter.py` & `t4gpd-0.9.0/t4gpd/io/ZipWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/isovist/STIsovistField2D.py` & `t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/isovist/STIsovistField2D_new.py` & `t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas import GeoDataFrame
-from shapely import Polygon
 from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.RayCasting4Lib import RayCasting4Lib
+# from t4gpd.commons.raycasting.PrepareMasksLib import PrepareMasksLib
+from t4gpd.commons.raycasting.RayCasting2DLib import RayCasting2DLib
 
 
 class STIsovistField2D_new(GeoProcess):
     '''
     classdocs
     '''
 
@@ -49,16 +49,20 @@
                 "Illegal argument: buildings and viewpoints must share shames CRS!")
 
         self.buildings = buildings
         # CLEAN GEOMETRIES
         self.buildings.geometry = self.buildings.geometry.apply(
             lambda g: g.buffer(0))
 
-        self.rays = RayCasting4Lib.get2DPanopticRaysGeoDataFrame(
+        # the following instruction seems to slow down processing
+        # self.buildings = PrepareMasksLib.getMasksAsBipoints(
+        #     buildings, oriented=True, make_valid=True)
+
+        self.rays = RayCasting2DLib.get2DPanopticRaysGeoDataFrame(
             viewpoints, rayLength, nRays)
         self.nRays = nRays
         self.withIndices = withIndices
 
     def run(self):
-        isovRaysField, isovField = RayCasting4Lib.multipleRayCast2D(
+        isovRaysField, isovField = RayCasting2DLib.multipleRayCast2D(
             self.buildings, self.rays, self.withIndices)
         return isovRaysField, isovField
```

### Comparing `t4gpd-0.8.0/t4gpd/misc/FrequencyHistogram.py` & `t4gpd-0.9.0/t4gpd/misc/FrequencyHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/OptimalNumberOfClusters.py` & `t4gpd-0.9.0/t4gpd/misc/OptimalNumberOfClusters.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/PlotAMatrixOfDiagrams.py` & `t4gpd-0.9.0/t4gpd/misc/PlotAMatrixOfDiagrams.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/PopulationPyramid.py` & `t4gpd-0.9.0/t4gpd/misc/PopulationPyramid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/RoseMappingTool.py` & `t4gpd-0.9.0/t4gpd/misc/RoseMappingTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/STCompass.py` & `t4gpd-0.9.0/t4gpd/misc/STCompass.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/STDendrogram.py` & `t4gpd-0.9.0/t4gpd/misc/STDendrogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/STKMeans.py` & `t4gpd-0.9.0/t4gpd/misc/STKMeans.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/StreetOrientationHistogram.py` & `t4gpd-0.9.0/t4gpd/misc/StreetOrientationHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/TimelineTool.py` & `t4gpd-0.9.0/t4gpd/misc/TimelineTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/misc/WindRose.py` & `t4gpd-0.9.0/t4gpd/misc/WindRose.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/GmshTriangulator.py` & `t4gpd-0.9.0/t4gpd/morph/GmshTriangulator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STAdaptativeGrid.py` & `t4gpd-0.9.0/t4gpd/morph/STAdaptativeGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STBBox.py` & `t4gpd-0.9.0/t4gpd/morph/STBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STClip.py` & `t4gpd-0.9.0/t4gpd/morph/STClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STCoolscapesTessellation.py` & `t4gpd-0.9.0/t4gpd/morph/STCoolscapesTessellation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STCrossroadsGeneration.py` & `t4gpd-0.9.0/t4gpd/morph/STCrossroadsGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STDilationErosion.py` & `t4gpd-0.9.0/t4gpd/morph/STDilationErosion.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STExtractOpenSpaces.py` & `t4gpd-0.9.0/t4gpd/morph/STExtractOpenSpaces.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STFacadesAnalysis.py` & `t4gpd-0.9.0/t4gpd/morph/STFacadesAnalysis.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STGradientOfDistancesToBuildings.py` & `t4gpd-0.9.0/t4gpd/morph/STGradientOfDistancesToBuildings.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,149 +42,169 @@
         if not isinstance(lines, GeoDataFrame):
             raise IllegalArgumentTypeException(lines, 'GeoDataFrame')
         self.lines = lines
 
         if not isinstance(buildings, GeoDataFrame):
             raise IllegalArgumentTypeException(buildings, 'GeoDataFrame')
         self.buildings = buildings
-        self.spatialIdx = buildings.sindex
 
         if (pathidFieldname is not None) and (pathidFieldname not in lines):
-            raise Exception('%s is not a relevant field name!' % (pathidFieldname))
+            raise Exception('%s is not a relevant field name!' %
+                            (pathidFieldname))
 
         self.sampleDist = sampleDist
         self.pathidFieldname = pathidFieldname
         self.threshold = threshold
 
         if not order in (1, 2, 3):
             raise IllegalArgumentTypeException(order, '(1, 2, 3)')
         self.fieldToTest = 'r_deriv%d' % (order)
 
     def __getType(self, _nodeRow):
         _value = _nodeRow[self.fieldToTest]
         if (_value is not None) and (self.threshold > abs(_value)):
             return 'canyon'
         return 'square'
-        
+
     def run(self):
 
         nodesRows, segmentsRows, linesRows = [], [], []
         for _id, row in self.lines.iterrows():
             _line = row.geometry
             _lineLen = _line.length
             if (self.sampleDist < _lineLen):
-                _pathid = _id if (self.pathidFieldname is None) else row[self.pathidFieldname] 
+                _pathid = _id if (
+                    self.pathidFieldname is None) else row[self.pathidFieldname]
                 _nSegm = int(round(_lineLen / self.sampleDist))
                 _sampleDist = _lineLen / _nSegm
 
                 _nodesRows, _segmentsRows = [], []
                 for i in range(0, _nSegm + 1):
                     _sampleGeom = _line.interpolate(i * _sampleDist)
                     _r, _nearestPoint, _ = GeomLib.getNearestFeature(
-                        self.buildings, self.spatialIdx, _sampleGeom, buffDist=40.0)
+                        self.buildings, _sampleGeom)
                     _nodesRows.append({
                         'pathid': _pathid,
                         'nodeid': i,
                         'geometry': _sampleGeom,
                         'curv_absc': i * _sampleDist,
                         'r': _r,
                         'r_deriv1': None,
                         'r_deriv2': None,
                         'r_deriv3': None,
                         'area_type': None
-                        })
+                    })
 
                     _segmentsRows.append({
                         'pathid': _pathid,
                         'nodeid': i,
                         'geometry': LineString([(_sampleGeom.x, _sampleGeom.y), (_nearestPoint.x, _nearestPoint.y)]),
                         'curv_absc': i * _sampleDist,
                         'r': _r,
                         'r_deriv1': None,
                         'r_deriv2': None,
                         'r_deriv3': None,
                         'area_type': None
-                        })
+                    })
 
                 # Assess 1st and 2nd order derivatives
                 for i in range(1, _nSegm):
-                    _hp1 = _nodesRows[i + 1]['geometry'].distance(_nodesRows[i]['geometry'])
-                    _hm1 = _nodesRows[i]['geometry'].distance(_nodesRows[i - 1]['geometry'])
+                    _hp1 = _nodesRows[i +
+                                      1]['geometry'].distance(_nodesRows[i]['geometry'])
+                    _hm1 = _nodesRows[i]['geometry'].distance(
+                        _nodesRows[i - 1]['geometry'])
+
+                    up1, u0, um1 = _nodesRows[i +
+                                              1]['r'], _nodesRows[i]['r'], _nodesRows[i - 1]['r']
 
-                    up1, u0, um1 = _nodesRows[i + 1]['r'], _nodesRows[i]['r'], _nodesRows[i - 1]['r']
-                    
                     _fwdDiff = (up1 - u0) / _hp1
                     _bwdDiff = (u0 - um1) / _hm1
                     _nodesRows[i]['r_deriv1'] = (_fwdDiff + _bwdDiff) / 2.0
                     _cenDiff = (up1 - 2 * u0 + um1) / (_hp1 * _hm1)
                     _nodesRows[i]['r_deriv2'] = _cenDiff
 
                     if (1 < i < _nSegm - 1):
-                        up2, um2 = _nodesRows[i + 2]['r'], _nodesRows[i - 2]['r']
-                        _hp2 = _nodesRows[i + 2]['geometry'].distance(_nodesRows[i + 1]['geometry'])
-                        _hm2 = _nodesRows[i - 2]['geometry'].distance(_nodesRows[i - 1]['geometry'])
-
-                        _fwdDiff2 = (up2 - 3 * up1 + 3 * u0 - um1) / (_hp2 * _hp1 * _hm1)
-                        _bwdDiff2 = (up1 - 3 * u0 + 3 * um1 - um2) / (_hp1 * _hm1 * _hm2)
+                        up2, um2 = _nodesRows[i +
+                                              2]['r'], _nodesRows[i - 2]['r']
+                        _hp2 = _nodesRows[i + 2]['geometry'].distance(
+                            _nodesRows[i + 1]['geometry'])
+                        _hm2 = _nodesRows[i - 2]['geometry'].distance(
+                            _nodesRows[i - 1]['geometry'])
+
+                        _fwdDiff2 = (up2 - 3 * up1 + 3 * u0 -
+                                     um1) / (_hp2 * _hp1 * _hm1)
+                        _bwdDiff2 = (up1 - 3 * u0 + 3 * um1 -
+                                     um2) / (_hp1 * _hm1 * _hm2)
 
-                        _nodesRows[i]['r_deriv3'] = (_fwdDiff2 + _bwdDiff2) / 2.0
+                        _nodesRows[i]['r_deriv3'] = (
+                            _fwdDiff2 + _bwdDiff2) / 2.0
                         _segmentsRows[i]['r_deriv3'] = _nodesRows[i]['r_deriv3']
 
                     elif (1 < i):
                         um2 = _nodesRows[i - 2]['r']
-                        _hm2 = _nodesRows[i - 2]['geometry'].distance(_nodesRows[i - 1]['geometry'])
+                        _hm2 = _nodesRows[i - 2]['geometry'].distance(
+                            _nodesRows[i - 1]['geometry'])
 
-                        _bwdDiff2 = (up1 - 3 * u0 + 3 * um1 - um2) / (_hp1 * _hm1 * _hm2)
+                        _bwdDiff2 = (up1 - 3 * u0 + 3 * um1 -
+                                     um2) / (_hp1 * _hm1 * _hm2)
 
                         _nodesRows[i]['r_deriv3'] = _bwdDiff2
                         _segmentsRows[i]['r_deriv3'] = _nodesRows[i]['r_deriv3']
 
                     elif (i < _nSegm - 1):
                         up2 = _nodesRows[i + 2]['r']
-                        _hp2 = _nodesRows[i + 2]['geometry'].distance(_nodesRows[i + 1]['geometry'])
+                        _hp2 = _nodesRows[i + 2]['geometry'].distance(
+                            _nodesRows[i + 1]['geometry'])
 
-                        _fwdDiff2 = (up2 - 3 * up1 + 3 * u0 - um1) / (_hp2 * _hp1 * _hm1)
+                        _fwdDiff2 = (up2 - 3 * up1 + 3 * u0 -
+                                     um1) / (_hp2 * _hp1 * _hm1)
 
                         _nodesRows[i]['r_deriv3'] = _fwdDiff2
                         _segmentsRows[i]['r_deriv3'] = _nodesRows[i]['r_deriv3']
 
                     _nodesRows[i]['area_type'] = self.__getType(_nodesRows[i])
 
                     _segmentsRows[i]['r_deriv1'] = _nodesRows[i]['r_deriv1']
                     _segmentsRows[i]['r_deriv2'] = _nodesRows[i]['r_deriv2']
                     _segmentsRows[i]['area_type'] = _nodesRows[i]['area_type']
 
-                _nodesRows[0]['r_deriv1'] = (_nodesRows[1]['r'] - _nodesRows[0]['r']) / _nodesRows[1]['geometry'].distance(_nodesRows[0]['geometry'])
+                _nodesRows[0]['r_deriv1'] = (_nodesRows[1]['r'] - _nodesRows[0]['r']) / \
+                    _nodesRows[1]['geometry'].distance(
+                        _nodesRows[0]['geometry'])
                 _nodesRows[0]['area_type'] = self.__getType(_nodesRows[0])
 
                 _segmentsRows[0]['r_deriv1'] = _nodesRows[0]['r_deriv1']
                 _segmentsRows[0]['area_type'] = _nodesRows[0]['area_type']
 
-                _nodesRows[-1]['r_deriv1'] = (_nodesRows[-1]['r'] - _nodesRows[-2]['r']) / _nodesRows[-1]['geometry'].distance(_nodesRows[-2]['geometry'])
+                _nodesRows[-1]['r_deriv1'] = (_nodesRows[-1]['r'] - _nodesRows[-2]['r']) / \
+                    _nodesRows[-1]['geometry'].distance(
+                        _nodesRows[-2]['geometry'])
                 _nodesRows[-1]['area_type'] = self.__getType(_nodesRows[-1])
 
                 _segmentsRows[-1]['r_deriv1'] = _nodesRows[-1]['r_deriv1']
                 _segmentsRows[-1]['area_type'] = _nodesRows[-1]['area_type']
 
                 nodesRows += _nodesRows
                 segmentsRows += _segmentsRows
 
                 # Extract "continuous" sub-linestrings
-                _prevRow, _prevStatus = _nodesRows[0], self.__getType(_nodesRows[0])
+                _prevRow, _prevStatus = _nodesRows[0], self.__getType(
+                    _nodesRows[0])
                 for i in range(1, _nSegm + 1):
                     _currRow = _nodesRows[i]
                     _currStatus = self.__getType(_currRow)
 
                     if (_prevStatus != _currStatus) or (_nSegm == i):
                         _line2d = GeomLib.removeZCoordinate(_line)
-                        _subls = substring(_line2d, _prevRow['curv_absc'], _currRow['curv_absc'])
+                        _subls = substring(
+                            _line2d, _prevRow['curv_absc'], _currRow['curv_absc'])
                         linesRows.append({
                             'pathid': _pathid,
                             'geometry': _subls,
                             'area_type': _prevStatus
-                            })
+                        })
                         _prevRow, _prevStatus = _currRow, _currStatus
 
         return [
             GeoDataFrame(nodesRows, crs=self.lines.crs),
             GeoDataFrame(segmentsRows, crs=self.lines.crs),
             GeoDataFrame(linesRows, crs=self.lines.crs)]
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STGrid.py` & `t4gpd-0.9.0/t4gpd/morph/STGrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 11 juin 2020
 
 @author: tleduc
 
-Copyright 2020-2023 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -28,15 +28,15 @@
 
 class STGrid(GeoProcess):
     '''
     classdocs
     '''
 
     def __init__(self, gdf, dx, dy=None, indoor=None, intoPoint=True,
-                 encode=True, withDist=False):
+                 encode=True, withDist=False, roi=None):
         '''
         Constructor
         '''
         if not isinstance(gdf, GeoDataFrame):
             raise IllegalArgumentTypeException(gdf, "GeoDataFrame")
 
         self.gdf = gdf
@@ -46,27 +46,60 @@
             self.indoor = indoor
         else:
             raise Exception(
                 "Illegal argument: indoor must be chosen in [None, True, False, 'both']!")
         self.intoPoint = intoPoint
         self.encode = encode
         self.withDist = withDist
+        self.roi = roi
 
     def run(self):
-        grid = GridLib.getGrid2(self.gdf, self.dx, self.dy, self.encode)
+        if self.roi is None:
+            grid = GridLib.getGrid2(self.gdf, self.dx, self.dy, self.encode)
+        else:
+            grid = GridLib.getGrid2(self.roi, self.dx, self.dy, self.encode)
 
         if self.indoor is None:
             pass
         elif ("both" == self.indoor):
             grid = GridLib.getIndoorOutdoorGrid(self.gdf, grid)
         elif self.indoor:
             grid = GridLib.getIndoorGrid(self.gdf, grid)
         else:
             grid = GridLib.getOutdoorGrid(self.gdf, grid)
 
         if self.intoPoint:
             grid.geometry = grid.centroid
 
         if self.withDist:
-            grid = GridLib.distanceToNearestContour(self.gdf, grid)
+            if (0 == len(self.gdf)):
+                grid["dist_to_ctr"] = float("inf")
+            else:
+                grid = GridLib.getDistanceToNearestContour(self.gdf, grid)
 
         return grid
+
+
+"""
+# -----
+import matplotlib.pyplot as plt
+from geopandas import clip
+from t4gpd.demos.GeoDataFrameDemos import GeoDataFrameDemos
+from t4gpd.demos.NantesBDT import NantesBDT
+from t4gpd.morph.STBBox import STBBox
+
+buffDist = 100
+roi = STBBox(GeoDataFrameDemos.squaresInNantes("Royale"), buffDist).run()
+buildings = NantesBDT.buildings(roi)
+
+dx = 30
+sensors = STGrid(buildings, dx=dx, dy=None, indoor=False,
+	intoPoint=False, withDist=True).execute()
+
+# -----
+fig, ax = plt.subplots(figsize=(1*8.26, 1*8.26))
+buildings.plot(ax=ax, color="grey")
+sensors.boundary.plot(ax=ax, color="black", linewidth=0.15)
+fig.tight_layout()
+plt.show()
+plt.close(fig)
+"""
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STHeightOfRoughness.py` & `t4gpd-0.9.0/t4gpd/morph/STHeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STIdentifyRowOfTrees.py` & `t4gpd-0.9.0/t4gpd/morph/STIdentifyRowOfTrees.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STMakeBlocks.py` & `t4gpd-0.9.0/t4gpd/commons/CartesianProductLib.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 12 feb. 2021
+Created on 30 jan. 2024
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -17,103 +17,121 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas import GeoDataFrame, overlay
-from pandas import concat
-from shapely.geometry import MultiPolygon, Polygon
-from shapely.ops import unary_union
-from t4gpd.commons.GeoProcess import GeoProcess
+from numpy.random import default_rng
+from pandas import DataFrame, merge
+from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.morph.STPolygonize import STPolygonize
 
 
-class STMakeBlocks(GeoProcess):
+class CartesianProductLib(object):
     '''
     classdocs
     '''
-
-    def __init__(self, buildings, roads, roi=None):
-        '''
-        Constructor
-        '''
-        if not isinstance(buildings, GeoDataFrame):
-            raise IllegalArgumentTypeException(buildings, 'GeoDataFrame')
-        self.buildings = buildings
-
-        if not isinstance(roads, GeoDataFrame):
-            raise IllegalArgumentTypeException(roads, 'GeoDataFrame')
-        self.roads = roads
-
-        if not((roi is None) or isinstance(roi, GeoDataFrame)):
-            raise IllegalArgumentTypeException(roi, 'GeoDataFrame or None')
-        self.roi = roi
-
     @staticmethod
-    def __mkBlocks(buildings, roads, roi):
-        # POLYGONIZE ROADS
-        if not roi is None:
-            _roads = GeoDataFrame(concat([roads[['geometry']], roi[['geometry']]]), crs=roads.crs)
-        else:
-            _roads = roads
-        _polygons = STPolygonize(_roads).run()
-
-        # GROUP BUILDINGS PER URBAN BLOCKS
-        _buildings = overlay(buildings[['geometry']], _polygons, how='intersection')
-        _blocks = _buildings.dissolve(by='gid', as_index=False)
-
-        # TRY TO REMOVE CONCAVITIES IN EACH BLOCK
-        roadsIdx = roads.sindex
-        _blocks.geometry = _blocks.geometry.apply(lambda g: STMakeBlocks.__deleteConcavities(g, roads, roadsIdx))
-
-        return _blocks
+    def product(df1, df2):
+        if not isinstance(df1, DataFrame):
+            raise IllegalArgumentTypeException(df1, "DataFrame")
+        if not isinstance(df2, DataFrame):
+            raise IllegalArgumentTypeException(df2, "DataFrame")
+
+        _df1, _df2 = df1.copy(deep=True), df2.copy(deep=True)
+        rng = default_rng()
+
+        while True:
+            fieldname = str(rng.integers(low=0, high=1e12, size=1)[0])
+            if (not (fieldname in df1) and not (fieldname in df2)):
+                _df1[fieldname] = 0
+                _df2[fieldname] = 0
+                result = merge(_df1, _df2, on=fieldname)
+                result.drop(columns=[fieldname], inplace=True)
+                return result
 
     @staticmethod
-    def __deleteConcavities(block, roads, roadsIdx):
-        _block = block.convex_hull
-        _subsetOfRoads = roads.loc[roadsIdx.intersection(_block.bounds)]
-
-        if (0 == len(list(filter(_block.intersects, _subsetOfRoads.geometry)))):
-            return _block
-
-        _concavities = _block.difference(block)
-        if isinstance(_concavities, Polygon):
-            _concavities = MultiPolygon([_concavities])
-        result = [block]
-        for _concavity in _concavities.geoms:
-            if (0 == len(list(filter(_concavity.intersects, _subsetOfRoads.geometry)))):
-                result.append(_concavity)
-        # return unary_union(result)
-        result = unary_union(result)
-        '''
-        for buffDist in [60, 50, 40, 30, 20, 10]:
-            _tmp = result.buffer(buffDist, join_style=JOIN_STYLE.round).buffer(-buffDist, join_style=JOIN_STYLE.bevel)
-            if (0 == len(list(filter(_tmp.intersects, _subsetOfRoads.geometry)))):
-                result = _tmp
-                print(buffDist)
-                break
-        '''
+    def product_within_distance(gdf1, gdf2, distance):
+        if not isinstance(gdf1, GeoDataFrame):
+            raise IllegalArgumentTypeException(gdf1, "GeoDataFrame")
+        if not isinstance(gdf2, GeoDataFrame):
+            raise IllegalArgumentTypeException(gdf2, "GeoDataFrame")
+        if not GeoDataFrameLib.shareTheSameCrs(gdf1, gdf2):
+            raise Exception(
+                "Illegal argument: gdf1 and gdf2 must share shames CRS!")
+        result = CartesianProductLib.product(gdf1, gdf2)
+        result = result.loc[result.apply(
+            lambda row: row.geometry_x.distance(row.geometry_y), axis=1) <= distance]
+        result.reset_index(drop=True, inplace=True)
         return result
 
-    def run(self):
-        return STMakeBlocks.__mkBlocks(self.buildings, self.roads, self.roi)
-
-'''
-rootdir = '/home/tleduc/Dropbox/crenau/2_papiers_a_ecrire/2021_wavelet/dev/data-p9'
-roads = gpd.read_file(rootdir + '/roads.shp')
-roi = gpd.read_file(rootdir + '/roi.shp')
-buildings = gpd.read_file(rootdir + '/buildings.shp')
-
-# buildings = GeoDataFrameDemos.singleBuildingInNantes()
-# print(buildings.geometry.squeeze().wkt)
-# roads = gpd.GeoDataFrame([{'geometry': loads('LINESTRING (353880 6695040, 353905 6695040)')}], crs=buildings.crs)
-# roads = gpd.GeoDataFrame([{'geometry': loads('LINESTRING (353935 6695030, 353949 6695030)')}], crs=buildings.crs)
-# roads = gpd.GeoDataFrame([{'geometry': loads('LINESTRING (353942 6695020, 353950 6695015)')}], crs=buildings.crs)
-# roads.to_file('/home/tleduc/Dropbox/crenau/2_papiers_a_ecrire/2021_wavelet/dev/data-p9/roads3.shp')
-
-blocks = STMakeBlocks(buildings, roads, roi).run()
-blocks.to_file(rootdir + '/_blocks2.shp')
-
-print('THE END')
-'''
+    @staticmethod
+    def product_within_distance2(gdf1, gdf2, distance):
+        if not isinstance(gdf1, GeoDataFrame):
+            raise IllegalArgumentTypeException(gdf1, "GeoDataFrame")
+        if not isinstance(gdf2, GeoDataFrame):
+            raise IllegalArgumentTypeException(gdf2, "GeoDataFrame")
+        if not GeoDataFrameLib.shareTheSameCrs(gdf1, gdf2):
+            raise Exception(
+                "Illegal argument: gdf1 and gdf2 must share shames CRS!")
+
+        _gdf1 = gdf1.copy(deep=True)
+        _gdf1["geometry_x"] = _gdf1.geometry
+
+        _gdf2 = gdf2.copy(deep=True)
+        _gdf2["geometry_y"] = _gdf2.geometry
+        _gdf2.geometry = _gdf2.geometry.apply(lambda g: g.buffer(distance))
+        _gdf1 = overlay(_gdf1, _gdf2, how="intersection", keep_geom_type=True)
+
+        args = {}
+        for fieldname in gdf1.columns:
+            if (fieldname in gdf2.columns):
+                args.update({f"{fieldname}_1": f"{fieldname}_x",
+                             f"{fieldname}_2": f"{fieldname}_y"})
+
+        _gdf1.rename(columns=args, inplace=True)
+        _gdf1.drop(columns="geometry", inplace=True)
+        return _gdf1
+
+
+"""
+from t4gpd.morph.STGrid import STGrid
+from shapely import box
+
+gdf = GeoDataFrame([{"geometry": box(0, 0, 100, 100)}])
+gdf1 = STGrid(gdf, dx=50, dy=None, indoor=None, intoPoint=True,
+              encode=True, withDist=False).run()
+gdf2 = STGrid(gdf, dx=2, dy=None, indoor=None, intoPoint=True,
+              encode=True, withDist=False).run()
+actual = CartesianProductLib.product_within_distance(gdf1, gdf2, distance=5)
+# actual.rename(columns={"geometry_y": "geometry"}, inplace=True)
+
+actual2 = CartesianProductLib.product_within_distance2(gdf1, gdf2, distance=5)
+# actual2.rename(columns={"geometry_y": "geometry"}, inplace=True)
+
+actual.to_csv("/tmp/1.csv", index=False, sep=";")
+actual2.to_csv("/tmp/2.csv", index=False, sep=";")
+
+import matplotlib.pyplot as plt
+fig, ax = plt.subplots(figsize=(1*8.26, 1*8.26))
+gdf1.plot(ax=ax, marker="v")
+gdf2.plot(ax=ax, marker="+")
+actual.plot(ax=ax, marker=".")
+plt.show()
+plt.close(fig)
+
+import matplotlib.pyplot as plt
+fig, ax = plt.subplots(figsize=(1*8.26, 1*8.26))
+gdf1.plot(ax=ax, marker="v")
+gdf2.plot(ax=ax, marker="+")
+actual2.plot(ax=ax, marker=".")
+plt.show()
+plt.close(fig)
+"""
+
+"""
+a = DataFrame(["a%d" % i for i in range(1, 4)], columns=["chpA"])
+b = DataFrame(["b%d" % i for i in range(1, 3)], columns=["chpB"])
+c = CartesianProductLib.product(a, b)
+print(f"{a}\n{b}\n\n{c}")
+"""
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STMakeGroundSurface.py` & `t4gpd-0.9.0/t4gpd/morph/STMakeGroundSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STMultipleOverlaps.py` & `t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STMultipleOverlaps2.py` & `t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STPointsDensifier.py` & `t4gpd-0.9.0/t4gpd/morph/STPointsDensifier.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STPointsDensifier2.py` & `t4gpd-0.9.0/t4gpd/morph/STPointsDensifier2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STPolygonize.py` & `t4gpd-0.9.0/t4gpd/morph/STPolygonize.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 31 dec. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,16 +16,17 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from shapely.ops import polygonize, unary_union
+from geopandas import GeoDataFrame
+from shapely import union_all
+from shapely.ops import polygonize
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
 class STPolygonize(GeoProcess):
     '''
@@ -33,23 +34,23 @@
     '''
 
     def __init__(self, inputGdf):
         '''
         Constructor
         '''
         if not isinstance(inputGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(inputGdf, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(inputGdf, "GeoDataFrame")
         self.inputGdf = inputGdf
-        
+
     def run(self):
         contours = []
         for geom in self.inputGdf.geometry:
             contours += GeomLib.toListOfLineStrings(geom)
 
         # Contour union
-        contourUnion = unary_union(contours)
+        contourUnion = union_all(contours)
         # Contour network polygonization
         patches = polygonize(contourUnion)
 
-        rows = [{'gid': i, 'geometry': patch} for i, patch in enumerate(patches)]
+        rows = [{"gid": i, "geometry": patch}
+                for i, patch in enumerate(patches)]
         return GeoDataFrame(rows, crs=self.inputGdf.crs)
-
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSkeletonize.py` & `t4gpd-0.9.0/t4gpd/morph/STSkeletonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSkeletonizeTheVoid.py` & `t4gpd-0.9.0/t4gpd/morph/STSkeletonizeTheVoid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSkyMap25D.py` & `t4gpd-0.9.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 24 jul. 2023
+Created on 8 juin 2023
 
 @author: tleduc
 
 Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -17,148 +17,155 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas import GeoDataFrame
-from numpy import arctan2, asarray, cos, linspace, pi, sin
-from shapely import Polygon
-from t4gpd.commons.ArrayCoding import ArrayCoding
+from pandas import DataFrame, Interval, IntervalIndex
 from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
-from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.RayCasting4Lib import RayCasting4Lib
 
 
-class STSkyMap25D(GeoProcess):
+class SnapUclimOnTrackUsingWaypoints(GeoProcess):
     '''
     classdocs
     '''
-    PIDIV2 = 0.5 * pi
 
-    def __init__(self, buildings, viewpoints, nRays=64, rayLength=100.0,
-                 elevationFieldname="HAUTEUR", h0=0.0, size=4.0, epsilon=1e-2,
-                 projectionName="Stereographic", withIndices=False, withAngles=False,
-                 encode=False):
+    def __init__(self, dfUclim, dfMob, tracks, waypoints):
         '''
         Constructor
         '''
-        if not isinstance(buildings, GeoDataFrame):
-            raise IllegalArgumentTypeException(
-                buildings, "buildings GeoDataFrame")
-        if not elevationFieldname in buildings:
-            raise Exception(
-                f"{elevationFieldname} is not a relevant field name!")
-        if not isinstance(viewpoints, GeoDataFrame):
-            raise IllegalArgumentTypeException(
-                viewpoints, "viewpoints GeoDataFrame")
-
-        if not GeoDataFrameLib.shareTheSameCrs(buildings, viewpoints):
-            raise Exception(
-                "Illegal argument: buildings and viewpoints must share shames CRS!")
-
-        self.buildings = buildings
-        self.elevationFieldname = elevationFieldname
-        # CLEAN GEOMETRIES
-        self.buildings.geometry = self.buildings.geometry.apply(
-            lambda g: g.buffer(0))
-        self.buildings.geometry = self.buildings.apply(
-            lambda row: row.geometry if row.geometry.has_z else GeomLib.forceZCoordinateToZ0(
-                row.geometry, row[self.elevationFieldname]),
-            axis=1
-        )
-
-        self.nRays = nRays
-        self.rayLength = rayLength
-        self.rays = RayCasting4Lib.get25DPanopticRaysGeoDataFrame(
-            viewpoints, rayLength, nRays, h0)
-
-        self.size = size
-        self.epsilon = epsilon
-        if not projectionName in ["Stereographic"]:
-            raise IllegalArgumentTypeException(
-                projectionName, "spherical projection as 'Stereographic'")
-        self.proj = self.__stereographic
-
-        self.withIndices = withIndices
-        self.withAngles = withAngles
-        self.encode = encode
-
-    def __stereographic(self, lat, lon):
-        radius = (self.size * cos(lat)) / (1.0 + sin(lat))
-        return (radius * cos(lon), radius * sin(lon))
-
-    def __angles(self, heights, widths, ray_ids):
-        lats = [arctan2(h, w) for h, w in zip(heights, widths)]
-        if (self.nRays != len(ray_ids)):
-            ray_ids = {ray_id: lats[i] for i, ray_id in enumerate(ray_ids)}
-            lats = [
-                ray_ids[i] if i in ray_ids else self.PIDIV2 for i in range(self.nRays)]
-        return lats
-
-    def __buildSkyMap(self, viewpoint, lats, lons):
-        viewpoint = viewpoint.centroid
-        pnodes = [self.proj(lats[i], lons[i])
-                  for i in range(len(lats))]
-        pnodes = [(viewpoint.x + pnode[0], viewpoint.y + pnode[1])
-                  for pnode in pnodes]
-        return Polygon(viewpoint.buffer(self.size + self.epsilon).exterior.coords, [pnodes])
+        if not isinstance(dfUclim, DataFrame):
+            raise IllegalArgumentTypeException(dfUclim, "DataFrame")
+        for fieldname in ["wp1", "wp2", "timestamps"]:
+            if fieldname not in dfUclim:
+                raise Exception(f"{fieldname} is not a relevant field name!")
+        assert dfUclim.wp1.is_monotonic_increasing, "dfImu.wp1 must be increasing!"
+        assert dfUclim.wp1.is_unique, "dfImu.wp1 must be strictly increasing!"
+        assert dfUclim.wp2.is_monotonic_increasing, "dfImu.wp2 must be increasing!"
+        assert dfUclim.wp2.is_unique, "dfImu.wp2 must be strictly increasing!"
+        self.dfUclim = dfUclim
+
+        if not isinstance(dfMob, DataFrame):
+            raise IllegalArgumentTypeException(dfMob, "DataFrame")
+        self.dfMob = dfMob
+
+        if not isinstance(tracks, GeoDataFrame):
+            raise IllegalArgumentTypeException(tracks, "GeoDataFrame")
+        self.track_geom = tracks.geometry.squeeze()
+
+        if not isinstance(waypoints, GeoDataFrame):
+            raise IllegalArgumentTypeException(waypoints, "GeoDataFrame")
+        if "id" not in waypoints:
+            raise Exception(f"'id' is not a relevant field name!")
+        self.waypoints = waypoints
+
+        assert GeoDataFrameLib.shareTheSameCrs(
+            tracks, waypoints), "tracks and waypoints must share the same crs!"
+        self.crs = tracks.crs
+
+    def _buildIntervalIndex(self):
+        intervals, rows = [], []
+        for _, row in self.dfUclim.iterrows():
+            wp1, dts = row.wp1, row.timestamps
+            for idx2 in range(0, len(dts), 2):
+                intervals.append(
+                    Interval(left=dts[idx2], right=dts[idx2 + 1], closed="right"))
+                rows.append(wp1)
+        return DataFrame(data=rows, columns=["wp1"], index=IntervalIndex(intervals))
+
+    def _getWps(self, intervals, dt):
+        idx = intervals.index.get_loc(dt)
+        row = intervals.iloc[idx]
+        return row.wp1
 
     def run(self):
-        smapRaysField = RayCasting4Lib.multipleRayCast25D(
-            self.buildings, self.rays, self.nRays, self.rayLength, self.elevationFieldname, self.withIndices, h0=0.0)
+        intervals = self._buildIntervalIndex()
 
-        if (0 < len(smapRaysField)):
-            lons = linspace(0, 2*pi, self.nRays, endpoint=False)
-            smapRaysField["angles"] = smapRaysField.apply(
-                lambda row: self.__angles(
-                    row.__RAY_DELTA_ALT__, row.__RAY_LEN__, row.__RAY_ID__),
-                axis=1
-            )
-            smapRaysField.geometry = smapRaysField.apply(lambda row: self.__buildSkyMap(
-                row.viewpoint, row.angles, lons), axis=1)
-            smapRaysField.angles = smapRaysField.angles.apply(
-                lambda v: (asarray(v) * 180)/pi)
-
-        fields = ["__RAY_ID__"]
-        for field in ["__RAY_LEN__", "__RAY_ALT__", "__RAY_DELTA_ALT__"]:
-            if field in smapRaysField.columns:
-                fields.append(field)
-
-        if not self.withAngles:
-            fields += ["angles"]
-
-        smapRaysField.drop(columns=fields, inplace=True)
-
-        if self.encode:
-            smapRaysField.viewpoint = smapRaysField.viewpoint.apply(
-                lambda vp: vp.wkt)
-            if "angles" in smapRaysField:
-                smapRaysField.angles = smapRaysField.angles.apply(
-                    lambda a: ArrayCoding.encode(a))
+        def _isInIntervalIndex(intervals, dt): return any(
+            intervals.index.contains(dt))
 
-        return smapRaysField
+        # SELECTION FROM THE SET OF MEASUREMENTS OF THOSE THAT FALL WITHIN THE INTERVALS
+        measures1 = self.dfMob[self.dfMob.timestamp.apply(
+            lambda dt: _isInIntervalIndex(intervals, dt))]
+        measures1 = measures1[["timestamp"]]
+        measures1["wp1"] = measures1.timestamp.apply(
+            lambda dt: self._getWps(intervals, dt))
+        measures1["inc"] = 1
+
+        measures2 = measures1.groupby(by="wp1").\
+            inc.expanding().sum().reset_index(level=[0])
+        measures2.inc = measures2.inc.astype(int)
+        measures2 = measures2.merge(measures2.groupby(by="wp1").transform("max"),
+                                    how="inner", left_index=True, right_index=True)
+
+        # ATTRIBUTE JOIN BETWEEN THE GIVEN TRACK AND ALL WAYPOINTS
+        wp = self.dfUclim[["warning", "actual_elapsed_time"]].merge(
+            self.waypoints[["id", "curv_absc", "sect_len"]],
+            how="left", left_index=True, right_index=True)
+        wp["sect_speed"] = wp.apply(
+            lambda row: row.sect_len/row.actual_elapsed_time, axis=1)
+
+        # ATTRIBUTE JOIN BETWEEN SELECTED MEASUREMENTS AND ALL WAYPOINTS
+        measures2 = measures2.merge(wp[["curv_absc", "sect_len", "actual_elapsed_time", "sect_speed", "warning"]],
+                                    how="inner", left_on="wp1", right_index=True)
+        measures2.rename(columns={"inc_x": "inc", "inc_y": "total", "curv_absc": "curv_absc0"},
+                         inplace=True)
+
+        # DISTRIBUTION OF MEASUREMENTS ON THE POLYLINE ACCORDING TO THEIR CURVILINEAR ABSCISSA VALUE
+        measures2["track"] = 1
+        measures2["curv_absc"] = measures2.apply(
+            lambda row: row.curv_absc0 + (row.inc * row.sect_len) / row.total,
+            axis=1)
+        measures2["geometry"] = measures2.curv_absc.apply(
+            lambda x: self.track_geom.interpolate(x, normalized=False))
+
+        # ADD COLUMNS "ptid" AND "timestamp" TO THE MEASUREMENTS DATAFRAME
+        measures3 = measures2[["track", "inc", "curv_absc", "sect_len",
+                               "actual_elapsed_time", "sect_speed", "warning", "geometry"]].merge(
+            measures1[["timestamp"]], how="inner", left_index=True, right_index=True)
+        measures3 = measures3.merge(
+            self.waypoints[["id", "curv_absc"]], how="left", on="curv_absc")
+        measures3.rename(columns={"id": "ptid"}, inplace=True)
+
+        measures3.at[0, "ptid"] = 1
+        measures3 = GeoDataFrame(measures3, crs=self.crs)
+
+        assert measures3.curv_absc.is_monotonic_increasing, "measures3.curv_absc must be increasing!"
+        assert measures3.curv_absc.is_unique, "measures3.curv_absc must be strictly increasing!"
+
+        # return intervals, measures1, measures2, measures3
+        return measures3
 
 
 """
-import matplotlib.pyplot as plt
-from shapely import Point
-from t4gpd.demos.GeoDataFrameDemos import GeoDataFrameDemos
+from t4gpd.picoclim.CampbellSciReader import CampbellSciReader
+from t4gpd.picoclim.UClimGuidingReader import UClimGuidingReader
+from t4gpd.picoclim.UClimTrackWaypointsReader import UClimTrackWaypointsReader
+
+dir1 = "/home/tleduc/prj/uclim/data/nantes_commerce_feydeau"
+dir2 = f"{dir1}/nantes_commerce_feydeau_20230607_track1_122846/raw_data"
+
+tracks, waypoints = UClimTrackWaypointsReader(f"{dir1}/nantes_commerce_feydeau_track1.csv").run()
+dfUclim = UClimGuidingReader(f"{dir2}/uclimLOC_nantes_commerce_feydeau_20230607T1228.txt").run()
+dfMob = CampbellSciReader(f"{dir2}/CR1000XSeries_TwoSec.dat").run() 
 
-buildings = GeoDataFrameDemos.districtRoyaleInNantesBuildings()
-pts = [ Point((355119.8, 6689339.2)), Point((355143.0, 6689359.4)),
-	Point((355113.4, 6689397.9)) ]
-sensors = GeoDataFrame([{"gid": i, "geometry": p} for i, p in enumerate(pts)],
-	crs=buildings.crs)
-# sensors.geometry = sensors.geometry.apply(lambda g: g.buffer(5))
-
-skymaps = STSkyMap25D(buildings, sensors, withIndices=True).run()
-
-print(skymaps)
-fig, ax = plt.subplots(figsize=(8.26, 8.26))
-buildings.plot(ax=ax, color="grey")
-sensors.plot(ax=ax, color="red")
-skymaps.plot(ax=ax, color="blue")
+r = SnapUclimOnTrackUsingWaypoints(dfUclim, dfMob, tracks, waypoints).run()
+
+import matplotlib.pyplot as plt
+fig, ax = plt.subplots(figsize=(1.5 * 8.26, 1.5 * 8.26))
+tracks.plot(ax=ax, color="red", linewidth=0.3)
+r.plot(ax=ax, marker="+", color="grey")
+waypoints.plot(ax=ax, marker="o", color="red")
+waypoints.apply(lambda x: ax.annotate(
+	text=x.id, xy=x.geometry.coords[0],
+	color="black", size=16, ha="left"), axis=1)
+ax.axis("off")
+fig.tight_layout()
 plt.show()
+
+waypoints.to_file("/tmp/1.gpkg", layer="waypoints")
+tracks.to_file("/tmp/1.gpkg", layer="tracks")
+r.to_file("/tmp/1.gpkg", layer="measures")
 """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSnappingPointsOnLines.py` & `t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 24 sept. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -39,15 +39,14 @@
         if not isinstance(pointsGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(pointsGdf, 'GeoDataFrame')
         self.pointsGdf = pointsGdf
 
         if not isinstance(linesGdf, GeoDataFrame):
             raise IllegalArgumentTypeException(linesGdf, 'GeoDataFrame')
         self.linesGdf = linesGdf
-        self.spatialIdx = linesGdf.sindex
 
         if stepCountFieldname is not None:
             if stepCountFieldname not in pointsGdf:
                 raise Exception('%s is not a relevant field name!' % (stepCountFieldname))
         self.stepCountFieldname = stepCountFieldname
 
     def __check(self, checksum):
@@ -60,15 +59,15 @@
 
     def run(self):
         checksum, rows = dict(), []
         for _, rowPoint in self.pointsGdf.iterrows():
             geomPoint = rowPoint.geometry
             buffDist = 40.0
             minDist, nearestPoint, nearestRow = GeomLib.getNearestFeature(
-                self.linesGdf, self.spatialIdx, geomPoint, buffDist)
+                self.linesGdf, geomPoint)
 
             nearestLine = nearestRow.geometry
             curvilinearAbscissa = nearestLine.project(nearestPoint)
             if self.stepCountFieldname is not None:
                 checksum[rowPoint[self.stepCountFieldname]] = curvilinearAbscissa
 
             rows.append(self.updateOrAppend(rowPoint, {
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSnappingPointsOnLines2.py` & `t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSpatialJoin.py` & `t4gpd-0.9.0/t4gpd/morph/STSpatialJoin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSquaredBBox.py` & `t4gpd-0.9.0/t4gpd/morph/STSquaredBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STSurfaceFraction.py` & `t4gpd-0.9.0/t4gpd/morph/STSurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STVariableWidthBuffer.py` & `t4gpd-0.9.0/t4gpd/morph/STVariableWidthBuffer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/STVoronoiPartition.py` & `t4gpd-0.9.0/t4gpd/morph/STVoronoiPartition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/AngularAbscissa.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AngularAbscissa.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/AspectRatio.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AspectRatio.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/BBox.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexHull.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from t4gpd.commons.BoundingBox import BoundingBox
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class BBox(AbstractGeoprocess):
+class ConvexHull(AbstractGeoprocess):
     '''
     classdocs
     '''
 
     @staticmethod
     def runWithArgs(row):
-        return { 'geometry': BoundingBox(row.geometry).asPolygon() }
+        return { 'geometry': row.geometry.convex_hull }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 18 juin 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,42 +16,39 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from shapely.geometry import Point
-
+from geopandas import GeoDataFrame
+from shapely import Point
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
 class BiggestInscribedDisc(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, masksGdf, nsegm=8):
+    def __init__(self, masksGdf, nsegm=16):
         '''
         Constructor
         '''
         if not isinstance(masksGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(masksGdf, "GeoDataFrame")
         self.masksGdf = masksGdf
-        self.spatialIdx = self.masksGdf.sindex
         self.nsegm = nsegm
 
     def runWithArgs(self, row):
         geom = row.geometry
         if not isinstance(geom, Point):
-            raise IllegalArgumentTypeException(geom, 'GeoDataFrame of Point')
+            raise IllegalArgumentTypeException(geom, "GeoDataFrame of Point")
 
-        buffDist = 40.0
-        minDist, _, _ = GeomLib.getNearestFeature(self.masksGdf, self.spatialIdx, geom, buffDist)
+        minDist, _, _ = GeomLib.getNearestFeature(self.masksGdf, geom)
 
         return {
-            'geometry': geom.buffer(minDist, self.nsegm),
-            'insc_diam': 2 * minDist
-            }
+            "geometry": geom.buffer(minDist, quad_segs=self.nsegm),
+            "insc_diam": 2 * minDist
+        }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/CircularityIndices.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CircularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/ConvexHull.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class ConvexHull(AbstractGeoprocess):
+class MABR(AbstractGeoprocess):
     '''
     classdocs
     '''
 
     @staticmethod
     def runWithArgs(row):
-        return { 'geometry': row.geometry.convex_hull }
+        return { 'geometry': row.geometry.minimum_rotated_rectangle }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/ConvexityIndices.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/Diameter.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Diameter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/EllipticityIndices.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/EllipticityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/FootprintExtruder.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/FootprintExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/GridFace.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/GridFace.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/HMean.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/HMean.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 17 sept. 2020
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,15 +16,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
+from geopandas import GeoDataFrame
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
 class IdentifyTheClosestPolyline(AbstractGeoprocess):
     '''
@@ -32,43 +32,43 @@
     '''
 
     def __init__(self, roadsGdf, roadsIdFieldname, defaultBuffDist=40.0):
         '''
         Constructor
         '''
         if not isinstance(roadsGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(roadsGdf, 'GeoDataFrame')
+            raise IllegalArgumentTypeException(roadsGdf, "GeoDataFrame")
         self.roadsGdf = roadsGdf
-        self.spatialIdx = roadsGdf.sindex
 
         if roadsIdFieldname not in roadsGdf:
-            raise Exception('%s is not a relevant field name!' % (roadsIdFieldname))
+            raise Exception(
+                f"{roadsIdFieldname} is not a relevant field name!")
         self.roadsIdFieldname = roadsIdFieldname
 
         self.buffDist = defaultBuffDist
 
     def __sign(self, x):
         if (0 == x):
             return 0
         return -1 if (x < 0) else 1
 
     def runWithArgs(self, row):
         geom = row.geometry
 
         self.buffDist = 40.0
         minDist, nearestPoint, nearestRow = GeomLib.getNearestFeature(
-            self.roadsGdf, self.spatialIdx, geom, self.buffDist)
+            self.roadsGdf, geom)
 
         nearestRoad = nearestRow.geometry
         curvilinearAbscissa = nearestRoad.project(nearestPoint)
 
         otherPoint = nearestRoad.interpolate(curvilinearAbscissa + 1e-2)
         roadSide = self.__sign(GeomLib.zCrossProduct(
             otherPoint.coords[0], nearestPoint.coords[0], geom.coords[0]))
 
-        return { 
-            # 'geometry': LineString((geom, nearestPoint)),
-            'road_id': nearestRow[self.roadsIdFieldname],
-            'road_dist': minDist,
-            'road_absc': curvilinearAbscissa,
-            'road_side': roadSide
-            }
+        return {
+            # "geometry": LineString((geom, nearestPoint)),
+            "road_id": nearestRow[self.roadsIdFieldname],
+            "road_dist": minDist,
+            "road_absc": curvilinearAbscissa,
+            "road_side": roadSide
+        }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABE.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABR.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RemoveHoles.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class MABR(AbstractGeoprocess):
+class RemoveHoles(AbstractGeoprocess):
     '''
     classdocs
     '''
 
     @staticmethod
     def runWithArgs(row):
-        return { 'geometry': row.geometry.minimum_rotated_rectangle }
+        geom = row.geometry
+        return { 'geometry': GeomLib.removeHoles(geom) }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/MABR2.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/MBC.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MBC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/MPBR.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MPBR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectangularityIndices.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectangularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectifyByFFT.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFFT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/RectifyByFWT.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFWT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/RemoveHoles.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Rotation2D.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 16 juin 2020
+Created on 11 sept. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,20 +16,27 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from t4gpd.commons.GeomLib import GeomLib
+from shapely.affinity import rotate
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class RemoveHoles(AbstractGeoprocess):
+class Rotation2D(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    @staticmethod
-    def runWithArgs(row):
-        geom = row.geometry
-        return { 'geometry': GeomLib.removeHoles(geom) }
+    def __init__(self, angle, origin='center', use_radians=False):
+        '''
+        Constructor
+        '''
+        self.angle = angle
+        self.origin = origin
+        self.use_radians = use_radians
+
+    def runWithArgs(self, row):
+        return { 'geometry': rotate(
+            row.geometry, self.angle, origin='center', use_radians=False) }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/RepresentativePoint.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RepresentativePoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/Rotation2D.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/WMean.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 11 sept. 2020
+Created on 28 sept. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,27 +16,40 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from shapely.affinity import rotate
+from geopandas.geodataframe import GeoDataFrame
+from numpy import mean
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class Rotation2D(AbstractGeoprocess):
+class WMean(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, angle, origin='center', use_radians=False):
+    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
         '''
         Constructor
         '''
-        self.angle = angle
-        self.origin = origin
-        self.use_radians = use_radians
+        if not isinstance(buildingsGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
+        self.buildingsGdf = buildingsGdf
+
+        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
+        self.maxRayLen = maxRayLen
 
     def runWithArgs(self, row):
-        return { 'geometry': rotate(
-            row.geometry, self.angle, origin='center', use_radians=False) }
+        viewPoint = row.geometry.centroid
+
+        _, _, hitDists = RayCasting3Lib.outdoorMultipleRayCast2D(
+            self.buildingsGdf, viewPoint, self.shootingDirs, self.maxRayLen)
+
+        return {
+            # 'hit_dists': ArrayCoding.encode(hitDists),
+            'wmean': float(mean(hitDists))
+            }
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/STGeoProcess.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/STGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyMap2D.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyViewFactor.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactor.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             self.method = SVFLib.svf2018
 
         self.background = background
 
     def runWithArgs(self, row):
         viewpoint = row.geometry.centroid
 
-        enclosingFeatures = GeomLib.getEnclosingFeatures(self.buildings, self.spatialIndex, viewpoint)
+        enclosingFeatures = GeomLib.getEnclosingFeatures(self.buildings, viewpoint)
 
         if (0 == len(enclosingFeatures)):
             # OUTDOOR/STREET-LEVEL VIEWPOINT
             _, _, hitDists, hitMasks, _ = RayCastingLib.multipleRayCast25D(
                 self.buildings, self.spatialIndex, viewpoint, self.shootingDirs,
                 self.maxRayLen, self.elevationFieldname, self.background)
```

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/StarShapedIndices.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/StarShapedIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/SurfaceFraction.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/Translation.py` & `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Translation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/morph/geoProcesses/WMean.py` & `t4gpd-0.9.0/t4gpd/graph/STDelaunayGraph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 28 sept. 2020
+Created on 26 oct. 2023
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,40 +16,29 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from numpy import mean
+from geopandas import GeoDataFrame
+from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
-from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
 
-class WMean(AbstractGeoprocess):
+class STDelaunayGraph(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
+    def __init__(self, roads):
         '''
         Constructor
         '''
-        if not isinstance(buildingsGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
-        self.buildingsGdf = buildingsGdf
-
-        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
-        self.maxRayLen = maxRayLen
-
-    def runWithArgs(self, row):
-        viewPoint = row.geometry.centroid
-
-        _, _, hitDists = RayCasting3Lib.outdoorMultipleRayCast2D(
-            self.buildingsGdf, viewPoint, self.shootingDirs, self.maxRayLen)
-
-        return {
-            # 'hit_dists': ArrayCoding.encode(hitDists),
-            'wmean': float(mean(hitDists))
-            }
+        if not isinstance(roads, GeoDataFrame):
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
+        self.roads = roads
+
+    def run(self):
+        ug = UrbanGraphFactory.create(self.roads, method=None)
+        return ug.delaunay_triangulation()
```

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/CampbellSciReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/CampbellSciReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/ExtraProcessing.py` & `t4gpd-0.9.0/t4gpd/picoclim/ExtraProcessing.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/InertialMeasureReWriter.py` & `t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/InertialMeasureReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/JoinByTimeDistance.py` & `t4gpd-0.9.0/t4gpd/picoclim/JoinByTimeDistance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/KestrelReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/KestrelReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/MeteoFranceReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/MeteoFranceReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py` & `t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/MetrologicalCampaignReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/SensirionReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/SensirionReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py` & `t4gpd-0.9.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/TracksWaypointsReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/TracksWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/UClimGuidingReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/UClimGuidingReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,22 +364,22 @@
 
         warnings.warn("\n" + "*"*70 + f"""{identifier}
 ****\tFROM: {dt0}
 ****\tTO: {dt1}
 ****\tTOTAL PERIOD: {deltaTotal//60} min. {deltaTotal%60} sec.
 ****\tACTUAL PERIOD: {deltaActual//60} min. {deltaActual%60} sec.
 ****\tMEASUREMENT PERFORMANCE: {perf:.1f} %
-****\tNB WAYPOINTS: {len(self.getDfUclim())}
+****\tNB SEGMENTS: {len(self.getDfUclim())}
 """ + "*"*70)
 
     def run(self):
         self.dfUclim = self.getDfUclim()
         self.dfUclim["actual_elapsed_time"] = self.dfUclim.timestamps.apply(
             lambda dts: self.timedeltaBetweenTwoWaypoints(dts).total_seconds())
         self.__check()
         self.audit()
         return self.dfUclim
 
 """
-ifile = "/home/tleduc/prj/uclim/flask/static/uploads/1686227346623113409/uclimLOC_nantes_commerce_feydeau_20230607T1228.txt"
+ifile = "/home/tleduc/prj/uclim/data/nantes_commerce_feydeau/nantes_commerce_feydeau_20230615_track1_092802/raw_data/uclimLOC_nantes_commerce_feydeau_20230615T0927.txt"
 df = UClimGuidingReader(ifile).run()
 """
```

### Comparing `t4gpd-0.8.0/t4gpd/picoclim/UClimTrackWaypointsReader.py` & `t4gpd-0.9.0/t4gpd/picoclim/UClimTrackWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyplot/MultipleMarkerStyles.py` & `t4gpd-0.9.0/t4gpd/pyplot/MultipleMarkerStyles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/AddMemoryLayer.py` & `t4gpd-0.9.0/t4gpd/pyqgis/AddMemoryLayer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/Emphasizer.py` & `t4gpd-0.9.0/t4gpd/pyqgis/Emphasizer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/MapPrinter.py` & `t4gpd-0.9.0/t4gpd/pyqgis/MapPrinter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/PdfMapWriter.py` & `t4gpd-0.9.0/t4gpd/pyqgis/PdfMapWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/SetSymbolLib.py` & `t4gpd-0.9.0/t4gpd/pyqgis/SetSymbolLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/ShowFeatureCount.py` & `t4gpd-0.9.0/t4gpd/pyqgis/ShowFeatureCount.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyqgis/ZoomLib.py` & `t4gpd-0.9.0/t4gpd/pyqgis/ZoomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/GeodeCiel.py` & `t4gpd-0.9.0/t4gpd/pyvista/GeodeCiel.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/Icosahedron.py` & `t4gpd-0.9.0/t4gpd/pyvista/Icosahedron.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/Plotter3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/Plotter3D.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,25 @@
 
 
 class Plotter3D(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, window_size=(1100, 1100), theme=themes.ParaViewTheme(), ofile=None):
+    def __init__(self, window_size=(1100, 1100), theme=themes.ParaViewTheme(),
+                 show_axes=True, ofile=None):
         '''
         Constructor
         '''
         self.ofile = ofile
 
         self.plotter = Plotter(off_screen=(ofile is not None), lighting="none",
                                window_size=window_size)
-        self.plotter.show_axes()
+        if show_axes:
+            self.plotter.show_axes()
         # pyvista.set_plot_theme(themes.DarkTheme())
         # pyvista.set_plot_theme(themes.DocumentTheme())
         # pyvista.set_plot_theme(themes.ParaViewTheme())
         pyvista.set_plot_theme(theme)
 
     def add_mesh(self, scene, color=None, opacity=1.0, show_edges=False,
                  show_scalar_bar=False):
@@ -87,16 +89,16 @@
                            i_size=length, j_size=length,
                            i_resolution=10, j_resolution=10)
         else:
             ground = Disc(center=[xc, yc, zmin], inner=0.0,
                           outer=length, normal=(0.0, 0.0, 1.0),
                           r_res=1, c_res=npts)
 
-        self.add_mesh(ground, color=color, show_edges=show_edges,
-                      show_scalar_bar=show_scalar_bar)
+        self.add_mesh(ground, color=color, opacity=opacity,
+                      show_edges=show_edges, show_scalar_bar=show_scalar_bar)
 
     def add_general_lighting(self, color="grey", intensity=0.95):
         xmin, xmax, ymin, ymax, zmin, zmax = self.plotter.bounds
         xc, yc, zc = self.plotter.center
         light = Light(
             position=(xc, yc, zmax+100),
             focal_point=(xc, yc, zc),
@@ -183,19 +185,19 @@
             h, r = row[trunk_height], row[crown_radius],
             xyz = list(row.geometry.coords[0])[0:2] + [h]
 
             houppier = Sphere(radius=r, center=xyz)
             tronc = Cylinder(center=xyz[0:2] + [xyz[2]/2],
                              direction=(0.0, 0.0, 1.0),
                              radius=0.2, height=h)
-            self.add_mesh(houppier, color=color, opacity=1.0,
-                          show_edges=False,
+            self.add_mesh(houppier, color=color, opacity=opacity,
+                          show_edges=show_edges,
                           show_scalar_bar=show_scalar_bar)
-            self.add_mesh(tronc, color=color, opacity=1.0,
-                          show_edges=False,
+            self.add_mesh(tronc, color=color, opacity=opacity,
+                          show_edges=show_edges,
                           show_scalar_bar=show_scalar_bar)
 
     def my_cpos_callback(self):
         # tuple: camera location, focus point, viewup vector
         # camera_position = [(x,y,z), (fx,fy,fz,), (nx,ny,nz)]
         cpos = self.plotter.camera_position
         (x, y, z), (fx, fy, fz,), (nx, ny, nz) = \
```

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/STRaysToViewFactors.py` & `t4gpd-0.9.0/t4gpd/pyvista/STRaysToViewFactors.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/ToPolyData.py` & `t4gpd-0.9.0/t4gpd/pyvista/ToPolyData.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/ToUnstructuredGrid.py` & `t4gpd-0.9.0/t4gpd/pyvista/ToUnstructuredGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/commons/Diameter3DLib.py` & `t4gpd-0.9.0/t4gpd/pyvista/commons/Diameter3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/commons/RayCasting3DLib.py` & `t4gpd-0.9.0/t4gpd/pyvista/commons/RayCasting3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py` & `t4gpd-0.9.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/commons/SVF3DLib.py` & `t4gpd-0.9.0/t4gpd/pyvista/commons/SVF3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/commons/Triangle3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/commons/Triangle3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/pyvista/geoProcesses/SVF3D.py` & `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/SVF3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/AbstractRasterGeoProcess.py` & `t4gpd-0.9.0/t4gpd/raster/AbstractRasterGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTClip.py` & `t4gpd-0.9.0/t4gpd/raster/RTClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTFromArrayToRaster.py` & `t4gpd-0.9.0/t4gpd/raster/RTFromArrayToRaster.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,106 +16,120 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-import rasterio
 from geopandas import GeoDataFrame
-from numpy import asarray, ndarray
+from numpy import asarray, dtype, ndarray
 from rasterio.io import DatasetReader
-from rasterio.shutil import copy
 from rasterio.transform import Affine
-from tempfile import TemporaryDirectory
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 from t4gpd.raster.AbstractRasterGeoProcess import AbstractRasterGeoProcess
 
 
 class RTFromArrayToRaster(AbstractRasterGeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, array, rasterOrRoi, debug=False):
+    def __init__(self, array, rasterOrRoi, ndv=-9999, debug=False):
         '''
         Constructor
         '''
         if not isinstance(array, (list, ndarray, tuple)):
             raise IllegalArgumentTypeException(
                 array, "list, numpy ndarray, or tuple")
-        self.array = asarray(array).astype("float32")
+        self.array = RTFromArrayToRaster.__asarray(array)
         if (1 == self.array.ndim):
             self.array = self.array.reshape(1, -1)
         if (2 != self.array.ndim):
             raise IllegalArgumentTypeException(
                 array, "*1D* or *2D* list, numpy ndarray, or tuple")
 
         if not isinstance(rasterOrRoi, (DatasetReader, GeoDataFrame)):
             raise IllegalArgumentTypeException(
                 rasterOrRoi, "DatasetReader or GeoDataFrame")
         self.rasterOrRoi = rasterOrRoi
+        self.ndv = ndv
         self.debug = debug
 
     @staticmethod
-    def __extract_metadata_from_DatasetReader(array, raster):
-        if (array.shape[0] != raster.height):
+    def __asarray(array):
+        array = asarray(array)
+        if (array.dtype == dtype(float)):
+            return array.astype("float32")
+        elif (array.dtype == dtype(int)):
+            # Conversion to uint16, int16, int32, etc. is automatic
+            return array.astype("uint8")
+        raise IllegalArgumentTypeException(array, "Array of int or float values")
+
+    def __extract_metadata_from_DatasetReader(self, raster):
+        if (self.array.shape[0] != raster.height):
             raise Exception(
-                f"array.shape[0] ({array.shape[0]}) <> raster.height ({raster.height})!")
-        if (array.shape[1] != raster.width):
+                f"array.shape[0] ({self.array.shape[0]}) <> raster.height ({raster.height})!")
+        if (self.array.shape[1] != raster.width):
             raise Exception(
-                f"array.shape[1] ({array.shape[1]}) <> raster.width ({raster.width})!")
+                f"array.shape[1] ({self.array.shape[1]}) <> raster.width ({raster.width})!")
 
         out_meta = raster.meta.copy()
         out_meta.update({
             "driver": "GTiff",
             "height": raster.height,
             "width": raster.width,
             "transform": raster.transform,
             "crs": raster.crs,
             "count": 1,
-            "dtype": array.dtype,
-            "nodata": -9999
+            "dtype": self.array.dtype,
+            "nodata": self.ndv
         })
         return out_meta
 
-    @staticmethod
-    def __extract_metadata_from_GeoDataFrame(array, roi):
+    def __extract_metadata_from_GeoDataFrame(self, roi):
         minx, miny, maxx, maxy = roi.total_bounds
-        nrows, ncols = array.shape
+        nrows, ncols = self.array.shape
 
         xres = (maxx-minx) / ncols
         yres = (maxy-miny) / nrows
 
         transform = Affine.translation(minx, maxy) * Affine.scale(xres, -yres)
 
         out_meta = {
             "driver": "GTiff",
             "height": nrows,
             "width": ncols,
             "transform": transform,
             "crs": roi.crs,
             "count": 1,
-            "dtype": array.dtype,
-            "nodata": -9999,
+            "dtype": self.array.dtype,
+            "nodata": self.ndv,
             # "blockxsize": 1,
             # "blockysize": 1,
             # "compress": "lzw",
         }
         return out_meta
 
     def run(self):
         if isinstance(self.rasterOrRoi, DatasetReader):
-            out_meta = RTFromArrayToRaster.__extract_metadata_from_DatasetReader(
-                self.array, self.rasterOrRoi)
+            out_meta = self.__extract_metadata_from_DatasetReader(
+                self.rasterOrRoi)
 
         elif isinstance(self.rasterOrRoi, GeoDataFrame):
-            out_meta = RTFromArrayToRaster.__extract_metadata_from_GeoDataFrame(
-                self.array, self.rasterOrRoi)
+            out_meta = self.__extract_metadata_from_GeoDataFrame(
+                self.rasterOrRoi)
 
+        #         print(f"""\theight / nrows = {out_meta['height']}
+        # \twidth / ncols  = {out_meta['width']}
+        # \tminx           = {out_meta['transform'][2]}
+        # \tmaxy           = {out_meta['transform'][5]}
+        # \txres           = {out_meta['transform'][0]}
+        # \tyres           = {out_meta['transform'][4]}
+        # \tndv            = {out_meta['nodata']}
+        # """)
         result = self._write_and_load(self.array, out_meta, self.debug)
         return result
 
 
 """
 import contextily as ctx
 import matplotlib.pyplot as plt
```

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py` & `t4gpd-0.9.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTLoad.py` & `t4gpd-0.9.0/t4gpd/raster/RTLoad.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTNdvi.py` & `t4gpd-0.9.0/t4gpd/raster/RTNdvi.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTToFile.py` & `t4gpd-0.9.0/t4gpd/raster/RTToFile.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/RTVectorize.py` & `t4gpd-0.9.0/t4gpd/raster/RTVectorize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/STRasterize.py` & `t4gpd-0.9.0/t4gpd/raster/STRasterize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/raster/STToRaster.py` & `t4gpd-0.9.0/t4gpd/raster/STToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/AbstractHardShadow.py` & `t4gpd-0.9.0/t4gpd/sun/AbstractHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/STHardShadow.py` & `t4gpd-0.9.0/t4gpd/sun/STHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/STSunMap2D.py` & `t4gpd-0.9.0/t4gpd/sun/STSunMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/STTreeHardShadow.py` & `t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/STTreeHardShadow2.py` & `t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py` & `t4gpd-0.9.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/geoProcesses/SunshineDuration.py` & `t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.8.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py` & `t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         return True
 
     def runWithArgs(self, row):
         # viewpoint = row.geometry.centroid
         viewpoint = row.geometry.representative_point()
 
-        enclosingFeatures = GeomLib.getEnclosingFeatures(self.masksGdf, self.masksSIdx, viewpoint)
+        enclosingFeatures = GeomLib.getEnclosingFeatures(self.masksGdf, viewpoint)
 
         if (0 == len(enclosingFeatures)):
             # OUTDOOR/STREET-LEVEL VIEWPOINT
             nbHits = 0
             for (sunAlti, radDir, rayLen) in self.sunPositions:
                 if self._beingInTheSun(viewpoint, radDir, rayLen, sunAlti):
                     nbHits += 1
```

### Comparing `t4gpd-0.8.0/t4gpd.egg-info/PKG-INFO` & `t4gpd-0.9.0/t4gpd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.8.0
+Version: 0.9.0
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
+Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
-Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
-Description: # t4gpd
-        Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
-        
-        ## Pre-requisites
-        To be able to use the **t4gpd** plugin, perform geoprocessing and display your own maps, you need a Python3 interpreter and recent versions of the geopandas, matplotlib, numpy, and shapely libraries. One possibility is to install a [Miniconda3](https://docs.conda.io/en/latest/miniconda.html) environment, in which you will first create and then configure a new environment (we will call it gpd):
-        > conda create -n gpd
-        
-        > conda activate gpd
-        
-        > conda config --env --add channels conda-forge
-        
-        > conda config --env --set channel_priority strict
-        
-        > conda install python=3.10 geopandas=0.12.2 jupyterlab matplotlib notebook scikit-learn xlrd openpyxl imageio rasterio networkx PyWavelets pysolar windrose geocube mapclassify seaborn plotly matplotlib-scalebar pyvista contextily xlwt
-        
-        > pip install Dijkstar suntimes pythermalcomfort
-        
-        ## Installation instructions
-        As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
-        > pip install t4gpd
-        
-        Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-        > pip install t4gpd-0.7.1.tar.gz
-        
-        ## Read the documentation
-        Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
-        
-        
-        
-        
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# t4gpd
+Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
+
+## Pre-requisites
+To be able to use the **t4gpd** plugin, perform geoprocessing and display your own maps, you need a Python3 interpreter and recent versions of the geopandas, matplotlib, numpy, and shapely libraries. One possibility is to install a [Miniconda3](https://docs.conda.io/en/latest/miniconda.html) environment, in which you will first create and then configure a new environment (we will call it gpd):
+> conda create -n gpd
+
+> conda activate gpd
+
+> conda config --env --add channels conda-forge
+
+> conda config --env --set channel_priority strict
+
+> conda install python=3.10 geopandas=0.12.2 contextily geocube imageio jupyterlab mapclassify matplotlib matplotlib-scalebar meshio networkx notebook openpyxl plotly pvlib Pyarrow pysolar pyvista pywavelets rasterio scikit-learn scipy seaborn windrose xlrd xlwt
+
+> pip install dijkstar pythermalcomfort suntimes
+
+## Installation instructions
+As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
+> pip install t4gpd
+
+Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
+> pip install t4gpd-0.9.0.tar.gz
+
+## Read the documentation
+Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
+
+
+
```

### Comparing `t4gpd-0.8.0/t4gpd.egg-info/SOURCES.txt` & `t4gpd-0.9.0/t4gpd.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,19 @@
 t4gpd/comfort/indices/__init__.py
 t4gpd/commons/AngleLib.py
 t4gpd/commons/ArrayCoding.py
 t4gpd/commons/BoundingBox.py
 t4gpd/commons/CSVLib.py
 t4gpd/commons/CalendarLib.py
 t4gpd/commons/CaliperLib.py
+t4gpd/commons/CartesianProductLib.py
 t4gpd/commons/Checksum.py
 t4gpd/commons/ChrystalAlgorithm.py
 t4gpd/commons/ColorTemperature.py
+t4gpd/commons/ConcaveLib.py
 t4gpd/commons/DataFrameLib.py
 t4gpd/commons/DateRangeLib.py
 t4gpd/commons/DatetimeLib.py
 t4gpd/commons/DiameterLib.py
 t4gpd/commons/Distances.py
 t4gpd/commons/Entropy.py
 t4gpd/commons/Epsilon.py
@@ -102,14 +104,15 @@
 t4gpd/commons/RayCastingLib.py
 t4gpd/commons/RotationLib.py
 t4gpd/commons/SVFLib.py
 t4gpd/commons/ShannonEntropy.py
 t4gpd/commons/SphericalCartesianCoordinates.py
 t4gpd/commons/SphericalProjectionLib.py
 t4gpd/commons/TestUtils.py
+t4gpd/commons/TypeLib.py
 t4gpd/commons/WarnUtils.py
 t4gpd/commons/__init__.py
 t4gpd/commons/crossroads_generation/Sequence.py
 t4gpd/commons/crossroads_generation/SequenceRadii.py
 t4gpd/commons/crossroads_generation/SequencesGeneration.py
 t4gpd/commons/crossroads_generation/__init__.py
 t4gpd/commons/crossroads_identification/AbstractMethod.py
@@ -122,21 +125,36 @@
 t4gpd/commons/ellipse/EllipseLib.py
 t4gpd/commons/ellipse/EllipticHullLib.py
 t4gpd/commons/ellipse/__init__.py
 t4gpd/commons/graph/AbstractUrbanGraphLib.py
 t4gpd/commons/graph/MCALib.py
 t4gpd/commons/graph/NeighborhoodLib.py
 t4gpd/commons/graph/ShortestPathLib.py
+t4gpd/commons/graph/UrbanGraph.py
+t4gpd/commons/graph/UrbanGraphFactory.py
 t4gpd/commons/graph/UrbanGraphLib.py
 t4gpd/commons/graph/UrbanGraphLibOld.py
+t4gpd/commons/graph/UrbanGraphVertex.py
 t4gpd/commons/graph/__init__.py
 t4gpd/commons/grid/AbstractGridLib.py
 t4gpd/commons/grid/GridLib.py
 t4gpd/commons/grid/__init__.py
 t4gpd/commons/isovists/__init__.py
+t4gpd/commons/moon/MoonLib.py
+t4gpd/commons/moon/__init__.py
+t4gpd/commons/proj/DoubleProjectionLib.py
+t4gpd/commons/proj/DoubleProjectionOfPointsLib.py
+t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py
+t4gpd/commons/proj/DoubleProjectionOfWallsLib.py
+t4gpd/commons/proj/__init__.py
+t4gpd/commons/raycasting/PanopticRaysLib.py
+t4gpd/commons/raycasting/PrepareMasksLib.py
+t4gpd/commons/raycasting/RayCasting25DLib.py
+t4gpd/commons/raycasting/RayCasting2DLib.py
+t4gpd/commons/raycasting/__init__.py
 t4gpd/commons/rnd/RandomPointPicking.py
 t4gpd/commons/rnd/__init__.py
 t4gpd/commons/sun/AbstractSunLib.py
 t4gpd/commons/sun/DaylightLib.py
 t4gpd/commons/sun/PySolarSunLib.py
 t4gpd/commons/sun/ShadowLib.py
 t4gpd/commons/sun/SoleneSunLib.py
@@ -169,14 +187,17 @@
 t4gpd/energy/PlotIrradiances.py
 t4gpd/energy/WilliamAtkinson.py
 t4gpd/energy/__init__.py
 t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
 t4gpd/energy/geoProcesses/__init__.py
 t4gpd/graph/STBetweennessCentrality.py
 t4gpd/graph/STClosenessCentrality.py
+t4gpd/graph/STDegreeCentrality.py
+t4gpd/graph/STDelaunayGraph.py
+t4gpd/graph/STMinimumSpanningTree.py
 t4gpd/graph/STRoadNeighborhood.py
 t4gpd/graph/STShortestPath.py
 t4gpd/graph/STToRoadsSections.py
 t4gpd/graph/STToRoadsSectionsNodes.py
 t4gpd/graph/__init__.py
 t4gpd/io/AbstractReader.py
 t4gpd/io/CSVInertialSensorReader.py
@@ -343,20 +364,29 @@
 t4gpd/raster/RTClip.py
 t4gpd/raster/RTFromArrayToRaster.py
 t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py
 t4gpd/raster/RTLoad.py
 t4gpd/raster/RTNdvi.py
 t4gpd/raster/RTToFile.py
 t4gpd/raster/RTVectorize.py
+t4gpd/raster/STFromGridToRaster.py
 t4gpd/raster/STRasterize.py
 t4gpd/raster/STToRaster.py
 t4gpd/raster/__init__.py
 t4gpd/sun/AbstractHardShadow.py
 t4gpd/sun/STHardShadow.py
 t4gpd/sun/STSunMap2D.py
 t4gpd/sun/STTreeHardShadow.py
 t4gpd/sun/STTreeHardShadow2.py
 t4gpd/sun/__init__.py
 t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
 t4gpd/sun/geoProcesses/SunshineDuration.py
 t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
-t4gpd/sun/geoProcesses/__init__.py
+t4gpd/sun/geoProcesses/__init__.py
+t4gpd/wrf/MeteoFranceAggregator.py
+t4gpd/wrf/MeteoFrancePredictor.py
+t4gpd/wrf/MeteoFranceReader.py
+t4gpd/wrf/SkyMapRadiationBalance.py
+t4gpd/wrf/SkyMapRadiationBalance2.py
+t4gpd/wrf/__init__.py
+t4gpd/ws/BDTopoWFSReader.py
+t4gpd/ws/__init__.py
```

