# Comparing `tmp/t4gpd-0.9.0.tar.gz` & `tmp/t4gpd-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t4gpd-0.9.0.tar", last modified: Mon Apr 15 13:22:43 2024, max compression
+gzip compressed data, was "t4gpd-0.9.5.tar", last modified: Thu May 16 19:21:33 2024, max compression
```

## Comparing `t4gpd-0.9.0.tar` & `t4gpd-0.9.5.tar`

### file list

```diff
@@ -1,434 +1,427 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 13:22:39.000000 t4gpd-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 13:22:43.727097 t4gpd-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 13:22:43.731097 t4gpd-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-15 13:22:39.000000 t4gpd-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.659097 t4gpd-0.9.0/t4gpd/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels3.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/commons/
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/AbstractEnergyDemand.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/Wh.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/avidon/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/AbstractScenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/CredocBasedScenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/FullLockdown.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/avidon/scenarios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.663097 t4gpd-0.9.0/t4gpd/comfort/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/EmpiricalThermalIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/LinearThermalIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/UniversalThermalIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.667096 t4gpd-0.9.0/t4gpd/comfort/algo/
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/CommonsLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/ConstantsLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/ETULib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PETLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PMVLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/PTLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/SETLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/SET_mist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/TmrtOutLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/UTCILib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/VDI_PET_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.667096 t4gpd-0.9.0/t4gpd/comfort/indices/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/ASV.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/DI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/ETU.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/H.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/HI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/NET.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/OUTSET.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PE.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PET.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PMV.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/PT.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/SET.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/SETmist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/THI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtOut.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/TmrtRadiometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/UTCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/WCT.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/comfort/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.675097 t4gpd-0.9.0/t4gpd/commons/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/AngleLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ArrayCoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CSVLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CalendarLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CaliperLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/CartesianProductLib.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ChrystalAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ColorTemperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ConcaveLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DataFrameLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DateRangeLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DatetimeLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/DiameterLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeoDataFrameLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeoProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeomLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GeomLib3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/GridFaceLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/IllegalArgumentTypeException.py
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/KernelLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LandoltRingLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LatLonLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/LineStringCuttingLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ListUtilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/Logos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/MyEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/MyNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/PolarCartesianCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting2Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting3Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCasting4Lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RayCastingLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/RotationLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SVFLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ShannonEntropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SphericalCartesianCoordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/SphericalProjectionLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/TestUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/TypeLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/WarnUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.675097 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/Sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequenceRadii.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/AbstractMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FFTMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FWTMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/crossroads_identification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/ellipse/
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/EllipseLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/EllipticHullLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/ellipse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/AbstractUrbanGraphLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/MCALib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/NeighborhoodLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/ShortestPathLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLibOld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphVertex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/AbstractGridLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/GridLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/isovists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/isovists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.679097 t4gpd-0.9.0/t4gpd/commons/moon/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/moon/MoonLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/moon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/proj/
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfPointsLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfWallsLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/proj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/raycasting/
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/PanopticRaysLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/PrepareMasksLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting25DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting2DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/raycasting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/rnd/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/rnd/RandomPointPicking.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/rnd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.683097 t4gpd-0.9.0/t4gpd/commons/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/AbstractSunLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/DaylightLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/PySolarSunLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/ShadowLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SoleneSunLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SunBeamLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/SunLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/commons/sun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.695097 t4gpd-0.9.0/t4gpd/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/AbstractGeoDataFrameDemos.py
--rw-r--r--   0 runner    (1001) docker     (127)    66648 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos2.py
--rw-r--r--   0 runner    (1001) docker     (127)   453528 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos3.py
--rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos4.py
--rw-r--r--   0 runner    (1001) docker     (127)   745426 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos5.py
--rw-r--r--   0 runner    (1001) docker     (127)   435846 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos6.py
--rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos7.py
--rw-r--r--   0 runner    (1001) docker     (127)   435537 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos8.py
--rw-r--r--   0 runner    (1001) docker     (127)    87828 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos9.py
--rw-r--r--   0 runner    (1001) docker     (127)   295105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosA.py
--rw-r--r--   0 runner    (1001) docker     (127)   165363 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosB.py
--rw-r--r--   0 runner    (1001) docker     (127)   220246 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosC.py
--rw-r--r--   0 runner    (1001) docker     (127)  5706650 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/NantesBDT.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/demos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/energy/
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Angstrom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/DirectSolarIrradianceLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Dogniaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/FelixMarboutin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Perez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/Perraudeau.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PerrinDeBrichambaut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PlotDirectNormalIrradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/PlotIrradiances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/WilliamAtkinson.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/energy/geoProcesses/
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/energy/geoProcesses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.699097 t4gpd-0.9.0/t4gpd/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STBetweennessCentrality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STClosenessCentrality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STDegreeCentrality.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STDelaunayGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STMinimumSpanningTree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STRoadNeighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STShortestPath.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STToRoadsSections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/STToRoadsSectionsNodes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.703096 t4gpd-0.9.0/t4gpd/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/AbstractReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVInertialSensorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVWKTReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CSVWKTWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirValReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CirWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/CityGMLReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GeoWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GpkgLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/GpkgWriter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/MedReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/MshReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ObjReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ObjWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/Reloading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/STLoadAndClip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SVGWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SalomeWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/SalomeWriterAndExtruder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/VTUWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ValReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ZipLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/ZipWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.703096 t4gpd-0.9.0/t4gpd/isovist/
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D_new.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/isovist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.707096 t4gpd-0.9.0/t4gpd/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/FrequencyHistogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/OptimalNumberOfClusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/PlotAMatrixOfDiagrams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/PopulationPyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/RoseMappingTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STCompass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STDendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/STKMeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/StreetOrientationHistogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/TimelineTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/WindRose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.711097 t4gpd-0.9.0/t4gpd/morph/
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/GmshTriangulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STAdaptativeGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STBBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STClip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STCoolscapesTessellation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STCrossroadsGeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STDilationErosion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STExtractOpenSpaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STFacadesAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STGradientOfDistancesToBuildings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STHeightOfRoughness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STIdentifyRowOfTrees.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMakeBlocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMakeGroundSurface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPointsDensifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPointsDensifier2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STPolygonize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkeletonize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkeletonizeTheVoid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSkyMap25D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSpatialJoin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSquaredBBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STSurfaceFraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STVariableWidthBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/STVoronoiPartition.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.715097 t4gpd-0.9.0/t4gpd/morph/geoProcesses/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AngularAbscissa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/AspectRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/BBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CircularityIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexHull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexityIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Diameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/EllipticityIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/FootprintExtruder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/GridFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/HMean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABE.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MBC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/MPBR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectangularityIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFFT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFWT.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RemoveHoles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/RepresentativePoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Rotation2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/STGeoProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyMap2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/StarShapedIndices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/SurfaceFraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/Translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/WMean.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/morph/geoProcesses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/picoclim/
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/CampbellSciReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/ExtraProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/JoinByTimeDistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/KestrelReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MeteoFranceReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SensirionReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/TracksWaypointsReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/UClimGuidingReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/UClimTrackWaypointsReader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/picoclim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/pyplot/
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyplot/MultipleMarkerStyles.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.719097 t4gpd-0.9.0/t4gpd/pyqgis/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/AddMemoryLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/Emphasizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/MapPrinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/PdfMapWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/SetSymbolLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/ShowFeatureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/ZoomLib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyqgis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/GeodeCiel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/Icosahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/Plotter3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/STRaysToViewFactors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/ToPolyData.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/ToUnstructuredGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/commons/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/Diameter3DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/RayCasting3DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/SVF3DLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/Triangle3D.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.723096 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/SVF3D.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/raster/
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/AbstractRasterGeoProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTClip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTFromArrayToRaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTNdvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTToFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/RTVectorize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4110 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STFromGridToRaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STRasterize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2916 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/STToRaster.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/raster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/AbstractHardShadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STHardShadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STSunMap2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/sun/geoProcesses/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/sun/geoProcesses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/wrf/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFranceAggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFrancePredictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/MeteoFranceReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/wrf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd/ws/
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/ws/BDTopoWFSReader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:39.000000 t4gpd-0.9.0/t4gpd/ws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:22:43.727097 t4gpd-0.9.0/t4gpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 13:22:43.000000 t4gpd-0.9.0/t4gpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.718084 t4gpd-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 19:21:30.000000 t4gpd-0.9.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 19:21:33.718084 t4gpd-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 19:21:30.000000 t4gpd-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 19:21:33.718084 t4gpd-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-16 19:21:30.000000 t4gpd-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.642083 t4gpd-0.9.5/t4gpd/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.646083 t4gpd-0.9.5/t4gpd/avidon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels3.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.646083 t4gpd-0.9.5/t4gpd/avidon/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/commons/AbstractEnergyDemand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/commons/EnergyDemandCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/commons/EnergyDemandCalculator2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/commons/Wh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.646083 t4gpd-0.9.5/t4gpd/avidon/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/scenarios/AbstractScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/scenarios/CredocBasedScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/scenarios/FullLockdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/avidon/scenarios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.646083 t4gpd-0.9.5/t4gpd/comfort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/EmpiricalThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/LinearThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/UniversalThermalIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.650083 t4gpd-0.9.5/t4gpd/comfort/algo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/CommonsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/ConstantsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/ETULib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/PETLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/PMVLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/PTLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/SETLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/SET_mist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/TmrtOutLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/UTCILib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/VDI_PET_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.654083 t4gpd-0.9.5/t4gpd/comfort/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/ASV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/AbstractThermalComfortIndice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/DI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/ETU.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/H.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/HI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/NET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/OUTSET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/PE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/PET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/PMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/PT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/SET.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/SETmist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/THI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/TmrtGlobeTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/TmrtOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/TmrtRadiometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/UTCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/WCT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/comfort/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.662083 t4gpd-0.9.5/t4gpd/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/AngleLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ArrayCoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/CSVLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/CalendarLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/CaliperLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/CartesianProductLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/Checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ChrystalAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ColorTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ConcaveLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/DataFrameLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/DateRangeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/DatetimeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/DiameterLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/Distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/Entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/Epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/GeoDataFrameLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/GeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/GeomLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/GeomLib3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/GridFaceLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/IllegalArgumentTypeException.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/KernelLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/LandoltRingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/LatLonLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/LineStringCuttingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ListUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/Logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/MyEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/MyNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/PointsDensifierLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/PointsDensifierLib3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/PolarCartesianCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/RayCasting3Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/RayCasting4Lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/RayCastingLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/RotationLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/SVFLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/SphericalCartesianCoordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/SphericalProjectionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/TypeLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/WarnUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.662083 t4gpd-0.9.5/t4gpd/commons/crossroads_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_generation/Sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_generation/SequenceRadii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_generation/SequencesGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.662083 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/AbstractMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/FFTMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/FWTMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/MeanVectorMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/crossroads_identification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.662083 t4gpd-0.9.5/t4gpd/commons/ellipse/
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ellipse/EllipseLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ellipse/EllipticHullLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/ellipse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/NeighborhoodLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphLibOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphVertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/grid/AbstractGridLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/grid/GridLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/isovists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/isovists/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/moon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/moon/MoonLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/moon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/proj/
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfPointsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfWallsLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/proj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/raycasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/raycasting/PanopticRaysLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/raycasting/PrepareMasksLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/raycasting/RayCasting25DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/raycasting/RayCasting2DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/raycasting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.666083 t4gpd-0.9.5/t4gpd/commons/rnd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/rnd/RandomPointPicking.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/rnd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.670083 t4gpd-0.9.5/t4gpd/commons/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/AbstractSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/DaylightLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/PySolarSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/ShadowLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/SoleneSunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/SunBeamLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/SunLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/commons/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.682083 t4gpd-0.9.5/t4gpd/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/AbstractGeoDataFrameDemos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66648 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   453528 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51714 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   745426 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos5.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435846 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos7.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435537 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87828 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos9.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295105 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosA.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165363 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosB.py
+-rw-r--r--   0 runner    (1001) docker     (127)   220246 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosC.py
+-rw-r--r--   0 runner    (1001) docker     (127)  5706650 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/NantesBDT.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/demos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.682083 t4gpd-0.9.5/t4gpd/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/Angstrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/DirectSolarIrradianceLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/Dogniaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/FelixMarboutin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/Perez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/Perraudeau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/PerrinDeBrichambaut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/PlotDirectNormalIrradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/PlotIrradiances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/WilliamAtkinson.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.686084 t4gpd-0.9.5/t4gpd/energy/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/energy/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.686084 t4gpd-0.9.5/t4gpd/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STBetweennessCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STClosenessCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STDegreeCentrality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STDelaunayGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STMinimumSpanningTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STRoadNeighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STShortestPath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STToRoadsSections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/STToRoadsSectionsNodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.690084 t4gpd-0.9.5/t4gpd/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/AbstractReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CSVInertialSensorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CSVReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CSVWKTReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CSVWKTWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CirReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CirValReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CirWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/CityGMLReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/GeoWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/GpkgLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/GpkgWriter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/MedReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/MshReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/ObjReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/ObjWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/Reloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/STLoadAndClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/SVGWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/SalomeWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/SalomeWriterAndExtruder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/VTUWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/ValReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/ZipLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/ZipWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.690084 t4gpd-0.9.5/t4gpd/isovist/
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/isovist/STIsovistField2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/isovist/STIsovistField2D_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/isovist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.694084 t4gpd-0.9.5/t4gpd/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/FrequencyHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/OptimalNumberOfClusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/PlotAMatrixOfDiagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/PopulationPyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/RoseMappingTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/STCompass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/STDendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/STKMeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/StreetOrientationHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/TimelineTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/WindRose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.698084 t4gpd-0.9.5/t4gpd/morph/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/GmshTriangulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STAdaptativeGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STBBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STCoolscapesTessellation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STCrossroadsGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STDilationErosion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STExtractOpenSpaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STFacadesAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STGradientOfDistancesToBuildings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STHeightOfRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STIdentifyRowOfTrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STMakeBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STMakeGroundSurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STMultipleOverlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STMultipleOverlaps2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STPointsDensifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STPointsDensifier2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STPolygonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSkeletonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSkeletonizeTheVoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSkyMap25D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSnappingPointsOnLines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSnappingPointsOnLines2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSpatialJoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSquaredBBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STSurfaceFraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STVariableWidthBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/STVoronoiPartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.706084 t4gpd-0.9.5/t4gpd/morph/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/AbstractGeoprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/AngularAbscissa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/AreaConvexityDefect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/AspectRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/BBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/CircularityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/ConvexHull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/ConvexityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadRecognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadsAngularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/Diameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/EllipticityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/FootprintExtruder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/GetInteriorPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/GridFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/HMean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/HeightOfRoughness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/MBC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/MPBR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectangularityIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectifyByFFT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectifyByFWT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/RemoveHoles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/RepresentativePoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/Rotation2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/STGeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyMap2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyViewFactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/StarShapedIndices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/SurfaceFraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/Translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/WMean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/morph/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.706084 t4gpd-0.9.5/t4gpd/picoclim/
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/CampbellSciReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/ExtraProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7497 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/InertialMeasureReWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/InertialMeasureReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/JoinByTimeDistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/KestrelReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/MeteoFranceReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/MetrologicalCampaignPlottings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/MetrologicalCampaignReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/SensirionReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/TracksWaypointsReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/UClimGuidingReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/UClimTrackWaypointsReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/picoclim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.706084 t4gpd-0.9.5/t4gpd/pyplot/
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyplot/MultipleMarkerStyles.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.710084 t4gpd-0.9.5/t4gpd/pyqgis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/AddMemoryLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/Emphasizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/MapPrinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/SetSymbolLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/ShowFeatureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/ZoomLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyqgis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.710084 t4gpd-0.9.5/t4gpd/pyvista/
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/GeodeCiel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/Icosahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/Plotter3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/STRaysToViewFactors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/ToPolyData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/ToUnstructuredGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.710084 t4gpd-0.9.5/t4gpd/pyvista/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/Diameter3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/RayCasting3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/RayCastingIn3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/SVF3DLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/Triangle3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.714084 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/RayCasting3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/SVF3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.714084 t4gpd-0.9.5/t4gpd/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/AbstractRasterGeoProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTClip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTFromArrayToRaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTNdvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTToFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/RTVectorize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4110 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/STFromGridToRaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/STRasterize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2916 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/STToRaster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/raster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.714084 t4gpd-0.9.5/t4gpd/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/AbstractHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/STHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/STSunMap2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/STTreeHardShadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/STTreeHardShadow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.714084 t4gpd-0.9.5/t4gpd/sun/geoProcesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/geoProcesses/SunshineDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/sun/geoProcesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.718084 t4gpd-0.9.5/t4gpd/wrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/MeteoFranceAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/MeteoFrancePredictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/MeteoFranceReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/SkyMapRadiationBalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/SkyMapRadiationBalance2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/wrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.718084 t4gpd-0.9.5/t4gpd/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/ws/BDTopoWFSReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:30.000000 t4gpd-0.9.5/t4gpd/ws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:33.718084 t4gpd-0.9.5/t4gpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 19:21:33.000000 t4gpd-0.9.5/t4gpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-05-16 19:21:33.000000 t4gpd-0.9.5/t4gpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:21:33.000000 t4gpd-0.9.5/t4gpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:21:33.000000 t4gpd-0.9.5/t4gpd.egg-info/top_level.txt
```

### Comparing `t4gpd-0.9.0/LICENSE.txt` & `t4gpd-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/PKG-INFO` & `t4gpd-0.9.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.9.0
+Version: 0.9.5
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -42,14 +42,14 @@
 > pip install dijkstar pythermalcomfort suntimes
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.9.0.tar.gz
+> pip install t4gpd-0.9.5.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.9.0/README.md` & `t4gpd-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 > pip install dijkstar pythermalcomfort suntimes
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.9.0.tar.gz
+> pip install t4gpd-0.9.5.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.9.0/setup.py` & `t4gpd-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/__init__.py` & `t4gpd-0.9.5/t4gpd/__init__.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/_version.py` & `t4gpd-0.9.5/t4gpd/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 # The following line *must* be the last in the module, exactly as formatted:
-__version__ = '0.9.0'
+__version__ = '0.9.5'
```

### Comparing `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment.py` & `t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment2.py` & `t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/EnergyDemandOfITEquipment3.py` & `t4gpd-0.9.5/t4gpd/avidon/EnergyDemandOfITEquipment3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels.py` & `t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels2.py` & `t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/STDeploymentOfPVPanels3.py` & `t4gpd-0.9.5/t4gpd/avidon/STDeploymentOfPVPanels3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/commons/AbstractEnergyDemand.py` & `t4gpd-0.9.5/t4gpd/avidon/commons/AbstractEnergyDemand.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator.py` & `t4gpd-0.9.5/t4gpd/avidon/commons/EnergyDemandCalculator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/commons/EnergyDemandCalculator2.py` & `t4gpd-0.9.5/t4gpd/avidon/commons/EnergyDemandCalculator2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/commons/Wh.py` & `t4gpd-0.9.5/t4gpd/avidon/commons/Wh.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/scenarios/AbstractScenario.py` & `t4gpd-0.9.5/t4gpd/avidon/scenarios/AbstractScenario.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/scenarios/CredocBasedScenario.py` & `t4gpd-0.9.5/t4gpd/avidon/scenarios/CredocBasedScenario.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/avidon/scenarios/FullLockdown.py` & `t4gpd-0.9.5/t4gpd/avidon/scenarios/FullLockdown.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/EmpiricalThermalIndices.py` & `t4gpd-0.9.5/t4gpd/comfort/EmpiricalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/LinearThermalIndices.py` & `t4gpd-0.9.5/t4gpd/comfort/LinearThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/UniversalThermalIndices.py` & `t4gpd-0.9.5/t4gpd/comfort/UniversalThermalIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/CommonsLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/CommonsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/ConstantsLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/ConstantsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/ETULib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/ETULib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/PETLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/PETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/PMVLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/PMVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/PTLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/PTLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/SETLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/SETLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/SET_mist.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/SET_mist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/TmrtGlobeTemperatureLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/TmrtOutLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/TmrtOutLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/UTCILib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/UTCILib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/VDI_PET_corrected.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/VDI_PET_corrected.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py` & `t4gpd-0.9.5/t4gpd/comfort/algo/WindSpeedExtrapolationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/ASV.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/ASV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/AbstractThermalComfortIndice.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/AbstractThermalComfortIndice.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/DI.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/DI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/ETU.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/ETU.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/H.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/H.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/HI.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/HI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/NET.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/NET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/OUTSET.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/OUTSET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/PE.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/PE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/PET.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/PET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/PMV.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/PMV.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/PT.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/PT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/SET.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/SET.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/SETmist.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/SETmist.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/THI.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/THI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtGlobeTemperature.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/TmrtGlobeTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtOut.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/TmrtOut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/TmrtRadiometer.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/TmrtRadiometer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/UTCI.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/UTCI.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/comfort/indices/WCT.py` & `t4gpd-0.9.5/t4gpd/comfort/indices/WCT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/AngleLib.py` & `t4gpd-0.9.5/t4gpd/commons/AngleLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ArrayCoding.py` & `t4gpd-0.9.5/t4gpd/commons/ArrayCoding.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/BoundingBox.py` & `t4gpd-0.9.5/t4gpd/commons/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/CSVLib.py` & `t4gpd-0.9.5/t4gpd/commons/CSVLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/CalendarLib.py` & `t4gpd-0.9.5/t4gpd/commons/CalendarLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/CaliperLib.py` & `t4gpd-0.9.5/t4gpd/commons/CaliperLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/CartesianProductLib.py` & `t4gpd-0.9.5/t4gpd/commons/CartesianProductLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/Checksum.py` & `t4gpd-0.9.5/t4gpd/commons/Checksum.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ChrystalAlgorithm.py` & `t4gpd-0.9.5/t4gpd/commons/ChrystalAlgorithm.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ColorTemperature.py` & `t4gpd-0.9.5/t4gpd/commons/ColorTemperature.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ConcaveLib.py` & `t4gpd-0.9.5/t4gpd/commons/ConcaveLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/DataFrameLib.py` & `t4gpd-0.9.5/t4gpd/commons/DataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/DateRangeLib.py` & `t4gpd-0.9.5/t4gpd/commons/DateRangeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/DatetimeLib.py` & `t4gpd-0.9.5/t4gpd/commons/DatetimeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/DiameterLib.py` & `t4gpd-0.9.5/t4gpd/commons/DiameterLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/Distances.py` & `t4gpd-0.9.5/t4gpd/commons/Distances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/Entropy.py` & `t4gpd-0.9.5/t4gpd/commons/Entropy.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/Epsilon.py` & `t4gpd-0.9.5/t4gpd/commons/Epsilon.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/GeoDataFrameLib.py` & `t4gpd-0.9.5/t4gpd/commons/GeoDataFrameLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/GeoProcess.py` & `t4gpd-0.9.5/t4gpd/commons/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/GeomLib.py` & `t4gpd-0.9.5/t4gpd/commons/GeomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/GeomLib3D.py` & `t4gpd-0.9.5/t4gpd/commons/GeomLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/GridFaceLib.py` & `t4gpd-0.9.5/t4gpd/commons/GridFaceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/IllegalArgumentTypeException.py` & `t4gpd-0.9.5/t4gpd/commons/IllegalArgumentTypeException.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/KernelLib.py` & `t4gpd-0.9.5/t4gpd/commons/KernelLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/LandoltRingLib.py` & `t4gpd-0.9.5/t4gpd/commons/LandoltRingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/LatLonLib.py` & `t4gpd-0.9.5/t4gpd/commons/LatLonLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/LineStringCuttingLib.py` & `t4gpd-0.9.5/t4gpd/commons/LineStringCuttingLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ListUtilities.py` & `t4gpd-0.9.5/t4gpd/commons/ListUtilities.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/Logos.py` & `t4gpd-0.9.5/t4gpd/commons/Logos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/MyEdge.py` & `t4gpd-0.9.5/t4gpd/commons/MyEdge.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/MyNode.py` & `t4gpd-0.9.5/t4gpd/commons/MyNode.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib.py` & `t4gpd-0.9.5/t4gpd/commons/PointsDensifierLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/PointsDensifierLib3D.py` & `t4gpd-0.9.5/t4gpd/commons/PointsDensifierLib3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/PolarCartesianCoordinates.py` & `t4gpd-0.9.5/t4gpd/commons/PolarCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/RayCasting2Lib.py` & `t4gpd-0.9.5/t4gpd/commons/RayCastingLib.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 8 avr. 2022
+Created on 17 juin 2020
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,281 +16,258 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas import GeoDataFrame
+from geopandas.geodataframe import GeoDataFrame
 from geopandas.sindex import PyGEOSSTRTreeIndex, SpatialIndex
