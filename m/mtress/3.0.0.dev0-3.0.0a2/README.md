# Comparing `tmp/mtress-3.0.0.dev0.tar.gz` & `tmp/mtress-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtress-3.0.0.dev0.tar", last modified: Fri Apr 22 10:03:36 2022, max compression
+gzip compressed data, was "mtress-3.0.0a2.tar", last modified: Thu May 16 19:52:23 2024, max compression
```

## Comparing `mtress-3.0.0.dev0.tar` & `mtress-3.0.0a2.tar`

### file list

```diff
@@ -1,39 +1,86 @@
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.335854 mtress-3.0.0.dev0/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1136 2022-01-11 14:30:13.000000 mtress-3.0.0.dev0/LICENSE
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1483 2022-04-22 10:03:36.335854 mtress-3.0.0.dev0/PKG-INFO
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      649 2022-01-10 18:35:49.000000 mtress-3.0.0.dev0/README.md
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.195187 mtress-3.0.0.dev0/example/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      291 2022-01-11 14:30:13.000000 mtress-3.0.0.dev0/example/__init__.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     5477 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/example/example.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.210818 mtress-3.0.0.dev0/mtress/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      470 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/__init__.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.242075 mtress-3.0.0.dev0/mtress/_helpers/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      247 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/_helpers/__init__.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      702 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/_helpers/_array_cast.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)    38787 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/_meta_model.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     2645 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/_run_mtress.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.257705 mtress-3.0.0.dev0/mtress/physics/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1033 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/physics/__init__.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      813 2022-01-10 18:35:49.000000 mtress-3.0.0.dev0/mtress/physics/_constants.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     2123 2022-04-22 10:02:26.000000 mtress-3.0.0.dev0/mtress/physics/_helper_functions.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.304595 mtress-3.0.0.dev0/mtress/technologies/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      594 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/__init__.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1424 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/_generic_technology.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     2114 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/_photovoltaics.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1478 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/_renewable_electricity_source.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      855 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/_wind_turbine.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.320233 mtress-3.0.0.dev0/mtress/technologies/layered_heat/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      455 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/layered_heat/__init__.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     2818 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/layered_heat/_heat_exchanger.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     4870 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/layered_heat/_heat_layers.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     5073 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/layered_heat/_layered_heat_pump.py
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     5367 2022-04-22 10:02:27.000000 mtress-3.0.0.dev0/mtress/technologies/layered_heat/_multi_layer_storage.py
-drwxrwxrwx   0 patrik    (1000) patrik    (1000)        0 2022-04-22 10:03:36.242075 mtress-3.0.0.dev0/mtress.egg-info/
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1483 2022-04-22 10:03:35.000000 mtress-3.0.0.dev0/mtress.egg-info/PKG-INFO
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)      918 2022-04-22 10:03:36.000000 mtress-3.0.0.dev0/mtress.egg-info/SOURCES.txt
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)        1 2022-04-22 10:03:35.000000 mtress-3.0.0.dev0/mtress.egg-info/dependency_links.txt
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)        1 2022-01-10 18:37:49.000000 mtress-3.0.0.dev0/mtress.egg-info/not-zip-safe
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)       58 2022-04-22 10:03:35.000000 mtress-3.0.0.dev0/mtress.egg-info/requires.txt
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)       15 2022-04-22 10:03:35.000000 mtress-3.0.0.dev0/mtress.egg-info/top_level.txt
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)       38 2022-04-22 10:03:36.335854 mtress-3.0.0.dev0/setup.cfg
--rwxrwxrwx   0 patrik    (1000) patrik    (1000)     1279 2022-04-22 10:02:34.000000 mtress-3.0.0.dev0/setup.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1105 2024-05-16 19:37:48.000000 mtress-3.0.0a2/LICENSE
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2855 2024-05-16 19:52:23.826678 mtress-3.0.0a2/PKG-INFO
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1833 2024-05-16 19:37:48.000000 mtress-3.0.0a2/README.md
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.818678 mtress-3.0.0a2/mtress/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      437 2024-05-16 19:45:20.000000 mtress-3.0.0a2/mtress/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     5383 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_abstract_component.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2914 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_data_handler.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/_helpers/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      447 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_helpers/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      757 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_helpers/_array_cast.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1508 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_helpers/_results.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3496 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_helpers/_util.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1782 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_helpers/_visualization.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      613 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_interfaces.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3921 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_location.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3341 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_meta_model.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     7041 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_oemof_storage_multiplexer.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2662 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_run_mtress.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3847 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/_solph_model.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/carriers/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      303 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/carriers/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1802 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/carriers/_abstract_carrier.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1723 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/carriers/_electricity.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2341 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/carriers/_gas.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     7008 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/carriers/_heat.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/demands/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      275 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      228 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/_abstract_demand.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2282 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/_electricity.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     5182 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/_fixed_temperature_heat.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2215 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/_gas.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2017 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/demands/_heat_sink.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/physics/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1638 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/physics/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      853 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/physics/_constants.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     4956 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/physics/_gas_definition.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3792 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/physics/_helper_functions.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/technologies/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1651 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     5261 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_abstract_homogenous_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2126 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_abstract_technology.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2347 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_air_heat_exchanger.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2849 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_battery_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)    10339 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_chp.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2830 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_compressor.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     6811 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_electrolyser.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     8672 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_fuel_cell.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2643 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_geothermal_heat_exchanger.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     5534 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heat_pump.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.822678 mtress-3.0.0a2/mtress/technologies/_heat_storage/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      362 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heat_storage/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1637 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heat_storage/_abstract_heat_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3156 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heat_storage/_fully_mixed_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     5076 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heat_storage/_multi_layer_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2441 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_heating_rod.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     6399 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_photovoltaics.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/mtress/technologies/_pressure_storage/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      169 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_pressure_storage/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2773 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_pressure_storage/_gas_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1199 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_pressure_storage/_h2_storage.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2310 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/_renewable_electricity_source.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/mtress/technologies/grid_connection/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      161 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      759 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/_abstract_gas_grid_connection.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      272 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/_abstract_grid_connection.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2472 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/_electricity.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2505 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/_gas.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1257 2024-05-16 19:37:48.000000 mtress-3.0.0a2/mtress/technologies/grid_connection/_heat.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/mtress.egg-info/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2855 2024-05-16 19:52:23.000000 mtress-3.0.0a2/mtress.egg-info/PKG-INFO
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2478 2024-05-16 19:52:23.000000 mtress-3.0.0a2/mtress.egg-info/SOURCES.txt
+-rw-r--r--   0 patrik    (1000) patrik    (1000)        1 2024-05-16 19:52:23.000000 mtress-3.0.0a2/mtress.egg-info/dependency_links.txt
+-rw-r--r--   0 patrik    (1000) patrik    (1000)        1 2024-05-16 19:51:44.000000 mtress-3.0.0a2/mtress.egg-info/not-zip-safe
+-rw-r--r--   0 patrik    (1000) patrik    (1000)      124 2024-05-16 19:52:23.000000 mtress-3.0.0a2/mtress.egg-info/requires.txt
+-rw-r--r--   0 patrik    (1000) patrik    (1000)       13 2024-05-16 19:52:23.000000 mtress-3.0.0a2/mtress.egg-info/top_level.txt
+-rw-r--r--   0 patrik    (1000) patrik    (1000)       38 2024-05-16 19:52:23.826678 mtress-3.0.0a2/setup.cfg
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1188 2024-05-16 19:45:33.000000 mtress-3.0.0a2/setup.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/tests/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/__init__.py
+drwxr-xr-x   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:52:23.826678 mtress-3.0.0a2/tests/unit_tests/
+-rw-r--r--   0 patrik    (1000) patrik    (1000)        0 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/unit_tests/__init__.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     3502 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/unit_tests/test_data_handler.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1743 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/unit_tests/test_location.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     1956 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/unit_tests/test_meta_model.py
+-rw-r--r--   0 patrik    (1000) patrik    (1000)     2958 2024-05-16 19:37:48.000000 mtress-3.0.0a2/tests/unit_tests/test_solph_model.py
```

### Comparing `mtress-3.0.0.dev0/LICENSE` & `mtress-3.0.0a2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Deutsches Zentrum für Luft- und Raumfahrt e.V. (DLR), KEHAG Energiehandel GmbH
+Copyright (c) Deutsches Zentrum für Luft- und Raumfahrt e.V. (DLR)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mtress-3.0.0.dev0/mtress/_helpers/_array_cast.py` & `mtress-3.0.0a2/mtress/_helpers/_array_cast.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 SPDX-License-Identifier: MIT
 """
 import numbers
 import numpy as np
 import pandas as pd
 
 
-def numeric_array(data, length):
+def numeric_array(data, length=None):
+    if length is None:
+        length = len(data)
     if isinstance(data, numbers.Number):
         data = np.full(length, fill_value=data)
     elif isinstance(data, list) and len(data) == length:
         data = np.array(data)
     elif isinstance(data, pd.Series) and len(data) == length:
         data = data.to_numpy()
     elif isinstance(data, np.ndarray):
```

### Comparing `mtress-3.0.0.dev0/mtress/_run_mtress.py` & `mtress-3.0.0a2/mtress/_run_mtress.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
 def run_mtress(parameters, solver="cbc"):
     """
     :param parameters: dict holding configuration
     :param solver: solver to use for oemof.solph
     """
     meta_model = MetaModel(**parameters)
     meta_model.solve(
-        solver=solver, solve_kwargs={"tee": False}, cmdline_options={"ratio": 0.01}
+        solver=solver,
+        solve_kwargs={"tee": False},
+        cmdline_options={"ratio": 0.01},
     )
 
     return meta_model
 
 
 if __name__ == "__main__":
     script_path = os.path.realpath(__file__)
```

### Comparing `mtress-3.0.0.dev0/mtress/physics/__init__.py` & `mtress-3.0.0a2/mtress/physics/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,49 +5,78 @@
 SPDX-FileCopyrightText: kehag Energiehandel GMbH
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Lucas Schmeling
 
 SPDX-License-Identifier: MIT
 """
 