-from numpy import arctan2, cos, pi, sin
-from rtree.index import Index 
+from numpy import cos, pi, sin
+from rtree.index import Index
 from shapely.geometry import LineString, MultiLineString, Point
-from shapely.ops import nearest_points
+from shapely.ops import nearest_points, linemerge
 from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
 
 
-class RayCasting2Lib(object):
+class RayCastingLib(object):
     '''
     classdocs
     '''
 
     @staticmethod
-    def areCovisible(ptA, ptB, masksGdf, maskElevationFieldname, masksSIdx):
-        # To avoid: "Inconsistent coordinate dimensionality"
-        A = ptA if GeomLib.is3D(ptA) else GeomLib.forceZCoordinateToZ0(ptA, z0=0.0)
-        B = ptB if GeomLib.is3D(ptB) else GeomLib.forceZCoordinateToZ0(ptB, z0=0.0)
-        # segm = LineString([Point((ptA.x, ptA.y)), Point((ptB.x, ptB.y))])
-        segm = LineString([A, B])
-        alpha = arctan2(B.z - A.z, segm.length)
-
-        masksIds = masksSIdx.intersection(segm.bounds)
-        for maskId in masksIds:
-            mask = masksGdf.loc[maskId]
-            maskGeom = mask.geometry
-            maskElevation = mask[maskElevationFieldname]
-
-            if segm.intersects(maskGeom):
-                tmpGeom = maskGeom.intersection(segm)
-                gc = tmpGeom.geoms if GeomLib.isMultipart(tmpGeom) else [tmpGeom]
-                for geom in gc:
-                    for vertex in geom.coords:
-                        hitPoint = Point(vertex)
-                        _dist = A.distance(hitPoint)
-                        _angle = arctan2(maskElevation - A.z, _dist)
-                        if (_angle >= alpha):
-                            return False, segm
-        return True, segm
-
-    @staticmethod
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
-    def outdoorSingleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength=100.0): 
+    def singleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength=100.0):
+        if not isinstance(masksGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
+        if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+        if not isinstance(viewPoint, Point):
+            raise IllegalArgumentTypeException(viewPoint, 'Point')
+
         # TL. 23.02.2021
         # To avoid: "Inconsistent coordinate dimensionality"
         viewPoint = Point((viewPoint.x, viewPoint.y))
-        remotePoint = Point((viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
-        ray = LineString([viewPoint, remotePoint])
-
-        anchorId = GeomLib.getAnchoringBuildingId(viewPoint, masksGdf, masksSIdx)
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
 
-        if anchorId is None:
-            # ======================================================================
-            # OUTDOOR VIEWPOINT
-            hitPoint, hitDist, hitMask = None, rayLength, None
-
-            masksIds = list(masksSIdx.intersection(ray.bounds))
-            for maskId in masksIds:
-                mask = masksGdf.loc[maskId]
-                maskGeom = mask.geometry
-
-                # if (ray.touches(maskGeom) or ray.crosses(maskGeom)):
-                if (ray.crosses(maskGeom)):
-                    # THE RAY HITS OR CROSSES THE BUILDING
-                    _tmp = maskGeom.intersection(ray)
-                    _, rp = nearest_points(viewPoint, _tmp)
-                    dist = viewPoint.distance(rp)
-                    if (dist < hitDist):
-                        hitPoint, hitDist, hitMask = rp, dist, mask
-
-            if hitPoint is not None:
-                ray = LineString([viewPoint, hitPoint])
-            else:
-                hitPoint = remotePoint
+        hitPoint, hitDist, hitMask = [None, rayLength, None]
 
+        masksIds = list(masksSIdx.intersection(ray.bounds))
+        for maskId in masksIds:
+            mask = masksGdf.loc[maskId]
+            maskGeom = mask.geometry
+            if ray.crosses(maskGeom):
+                _tmp = maskGeom.intersection(ray)
+                _, rp = nearest_points(viewPoint, _tmp)
+                dist = viewPoint.distance(rp)
+                if (dist < hitDist):
+                    hitPoint, hitDist, hitMask = rp, dist, mask
+
+        if hitPoint is not None:
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
         else:
-            if GeomLib.isAnIndoorPoint(viewPoint, masksGdf):
-                # ======================================================================
-                # INDOOR VIEWPOINT
-                ray, hitPoint, hitDist, hitMask = None, None, 0.0, anchorId
-
-            elif GeomLib.isABorderPoint(viewPoint, masksGdf):
-                # ======================================================================
-                # VIEWPOINT ON A WALL
-                buildingGeom = masksGdf.loc[anchorId].geometry
-                _relate = ray.relate(buildingGeom)
-
-                if (_relate in ['1FF00F212', 'F1FF0F212', 'F1FF0F212']):
-                    # THE RAY GOES ALONG OR INTO THE "ANCHORING" BUILDING
-                    ray, hitPoint, hitDist, hitMask = None, None, 0.0, anchorId
-
-                elif ('FF1F00212' == _relate):
-                    # THE RAY MOVES AWAY FROM THE "ANCHORING" BUILDING
-                    hitPoint, hitDist, hitMask = None, rayLength, None
-
-                    masksIds = list(masksSIdx.intersection(ray.bounds))
-                    masksIds.remove(anchorId)
-                    for maskId in masksIds:
-                        mask = masksGdf.loc[maskId]
-                        maskGeom = mask.geometry
-
-                        if (ray.touches(maskGeom) or ray.crosses(maskGeom)):
-                            # THE RAY HITS OR CROSSES THE "NON-ANCHORING" BUILDING
-                            _tmp = maskGeom.intersection(ray)
-                            _, rp = nearest_points(viewPoint, _tmp)
-                            dist = viewPoint.distance(rp)
-                            if (dist < hitDist):
-                                hitPoint, hitDist, hitMask = rp, dist, mask
-
-                    if hitPoint is not None:
-                        ray = LineString([viewPoint, hitPoint])
-                    else:
-                        hitPoint = remotePoint
-
-                else:
-                    raise Exception('Unreachable instruction!')
+            hitPoint = remotePoint
 
-            else:
-                raise Exception('Unreachable instruction!')
         return [ray, hitPoint, hitDist, hitMask]
 
     @staticmethod
-    def outdoorSingleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
-                                elevationFieldName, background, h0=0.0):
-        # DEFAULT ALTITUDE OF THE VIEWPOINT
-        h0 = viewPoint.z if (viewPoint.has_z) else 1.6
+    def singleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
+                         elevationFieldName, background, h0=0.0):
+        if not isinstance(masksGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
+        if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+        if not isinstance(viewPoint, Point):
+            raise IllegalArgumentTypeException(viewPoint, 'Point')
+        if elevationFieldName not in masksGdf:
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
         # TL. 23.02.2021
         # To avoid: "Inconsistent coordinate dimensionality"
         viewPoint = Point((viewPoint.x, viewPoint.y, h0))
-        remotePoint = Point((viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength, h0))
-        ray = LineString([viewPoint, remotePoint])
-
-        anchorId = GeomLib.getAnchoringBuildingId(viewPoint, masksGdf, masksSIdx)
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength, h0))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
 
-        if anchorId is None:
-            # ======================================================================
-            # OUTDOOR VIEWPOINT
-            hitPoint, hitDist, hitMask, hitHW = None, rayLength, None, 0.0
-
-            masksIds = list(masksSIdx.intersection(ray.bounds))
-            for maskId in masksIds:
-                mask = masksGdf.loc[maskId]
-                maskGeom = mask.geometry
-
-                # if (ray.touches(maskGeom) or ray.crosses(maskGeom)):
-                if (ray.crosses(maskGeom)):
-                    # THE RAY HITS OR CROSSES THE BUILDING
-                    _tmp = maskGeom.intersection(ray)
-                    _, rp = nearest_points(viewPoint, _tmp)
-                    height, dist = mask[elevationFieldName], viewPoint.distance(rp)
-                    hw = (height - h0) / dist
-                    if background and (hitHW < hw):
-                        hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
-                    elif (not background) and (dist < hitDist):
-                        hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
-
-            if hitPoint is not None:
-                ray = LineString([viewPoint, hitPoint])
-            else:
-                hitPoint = remotePoint
+        hitPoint, hitDist, hitMask, hitHW = [None, rayLength, None, 0]
 
+        masksIds = list(masksSIdx.intersection(ray.bounds))
+        for maskId in masksIds:
+            mask = masksGdf.loc[maskId]
+            maskGeom = mask.geometry
+            if ray.crosses(maskGeom):
+                _tmp = maskGeom.intersection(ray)
+                _, rp = nearest_points(viewPoint, _tmp)
+                height, dist = mask[elevationFieldName], viewPoint.distance(rp)
+                hw = height / dist
+                if background and (hitHW < hw):
+                    hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
+                elif (not background) and (dist < hitDist):
+                    hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
+
+        if hitPoint is not None:
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
         else:
-            anchor = masksGdf.loc[anchorId]
-            if GeomLib.isAnIndoorPoint(viewPoint, masksGdf):
-                # ======================================================================
-                # INDOOR VIEWPOINT
-                ray, hitPoint, hitDist, hitMask, hitHW = None, None, 0.0, anchor, None
-
-            elif GeomLib.isABorderPoint(viewPoint, masksGdf):
-                # ======================================================================
-                # VIEWPOINT ON A WALL
-                buildingGeom = anchor.geometry
-                _relate = ray.relate(buildingGeom)
-
-                if (_relate in ['1FF00F212', 'F1FF0F212', 'F1FF0F212', 'F11F00212', '101F00212']):
-                    # THE RAY GOES ALONG OR INTO THE "ANCHORING" BUILDING
-                    ray, hitPoint, hitDist, hitMask, hitHW = None, None, 0.0, anchor, None
-
-                elif ('FF1F00212' == _relate):
-                    # THE RAY MOVES AWAY FROM THE "ANCHORING" BUILDING
-                    hitPoint, hitDist, hitMask, hitHW = None, rayLength, None, 0.0
-
-                    masksIds = list(masksSIdx.intersection(ray.bounds))
-                    masksIds.remove(anchorId)
-                    for maskId in masksIds:
-                        mask = masksGdf.loc[maskId]
-                        maskGeom = mask.geometry
-
-                        if (ray.touches(maskGeom) or ray.crosses(maskGeom)):
-                            # THE RAY HITS OR CROSSES THE "NON-ANCHORING" BUILDING
-                            _tmp = maskGeom.intersection(ray)
-                            _, rp = nearest_points(viewPoint, _tmp)
-                            height, dist = mask[elevationFieldName], viewPoint.distance(rp)
-                            hw = (height - h0) / dist
-                            if background and (hitHW < hw):
-                                hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
-                            elif (not background) and (dist < hitDist):
-                                hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
-
-                    if hitPoint is not None:
-                        ray = LineString([viewPoint, hitPoint])
-                    else:
-                        hitPoint = remotePoint
+            hitPoint = remotePoint
+
+        return [ray, hitPoint, hitDist, hitMask, hitHW]
+
+    @staticmethod
+    def singleRayCastOnTopOfRoof(masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
+                                 h0, elevationFieldName, background):
+
+        if not isinstance(masksGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
+        if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+        if not isinstance(viewPoint, Point):
+            raise IllegalArgumentTypeException(viewPoint, 'Point')
+        if elevationFieldName not in masksGdf:
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
 
-                else:
-                    raise Exception('Unreachable instruction!')
+        # TL. 23.02.2021
+        # To avoid: "Inconsistent coordinate dimensionality"
+        viewPoint = Point((viewPoint.x, viewPoint.y))
+        remotePoint = Point(
+            (viewPoint.x + shootingDir[0] * rayLength, viewPoint.y + shootingDir[1] * rayLength))
+        ray = LineString([(viewPoint.x, viewPoint.y),
+                         (remotePoint.x, remotePoint.y)])
+
+        hitPoint, hitDist, hitMask, hitHW = [None, rayLength, None, 0]
+
+        masksIds = list(masksSIdx.intersection(ray.bounds))
+        for maskId in masksIds:
+            mask = masksGdf.loc[maskId]
+            maskGeom = mask.geometry
+            if ray.crosses(maskGeom):
+                _tmp = maskGeom.intersection(ray)
+                _, rp = nearest_points(viewPoint, _tmp)
+                height, dist = mask[elevationFieldName], viewPoint.distance(rp)
+                hw = (height - h0) / dist
+                if background and (hitHW < hw):
+                    hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
+                elif (not background) and (dist < hitDist) and (0 < hw):
+                    hitPoint, hitDist, hitMask, hitHW = rp, dist, mask, hw
+
+        if hitPoint is not None:
+            ray = LineString(
+                [(viewPoint.x, viewPoint.y), (hitPoint.x, hitPoint.y)])
+        else:
+            hitPoint = remotePoint
 
-            else:
-                raise Exception('Unreachable instruction!')
         return [ray, hitPoint, hitDist, hitMask, hitHW]
 
     @staticmethod
-    def outdoorMultipleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength=100.0):
+    def multipleRayCast2D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength=100.0):
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
-            ray, hitPoint, hitDist, hitMask = RayCasting2Lib.outdoorSingleRayCast2D(
+            ray, hitPoint, hitDist, hitMask = RayCastingLib.singleRayCast2D(
                 masksGdf, masksSIdx, viewPoint, shootingDir, rayLength)
-            if not ray is None:
-                rays.append(ray)
-                hitPoints.append(hitPoint)
+            rays.append(ray)
+            hitPoints.append(hitPoint)
             hitDists.append(hitDist)
             hitMasks.append(hitMask)
 
         return [MultiLineString(rays), hitPoints, hitDists, hitMasks]
 
     @staticmethod
-    def outdoorMultipleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength,
-                                  elevationFieldName, background, h0=0.0):
+    def multipleRayCast25D(masksGdf, masksSIdx, viewPoint, shootingDirs, rayLength,
+                           elevationFieldName, background, h0=0.0):
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
-            ray, hitPoint, hitDist, hitMask, hitHW = RayCasting2Lib.outdoorSingleRayCast25D(
+            ray, hitPoint, hitDist, hitMask, hitHW = RayCastingLib.singleRayCast25D(
                 masksGdf, masksSIdx, viewPoint, shootingDir, rayLength,
                 elevationFieldName, background, h0)
-            if not ray is None:
-                rays.append(ray)
-                hitPoints.append(hitPoint)
+            rays.append(ray)
+            hitPoints.append(hitPoint)
+            hitDists.append(hitDist)
+            hitMasks.append(hitMask)
+            hitHWs.append(hitHW)
+
+        return [MultiLineString(rays), hitPoints, hitDists, hitMasks, hitHWs]
+
+    @staticmethod
+    def multipleRayCastOnTopOfRoof(masksGdf, masksSIdx, viewPoint, shootingDirs,
+                                   rayLength, enclosingFeatures, elevationFieldName,
+                                   background):
+        if not isinstance(masksGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(masksGdf, 'GeoDataFrame')
+        if not isinstance(masksSIdx, (Index, PyGEOSSTRTreeIndex, SpatialIndex)):
+            raise IllegalArgumentTypeException(
+                masksSIdx, 'Index, PyGEOSSTRTreeIndex or SpatialIndex')
+        if not isinstance(viewPoint, Point):
+            raise IllegalArgumentTypeException(viewPoint, 'Point')
+        if elevationFieldName not in masksGdf:
+            raise Exception('%s is not a relevant field name!' %
+                            (elevationFieldName))
+
+        rays, hitPoints, hitDists, hitMasks, hitHWs = [[], [], [], [], []]
+        h0 = min([f[elevationFieldName] for f in enclosingFeatures])
+
+        for shootingDir in shootingDirs:
+            ray, hitPoint, hitDist, hitMask, hitHW = RayCastingLib.singleRayCastOnTopOfRoof(
+                masksGdf, masksSIdx, viewPoint, shootingDir, rayLength, h0,
+                elevationFieldName, background)
+            rays.append(ray)
+            hitPoints.append(hitPoint)
             hitDists.append(hitDist)
             hitMasks.append(hitMask)
             hitHWs.append(hitHW)
 
         return [MultiLineString(rays), hitPoints, hitDists, hitMasks, hitHWs]
+
+    @staticmethod
+    def assessStreetWidth(masksGdf, masksSIdx, viewPoint, rayLength=100.0):
+        if GeomLib.isAnIndoorPoint(viewPoint, masksGdf):
+            return None, -1, [-1, -1]
+
+        _shootingDirs = RayCastingLib.prepareOrientedRays(
+            masksGdf, masksSIdx, viewPoint)
+        rays, _, hitDists, _ = RayCastingLib.multipleRayCast2D(
+            masksGdf, masksSIdx, viewPoint, _shootingDirs, rayLength)
+        return linemerge(rays), sum(hitDists), hitDists
```

### Comparing `t4gpd-0.9.0/t4gpd/commons/RayCasting3Lib.py` & `t4gpd-0.9.5/t4gpd/commons/RayCasting3Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/RayCasting4Lib.py` & `t4gpd-0.9.5/t4gpd/commons/RayCasting4Lib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/RotationLib.py` & `t4gpd-0.9.5/t4gpd/commons/RotationLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/SVFLib.py` & `t4gpd-0.9.5/t4gpd/commons/SVFLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ShannonEntropy.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/CircularityIndices.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 15 janv. 2021
+Created on 18 dec. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,52 +16,40 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from numpy import log2, log
+from numpy import pi, sqrt
+from t4gpd.commons.ChrystalAlgorithm import ChrystalAlgorithm
+from t4gpd.commons.DiameterLib import DiameterLib
+from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class ShannonEntropy(object):
+class CircularityIndices(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, probs):
-        '''
-        Constructor
-        '''
-        for prob in probs:
-            if not (0 <= prob <= 1):
-                raise IllegalArgumentTypeException(prob, 'float value between 0.0 and 1.0')
-        self.probs = probs
-
-    @staticmethod
-    def createFromIntValuesArray(intValues):
-        mapOfNbOccurrences = dict()
-        for value in intValues:
-            if value in mapOfNbOccurrences:
-                mapOfNbOccurrences[value] += 1
-            else:
-                mapOfNbOccurrences[value] = 1
-        probs = [float(nbOccurr) / len(intValues) for nbOccurr in list(mapOfNbOccurrences.values())]
-        return ShannonEntropy(probs)
-
-    @staticmethod
-    def createFromDoubleValuesArray(doubleValues, precision=1.0):
-        intValues = [int(x / precision) for x in doubleValues]
-        return ShannonEntropy.createFromIntValuesArray(intValues)
-
     @staticmethod
-    def createFromString(string):
-        arrayOfChars = [ord(c) for c in string]
-        return ShannonEntropy.createFromIntValuesArray(arrayOfChars)
-
-    def h(self, base=2):
-        if (2 == base):
-            return -sum([prob * log2(prob) for prob in self.probs if (0.0 < prob)])
-        elif (2 < base) and (isinstance(base, int)):
-            return -sum([prob * log(prob) / log(base) for prob in self.probs if (0.0 < prob)])
-        raise IllegalArgumentTypeException(base, 'int (greater or equal than 2)')
+    def runWithArgs(row):
+        geom = row.geometry
+        area, perim = geom.area, geom.length
+        _, diamLen, _ = DiameterLib.diameter(geom)
+
+        gravelius = perim / sqrt(4.0 * pi * area) if (0.0 < area) else None
+        jaggedness = (perim * perim) / area if (0.0 < area) else None
+        miller = (4.0 * pi * area) / (perim * perim) if (0.0 < perim) else None
+        morton = (4.0 * area) / (pi * diamLen * diamLen) if (0.0 < diamLen) else None
+
+        _, _, radius = ChrystalAlgorithm(geom).run()
+        mbcArea = pi * radius * radius        
+        areaCircDefect = area / mbcArea if (0.0 < mbcArea) else None
+
+        return {
+            'gravelius': gravelius,
+            'jaggedness': jaggedness,
+            'miller': miller,
+            'morton': morton,
+            'a_circ_def': areaCircDefect
+            }
```

### Comparing `t4gpd-0.9.0/t4gpd/commons/SphericalCartesianCoordinates.py` & `t4gpd-0.9.5/t4gpd/commons/SphericalCartesianCoordinates.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/SphericalProjectionLib.py` & `t4gpd-0.9.5/t4gpd/commons/SphericalProjectionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/TestUtils.py` & `t4gpd-0.9.5/t4gpd/commons/TestUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/TypeLib.py` & `t4gpd-0.9.5/t4gpd/commons/TypeLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/WarnUtils.py` & `t4gpd-0.9.5/t4gpd/commons/WarnUtils.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/Sequence.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_generation/Sequence.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequenceRadii.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_generation/SequenceRadii.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_generation/SequencesGeneration.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_generation/SequencesGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/AbstractMethod.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/AbstractMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/CrossroadRecognitionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FFTMethod.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/FFTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/FWTMethod.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/FWTMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/MeanAngularityMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/crossroads_identification/MeanVectorMethod.py` & `t4gpd-0.9.5/t4gpd/commons/crossroads_identification/MeanVectorMethod.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ellipse/EllipseLib.py` & `t4gpd-0.9.5/t4gpd/commons/ellipse/EllipseLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/ellipse/EllipticHullLib.py` & `t4gpd-0.9.5/t4gpd/commons/ellipse/EllipticHullLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/NeighborhoodLib.py` & `t4gpd-0.9.5/t4gpd/commons/graph/NeighborhoodLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/ShortestPathLib.py` & `t4gpd-0.9.5/t4gpd/graph/STShortestPath.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 21 nov. 2020
+Created on 12 nov. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -16,63 +16,56 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from dijkstar.algorithm import find_path, NoPathError
-from shapely.geometry import MultiLineString
-from shapely.wkt import loads
+from geopandas import GeoDataFrame
+from pandas import concat
+from shapely.geometry import Point
+from t4gpd.commons.GeoProcess import GeoProcess
+from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
 
-from t4gpd.commons.graph.AbstractUrbanGraphLib import AbstractUrbanGraphLib
 
-
-class ShortestPathLib(AbstractUrbanGraphLib):
+class STShortestPath(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, roads, roi=None):
+    def __init__(self, roads, fromPoints, toPoints):
         '''
         Constructor
         '''
-        self.roads, self.graph, self.ciVertices, self.icVertices, self.edges = AbstractUrbanGraphLib.initializeGraph(roads, roi)
-        self.spatialIdx = self.roads.sindex
-        self.roi = roi
-
-    def shortestPath(self, fromPoint, toPoint):
-        # Backup the input graph
-        _graph, _ciVertices, _icVertices, _edges = AbstractUrbanGraphLib.backupUrbanGraph(
-            self.graph, self.ciVertices, self.icVertices, self.edges)
-
-        if (fromPoint == toPoint):
-            return MultiLineString([]), 0.0
-
-        str_coord = AbstractUrbanGraphLib.hashCoord([fromPoint.x, fromPoint.y])
-        if str_coord in self.ciVertices:
-            fromIdx = self.ciVertices[str_coord]
-        else:
-            fromIdx, _ = AbstractUrbanGraphLib.addEndPoint(
-                self.roads, self.spatialIdx, self.graph, self.ciVertices, self.icVertices, self.edges, fromPoint)
+        if not isinstance(roads, GeoDataFrame):
+            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
+        if not isinstance(fromPoints, (GeoDataFrame, Point)):
+            raise IllegalArgumentTypeException(
+                fromPoints, "GeoDataFrame or single Point")
+        if not isinstance(toPoints, (GeoDataFrame, Point)):
+            raise IllegalArgumentTypeException(
+                toPoints, "GeoDataFrame or single Point")
+
+        self.graph = UrbanGraphFactory.create(roads, method="networkx")
 
-        str_coord = AbstractUrbanGraphLib.hashCoord([toPoint.x, toPoint.y])
-        if str_coord in self.ciVertices:
-            toIdx = self.ciVertices[str_coord]
+        self.roads = roads
+
+        if isinstance(fromPoints, GeoDataFrame):
+            self.fromPoints = list(fromPoints.centroid)
         else:
-            toIdx, _ = AbstractUrbanGraphLib.addEndPoint(
-                self.roads, self.spatialIdx, self.graph, self.ciVertices, self.icVertices, self.edges, toPoint)
+            self.fromPoints = [fromPoints]
 
-        try:
-            tmp = find_path(self.graph, fromIdx, toIdx, cost_func=AbstractUrbanGraphLib.cost_function)
-            pathGeom = MultiLineString([loads(wkt) for _, wkt in tmp.edges])
-            pathLen = tmp.total_cost
-
-        except NoPathError as error:
-            pathGeom, pathLen = None, None
-            print(error)
-
-        finally:
-            # Rollback to the input graph (must be executed under all circumstances)
-            self.graph, self.ciVertices, self.icVertices, self.edges = _graph, _ciVertices, _icVertices, _edges
+        if isinstance(toPoints, GeoDataFrame):
+            self.toPoints = list(toPoints.centroid)
+        else:
+            self.toPoints = [toPoints]
 
-        return pathGeom, pathLen
+    def run(self):
+        gdfs = []
+        for fromPoint in self.fromPoints:
+            for toPoint in self.toPoints:
+                gdfs.append(self.graph.shortest_path(fromPoint, toPoint))
+
+        result = GeoDataFrame(concat(gdfs), crs=self.roads.crs)
+        result["gid"] = range(len(result))
+        return result
```

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraph.py` & `t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraph.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphFactory.py` & `t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphFactory.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphLib.py` & `t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphLibOld.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,37 +16,99 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from shapely.geometry import LineString, Point
-from t4gpd.commons.graph.AbstractUrbanGraphLib import AbstractUrbanGraphLib
+from shapely.geometry import LinearRing, LineString, Point, Polygon
 
+from t4gpd.commons.GeomLib import GeomLib
 
-class UrbanGraphLib(AbstractUrbanGraphLib):
+
+class UrbanGraphLibOld(object):
     '''
     classdocs
     '''
 
-    def __init__(self, roads):
+    def __init__(self):
         '''
         Constructor
         '''
-        self.roads, self.graph, self.ciVertices, self.icVertices, self.edges = AbstractUrbanGraphLib.initializeGraph(roads)
-        self.spatialIdx = self.roads.sindex
+        self.ciVertices = dict()
+        self.icVertices = dict()
+        self.edges = dict()
+
+    def add(self, features):
+        if isinstance(features, list):
+            for feature in features:
+                self.add(feature)
+        else:
+            if GeomLib.isAShapelyGeometry(features):
+                geom = features
+            else:
+                geom = features.geometry
+
+            if GeomLib.isMultipart(geom):
+                for g in geom.geoms:
+                    self.add(g)
+            elif isinstance(geom, LineString):
+                self.__addPolyline(geom)
+            elif isinstance(geom, Polygon):
+                self.__addPolyline(geom.exterior)
+                for g in geom.interiors:
+                    self.__addPolyline(g)
+            else:
+                raise Exception('Illegal argument in UrbanGraphLib.add(...)!')
+        # print('self.icVertices: %s' % self.icVertices)
+        # print('self.edges: %s' % self.edges)
+
+    def __addPolyline(self, line):
+        if isinstance(line, LinearRing):
+            coords = line.coords[:-1]
+        else:
+            coords = line.coords
+
+        if (2 <= len(coords)):
+            prev = self.__addAndGetANode(coords[0])
+            for i in range(1, len(coords)):
+                curr = self.__addAndGetANode(coords[i]);
+                if self.edges.get(prev) is None:
+                    self.edges[prev] = set([ curr ])
+                else:
+                    self.edges[prev].add(curr)
+                if self.edges.get(curr) is None:
+                    self.edges[curr] = set([ prev ])
+                else:
+                    self.edges[curr].add(prev)
+                prev = curr;
+
+    @staticmethod
+    def hashCoord(coord):
+        str_coord = ('%f_%f') % (coord[0], coord[1])
+        return str_coord
+
+    def __addAndGetANode(self, coord):
+        str_coord = UrbanGraphLibOld.hashCoord(coord)
+        if self.ciVertices.get(str_coord) is None:
+            nodeIndex = len(self.ciVertices)
+            self.ciVertices[str_coord] = nodeIndex
+            self.icVertices[nodeIndex] = coord
+            return nodeIndex   
+        else:
+            nodeIndex = self.ciVertices[str_coord]
+            return nodeIndex   
 
     def getUniqueRoadsSectionsNodes(self):
         result = list()
-        for k, v in self.edges.items():
+        for k, v in list(self.edges.items()):
             nbConnectedVertices = len(v)
             if 2 != nbConnectedVertices:
-                result.append({'geometry': Point(self.icVertices[k]), 'gid': k,
-                               'nb_connections': nbConnectedVertices })
+                result.append({ 'geometry': Point(self.icVertices[k]), 'gid': k,
+                               'valency': nbConnectedVertices })
         return result
 
     def __getNextVertex(self, prev, curr):
         succ = list(self.edges[curr])
         if 2 == len(succ):
             if (prev == succ[0]) and not (prev == succ[1]):
                 return succ[1]
@@ -58,15 +120,15 @@
         minIdx = min(idx1, idx2)
         maxidx = max(idx1, idx2)
         if minIdx in burnedEdges:
             burnedEdges[minIdx].add(maxidx)
         else:
             burnedEdges[minIdx] = set({ maxidx })
 
-    def __buildRoadSection(self, vertexIndex, nextVertexIndex, burnedEdges):
+    def _buildRoadSection(self, vertexIndex, nextVertexIndex, burnedEdges):
         result = []
 
         prevIdx = vertexIndex
         result.append(self.icVertices[prevIdx])
         currIdx = nextVertexIndex
         result.append(self.icVertices[currIdx])
         self.__burnEdge(prevIdx, currIdx, burnedEdges)
@@ -93,24 +155,24 @@
             nbConnectedVertices = len(self.edges[vertexIndex])
             if 2 != nbConnectedVertices:
                 # current vertex is a 'boundary' of a 'road section'
                 for nextVertexIndex in self.edges[vertexIndex]:
                     minIdx = min(vertexIndex, nextVertexIndex)
                     maxIdx = max(vertexIndex, nextVertexIndex)
                     if not (minIdx in burnedEdges and (maxIdx in burnedEdges[minIdx])):
-                        geom = self.__buildRoadSection(vertexIndex, nextVertexIndex, burnedEdges)
+                        geom = self._buildRoadSection(vertexIndex, nextVertexIndex, burnedEdges)
                         result.append({ 'geometry': geom, 'gid': len(result),
                                        'distance': geom.length })
         return result
 
     def getUniqueRoadsSectionsWithoutCulDeSac(self):
         result = []
 
         rs = self.getUniqueRoadsSections()
         for row in rs:
             _coords = list(row['geometry'].coords)
-            startHash = UrbanGraphLib.hashCoord(_coords[0])
-            stopHash = UrbanGraphLib.hashCoord(_coords[-1])
+            startHash = UrbanGraphLibOld.hashCoord(_coords[0])
+            stopHash = UrbanGraphLibOld.hashCoord(_coords[-1])
             if ((1 < len(self.edges[self.ciVertices[startHash]])) and
                 (1 < len(self.edges[self.ciVertices[stopHash]]))):
                 result.append(row)
         return result
```

### Comparing `t4gpd-0.9.0/t4gpd/commons/graph/UrbanGraphVertex.py` & `t4gpd-0.9.5/t4gpd/commons/graph/UrbanGraphVertex.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/grid/AbstractGridLib.py` & `t4gpd-0.9.5/t4gpd/commons/grid/AbstractGridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/grid/GridLib.py` & `t4gpd-0.9.5/t4gpd/commons/grid/GridLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/moon/MoonLib.py` & `t4gpd-0.9.5/t4gpd/commons/moon/MoonLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionLib.py` & `t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfPointsLib.py` & `t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfPointsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py` & `t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfSpheresLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/proj/DoubleProjectionOfWallsLib.py` & `t4gpd-0.9.5/t4gpd/commons/proj/DoubleProjectionOfWallsLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/raycasting/PanopticRaysLib.py` & `t4gpd-0.9.5/t4gpd/commons/raycasting/PanopticRaysLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/raycasting/PrepareMasksLib.py` & `t4gpd-0.9.5/t4gpd/commons/raycasting/PrepareMasksLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting25DLib.py` & `t4gpd-0.9.5/t4gpd/commons/raycasting/RayCasting25DLib.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         alt0 = min([ray.coords[0][2] for ray in _rays], initial=0)
         rayDeltaAlts = full(nRays, default_height-alt0)
         for i, ray_id in enumerate(ray_ids):
             rayDeltaAlts[ray_id] = _rayDeltaAlts[i]
         return rayDeltaAlts
 
     @staticmethod
-    def multipleRayCast25D(viewpoints, buildings, rays, nRays, rayLength, elevationFieldName,
+    def multipleRayCast25D(viewpoints, buildings, rays, nRays, elevationFieldName,
                            withIndices, h0=0.0, threshold=1e-9):
         if not GeoDataFrameLib.shareTheSameCrs(buildings, rays):
             raise Exception(
                 "Illegal argument: buildings and rays must share shames CRS!")
         # rays.to_csv("/tmp/1.csv", index=False) # DEBUG
 
         rays.geometry = rays.geometry.apply(lambda geom: GeomLib.forceZCoordinateToZ0(
@@ -138,16 +138,20 @@
             # Debug 25.03.2024
             smapRaysField.geometry = smapRaysField.apply(
                 lambda row: GeomLib.forceZCoordinateToZ0(
                     row.geometry, row[elevationFieldName]),
                 axis=1)
             # smapRaysField.to_csv("/tmp/2.csv") # DEBUG
 
-            smapRaysField = smapRaysField.dissolve(by=["__VPT_ID__", "__RAY_ID__"], as_index=False, aggfunc={
-                "gid": "first", "viewpoint": "first"})
+            # Debug 06.05.2024
+            # smapRaysField = smapRaysField.dissolve(
+            #     by=["__VPT_ID__", "__RAY_ID__"], as_index=False, aggfunc={
+            #     "gid": "first", "viewpoint": "first"})
+            smapRaysField = smapRaysField.dissolve(
+                by=["__VPT_ID__", "__RAY_ID__"], as_index=False, aggfunc="first")
             # smapRaysField.to_csv("/tmp/3.csv") # DEBUG
             smapRaysField.geometry = smapRaysField.apply(lambda row: RayCasting25DLib.__keepTheLargestSolidAngle(
                 row.viewpoint, row.geometry, threshold), axis=1)
             # smapRaysField.to_csv("/tmp/31.csv") # DEBUG
 
             left = rays.set_index(["__VPT_ID__", "__RAY_ID__"], drop=False)
             left.drop(columns=["__VPT_ID__"], inplace=True)
@@ -176,22 +180,31 @@
                 "gid", "geometry"]]
             viewpoints2 = sjoin_nearest(
                 viewpoints2, buildings[["geometry", elevationFieldName]])
             viewpoints2 = viewpoints2[["gid", elevationFieldName]].groupby(
                 by="gid").agg("mean").to_dict("index")
             viewpoints2 = {
                 key: viewpoints2[key][elevationFieldName] for key in viewpoints2.keys()}
+            # FROM: ...apply(lambda row: ... if ... else None)
+            # TO: ...apply(lambda row: ... if ... else h0)
+            # Debug 30.04.2024
             smapRaysField["__HAUTEUR_VP__"] = smapRaysField.apply(
-                lambda row: viewpoints2[row.gid] if row.gid in viewpoints2 else None,
+                lambda row: viewpoints2[row.gid] if row.gid in viewpoints2 else h0,
                 axis=1)
         # smapRaysField.to_csv("/tmp/4.csv") # DEBUG
 
-        smapRaysField = smapRaysField.dissolve(
-            by="__VPT_ID__", as_index=False, aggfunc={
-                "__RAY_ID__": list, "gid": "first", "viewpoint": "first", "__HAUTEUR_VP__": "first"})
+        # Debug 06.05.2024
+        # smapRaysField = smapRaysField.dissolve(
+        #     by="__VPT_ID__", as_index=False, aggfunc={
+        #         "__RAY_ID__": list, "gid": "first", "viewpoint": "first", "__HAUTEUR_VP__": "first"})
+        aggfunc = dict({"__RAY_ID__": list})
+        for f in smapRaysField.columns:
+            if f not in ["__VPT_ID__", "__RAY_ID__", "geometry"]:
+                aggfunc[f] = "first"
+        smapRaysField = smapRaysField.dissolve(by="__VPT_ID__", as_index=False, aggfunc=aggfunc)
         smapRaysField.drop(columns=["__VPT_ID__"], inplace=True)
         # smapRaysField.to_csv("/tmp/5.csv") # DEBUG
 
         if (0 < len(smapRaysField)):
             smapRaysField["__RAY_LEN__"] = smapRaysField.apply(
                 lambda row: RayCasting25DLib.__from25DRaysToRayLengths(nRays, row.__RAY_ID__, row.geometry), axis=1)
             smapRaysField["__RAY_ALT__"] = smapRaysField.apply(
```

### Comparing `t4gpd-0.9.0/t4gpd/commons/raycasting/RayCasting2DLib.py` & `t4gpd-0.9.5/t4gpd/commons/raycasting/RayCasting2DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/rnd/RandomPointPicking.py` & `t4gpd-0.9.5/t4gpd/commons/rnd/RandomPointPicking.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/AbstractSunLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/AbstractSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/DaylightLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/DaylightLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/PySolarSunLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/PySolarSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/ShadowLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/ShadowLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/SoleneSunLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/SoleneSunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/SunBeamLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/SunBeamLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/commons/sun/SunLib.py` & `t4gpd-0.9.5/t4gpd/commons/sun/SunLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/AbstractGeoDataFrameDemos.py` & `t4gpd-0.9.5/t4gpd/demos/AbstractGeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos2.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos3.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos3.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos4.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos4.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos5.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos5.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos6.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos6.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos7.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos7.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos8.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos8.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemos9.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemos9.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosA.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosA.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosB.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosB.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/GeoDataFrameDemosC.py` & `t4gpd-0.9.5/t4gpd/demos/GeoDataFrameDemosC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/demos/NantesBDT.py` & `t4gpd-0.9.5/t4gpd/demos/NantesBDT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/Angstrom.py` & `t4gpd-0.9.5/t4gpd/energy/Angstrom.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/DirectSolarIrradianceLib.py` & `t4gpd-0.9.5/t4gpd/energy/DirectSolarIrradianceLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/Dogniaux.py` & `t4gpd-0.9.5/t4gpd/energy/Dogniaux.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/FelixMarboutin.py` & `t4gpd-0.9.5/t4gpd/energy/FelixMarboutin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/Perez.py` & `t4gpd-0.9.5/t4gpd/energy/Perez.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/Perraudeau.py` & `t4gpd-0.9.5/t4gpd/energy/Perraudeau.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/PerrinDeBrichambaut.py` & `t4gpd-0.9.5/t4gpd/energy/PerrinDeBrichambaut.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/PlotDirectNormalIrradiance.py` & `t4gpd-0.9.5/t4gpd/energy/PlotDirectNormalIrradiance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/PlotIrradiances.py` & `t4gpd-0.9.5/t4gpd/energy/PlotIrradiances.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/WilliamAtkinson.py` & `t4gpd-0.9.5/t4gpd/energy/WilliamAtkinson.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py` & `t4gpd-0.9.5/t4gpd/energy/geoProcesses/DirectSolarIrradiation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STBetweennessCentrality.py` & `t4gpd-0.9.5/t4gpd/graph/STBetweennessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STClosenessCentrality.py` & `t4gpd-0.9.5/t4gpd/graph/STClosenessCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STDegreeCentrality.py` & `t4gpd-0.9.5/t4gpd/graph/STDegreeCentrality.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STDelaunayGraph.py` & `t4gpd-0.9.5/t4gpd/graph/STDelaunayGraph.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STMinimumSpanningTree.py` & `t4gpd-0.9.5/t4gpd/graph/STMinimumSpanningTree.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STRoadNeighborhood.py` & `t4gpd-0.9.5/t4gpd/graph/STRoadNeighborhood.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STShortestPath.py` & `t4gpd-0.9.5/t4gpd/isovist/STIsovistField2D_new.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 12 nov. 2020
+Created on 24 jul. 2023
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2023 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -17,55 +17,52 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas import GeoDataFrame
-from pandas import concat
-from shapely.geometry import Point
+from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.graph.UrbanGraphFactory import UrbanGraphFactory
+# from t4gpd.commons.raycasting.PrepareMasksLib import PrepareMasksLib
+from t4gpd.commons.raycasting.RayCasting2DLib import RayCasting2DLib
 
 
-class STShortestPath(GeoProcess):
+class STIsovistField2D_new(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, roads, fromPoints, toPoints):
+    def __init__(self, buildings, viewpoints, nRays=64, rayLength=100.0, withIndices=False):
         '''
         Constructor
         '''
-        if not isinstance(roads, GeoDataFrame):
-            raise IllegalArgumentTypeException(roads, "GeoDataFrame")
-        if not isinstance(fromPoints, (GeoDataFrame, Point)):
+        if not isinstance(buildings, GeoDataFrame):
             raise IllegalArgumentTypeException(
-                fromPoints, "GeoDataFrame or single Point")
-        if not isinstance(toPoints, (GeoDataFrame, Point)):
+                buildings, "buildings GeoDataFrame")
+        if not isinstance(viewpoints, GeoDataFrame):
             raise IllegalArgumentTypeException(
-                toPoints, "GeoDataFrame or single Point")
+                viewpoints, "viewpoints GeoDataFrame")
 
-        self.graph = UrbanGraphFactory.create(roads, method="networkx")
-
-        self.roads = roads
-
-        if isinstance(fromPoints, GeoDataFrame):
-            self.fromPoints = list(fromPoints.centroid)
-        else:
-            self.fromPoints = [fromPoints]
-
-        if isinstance(toPoints, GeoDataFrame):
-            self.toPoints = list(toPoints.centroid)
-        else:
-            self.toPoints = [toPoints]
+        if not GeoDataFrameLib.shareTheSameCrs(buildings, viewpoints):
+            raise Exception(
+                "Illegal argument: buildings and viewpoints must share shames CRS!")
+
+        self.buildings = buildings
+        # CLEAN GEOMETRIES
+        self.buildings.geometry = self.buildings.geometry.apply(
+            lambda g: g.buffer(0))
+
+        # the following instruction seems to slow down processing
+        # self.buildings = PrepareMasksLib.getMasksAsBipoints(
+        #     buildings, oriented=True, make_valid=True)
+
+        self.rays = RayCasting2DLib.get2DPanopticRaysGeoDataFrame(
+            viewpoints, rayLength, nRays)
+        self.nRays = nRays
+        self.withIndices = withIndices
 
     def run(self):
-        gdfs = []
-        for fromPoint in self.fromPoints:
-            for toPoint in self.toPoints:
-                gdfs.append(self.graph.shortest_path(fromPoint, toPoint))
-
-        result = GeoDataFrame(concat(gdfs), crs=self.roads.crs)
-        result["gid"] = range(len(result))
-        return result
+        isovRaysField, isovField = RayCasting2DLib.multipleRayCast2D(
+            self.buildings, self.rays, self.withIndices)
+        return isovRaysField, isovField
```

### Comparing `t4gpd-0.9.0/t4gpd/graph/STToRoadsSections.py` & `t4gpd-0.9.5/t4gpd/graph/STToRoadsSections.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/graph/STToRoadsSectionsNodes.py` & `t4gpd-0.9.5/t4gpd/graph/STToRoadsSectionsNodes.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/AbstractReader.py` & `t4gpd-0.9.5/t4gpd/io/AbstractReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CSVInertialSensorReader.py` & `t4gpd-0.9.5/t4gpd/io/CSVInertialSensorReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CSVReader.py` & `t4gpd-0.9.5/t4gpd/io/CSVReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CSVWKTReader.py` & `t4gpd-0.9.5/t4gpd/io/CSVWKTReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CSVWKTWriter.py` & `t4gpd-0.9.5/t4gpd/io/CSVWKTWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CirReader.py` & `t4gpd-0.9.5/t4gpd/io/CirReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CirValReader.py` & `t4gpd-0.9.5/t4gpd/io/CirValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CirWriter.py` & `t4gpd-0.9.5/t4gpd/io/CirWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/CityGMLReader.py` & `t4gpd-0.9.5/t4gpd/io/CityGMLReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/GeoWriter.py` & `t4gpd-0.9.5/t4gpd/io/GeoWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/GpkgLoader.py` & `t4gpd-0.9.5/t4gpd/io/GpkgLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/GpkgWriter.py` & `t4gpd-0.9.5/t4gpd/io/GpkgWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/MedReader.py` & `t4gpd-0.9.5/t4gpd/io/MedReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/MshReader.py` & `t4gpd-0.9.5/t4gpd/io/MshReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/ObjReader.py` & `t4gpd-0.9.5/t4gpd/io/ObjReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/ObjWriter.py` & `t4gpd-0.9.5/t4gpd/io/ObjWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/Reloading.py` & `t4gpd-0.9.5/t4gpd/io/Reloading.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/STLoadAndClip.py` & `t4gpd-0.9.5/t4gpd/io/STLoadAndClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/SVGWriter.py` & `t4gpd-0.9.5/t4gpd/io/SVGWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/SalomeWriter.py` & `t4gpd-0.9.5/t4gpd/io/SalomeWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/SalomeWriterAndExtruder.py` & `t4gpd-0.9.5/t4gpd/io/SalomeWriterAndExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/VTUWriter.py` & `t4gpd-0.9.5/t4gpd/io/VTUWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/ValReader.py` & `t4gpd-0.9.5/t4gpd/io/ValReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/ZipLoader.py` & `t4gpd-0.9.5/t4gpd/io/ZipLoader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/io/ZipWriter.py` & `t4gpd-0.9.5/t4gpd/io/ZipWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D.py` & `t4gpd-0.9.5/t4gpd/isovist/STIsovistField2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/isovist/STIsovistField2D_new.py` & `t4gpd-0.9.5/t4gpd/morph/STExtractOpenSpaces.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 24 jul. 2023
+Created on 14 dec. 2020
 
 @author: tleduc
 
-Copyright 2020-2023 Thomas Leduc
+Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,53 +16,48 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas import GeoDataFrame
-from t4gpd.commons.GeoDataFrameLib import GeoDataFrameLib
+from geopandas.geodataframe import GeoDataFrame
+from shapely.ops import unary_union
 from t4gpd.commons.GeoProcess import GeoProcess
+from t4gpd.commons.GeomLib import GeomLib
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-# from t4gpd.commons.raycasting.PrepareMasksLib import PrepareMasksLib
-from t4gpd.commons.raycasting.RayCasting2DLib import RayCasting2DLib
 
 
-class STIsovistField2D_new(GeoProcess):
+class STExtractOpenSpaces(GeoProcess):
     '''
     classdocs
     '''
+    EPSILON = 1e-3
 
-    def __init__(self, buildings, viewpoints, nRays=64, rayLength=100.0, withIndices=False):
+    def __init__(self, envelopeGdf, buildings, removeCourtyards=False):
         '''
         Constructor
         '''
-        if not isinstance(buildings, GeoDataFrame):
-            raise IllegalArgumentTypeException(
-                buildings, "buildings GeoDataFrame")
-        if not isinstance(viewpoints, GeoDataFrame):
-            raise IllegalArgumentTypeException(
-                viewpoints, "viewpoints GeoDataFrame")
-
-        if not GeoDataFrameLib.shareTheSameCrs(buildings, viewpoints):
-            raise Exception(
-                "Illegal argument: buildings and viewpoints must share shames CRS!")
+        if not isinstance(envelopeGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(envelopeGdf, 'GeoDataFrame')
+        self.envelopeGdf = envelopeGdf
 
+        if not isinstance(buildings, GeoDataFrame):
+            raise IllegalArgumentTypeException(buildings, 'GeoDataFrame')
         self.buildings = buildings
-        # CLEAN GEOMETRIES
-        self.buildings.geometry = self.buildings.geometry.apply(
-            lambda g: g.buffer(0))
-
-        # the following instruction seems to slow down processing
-        # self.buildings = PrepareMasksLib.getMasksAsBipoints(
-        #     buildings, oriented=True, make_valid=True)
-
-        self.rays = RayCasting2DLib.get2DPanopticRaysGeoDataFrame(
-            viewpoints, rayLength, nRays)
-        self.nRays = nRays
-        self.withIndices = withIndices
+
+        self.removeCourtyards = removeCourtyards
 
     def run(self):
-        isovRaysField, isovField = RayCasting2DLib.multipleRayCast2D(
-            self.buildings, self.rays, self.withIndices)
-        return isovRaysField, isovField
+        # Use a buffer to avoid slivers
+        xunion = lambda gdf: unary_union([g.buffer(self.EPSILON) for g in gdf.geometry]).buffer(self.EPSILON)
+
+        envelope = xunion(self.envelopeGdf)
+        buildings = xunion(self.buildings)
+        if self.removeCourtyards:
+            buildings = GeomLib.removeHoles(buildings)
+
+        result = envelope.difference(buildings)
+        # Use a buffer to avoid slivers
+        result = result.buffer(self.EPSILON)
+
+        return GeoDataFrame([{'geometry':result}], crs=self.buildings.crs)
```

### Comparing `t4gpd-0.9.0/t4gpd/misc/FrequencyHistogram.py` & `t4gpd-0.9.5/t4gpd/misc/FrequencyHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/OptimalNumberOfClusters.py` & `t4gpd-0.9.5/t4gpd/misc/OptimalNumberOfClusters.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/PlotAMatrixOfDiagrams.py` & `t4gpd-0.9.5/t4gpd/misc/PlotAMatrixOfDiagrams.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/PopulationPyramid.py` & `t4gpd-0.9.5/t4gpd/misc/PopulationPyramid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/RoseMappingTool.py` & `t4gpd-0.9.5/t4gpd/misc/RoseMappingTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/STCompass.py` & `t4gpd-0.9.5/t4gpd/misc/STCompass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 15 mars 2022
 
 @author: tleduc
 
-Copyright 2020-2022 Thomas Leduc
+Copyright 2020-2024 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -23,32 +23,35 @@
 from geopandas import GeoDataFrame
 from matplotlib.colors import ListedColormap
 from numpy import ndarray
 from shapely.affinity import translate, scale
 from shapely.geometry import Point, Polygon
 from t4gpd.commons.GeoProcess import GeoProcess
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.morph.STBBox import STBBox
 
 
 class STCompass(GeoProcess):
     '''
     classdocs
     '''
 
-    def __init__(self, basemap, bounds, crs, magnitude=0.015):
+    def __init__(self, basemap, bounds, crs, magnitude=0.015, bgcolor="white"):
         '''
         Constructor
         '''
         if isinstance(bounds, (list, tuple, ndarray)) and (4 == len(bounds)):
             self.basemap = basemap
             self.bounds = bounds
             self.crs = crs
             self.magnitude = magnitude
+            self.bgcolor = bgcolor
         else:
-            raise IllegalArgumentTypeException(bounds, 'box (minx, miny, maxx, maxy)')
+            raise IllegalArgumentTypeException(
+                bounds, "box (minx, miny, maxx, maxy)")
 
     @staticmethod
     def __letter():
         h, w = 1.45, 0.45
         return Polygon([(-0.5 - w, 3), (-0.5, 3), (-0.5, 3 + h - w), (0.5, 3),
                         (0.5 + w, 3), (0.5 + w, 3 + h), (0.5, 3 + h), (0.5, 3 + w),
                         (-0.5, 3 + h), (-0.5 - w, 3 + h)])
@@ -60,29 +63,49 @@
     @staticmethod
     def __right_arrow():
         return Polygon([(0, 0), (2, -1.5), (0, 2)])
 
     def __translation_and_dilation(self, arrow):
         minx, miny, maxx, maxy = self.bounds
 
-        deltax, deltay = maxx - minx, maxy - miny 
+        deltax, deltay = maxx - minx, maxy - miny
         delta = min(deltax, deltay)
 
-        arrow = scale(arrow, xfact=self.magnitude * delta, yfact=self.magnitude * delta, origin=Point([0, 0]))
-        arrow = translate(arrow, xoff=minx + 2 * self.magnitude * delta, yoff=maxy - 4.5 * self.magnitude * delta)
+        arrow = scale(arrow, xfact=self.magnitude * delta,
+                      yfact=self.magnitude * delta, origin=Point([0, 0]))
+        arrow = translate(arrow, xoff=minx + 2 * self.magnitude *
+                          delta, yoff=maxy - 4.5 * self.magnitude * delta)
         return arrow
 
     def run(self):
         _left_arrow = self.__translation_and_dilation(self.__left_arrow())
         _right_arrow = self.__translation_and_dilation(self.__right_arrow())
         _letter = self.__translation_and_dilation(self.__letter())
 
-        my_rgb_cmap = ListedColormap(['white', 'black', 'black'])
+        my_rgb_cmap = ListedColormap(["white", "black", "black"])
 
         gdf = GeoDataFrame([
-            {'gid': 0, 'geometry': _left_arrow},
-            {'gid': 1, 'geometry': _right_arrow},
-            {'gid': 2, 'geometry': _letter}
-            ], crs=self.crs)
-        gdf.plot(ax=self.basemap, edgecolor='black', column='gid', cmap=my_rgb_cmap)
+            {"gid": 0, "geometry": _left_arrow},
+            {"gid": 1, "geometry": _right_arrow},
+            {"gid": 2, "geometry": _letter}
+        ], crs=self.crs)
+
+        bb = STBBox(gdf, buffDist=3).run()
+        bb.plot(ax=self.basemap, color=self.bgcolor, alpha=0.35)
+
+        gdf.plot(ax=self.basemap, edgecolor="black",
+                 column="gid", cmap=my_rgb_cmap)
 
         return gdf
+
+
+"""
+import matplotlib.pyplot as plt
+from t4gpd.demos.GeoDataFrameDemos import GeoDataFrameDemos
+
+buildings = GeoDataFrameDemos.ensaNantesBuildings()
+
+fig, ax = plt.subplots()
+buildings.plot(ax=ax)
+STCompass(ax, buildings.total_bounds, buildings.crs).run()
+plt.show()
+"""
```

### Comparing `t4gpd-0.9.0/t4gpd/misc/STDendrogram.py` & `t4gpd-0.9.5/t4gpd/misc/STDendrogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/STKMeans.py` & `t4gpd-0.9.5/t4gpd/misc/STKMeans.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/StreetOrientationHistogram.py` & `t4gpd-0.9.5/t4gpd/misc/StreetOrientationHistogram.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/TimelineTool.py` & `t4gpd-0.9.5/t4gpd/misc/TimelineTool.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/misc/WindRose.py` & `t4gpd-0.9.5/t4gpd/misc/WindRose.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/GmshTriangulator.py` & `t4gpd-0.9.5/t4gpd/morph/GmshTriangulator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STAdaptativeGrid.py` & `t4gpd-0.9.5/t4gpd/morph/STAdaptativeGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STBBox.py` & `t4gpd-0.9.5/t4gpd/morph/STBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STClip.py` & `t4gpd-0.9.5/t4gpd/morph/STClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STCoolscapesTessellation.py` & `t4gpd-0.9.5/t4gpd/morph/STCoolscapesTessellation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STCrossroadsGeneration.py` & `t4gpd-0.9.5/t4gpd/morph/STCrossroadsGeneration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STDilationErosion.py` & `t4gpd-0.9.5/t4gpd/morph/STDilationErosion.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STExtractOpenSpaces.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/WMean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Created on 14 dec. 2020
+Created on 28 sept. 2020
 
 @author: tleduc
 
 Copyright 2020 Thomas Leduc
 
 This file is part of t4gpd.
 
@@ -17,47 +17,39 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
 from geopandas.geodataframe import GeoDataFrame
-from shapely.ops import unary_union
-from t4gpd.commons.GeoProcess import GeoProcess
-from t4gpd.commons.GeomLib import GeomLib
+from numpy import mean
 from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
+from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
+from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class STExtractOpenSpaces(GeoProcess):
+class WMean(AbstractGeoprocess):
     '''
     classdocs
     '''
-    EPSILON = 1e-3
 
-    def __init__(self, envelopeGdf, buildings, removeCourtyards=False):
+    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
         '''
         Constructor
         '''
-        if not isinstance(envelopeGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(envelopeGdf, 'GeoDataFrame')
-        self.envelopeGdf = envelopeGdf
-
-        if not isinstance(buildings, GeoDataFrame):
-            raise IllegalArgumentTypeException(buildings, 'GeoDataFrame')
-        self.buildings = buildings
-
-        self.removeCourtyards = removeCourtyards
-
-    def run(self):
-        # Use a buffer to avoid slivers
-        xunion = lambda gdf: unary_union([g.buffer(self.EPSILON) for g in gdf.geometry]).buffer(self.EPSILON)
-
-        envelope = xunion(self.envelopeGdf)
-        buildings = xunion(self.buildings)
-        if self.removeCourtyards:
-            buildings = GeomLib.removeHoles(buildings)
-
-        result = envelope.difference(buildings)
-        # Use a buffer to avoid slivers
-        result = result.buffer(self.EPSILON)
-
-        return GeoDataFrame([{'geometry':result}], crs=self.buildings.crs)
+        if not isinstance(buildingsGdf, GeoDataFrame):
+            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
+        self.buildingsGdf = buildingsGdf
+
+        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
+        self.maxRayLen = maxRayLen
+
+    def runWithArgs(self, row):
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

### Comparing `t4gpd-0.9.0/t4gpd/morph/STFacadesAnalysis.py` & `t4gpd-0.9.5/t4gpd/morph/STFacadesAnalysis.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STGradientOfDistancesToBuildings.py` & `t4gpd-0.9.5/t4gpd/morph/STGradientOfDistancesToBuildings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STGrid.py` & `t4gpd-0.9.5/t4gpd/morph/STGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STHeightOfRoughness.py` & `t4gpd-0.9.5/t4gpd/morph/STHeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STIdentifyRowOfTrees.py` & `t4gpd-0.9.5/t4gpd/morph/STIdentifyRowOfTrees.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STMakeBlocks.py` & `t4gpd-0.9.5/t4gpd/morph/STMakeBlocks.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STMakeGroundSurface.py` & `t4gpd-0.9.5/t4gpd/morph/STMakeGroundSurface.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps.py` & `t4gpd-0.9.5/t4gpd/morph/STMultipleOverlaps.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STMultipleOverlaps2.py` & `t4gpd-0.9.5/t4gpd/morph/STMultipleOverlaps2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STPointsDensifier.py` & `t4gpd-0.9.5/t4gpd/morph/STPointsDensifier.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STPointsDensifier2.py` & `t4gpd-0.9.5/t4gpd/morph/STPointsDensifier2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STPolygonize.py` & `t4gpd-0.9.5/t4gpd/morph/STPolygonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSkeletonize.py` & `t4gpd-0.9.5/t4gpd/morph/STSkeletonize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSkeletonizeTheVoid.py` & `t4gpd-0.9.5/t4gpd/morph/STSkeletonizeTheVoid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines.py` & `t4gpd-0.9.5/t4gpd/morph/STSnappingPointsOnLines.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSnappingPointsOnLines2.py` & `t4gpd-0.9.5/t4gpd/morph/STSnappingPointsOnLines2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSpatialJoin.py` & `t4gpd-0.9.5/t4gpd/morph/STSpatialJoin.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSquaredBBox.py` & `t4gpd-0.9.5/t4gpd/morph/STSquaredBBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STSurfaceFraction.py` & `t4gpd-0.9.5/t4gpd/morph/STSurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STVariableWidthBuffer.py` & `t4gpd-0.9.5/t4gpd/morph/STVariableWidthBuffer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/STVoronoiPartition.py` & `t4gpd-0.9.5/t4gpd/morph/STVoronoiPartition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AbstractGeoprocess.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/AbstractGeoprocess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AngularAbscissa.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/AngularAbscissa.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AreaConvexityDefect.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/AreaConvexityDefect.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/AspectRatio.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/AspectRatio.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/BBox.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/BBox.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/BiggestInscribedDisc.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/CanyonStreetOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexHull.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/ConvexityIndices.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/ConvexityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadRecognition.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadRecognition.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsAngularity.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadsAngularity.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/CrossroadsStarDomain.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Diameter.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/Diameter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/EllipticityIndices.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/EllipticityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/FootprintExtruder.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/FootprintExtruder.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/GetInteriorPoint.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/GetInteriorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/GridFace.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/GridFace.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/HMean.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/HMean.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/HeightOfRoughness.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/HeightOfRoughness.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/IdentifyTheClosestPolyline.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/IsAnIndoorPoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABE.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABE.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MABR2.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/MABR2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MBC.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/MBC.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/MPBR.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/MPBR.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectangularityIndices.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectangularityIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFFT.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectifyByFFT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RectifyByFWT.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/RectifyByFWT.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RemoveHoles.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/RemoveHoles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/RepresentativePoint.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/RepresentativePoint.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Rotation2D.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/Rotation2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/STGeoProcess.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/STGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyMap2D.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactor.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyViewFactor.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/SkyViewFactorOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/StarShapedIndices.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/StarShapedIndices.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/SurfaceFraction.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/SurfaceFraction.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/Translation.py` & `t4gpd-0.9.5/t4gpd/morph/geoProcesses/Translation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/morph/geoProcesses/WMean.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/MoveSensorsAwayFromSurface.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
-Created on 28 sept. 2020
+Created on 22 juin 2022
 
 @author: tleduc
 
-Copyright 2020 Thomas Leduc
+Copyright 2020-2022 Thomas Leduc
 
 This file is part of t4gpd.
 
 t4gpd is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
@@ -16,40 +16,37 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with t4gpd.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from geopandas.geodataframe import GeoDataFrame
-from numpy import mean
-from t4gpd.commons.IllegalArgumentTypeException import IllegalArgumentTypeException
-from t4gpd.commons.RayCasting3Lib import RayCasting3Lib
+from geopandas import GeoDataFrame
+from shapely.geometry import Point
 from t4gpd.morph.geoProcesses.AbstractGeoprocess import AbstractGeoprocess
 
 
-class WMean(AbstractGeoprocess):
+class MoveSensorsAwayFromSurface(AbstractGeoprocess):
     '''
     classdocs
     '''
 
-    def __init__(self, buildingsGdf, nRays=64, maxRayLen=100.0):
+    def __init__(self, sensorsGdf, normalFieldname, dist=1e-6):
         '''
         Constructor
         '''
-        if not isinstance(buildingsGdf, GeoDataFrame):
-            raise IllegalArgumentTypeException(buildingsGdf, 'GeoDataFrame')
-        self.buildingsGdf = buildingsGdf
-
-        self.shootingDirs = RayCasting3Lib.preparePanopticRays(nRays)
-        self.maxRayLen = maxRayLen
+        assert isinstance(sensorsGdf, GeoDataFrame), 'sensorsGdf must be a GeoDataFrame'
+        assert (normalFieldname in sensorsGdf), 'f{normalFieldname} must be a sensorsGdf field name'
+        self.sensorsGdf = sensorsGdf
+        self.normalFieldname = normalFieldname
+        self.dist = dist
 
     def runWithArgs(self, row):
-        viewPoint = row.geometry.centroid
-
-        _, _, hitDists = RayCasting3Lib.outdoorMultipleRayCast2D(
-            self.buildingsGdf, viewPoint, self.shootingDirs, self.maxRayLen)
-
-        return {
-            # 'hit_dists': ArrayCoding.encode(hitDists),
-            'wmean': float(mean(hitDists))
-            }
+        p = row.geometry
+        assert isinstance(p, Point), 'sensorsGdf must be a GeoDataFrame of Points'
+        n = row[self.normalFieldname]
+
+        return { 'geometry': Point([
+            p.x + self.dist * n[0],
+            p.y + self.dist * n[1],
+            p.z + self.dist * n[2],
+            ]) }
```

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/CampbellSciReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/CampbellSciReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/ExtraProcessing.py` & `t4gpd-0.9.5/t4gpd/picoclim/ExtraProcessing.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReWriter.py` & `t4gpd-0.9.5/t4gpd/picoclim/InertialMeasureReWriter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/InertialMeasureReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/InertialMeasureReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/JoinByTimeDistance.py` & `t4gpd-0.9.5/t4gpd/picoclim/JoinByTimeDistance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/KestrelReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/KestrelReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/MeteoFranceReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/MeteoFranceReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignPlottings.py` & `t4gpd-0.9.5/t4gpd/picoclim/MetrologicalCampaignPlottings.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/MetrologicalCampaignReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/MetrologicalCampaignReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/SensirionReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/SensirionReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py` & `t4gpd-0.9.5/t4gpd/picoclim/SnapImuOnTrackUsingWaypoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py` & `t4gpd-0.9.5/t4gpd/picoclim/SnapUclimOnTrackUsingWaypoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/TracksWaypointsReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/TracksWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/UClimGuidingReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/UClimGuidingReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/picoclim/UClimTrackWaypointsReader.py` & `t4gpd-0.9.5/t4gpd/picoclim/UClimTrackWaypointsReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyplot/MultipleMarkerStyles.py` & `t4gpd-0.9.5/t4gpd/pyplot/MultipleMarkerStyles.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/AddMemoryLayer.py` & `t4gpd-0.9.5/t4gpd/pyqgis/AddMemoryLayer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/Emphasizer.py` & `t4gpd-0.9.5/t4gpd/pyqgis/Emphasizer.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/MapPrinter.py` & `t4gpd-0.9.5/t4gpd/pyqgis/MapPrinter.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/SetSymbolLib.py` & `t4gpd-0.9.5/t4gpd/pyqgis/SetSymbolLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/ShowFeatureCount.py` & `t4gpd-0.9.5/t4gpd/pyqgis/ShowFeatureCount.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyqgis/ZoomLib.py` & `t4gpd-0.9.5/t4gpd/pyqgis/ZoomLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/GeodeCiel.py` & `t4gpd-0.9.5/t4gpd/pyvista/GeodeCiel.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/Icosahedron.py` & `t4gpd-0.9.5/t4gpd/pyvista/Icosahedron.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/Plotter3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/Plotter3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/STRaysToViewFactors.py` & `t4gpd-0.9.5/t4gpd/pyvista/STRaysToViewFactors.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/ToPolyData.py` & `t4gpd-0.9.5/t4gpd/pyvista/ToPolyData.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/ToUnstructuredGrid.py` & `t4gpd-0.9.5/t4gpd/pyvista/ToUnstructuredGrid.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/commons/Diameter3DLib.py` & `t4gpd-0.9.5/t4gpd/pyvista/commons/Diameter3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/commons/RayCasting3DLib.py` & `t4gpd-0.9.5/t4gpd/pyvista/commons/RayCasting3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/commons/RayCastingIn3DLib.py` & `t4gpd-0.9.5/t4gpd/pyvista/commons/RayCastingIn3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/commons/SVF3DLib.py` & `t4gpd-0.9.5/t4gpd/pyvista/commons/SVF3DLib.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/commons/Triangle3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/commons/Triangle3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/AutomaticFaceOrientation.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/FromContourToNormalVector.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/OrientedRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/PanopticRayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/RayCasting3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/RayCasting3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/pyvista/geoProcesses/SVF3D.py` & `t4gpd-0.9.5/t4gpd/pyvista/geoProcesses/SVF3D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/AbstractRasterGeoProcess.py` & `t4gpd-0.9.5/t4gpd/raster/AbstractRasterGeoProcess.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTClip.py` & `t4gpd-0.9.5/t4gpd/raster/RTClip.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTFromArrayToRaster.py` & `t4gpd-0.9.5/t4gpd/raster/RTFromArrayToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py` & `t4gpd-0.9.5/t4gpd/raster/RTFromRasterToGeoDataFrameOfPoints.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTLoad.py` & `t4gpd-0.9.5/t4gpd/raster/RTLoad.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTNdvi.py` & `t4gpd-0.9.5/t4gpd/raster/RTNdvi.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTToFile.py` & `t4gpd-0.9.5/t4gpd/raster/RTToFile.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/RTVectorize.py` & `t4gpd-0.9.5/t4gpd/raster/RTVectorize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/STFromGridToRaster.py` & `t4gpd-0.9.5/t4gpd/raster/STFromGridToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/STRasterize.py` & `t4gpd-0.9.5/t4gpd/raster/STRasterize.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/raster/STToRaster.py` & `t4gpd-0.9.5/t4gpd/raster/STToRaster.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/AbstractHardShadow.py` & `t4gpd-0.9.5/t4gpd/sun/AbstractHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/STHardShadow.py` & `t4gpd-0.9.5/t4gpd/sun/STHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/STSunMap2D.py` & `t4gpd-0.9.5/t4gpd/sun/STSunMap2D.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow.py` & `t4gpd-0.9.5/t4gpd/sun/STTreeHardShadow.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/STTreeHardShadow2.py` & `t4gpd-0.9.5/t4gpd/sun/STTreeHardShadow2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py` & `t4gpd-0.9.5/t4gpd/sun/geoProcesses/AbstractSunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDuration.py` & `t4gpd-0.9.5/t4gpd/sun/geoProcesses/SunshineDuration.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py` & `t4gpd-0.9.5/t4gpd/sun/geoProcesses/SunshineDurationOnTopOfRoof.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/wrf/MeteoFranceAggregator.py` & `t4gpd-0.9.5/t4gpd/wrf/MeteoFranceAggregator.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/wrf/MeteoFrancePredictor.py` & `t4gpd-0.9.5/t4gpd/wrf/MeteoFrancePredictor.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/wrf/MeteoFranceReader.py` & `t4gpd-0.9.5/t4gpd/wrf/MeteoFranceReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance.py` & `t4gpd-0.9.5/t4gpd/wrf/SkyMapRadiationBalance.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/wrf/SkyMapRadiationBalance2.py` & `t4gpd-0.9.5/t4gpd/wrf/SkyMapRadiationBalance2.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd/ws/BDTopoWFSReader.py` & `t4gpd-0.9.5/t4gpd/ws/BDTopoWFSReader.py`

 * *Files identical despite different names*

### Comparing `t4gpd-0.9.0/t4gpd.egg-info/PKG-INFO` & `t4gpd-0.9.5/t4gpd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4gpd
-Version: 0.9.0
+Version: 0.9.5
 Summary: Set of tools based on Python, GeoPandas and Shapely to achieve urban geoprocessing
 Home-page: https://t4gpd-docs.readthedocs.io
 Download-URL: https://sourcesup.renater.fr/frs/?group_id=463
 Author: Thomas Leduc
 Author-email: thomas.leduc@crenau.archi.fr
 License: GPLv3+
 Keywords: Geospatial analysis,Urban form,Urban morphology,Isovist
@@ -42,14 +42,14 @@
 > pip install dijkstar pythermalcomfort suntimes
 
 ## Installation instructions
 As **t4gpd** is now on [PyPI](https://pypi.org/project/t4gpd/), the easiest way to install the latest version is to use the pip command as follows:
 > pip install t4gpd
 
 Alternatively, you can download the **t4gpd** latest version from the [SourceSup website](https://sourcesup.renater.fr/projects/t4gs). Then, install the Python3 plugin you downloaded:
-> pip install t4gpd-0.9.0.tar.gz
+> pip install t4gpd-0.9.5.tar.gz
 
 ## Read the documentation
 Go to [https://t4gpd-docs.readthedocs.io](https://t4gpd-docs.readthedocs.io) to consult the documentation.
```

### Comparing `t4gpd-0.9.0/t4gpd.egg-info/SOURCES.txt` & `t4gpd-0.9.5/t4gpd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -94,21 +94,19 @@
 t4gpd/commons/ListUtilities.py
 t4gpd/commons/Logos.py
 t4gpd/commons/MyEdge.py
 t4gpd/commons/MyNode.py
 t4gpd/commons/PointsDensifierLib.py
 t4gpd/commons/PointsDensifierLib3D.py
 t4gpd/commons/PolarCartesianCoordinates.py
-t4gpd/commons/RayCasting2Lib.py
 t4gpd/commons/RayCasting3Lib.py
 t4gpd/commons/RayCasting4Lib.py
 t4gpd/commons/RayCastingLib.py
 t4gpd/commons/RotationLib.py
 t4gpd/commons/SVFLib.py
-t4gpd/commons/ShannonEntropy.py
 t4gpd/commons/SphericalCartesianCoordinates.py
 t4gpd/commons/SphericalProjectionLib.py
 t4gpd/commons/TestUtils.py
 t4gpd/commons/TypeLib.py
 t4gpd/commons/WarnUtils.py
 t4gpd/commons/__init__.py
 t4gpd/commons/crossroads_generation/Sequence.py
@@ -121,21 +119,17 @@
 t4gpd/commons/crossroads_identification/FWTMethod.py
 t4gpd/commons/crossroads_identification/MeanAngularityMethod.py
 t4gpd/commons/crossroads_identification/MeanVectorMethod.py
 t4gpd/commons/crossroads_identification/__init__.py
 t4gpd/commons/ellipse/EllipseLib.py
 t4gpd/commons/ellipse/EllipticHullLib.py
 t4gpd/commons/ellipse/__init__.py
-t4gpd/commons/graph/AbstractUrbanGraphLib.py
-t4gpd/commons/graph/MCALib.py
 t4gpd/commons/graph/NeighborhoodLib.py
-t4gpd/commons/graph/ShortestPathLib.py
 t4gpd/commons/graph/UrbanGraph.py
 t4gpd/commons/graph/UrbanGraphFactory.py
-t4gpd/commons/graph/UrbanGraphLib.py
 t4gpd/commons/graph/UrbanGraphLibOld.py
 t4gpd/commons/graph/UrbanGraphVertex.py
 t4gpd/commons/graph/__init__.py
 t4gpd/commons/grid/AbstractGridLib.py
 t4gpd/commons/grid/GridLib.py
 t4gpd/commons/grid/__init__.py
 t4gpd/commons/isovists/__init__.py
@@ -330,15 +324,14 @@
 t4gpd/picoclim/UClimTrackWaypointsReader.py
 t4gpd/picoclim/__init__.py
 t4gpd/pyplot/MultipleMarkerStyles.py
 t4gpd/pyplot/__init__.py
 t4gpd/pyqgis/AddMemoryLayer.py
 t4gpd/pyqgis/Emphasizer.py
 t4gpd/pyqgis/MapPrinter.py
-t4gpd/pyqgis/PdfMapWriter.py
 t4gpd/pyqgis/SetSymbolLib.py
 t4gpd/pyqgis/ShowFeatureCount.py
 t4gpd/pyqgis/ZoomLib.py
 t4gpd/pyqgis/__init__.py
 t4gpd/pyvista/GeodeCiel.py
 t4gpd/pyvista/Icosahedron.py
 t4gpd/pyvista/Plotter3D.py
```