+from ._constants import (
+
+    H2O_DENSITY,
+    H2O_HEAT_CAPACITY,
+    H2O_HEAT_FUSION,
+    HHV_WP,
+    HS_PER_HI_GAS,
+    IDEAL_GAS_CONSTANT,
+    HS_PER_HI_WP,
+    SECONDS_PER_HOUR,
+    TC_CONCRETE,
+    TC_INSULATION,
+    ZERO_CELSIUS,
+)
 from ._helper_functions import (
-    kilo_to_mega,
+    bar_to_pascal,
+    calc_cop,
+    calc_isothermal_compression_energy,
     celsius_to_kelvin,
     kelvin_to_celsius,
+    kilo_to_mega,
     kJ_to_MWh,
-    mean_logarithmic_temperature,
     lorenz_cop,
-    calc_cop,
+    mean_logarithmic_temperature,
+    mega_to_one,
+    one_to_mega
 )
 
-from ._constants import (
-    ZERO_CELSIUS,
-    HS_PER_HI_GAS,
-    HS_PER_HI_WP,
-    HHV_WP,
-    H2O_HEAT_CAPACITY,
-    H2O_HEAT_FUSION,
-    H2O_DENSITY,
-    TC_CONCRETE,
-    TC_INSULATION,
-    SECONDS_PER_HOUR,
+from ._gas_definition import (
+    Gas,
+    HYDROGEN,
+    NATURAL_GAS,
+    BIO_METHANE,
+    BIOGAS,
+    calc_hydrogen_density,
+    calc_biogas_heating_value,
+    calc_biogas_molar_mass,
+    calc_natural_gas_molar_mass,
 )
 
 __all__ = [
     "kilo_to_mega",
     "celsius_to_kelvin",
     "kelvin_to_celsius",
     "kJ_to_MWh",
+    "bar_to_pascal",
     "mean_logarithmic_temperature",
     "lorenz_cop",
     "calc_cop",
     "ZERO_CELSIUS",
     "HS_PER_HI_GAS",
     "HS_PER_HI_WP",
     "HHV_WP",
     "H2O_HEAT_CAPACITY",
     "H2O_HEAT_FUSION",
     "H2O_DENSITY",
+    "IDEAL_GAS_CONSTANT",
     "TC_CONCRETE",
     "TC_INSULATION",
     "SECONDS_PER_HOUR",
+    "calc_isothermal_compression_energy",
+    "calc_hydrogen_density",
+    "calc_biogas_heating_value",
+    "Gas",
+    "HYDROGEN",
+    "NATURAL_GAS",
+    "BIO_METHANE",
+    "BIOGAS",
+    "mega_to_one",
+    "one_to_mega"
 ]
```

### Comparing `mtress-3.0.0.dev0/mtress/physics/_constants.py` & `mtress-3.0.0a2/mtress/physics/_constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 
 # 0°C in K
 ZERO_CELSIUS = 273.15  # K
 
 # Natural gas
 HS_PER_HI_GAS = 1.11  # according to DIN V 18599
 
+IDEAL_GAS_CONSTANT = 8.314  # J/(mol·K)
+
 # Wood pellets
 HS_PER_HI_WP = 1.08  # according to DIN V 18599
 # higher heating value(?)
-HHV_WP = 4.8  # kWh/kg  /  MWh/t
+HHV_WP = 4800  # Wh/kg  /  kWh/t
 
 # Water in heat storage
-H2O_HEAT_CAPACITY = 4.182  # kJ/(kg*K)
+H2O_HEAT_CAPACITY = 4182  # J/(kg*K)
 H2O_HEAT_FUSION = 0.09265  # MWh/t, = 333.55 J/g
-H2O_DENSITY = 1000  # Kg/m^3
+H2O_DENSITY = 1000  # kg/m³
 
 # Thermal conductivity
 TC_CONCRETE = 0.8  # W / (m * K)
 TC_INSULATION = 0.04  # W / (m * K)
 
 # improve readability, used e.g. for J -> Wh
 SECONDS_PER_HOUR = 3600
```

### Comparing `mtress-3.0.0.dev0/mtress/technologies/layered_heat/_layered_heat_pump.py` & `mtress-3.0.0a2/mtress/technologies/_heat_pump.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-# -*- coding: utf-8 -*-
-
 """
-heat pump to be used with HeatLayer
+Heat pump to be used with the layered heat energy carrier.
 
 SPDX-FileCopyrightText: Deutsches Zentrum für Luft und Raumfahrt
 SPDX-FileCopyrightText: kehag Energiehandel GMbH
 SPDX-FileCopyrightText: Patrik Schönfeldt
 SPDX-FileCopyrightText: Lucas Schmeling
 
 SPDX-License-Identifier: MIT
 """
+from typing import Optional
 
-from oemof import solph
+from oemof.solph import Bus, Flow
+from oemof.solph.components import Source, Converter
 
-from mtress.physics import calc_cop, celsius_to_kelvin
+from .._abstract_component import AbstractSolphRepresentation
+from ..carriers import Electricity, Heat
+from ..physics import calc_cop, celsius_to_kelvin
+from ._abstract_technology import AbstractAnergySource, AbstractTechnology
 
 
-class LayeredHeatPump:
+class HeatPump(AbstractTechnology, AbstractSolphRepresentation):
     """
-    Clustered heat pump for modeling power flows
-    with variable temperature levels.
-    Connects any input to any output using solph.Transformer
+    Clustered heat pump for modeling power flows with variable temperature levels.
+
+    Connects any input to any output using Converter
     with shared resources, see https://arxiv.org/abs/2012.12664
 
     Flows:
     E --> HP1,         E --> HP2,       E --> HP3
     A --> HP1,         A --> HP2,       A --> HP3
     1HP --> HP1,     1HP --> HP2,     1HP --> HP3
     HP0 --> Qin(T1), HP1 --> Qin(T2), HP2 --> Qin(T3)
@@ -39,106 +42,96 @@
          │     ┃  │┌─────↗    ┃            ↓
          └─────╂──┼┼───→[HP1]─╂────────→(Qin(T1))
                ┃ [1HP]────↗   ┃
                ┗━━━━━━━━━━━━━━┛
 
     The heat pump is modelled as an array of virtual heat pumps,
     each with the correct COP for the corresponding temperatures.
-    To not allow producing more heat then the real heat pump,
+    To not allow producing more heat than the real heat pump,
     all these virtual heat pumps share anergy and energy sources
     and can further have one shared virtual normalisation source (1HP).
+
+    The heat pump also connects to every available anergy source at
+    the location. The COPs are automatically calculated based on the
+    information given by the heat carrier and the anergy sources.
     """
 
     def __init__(
         self,
-        heat_layers,
-        electricity_source,
-        heat_sources,
-        thermal_power_limit=None,
-        cop_0_35=4.6,
-        label="",
+        name: str,
+        thermal_power_limit: float = None,
+        cop_0_35: float = 4.6,
+        anergy_sources: Optional[list] = None,
     ):
         """
-        :param heat_layers: HeatLayers object to attach to
-        :param electricity_source:
-        :param heat_sources:
-        :param cop_0_35:
-        :param label:
+        Initialize heat pump component.
+
+        :param thermal_power_limit: Thermal power limit on all temperature ranges
+        :param cop_0_35: COP for the temperature rise 0°C to 35°C
+        :param anergy_sources: Anergy sources (names) to connect to, defaults to all
         """
-        self.b_th_in = dict()
-        self.cop = dict()
-        self.heat_out_flows = list()
-
-        energy_system = heat_layers.energy_system
-
-        if len(label) > 0:
-            label = label + "_"
-
-        electricity_bus = solph.Bus(
-            label=label + "heat_pump_electricity",
-            inputs={electricity_source: solph.Flow()},
+        super().__init__(name=name)
+
+        self.thermal_power_limit = thermal_power_limit
+        self.cop_0_35 = cop_0_35
+        self.anergy_sources = anergy_sources
+
+        # Solph specific parameters
+        self.electricity_bus = None
+        self.heat_budget_bus = None
+
+    def build_core(self):
+        """Build core structure of oemof.solph representation."""
+        # Add electrical connection
+        electricity_carrier = self.location.get_carrier(Electricity)
+
+        self.electricity_bus = self.create_solph_node(
+            label="electricity",
+            node_type=Bus,
+            inputs={electricity_carrier.distribution: Flow()},
         )
 
-        heat_budget_split = solph.Bus(label=label + "heat_budget_split")
-        if thermal_power_limit:
-            heat_budget = solph.Source(
-                label=label + "heat_budget",
-                outputs={
-                    heat_budget_split: solph.Flow(nominal_value=thermal_power_limit)
-                },
-            )
-        else:
-            heat_budget = solph.Source(
-                label=label + "heat_budget", outputs={heat_budget_split: solph.Flow()}
-            )
-
-        self.heat_budget_flow = (heat_budget.label, heat_budget_split.label)
-
-        energy_system.add(electricity_bus, heat_budget_split, heat_budget)
-
-        for source in heat_sources:
-            temperature_lower = heat_sources[source]
-            heat_source = solph.Bus(label=label + "in_" + source)
-            self.b_th_in[source] = heat_source
-            energy_system.add(heat_source)
-
-            for target_temperature in heat_layers.temperature_levels:
-                temperature_higher_str = "{0:.0f}".format(target_temperature)
-                hp_str = label + source + "_" + temperature_higher_str
-
-                cop = calc_cop(
-                    temp_input=celsius_to_kelvin(temperature_lower),
-                    temp_output=celsius_to_kelvin(target_temperature),
-                    cop_0_35=cop_0_35,
-                )
-
-                self.cop[(source, target_temperature)] = cop
-
-                heat_pump_level = solph.Transformer(
-                    label=hp_str,
-                    inputs={
-                        heat_source: solph.Flow(),
-                        electricity_bus: solph.Flow(),
-                        heat_budget_split: solph.Flow(),
-                    },
-                    outputs={heat_layers.b_th_in[target_temperature]: solph.Flow()},
-                    conversion_factors={
-                        heat_source: (cop - 1) / cop,
-                        electricity_bus: 1 / cop,
-                        heat_layers.b_th_in[target_temperature]: 1,
-                    },
-                )
-
-                self.heat_out_flows.append(
-                    (
-                        heat_pump_level.label,
-                        heat_layers.b_th_in[target_temperature].label,
-                    )
-                )
+        # Create bus and source for a combined thermal power limit on all temperature
+        # levels
+        self.heat_budget_bus = heat_budget_bus = self.create_solph_node(
+            label="heat_budget_bus",
+            node_type=Bus,
+        )
 
-                energy_system.add(heat_pump_level)
+        self.create_solph_node(
+            label="heat_budget_source",
+            node_type=Source,
+            outputs={heat_budget_bus: Flow(nominal_value=self.thermal_power_limit)},
+        )
 
-    def heat_output(self, results_dict):
-        """
-        Total energy
-        """
-        return results_dict[self.heat_budget_flow]["sequences"]["flow"]
+    def establish_interconnections(self):
+        """Add connections to anergy sources."""
+        heat_carrier = self.location.get_carrier(Heat)
+
+        for anergy_source in self.location.get_technology(AbstractAnergySource):
+            if self.anergy_sources is None or anergy_source.name in self.anergy_sources:
+                # Add tranformers for each heat source.
+                for target_temperature in heat_carrier.input_levels:
+                    cop = calc_cop(
+                        temp_input=celsius_to_kelvin(anergy_source.temperature),
+                        temp_output=celsius_to_kelvin(target_temperature),
+                        cop_0_35=self.cop_0_35,
+                    )
+
+                    self.create_solph_node(
+                        label=f"{anergy_source.name}_{target_temperature:.0f}",
+                        node_type=Converter,
+                        inputs={
+                            anergy_source.bus: Flow(),
+                            self.electricity_bus: Flow(),
+                            self.heat_budget_bus: Flow(),
+                        },
+                        outputs={
+                            heat_carrier.inputs[target_temperature]: Flow(),
+                        },
+                        conversion_factors={
+                            self.heat_budget_bus: 1,
+                            anergy_source.bus: (cop - 1) / cop,
+                            self.electricity_bus: 1 / cop,
+                            heat_carrier.inputs[target_temperature]: 1,
+                        },
+                    )
```

### Comparing `mtress-3.0.0.dev0/setup.py` & `mtress-3.0.0a2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name="mtress",
-    version="3.0.0dev0",
+    version="3.0.0a2",
     url="https://github.com/mtress/mtress",
     author="Deutsches Zentrum für Luft- und Raumfahrt e.V. (DLR)",
     author_email="patrik.schoenfeldt@dlr.de",
     packages=find_packages(),
     classifiers=[
         # complete classifier list:
         # http://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -23,18 +23,13 @@
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.10",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     zip_safe=False,
-    install_requires=[
-        "oemof.solph >= 0.4.4",
-        "oemof.thermal >= 0.0.5",
-        "pyyaml >= 6.0",
-        "pvlib"
-    ],
+    install_requires=read("requirements.txt"),
 )
```

