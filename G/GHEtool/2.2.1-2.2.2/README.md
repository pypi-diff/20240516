# Comparing `tmp/GHEtool-2.2.1.tar.gz` & `tmp/ghetool-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GHEtool-2.2.1.tar", last modified: Sat Jan 27 12:45:41 2024, max compression
+gzip compressed data, was "ghetool-2.2.2.tar", last modified: Thu May 16 16:21:44 2024, max compression
```

## Comparing `GHEtool-2.2.1.tar` & `ghetool-2.2.2.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.508776 GHEtool-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.496776 GHEtool-2.2.1/GHEtool/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.500776 GHEtool-2.2.1/GHEtool/Validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/sizing_method_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/sizing_method_comparison_L2_L3_L4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/speed_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/validate_deep_sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/Validation/validation_effective_borehole_thermal_resistance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.500776 GHEtool-2.2.1/GHEtool/VariableClasses/
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/BaseClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/Borehole.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/CalculationSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/CustomGFunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/FluidData.py
--rw-r--r--   0 runner    (1001) docker     (127)    23596 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GFunction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.500776 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundConstantTemperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundFluxTemperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundTemperatureGradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/Temperature_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/_GroundData.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.500776 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.500776 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoadMultiYear.py
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadAbsolute.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadRelative.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19889 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/_LoadData.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.504776 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/CoaxialPipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/DoubleUTube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/MultipleUTube.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/SingleUTube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/_PipeData.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/VariableClasses/cylindrical_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.504776 GHEtool-2.2.1/GHEtool/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/logger/ghe_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    84207 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/main_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.496776 GHEtool-2.2.1/GHEtool/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.504776 GHEtool-2.2.1/GHEtool/test/general_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/general_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/general_tests/test_GHEtool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/general_tests/test_GHEtool_two.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.504776 GHEtool-2.2.1/GHEtool/test/methods/
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/methods/TestMethodClass.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23320 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/methods/method_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/methods/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.508776 GHEtool-2.2.1/GHEtool/test/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_baseclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_borehole.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_calculation_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_custom_gfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_fluiddata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18414 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_gfunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_grounddata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_hourly_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44728 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_main_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_monthly_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-01-27 12:45:34.000000 GHEtool-2.2.1/GHEtool/test/unit-tests/test_pipedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 12:45:41.508776 GHEtool-2.2.1/GHEtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-01-27 12:45:41.000000 GHEtool-2.2.1/GHEtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-27 12:45:41.000000 GHEtool-2.2.1/GHEtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 12:45:41.000000 GHEtool-2.2.1/GHEtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-27 12:45:41.000000 GHEtool-2.2.1/GHEtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-27 12:45:41.000000 GHEtool-2.2.1/GHEtool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-27 12:45:34.000000 GHEtool-2.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18360 2024-01-27 12:45:41.508776 GHEtool-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17792 2024-01-27 12:45:34.000000 GHEtool-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-27 12:45:34.000000 GHEtool-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-27 12:45:41.508776 GHEtool-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.356080 ghetool-2.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.344080 ghetool-2.2.2/GHEtool/
+-rw-r--r--   0 runner    (1001) docker     (127)    90861 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Borefield.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.344080 ghetool-2.2.2/GHEtool/Validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/sizing_method_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/sizing_method_comparison_L2_L3_L4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/speed_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/validate_deep_sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/Validation/validation_effective_borehole_thermal_resistance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.348080 ghetool-2.2.2/GHEtool/VariableClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/BaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/Borehole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/CalculationSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11017 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/CustomGFunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/FluidData.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24529 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GFunction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.348080 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundConstantTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundFluxTemperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundTemperatureGradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/_GroundData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/GroundData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.348080 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.348080 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoadMultiYear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadAbsolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadMultiYear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadRelative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19991 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/_LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/LoadData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.352080 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/CoaxialPipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/DoubleUTube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/MultipleUTube.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/SingleUTube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/_PipeData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/PipeData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/VariableClasses/cylindrical_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.352080 ghetool-2.2.2/GHEtool/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/logger/ghe_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.344080 ghetool-2.2.2/GHEtool/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.352080 ghetool-2.2.2/GHEtool/test/general_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/general_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/general_tests/test_GHEtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/general_tests/test_GHEtool_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/general_tests/test_multiple_years.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.352080 ghetool-2.2.2/GHEtool/test/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/methods/TestMethodClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28230 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/methods/method_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/methods/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.356080 ghetool-2.2.2/GHEtool/test/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_borehole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_calculation_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_custom_gfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_fluiddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18840 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_gfunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_grounddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17875 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_hourly_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48619 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_main_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_monthly_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_monthly_load_multi_year.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-16 16:21:40.000000 ghetool-2.2.2/GHEtool/test/unit-tests/test_pipedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:44.356080 ghetool-2.2.2/GHEtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-16 16:21:44.000000 ghetool-2.2.2/GHEtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-16 16:21:44.000000 ghetool-2.2.2/GHEtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:21:44.000000 ghetool-2.2.2/GHEtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 16:21:44.000000 ghetool-2.2.2/GHEtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 16:21:44.000000 ghetool-2.2.2/GHEtool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-16 16:21:40.000000 ghetool-2.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-16 16:21:44.356080 ghetool-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18550 2024-05-16 16:21:40.000000 ghetool-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 16:21:40.000000 ghetool-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 16:21:44.356080 ghetool-2.2.2/setup.cfg
```

### Comparing `GHEtool-2.2.1/GHEtool/Validation/cases.py` & `ghetool-2.2.2/GHEtool/Validation/cases.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/Validation/sizing_method_comparison.py` & `ghetool-2.2.2/GHEtool/Validation/sizing_method_comparison.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/Validation/sizing_method_comparison_L2_L3_L4.py` & `ghetool-2.2.2/GHEtool/Validation/sizing_method_comparison_L2_L3_L4.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     borefield.Rb = 0.12
 
     # set the borefield
     borefield.create_rectangular_borefield(10, 10, 6, 6, 110, 1, 0.075)
 
     # load the hourly profile
     load = HourlyGeothermalLoad()
-    print(FOLDER)
     load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"), header=True, separator=";")
     borefield.load = load
     borefield.simulation_period = 100
 
     ### size the borefield
     # according to L2
     L2_start = time.time()
```

### Comparing `GHEtool-2.2.1/GHEtool/Validation/speed_comparison.py` & `ghetool-2.2.2/GHEtool/Validation/speed_comparison.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/Validation/validate_deep_sizing.py` & `ghetool-2.2.2/GHEtool/Validation/validate_deep_sizing.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/Validation/validation_effective_borehole_thermal_resistance.py` & `ghetool-2.2.2/GHEtool/Validation/validation_effective_borehole_thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/BaseClass.py` & `ghetool-2.2.2/GHEtool/VariableClasses/BaseClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 This document contains the information for the BaseClass.
 This class is used as a super class for different variable classes.
 """
 from __future__ import annotations
+
+import warnings
 from typing import List
 
 import numpy as np
 from numpy import ndarray
 from pygfunction.boreholes import Borehole
 from importlib import import_module
 
@@ -166,15 +168,20 @@
         """
         # get all variables in class
         if hasattr(self, "__slots__"):
             variables: List[str] = list(self.__slots__)
         else:
             variables: List[str] = [attr for attr in dir(self) if not callable(getattr(self, attr)) and not attr.startswith("__")]
 
-        return all(getattr(self, var) is not None for var in variables)
+        temp = [getattr(self, var) is not None for var in variables]
+        if all(temp):
+            return True
+        else:
+            # print(f'There is a problem with the {[var for idx, var in enumerate(variables) if not temp[idx]]} variables.')
+            return False
 
 
 class UnsolvableDueToTemperatureGradient(Exception):
     """
     This Exception occurs when there is an unsizeble borefield due to incompatibility between 1) peak cooling,
     which requires a deeper borefield and 2) a temperature gradient, which causes a higher ground temperature when
     the field is drilled deeper. This leads to unsizeble solutions.
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/Borehole.py` & `ghetool-2.2.2/GHEtool/VariableClasses/Borehole.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This document contains all the information of the borehole class.
 """
 
 from GHEtool.VariableClasses.BaseClass import BaseClass
 from GHEtool.VariableClasses.FluidData import FluidData
 from GHEtool.VariableClasses.PipeData import _PipeData, MultipleUTube
-from math import pi
+from typing import Union
 
 import matplotlib.pyplot as plt
 import pygfunction as gt
 
 
 class Borehole(BaseClass):
 
@@ -165,28 +165,28 @@
         Returns
         -------
         None
         """
         self._pipe_data = MultipleUTube()
         self.use_constant_Rb = True
 
-    def calculate_Rb(self, H: float, D: float, r_b: float, k_s: float) -> float:
+    def calculate_Rb(self, H: float, D: float, r_b: float, k_s: Union[float, callable]) -> float:
         """
         This function calculates the equivalent borehole thermal resistance.
 
         Parameters
         ----------
         H : float
             Borehole depth [m]
         D : float
             Borehole burial depth [m]
         r_b : float
             Borehole radius [m]
-        k_s : float
-            Ground thermal conductivity [mk/W]
+        k_s : float or callable
+            (Function to calculate the) ground thermal conductivity [mk/W]
 
         Returns
         -------
         Rb : float
             Equivalent borehole thermal resistance
 
         Raises
@@ -198,43 +198,43 @@
         if not self.pipe_data.check_values() or not self.fluid_data.check_values():
             print("Please make sure you set al the pipe and fluid data.")
             raise ValueError
 
         # initiate temporary borefield
         borehole = gt.boreholes.Borehole(H, D, r_b, 0, 0)
         # initiate pipe
-        pipe = self.pipe_data.pipe_model(self.fluid_data, k_s, borehole)
+        pipe = self.pipe_data.pipe_model(self.fluid_data, k_s if isinstance(k_s, (float, int)) else k_s(H), borehole)
 
         return pipe.effective_borehole_thermal_resistance(self.fluid_data.mfr, self.fluid_data.Cp)
 
-    def get_Rb(self, H: float, D: float, r_b: float, k_s: float) -> float:
+    def get_Rb(self, H: float, D: float, r_b: float, k_s: Union[callable, float]) -> float:
         """
         This function returns the equivalent borehole thermal resistance.
         If use_constant_Rb is True, self._Rb is returned, otherwise the resistance is calculated.
 
         Parameters
         ----------
         H : float
             Borehole depth [m]
         D : float
             Borehole burial depth [m]
         r_b : float
             Borehole radius [m]
-        k_s : float
-            Ground thermal conductivity [mk/W]
+        k_s : float or callable
+            (Function to calculate) ground thermal conductivity in function of depth [mk/W]
 
         Returns
         -------
         Rb* : float
             Equivalent borehole thermal resistance [mK/W]
         """
         if self.use_constant_Rb:
             return self.Rb
 
-        return self.calculate_Rb(H, D, r_b, k_s)
+        return self.calculate_Rb(H, D, r_b, k_s if isinstance(k_s, (int, float)) else k_s(H))
 
     def __eq__(self, other):
         if not isinstance(other, Borehole):
             return False
         for i in self.__slots__:
             if getattr(self, i) != getattr(other, i):
                 return False
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/CalculationSetup.py` & `ghetool-2.2.2/GHEtool/VariableClasses/CalculationSetup.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/CustomGFunction.py` & `ghetool-2.2.2/GHEtool/VariableClasses/CustomGFunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file contains both the CustomGFunction class and all the relevant information w.r.t. custom gfunctions.
 """
+import copy
 import pickle
 import warnings
 from typing import List, Union
 
 import numpy as np
 import pygfunction as gt
 from scipy import interpolate
@@ -186,43 +187,43 @@
                 "The requested time of " + str(min_time_value) + "s is outside the bounds of " + str(self.min_t) +
                 " and " + str(self.max_t) + " of the precalculated data. The gfunctions will be calculated jit.",
                 UserWarning)
             return False
 
         return True
 
-    def create_custom_dataset(self, borefield: List[gt.boreholes.Borehole], alpha: float) -> None:
+    def create_custom_dataset(self, borefield: List[gt.boreholes.Borehole], alpha: Union[float, callable]) -> None:
         """
         This function creates the custom dataset.
 
         Parameters
         ----------
         borefield : list[pygfunction.boreholes.Borehole]
             Borefield object for which the custom dataset should be created
-        alpha : float
-            Ground thermal diffusivity [m2/s]
+        alpha : float or callable
+            Ground thermal diffusivity [m2/s] or function to calculate it at a certain depth
 
         Returns
         -------
         None
         """
         # chek if there is a method in options
         if not "method" in self.options:
             self.options["method"] = "equivalent"
 
         for idx, H in enumerate(self.depth_array):
             ghe_logger.info(f'Start H: {H}')
 
             # Calculate the g-function for uniform borehole wall temperature
-
+            borefield = copy.deepcopy(borefield)
             # set borehole depth in borefield
             for borehole in borefield:
                 borehole.H = H
 
-            gfunc_uniform_T = gt.gfunction.gFunction(borefield, alpha,
+            gfunc_uniform_T = gt.gfunction.gFunction(borefield, alpha if isinstance(alpha, float) else alpha(H),
                                                      self.time_array, options=self.options,
                                                      method=self.options["method"])
 
             self.gvalues_array[idx] = gfunc_uniform_T.gFunc
 
     def dump_custom_dataset(self, path: str, name: str) -> None:
         """
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/FluidData.py` & `ghetool-2.2.2/GHEtool/VariableClasses/FluidData.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/GFunction.py` & `ghetool-2.2.2/GHEtool/VariableClasses/GFunction.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,29 +86,60 @@
     """
 
     DEFAULT_TIMESTEPS: np.ndarray = _time_values()
     DEFAULT_NUMBER_OF_TIMESTEPS: int = DEFAULT_TIMESTEPS.size
     DEFAULT_STORE_PREVIOUS_VALUES: bool = True
 
     def __init__(self):
-        self.store_previous_values: bool = GFunction.DEFAULT_STORE_PREVIOUS_VALUES
+        self._store_previous_values: bool = GFunction.DEFAULT_STORE_PREVIOUS_VALUES
+        self._store_previous_values_backup: bool= GFunction.DEFAULT_STORE_PREVIOUS_VALUES
         self.options: dict = {'method': 'equivalent'}
         self.alpha: float = 0.
         self.borefield: list[gt.boreholes.Borehole] = []
         self.depth_array: np.ndarray = np.array([])
         self.time_array: np.ndarray = np.array([])
         self.previous_gfunctions: np.ndarray = np.array([])
         self.previous_depth: float = 0.
         self.use_cyl_correction_when_negative: bool = True
 
         self.no_extrapolation: bool = True
         self.threshold_depth_interpolation: float = .25  # %
 
         self.fifo_list: FIFO = FIFO(8)
 
+
+    @property
+    def store_previous_values(self) -> bool:
+        """
+        This returns the truth value of the store_previous_values attribute.
+
+        Returns
+        -------
+        bool
+            True if the previously calculated gfunction values should be saved.
+        """
+        return self._store_previous_values
+
+    @store_previous_values.setter
+    def store_previous_values(self, store: bool) -> None:
+        """
+        This function sets the store previous values attribute and also its backup.
+
+        Parameters
+        ----------
+        store : bool
+            True if the previous calculated g-function values should be stored.
+
+        Returns
+        -------
+        None
+        """
+        self._store_previous_values = store
+        self._store_previous_values_backup = store
+
     def calculate(self, time_value: Union[list, float, np.ndarray], borefield: List[gt.boreholes.Borehole],
                   alpha: float, interpolate: bool = None):
         """
         This function returns the gvalues either by interpolation or by calculating them.
         It does so by calling the function gvalues which does this calculation.
         This calculation function also stores the previous calculated data and makes interpolations
         whenever the requested list of time_value are longer then DEFAULT_NUMBER_OF_TIMESTEPS.
@@ -198,15 +229,14 @@
 
                     backup = self.options.get('Cylindrical_correction')
 
                     self.options["cylindrical_correction"] = True
                     gfunc_calculated = gt.gfunction.gFunction(borefield, alpha, time_values, options=self.options, method=self.options['method']).gFunc
                     self.options["cylindrical_correction"] = backup
 
-
             # store the calculated g-values
             self.set_new_calculated_data(time_values, depth, gfunc_calculated, borefield, alpha)
 
             return gfunc_calculated
 
         # get depth from borefield
         depth = borefield[0].H
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundConstantTemperature.py` & `ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundConstantTemperature.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundFluxTemperature.py` & `ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundFluxTemperature.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,24 +39,26 @@
         Returns
         -------
         Tg : float
             Ground temperature [deg C]
         """
         # geothermal gradient is equal to the geothermal heat flux divided by the thermal conductivity
         # avg ground temperature is (Tg + gradient + Tg) / 2 = Tg + gradient / 2
-        return self.Tg + H * self.flux / self.k_s / 2
+        return self.Tg + H * self.flux / self.k_s(H) / 2
 
-    def calculate_delta_H(self, temperature_diff: float) -> float:
+    def calculate_delta_H(self, temperature_diff: float, H: float = 100) -> float:
         """
         This function calculates the difference in depth for a given difference in temperature.
 
         Parameters
         ----------
         temperature_diff : float
             Difference in temperature [deg C]
+        H : float
+            Depth at which the average ground thermal conductivity should be taken [m]
 
         Returns
         -------
         float
             Difference in depth [m]
         """
-        return temperature_diff * 2 * self.k_s / self.flux
+        return temperature_diff * 2 * self.k_s(H) / self.flux
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/GroundData/GroundTemperatureGradient.py` & `ghetool-2.2.2/GHEtool/VariableClasses/GroundData/GroundTemperatureGradient.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoad.py` & `ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
 
 import warnings
 
-from typing import Union, Tuple, TYPE_CHECKING
+from typing import Tuple, TYPE_CHECKING
 
 from GHEtool.VariableClasses.LoadData._LoadData import _LoadData
 from GHEtool.logger import ghe_logger
 
 if TYPE_CHECKING:
-    from numpy.typing import ArrayLike, NDArray
+    from numpy.typing import ArrayLike
 
 
 class HourlyGeothermalLoad(_LoadData):
     """
     This class contains all the information for geothermal load data with a monthly resolution and absolute input.
     This means that the inputs are both in kWh/month and kW/month.
     """
 
-    __slots__ = tuple(_LoadData.__slots__) + ('_heating_load', '_cooling_load')
+    __slots__ = tuple(_LoadData.__slots__) + ("_heating_load", "_cooling_load")
 
-    # define parameters for conversion to monthly loads
-    START = pd.to_datetime("2019-01-01 00:00:00")
-    END = pd.to_datetime("2019-12-31 23:59:00")
-    HOURS_SERIES = pd.Series(pd.date_range(START, END, freq="1H"))
-
-    def __init__(self, heating_load: ArrayLike | None = None,
-                 cooling_load: ArrayLike | None = None,
+    def __init__(self, heating_load: ArrayLike = None,
+                 cooling_load: ArrayLike = None,
                  simulation_period: int = 20,
                  dhw: float = 0.):
         """
 
         Parameters
         ----------
         heating_load : np.ndarray, list, tuple
@@ -44,46 +39,46 @@
         dhw : float
             Yearly consumption of domestic hot water [kWh/year]
         """
 
         super().__init__(hourly_resolution=True, simulation_period=simulation_period)
 
         # initiate variables
-        self._hourly_heating_load: NDArray[np.float64] = np.zeros(8760)
-        self._hourly_cooling_load: NDArray[np.float64] = np.zeros(8760)
+        self._hourly_heating_load: np.ndarray = np.zeros(8760)
+        self._hourly_cooling_load: np.ndarray = np.zeros(8760)
 
         # set variables
-        self.hourly_heating_load: NDArray[np.float64] = np.zeros(8760) if heating_load is None else np.array(heating_load)
-        self.hourly_cooling_load: NDArray[np.float64] = np.zeros(8760) if cooling_load is None else np.array(cooling_load)
+        self.hourly_heating_load: np.ndarray = np.zeros(8760) if heating_load is None else np.array(heating_load)
+        self.hourly_cooling_load: np.ndarray = np.zeros(8760) if cooling_load is None else np.array(cooling_load)
         self.dhw = dhw
 
-    def _check_input(self, input: Union[np.ndarray, list, tuple]) -> bool:
+    def _check_input(self, load_array: ArrayLike) -> bool:
         """
         This function checks whether the input is valid or not.
         The input is correct if and only if:
         1) the input is a np.ndarray, list or tuple
         2) the length of the input is 8760
         3) the input does not contain any negative values.
 
         Parameters
         ----------
-        input : np.ndarray, list or tuple
+        load_array : np.ndarray, list or tuple
 
         Returns
         -------
         bool
             True if the inputs are valid
         """
-        if not isinstance(input, (np.ndarray, list, tuple)):
+        if not isinstance(load_array, (np.ndarray, list, tuple)):
             ghe_logger.error("The load should be of type np.ndarray, list or tuple.")
             return False
-        if not len(input) == 8760:
-            ghe_logger.error("The length of the load should be 12.")
+        if not len(load_array) == 8760:
+            ghe_logger.error("The length of the load should be 8760.")
             return False
-        if np.min(input) < 0:
+        if np.min(load_array) < 0:
             ghe_logger.error("No value in the load can be smaller than zero.")
             return False
         return True
 
     @property
     def hourly_heating_load(self) -> np.ndarray:
         """
@@ -93,15 +88,15 @@
         -------
         hourly heating : np.ndarray
             Hourly heating values (incl. DHW) [kWh/h] for one year, so the length of the array is 8760
         """
         return self.correct_for_start_month(self._hourly_heating_load + self.dhw / 8760)
 
     @hourly_heating_load.setter
-    def hourly_heating_load(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def hourly_heating_load(self, load: ArrayLike) -> None:
         """
         This function sets the hourly heating load [kWh/h] after it has been checked.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
             Hourly heating [kWh/h]
@@ -117,15 +112,15 @@
             values
         """
         if self._check_input(load):
             self._hourly_heating_load = load
             return
         raise ValueError
 
-    def set_hourly_heating(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_hourly_heating(self, load: ArrayLike) -> None:
         """
         This function sets the hourly heating load [kWh/h] after it has been checked.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
             Hourly heating [kWh/h]
@@ -151,15 +146,15 @@
         -------
         hourly cooling : np.ndarray
             Hourly cooling values [kWh/h] for one year, so the length of the array is 8760
         """
         return self.correct_for_start_month(self._hourly_cooling_load)
 
     @hourly_cooling_load.setter
-    def hourly_cooling_load(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def hourly_cooling_load(self, load: ArrayLike) -> None:
         """
         This function sets the hourly cooling load [kWh/h] after it has been checked.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
             Hourly cooling [kWh/h]
@@ -175,15 +170,15 @@
             values
         """
         if self._check_input(load):
             self._hourly_cooling_load = load
             return
         raise ValueError
 
-    def set_hourly_cooling(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_hourly_cooling(self, load: ArrayLike) -> None:
         """
         This function sets the hourly cooling load [kWh/h] after it has been checked.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
             Hourly cooling [kWh/h]
@@ -221,24 +216,20 @@
         hourly_load : np.ndarray
             Hourly loads in kWh/h
 
         Returns
         -------
         peak loads [kW], monthly average loads [kWh/month] : np.ndarray, np.ndarray
         """
-        # create dataframe
-        df = pd.DataFrame(hourly_load, index=HourlyGeothermalLoad.HOURS_SERIES, columns=['load'])
+        data = np.array_split(hourly_load, np.cumsum(self.UPM)[:-1])
 
         if self.all_months_equal:
-            return np.max(np.array_split(hourly_load, 12), axis=1), np.sum(np.array_split(hourly_load, 12), axis=1)
-
-        # resample
-        return np.array(df.resample('M').agg({'load': 'max'})['load']),\
-            np.array(df.resample('M').agg({'load': 'sum'})['load'])
+            return np.max(data, axis=1), np.sum(data, axis=1)
 
+        return np.array([np.max(i) for i in data]), np.array([np.sum(i) for i in data])
 
     @property
     def baseload_cooling(self) -> np.ndarray:
         """
         This function returns the baseload cooling in kWh/month.
 
         Returns
@@ -315,16 +306,17 @@
         Returns
         -------
         hourly heating : np.ndarray
             hourly heating for the whole simulation period
         """
         return np.tile(self.hourly_heating_load, self.simulation_period)
 
-    def load_hourly_profile(self, file_path: str, header: bool = True, separator: str = ";",
-                            decimal_seperator: str = ".", col_heating: int = 0, col_cooling: int = 1) -> None:
+    def load_hourly_profile(
+        self, file_path: str, header: bool = True, separator: str = ";", decimal_seperator: str = ".", col_heating: int = 0, col_cooling: int = 1
+    ) -> None:
         """
         This function loads in an hourly load profile [kW].
 
         Parameters
         ----------
         file_path : str
             Path to the hourly load file
@@ -371,26 +363,30 @@
         if not self.simulation_period == other.simulation_period:
             return False
         return True
 
     def __add__(self, other):
         if isinstance(other, HourlyGeothermalLoad):
             if self.simulation_period != other.simulation_period:
-                warnings.warn(f'The simulation period for both load classes are different. '
-                              f'The maximum simulation period of '
-                              f'{max(self.simulation_period, other.simulation_period)} years will be taken.')
-            return HourlyGeothermalLoad(self._hourly_heating_load + other._hourly_heating_load,
-                                        self._hourly_cooling_load + other._hourly_cooling_load,
-                                        max(self.simulation_period, other.simulation_period),
-                                        self.dhw + other.dhw)
+                warnings.warn(
+                    f"The simulation period for both load classes are different. "
+                    f"The maximum simulation period of "
+                    f"{max(self.simulation_period, other.simulation_period)} years will be taken."
+                )
+            return HourlyGeothermalLoad(
+                self._hourly_heating_load + other._hourly_heating_load,
+                self._hourly_cooling_load + other._hourly_cooling_load,
+                max(self.simulation_period, other.simulation_period),
+                self.dhw + other.dhw,
+            )
 
         try:
             return other.__add__(self)
         except TypeError:  # pragma: no cover
-            raise TypeError('Cannot perform addition. Please check if you use correct classes.')  # pragma: no cover
+            raise TypeError("Cannot perform addition. Please check if you use correct classes.")  # pragma: no cover
 
     @property
     def _start_hour(self) -> int:
         """
         This function returns the hour at which the year starts based on the start month.
 
         Returns
@@ -413,8 +409,8 @@
 
         Returns
         -------
         load : np.ndarray
         """
         if self.start_month == 1:
             return array
-        return np.concatenate((array[self._start_hour:], array[:self._start_hour]))
+        return np.concatenate((array[self._start_hour :], array[: self._start_hour]))
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadAbsolute.py` & `ghetool-2.2.2/GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadAbsolute.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import warnings
 
 import numpy as np
 
-from typing import Union
 from GHEtool.VariableClasses.LoadData._LoadData import _LoadData
 from GHEtool.VariableClasses.LoadData.GeothermalLoad import HourlyGeothermalLoad
 from GHEtool.VariableClasses.LoadData.GeothermalLoad.HourlyGeothermalLoadMultiYear import HourlyGeothermalLoadMultiYear
 from GHEtool.logger.ghe_logger import ghe_logger
 
+from numpy.typing import ArrayLike
+
 
 class MonthlyGeothermalLoadAbsolute(_LoadData):
     """
     This class contains all the information for geothermal load data with a monthly resolution and absolute input.
     This means that the inputs are both in kWh/month and kW/month.
     """
 
-    __slots__ = tuple(_LoadData.__slots__) + ('_baseload_heating', '_baseload_cooling',
-                                              '_peak_heating', '_peak_cooling')
+    __slots__ = tuple(_LoadData.__slots__) + ("_baseload_heating", "_baseload_cooling", "_peak_heating", "_peak_cooling")
 
-    def __init__(self, baseload_heating: Union[np.ndarray, list, tuple] = np.zeros(12),
-                 baseload_cooling: Union[np.ndarray, list, tuple] = np.zeros(12),
-                 peak_heating: Union[np.ndarray, list, tuple] = np.zeros(12),
-                 peak_cooling: Union[np.ndarray, list, tuple] = np.zeros(12),
-                 simulation_period: int = 20,
-                 dhw: float = 0.):
+    def __init__(
+        self,
+        baseload_heating: ArrayLike = None,
+        baseload_cooling: ArrayLike = None,
+        peak_heating: ArrayLike = None,
+        peak_cooling: ArrayLike = None,
+        simulation_period: int = 20,
+        dhw: float = 0.0,
+    ):
         """
 
         Parameters
         ----------
         baseload_heating : np.ndarray, list, tuple
             Baseload heating values [kWh/month]
         baseload_cooling : np.ndarray, list, tuple
@@ -47,63 +50,62 @@
         # initiate variables
         self._baseload_heating: np.ndarray = np.zeros(12)
         self._baseload_cooling: np.ndarray = np.zeros(12)
         self._peak_heating: np.ndarray = np.zeros(12)
         self._peak_cooling: np.ndarray = np.zeros(12)
 
         # set variables
-        self.baseload_heating = baseload_heating
-        self.baseload_cooling = baseload_cooling
-        self.peak_heating = peak_heating
-        self.peak_cooling = peak_cooling
+        self.baseload_heating = np.zeros(12) if baseload_heating is None else baseload_heating
+        self.baseload_cooling = np.zeros(12) if baseload_cooling is None else baseload_cooling
+        self.peak_heating = np.zeros(12) if peak_heating is None else peak_heating
+        self.peak_cooling = np.zeros(12) if peak_cooling is None else peak_cooling
         self.dhw = dhw
 
-    def _check_input(self, input: Union[np.ndarray, list, tuple]) -> bool:
+    def _check_input(self, load_array: ArrayLike) -> bool:
         """
         This function checks whether the input is valid or not.
         The input is correct if and only if:
         1) the input is a np.ndarray, list or tuple
         2) the length of the input is 12
         3) the input does not contain any negative values.
 
         Parameters
         ----------
-        input : np.ndarray, list or tuple
+        load_array : np.ndarray, list or tuple
 
         Returns
         -------
         bool
             True if the inputs are valid
         """
-        if not isinstance(input, (np.ndarray, list, tuple)):
+        if not isinstance(load_array, (np.ndarray, list, tuple)):
             ghe_logger.error("The load should be of type np.ndarray, list or tuple.")
             return False
-        if not len(input) == 12:
+        if not len(load_array) == 12:
             ghe_logger.error("The length of the load should be 12.")
             return False
-        if np.min(input) < 0:
+        if np.min(load_array) < 0:
             ghe_logger.error("No value in the load can be smaller than zero.")
             return False
         return True
 
     @property
     def baseload_cooling(self) -> np.ndarray:
         """
         This function returns the baseload cooling in kWh/month.
 
         Returns
         -------
         baseload cooling : np.ndarray
             Baseload cooling values [kWh/month] for one year, so the length of the array is 12
         """
-        return  self.correct_for_start_month(
-            self._baseload_cooling)
+        return self.correct_for_start_month(self._baseload_cooling)
 
     @baseload_cooling.setter
-    def baseload_cooling(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def baseload_cooling(self, load: ArrayLike) -> None:
         """
         This function sets the baseload cooling [kWh/month] after it has been checked.
         If the baseload cooling gives a higher average power than the peak power,
         this is taken as the peak power in that month.
 
         Parameters
         ----------
@@ -121,15 +123,15 @@
             values
         """
         if self._check_input(load):
             self._baseload_cooling = np.array(load)
             return
         raise ValueError
 
-    def set_baseload_cooling(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_baseload_cooling(self, load: ArrayLike) -> None:
         """
         This function sets the baseload cooling [kWh/month] after it has been checked.
         If the baseload cooling gives a higher average power than the peak power,
         this is taken as the peak power in that month.
 
         Parameters
         ----------
@@ -154,19 +156,18 @@
         This function returns the baseload heating in kWh/month (incl. DHW).
 
         Returns
         -------
         baseload heating : np.ndarray
             Baseload heating values (incl. DHW) [kWh/month] for one year, so the length of the array is 12
         """
-        return self.correct_for_start_month(
-            self._baseload_heating + self.dhw / 8760 * self.UPM)
+        return self.correct_for_start_month(self._baseload_heating + self.dhw / 8760 * self.UPM)
 
     @baseload_heating.setter
-    def baseload_heating(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def baseload_heating(self, load: ArrayLike) -> None:
         """
         This function sets the baseload heating [kWh/month] after it has been checked.
         If the baseload heating gives a higher average power than the peak power,
         this is taken as the peak power in that month.
 
         Parameters
         ----------
@@ -184,15 +185,15 @@
             values
         """
         if self._check_input(load):
             self._baseload_heating = np.array(load)
             return
         raise ValueError
 
-    def set_baseload_heating(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_baseload_heating(self, load: ArrayLike) -> None:
         """
         This function sets the baseload heating [kWh/month] after it has been checked.
         If the baseload heating gives a higher average power than the peak power,
         this is taken as the peak power in that month.
 
         Parameters
         ----------
@@ -217,16 +218,15 @@
         This function returns the peak cooling load in kW/month.
 
         Returns
         -------
         peak cooling : np.ndarray
             Peak cooling values for one year, so the length of the array is 12
         """
-        return self.correct_for_start_month(
-            np.maximum(self._peak_cooling, self.baseload_cooling_power))
+        return self.correct_for_start_month(np.maximum(self._peak_cooling, self.baseload_cooling_power))
 
     @peak_cooling.setter
     def peak_cooling(self, load) -> None:
         """
         This function sets the peak cooling load [kW/month] after it has been checked.
         If the baseload cooling gives a higher average power, this is taken as the peak power in that month.
 
@@ -246,15 +246,15 @@
             values
         """
         if self._check_input(load):
             self._peak_cooling = np.array(load)
             return
         raise ValueError
 
-    def set_peak_cooling(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_peak_cooling(self, load: ArrayLike) -> None:
         """
         This function sets the peak cooling load [kW/month] after it has been checked.
         If the baseload cooling gives a higher average power, this is taken as the peak power in that month.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
@@ -278,19 +278,18 @@
         This function returns the peak heating load in kW/month.
 
         Returns
         -------
         peak heating : np.ndarray
             Peak heating values for one year, so the length of the array is 12
         """
-        return self.correct_for_start_month(
-            np.maximum(np.array(self._peak_heating) + self.dhw_power, self.baseload_heating_power))
+        return self.correct_for_start_month(np.maximum(np.array(self._peak_heating) + self.dhw_power, self.baseload_heating_power))
 
     @peak_heating.setter
-    def peak_heating(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def peak_heating(self, load: ArrayLike) -> None:
         """
         This function sets the peak heating load [kW/month] after it has been checked.
         If the baseload heating gives a higher average power, this is taken as the peak power in that month.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
@@ -307,15 +306,15 @@
             values
         """
         if self._check_input(load):
             self._peak_heating = np.array(load)
             return
         raise ValueError
 
-    def set_peak_heating(self, load: Union[np.ndarray, list, tuple]) -> None:
+    def set_peak_heating(self, load: ArrayLike) -> None:
         """
         This function sets the peak heating load [kW/month] after it has been checked.
         If the baseload heating gives a higher average power, this is taken as the peak power in that month.
 
         Parameters
         ----------
         load : np.ndarray, list or tuple
@@ -347,64 +346,76 @@
         if not self.simulation_period == other.simulation_period:
             return False
         return True
 
     def __add__(self, other):
         if isinstance(other, MonthlyGeothermalLoadAbsolute):
             if self.simulation_period != other.simulation_period:
-                warnings.warn(f'The simulation period for both load classes are different. '
-                              f'The maximum simulation period of '
-                              f'{max(self.simulation_period, other.simulation_period)} years will be taken.')
+                warnings.warn(
+                    f"The simulation period for both load classes are different. "
+                    f"The maximum simulation period of "
+                    f"{max(self.simulation_period, other.simulation_period)} years will be taken."
+                )
             if self.peak_cooling_duration != other.peak_cooling_duration:
-                warnings.warn(f'The peak cooling duration for both load classes are different. '
-                              f'The maximum peak cooling duration of '
-                              f'{max(self.peak_cooling_duration, other.peak_cooling_duration)} hours will be taken.')
+                warnings.warn(
+                    f"The peak cooling duration for both load classes are different. "
+                    f"The maximum peak cooling duration of "
+                    f"{max(self.peak_cooling_duration, other.peak_cooling_duration)} hours will be taken."
+                )
             if self.peak_heating_duration != other.peak_heating_duration:
-                warnings.warn(f'The peak heating duration for both load classes are different. '
-                              f'The maximum peak heating duration of '
-                              f'{max(self.peak_heating_duration, other.peak_heating_duration)} hours will be taken.')
-
-            result = MonthlyGeothermalLoadAbsolute(self._baseload_heating + other._baseload_heating,
-                                                   self._baseload_cooling + other._baseload_cooling,
-                                                   self._peak_heating + other._peak_heating,
-                                                   self._peak_cooling + other._peak_cooling,
-                                                   max(self.simulation_period, other.simulation_period),
-                                                   self.dhw + other.dhw)
+                warnings.warn(
+                    f"The peak heating duration for both load classes are different. "
+                    f"The maximum peak heating duration of "
+                    f"{max(self.peak_heating_duration, other.peak_heating_duration)} hours will be taken."
+                )
+
+            result = MonthlyGeothermalLoadAbsolute(
+                self._baseload_heating + other._baseload_heating,
+                self._baseload_cooling + other._baseload_cooling,
+                self._peak_heating + other._peak_heating,
+                self._peak_cooling + other._peak_cooling,
+                max(self.simulation_period, other.simulation_period),
+                self.dhw + other.dhw,
+            )
             result.peak_cooling_duration = max(self._peak_cooling_duration, other._peak_cooling_duration)
             result.peak_heating_duration = max(self._peak_heating_duration, other._peak_heating_duration)
 
             return result
 
         # multiyear hourly
         if isinstance(other, HourlyGeothermalLoadMultiYear):
-            raise TypeError('You cannot add an HourlyMultiYear input with a monthly based input.')
+            raise TypeError("You cannot add an HourlyMultiYear input with a monthly based input.")
 
         # hourly load
         if isinstance(other, HourlyGeothermalLoad):
-            warnings.warn('You add an hourly to a monthly load, the result will hence be a monthly load.')
+            warnings.warn("You add an hourly to a monthly load, the result will hence be a monthly load.")
             if self.simulation_period != other.simulation_period:
-                warnings.warn(f'The simulation period for both load classes are different. '
-                              f'The maximum simulation period of '
-                              f'{max(self.simulation_period, other.simulation_period)} years will be taken.')
+                warnings.warn(
+                    f"The simulation period for both load classes are different. "
+                    f"The maximum simulation period of "
+                    f"{max(self.simulation_period, other.simulation_period)} years will be taken."
+                )
 
             peak_heating, baseload_heating = other.resample_to_monthly(other._hourly_heating_load)
             peak_cooling, baseload_cooling = other.resample_to_monthly(other._hourly_cooling_load)
 
-            result = MonthlyGeothermalLoadAbsolute(self._baseload_heating + baseload_heating,
-                                                   self._baseload_cooling + baseload_cooling,
-                                                   self._peak_heating + peak_heating,
-                                                   self._peak_cooling + peak_cooling,
-                                                   max(self.simulation_period, other.simulation_period),
-                                                   self.dhw + other.dhw)
+            result = MonthlyGeothermalLoadAbsolute(
+                self._baseload_heating + baseload_heating,
+                self._baseload_cooling + baseload_cooling,
+                self._peak_heating + peak_heating,
+                self._peak_cooling + peak_cooling,
+                max(self.simulation_period, other.simulation_period),
+                self.dhw + other.dhw,
+            )
             result.peak_cooling_duration = self._peak_cooling_duration
             result.peak_heating_duration = self._peak_heating_duration
 
             return result
 
-        raise TypeError('Cannot perform addition. Please check if you use correct classes.')
+        raise TypeError("Cannot perform addition. Please check if you use correct classes.")
 
     def correct_for_start_month(self, array: np.ndarray) -> np.ndarray:
         """
         This function corrects the load for the correct start month.
         If the simulation starts in september, the start month is 9 and hence the array should start
         at index 9.
 
@@ -415,8 +426,8 @@
 
         Returns
         -------
         load : np.ndarray
         """
         if self.start_month == 1:
             return array
-        return np.concatenate((array[self.start_month-1:], array[:self.start_month-1]))
+        return np.concatenate((array[self.start_month - 1 :], array[: self.start_month - 1]))
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/LoadData/_LoadData.py` & `ghetool-2.2.2/GHEtool/VariableClasses/LoadData/_LoadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
 
         Returns
         -------
         Hours per month : np.ndarray
         """
         if self.all_months_equal:
             # every month has equal length
-            return np.ones(12) * _LoadData.AVG_UPM
+            return np.full(12, _LoadData.AVG_UPM, dtype=np.int64)
         else:
-            return np.array([744, 672, 744, 720, 744, 720, 744, 744, 720, 744, 720, 744])
+            return np.array([744, 672, 744, 720, 744, 720, 744, 744, 720, 744, 720, 744], dtype=np.int64)
 
     @abc.abstractmethod
     def _check_input(self, input: Union[np.ndarray, list, tuple]) -> bool:
         """
         This function checks whether the input is valid or not.
 
         Parameters
@@ -269,15 +269,15 @@
             peak cooling for the whole simulation period
         """
         return np.tile(self.peak_cooling, self.simulation_period)
 
     @property
     def baseload_heating_power_simulation_period(self) -> np.ndarray:
         """
-        This function returns the avergae heating power in kW avg/month for a whole simulation period.
+        This function returns the average heating power in kW avg/month for a whole simulation period.
 
         Returns
         -------
         average heating power : np.ndarray
             average heating power for the whole simulation period
         """
         return np.tile(self.baseload_heating_power, self.simulation_period)
@@ -322,15 +322,15 @@
         """
         This function calculates the average monthly load in kW for the whole simulation period.
 
         Returns
         -------
         monthly average load : np.ndarray
         """
-        return np.tile(self.monthly_average_load, self.simulation_period)
+        return self.baseload_cooling_power_simulation_period - self.baseload_heating_power_simulation_period
 
     @property
     def peak_heating_duration(self) -> float:
         """
         Length of the peak in heating.
 
         Returns
@@ -588,26 +588,26 @@
         """
         This returns the max peak cooling in kW.
 
         Returns
         -------
         max peak cooling : float
         """
-        return np.max(self.peak_cooling)
+        return np.max(self.peak_cooling_simulation_period)
 
     @property
     def max_peak_heating(self) -> float:
         """
         This returns the max peak heating in kW.
 
         Returns
         -------
         max peak heating : float
         """
-        return np.max(self.peak_heating)
+        return np.max(self.peak_heating_simulation_period)
 
     def add_dhw(self, dhw: float) -> None:
         """
         This function adds the domestic hot water (dhw).
         An error is raies is the dhw is not positive.
 
         Parameters
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/CoaxialPipe.py` & `ghetool-2.2.2/GHEtool/VariableClasses/PipeData/CoaxialPipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,51 +5,56 @@
 
 from GHEtool.VariableClasses.PipeData._PipeData import _PipeData
 from GHEtool.VariableClasses.FluidData import FluidData
 
 
 class CoaxialPipe(_PipeData):
     """
-    Contains information regarding the Multiple U-Tube class.
+    Contains information regarding the Coaxial pipe class.
     """
 
-    __slots__ = 'r_in_in', 'r_in_out', 'r_out_in', 'r_out_out', 'k_g', 'is_inner_inlet', 'R_ff', 'R_fp'
+    __slots__ = 'r_in_in', 'r_in_out', 'r_out_in', 'r_out_out', 'k_g', 'is_inner_inlet', 'R_ff', 'R_fp', 'k_p_out'
 
     def __init__(self, r_in_in: float = None, r_in_out: float = None,
                  r_out_in: float = None, r_out_out: float = None, k_p: float = None, k_g: float = None,
-                 epsilon: float = 1e-6, is_inner_inlet: bool = True):
+                 epsilon: float = 1e-6, is_inner_inlet: bool = True, k_p_out: float = None):
         """
 
         Parameters
         ----------
         r_in_in : float
             Inner radius of the inner annulus [m]
         r_in_out : float
             Outer radius of the inner annulus [m]
         r_out_in : float
             Inner radius of the outer annulus [m]
         r_out_out : float
             Outer radius of the outer annulus [m]
         k_p : float
-            Pipe thermal conductivity  [W/mK]
+            Pipe thermal conductivity of the inner and outer pipe [W/mK]. If k_p_out is set, k_p is only used for
+            the conductivity of the inner pipe.
         k_g : float
             Thermal conductivity of the grout [W/mK]
         epsilon : float
             Pipe roughness of the tube [m]
         is_inner_inlet : bool
             True if the inlet of the fluid is through the inner annulus
+        k_p_out : float
+            Pipe conductivity of the outer pipe [W/mK]. If None, it is assumed that the outer pipe has the same
+            conductivity as the inner pipe (k_p).
         """
         super().__init__(epsilon=epsilon, k_g=k_g, k_p=k_p)
         self.r_in_in: float = r_in_in
         self.r_in_out: float = r_in_out
         self.r_out_in: float = r_out_in
         self.r_out_out: float = r_out_out
         self.is_inner_inlet: bool = is_inner_inlet
         self.R_ff: float = 0.
         self.R_fp: float = 0.
+        self.k_p_out = k_p if k_p_out is None else k_p_out
 
     def calculate_resistances(self, fluid_data: FluidData) -> None:
         """
         This function calculates the conductive and convective resistances, which are constant.
 
         Parameters
         ----------
@@ -62,15 +67,16 @@
         """
         # Pipe thermal resistances [m.K/W]
         # Inner pipe
         R_p_in = gt.pipes.conduction_thermal_resistance_circular_pipe(
             self.r_in_in, self.r_in_out, self.k_p)
         # Outer pipe
         R_p_out = gt.pipes.conduction_thermal_resistance_circular_pipe(
-            self.r_out_in, self.r_out_out, self.k_p)
+            self.r_out_in, self.r_out_out, self.k_p_out)
+
         # Fluid-to-fluid thermal resistance [m.K/W]
         # Inner pipe
         h_f_in = gt.pipes.convective_heat_transfer_coefficient_circular_pipe(
             fluid_data.mfr, self.r_in_in, fluid_data.mu, fluid_data.rho, fluid_data.k_f, fluid_data.Cp, self.epsilon)
         R_f_in = 1.0 / (h_f_in * 2 * np.pi * self.r_in_in)
         # Outer pipe
         h_f_a_in, h_f_a_out = \
```

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/DoubleUTube.py` & `ghetool-2.2.2/GHEtool/VariableClasses/PipeData/DoubleUTube.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/MultipleUTube.py` & `ghetool-2.2.2/GHEtool/VariableClasses/PipeData/MultipleUTube.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/SingleUTube.py` & `ghetool-2.2.2/GHEtool/VariableClasses/PipeData/SingleUTube.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/PipeData/_PipeData.py` & `ghetool-2.2.2/GHEtool/VariableClasses/PipeData/_PipeData.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/Result.py` & `ghetool-2.2.2/GHEtool/VariableClasses/Result.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/VariableClasses/cylindrical_correction.py` & `ghetool-2.2.2/GHEtool/VariableClasses/cylindrical_correction.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/logger/ghe_logger.py` & `ghetool-2.2.2/GHEtool/logger/ghe_logger.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/main_class.py` & `ghetool-2.2.2/GHEtool/Borefield.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,2032 +1,2302 @@
-"""
-This file contains all the code for the borefield calculations.
-"""
-from __future__ import annotations
-
-import copy
-import warnings
-from math import pi
-from pathlib import Path
-from typing import Tuple
-import logging
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pygfunction as gt
-from scipy.signal import convolve
-from warnings import warn
-
-from GHEtool.VariableClasses import FluidData, Borehole, GroundConstantTemperature, Results
-from GHEtool.VariableClasses import CustomGFunction, load_custom_gfunction, GFunction, CalculationSetup
-from GHEtool.VariableClasses.LoadData import *
-from GHEtool.VariableClasses.LoadData import _LoadData
-from GHEtool.VariableClasses.PipeData import _PipeData
-from GHEtool.VariableClasses.BaseClass import BaseClass, UnsolvableDueToTemperatureGradient, MaximumNumberOfIterations
-from GHEtool.VariableClasses.GroundData._GroundData import _GroundData
-from GHEtool.logger.ghe_logger import ghe_logger
-
-
-class Borefield(BaseClass):
-    """Main borefield class"""
-    UPM: float = 730.  # number of hours per month
-    THRESHOLD_BOREHOLE_DEPTH: float = 0.05  # threshold for iteration
-    MAX_SIMULATION_PERIOD: int = 100  # maximal value for simulation
-
-    # define default values
-    DEFAULT_INVESTMENT: list = [35, 0]  # 35 EUR/m
-    DEFAULT_LENGTH_PEAK: int = 6  # hours
-    THRESHOLD_DEPTH_ERROR: int = 10000  # m
-
-    HOURLY_LOAD_ARRAY: np.ndarray = np.arange(0, 8761, UPM).astype(np.uint32)
-
-    __slots__ = 'H', 'borehole', \
-        'number_of_boreholes', '_borefield', 'cost_investment', \
-        'Tf_max', 'Tf_min', 'limiting_quadrant', \
-        'Tf', \
-        '_ground_data', '_borefield_load', \
-        'options_pygfunction', \
-        'THRESHOLD_WARNING_SHALLOW_FIELD', \
-        'D', 'r_b', 'gfunction_calculation_object', \
-        '_calculation_setup', \
-        '_secundary_borefield_load', '_building_load', '_external_load'
-
-    def __init__(self, peak_heating: np.ndarray | list = None,
-                 peak_cooling: np.ndarray | list = None,
-                 baseload_heating: np.ndarray | list = None,
-                 baseload_cooling: np.ndarray | list = None,
-                 borefield=None,
-                 custom_gfunction: CustomGFunction = None,
-                 load: _LoadData = None):
-        """
-
-        Parameters
-        ----------
-        peak_heating : list, numpy array
-            Monthly peak heating values [kW]
-        peak_cooling : list, numpy array
-            Monthly peak cooling values [kW]
-        baseload_heating : list, numpy array
-            Monthly baseload heating values [kWh]
-        baseload_cooling : list, numpy array
-            Monthly baseload heating values [kWh]
-        borefield : pygfunction borehole/borefield object
-            Set the borefield for which the calculations will be carried out
-        custom_gfunction : CustomGFunction
-            Custom gfunction dataset
-
-        Examples
-        --------
-
-        monthly peak values [kW]
-
-        >>> peak_cooling = np.array([0., 0, 34., 69., 133., 187., 213., 240., 160., 37., 0., 0.])
-        >>> peak_heating = np.array([160., 142, 102., 55., 0., 0., 0., 0., 40.4, 85., 119., 136.])
-
-        annual heating and cooling load [kWh]
-
-        >>> annual_heating_load = 300 * 10 ** 3
-        >>> annual_cooling_load = 160 * 10 ** 3
-
-        percentage of annual load per month (15.5% for January ...)
-
-        >>> monthly_load_heating_percentage = np.array([0.155, 0.148, 0.125, .099, .064, 0., 0., 0., 0.061, 0.087, 0.117, 0.144])
-        >>> monthly_load_cooling_percentage = np.array([0.025, 0.05, 0.05, .05, .075, .1, .2, .2, .1, .075, .05, .025])
-
-        resulting load per month [kWh]
-
-        >>> monthly_load_heating = annual_heating_load * monthly_load_heating_percentage
-        >>> monthly_load_cooling = annual_cooling_load * monthly_load_cooling_percentage
-
-        create the borefield object
-
-        >>> borefield = Borefield()
-
-        set the load
-
-        >>> load = MonthlyGeothermalLoadAbsolute(monthly_load_heating, monthly_load_cooling, peak_heating, peak_cooling)
-        >>> borefield.load = load
-
-        """
-
-        # initiate vars
-        LIST_OF_ZEROS = np.zeros(12)
-        if baseload_cooling is None:
-            baseload_cooling: np.ndarray = LIST_OF_ZEROS
-        if baseload_heating is None:
-            baseload_heating: np.ndarray = LIST_OF_ZEROS
-        if peak_cooling is None:
-            peak_cooling: np.ndarray = LIST_OF_ZEROS
-        if peak_heating is None:
-            peak_heating: np.ndarray = LIST_OF_ZEROS
-
-        self.limiting_quadrant: int = 0  # parameter that tells in which quadrant the field is limited
-        # m hereafter one needs to chance to fewer boreholes with more depth, because the calculations are no longer
-        # that accurate.
-        self.THRESHOLD_WARNING_SHALLOW_FIELD: int = 50
-
-        self.custom_gfunction: CustomGFunction = custom_gfunction
-        self.gfunction_calculation_object: GFunction = GFunction()
-
-        ## params w.r.t. pygfunction
-        self.options_pygfunction: dict = {"method": "equivalent"}
-
-        # initialize variables for temperature plotting
-        self.results = Results()
-
-        # initiate ground parameters
-        self.H = 0.  # borehole depth m
-        self.number_of_boreholes = 0  # number of total boreholes #
-        self._ground_data: _GroundData = GroundConstantTemperature()
-        self.D: float = 0.  # buried depth of the borehole [m]
-        self.r_b: float = 0.  # borehole radius [m]
-
-        # initiate fluid parameters
-        self.Tf: float = 0.  # temperature of the fluid
-        self.Tf_max: float = 16.  # maximum temperature of the fluid
-        self.Tf_min: float = 0.  # minimum temperature of the fluid
-
-        # initiale borehole
-        self.borehole = Borehole()
-
-        # initiate different sizing
-        self._calculation_setup: CalculationSetup = CalculationSetup()
-        self.calculation_setup()
-
-        # load on the geothermal borefield, used in calculations
-        self._borefield_load = MonthlyGeothermalLoadAbsolute()
-        # geothermal load, but converted to a secundary demand in optimise_load_profile
-        self._secundary_borefield_load: HourlyGeothermalLoad = HourlyGeothermalLoad()
-        # secundary load of the building, used in optimise_load_profile
-        self._building_load: HourlyGeothermalLoad = HourlyGeothermalLoad()
-
-        if load is not None:
-            self.load = load
-        else:
-            self.load = MonthlyGeothermalLoadAbsolute(baseload_heating, baseload_cooling,
-                                                      peak_heating, peak_cooling)
-
-        # set investment cost
-        self.cost_investment: list = Borefield.DEFAULT_INVESTMENT
-
-        # set a custom borefield
-        self.borefield = borefield
-
-        ghe_logger.main_info("Borefield object has been created.")
-
-    @staticmethod
-    def activate_logger() -> None:
-        """
-        This function activates the logging.
-
-        Returns
-        -------
-        None
-        """
-        ghe_logger.setLevel("MAIN_INFO")
-
-    @staticmethod
-    def deactivate_logger() -> None:
-        """
-        This function deactivates the logging.
-
-        Returns
-        -------
-        None
-        """
-        ghe_logger.setLevel(logging.INFO)
-
-    def _set_number_of_boreholes(self) -> None:
-        """
-        This functions sets the number of boreholes based on the length of the borefield attribute.
-
-        Returns
-        -------
-        None
-        """
-        self.number_of_boreholes = len(self.borefield) if self.borefield is not None else 0
-
-    def set_borefield(self, borefield: list[gt.boreholes.Borehole] = None) -> None:
-        """
-        This function set the borefield object. When None is given, the borefield will be deleted.
-
-        Parameters
-        ----------
-        borefield : List[pygfunction.boreholes.Borehole]
-            Borefield created with the pygfunction package
-
-        Returns
-        -------
-        None
-        """
-        self.borefield = borefield
-
-    def create_rectangular_borefield(self, N_1: int, N_2: int, B_1: int, B_2: int, H: float, D: float = 1,
-                                     r_b: float = 0.075):
-        """
-        This function creates a rectangular borefield.
-        It calls the pygfunction module in the background.
-        The documentation of this function is based on pygfunction.
-
-        Parameters
-        ----------
-        N_1 : int
-            Number of boreholes in the x direction
-        N_2 : int
-            Number of boreholes in the y direction
-        B_1 : int
-            Distance between adjacent boreholes in the x direction [m]
-        B_2 : int
-            Distance between adjacent boreholes in the y direction [m]
-        H : float
-            Borehole depth [m]
-        D : float
-            Borehole buried depth [m]
-        r_b : float
-            Borehole radius [m]
-
-        Returns
-        -------
-        pygfunction borefield object
-        """
-        borefield = gt.boreholes.rectangle_field(N_1, N_2, B_1, B_2, H, D, r_b)
-        self.set_borefield(borefield)
-
-        return borefield
-
-    def create_circular_borefield(self, N: int, R: float, H: float, D: float = 1, r_b: float = 0.075):
-        """
-        This function creates a circular borefield.
-        It calls the pygfunction module in the background.
-        The documentation of this function is based on pygfunction.
-
-        Parameters
-        ----------
-        N : int
-            Number of boreholes in the borefield
-        R : float
-            Distance of boreholes from the center of the field
-        H : float
-            Borehole depth [m]
-        D : float
-            Borehole buried depth [m]
-        r_b : float
-            Borehole radius [m]
-
-        Returns
-        -------
-        pygfunction borefield object
-        """
-        borefield = gt.boreholes.circle_field(N, R, H, D, r_b)
-        self.set_borefield(borefield)
-        return borefield
-
-    @property
-    def borefield(self):
-        """
-        Returns the hidden _borefield variable.
-
-        Returns
-        -------
-        Hidden _borefield object
-        """
-        return self._borefield
-
-    @borefield.setter
-    def borefield(self, borefield: list[gt.boreholes.Borehole] = None) -> None:
-        """
-        This function sets the borefield configuration. When no input is given, the borefield variable will be deleted.
-
-        Parameters
-        ----------
-        borefield : List[pygfunction.boreholes.Borehole]
-            Borefield created with the pygfunction package
-
-        Returns
-        -------
-        None
-        """
-        if borefield is None:
-            del self.borefield
-            return
-        self._borefield = borefield
-        self._set_number_of_boreholes()
-        self.D = borefield[0].D
-        self.r_b = borefield[0].r_b
-        self.H = borefield[0].H
-        self.gfunction_calculation_object.remove_previous_data()
-
-    @borefield.deleter
-    def borefield(self):
-        """
-        This function deletes the hidden _borefield object.
-        It also sets the number of boreholes to zero
-
-        Returns
-        -------
-        None
-        """
-        self._borefield = None
-        self._set_number_of_boreholes()
-        self.gfunction_calculation_object.remove_previous_data()
-        self.custom_gfunction = None
-
-    def _update_borefield_depth(self, H: float = None) -> None:
-        """
-        This function updates the borehole depth.
-
-        Parameters
-        ----------
-        H : float
-            Borehole depth.
-
-        Returns
-        -------
-        None
-        """
-        H = H if H is not None else self.H
-
-        if self._borefield[0].H == H:
-            # the borefield is already at the correct depth
-            return
-
-        for bor in self._borefield:
-            bor.H = H
-
-    def load_custom_gfunction(self, location: str) -> None:
-        """
-        This function loads the custom gfunction.
-
-        Parameters
-        ----------
-        location : str
-            Path to the location of the custom gfunction file
-
-        Returns
-        -------
-        None
-        """
-
-        self.custom_gfunction = load_custom_gfunction(location)
-        ghe_logger.main_info("Custom g-function has been loaded.")
-
-    def set_investment_cost(self, investment_cost: list = None) -> None:
-        """
-        This function sets the investment cost. This is linear with respect to the total field length.
-        If None, the default is set.
-
-        Parameters
-        ----------
-        investment_cost : list
-            1D array of polynomial coefficients (including coefficients equal to zero) from highest degree to the constant term
-
-        Returns
-        -------
-        None
-        """
-        if investment_cost is None:
-            investment_cost = Borefield.DEFAULT_INVESTMENT
-        self.cost_investment: list = investment_cost
-
-    def set_length_peak(self, length: float = DEFAULT_LENGTH_PEAK) -> None:
-        """
-        This function sets the length of the peak.
-
-        Parameters
-        ----------
-        length : float
-            Length of the peak [hours]
-
-        Returns
-        -------
-        None
-        """
-        self._borefield_load.peak_duration = length
-
-    def set_load(self, load: _LoadData) -> None:
-        """
-        This function sets the _load attribute.
-
-        Parameters
-        ----------
-        load : _LoadData
-            Load data object
-
-        Returns
-        -------
-        None
-        """
-        self.load = load
-
-    @property
-    def load(self) -> _LoadData | HourlyGeothermalLoad | MonthlyGeothermalLoadAbsolute:
-        """
-        This returns the LoadData object.
-
-        Returns
-        -------
-        Load data: LoadData
-        """
-        return self._borefield_load
-
-    @load.setter
-    def load(self, load: _LoadData) -> None:
-        """
-        This function sets the _load attribute.
-
-        Parameters
-        ----------
-        load : _LoadData
-            Load data object
-
-        Returns
-        -------
-        None
-        """
-        self._borefield_load = load
-        self._delete_calculated_temperatures()
-
-    @property
-    def simulation_period(self) -> int:
-        """
-        This returns the simulation period from the LoadData object.
-
-        Returns
-        -------
-        Simulation period [years] : int
-        """
-        return self.load.simulation_period
-
-    @simulation_period.setter
-    def simulation_period(self, simulation_period: float) -> None:
-        """
-        This function sets the simulation period.
-
-        Parameters
-        ----------
-        simulation_period : float
-            Simulation period in years
-
-        Returns
-        -------
-        None
-        """
-        self._borefield_load.simulation_period = simulation_period
-
-    @property
-    def Rb(self) -> float:
-        """
-        This function returns the equivalent borehole thermal resistance.
-
-        Returns
-        -------
-        Rb : float
-            Equivalent borehole thermal resistance [mK/W]
-        """
-        return self.borehole.get_Rb(self.H, self.D, self.r_b, self.ground_data.k_s)
-
-    @Rb.setter
-    def Rb(self, Rb: float) -> None:
-        """
-        This function sets the constant equivalent borehole thermal resistance.
-
-        Parameters
-        ----------
-        Rb : float
-            Equivalent borehole thermal resistance [mk/W]
-
-        Returns
-        -------
-        None
-        """
-        self.set_Rb(Rb)
-
-    @property
-    def ground_data(self) -> _GroundData:
-        """"
-        This function returns the ground data.
-
-        Returns
-        -------
-        ground data : GroundData
-
-        """
-        return self._ground_data
-
-    @ground_data.setter
-    def ground_data(self, data: _GroundData) -> None:
-        """
-        This function sets the relevant ground parameters.
-
-        Parameters
-        ----------
-        data : GroundData
-            All the relevant ground data
-
-        Returns
-        -------
-        None
-        """
-        # Ground properties
-        self._ground_data = data
-
-        # new ground data implies that a new g-function should be loaded
-        self.custom_gfunction = None
-
-        # the stored gfunction data should be deleted
-        self.gfunction_calculation_object.remove_previous_data()
-
-    def set_ground_parameters(self, data: _GroundData) -> None:
-        """
-        This function sets the relevant ground parameters.
-
-        Parameters
-        ----------
-        data : GroundData
-            All the relevant ground data
-
-        Returns
-        -------
-        None
-        """
-
-        # Ground properties
-        self.ground_data = data
-
-    def set_fluid_parameters(self, data: FluidData) -> None:
-        """
-        This function sets the fluid parameters.
-
-        Parameters
-        ----------
-        data : FluidData
-            All the relevant fluid data
-
-        Returns
-        -------
-        None
-        """
-        self.borehole.fluid_data = data
-
-    def set_pipe_parameters(self, data: _PipeData) -> None:
-        """
-        This function sets the pipe parameters.
-
-        Parameters
-        ----------
-        data : PipeData
-            All the relevant pipe parameters
-
-        Returns
-        -------
-        None
-        """
-        self.borehole.pipe_data = data
-
-    def set_Rb(self, Rb: float) -> None:
-        """
-        This function sets the constant equivalent borehole thermal resistance.
-
-        Parameters
-        ----------
-        Rb : float
-            Equivalent borehole thermal resistance (mK/W)
-
-        Returns
-        -------
-        None
-        """
-        self.borehole.Rb = Rb
-
-    def set_max_avg_fluid_temperature(self, temp: float) -> None:
-        """
-        This functions sets the maximal average fluid temperature to temp.
-
-        Parameters
-        ----------
-        temp : float
-            Maximal average fluid temperature [deg C]
-
-        Returns
-        -------
-        None
-
-        Raises
-        ------
-        ValueError
-            When the maximal average fluid temperature is lower than the minimal average fluid temperature
-        """
-        if temp <= self.Tf_min:
-            raise ValueError(f'The maximum average fluid temperature {temp} is lower than the minimum average fluid temperature {self.Tf_min}')
-        self.Tf_max: float = temp
-
-    def set_min_avg_fluid_temperature(self, temp: float) -> None:
-        """
-        This functions sets the minimal average fluid temperature to temp.
-
-        Parameters
-        ----------
-        temp : float
-            Minimal average fluid temperature [deg C]
-
-        Returns
-        -------
-        None
-
-        Raises
-        ------
-        ValueError
-            When the maximal average temperature is lower than the minimal average temperature
-        """
-        if temp >= self.Tf_max:
-            raise ValueError(f'The minimum average fluid temperature {temp} is lower than the maximum average fluid temperature {self.Tf_max}')
-        self.Tf_min: float = temp
-
-    def _Tg(self, H: float = None) -> float:
-        """
-        This function gives back the ground temperature.
-
-        Parameters
-        ----------
-        H : float
-            Depth of the field at which the temperature is to be evaluated
-
-        Returns
-        -------
-        Temperature of the ground : float
-        """
-        # check if specific depth is given
-        if H is None:
-            H = self.H
-
-        return self.ground_data.calculate_Tg(H)
-
-    def _check_convergence(self, new_depth: float, old_depth: float, iter: int) -> bool:
-        """
-        This function checks, with the absolute and relative tolerance, if the depth is converged.
-        This is the case if both criteria are met. Raises MaximumNumberOfIterations error if the max number of iterations is crossed.
-
-        Parameters
-        ----------
-        new_depth : float
-            Depth from the current interation [m]
-        old_depth : float
-            Depth from the previous iteration [m]
-        iter : int
-            Current number of iteration
-
-        Returns
-        -------
-        bool
-            True if the depth is converged
-
-        Raises
-        ------
-        MaximumNumberOfIterations
-            MaximumNumberOfIterations if the max number of iterations is crossed
-        """
-        if iter + 1 > self._calculation_setup.max_nb_of_iterations:
-            raise MaximumNumberOfIterations(self._calculation_setup.max_nb_of_iterations)
-
-        if old_depth == 0:
-            return False
-        test_a_tol = abs(new_depth - old_depth) <= self._calculation_setup.atol if self._calculation_setup.atol != False else True
-        test_rtol = abs(
-            new_depth - old_depth) / old_depth <= self._calculation_setup.rtol if self._calculation_setup.rtol != False else True
-
-        return test_a_tol and test_rtol
-
-    def _Ahmadfard(self, th: float, qh: float, qm: float, qa: float) -> float:
-        """
-        This function sizes the field based on the last year of operation, i.e. quadrants 2 and 4.
-
-        It uses the methodology developed by (Ahmadfard and Bernier, 2019) [#Ahmadfard2019]_.
-        The concept of borefield quadrants is developed by (Peere et al., 2020) [#PeereBS]_ [#PeereThesis]_.
-
-        Parameters
-        ----------
-        th : float
-            Peak duration [s]
-        qh : float
-            Peak load [W]
-        qm : float
-            Monthly average load [W]
-        qa : float
-            Yearly imbalance load [W]
-
-        Returns
-        -------
-        H : float
-            Required borehole depth [m]
-
-        References
-        ----------
-        .. [#Ahmadfard2019] Ahmadfard M. and Bernier M., A review of vertical ground heat exchanger sizing tools including an inter-model comparison,
-        Renewable and Sustainable Energy Reviews, Volume 110, 2019, Pages 247-265, ISSN 1364-0321, https://doi.org/10.1016/j.rser.2019.04.045
-        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
-        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
-        """
-        # initiate iteration
-        H_prev = 0
-        # set minimal depth to 50 m
-        self.H = 50 if self.H < 1 else self.H
-
-        time = np.array([th, th + self.load.tm, self.load.ty + self.load.tm + th])
-        # Iterates as long as there is no convergence
-        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
-        i = 0
-        while not self._check_convergence(self.H, H_prev, i):
-            # calculate the required g-function values
-            gfunct_uniform_T = self.gfunction(time, max(1, self.H))
-            # calculate the thermal resistances
-            Ra = (gfunct_uniform_T[2] - gfunct_uniform_T[1]) / (2 * pi * self.ground_data.k_s)
-            Rm = (gfunct_uniform_T[1] - gfunct_uniform_T[0]) / (2 * pi * self.ground_data.k_s)
-            Rd = (gfunct_uniform_T[0]) / (2 * pi * self.ground_data.k_s)
-            # calculate the total borehole length
-            L = (qa * Ra + qm * Rm + qh * Rd + qh * self.Rb) / abs(self.Tf - self._Tg())
-            # updating the depth values
-            H_prev = self.H
-            self.H = L / self.number_of_boreholes
-            i += 1
-
-        return self.H
-
-    def _Carcel(self, th: float, tcm: float, qh: float, qpm: float, qm: float) -> float:
-        """
-        This function sizes the field based on the first year of operation, i.e. quadrants 1 and 3.
-
-        It uses the methodology developed by (Monzo et al., 2016) [#Monzo]_ and adapted by (Peere et al., 2021) [#PeereBS]_.
-        The concept of borefield quadrants is developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_.
-
-        Returns
-        -------
-        H : float
-            Required borehole depth [m]
-
-        References
-        ----------
-        .. [#Monzo] Monzo, P., M. Bernier, J. Acuna, and P. Mogensen. (2016). A monthly based bore field sizing methodology with applications to optimum borehole spacing. ASHRAE Transactions 122, 111–126.
-        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
-        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
-        """
-
-        # initiate iteration
-        H_prev = 0
-        time_steps = [th, th + self.load.tm, tcm + th]
-        if self.H < 1:
-            self.H = 50
-
-        # Iterates as long as there is no convergence
-        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
-        i = 0
-        while not self._check_convergence(self.H, H_prev, i):
-            # get the g-function values
-            gfunc_uniform_T = self.gfunction(time_steps, max(1, self.H))
-
-            # calculate the thermal resistances
-            Rpm = (gfunc_uniform_T[2] - gfunc_uniform_T[1]) / (2 * pi * self.ground_data.k_s)
-            Rcm = (gfunc_uniform_T[1] - gfunc_uniform_T[0]) / (2 * pi * self.ground_data.k_s)
-            Rh = (gfunc_uniform_T[0]) / (2 * pi * self.ground_data.k_s)
-
-            # calculate the total length
-            L = (qh * self.Rb + qh * Rh + qm * Rcm + qpm * Rpm) / abs(self.Tf - self._Tg())
-
-            # updating the depth values
-            H_prev = self.H
-            self.H = L / self.number_of_boreholes
-            i += 1
-        return self.H
-
-    def calculation_setup(self, calculation_setup: CalculationSetup = None, use_constant_Rb: bool = None, **kwargs) -> None:
-        """
-        This function sets the options for the sizing function.
-
-        * The L2 sizing is the one explained in (Peere et al., 2021) [#PeereBS]_ and is the quickest method (it uses 3 pulses)
-
-        * The L3 sizing is a more general approach which is slower but more accurate (it uses 24 pulses/year)
-
-        * The L4 sizing is the most exact one, since it uses hourly data (8760 pulses/year)
-
-        Parameters
-        ----------
-        calculation_setup : CalculationSetup
-            An instance of the CalculationSetup class. When this argument differs from None, all the other parameters are
-            set based on this calculation_setup
-        use_constant_Rb : bool
-            True if a constant borehole equivalent resistance (Rb*) value should be used
-        kwargs
-            Dictionary with all the other options that can be set within GHEtool. For a complete list,
-            see the documentation in the CalculationSetup class.
-
-        Returns
-        -------
-        None
-
-        References
-        ----------
-        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
-        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
-        """
-
-        # if calculation_setup is not None, then the sizing setup is set directly
-        if calculation_setup is not None:
-            self._calculation_setup = calculation_setup
-            return
-
-        self._calculation_setup.update_variables(**kwargs)
-
-        if not use_constant_Rb is None:
-            self.borehole.use_constant_Rb = use_constant_Rb
-
-    def size(self, H_init: float = None, use_constant_Rb: bool = None, L2_sizing: bool = None,
-             L3_sizing: bool = None, L4_sizing: bool = None, quadrant_sizing: int = None, **kwargs) -> float:
-        """
-        This function sets the options for the sizing function.
-
-        * The L2 sizing is the one explained in (Peere et al., 2021) [#PeereBS]_ and is the quickest method (it uses 3 pulses)
-
-        * The L3 sizing is a more general approach which is slower but more accurate (it uses 24 pulses/year)
-
-        * The L4 sizing is the most exact one, since it uses hourly data (8760 pulses/year)
-
-        Please note that the changes sizing setup changes here are not saved! Use self.setupSizing for this.
-
-        Parameters
-        ----------
-        H_init : float
-            Initial depth for the iteration. If None, the default H_init is chosen.
-        use_constant_Rb : bool
-            True if a constant borehole equivalent resistance (Rb*) value should be used
-        L2_sizing : bool
-            True if a sizing with the L2 method is needed
-        L3_sizing : bool
-            True if a sizing with the L3 method is needed
-        L4_sizing : bool
-            True if a sizing with the L4 method is needed
-        quadrant_sizing : int
-            Differs from 0 when a sizing in a certain quadrant is desired.
-            Quadrants are developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_
-        kwargs : dict
-            Dictionary with all the other options that can be set within GHEtool. For a complete list,
-            see the documentation in the CalculationSetup class.
-
-        Returns
-        -------
-        borehole depth : float
-
-        Raises
-        ------
-        ValueError
-            ValueError when no ground data is provided
-        """
-        # check ground data
-        if not self.ground_data.check_values():
-            raise ValueError("Please provide ground data.")
-
-        # make backup of initial parameter states
-        self._calculation_setup.make_backup()
-        use_constant_Rb_backup = self.borehole.use_constant_Rb
-
-        # run the sizing setup
-        self._calculation_setup.update_variables(H_init=H_init, L2_sizing=L2_sizing, L3_sizing=L3_sizing,
-                                                 L4_sizing=L4_sizing,
-                                                 quadrant_sizing=quadrant_sizing)
-        self._calculation_setup.update_variables(**kwargs)
-
-        if not use_constant_Rb is None:
-            self.borehole.use_constant_Rb = use_constant_Rb
-
-        # sizes according to the correct algorithm
-        if self._calculation_setup.L2_sizing:
-            depth = self.size_L2(H_init, self._calculation_setup.quadrant_sizing)
-        if self._calculation_setup.L3_sizing:
-            depth = self.size_L3(H_init, self._calculation_setup.quadrant_sizing)
-        if self._calculation_setup.L4_sizing:
-            depth = self.size_L4(H_init, self._calculation_setup.quadrant_sizing)
-
-        # reset initial parameters
-        self._calculation_setup.restore_backup()
-        self.borehole.use_constant_Rb = use_constant_Rb_backup
-
-        # check if the field is not shallow
-        if depth < self.THRESHOLD_WARNING_SHALLOW_FIELD:
-            ghe_logger.warning(f"The field has a calculated depth of {round(depth, 2)}"
-                               f"m which is lower than the proposed minimum "
-                               f"of {self.THRESHOLD_WARNING_SHALLOW_FIELD} m. "
-                               f"Please change your configuration accordingly to have a not so shallow field.")
-
-        ghe_logger.info("The borefield has been sized.")
-        return depth
-
-    def _select_size(self, size_max_temp: float, size_min_temp: float, hourly: bool = False) -> float:
-        """
-        This function selects the correct size based on a size for the minimum and maximum temperature.
-        When no temperature gradient is taken into account, this is just the maximum value of the two.
-        When there is a temperature gradient and the sizing for the minimum temperature is higher than the sizing
-        for the max temperature, it is checked if this sizing does not cross the maximum temperature limit.
-        If it does, an error is returned.
-
-        Parameters
-        ----------
-        size_max_temp : float
-            Sizing according to the quadrants limited by the maximum temperature [m]
-        size_min_temp : float
-            Sizing according to the quadrants limited by the minimum temperature [m]
-        hourly : bool
-            True if the sizing was hourly
-
-        Returns
-        -------
-        depth : float
-            Required borehole depth [m]
-
-        Raises
-        ------
-        UnsolvableDueToTemperatureGradient
-            Error when no solution can be found
-        """
-        # return the max of both sizes when no temperature gradient is used
-        if not self.ground_data.variable_Tg:
-            return max(size_max_temp, size_min_temp)
-
-        if size_max_temp > size_min_temp:
-            # no problem, since the field is already sized by the maximum temperature
-            return size_max_temp
-
-        # check if sizing by the minimum temperature (quadrant 3/4) does not cross the temperature boundary
-        self.calculate_temperatures(size_min_temp, hourly=hourly)
-        if np.max(self.results.peak_cooling) <= self.Tf_max:
-            return size_min_temp
-        raise UnsolvableDueToTemperatureGradient
-
-    def size_L2(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
-        """
-        This function sizes the  of the given configuration according to the methodology explained in
-        (Peere et al., 2021) [#PeereBS]_, which is a L2 method. When quadrant sizing is other than 0, it sizes the field based on
-        the asked quadrant. It returns the borefield depth.
-
-        Parameters
-        ----------
-        H_init : float
-            Initial depth from where to start the iteration [m]
-        quadrant_sizing : int
-            If a quadrant is given the sizing is performed for this quadrant else for the relevant
-
-        Returns
-        -------
-        H : float
-            Required depth of the borefield [m]
-
-        Raises
-        ------
-        ValueError
-            ValueError when no ground data is provided or quadrant is not in range.
-        """
-        # check ground data
-        if not self.ground_data.check_values():
-            raise ValueError("Please provide ground data.")
-        # check quadrants
-        if not quadrant_sizing in range(0, 5):
-            raise ValueError(f'Quadrant {quadrant_sizing} does not exist.')
-
-        # initiate with a given depth
-        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
-
-        def size_quadrant1():
-            th, _, tcm, qh, qpm, qm = self.load._calculate_first_year_params(False)  # calculate parameters
-            self.Tf = self.Tf_max
-            return self._Carcel(th, tcm, qh, qpm, qm)  # size
-
-        def size_quadrant2():
-            th, qh, qm, qa = self.load._calculate_last_year_params(False)  # calculate parameters
-            self.Tf = self.Tf_max
-            return self._Ahmadfard(th, qh, qm, qa)  # size
-
-        def size_quadrant3():
-            th, _, tcm, qh, qpm, qm = self.load._calculate_first_year_params(True)  # calculate parameters
-            self.Tf = self.Tf_min
-            return self._Carcel(th, tcm, qh, qpm, qm)  # size
-
-        def size_quadrant4():
-            th, qh, qm, qa = self.load._calculate_last_year_params(True)  # calculate parameters
-            self.Tf = self.Tf_min
-            return self._Ahmadfard(th, qh, qm, qa)  # size
-
-        if quadrant_sizing != 0:
-            # size according to a specific quadrant
-            if quadrant_sizing == 1:
-                self.H = size_quadrant1()
-            elif quadrant_sizing == 2:
-                self.H = size_quadrant2()
-            elif quadrant_sizing == 3:
-                self.H = size_quadrant3()
-            else:
-                self.H = size_quadrant4()
-            self.limiting_quadrant = quadrant_sizing
-        else:
-            # size according to the biggest quadrant
-            # determine which quadrants are relevant
-            if self.load.imbalance <= 0:
-                # extraction dominated, so quadrants 1 and 4 are relevant
-                if self.load.max_peak_cooling != 0:
-                    quadrant1 = size_quadrant1()
-                else:
-                    quadrant1 = 0
-                quadrant4 = size_quadrant4()
-
-                self.H = self._select_size(quadrant1, quadrant4)
-
-                if quadrant1 == self.H:
-                    self.limiting_quadrant = 1
-                else:
-                    self.limiting_quadrant = 4
-            else:
-                # injection dominated, so quadrants 2 and 3 are relevant
-                quadrant2 = size_quadrant2()
-                if self.load.max_peak_heating != 0:
-                    quadrant3 = size_quadrant3()
-                else:
-                    quadrant3 = 0
-
-                self.H = self._select_size(quadrant2, quadrant3)
-
-                if quadrant2 == self.H:
-                    self.limiting_quadrant = 2
-                else:
-                    self.limiting_quadrant = 3
-
-        return self.H
-
-    def size_L3(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
-        """
-        This function sizes the borefield based on a monthly (L3) method.
-
-        Parameters
-        ----------
-        H_init : float
-            Initial depth from where to start the iteration [m]
-        quadrant_sizing : int
-            If a quadrant is given the sizing is performed for this quadrant else for the relevant
-
-        Returns
-        -------
-        H : float
-            Required depth of the borefield [m]
-
-        Raises
-        ------
-         ValueError
-            ValueError when no ground data is provided or quadrant is not in range.
-        UnsolvableDueToTemperatureGradient
-            Error when the field cannot be sized.
-        """
-        # check ground data
-        if not self.ground_data.check_values():
-            raise ValueError("Please provide ground data.")
-        # check quadrants
-        if not quadrant_sizing in range(0, 5):
-            raise ValueError(f'Quadrant {quadrant_sizing} does not exist.')
-
-        # initiate with a given depth
-        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
-
-        if quadrant_sizing != 0:
-            # size according to a specific quadrant
-            self.H, _ = self._size_based_on_temperature_profile(quadrant_sizing)
-            return self.H
-        else:
-            try:
-                max_temp, sized = self._size_based_on_temperature_profile(10, deep_sizing=self._calculation_setup.force_deep_sizing)
-            except MaximumNumberOfIterations as e:
-                # no convergence with normal method, but perhaps with deep_sizing enabled
-                if self._calculation_setup.deep_sizing and self.ground_data.variable_Tg:
-                    max_temp, sized = self._size_based_on_temperature_profile(10, deep_sizing=True)
-                else:
-                    raise e
-            if sized:
-                # already correct size
-                self.H = max_temp
-                if self.load.imbalance <= 0:
-                    self.limiting_quadrant = 1
-                else:
-                    self.limiting_quadrant = 2
-                return max_temp
-            min_temp, sized = self._size_based_on_temperature_profile(20)
-            if sized:
-                self.H = min_temp
-                if self.load.imbalance <= 0:
-                    self.limiting_quadrant = 4
-                else:
-                    self.limiting_quadrant = 3
-                return min_temp
-            raise UnsolvableDueToTemperatureGradient
-
-    def size_L4(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
-        """
-        This function sizes the borefield based on an hourly (L4) sizing methodology.
-
-        Parameters
-        ----------
-        H_init : float
-            Initial depth from where to start the iteration [m]
-        quadrant_sizing : int
-            If a quadrant is given the sizing is performed for this quadrant else for the relevant
-
-        Returns
-        -------
-        H : float
-            Required depth of the borefield [m]
-
-        Raises
-        ------
-        ValueError
-           ValueError when no ground data is provided or quadrant is not in range.
-        UnsolvableDueToTemperatureGradient
-           When the field cannot be sized due to the temperature gradient.
-        """
-        # check ground data
-        if not self.ground_data.check_values():
-            raise ValueError("Please provide ground data.")
-        # check quadrants
-        if not quadrant_sizing in range(0, 5):
-            raise ValueError(f'Quadrant {quadrant_sizing} does not exist.')
-
-        # check if hourly data is given
-        if not self.load.hourly_resolution:
-            raise ValueError("There is no hourly resolution available!")
-
-        # initiate with a given depth
-        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
-
-        if quadrant_sizing != 0:
-            # size according to a specific quadrant
-            self.H, _ = self._size_based_on_temperature_profile(quadrant_sizing, hourly=True)
-            return self.H
-        else:
-            try:
-                max_temp, sized = self._size_based_on_temperature_profile(10, hourly=True, deep_sizing=self._calculation_setup.force_deep_sizing) if np.any(self.load.hourly_cooling_load) else (0, False)
-            except MaximumNumberOfIterations as e:
-                # no convergence with normal method, but perhaps with deep_sizing enabled
-                if self._calculation_setup.deep_sizing and self.ground_data.variable_Tg:
-                    max_temp, sized = self._size_based_on_temperature_profile(10, hourly=True, deep_sizing=True) if np.any(self.load.hourly_cooling_load) else (0, False)
-                else:
-                    raise e
-            if sized:
-                # already correct size
-                self.H = max_temp
-                if self.load.imbalance <= 0:
-                    self.limiting_quadrant = 1
-                else:
-                    self.limiting_quadrant = 2
-                return max_temp
-            min_temp, sized = self._size_based_on_temperature_profile(20, hourly=True) if np.any(self.load.hourly_heating_load) else (0, False)
-            if sized:
-                if self.load.imbalance <= 0:
-                    self.limiting_quadrant = 4
-                else:
-                    self.limiting_quadrant = 3
-                self.H = min_temp
-                return min_temp
-            raise UnsolvableDueToTemperatureGradient
-
-    def calculate_next_depth_deep_sizing(self, current_depth: float) -> float:
-        """
-        This method is a slower but more robust way of calculating the next depth in the sizing iteration when the
-        borefield is sized for the maximum fluid temperature when there is a non-constant ground temperature.
-        The method is based (as can be seen in its corresponding validation document) on the assumption that the
-        difference between the maximum temperature in peak cooling and the average undisturbed ground temperature
-        is irreversily proportional to the depth. In this way, given this difference in temperature and the current
-        depth, a new depth can be calculated.
-
-        Parameters
-        ----------
-        current_depth : float
-            The current depth of the borefield [m]
-
-        Returns
-        -------
-        float
-            New depth of the borefield [m]
-        """
-        # diff between the max temperature in peak cooling and the avg undisturbed ground temperature at current_depth
-        delta_temp = np.max(self.results.peak_cooling - self.ground_data.calculate_Tg(current_depth))
-
-        # calculate the maximum temperature difference between the temperature limit and the ground temperature
-        # at current_depth
-        delta_wrt_max = self.Tf_max - self.ground_data.calculate_Tg(current_depth)
-
-        # delta_t1/H1 ~ delta_t2/H2
-        # H2 = delta_t2/delta_t1*current_depth
-        rel_diff = delta_wrt_max/delta_temp
-        new_depth = current_depth/rel_diff
-
-        return new_depth
-
-    def _size_based_on_temperature_profile(self, quadrant: int, hourly: bool = False, deep_sizing: bool = False) -> (float, bool):
-        """
-        This function sizes based on the temperature profile.
-        It sizes for a specific quadrant and can both size with a monthly or an hourly resolution.
-
-        Parameters
-        ----------
-        quadrant : int
-            Differs from 0 when a sizing in a certain quadrant is desired.
-            Quadrants are developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_
-        hourly : bool
-            True if an hourly resolution should be used
-        deep_sizing : bool
-            True if the slower method should be used for the sizing, which is robuster.
-
-        Returns
-        -------
-        Depth : float
-            Required depth of the borefield [m]
-        Sized : bool
-            True if the required depth also satisfies the other temperature constraint [m]
-        """
-        # initiate iteration
-        H_prev = 0
-
-        if self.H < 1:
-            self.H = 50
-
-        # define loads for sizing
-        # it only calculates the first and the last year, so the sizing is less computationally expensive
-        # loads_short = self.load.hourly_cooling_load - self.load.hourly_heating_load if hourly else self.load.monthly_average_load
-        # loads_short_rev = loads_short[::-1]
-        # loads_long = np.tile(loads_short, 2)
-        #
-        # # initialise the results array
-        # results = np.zeros(loads_short.size * 2)
-
-        if deep_sizing:
-            # set borefield to minimal depth
-            self.H = 20
-
-        # Iterates as long as there is no convergence
-        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
-        i = 0
-        while not self._check_convergence(self.H, H_prev, i):
-
-            if hourly:
-                # # calculate g-values
-                # g_values = self.gfunction(self.load.time_L4, self.H)
-                #
-                # # calculation of needed differences of the g-function values. These are the weight factors
-                # # in the calculation of Tb.
-                # g_value_differences = np.diff(g_values, prepend=0)
-                #
-                # # convolution to get the monthly results
-                # results[:8760] = convolve(loads_short * 1000, g_value_differences[:8760])[:8760]
-                #
-                # g_sum_n1 = g_value_differences[:8760 * (self.simulation_period - 1)].reshape(self.simulation_period - 1,
-                #                                                                              8760).sum(axis=0)
-                # g_sum = g_sum_n1 + g_value_differences[8760 * (self.simulation_period - 1):]
-                # g_sum_n2 = np.concatenate((np.array([0]), g_sum_n1[::-1]))[:-1]
-                #
-                # results[8760:] = convolve(loads_short * 1000, g_sum)[:8760] + convolve(loads_short_rev * 1000,
-                #                                                                        g_sum_n2)[:8760][::-1]
-                #
-                # # calculation the borehole wall temperature for every month i
-                # Tb = results / (2 * pi * self.ground_data.k_s) / (self.H * self.number_of_boreholes) + self._Tg(self.H)
-                #
-                # self.Tb = Tb
-                # # now the Tf will be calculated based on
-                # # Tf = Tb + Q * R_b
-                # temperature_result = Tb + loads_long * 1000 * (self.Rb / self.number_of_boreholes / self.H)
-                # # reset other variables
-                # self.results.peak_heating = temperature_result
-                # self.results.peak_cooling = temperature_result
-                self._calculate_temperature_profile(self.H, hourly=True)
-
-            else:
-                # # calculate g-values
-                # g_values = self.gfunction(self.load.time_L3, self.H)
-                #
-                # # the g-function value of the peak with length_peak hours
-                # g_value_peak_cooling = self.gfunction(self.load.peak_cooling_duration, self.H)[0]
-                # if self.load.peak_cooling_duration == self.load.peak_heating_duration:
-                #     g_value_peak_heating = g_value_peak_cooling
-                # else:
-                #     g_value_peak_heating = self.gfunction(self.load.peak_heating_duration, self.H)[0]
-                #
-                # # calculation of needed differences of the g-function values. These are the weight factors in
-                # # the calculation of Tb.
-                # g_value_differences = np.diff(g_values, prepend=0)
-                #
-                # # convolution to get the monthly results
-                # results[:12] = convolve(loads_short * 1000, g_value_differences[:12])[:12]
-                #
-                # g_sum_n1 = g_value_differences[:12 * (self.load.simulation_period - 1)]\
-                #     .reshape(self.load.simulation_period - 1, 12).sum(axis=0)
-                # g_sum = g_sum_n1 + g_value_differences[12 * (self.load.simulation_period - 1):]
-                # g_sum_n2 = np.concatenate((np.array([0]), g_sum_n1[::-1]))[:-1]
-                #
-                # results[12:] = convolve(loads_short * 1000, g_sum)[:12]\
-                #                + convolve(loads_short_rev * 1000, g_sum_n2)[:12][::-1]
-                #
-                # # calculation the borehole wall temperature for every month i
-                # Tb = results / (2 * pi * self.ground_data.k_s) / (self.H * self.number_of_boreholes) + self._Tg(self.H)
-                #
-                # self.Tb = Tb
-                # # now the Tf will be calculated based on
-                # # Tf = Tb + Q * R_b
-                # results_month_cooling = Tb + np.tile(self.load.baseload_cooling_power, 2) * 1000 \
-                #                         * (self.Rb / self.number_of_boreholes / self.H)
-                # results_month_heating = Tb - np.tile(self.load.baseload_heating_power, 2) * 1000 \
-                #                         * (self.Rb / self.number_of_boreholes / self.H)
-                #
-                # # extra summation if the g-function value for the peak is included
-                # results_peak_cooling = results_month_cooling +\
-                #                        np.tile(self.load.peak_cooling - self.load.baseload_cooling_power, 2) * 1000 *\
-                #                        (g_value_peak_cooling / self.ground_data.k_s / 2 / pi + self.Rb) / self.number_of_boreholes / self.H
-                # results_peak_heating = results_month_heating - np.tile(self.load.peak_heating - self.load.baseload_heating_power, 2) * 1000 \
-                #                        * (g_value_peak_heating / self.ground_data.k_s / 2 / pi + self.Rb)\
-                #                        / self.number_of_boreholes / self.H
-                #
-                # # save temperatures under variable
-                # self.results.peak_heating = results_peak_heating
-                # self.results.peak_cooling = results_peak_cooling
-                self._calculate_temperature_profile(self.H, hourly=False)
-            H_prev = self.H
-            if not deep_sizing:
-                if quadrant == 1:
-                    # maximum temperature
-                    # convert back to required length
-                    self.H = (np.max(self.results.peak_cooling[:8760 if hourly else 12]) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
-                elif quadrant == 2:
-                    # maximum temperature
-                    # convert back to required length
-                    self.H = (np.max(self.results.peak_cooling[-8760 if hourly else -12:]) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
-                elif quadrant == 3:
-                    # minimum temperature
-                    # convert back to required length
-                    self.H = (np.min(self.results.peak_heating[:8760 if hourly else 12]) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
-                elif quadrant == 4:
-                    # minimum temperature
-                    # convert back to required length
-                    self.H = (np.min(self.results.peak_heating[-8760 if hourly else -12:]) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
-                elif quadrant == 10:
-                    # over all years
-                    # maximum temperature
-                    # convert back to required length
-                    self.H = (np.max(self.results.peak_cooling) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
-                elif quadrant == 20:
-                    # over all years
-                    # minimum temperature
-                    # convert back to required length
-                    self.H = (np.min(self.results.peak_heating) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
-            elif self.ground_data.variable_Tg:
-                # for when the temperature gradient is active and it is cooling
-                self.H = self.calculate_next_depth_deep_sizing(H_prev)
-            if self.H < 0:
-                return 0, False
-
-            i += 1
-
-        return self.H, (np.max(self.results.peak_cooling) <= self.Tf_max + 0.05 or
-                        (quadrant == 10 or quadrant == 1 or quadrant == 2))\
-                       and (np.min(self.results.peak_heating) >= self.Tf_min - 0.05 or
-                            (quadrant == 20 or quadrant == 3 or quadrant == 4))
-    @property
-    def investment_cost(self) -> float:
-        """
-        This function calculates the investment cost based on a cost profile linear to the total borehole length.
-
-        Returns
-        -------
-        float
-            Investment cost
-        """
-        return np.polyval(self.cost_investment, self.H * self.number_of_boreholes)
-
-    def calculate_temperatures(self, depth: float = None, hourly: bool = False) -> None:
-        """
-        Calculate all the temperatures without plotting the figure. When depth is given, it calculates it for a given
-        depth.
-
-        Parameters
-        ----------
-        depth : float
-            Depth for which the temperature profile should be calculated for [m]
-        hourly : bool
-            True when the temperatures should be calculated based on hourly data
-
-        Returns
-        -------
-        None
-        """
-        self._calculate_temperature_profile(H=depth, hourly=hourly)
-
-    def print_temperature_profile(self, legend: bool = True, plot_hourly: bool = False) -> None:
-        """
-        This function plots the temperature profile for the calculated depth.
-        It uses the available temperature profile data.
-
-        Parameters
-        ----------
-        legend : bool
-            True if the legend should be printed
-        plot_hourly : bool
-            True if the temperature profile printed should be based on the hourly load profile.
-
-        Returns
-        -------
-        fig, ax
-            Figure object
-        """
-        # calculate temperature profile
-        self._calculate_temperature_profile(hourly=plot_hourly)
-
-        return self._plot_temperature_profile(legend=legend, plot_hourly=plot_hourly)
-
-    def print_temperature_profile_fixed_depth(self, depth: float, legend: bool = True, plot_hourly: bool = False):
-        """
-        This function plots the temperature profile for a fixed depth.
-        It uses the already calculated temperature profile data, if available.
-
-        Parameters
-        ----------
-        depth : float
-            Depth at which the temperature profile should be shown
-        legend : bool
-            True if the legend should be printed
-        plot_hourly : bool
-            True if the temperature profile printed should be based on the hourly load profile.
-
-        Returns
-        -------
-        fig, ax
-            Figure object
-        """
-        # calculate temperature profile
-        self._calculate_temperature_profile(H=depth, hourly=plot_hourly)
-
-        return self._plot_temperature_profile(legend=legend, plot_hourly=plot_hourly)
-
-    def _plot_temperature_profile(self, legend: bool = True, plot_hourly: bool = False) -> Tuple[plt.Figure, plt.Axes]:
-        """
-        This function plots the temperature profile.
-
-        Parameters
-        ----------
-        legend : bool
-            True if the legend should be printed
-        plot_hourly : bool
-            True if the temperature profile printed should be based on the hourly load profile.
-
-        Returns
-        -------
-        fig, ax
-            Figure object
-        """
-
-        # make a time array
-        if plot_hourly:
-            time_array = self.load.time_L4 / 12 / 3600 / 730
-        else:
-            time_array = self.load.time_L3 / 12 / 730. / 3600.
-
-        # plt.rc('figure')
-        # create new figure and axes if it not already exits otherwise clear it.
-        fig = plt.figure()
-        ax = fig.add_subplot(111)
-        # set axes labelsv
-        ax.set_xlabel(r'Time (year)')
-        ax.set_ylabel(r'Temperature ($^\circ C$)')
-        ax.yaxis.label.set_color(plt.rcParams["axes.labelcolor"])
-        ax.xaxis.label.set_color(plt.rcParams["axes.labelcolor"])
-
-        # plot Temperatures
-        ax.step(time_array, self.results.Tb, 'k-', where="post", lw=1.5, label="Tb")
-
-        if plot_hourly:
-            ax.step(time_array, self.results.peak_cooling, 'b-', where="post", lw=1, label='Tf')
-        else:
-            ax.step(time_array, self.results.peak_cooling, 'b-', where="post", lw=1.5, label='Tf peak cooling')
-            ax.step(time_array, self.results.peak_heating, 'r-', where="post", lw=1.5, label='Tf peak heating')
-
-            ax.step(time_array, self.results.monthly_cooling, color='b', linestyle="dashed", where="post", lw=1.5,
-                    label='Tf base cooling')
-            ax.step(time_array, self.results.monthly_heating, color='r', linestyle="dashed", where="post", lw=1.5,
-                    label='Tf base heating')
-
-        # define temperature bounds
-        ax.hlines(self.Tf_min, 0, self.simulation_period, colors='r', linestyles='dashed', label='', lw=1)
-        ax.hlines(self.Tf_max, 0, self.simulation_period, colors='b', linestyles='dashed', label='', lw=1)
-        ax.set_xticks(range(0, self.simulation_period + 1, 2))
-
-        # Plot legend
-        if legend:
-            ax.legend()
-        ax.set_xlim(left=0, right=self.simulation_period)
-        plt.show()
-        return fig, ax
-
-    def _delete_calculated_temperatures(self) -> None:
-        """
-        This function deletes all the calculated temperatures.
-
-        Returns
-        -------
-        None
-        """
-        self.results = Results()
-        self._building_load = HourlyGeothermalLoad()
-        self._secundary_borefield_load = HourlyGeothermalLoad()
-        ghe_logger.info("Deleted all stored temperatures from previous calculations.")
-
-    def _calculate_temperature_profile(self, H: float = None, hourly: bool = False) -> None:
-        """
-        This function calculates the evolution in the fluid temperature and borehole wall temperature.
-
-        Parameters
-        ----------
-        H : float
-            Depth at which the temperatures should be evaluated [m]. If None, than the current depth is taken.
-        hourly : bool
-            True if the temperature evolution should be calculated on an hourly basis.
-
-        Returns
-        -------
-        None
-        """
-
-        # set Rb* value
-        Rb = self.borehole.get_Rb(H if H is not None else self.H, self.D, self.r_b, self.ground_data.k_s)
-        H = H if H is not None else self.H
-
-        if not hourly:
-            # self.g-function is a function that uses the precalculated data to interpolate the correct values of the
-            # g-function. This dataset is checked over and over again and is correct
-            g_values = self.gfunction(self.load.time_L3, H)
-
-            # the g-function value of the peak with length_peak hours
-            g_value_peak_cooling = self.gfunction(self.load.peak_cooling_duration, H)[0]
-            if self.load.peak_cooling_duration == self.load.peak_heating_duration:
-                g_value_peak_heating = g_value_peak_cooling
-            else:
-                g_value_peak_heating = self.gfunction(self.load.peak_heating_duration, H)[0]
-
-            # calculation of needed differences of the g-function values. These are the weight factors in the calculation
-            # of Tb.
-            g_value_differences = np.diff(g_values, prepend=0)
-
-            # convolution to get the monthly results
-            results = convolve(self.load.monthly_average_load_simulation_period * 1000,
-                               g_value_differences)[:12 * self.simulation_period]
-
-            # calculation the borehole wall temperature for every month i
-            Tb = results / (2 * pi * self.ground_data.k_s) / (H * self.number_of_boreholes) + self._Tg(H)
-
-            # now the Tf will be calculated based on
-            # Tf = Tb + Q * R_b
-            results_month_cooling = Tb + self.load.baseload_cooling_power_simulation_period * 1000 \
-                                    * (Rb / self.number_of_boreholes / H)
-            results_month_heating = Tb - self.load.baseload_heating_power_simulation_period * 1000 \
-                                    * (Rb / self.number_of_boreholes / H)
-
-            # extra summation if the g-function value for the peak is included
-            results_peak_cooling = results_month_cooling + (
-                    self.load.peak_cooling_simulation_period - self.load.baseload_cooling_power_simulation_period) * 1000 \
-                                   * (
-                                           g_value_peak_cooling / self.ground_data.k_s / 2 / pi + Rb) / self.number_of_boreholes / H
-            results_peak_heating = results_month_heating - (
-                    self.load.peak_heating_simulation_period - self.load.baseload_heating_power_simulation_period) * 1000 \
-                                   * (
-                                           g_value_peak_heating / self.ground_data.k_s / 2 / pi + Rb) / self.number_of_boreholes / H
-
-            # save temperatures under variable
-            self.results = Results(borehole_wall_temp=Tb,
-                                   peak_heating=results_peak_heating,
-                                   peak_cooling=results_peak_cooling,
-                                   monthly_heating=results_month_heating,
-                                   monthly_cooling=results_month_cooling)
-
-        if hourly:
-            # check for hourly data if this is requested
-            if not self.load.hourly_resolution:
-                raise ValueError("There is no hourly resolution available!")
-
-            hourly_load = self.load.hourly_load_simulation_period
-
-            # self.g-function is a function that uses the precalculated data to interpolate the correct values of the
-            # g-function. This dataset is checked over and over again and is correct
-            g_values = self.gfunction(self.load.time_L4, H)
-
-            # calculation of needed differences of the g-function values. These are the weight factors in the calculation
-            # of Tb.
-            g_value_differences = np.diff(g_values, prepend=0)
-
-            # convolution to get the monthly results
-            results = convolve(hourly_load * 1000, g_value_differences)[:len(hourly_load)]
-
-            # calculation the borehole wall temperature for every month i
-            Tb = results / (2 * pi * self.ground_data.k_s) / (H * self.number_of_boreholes) + self._Tg(H)
-
-            # now the Tf will be calculated based on
-            # Tf = Tb + Q * R_b
-            temperature_result = Tb + hourly_load * 1000 * (Rb / self.number_of_boreholes / H)
-
-            # reset other variables
-            self.results = Results(borehole_wall_temp=Tb,
-                                   peak_heating=temperature_result,
-                                   peak_cooling=temperature_result)
-
-    def set_options_gfunction_calculation(self, options: dict) -> None:
-        """
-        This function sets the options for the gfunction calculation of pygfunction.
-        This dictionary is directly passed through to the gFunction class of pygfunction.
-        For more information, please visit the documentation of pygfunction.
-
-        Parameters
-        ----------
-        options : dict
-            Dictionary with options for the gFunction class of pygfunction
-
-        Returns
-        -------
-        None
-        """
-        self.gfunction_calculation_object.set_options_gfunction_calculation(options)
-
-    def gfunction(self, time_value: list | float | np.ndarray, H: float = None) -> np.ndarray:
-        """
-        This function returns the gfunction value.
-        It can do so by either calculating the gfunctions just-in-time or by interpolating from a
-        loaded custom data file.
-
-        Parameters
-        ----------
-        time_value : list, float, np.ndarray
-            Time value(s) in seconds at which the gfunctions should be calculated
-        H : float
-            Depth [m] at which the gfunctions should be calculated.
-            If no depth is given, the current depth is taken.
-
-        Returns
-        -------
-        gvalue : np.ndarray
-            1D array with the g-values for all the requested time_value(s)
-        """
-        if H is None:
-            H = self.H
-        # when using a variable ground temperature, sometimes no solution can be found
-        if not isinstance(self.ground_data, GroundConstantTemperature) and H > Borefield.THRESHOLD_DEPTH_ERROR:
-            raise UnsolvableDueToTemperatureGradient
-
-        def jit_gfunction_calculation() -> np.ndarray:
-            """
-            This function calculates the gfunction just-in-time.
-
-            Returns
-            -------
-            gvalues : np.ndarray
-                1D array with the g-values for the requested time intervals
-            """
-            # set the correct depth of the borefield
-            self._update_borefield_depth(H=H)
-            return self.gfunction_calculation_object.calculate(time_value, self.borefield, self.ground_data.alpha,
-                                                               interpolate=self._calculation_setup.interpolate_gfunctions)
-
-        ## 1 bypass any possible precalculated g-functions
-        # if calculate is False, then the gfunctions are calculated jit
-        if not self._calculation_setup.use_precalculated_dataset:
-            return jit_gfunction_calculation()
-
-        ## 2 use precalculated g-functions when available
-        if self.custom_gfunction is not None:
-            # there is precalculated data available
-            # check if the requested values can be calculated using the custom_gfunction
-            if self.custom_gfunction.within_range(time_value, H):
-                return self.custom_gfunction.calculate_gfunction(time_value, H)
-
-        ## 3 calculate g-function jit
-        return jit_gfunction_calculation()
-
-    def create_custom_dataset(self, time_array: list | np.ndarray = None,
-                              depth_array: list | np.ndarray = None,
-                              options: dict = {}) -> None:
-        """
-        This function makes a datafile for a given custom borefield and sets it for the borefield object.
-        It automatically sets this datafile in the current borefield object so it can be used as a source for
-        the interpolation of g-values.
-
-        Parameters
-        ----------
-        time_array : list, np.array
-            Time values (in seconds) used for the calculation of the datafile
-        depth_array : list, np.array
-            List or arrays of depths for which the datafile should be created
-        options : dict
-            Options for the g-function calculation (check pygfunction.gfunction.gFunction() for more information)
-
-        Returns
-        -------
-        None
-
-        Raises
-        ------
-        ValueError
-            When no borefield or ground data is set
-        """
-
-        try:
-            self.borefield[0]
-        except TypeError:
-            raise ValueError("No borefield is set for which the gfunctions should be calculated")
-        try:
-            self.ground_data.alpha
-        except AttributeError:
-            raise ValueError("No ground data is set for which the gfunctions should be calculated")
-
-        self.custom_gfunction = CustomGFunction(time_array, depth_array, options)
-        self.custom_gfunction.create_custom_dataset(self.borefield, self.ground_data.alpha)
-
-    @property
-    def Re(self) -> float:
-        """
-        Reynolds number.
-
-        Returns
-        -------
-        float
-            Reynolds number
-        """
-        return self.borehole.Re
-
-    def optimise_load_profile(self, building_load: HourlyGeothermalLoad, depth: float = None, SCOP: float = 10 ** 6,
-                              SEER: float = 10 ** 6, print_results: bool = False, temperature_threshold: float = 0.05) -> None:
-        """
-        This function optimises the load based on the given borefield and the given hourly load.
-        (When the load is not geothermal, the SCOP and SEER are used to convert it to a geothermal load.)
-        It does so based on a load-duration curve. The temperatures of the borefield are calculated on a monthly
-        basis, even though we have hourly data, for an hourly calculation of the temperatures
-        would take a very long time.
-
-        Parameters
-        ----------
-        building_load : _LoadData
-            Load data used for the optimisation
-        depth : float
-            Depth of the boreholes in the borefield [m]
-        SCOP : float
-            SCOP of the geothermal system (needed to convert hourly building load to geothermal load)
-        SEER : float
-            SEER of the geothermal system (needed to convert hourly building load to geothermal load)
-        print_results : bool
-            True when the results of this optimisation are to be printed in the terminal
-        temperature_threshold : float
-            The maximum allowed temperature difference between the maximum and minimum fluid temperatures and their
-            respective limits. The lower this threshold, the longer the convergence will take.
-
-        Returns
-        -------
-        None
-
-        Raises
-        ------
-        ValueError
-            ValueError if no hourly load is given or the threshold is negative
-        """
-
-        ## Explain variables
-        # load --> primary, geothermal load
-        # _building_load --> secundary, building load
-        # _secundary_borefield_load --> secundary, geothermal load
-
-        # check if hourly load is given
-        if not building_load.hourly_resolution:
-            raise ValueError("No hourly load was given!")
-
-        # check if threshold is positive
-        if temperature_threshold < 0:
-            raise ValueError(f'The temperature threshold is {temperature_threshold}, but it cannot be below 0!')
-
-        # set depth
-        if depth is None:
-            depth = self.H
-
-        # since the depth does not change, the Rb* value is constant
-        # set to use a constant Rb* value but save the initial parameters
-        Rb_backup = self.borehole.Rb
-        use_constant_Rb_backup = self.borehole.use_constant_Rb
-        self.Rb = self.borehole.get_Rb(depth, self.D, self.r_b, self.ground_data.k_s)
-
-        # load hourly heating and cooling load and convert it to geothermal loads
-        primary_geothermal_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
-        primary_geothermal_load.set_hourly_cooling(building_load.hourly_cooling_load.copy() * (1 + 1 / SEER))
-        primary_geothermal_load.set_hourly_heating(building_load.hourly_heating_load.copy() * (1 - 1 / SCOP))
-
-        # set geothermal load
-        self.load = copy.deepcopy(primary_geothermal_load)
-
-        # set initial peak loads
-        init_peak_heating: float = self.load.max_peak_heating
-        init_peak_cooling: float = self.load.max_peak_cooling
-
-        # peak loads for iteration
-        peak_heat_load_geo: float = init_peak_heating
-        peak_cool_load_geo: float = init_peak_cooling
-
-        # set iteration criteria
-        cool_ok, heat_ok = False, False
-
-        while not cool_ok or not heat_ok:
-            # limit the primary geothermal heating and cooling load to peak_heat_load_geo and peak_cool_load_geo
-            self.load.set_hourly_cooling(np.minimum(peak_cool_load_geo, primary_geothermal_load.hourly_cooling_load))
-            self.load.set_hourly_heating(np.minimum(peak_heat_load_geo, primary_geothermal_load.hourly_heating_load))
-
-            # calculate temperature profile, just for the results
-            self.calculate_temperatures(depth=depth)
-
-            # deviation from minimum temperature
-            if abs(min(self.results.peak_heating) - self.Tf_min) > temperature_threshold:
-
-                # check if it goes below the threshold
-                if min(self.results.peak_heating) < self.Tf_min:
-                    peak_heat_load_geo = max(0.1,
-                                             peak_heat_load_geo - 1 * max(1, 10 * (self.Tf_min - min(self.results.peak_heating))))
-                else:
-                    peak_heat_load_geo = min(init_peak_heating, peak_heat_load_geo * 1.01)
-                    if peak_heat_load_geo == init_peak_heating:
-                        heat_ok = True
-            else:
-                heat_ok = True
-
-            # deviation from maximum temperature
-            if abs(np.max(self.results.peak_cooling) - self.Tf_max) > temperature_threshold:
-
-                # check if it goes above the threshold
-                if np.max(self.results.peak_cooling) > self.Tf_max:
-                    peak_cool_load_geo = max(0.1,
-                                             peak_cool_load_geo - 1 * max(1, 10 * (-self.Tf_max + np.max(self.results.peak_cooling))))
-                else:
-                    peak_cool_load_geo = min(init_peak_cooling, peak_cool_load_geo * 1.01)
-                    if peak_cool_load_geo == init_peak_cooling:
-                        cool_ok = True
-            else:
-                cool_ok = True
-
-        # calculate the resulting secundary hourly profile that can be put on the borefield
-        self._secundary_borefield_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
-        self._secundary_borefield_load.set_hourly_cooling(self.load.hourly_cooling_load / (1 + 1 / SEER))
-        self._secundary_borefield_load.set_hourly_heating(self.load.hourly_heating_load / (1 - 1 / SCOP))
-
-        # set building load
-        self._building_load = building_load
-
-        # calculate external load
-        self._external_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
-        self._external_load.set_hourly_heating(np.maximum(0, building_load.hourly_heating_load -
-                                                          self._secundary_borefield_load.hourly_heating_load))
-        self._external_load.set_hourly_cooling(np.maximum(0, building_load.hourly_cooling_load -
-                                                          self._secundary_borefield_load.hourly_cooling_load))
-
-        # restore the initial parameters
-        self.Rb = Rb_backup
-        self.borehole.use_constant_Rb = use_constant_Rb_backup
-
-        if print_results:
-            # print results
-            print("The peak load heating is: ", f'{self._secundary_borefield_load.max_peak_heating:.0f}',
-                  "kW, leading to",
-                  f'{np.sum(self._secundary_borefield_load.hourly_heating_load):.0f}', "kWh of heating.")
-            print("This is", f'{self._percentage_heating:.0f}',
-                  "% of the total heating load.")
-            print("Another", f'{np.sum(self._external_load.hourly_heating_load):.0f}',
-                  "kWh of heating should come from another source, with a peak of",
-                  f'{self._external_load.max_peak_heating:.0f}', "kW.")
-            print("------------------------------------------")
-            print("The peak load cooling is: ", f'{self._secundary_borefield_load.max_peak_cooling:.0f}',
-                  "kW, leading to",
-                  f'{np.sum(self._secundary_borefield_load.hourly_cooling_load):.0f}', "kWh of cooling.")
-            print("This is", f'{self._percentage_cooling:.0f}',
-                  "% of the total cooling load.")
-            print("Another", f'{np.sum(self._external_load.hourly_cooling_load):.0f}',
-                  "kWh of cooling should come from another source, with a peak of",
-                  f'{self._external_load.max_peak_cooling:.0f}', "kW.")
-
-            # plot results
-            self.print_temperature_profile_fixed_depth(depth=depth)
-
-    @property
-    def _percentage_heating(self) -> float:
-        """
-        This function returns the percentage of heating load that can be done geothermally.
-
-        Returns
-        -------
-        float
-            Percentage of heating load that can be done geothermally.
-        """
-        return np.sum(self._secundary_borefield_load.hourly_heating_load) / \
-            np.sum(self._building_load.hourly_heating_load) * 100
-
-    @property
-    def _percentage_cooling(self) -> float:
-        """
-        This function returns the percentage of cooling load that can be done geothermally.
-
-        Returns
-        -------
-        float
-            Percentage of cooling load that can be done geothermally.
-        """
-        return np.sum(self._secundary_borefield_load.hourly_cooling_load) / \
-            np.sum(self._building_load.hourly_cooling_load) * 100
-
-    def calculate_quadrant(self) -> int:
-        """
-        This function returns the borefield quadrant (as defined by Peere et al., 2021 [#PeereEtAl]_)
-        based on the calculated temperature profile.
-        If there is no limiting quadrant, None is returned.\n
-        Quadrant 1 is limited in the first year by the maximum temperature\n
-        Quadrant 2 is limited in the last year by the maximum temperature\n
-        Quadrant 3 is limited in the first year by the minimum temperature\n
-        Quadrant 4 is limited in the last year by the maximum temperature
-
-        Returns
-        ----------
-        quadrant : int
-            The quadrant which limits the borefield
-
-        References
-        ----------
-        .. [#PeereEtAl] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
-        """
-
-        # calculate temperatures if they are not calculated
-        if not np.any(self.results.peak_heating):
-            ghe_logger.warning('There are not yet temperatures calculated, hence there is no limiting quadrant.'
-                               'The temperature is calculated now, based on monthly values.')
-            self.calculate_temperatures()
-
-        # calculate max/min fluid temperatures
-        max_temp = np.max(self.results.peak_cooling)
-        min_temp = np.min(self.results.peak_heating)
-
-        # calculate temperature difference w.r.t. the limits
-        DT_max = - self.Tf_max + max_temp + 1000  # + 1000 to have no problems with negative temperatures
-        DT_min = self.Tf_min - min_temp + 1000
-
-        # if the temperature limit is not crossed, return None
-        if self.Tf_max - 0.1 > max_temp and self.Tf_min + 0.1 < min_temp:
-            return
-
-        # True if heating/extraction dominated
-        if self.load.imbalance < 0:
-            # either quadrant 1 or 4
-            if DT_min > DT_max:
-                # limited by minimum temperature
-                return 4
-            return 1
-
-        # quadrant 2 or 3
-        if DT_min > DT_max:
-            # limited by minimum temperature
-            return 3
-        return 2
-
-    def plot_load_duration(self, legend: bool = False) -> Tuple[plt.Figure, plt.Axes]:
-        """
-        This function makes a load-duration curve from the hourly values.
-
-        Parameters
-        ----------
-        legend : bool
-            True if the figure should have a legend
-
-        Returns
-        ----------
-        Tuple
-            plt.Figure, plt.Axes
-        """
-        # check if there are hourly values
-        if not self.load.hourly_resolution:
-            raise ValueError("There is no hourly resolution available!")
-
-        # sort heating and cooling load
-        heating = self.load.hourly_heating_load.copy()
-        heating[::-1].sort()
-
-        cooling = self.load.hourly_cooling_load.copy()
-        cooling.sort()
-        cooling = cooling * (-1)
-        # create new figure and axes if it not already exits otherwise clear it.
-        fig = plt.figure()
-        ax = fig.add_subplot(111)
-        # add sorted loads to plot
-        ax.step(np.arange(0, 8760, 1), heating, 'r-', label="Heating")
-        ax.step(np.arange(0, 8760, 1), cooling, 'b-', label="Cooling")
-        # create 0 line
-        ax.hlines(0, 0, 8759, color="black")
-        # add labels
-        ax.set_xlabel("Time [hours]")
-        ax.set_ylabel("Power [kW]")
-        # set x limits to 8760
-        ax.set_xlim(0, 8760)
-        # plot legend if wanted
-        if legend:
-            ax.legend()  #
-        plt.show()
-        return fig, ax
+"""
+This file contains all the code for the borefield calculations.
+"""
+from __future__ import annotations
+
+import copy
+import warnings
+from math import pi
+from pathlib import Path
+from typing import Tuple
+import logging
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pygfunction as gt
+
+from numpy.typing import ArrayLike
+from scipy.signal import convolve
+
+from GHEtool.VariableClasses import FluidData, Borehole, GroundConstantTemperature, Results
+from GHEtool.VariableClasses import CustomGFunction, load_custom_gfunction, GFunction, CalculationSetup
+from GHEtool.VariableClasses.LoadData import *
+from GHEtool.VariableClasses.LoadData import _LoadData
+from GHEtool.VariableClasses.PipeData import _PipeData
+from GHEtool.VariableClasses.BaseClass import BaseClass, UnsolvableDueToTemperatureGradient, MaximumNumberOfIterations
+from GHEtool.VariableClasses.GroundData._GroundData import _GroundData
+from GHEtool.logger.ghe_logger import ghe_logger
+
+
+class Borefield(BaseClass):
+    """Main borefield class"""
+
+    UPM: float = 730.0  # number of hours per month
+    THRESHOLD_BOREHOLE_DEPTH: float = 0.05  # threshold for iteration
+
+    # define default values
+    DEFAULT_INVESTMENT: list = [35, 0]  # 35 EUR/m
+    DEFAULT_LENGTH_PEAK: int = 6  # hours
+    THRESHOLD_DEPTH_ERROR: int = 10000  # m
+
+    HOURLY_LOAD_ARRAY: np.ndarray = np.arange(0, 8761, UPM).astype(np.uint32)
+
+    def __init__(
+        self,
+        peak_heating: ArrayLike = None,
+        peak_cooling: ArrayLike = None,
+        baseload_heating: ArrayLike = None,
+        baseload_cooling: ArrayLike = None,
+        borefield: list[gt.boreholes.Borehole] = None,
+        custom_gfunction: CustomGFunction = None,
+        load: _LoadData = None,
+    ):
+        """
+
+        Parameters
+        ----------
+        peak_heating : list, numpy array
+            Monthly peak heating values [kW]
+        peak_cooling : list, numpy array
+            Monthly peak cooling values [kW]
+        baseload_heating : list, numpy array
+            Monthly baseload heating values [kWh]
+        baseload_cooling : list, numpy array
+            Monthly baseload heating values [kWh]
+        borefield : pygfunction borehole/borefield object
+            Set the borefield for which the calculations will be carried out
+        custom_gfunction : CustomGFunction
+            Custom gfunction dataset
+
+        Examples
+        --------
+
+        monthly peak values [kW]
+
+        >>> peak_cooling = np.array([0., 0, 34., 69., 133., 187., 213., 240., 160., 37., 0., 0.])
+        >>> peak_heating = np.array([160., 142, 102., 55., 0., 0., 0., 0., 40.4, 85., 119., 136.])
+
+        annual heating and cooling load [kWh]
+
+        >>> annual_heating_load = 300 * 10 ** 3
+        >>> annual_cooling_load = 160 * 10 ** 3
+
+        percentage of annual load per month (15.5% for January ...)
+
+        >>> monthly_load_heating_percentage = np.array([0.155, 0.148, 0.125, .099, .064, 0., 0., 0., 0.061, 0.087, 0.117, 0.144])
+        >>> monthly_load_cooling_percentage = np.array([0.025, 0.05, 0.05, .05, .075, .1, .2, .2, .1, .075, .05, .025])
+
+        resulting load per month [kWh]
+
+        >>> monthly_load_heating = annual_heating_load * monthly_load_heating_percentage
+        >>> monthly_load_cooling = annual_cooling_load * monthly_load_cooling_percentage
+
+        create the borefield object
+
+        >>> borefield = Borefield()
+
+        set the load
+
+        >>> load = MonthlyGeothermalLoadAbsolute(monthly_load_heating, monthly_load_cooling, peak_heating, peak_cooling)
+        >>> borefield.load = load
+
+        """
+
+        # initiate vars
+        baseload_cooling: np.ndarray = np.zeros(12) if baseload_cooling is None else baseload_cooling
+        baseload_heating: np.ndarray = np.zeros(12) if baseload_heating is None else baseload_heating
+        peak_cooling: np.ndarray = np.zeros(12) if peak_cooling is None else peak_cooling
+        peak_heating: np.ndarray = np.zeros(12) if peak_heating is None else peak_heating
+
+        self.limiting_quadrant: int = 0  # parameter that tells in which quadrant the field is limited
+        # m hereafter one needs to chance to fewer boreholes with more depth, because the calculations are no longer
+        # that accurate.
+        self.THRESHOLD_WARNING_SHALLOW_FIELD: int = 50
+
+        self.custom_gfunction: CustomGFunction = custom_gfunction
+        self.gfunction_calculation_object: GFunction = GFunction()
+
+        ## params w.r.t. pygfunction
+        self.options_pygfunction: dict = {"method": "equivalent"}
+
+        # initialize variables for temperature plotting
+        self.results = Results()
+
+        # initiate ground parameters
+        self._H = 0.0  # borehole depth m
+        self._ground_data: _GroundData = GroundConstantTemperature()
+        self.D: float = 0.0  # buried depth of the borehole [m]
+        self.r_b: float = 0.0  # borehole radius [m]
+
+        # initiate fluid parameters
+        self.Tf_max: float = 16.0  # maximum temperature of the fluid
+        self.Tf_min: float = 0.0  # minimum temperature of the fluid
+
+        # initiale borehole
+        self.borehole = Borehole()
+
+        # initiate different sizing
+        self._calculation_setup: CalculationSetup = CalculationSetup()
+        self.calculation_setup()
+
+        # load on the geothermal borefield, used in calculations
+        self._borefield_load = MonthlyGeothermalLoadAbsolute()
+        # geothermal load, but converted to a secundary demand in optimise_load_profile
+        self._secundary_borefield_load: HourlyGeothermalLoad = HourlyGeothermalLoad()
+        # secundary load of the building, used in optimise_load_profile
+        self._building_load: HourlyGeothermalLoad = HourlyGeothermalLoad()
+
+        if load is not None:
+            self.load = load
+        else:
+            self.load = MonthlyGeothermalLoadAbsolute(baseload_heating, baseload_cooling, peak_heating, peak_cooling)
+
+        # set investment cost
+        self.cost_investment: list = Borefield.DEFAULT_INVESTMENT
+
+        # set a custom borefield
+        self.borefield = borefield
+
+        ghe_logger.main_info("Borefield object has been created.")
+
+    @staticmethod
+    def activate_logger() -> None:
+        """
+        This function activates the logging.
+
+        Returns
+        -------
+        None
+        """
+        ghe_logger.setLevel("MAIN_INFO")
+
+    @staticmethod
+    def deactivate_logger() -> None:
+        """
+        This function deactivates the logging.
+
+        Returns
+        -------
+        None
+        """
+        ghe_logger.setLevel(logging.INFO)
+
+    @property
+    def number_of_boreholes(self) -> int:
+        """
+        This returns the number of boreholes in the borefield attribute.
+
+        Returns
+        -------
+        int
+            Number of boreholes
+        """
+        return len(self.borefield) if self.borefield is not None else 0
+
+    @property
+    def H(self) -> float:
+        """
+        This function returns the borehole depth.
+
+        Returns
+        -------
+        float
+            Borehole depth [meters]
+        """
+        return self._H
+
+    @H.setter
+    def H(self, H: float) -> None:
+        """
+        This function sets the borehole depth.
+
+        Parameters
+        ----------
+        H : float
+            Borehole depth [meters]
+
+        Returns
+        -------
+        None
+        """
+        self._H = H
+        self._update_borefield_depth(H)
+
+    def set_borefield(self, borefield: list[gt.boreholes.Borehole] = None) -> None:
+        """
+        This function set the borefield object. When None is given, the borefield will be deleted.
+
+        Parameters
+        ----------
+        borefield : List[pygfunction.boreholes.Borehole]
+            Borefield created with the pygfunction package
+
+        Returns
+        -------
+        None
+        """
+        self.borefield = borefield
+
+    def create_rectangular_borefield(self, N_1: int, N_2: int, B_1: float, B_2: float, H: float, D: float = 1, r_b: float = 0.075):
+        """
+        This function creates a rectangular borefield.
+        It calls the pygfunction module in the background.
+        The documentation of this function is based on pygfunction.
+
+        Parameters
+        ----------
+        N_1 : int
+            Number of boreholes in the x direction
+        N_2 : int
+            Number of boreholes in the y direction
+        B_1 : int
+            Distance between adjacent boreholes in the x direction [m]
+        B_2 : int
+            Distance between adjacent boreholes in the y direction [m]
+        H : float
+            Borehole depth [m]
+        D : float
+            Borehole buried depth [m]
+        r_b : float
+            Borehole radius [m]
+
+        Returns
+        -------
+        pygfunction borefield object
+        """
+        borefield = gt.boreholes.rectangle_field(N_1, N_2, B_1, B_2, H, D, r_b)
+        self.set_borefield(borefield)
+
+        return borefield
+
+    def create_circular_borefield(self, N: int, R: float, H: float, D: float = 1, r_b: float = 0.075):
+        """
+        This function creates a circular borefield.
+        It calls the pygfunction module in the background.
+        The documentation of this function is based on pygfunction.
+
+        Parameters
+        ----------
+        N : int
+            Number of boreholes in the borefield
+        R : float
+            Distance of boreholes from the center of the field
+        H : float
+            Borehole depth [m]
+        D : float
+            Borehole buried depth [m]
+        r_b : float
+            Borehole radius [m]
+
+        Returns
+        -------
+        pygfunction borefield object
+        """
+        borefield = gt.boreholes.circle_field(N, R, H, D, r_b)
+        self.set_borefield(borefield)
+        return borefield
+
+    def create_U_shaped_borefield(self, N_1: int, N_2: int, B_1: float, B_2: float, H: float, D: float = 1, r_b: float = 0.075):
+        """
+        This function creates a U shaped borefield.
+        It calls the pygfunction module in the background.
+        The documentation of this function is based on pygfunction.
+
+        Parameters
+        ----------
+        N_1 : int
+            Number of boreholes in the x direction
+        N_2 : int
+            Number of boreholes in the y direction
+        B_1 : int
+            Distance between adjacent boreholes in the x direction [m]
+        B_2 : int
+            Distance between adjacent boreholes in the y direction [m]
+        H : float
+            Borehole depth [m]
+        D : float
+            Borehole buried depth [m]
+        r_b : float
+            Borehole radius [m]
+
+        Returns
+        -------
+        pygfunction borefield object
+        """
+        borefield = gt.boreholes.U_shaped_field(N_1, N_2, B_1, B_2, H, D, r_b)
+        self.set_borefield(borefield)
+        return borefield
+
+    def create_L_shaped_borefield(self, N_1: int, N_2: int, B_1: float, B_2: float, H: float, D: float = 1, r_b: float = 0.075):
+        """
+        This function creates a L shaped borefield.
+        It calls the pygfunction module in the background.
+        The documentation of this function is based on pygfunction.
+
+        Parameters
+        ----------
+        N_1 : int
+            Number of boreholes in the x direction
+        N_2 : int
+            Number of boreholes in the y direction
+        B_1 : int
+            Distance between adjacent boreholes in the x direction [m]
+        B_2 : int
+            Distance between adjacent boreholes in the y direction [m]
+        H : float
+            Borehole depth [m]
+        D : float
+            Borehole buried depth [m]
+        r_b : float
+            Borehole radius [m]
+
+        Returns
+        -------
+        pygfunction borefield object
+        """
+        borefield = gt.boreholes.L_shaped_field(N_1, N_2, B_1, B_2, H, D, r_b)
+        self.set_borefield(borefield)
+        return borefield
+
+    def create_box_shaped_borefield(self, N_1: int, N_2: int, B_1: float, B_2: float, H: float, D: float = 1, r_b: float = 0.075):
+        """
+        This function creates a box shaped borefield.
+        It calls the pygfunction module in the background.
+        The documentation of this function is based on pygfunction.
+
+        Parameters
+        ----------
+        N_1 : int
+            Number of boreholes in the x direction
+        N_2 : int
+            Number of boreholes in the y direction
+        B_1 : int
+            Distance between adjacent boreholes in the x direction [m]
+        B_2 : int
+            Distance between adjacent boreholes in the y direction [m]
+        H : float
+            Borehole depth [m]
+        D : float
+            Borehole buried depth [m]
+        r_b : float
+            Borehole radius [m]
+
+        Returns
+        -------
+        pygfunction borefield object
+        """
+        borefield = gt.boreholes.box_shaped_field(N_1, N_2, B_1, B_2, H, D, r_b)
+        self.set_borefield(borefield)
+        return borefield
+
+    @property
+    def borefield(self):
+        """
+        Returns the hidden _borefield variable.
+
+        Returns
+        -------
+        Hidden _borefield object
+        """
+        return self._borefield
+
+    @borefield.setter
+    def borefield(self, borefield: list[gt.boreholes.Borehole] = None) -> None:
+        """
+        This function sets the borefield configuration. When no input is given, the borefield variable will be deleted.
+
+        Parameters
+        ----------
+        borefield : List[pygfunction.boreholes.Borehole]
+            Borefield created with the pygfunction package
+
+        Returns
+        -------
+        None
+        """
+        if borefield is None:
+            del self.borefield
+            return
+        self._borefield = borefield
+        self.D = np.average([bor.D for bor in borefield])
+        self.r_b = np.average([bor.r_b for bor in borefield])
+        self._H = np.average([bor.H for bor in borefield])
+        self.gfunction_calculation_object.remove_previous_data()
+        unequal_depth = np.any([bor.H != borefield[0].H for bor in borefield])
+        if unequal_depth:
+            self.gfunction_calculation_object._store_previous_values = not unequal_depth
+        else:
+            self.gfunction_calculation_object.store_previous_values = \
+                self.gfunction_calculation_object._store_previous_values_backup
+
+    @borefield.deleter
+    def borefield(self):
+        """
+        This function deletes the hidden _borefield object.
+        It also sets the number of boreholes to zero
+
+        Returns
+        -------
+        None
+        """
+        self._borefield = None
+        self.gfunction_calculation_object.remove_previous_data()
+        self.custom_gfunction = None
+
+    def _update_borefield_depth(self, H: float) -> None:
+        """
+        This function updates the borehole depth.
+
+        Parameters
+        ----------
+        H : float
+            Borehole depth.
+
+        Returns
+        -------
+        None
+        """
+        for bor in self._borefield:
+            bor.H = H
+
+        # the boreholes are equal in length
+        self.gfunction_calculation_object.store_previous_values = \
+            self.gfunction_calculation_object._store_previous_values_backup
+
+    def load_custom_gfunction(self, location: str) -> None:
+        """
+        This function loads the custom gfunction.
+
+        Parameters
+        ----------
+        location : str
+            Path to the location of the custom gfunction file
+
+        Returns
+        -------
+        None
+        """
+
+        self.custom_gfunction = load_custom_gfunction(location)
+        ghe_logger.main_info("Custom g-function has been loaded.")
+
+    def set_investment_cost(self, investment_cost: list = None) -> None:
+        """
+        This function sets the investment cost. This is linear with respect to the total field length.
+        If None, the default is set.
+
+        Parameters
+        ----------
+        investment_cost : list
+            1D array of polynomial coefficients (including coefficients equal to zero) from highest degree to the constant term
+
+        Returns
+        -------
+        None
+        """
+        if investment_cost is None:
+            investment_cost = Borefield.DEFAULT_INVESTMENT
+        self.cost_investment: list = investment_cost
+
+    def set_load(self, load: _LoadData) -> None:
+        """
+        This function sets the _load attribute.
+
+        Parameters
+        ----------
+        load : _LoadData
+            Load data object
+
+        Returns
+        -------
+        None
+        """
+        self.load = load
+
+    @property
+    def load(self) -> _LoadData | HourlyGeothermalLoad | MonthlyGeothermalLoadAbsolute:
+        """
+        This returns the LoadData object.
+
+        Returns
+        -------
+        Load data: LoadData
+        """
+        return self._borefield_load
+
+    @load.setter
+    def load(self, load: _LoadData) -> None:
+        """
+        This function sets the _load attribute.
+
+        Parameters
+        ----------
+        load : _LoadData
+            Load data object
+
+        Returns
+        -------
+        None
+        """
+        self._borefield_load = load
+        self._delete_calculated_temperatures()
+
+    @property
+    def simulation_period(self) -> int:
+        """
+        This returns the simulation period from the LoadData object.
+
+        Returns
+        -------
+        Simulation period [years] : int
+        """
+        return self.load.simulation_period
+
+    @simulation_period.setter
+    def simulation_period(self, simulation_period: float) -> None:
+        """
+        This function sets the simulation period.
+
+        Parameters
+        ----------
+        simulation_period : float
+            Simulation period in years
+
+        Returns
+        -------
+        None
+        """
+        self._borefield_load.simulation_period = simulation_period
+
+    @property
+    def Rb(self) -> float:
+        """
+        This function returns the equivalent borehole thermal resistance.
+
+        Returns
+        -------
+        Rb : float
+            Equivalent borehole thermal resistance [mK/W]
+        """
+        return self.borehole.get_Rb(self.H, self.D, self.r_b, self.ground_data.k_s)
+
+    @Rb.setter
+    def Rb(self, Rb: float) -> None:
+        """
+        This function sets the constant equivalent borehole thermal resistance.
+
+        Parameters
+        ----------
+        Rb : float
+            Equivalent borehole thermal resistance [mk/W]
+
+        Returns
+        -------
+        None
+        """
+        self.set_Rb(Rb)
+
+    @property
+    def ground_data(self) -> _GroundData:
+        """
+        This function returns the ground data.
+
+        Returns
+        -------
+        ground data : GroundData
+
+        """
+        return self._ground_data
+
+    @ground_data.setter
+    def ground_data(self, data: _GroundData) -> None:
+        """
+        This function sets the relevant ground parameters.
+
+        Parameters
+        ----------
+        data : GroundData
+            All the relevant ground data
+
+        Returns
+        -------
+        None
+        """
+        # Ground properties
+        self._ground_data = data
+
+        # new ground data implies that a new g-function should be loaded
+        self.custom_gfunction = None
+
+        # the stored gfunction data should be deleted
+        self.gfunction_calculation_object.remove_previous_data()
+
+    def set_ground_parameters(self, data: _GroundData) -> None:
+        """
+        This function sets the relevant ground parameters.
+
+        Parameters
+        ----------
+        data : GroundData
+            All the relevant ground data
+
+        Returns
+        -------
+        None
+        """
+
+        # Ground properties
+        self.ground_data = data
+
+    def set_fluid_parameters(self, data: FluidData) -> None:
+        """
+        This function sets the fluid parameters.
+
+        Parameters
+        ----------
+        data : FluidData
+            All the relevant fluid data
+
+        Returns
+        -------
+        None
+        """
+        self.borehole.fluid_data = data
+
+    def set_pipe_parameters(self, data: _PipeData) -> None:
+        """
+        This function sets the pipe parameters.
+
+        Parameters
+        ----------
+        data : PipeData
+            All the relevant pipe parameters
+
+        Returns
+        -------
+        None
+        """
+        self.borehole.pipe_data = data
+
+    def set_Rb(self, Rb: float) -> None:
+        """
+        This function sets the constant equivalent borehole thermal resistance.
+
+        Parameters
+        ----------
+        Rb : float
+            Equivalent borehole thermal resistance (mK/W)
+
+        Returns
+        -------
+        None
+        """
+        self.borehole.Rb = Rb
+
+    def set_max_avg_fluid_temperature(self, temp: float) -> None:
+        """
+        This functions sets the maximal average fluid temperature to temp.
+
+        Parameters
+        ----------
+        temp : float
+            Maximal average fluid temperature [deg C]
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            When the maximal average fluid temperature is lower than the minimal average fluid temperature
+        """
+        if temp <= self.Tf_min:
+            raise ValueError(f"The maximum average fluid temperature {temp} is lower than the minimum average fluid temperature {self.Tf_min}")
+        self.Tf_max: float = temp
+
+    def set_min_avg_fluid_temperature(self, temp: float) -> None:
+        """
+        This functions sets the minimal average fluid temperature to temp.
+
+        Parameters
+        ----------
+        temp : float
+            Minimal average fluid temperature [deg C]
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            When the maximal average temperature is lower than the minimal average temperature
+        """
+        if temp >= self.Tf_max:
+            raise ValueError(f"The minimum average fluid temperature {temp} is lower than the maximum average fluid temperature {self.Tf_max}")
+        self.Tf_min: float = temp
+
+    def _Tg(self, H: float = None) -> float:
+        """
+        This function gives back the ground temperature.
+
+        Parameters
+        ----------
+        H : float
+            Depth of the field at which the temperature is to be evaluated
+
+        Returns
+        -------
+        Temperature of the ground : float
+        """
+        # check if specific depth is given
+        if H is None:
+            H = self.H
+
+        return self.ground_data.calculate_Tg(H)
+
+    def _check_convergence(self, new_depth: float, old_depth: float, iter: int) -> bool:
+        """
+        This function checks, with the absolute and relative tolerance, if the depth is converged.
+        This is the case if both criteria are met. Raises MaximumNumberOfIterations error if the max number of iterations is crossed.
+
+        Parameters
+        ----------
+        new_depth : float
+            Depth from the current interation [m]
+        old_depth : float
+            Depth from the previous iteration [m]
+        iter : int
+            Current number of iteration
+
+        Returns
+        -------
+        bool
+            True if the depth is converged
+
+        Raises
+        ------
+        MaximumNumberOfIterations
+            MaximumNumberOfIterations if the max number of iterations is crossed
+        """
+        if iter + 1 > self._calculation_setup.max_nb_of_iterations:
+            raise MaximumNumberOfIterations(self._calculation_setup.max_nb_of_iterations)
+
+        if old_depth == 0:
+            return False
+        test_a_tol = abs(new_depth - old_depth) <= self._calculation_setup.atol if self._calculation_setup.atol != False else True
+        test_rtol = abs(new_depth - old_depth) / old_depth <= self._calculation_setup.rtol if self._calculation_setup.rtol != False else True
+
+        return test_a_tol and test_rtol
+
+    def _Ahmadfard(self, th: float, qh: float, qm: float, qa: float, Tf: float) -> float:
+        """
+        This function sizes the field based on the last year of operation, i.e. quadrants 2 and 4.
+
+        It uses the methodology developed by (Ahmadfard and Bernier, 2019) [#Ahmadfard2019]_.
+        The concept of borefield quadrants is developed by (Peere et al., 2020) [#PeereBS]_ [#PeereThesis]_.
+
+        Parameters
+        ----------
+        th : float
+            Peak duration [s]
+        qh : float
+            Peak load [W]
+        qm : float
+            Monthly average load [W]
+        qa : float
+            Yearly imbalance load [W]
+        Tf : float
+            Temperature limit of the fluid [°C]
+
+        Returns
+        -------
+        H : float
+            Required borehole depth [m]
+
+        References
+        ----------
+        .. [#Ahmadfard2019] Ahmadfard M. and Bernier M., A review of vertical ground heat exchanger sizing tools including an inter-model comparison,
+        Renewable and Sustainable Energy Reviews, Volume 110, 2019, Pages 247-265, ISSN 1364-0321, https://doi.org/10.1016/j.rser.2019.04.045
+        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
+        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
+        """
+        # initiate iteration
+        H_prev = 0
+        # set minimal depth to 50 m
+        self.H = 50 if self.H < 1 else self.H
+
+        time = np.array([th, th + self.load.tm, self.load.ty + self.load.tm + th])
+        # Iterates as long as there is no convergence
+        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
+        i = 0
+        while not self._check_convergence(self.H, H_prev, i):
+            # calculate the required g-function values
+            gfunct_uniform_T = self.gfunction(time, max(1, self.H))
+            # calculate the thermal resistances
+            k_s = self.ground_data.k_s(self.H)
+            Ra = (gfunct_uniform_T[2] - gfunct_uniform_T[1]) / (2 * pi * k_s)
+            Rm = (gfunct_uniform_T[1] - gfunct_uniform_T[0]) / (2 * pi * k_s)
+            Rd = (gfunct_uniform_T[0]) / (2 * pi * k_s)
+            # calculate the total borehole length
+            L = (qa * Ra + qm * Rm + qh * Rd + qh * self.Rb) / abs(Tf - self._Tg())
+            # updating the depth values
+            H_prev = self.H
+            self.H = L / self.number_of_boreholes
+            i += 1
+
+        return self.H
+
+    def _Carcel(self, th: float, tcm: float, qh: float, qpm: float, qm: float, Tf: float) -> float:
+        """
+        This function sizes the field based on the first year of operation, i.e. quadrants 1 and 3.
+
+        It uses the methodology developed by (Monzo et al., 2016) [#Monzo]_ and adapted by (Peere et al., 2021) [#PeereBS]_.
+        The concept of borefield quadrants is developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_.
+
+                Parameters
+        ----------
+        th : float
+            Peak duration [s]
+        tcm : float
+            Duration of the current month [s]
+        qp : float
+            Peak load [W]
+        qpm : float
+            Average load of the past months [W]
+        qm : float
+            Monthly average load [W]
+        Tf :float
+            Temperature limit of the fluid [°C]
+
+        Returns
+        -------
+        H : float
+            Required borehole depth [m]
+
+        References
+        ----------
+        .. [#Monzo] Monzo, P., M. Bernier, J. Acuna, and P. Mogensen. (2016). A monthly based bore field sizing methodology with applications to optimum borehole spacing. ASHRAE Transactions 122, 111–126.
+        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
+        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
+        """
+
+        # initiate iteration
+        H_prev = 0
+        time_steps = [th, th + self.load.tm, tcm + th]
+        if self.H < 1:
+            self.H = 50
+
+        # Iterates as long as there is no convergence
+        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
+        i = 0
+        while not self._check_convergence(self.H, H_prev, i):
+            # get the g-function values
+            gfunc_uniform_T = self.gfunction(time_steps, max(1, self.H))
+
+            # calculate the thermal resistances
+            k_s = self.ground_data.k_s(self.H)
+            Rpm = (gfunc_uniform_T[2] - gfunc_uniform_T[1]) / (2 * pi * k_s)
+            Rcm = (gfunc_uniform_T[1] - gfunc_uniform_T[0]) / (2 * pi * k_s)
+            Rh = (gfunc_uniform_T[0]) / (2 * pi * k_s)
+
+            # calculate the total length
+            L = (qh * self.Rb + qh * Rh + qm * Rcm + qpm * Rpm) / abs(Tf - self._Tg())
+
+            # updating the depth values
+            H_prev = self.H
+            self.H = L / self.number_of_boreholes
+            i += 1
+        return self.H
+
+    def calculation_setup(self, calculation_setup: CalculationSetup = None, use_constant_Rb: bool = None, **kwargs) -> None:
+        """
+        This function sets the options for the sizing function.
+
+        * The L2 sizing is the one explained in (Peere et al., 2021) [#PeereBS]_ and is the quickest method (it uses 3 pulses)
+
+        * The L3 sizing is a more general approach which is slower but more accurate (it uses 24 pulses/year)
+
+        * The L4 sizing is the most exact one, since it uses hourly data (8760 pulses/year)
+
+        Parameters
+        ----------
+        calculation_setup : CalculationSetup
+            An instance of the CalculationSetup class. When this argument differs from None, all the other parameters are
+            set based on this calculation_setup
+        use_constant_Rb : bool
+            True if a constant borehole equivalent resistance (Rb*) value should be used
+        kwargs
+            Dictionary with all the other options that can be set within GHEtool. For a complete list,
+            see the documentation in the CalculationSetup class.
+
+        Returns
+        -------
+        None
+
+        References
+        ----------
+        .. [#PeereBS] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
+        .. [#PeereThesis] Peere, W. (2020) Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
+        """
+
+        # if calculation_setup is not None, then the sizing setup is set directly
+        if calculation_setup is not None:
+            self._calculation_setup = calculation_setup
+            return
+
+        self._calculation_setup.update_variables(**kwargs)
+
+        if not use_constant_Rb is None:
+            self.borehole.use_constant_Rb = use_constant_Rb
+
+    def size(self,H_init: float = None,
+        use_constant_Rb: bool = None,
+        L2_sizing: bool = None,
+        L3_sizing: bool = None,
+        L4_sizing: bool = None,
+        quadrant_sizing: int = None,
+        **kwargs,
+    ) -> float:
+        """
+        This function sets the options for the sizing function.
+
+        * The L2 sizing is the one explained in (Peere et al., 2021) [#PeereBS]_ and is the quickest method (it uses 3 pulses)
+
+        * The L3 sizing is a more general approach which is slower but more accurate (it uses 24 pulses/year)
+
+        * The L4 sizing is the most exact one, since it uses hourly data (8760 pulses/year)
+
+        Please note that the changes sizing setup changes here are not saved! Use self.setupSizing for this.
+
+        Parameters
+        ----------
+        H_init : float
+            Initial depth for the iteration. If None, the default H_init is chosen.
+        use_constant_Rb : bool
+            True if a constant borehole equivalent resistance (Rb*) value should be used
+        L2_sizing : bool
+            True if a sizing with the L2 method is needed
+        L3_sizing : bool
+            True if a sizing with the L3 method is needed
+        L4_sizing : bool
+            True if a sizing with the L4 method is needed
+        quadrant_sizing : int
+            Differs from 0 when a sizing in a certain quadrant is desired.
+            Quadrants are developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_
+        kwargs : dict
+            Dictionary with all the other options that can be set within GHEtool. For a complete list,
+            see the documentation in the CalculationSetup class.
+
+        Returns
+        -------
+        borehole depth : float
+
+        Raises
+        ------
+        ValueError
+            ValueError when no ground data is provided
+        """
+        # check ground data
+        if not self.ground_data.check_values():
+            raise ValueError("Please provide ground data.")
+
+        # make backup of initial parameter states
+        self._calculation_setup.make_backup()
+        use_constant_Rb_backup = self.borehole.use_constant_Rb
+
+        # run the sizing setup
+        self._calculation_setup.update_variables(H_init=H_init, L2_sizing=L2_sizing, L3_sizing=L3_sizing, L4_sizing=L4_sizing, quadrant_sizing=quadrant_sizing)
+        self._calculation_setup.update_variables(**kwargs)
+
+        if not use_constant_Rb is None:
+            self.borehole.use_constant_Rb = use_constant_Rb
+
+        # sizes according to the correct algorithm
+        if self._calculation_setup.L2_sizing:
+            depth = self.size_L2(H_init, self._calculation_setup.quadrant_sizing)
+        if self._calculation_setup.L3_sizing:
+            depth = self.size_L3(H_init, self._calculation_setup.quadrant_sizing)
+        if self._calculation_setup.L4_sizing:
+            depth = self.size_L4(H_init, self._calculation_setup.quadrant_sizing)
+
+        # reset initial parameters
+        self._calculation_setup.restore_backup()
+        self.borehole.use_constant_Rb = use_constant_Rb_backup
+
+        # check if the field is not shallow
+        if depth < self.THRESHOLD_WARNING_SHALLOW_FIELD:
+            ghe_logger.warning(
+                f"The field has a calculated depth of {round(depth, 2)}"
+                f"m which is lower than the proposed minimum "
+                f"of {self.THRESHOLD_WARNING_SHALLOW_FIELD} m. "
+                f"Please change your configuration accordingly to have a not so shallow field."
+            )
+
+        ghe_logger.info("The borefield has been sized.")
+        return depth
+
+    def _select_size(self, size_max_temp: float, size_min_temp: float, hourly: bool = False) -> float:
+        """
+        This function selects the correct size based on a size for the minimum and maximum temperature.
+        When no temperature gradient is taken into account, this is just the maximum value of the two.
+        When there is a temperature gradient and the sizing for the minimum temperature is higher than the sizing
+        for the max temperature, it is checked if this sizing does not cross the maximum temperature limit.
+        If it does, an error is returned.
+
+        Parameters
+        ----------
+        size_max_temp : float
+            Sizing according to the quadrants limited by the maximum temperature [m]
+        size_min_temp : float
+            Sizing according to the quadrants limited by the minimum temperature [m]
+        hourly : bool
+            True if the sizing was hourly
+
+        Returns
+        -------
+        depth : float
+            Required borehole depth [m]
+
+        Raises
+        ------
+        UnsolvableDueToTemperatureGradient
+            Error when no solution can be found
+        """
+        # return the max of both sizes when no temperature gradient is used
+        if not self.ground_data.variable_Tg:
+            return max(size_max_temp, size_min_temp)
+
+        if size_max_temp > size_min_temp:
+            # no problem, since the field is already sized by the maximum temperature
+            return size_max_temp
+
+        # check if sizing by the minimum temperature (quadrant 3/4) does not cross the temperature boundary
+        self.calculate_temperatures(size_min_temp, hourly=hourly)
+        if np.max(self.results.peak_cooling) <= self.Tf_max:
+            return size_min_temp
+        raise UnsolvableDueToTemperatureGradient
+
+    def size_L2(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
+        """
+        This function sizes the  of the given configuration according to the methodology explained in
+        (Peere et al., 2021) [#PeereBS]_, which is a L2 method. When quadrant sizing is other than 0, it sizes the field based on
+        the asked quadrant. It returns the borefield depth.
+
+        Parameters
+        ----------
+        H_init : float
+            Initial depth from where to start the iteration [m]
+        quadrant_sizing : int
+            If a quadrant is given the sizing is performed for this quadrant else for the relevant
+
+        Returns
+        -------
+        H : float
+            Required depth of the borefield [m]
+
+        Raises
+        ------
+        ValueError
+            ValueError when no ground data is provided or quadrant is not in range.
+        """
+        # check ground data
+        if not self.ground_data.check_values():
+            raise ValueError("Please provide ground data.")
+        # check quadrants
+        if not quadrant_sizing in range(0, 5):
+            raise ValueError(f"Quadrant {quadrant_sizing} does not exist.")
+
+        # initiate with a given depth
+        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
+
+        def size_quadrant1():
+            th, _, tcm, qh, qpm, qm = self.load._calculate_first_year_params(False)  # calculate parameters
+            return self._Carcel(th, tcm, qh, qpm, qm, self.Tf_max)  # size
+
+        def size_quadrant2():
+            th, qh, qm, qa = self.load._calculate_last_year_params(False)  # calculate parameters
+            return self._Ahmadfard(th, qh, qm, qa, self.Tf_max)  # size
+
+        def size_quadrant3():
+            th, _, tcm, qh, qpm, qm = self.load._calculate_first_year_params(True)  # calculate parameters
+            return self._Carcel(th, tcm, qh, qpm, qm, self.Tf_min)  # size
+
+        def size_quadrant4():
+            th, qh, qm, qa = self.load._calculate_last_year_params(True)  # calculate parameters
+            return self._Ahmadfard(th, qh, qm, qa, self.Tf_min)  # size
+
+        if quadrant_sizing != 0:
+            # size according to a specific quadrant
+            if quadrant_sizing == 1:
+                self.H = size_quadrant1()
+            elif quadrant_sizing == 2:
+                self.H = size_quadrant2()
+            elif quadrant_sizing == 3:
+                self.H = size_quadrant3()
+            else:
+                self.H = size_quadrant4()
+            self.limiting_quadrant = quadrant_sizing
+        else:
+            # size according to the biggest quadrant
+            # determine which quadrants are relevant
+            if self.load.imbalance <= 0:
+                # extraction dominated, so quadrants 1 and 4 are relevant
+                if self.load.max_peak_cooling != 0:
+                    quadrant1 = size_quadrant1()
+                else:
+                    quadrant1 = 0
+                quadrant4 = size_quadrant4()
+
+                self.H = self._select_size(quadrant1, quadrant4)
+
+                if quadrant1 == self.H:
+                    self.limiting_quadrant = 1
+                else:
+                    self.limiting_quadrant = 4
+            else:
+                # injection dominated, so quadrants 2 and 3 are relevant
+                quadrant2 = size_quadrant2()
+                if self.load.max_peak_heating != 0:
+                    quadrant3 = size_quadrant3()
+                else:
+                    quadrant3 = 0
+
+                self.H = self._select_size(quadrant2, quadrant3)
+
+                if quadrant2 == self.H:
+                    self.limiting_quadrant = 2
+                else:
+                    self.limiting_quadrant = 3
+
+        return self.H
+
+    def size_L3(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
+        """
+        This function sizes the borefield based on a monthly (L3) method.
+
+        Parameters
+        ----------
+        H_init : float
+            Initial depth from where to start the iteration [m]
+        quadrant_sizing : int
+            If a quadrant is given the sizing is performed for this quadrant else for the relevant
+
+        Returns
+        -------
+        H : float
+            Required depth of the borefield [m]
+
+        Raises
+        ------
+         ValueError
+            ValueError when no ground data is provided or quadrant is not in range.
+        UnsolvableDueToTemperatureGradient
+            Error when the field cannot be sized.
+        """
+        # check ground data
+        if not self.ground_data.check_values():
+            raise ValueError("Please provide ground data.")
+        # check quadrants
+        if not quadrant_sizing in range(0, 5):
+            raise ValueError(f"Quadrant {quadrant_sizing} does not exist.")
+
+        # initiate with a given depth
+        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
+
+        if quadrant_sizing != 0:
+            # size according to a specific quadrant
+            self.H, _ = self._size_based_on_temperature_profile(quadrant_sizing)
+            return self.H
+        else:
+            try:
+                max_temp, sized = self._size_based_on_temperature_profile(10, deep_sizing=self._calculation_setup.force_deep_sizing)
+            except MaximumNumberOfIterations as e:
+                # no convergence with normal method, but perhaps with deep_sizing enabled
+                if self._calculation_setup.deep_sizing and self.ground_data.variable_Tg:
+                    max_temp, sized = self._size_based_on_temperature_profile(10, deep_sizing=True)
+                else:
+                    raise e
+            if sized:
+                # already correct size
+                self.H = max_temp
+                if self.load.imbalance <= 0:
+                    self.limiting_quadrant = 1
+                else:
+                    self.limiting_quadrant = 2
+                return max_temp
+            min_temp, sized = self._size_based_on_temperature_profile(20)
+            if sized:
+                self.H = min_temp
+                if self.load.imbalance <= 0:
+                    self.limiting_quadrant = 4
+                else:
+                    self.limiting_quadrant = 3
+                return min_temp
+            raise UnsolvableDueToTemperatureGradient
+
+    def size_L4(self, H_init: float = None, quadrant_sizing: int = 0) -> float:
+        """
+        This function sizes the borefield based on an hourly (L4) sizing methodology.
+
+        Parameters
+        ----------
+        H_init : float
+            Initial depth from where to start the iteration [m]
+        quadrant_sizing : int
+            If a quadrant is given the sizing is performed for this quadrant else for the relevant
+
+        Returns
+        -------
+        H : float
+            Required depth of the borefield [m]
+
+        Raises
+        ------
+        ValueError
+           ValueError when no ground data is provided or quadrant is not in range.
+        UnsolvableDueToTemperatureGradient
+           When the field cannot be sized due to the temperature gradient.
+        """
+        # check ground data
+        if not self.ground_data.check_values():
+            raise ValueError("Please provide ground data.")
+        # check quadrants
+        if not quadrant_sizing in range(0, 5):
+            raise ValueError(f"Quadrant {quadrant_sizing} does not exist.")
+
+        # check if hourly data is given
+        if not self.load.hourly_resolution:
+            raise ValueError("There is no hourly resolution available!")
+
+        # initiate with a given depth
+        self.H: float = H_init if H_init is not None else self._calculation_setup.H_init
+
+        if quadrant_sizing != 0:
+            # size according to a specific quadrant
+            self.H, _ = self._size_based_on_temperature_profile(quadrant_sizing, hourly=True)
+            return self.H
+        else:
+            try:
+                max_temp, sized = (
+                    self._size_based_on_temperature_profile(10, hourly=True, deep_sizing=self._calculation_setup.force_deep_sizing)
+                    if np.any(self.load.hourly_cooling_load)
+                    else (0, False)
+                )
+            except MaximumNumberOfIterations as e:
+                # no convergence with normal method, but perhaps with deep_sizing enabled
+                if self._calculation_setup.deep_sizing and self.ground_data.variable_Tg:
+                    max_temp, sized = (
+                        self._size_based_on_temperature_profile(10, hourly=True, deep_sizing=True) if np.any(self.load.hourly_cooling_load) else (0, False)
+                    )
+                else:
+                    raise e
+            if sized:
+                # already correct size
+                self.H = max_temp
+                if self.load.imbalance <= 0:
+                    self.limiting_quadrant = 1
+                else:
+                    self.limiting_quadrant = 2
+                return max_temp
+            min_temp, sized = self._size_based_on_temperature_profile(20, hourly=True) if np.any(self.load.hourly_heating_load) else (0, False)
+            if sized:
+                if self.load.imbalance <= 0:
+                    self.limiting_quadrant = 4
+                else:
+                    self.limiting_quadrant = 3
+                self.H = min_temp
+                return min_temp
+            raise UnsolvableDueToTemperatureGradient
+
+    def calculate_next_depth_deep_sizing(self, current_depth: float) -> float:
+        """
+        This method is a slower but more robust way of calculating the next depth in the sizing iteration when the
+        borefield is sized for the maximum fluid temperature when there is a non-constant ground temperature.
+        The method is based (as can be seen in its corresponding validation document) on the assumption that the
+        difference between the maximum temperature in peak cooling and the average undisturbed ground temperature
+        is irreversily proportional to the depth. In this way, given this difference in temperature and the current
+        depth, a new depth can be calculated.
+
+        Parameters
+        ----------
+        current_depth : float
+            The current depth of the borefield [m]
+
+        Returns
+        -------
+        float
+            New depth of the borefield [m]
+        """
+        # diff between the max temperature in peak cooling and the avg undisturbed ground temperature at current_depth
+        delta_temp = np.max(self.results.peak_cooling - self.ground_data.calculate_Tg(current_depth))
+
+        # calculate the maximum temperature difference between the temperature limit and the ground temperature
+        # at current_depth
+        delta_wrt_max = self.Tf_max - self.ground_data.calculate_Tg(current_depth)
+
+        # delta_t1/H1 ~ delta_t2/H2
+        # H2 = delta_t2/delta_t1*current_depth
+        rel_diff = delta_wrt_max / delta_temp
+        new_depth = current_depth / rel_diff
+
+        return new_depth
+
+    def _size_based_on_temperature_profile(self, quadrant: int, hourly: bool = False, deep_sizing: bool = False) -> (float, bool):
+        """
+        This function sizes based on the temperature profile.
+        It sizes for a specific quadrant and can both size with a monthly or an hourly resolution.
+
+        Parameters
+        ----------
+        quadrant : int
+            Differs from 0 when a sizing in a certain quadrant is desired.
+            Quadrants are developed by (Peere et al., 2021) [#PeereBS]_, [#PeereThesis]_
+        hourly : bool
+            True if an hourly resolution should be used
+        deep_sizing : bool
+            True if the slower method should be used for the sizing, which is robuster.
+
+        Returns
+        -------
+        Depth : float
+            Required depth of the borefield [m]
+        Sized : bool
+            True if the required depth also satisfies the other temperature constraint [m]
+        """
+        # initiate iteration
+        H_prev = 0
+
+        if self.H < 1:
+            self.H = 50
+
+        # define loads for sizing
+        # it only calculates the first and the last year, so the sizing is less computationally expensive
+        # loads_short = self.load.hourly_cooling_load - self.load.hourly_heating_load if hourly else self.load.monthly_average_load
+        # loads_short_rev = loads_short[::-1]
+        # loads_long = np.tile(loads_short, 2)
+        #
+        # # initialise the results array
+        # results = np.zeros(loads_short.size * 2)
+
+        if deep_sizing:
+            # set borefield to minimal depth
+            self.H = 20
+
+        # Iterates as long as there is no convergence
+        # (convergence if difference between depth in iterations is smaller than THRESHOLD_BOREHOLE_DEPTH)
+        i = 0
+        while not self._check_convergence(self.H, H_prev, i):
+            if hourly:
+                self._calculate_temperature_profile(self.H, hourly=True)
+            else:
+                self._calculate_temperature_profile(self.H, hourly=False)
+            H_prev = self.H
+            if not deep_sizing:
+                if quadrant == 1:
+                    # maximum temperature
+                    # convert back to required length
+                    self.H = (np.max(self.results.peak_cooling[: 8760 if hourly else 12]) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
+                elif quadrant == 2:
+                    # maximum temperature
+                    # convert back to required length
+                    self.H = (np.max(self.results.peak_cooling[-8760 if hourly else -12 :]) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
+                elif quadrant == 3:
+                    # minimum temperature
+                    # convert back to required length
+                    self.H = (np.min(self.results.peak_heating[: 8760 if hourly else 12]) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
+                elif quadrant == 4:
+                    # minimum temperature
+                    # convert back to required length
+                    self.H = (np.min(self.results.peak_heating[-8760 if hourly else -12 :]) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
+                elif quadrant == 10:
+                    # over all years
+                    # maximum temperature
+                    # convert back to required length
+                    self.H = (np.max(self.results.peak_cooling) - self._Tg()) / (self.Tf_max - self._Tg()) * H_prev
+                elif quadrant == 20:
+                    # over all years
+                    # minimum temperature
+                    # convert back to required length
+                    self.H = (np.min(self.results.peak_heating) - self._Tg()) / (self.Tf_min - self._Tg()) * H_prev
+            elif self.ground_data.variable_Tg:
+                # for when the temperature gradient is active and it is cooling
+                self.H = self.calculate_next_depth_deep_sizing(H_prev)
+            if self.H < 0:
+                return 0, False
+
+            i += 1
+
+        return self.H, (np.max(self.results.peak_cooling) <= self.Tf_max + 0.05 or (quadrant == 10 or quadrant == 1 or quadrant == 2)) and (
+            np.min(self.results.peak_heating) >= self.Tf_min - 0.05 or (quadrant == 20 or quadrant == 3 or quadrant == 4)
+        )
+
+    @property
+    def investment_cost(self) -> float:
+        """
+        This function calculates the investment cost based on a cost profile linear to the total borehole length.
+
+        Returns
+        -------
+        float
+            Investment cost
+        """
+        return np.polyval(self.cost_investment, self.H * self.number_of_boreholes)
+
+    def calculate_temperatures(self, depth: float = None, hourly: bool = False) -> None:
+        """
+        Calculate all the temperatures without plotting the figure. When depth is given, it calculates it for a given
+        depth.
+
+        Parameters
+        ----------
+        depth : float
+            Depth for which the temperature profile should be calculated for [m]
+        hourly : bool
+            True when the temperatures should be calculated based on hourly data
+
+        Returns
+        -------
+        None
+        """
+        self._calculate_temperature_profile(H=depth, hourly=hourly)
+
+    def print_temperature_profile(self, legend: bool = True, plot_hourly: bool = False) -> None:
+        """
+        This function plots the temperature profile for the calculated depth.
+        It uses the available temperature profile data.
+
+        Parameters
+        ----------
+        legend : bool
+            True if the legend should be printed
+        plot_hourly : bool
+            True if the temperature profile printed should be based on the hourly load profile.
+
+        Returns
+        -------
+        fig, ax
+            Figure object
+        """
+        # calculate temperature profile
+        self._calculate_temperature_profile(hourly=plot_hourly)
+
+        return self._plot_temperature_profile(legend=legend, plot_hourly=plot_hourly)
+
+    def print_temperature_profile_fixed_depth(self, depth: float, legend: bool = True, plot_hourly: bool = False):
+        """
+        This function plots the temperature profile for a fixed depth.
+        It uses the already calculated temperature profile data, if available.
+
+        Parameters
+        ----------
+        depth : float
+            Depth at which the temperature profile should be shown
+        legend : bool
+            True if the legend should be printed
+        plot_hourly : bool
+            True if the temperature profile printed should be based on the hourly load profile.
+
+        Returns
+        -------
+        fig, ax
+            Figure object
+        """
+        # calculate temperature profile
+        self._calculate_temperature_profile(H=depth, hourly=plot_hourly)
+
+        return self._plot_temperature_profile(legend=legend, plot_hourly=plot_hourly)
+
+    def _plot_temperature_profile(self, legend: bool = True, plot_hourly: bool = False) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        This function plots the temperature profile.
+
+        Parameters
+        ----------
+        legend : bool
+            True if the legend should be printed
+        plot_hourly : bool
+            True if the temperature profile printed should be based on the hourly load profile.
+
+        Returns
+        -------
+        fig, ax
+            Figure object
+        """
+
+        # make a time array
+        if plot_hourly:
+            time_array = self.load.time_L4 / 12 / 3600 / 730
+        else:
+            time_array = self.load.time_L3 / 12 / 730.0 / 3600.0
+
+        # plt.rc('figure')
+        # create new figure and axes if it not already exits otherwise clear it.
+        fig = plt.figure()
+        ax = fig.add_subplot(111)
+        # set axes labelsv
+        ax.set_xlabel(r"Time (year)")
+        ax.set_ylabel(r"Temperature ($^\circ C$)")
+        ax.yaxis.label.set_color(plt.rcParams["axes.labelcolor"])
+        ax.xaxis.label.set_color(plt.rcParams["axes.labelcolor"])
+
+        # plot Temperatures
+        ax.step(time_array, self.results.Tb, "k-", where="post", lw=1.5, label="Tb")
+
+        if plot_hourly:
+            ax.step(time_array, self.results.peak_cooling, "b-", where="post", lw=1, label="Tf")
+        else:
+            ax.step(time_array, self.results.peak_cooling, "b-", where="post", lw=1.5, label="Tf peak cooling")
+            ax.step(time_array, self.results.peak_heating, "r-", where="post", lw=1.5, label="Tf peak heating")
+
+            ax.step(time_array, self.results.monthly_cooling, color="b", linestyle="dashed", where="post", lw=1.5, label="Tf base cooling")
+            ax.step(time_array, self.results.monthly_heating, color="r", linestyle="dashed", where="post", lw=1.5, label="Tf base heating")
+
+        # define temperature bounds
+        ax.hlines(self.Tf_min, 0, self.simulation_period, colors="r", linestyles="dashed", label="", lw=1)
+        ax.hlines(self.Tf_max, 0, self.simulation_period, colors="b", linestyles="dashed", label="", lw=1)
+        ax.set_xticks(range(0, self.simulation_period + 1, 2))
+
+        # Plot legend
+        if legend:
+            ax.legend()
+        ax.set_xlim(left=0, right=self.simulation_period)
+        plt.show()
+        return fig, ax
+
+    def _delete_calculated_temperatures(self) -> None:
+        """
+        This function deletes all the calculated temperatures.
+
+        Returns
+        -------
+        None
+        """
+        self.results = Results()
+        self._building_load = HourlyGeothermalLoad()
+        self._secundary_borefield_load = HourlyGeothermalLoad()
+        ghe_logger.info("Deleted all stored temperatures from previous calculations.")
+
+    def _calculate_temperature_profile(self, H: float = None, hourly: bool = False) -> None:
+        """
+        This function calculates the evolution in the fluid temperature and borehole wall temperature.
+
+        Parameters
+        ----------
+        H : float
+            Depth at which the temperatures should be evaluated [m]. If None, than the current depth is taken.
+        hourly : bool
+            True if the temperature evolution should be calculated on an hourly basis.
+
+        Returns
+        -------
+        None
+        """
+
+        # set Rb* value
+        Rb = self.borehole.get_Rb(H if H is not None else self.H, self.D, self.r_b, self.ground_data.k_s(self.H))
+        H = H if H is not None else self.H
+
+        if not hourly:
+            # self.g-function is a function that uses the precalculated data to interpolate the correct values of the
+            # g-function. This dataset is checked over and over again and is correct
+            g_values = self.gfunction(self.load.time_L3, H)
+
+            # the g-function value of the peak with length_peak hours
+            g_value_peak_cooling = self.gfunction(self.load.peak_cooling_duration, H)[0]
+            if self.load.peak_cooling_duration == self.load.peak_heating_duration:
+                g_value_peak_heating = g_value_peak_cooling
+            else:
+                g_value_peak_heating = self.gfunction(self.load.peak_heating_duration, H)[0]
+
+            # calculation of needed differences of the g-function values. These are the weight factors in the calculation
+            # of Tb.
+            g_value_differences = np.diff(g_values, prepend=0)
+
+            # convolution to get the monthly results
+            results = convolve(self.load.monthly_average_load_simulation_period * 1000, g_value_differences)[: 12 * self.simulation_period]
+
+            # calculation the borehole wall temperature for every month i
+            k_s = self.ground_data.k_s(H)
+            Tb = results / (2 * pi * k_s) / (H * self.number_of_boreholes) + self._Tg(H)
+
+            # now the Tf will be calculated based on
+            # Tf = Tb + Q * R_b
+            results_month_cooling = Tb + self.load.baseload_cooling_power_simulation_period * 1000 * (Rb / self.number_of_boreholes / H)
+            results_month_heating = Tb - self.load.baseload_heating_power_simulation_period * 1000 * (Rb / self.number_of_boreholes / H)
+
+            # extra summation if the g-function value for the peak is included
+            results_peak_cooling = (
+                results_month_cooling
+                + (self.load.peak_cooling_simulation_period - self.load.baseload_cooling_power_simulation_period)
+                * 1000
+                * (g_value_peak_cooling / k_s / 2 / pi + Rb)
+                / self.number_of_boreholes
+                / H
+            )
+            results_peak_heating = (
+                results_month_heating
+                - (self.load.peak_heating_simulation_period - self.load.baseload_heating_power_simulation_period)
+                * 1000
+                * (g_value_peak_heating / k_s / 2 / pi + Rb)
+                / self.number_of_boreholes
+                / H
+            )
+
+            # save temperatures under variable
+            self.results = Results(
+                borehole_wall_temp=Tb,
+                peak_heating=results_peak_heating,
+                peak_cooling=results_peak_cooling,
+                monthly_heating=results_month_heating,
+                monthly_cooling=results_month_cooling,
+            )
+
+        if hourly:
+            # check for hourly data if this is requested
+            if not self.load.hourly_resolution:
+                raise ValueError("There is no hourly resolution available!")
+
+            hourly_load = self.load.hourly_load_simulation_period
+
+            # self.g-function is a function that uses the precalculated data to interpolate the correct values of the
+            # g-function. This dataset is checked over and over again and is correct
+            g_values = self.gfunction(self.load.time_L4, H)
+
+            # calculation of needed differences of the g-function values. These are the weight factors in the calculation
+            # of Tb.
+            g_value_differences = np.diff(g_values, prepend=0)
+
+            # convolution to get the monthly results
+            results = convolve(hourly_load * 1000, g_value_differences)[: len(hourly_load)]
+
+            # calculation the borehole wall temperature for every month i
+            Tb = results / (2 * pi * self.ground_data.k_s(H)) / (H * self.number_of_boreholes) + self._Tg(H)
+
+            # now the Tf will be calculated based on
+            # Tf = Tb + Q * R_b
+            temperature_result = Tb + hourly_load * 1000 * (Rb / self.number_of_boreholes / H)
+
+            # reset other variables
+            self.results = Results(borehole_wall_temp=Tb, peak_heating=temperature_result, peak_cooling=temperature_result)
+
+    def set_options_gfunction_calculation(self, options: dict) -> None:
+        """
+        This function sets the options for the gfunction calculation of pygfunction.
+        This dictionary is directly passed through to the gFunction class of pygfunction.
+        For more information, please visit the documentation of pygfunction.
+
+        Parameters
+        ----------
+        options : dict
+            Dictionary with options for the gFunction class of pygfunction
+
+        Returns
+        -------
+        None
+        """
+        self.gfunction_calculation_object.set_options_gfunction_calculation(options)
+
+    def gfunction(self, time_value: ArrayLike, H: float = None) -> np.ndarray:
+        """
+        This function returns the gfunction value.
+        It can do so by either calculating the gfunctions just-in-time or by interpolating from a
+        loaded custom data file.
+
+        Parameters
+        ----------
+        time_value : list, float, np.ndarray
+            Time value(s) in seconds at which the gfunctions should be calculated
+        H : float
+            Depth [m] at which the gfunctions should be calculated.
+            If no depth is given, the current depth is taken.
+
+        Returns
+        -------
+        gvalue : np.ndarray
+            1D array with the g-values for all the requested time_value(s)
+        """
+        H_var = H
+        if H is None:
+            H_var = self.H
+        # when using a variable ground temperature, sometimes no solution can be found
+        if not isinstance(self.ground_data, GroundConstantTemperature) and H_var > Borefield.THRESHOLD_DEPTH_ERROR:
+            raise UnsolvableDueToTemperatureGradient
+
+        def jit_gfunction_calculation() -> np.ndarray:
+            """
+            This function calculates the gfunction just-in-time.
+
+            Returns
+            -------
+            gvalues : np.ndarray
+                1D array with the g-values for the requested time intervals
+            """
+            # set the correct depth of the borefield
+            if not H is None:
+                # only update if H is provided, otherwise the depths of the borefield itself will be used
+                self._update_borefield_depth(H=H)
+            return self.gfunction_calculation_object.calculate(
+                time_value, self.borefield, self.ground_data.alpha(H_var), interpolate=self._calculation_setup.interpolate_gfunctions
+            )
+
+        ## 1 bypass any possible precalculated g-functions
+        # if calculate is False, then the gfunctions are calculated jit
+        if not self._calculation_setup.use_precalculated_dataset:
+            return jit_gfunction_calculation()
+
+        ## 2 use precalculated g-functions when available
+        if self.custom_gfunction is not None:
+            # there is precalculated data available
+            # check if the requested values can be calculated using the custom_gfunction
+            if self.custom_gfunction.within_range(time_value, H_var):
+                return self.custom_gfunction.calculate_gfunction(time_value, H_var)
+
+        ## 3 calculate g-function jit
+        return jit_gfunction_calculation()
+
+    def create_custom_dataset(self, time_array: ArrayLike = None, depth_array: ArrayLike = None, options: dict = {}) -> None:
+        """
+        This function makes a datafile for a given custom borefield and sets it for the borefield object.
+        It automatically sets this datafile in the current borefield object, so it can be used as a source for
+        the interpolation of g-values.
+
+        Parameters
+        ----------
+        time_array : list, np.array
+            Time values (in seconds) used for the calculation of the datafile
+        depth_array : list, np.array
+            List or arrays of depths for which the datafile should be created
+        options : dict
+            Options for the g-function calculation (check pygfunction.gfunction.gFunction() for more information)
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            When no borefield or ground data is set
+        """
+
+        try:
+            self.borefield[0]
+        except TypeError:
+            raise ValueError("No borefield is set for which the gfunctions should be calculated")
+        try:
+            self.ground_data.alpha(H=100)
+        except AttributeError:
+            raise ValueError("No ground data is set for which the gfunctions should be calculated")
+
+        self.custom_gfunction = CustomGFunction(time_array, depth_array, options)
+        self.custom_gfunction.create_custom_dataset(self.borefield, self.ground_data.alpha)
+
+    @property
+    def Re(self) -> float:
+        """
+        Reynolds number.
+
+        Returns
+        -------
+        float
+            Reynolds number
+        """
+        return self.borehole.Re
+
+    def optimise_load_profile(self,
+        building_load: HourlyGeothermalLoad,
+        depth: float = None,
+        SCOP: float = 10**6,
+        SEER: float = 10**6,
+        temperature_threshold: float = 0.05,
+        print_results: bool = False):
+
+        warnings.warn(DeprecationWarning('Optimise_load_profile is replaced by optimise_load_profile_power'
+                                         'or optimise_load_profile_energy. This method will be depreciated in '
+                                         'v2.3.1.'))
+
+        self.optimise_load_profile_power(building_load=building_load,
+                                         depth=depth,
+                                         SCOP=SCOP,
+                                         SEER=SEER,
+                                         temperature_threshold=temperature_threshold)
+
+        if print_results:
+            warnings.warn(DeprecationWarning('print_results will be depreciated from v2.3.1 onwards for code clarity. '
+                                             'The user can replicate the same behaviour manually.'))
+            # print results
+            print(
+                "The peak load heating is: ",
+                f"{self._secundary_borefield_load.max_peak_heating:.0f}",
+                "kW, leading to",
+                f"{np.sum(self._secundary_borefield_load.hourly_heating_load):.0f}",
+                "kWh of heating.",
+            )
+            print("This is", f"{self._percentage_heating:.0f}", "% of the total heating load.")
+            print(
+                "Another",
+                f"{np.sum(self._external_load.hourly_heating_load):.0f}",
+                "kWh of heating should come from another source, with a peak of",
+                f"{self._external_load.max_peak_heating:.0f}",
+                "kW.",
+            )
+            print("------------------------------------------")
+            print(
+                "The peak load cooling is: ",
+                f"{self._secundary_borefield_load.max_peak_cooling:.0f}",
+                "kW, leading to",
+                f"{np.sum(self._secundary_borefield_load.hourly_cooling_load):.0f}",
+                "kWh of cooling.",
+            )
+            print("This is", f"{self._percentage_cooling:.0f}", "% of the total cooling load.")
+            print(
+                "Another",
+                f"{np.sum(self._external_load.hourly_cooling_load):.0f}",
+                "kWh of cooling should come from another source, with a peak of",
+                f"{self._external_load.max_peak_cooling:.0f}",
+                "kW.",
+            )
+
+            # plot results
+            self.print_temperature_profile_fixed_depth(depth=depth)
+
+    def optimise_load_profile_power(
+        self,
+        building_load: HourlyGeothermalLoad,
+        depth: float = None,
+        SCOP: float = 10**6,
+        SEER: float = 10**6,
+        temperature_threshold: float = 0.05,
+        use_hourly_resolution: bool = True
+    ) -> None:
+        """
+        This function optimises the load based on the given borefield and the given hourly load.
+        (When the load is not geothermal, the SCOP and SEER are used to convert it to a geothermal load.)
+        It does so based on a load-duration curve. The temperatures of the borefield are calculated on a monthly
+        basis, even though we have hourly data, for an hourly calculation of the temperatures
+        would take a very long time.
+
+        Parameters
+        ----------
+        building_load : _LoadData
+            Load data used for the optimisation
+        depth : float
+            Depth of the boreholes in the borefield [m]
+        SCOP : float
+            SCOP of the geothermal system (needed to convert hourly building load to geothermal load)
+        SEER : float
+            SEER of the geothermal system (needed to convert hourly building load to geothermal load)
+        temperature_threshold : float
+            The maximum allowed temperature difference between the maximum and minimum fluid temperatures and their
+            respective limits. The lower this threshold, the longer the convergence will take.
+        use_hourly_resolution : bool
+            If use_hourly_resolution is used, the hourly data will be used for this optimisation. This can take some
+            more time than using the monthly resolution, but it will give more accurate results.
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            ValueError if no hourly load is given or the threshold is negative
+        """
+
+        ## Explain variables
+        # load --> primary, geothermal load
+        # _building_load --> secundary, building load
+        # _secundary_borefield_load --> secundary, geothermal load
+
+        # check if hourly load is given
+        if not building_load.hourly_resolution:
+            raise ValueError("No hourly load was given!")
+
+        # check if threshold is positive
+        if temperature_threshold < 0:
+            raise ValueError(f"The temperature threshold is {temperature_threshold}, but it cannot be below 0!")
+
+        # set depth
+        if depth is None:
+            depth = self.H
+
+        # since the depth does not change, the Rb* value is constant
+        # set to use a constant Rb* value but save the initial parameters
+        Rb_backup = self.borehole.Rb
+        use_constant_Rb_backup = self.borehole.use_constant_Rb
+        self.Rb = self.borehole.get_Rb(depth, self.D, self.r_b, self.ground_data.k_s(depth))
+
+        # load hourly heating and cooling load and convert it to geothermal loads
+        primary_geothermal_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
+        primary_geothermal_load.set_hourly_cooling(building_load.hourly_cooling_load.copy() * (1 + 1 / SEER))
+        primary_geothermal_load.set_hourly_heating(building_load.hourly_heating_load.copy() * (1 - 1 / SCOP))
+
+        # set geothermal load
+        self.load = copy.deepcopy(primary_geothermal_load)
+
+        # set initial peak loads
+        init_peak_heating: float = self.load.max_peak_heating
+        init_peak_cooling: float = self.load.max_peak_cooling
+
+        # peak loads for iteration
+        peak_heat_load_geo: float = init_peak_heating
+        peak_cool_load_geo: float = init_peak_cooling
+
+        # set iteration criteria
+        cool_ok, heat_ok = False, False
+
+        while not cool_ok or not heat_ok:
+            # limit the primary geothermal heating and cooling load to peak_heat_load_geo and peak_cool_load_geo
+            self.load.set_hourly_cooling(np.minimum(peak_cool_load_geo, primary_geothermal_load.hourly_cooling_load))
+            self.load.set_hourly_heating(np.minimum(peak_heat_load_geo, primary_geothermal_load.hourly_heating_load))
+
+            # calculate temperature profile, just for the results
+            self.calculate_temperatures(depth=depth, hourly=use_hourly_resolution)
+
+            # deviation from minimum temperature
+            if abs(min(self.results.peak_heating) - self.Tf_min) > temperature_threshold:
+                # check if it goes below the threshold
+                if min(self.results.peak_heating) < self.Tf_min:
+                    peak_heat_load_geo = max(0.1, peak_heat_load_geo - 1 * max(1, 10 * (self.Tf_min - min(self.results.peak_heating))))
+                else:
+                    peak_heat_load_geo = min(init_peak_heating, peak_heat_load_geo * 1.01)
+                    if peak_heat_load_geo == init_peak_heating:
+                        heat_ok = True
+            else:
+                heat_ok = True
+
+            # deviation from maximum temperature
+            if abs(np.max(self.results.peak_cooling) - self.Tf_max) > temperature_threshold:
+                # check if it goes above the threshold
+                if np.max(self.results.peak_cooling) > self.Tf_max:
+                    peak_cool_load_geo = max(0.1, peak_cool_load_geo - 1 * max(1, 10 * (-self.Tf_max + np.max(self.results.peak_cooling))))
+                else:
+                    peak_cool_load_geo = min(init_peak_cooling, peak_cool_load_geo * 1.01)
+                    if peak_cool_load_geo == init_peak_cooling:
+                        cool_ok = True
+            else:
+                cool_ok = True
+
+        # calculate the resulting secundary hourly profile that can be put on the borefield
+        self._secundary_borefield_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
+        self._secundary_borefield_load.set_hourly_cooling(self.load.hourly_cooling_load / (1 + 1 / SEER))
+        self._secundary_borefield_load.set_hourly_heating(self.load.hourly_heating_load / (1 - 1 / SCOP))
+
+        # set building load
+        self._building_load = building_load
+
+        # calculate external load
+        self._external_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
+        self._external_load.set_hourly_heating(np.maximum(0, building_load.hourly_heating_load - self._secundary_borefield_load.hourly_heating_load))
+        self._external_load.set_hourly_cooling(np.maximum(0, building_load.hourly_cooling_load - self._secundary_borefield_load.hourly_cooling_load))
+
+        # restore the initial parameters
+        self.Rb = Rb_backup
+        self.borehole.use_constant_Rb = use_constant_Rb_backup
+
+    def optimise_load_profile_energy(
+        self,
+        building_load: HourlyGeothermalLoad,
+        depth: float = None,
+        SCOP: float = 10**6,
+        SEER: float = 10**6,
+        temperature_threshold: float = 0.05,
+    ) -> None:
+        """
+        This function optimises the load based on the given borefield and the given hourly load.
+        (When the load is not geothermal, the SCOP and SEER are used to convert it to a geothermal load.)
+        It does so based on a load-duration curve. The temperatures of the borefield are calculated on a monthly
+        basis, even though we have hourly data, for an hourly calculation of the temperatures
+        would take a very long time.
+
+        Parameters
+        ----------
+        building_load : _LoadData
+            Load data used for the optimisation
+        depth : float
+            Depth of the boreholes in the borefield [m]
+        SCOP : float
+            SCOP of the geothermal system (needed to convert hourly building load to geothermal load)
+        SEER : float
+            SEER of the geothermal system (needed to convert hourly building load to geothermal load)
+        temperature_threshold : float
+            The maximum allowed temperature difference between the maximum and minimum fluid temperatures and their
+            respective limits. The lower this threshold, the longer the convergence will take.
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            ValueError if no hourly load is given or the threshold is negative
+        """
+
+        ## Explain variables
+        # load --> primary, geothermal load
+        # _building_load --> secundary, building load
+        # _secundary_borefield_load --> secundary, geothermal load
+
+        # check if hourly load is given
+        if not building_load.hourly_resolution:
+            raise ValueError("No hourly load was given!")
+
+        # check if threshold is positive
+        if temperature_threshold < 0:
+            raise ValueError(f"The temperature threshold is {temperature_threshold}, but it cannot be below 0!")
+
+        # set depth
+        if depth is None:
+            depth = self.H
+
+        # since the depth does not change, the Rb* value is constant
+        # set to use a constant Rb* value but save the initial parameters
+        Rb_backup = self.borehole.Rb
+        use_constant_Rb_backup = self.borehole.use_constant_Rb
+        self.Rb = self.borehole.get_Rb(depth, self.D, self.r_b, self.ground_data.k_s)
+
+        # load hourly heating and cooling load and convert it to geothermal loads
+        primary_geothermal_load = HourlyGeothermalLoad(simulation_period=building_load.simulation_period)
+        primary_geothermal_load.set_hourly_cooling(building_load.hourly_cooling_load.copy() * (1 + 1 / SEER))
+        primary_geothermal_load.set_hourly_heating(building_load.hourly_heating_load.copy() * (1 - 1 / SCOP))
+
+        # set relation qh-qm
+        nb_points = 100
+
+        power_heating_range = np.linspace(0.001, primary_geothermal_load.max_peak_heating, nb_points)
+        power_cooling_range = np.linspace(0.001, primary_geothermal_load.max_peak_cooling, nb_points)
+
+        # relationship between the peak load and the corresponding monthly load
+        heating_peak_bl = np.zeros((nb_points, 12))
+        cooling_peak_bl = np.zeros((nb_points, 12))
+
+        for idx in range(nb_points):
+            heating_peak_bl[idx] = primary_geothermal_load.resample_to_monthly(np.minimum(power_heating_range[idx], primary_geothermal_load.hourly_heating_load))[1]
+            cooling_peak_bl[idx] = primary_geothermal_load.resample_to_monthly(np.minimum(power_cooling_range[idx], primary_geothermal_load.hourly_cooling_load))[1]
+
+        # create monthly multi-load
+        primary_monthly_load = \
+            MonthlyGeothermalLoadMultiYear(baseload_heating=primary_geothermal_load.baseload_heating_simulation_period,
+                                           baseload_cooling=primary_geothermal_load.baseload_cooling_simulation_period,
+                                           peak_heating=primary_geothermal_load.peak_heating_simulation_period,
+                                           peak_cooling=primary_geothermal_load.peak_cooling_simulation_period)
+
+        self.load = primary_monthly_load
+
+        # store initial monthly peak loads
+        peak_heating = primary_geothermal_load.peak_heating
+        peak_cooling = primary_geothermal_load.peak_cooling
+
+        for i in range(12 * self.load.simulation_period):
+            # set iteration criteria
+            cool_ok, heat_ok = False, False
+
+            while not cool_ok or not heat_ok:
+                # calculate temperature profile, just for the results
+                self.calculate_temperatures(depth)
+
+                # deviation from minimum temperature
+                if abs(self.results.peak_heating[i] - self.Tf_min) > temperature_threshold:
+                    # check if it goes below the threshold
+                    curr_heating_peak = self.load.peak_heating_simulation_period[i]
+                    if self.results.peak_heating[i] < self.Tf_min:
+                        curr_heating_peak = max(0.1, curr_heating_peak - 1 * max(1, 10 * (self.Tf_min - self.results.peak_heating[i])))
+                    else:
+                        curr_heating_peak = min(peak_heating[i % 12], curr_heating_peak * 1.01)
+                        if curr_heating_peak == peak_heating[i % 12]:
+                            heat_ok = True
+                    self.load._peak_heating[i], self.load._baseload_heating[i] =\
+                        curr_heating_peak, np.interp(curr_heating_peak, power_heating_range, heating_peak_bl[:, i % 12])
+                else:
+                    heat_ok = True
+
+                # deviation from maximum temperature
+                if abs(self.results.peak_cooling[i] - self.Tf_max) > temperature_threshold:
+                    # check if it goes above the threshold
+                    curr_cooling_peak = self.load.peak_cooling_simulation_period[i]
+                    if self.results.peak_cooling[i] > self.Tf_max:
+                        curr_cooling_peak = max(0.1, curr_cooling_peak - 1 * max(1, 10 * (
+                                    -self.Tf_max + np.max(self.results.peak_cooling))))
+                    else:
+                        curr_cooling_peak = min(peak_cooling[i % 12], curr_cooling_peak * 1.01)
+                        if curr_cooling_peak == peak_cooling[i % 12]:
+                            cool_ok = True
+                    self.load._peak_cooling[i], self.load._baseload_cooling[i] = \
+                        curr_cooling_peak, np.interp(curr_cooling_peak, power_cooling_range, cooling_peak_bl[:, i % 12])
+                else:
+                    cool_ok = True
+
+        def f(hourly_load, monthly_peak) -> np.ndarray:
+            """
+            This function creates a new hourly load where the values are limited by the monthly peaks.
+
+            Parameters
+            ----------
+            hourly_load : np.ndarray
+                An array with hourly values
+            monthly_peak : np.ndarray
+                An array with monthly values
+
+            Returns
+            -------
+            np.ndarray
+                New array with hourly values where each value is the minimum of the monthly and hourly array
+            """
+            new_load = np.zeros_like(hourly_load)
+            UPM = np.cumsum(np.tile(building_load.UPM, building_load.simulation_period))
+            month_idx = 0
+            for idx, val in enumerate(hourly_load):
+                if idx == UPM[month_idx] and not month_idx == len(UPM) - 1:
+                    month_idx += 1
+                new_load[idx] = min(val, monthly_peak[month_idx])
+            return new_load
+
+        # calculate hourly load
+        temp = HourlyGeothermalLoadMultiYear()
+        temp.hourly_heating_load = f(primary_geothermal_load.hourly_heating_load_simulation_period, self.load.peak_heating_simulation_period)
+        temp.hourly_cooling_load = f(primary_geothermal_load.hourly_cooling_load_simulation_period, self.load.peak_cooling_simulation_period)
+
+        # set correct hourly load
+        self.load = temp
+
+        # calculate the corresponding geothermal load
+        self._secundary_borefield_load = HourlyGeothermalLoadMultiYear()
+        self._secundary_borefield_load.hourly_cooling_load = self.load.hourly_cooling_load_simulation_period / (1 + 1 / SEER)
+        self._secundary_borefield_load.hourly_heating_load = self.load.hourly_heating_load_simulation_period / (1 - 1 / SCOP)
+
+        # set building load
+        self._building_load = building_load
+
+        # calculate external load
+        self._external_load = HourlyGeothermalLoadMultiYear()
+        self._external_load.hourly_heating_load = np.maximum(0, building_load.hourly_heating_load_simulation_period - self._secundary_borefield_load.hourly_heating_load_simulation_period)
+        self._external_load.hourly_cooling_load = np.maximum(0, building_load.hourly_cooling_load_simulation_period - self._secundary_borefield_load.hourly_cooling_load_simulation_period)
+
+        # restore the initial parameters
+        self.Rb = Rb_backup
+        self.borehole.use_constant_Rb = use_constant_Rb_backup
+
+
+    @property
+    def _percentage_heating(self) -> float:
+        """
+        This function returns the percentage of heating load that can be done geothermally.
+
+        Returns
+        -------
+        float
+            Percentage of heating load that can be done geothermally.
+        """
+        return np.sum(self._secundary_borefield_load.hourly_heating_load_simulation_period) /\
+            np.sum(self._building_load.hourly_heating_load_simulation_period) * 100
+
+    @property
+    def _percentage_cooling(self) -> float:
+        """
+        This function returns the percentage of cooling load that can be done geothermally.
+
+        Returns
+        -------
+        float
+            Percentage of cooling load that can be done geothermally.
+        """
+        return np.sum(self._secundary_borefield_load.hourly_cooling_load_simulation_period) /np.sum(self._building_load.hourly_cooling_load_simulation_period) * 100
+
+    def calculate_quadrant(self) -> int:
+        """
+        This function returns the borefield quadrant (as defined by Peere et al., 2021 [#PeereEtAl]_)
+        based on the calculated temperature profile.
+        If there is no limiting quadrant, None is returned.\n
+        Quadrant 1 is limited in the first year by the maximum temperature\n
+        Quadrant 2 is limited in the last year by the maximum temperature\n
+        Quadrant 3 is limited in the first year by the minimum temperature\n
+        Quadrant 4 is limited in the last year by the maximum temperature
+
+        Returns
+        ----------
+        quadrant : int
+            The quadrant which limits the borefield
+
+        References
+        ----------
+        .. [#PeereEtAl] Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021) Validated combined first and last year borefield sizing methodology. In Proceedings of International Building Simulation Conference 2021. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
+        """
+
+        # calculate temperatures if they are not calculated
+        if not np.any(self.results.peak_heating):
+            ghe_logger.warning(
+                "There are not yet temperatures calculated, hence there is no limiting quadrant." "The temperature is calculated now, based on monthly values."
+            )
+            self.calculate_temperatures()
+
+        # calculate max/min fluid temperatures
+        max_temp = np.max(self.results.peak_cooling)
+        min_temp = np.min(self.results.peak_heating)
+
+        # calculate temperature difference w.r.t. the limits
+        DT_max = -self.Tf_max + max_temp + 1000  # + 1000 to have no problems with negative temperatures
+        DT_min = self.Tf_min - min_temp + 1000
+
+        # if the temperature limit is not crossed, return None
+        if self.Tf_max - 0.1 > max_temp and self.Tf_min + 0.1 < min_temp:
+            return
+
+        # True if heating/extraction dominated
+        if self.load.imbalance < 0:
+            # either quadrant 1 or 4
+            if DT_min > DT_max:
+                # limited by minimum temperature
+                return 4
+            return 1
+
+        # quadrant 2 or 3
+        if DT_min > DT_max:
+            # limited by minimum temperature
+            return 3
+        return 2
+
+    def plot_load_duration(self, legend: bool = False) -> Tuple[plt.Figure, plt.Axes]:
+        """
+        This function makes a load-duration curve from the hourly values.
+
+        Parameters
+        ----------
+        legend : bool
+            True if the figure should have a legend
+
+        Returns
+        ----------
+        Tuple
+            plt.Figure, plt.Axes
+        """
+        # check if there are hourly values
+        if not self.load.hourly_resolution:
+            raise ValueError("There is no hourly resolution available!")
+
+        # sort heating and cooling load
+        heating = self.load.hourly_heating_load.copy()
+        heating[::-1].sort()
+
+        cooling = self.load.hourly_cooling_load.copy()
+        cooling.sort()
+        cooling = cooling * (-1)
+        # create new figure and axes if it not already exits otherwise clear it.
+        fig = plt.figure()
+        ax = fig.add_subplot(111)
+        # add sorted loads to plot
+        ax.step(np.arange(0, 8760, 1), heating, "r-", label="Heating")
+        ax.step(np.arange(0, 8760, 1), cooling, "b-", label="Cooling")
+        # create 0 line
+        ax.hlines(0, 0, 8759, color="black")
+        # add labels
+        ax.set_xlabel("Time [hours]")
+        ax.set_ylabel("Power [kW]")
+        # set x limits to 8760
+        ax.set_xlim(0, 8760)
+        # plot legend if wanted
+        if legend:
+            ax.legend()  #
+        plt.show()
+        return fig, ax
```

### Comparing `GHEtool-2.2.1/GHEtool/test/general_tests/test_GHEtool.py` & `ghetool-2.2.2/GHEtool/test/general_tests/test_GHEtool.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,26 +243,20 @@
 
     borefield = Borefield(load=MonthlyGeothermalLoadAbsolute(*load_case(1)))
 
     borefield.set_ground_parameters(data)
     borefield.set_borefield(borefield_pyg)
     borefield.set_Rb(0.2)
 
-    try:
+    with raises(MaximumNumberOfIterations):
         borefield.size()
-        assert False  # pragma: no cover
-    except MaximumNumberOfIterations:
-        assert True
 
     borefield.calculation_setup(max_nb_of_iterations=500)
-    try:
+    with raises(UnsolvableDueToTemperatureGradient):
         borefield.size()
-        assert False  # pragma: no cover
-    except UnsolvableDueToTemperatureGradient:
-        assert True
 
 
 def test_borefield_with_constant_peaks(borefield):
     # test first year
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(1))
     # do not save previous g-functions
     borefield.gfunction_calculation_object.store_previous_values = False
```

### Comparing `GHEtool-2.2.1/GHEtool/test/methods/TestMethodClass.py` & `ghetool-2.2.2/GHEtool/test/methods/TestMethodClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,27 +23,29 @@
         self.name = name
 
 
 class OptimiseLoadProfileObject:
 
     def __init__(self, borefield: Borefield, load, depth: float, SCOP: float, SEER: float, percentage_heating: float,
                  percentage_cooling: float, peak_heating_geo: float, peak_cooling_geo: float, peak_heating_ext: float,
-                 peak_cooling_ext: float, name: str = ""):
+                 peak_cooling_ext: float, name: str = "", power: bool = True, hourly: bool = True):
         self.borefield = copy.deepcopy(borefield)
         self.load = copy.deepcopy(load)
         self.depth = depth
         self.SCOP = SCOP
         self.SEER = SEER
         self.percentage_heating = percentage_heating
         self.percentage_cooling = percentage_cooling
         self.peak_heating_geo = peak_heating_geo
         self.peak_cooling_geo = peak_cooling_geo
         self.peak_heating_ext = peak_heating_ext
         self.peak_cooling_ext = peak_cooling_ext
         self.name = name
+        self.power = power
+        self.hourly = hourly
 
     def test(self):  # pragma: no cover
         self.borefield.optimise_load_profile(self.load, self.depth, self.SCOP, self.SEER)
         assert np.isclose(self.borefield._percentage_heating, self.percentage_heating)
         assert np.isclose(self.borefield._percentage_cooling, self.percentage_cooling)
         assert np.isclose(self.borefield.load.max_peak_heating, self.peak_heating_geo)
         assert np.isclose(self.borefield.load.max_peak_cooling, self.peak_cooling_geo)
@@ -175,15 +177,15 @@
 
     @property
     def optimise_load_profile_input(self) -> list:
         temp = []
         for _, i in enumerate(self.list_of_test_objects):
             if isinstance(i, SizingObject):
                 continue
-            temp.append((copy.deepcopy(i.borefield), copy.deepcopy(i.load), i.depth, i.SCOP, i.SEER))
+            temp.append((copy.deepcopy(i.borefield), copy.deepcopy(i.load), i.depth, i.SCOP, i.SEER, i.power, i.hourly))
         return temp
 
     @property
     def optimise_load_profile_output(self) -> list:
         temp = []
         for _, i in enumerate(self.list_of_test_objects):
             if isinstance(i, SizingObject):
```

### Comparing `GHEtool-2.2.1/GHEtool/test/methods/method_data.py` & `ghetool-2.2.2/GHEtool/test/methods/method_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 load = MonthlyGeothermalLoadAbsolute(monthly_heating, monthly_cooling, peak_heating, peak_cooling, 25)
 borefield = Borefield(load=load)
 borefield.create_rectangular_borefield(4, 5, 8, 8, 110, 0.8, 0.07)
 borefield.set_ground_parameters(ground_data_IKC)
 borefield.set_fluid_parameters(fluid_data_IKC)
 borefield.set_pipe_parameters(pipe_data_IKC)
 borefield.calculation_setup(use_constant_Rb=False)
-borefield.set_length_peak(10)
+borefield.load.peak_duration = 10
 borefield.set_max_avg_fluid_temperature(25)
 borefield.set_min_avg_fluid_temperature(0)
 list_of_test_objects.add(SizingObject(borefield, error_L2=UnsolvableDueToTemperatureGradient, error_L3=UnsolvableDueToTemperatureGradient, name='Real case 1 (Error)'))
 borefield.calculation_setup(max_nb_of_iterations=20)
 list_of_test_objects.add(SizingObject(borefield, error_L2=RuntimeError, error_L3=UnsolvableDueToTemperatureGradient, name='Real case 1 (Error, max nb of iter)'))
 
 ground_data_IKC = GroundFluxTemperature(2.3, 10.5, flux=2.3*2.85/100)
@@ -334,56 +334,110 @@
 temp = hourly_load.hourly_heating_load
 temp[0] = 100_000
 borefield._borefield_load.hourly_heating_load = temp
 list_of_test_objects.add(SizingObject(borefield, L4_output=18602.210559679363, quadrant=3, name='Hourly profile, quadrant 3'))
 
 hourly_load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 87.506, 97.012,
-                                                   305.842, 384.204, 230.193, 292.212, name='Optimise load profile 1'))
+                                                   305.842, 384.204, 230.193, 292.212, name='Optimise load profile 1 (power)', power=True, hourly=False))
 
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 70.054, 87.899,
-                                                   210.800, 247.186, 325.236, 429.231, name='Optimise load profile 2'))
+                                                   210.800, 247.186, 325.236, 429.231, name='Optimise load profile 2 (power)', power=True, hourly=False))
 
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 50, 10**6, 10**6, 45.096, 63.799,
-                                                   118.898, 117.804, 417.138, 558.612, name='Optimise load profile 3'))
+                                                   118.898, 117.804, 417.138, 558.612, name='Optimise load profile 3 (power)', power=True, hourly=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 87.506, 96.404,
+                                                   305.842, 368.463, 230.193, 307.954, name='Optimise load profile 1 (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 69.662, 87.022,
+                                                   209.053, 239.590, 326.983, 436.827, name='Optimise load profile 2 (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 50, 10**6, 10**6, 44.635, 63.467,
+                                                   117.388, 116.699, 418.648, 559.718, name='Optimise load profile 3 (power, hourly)', power=True, hourly=True))
+
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 93.227, 99.557,
+                                                   536.035, 663.791, 233.455, 290.487, name='Optimise load profile 1 (energy)', power=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 77.527, 96.245,
+                                                   385.562, 414.703, 316.333, 422.325, name='Optimise load profile 2 (energy)', power=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 50, 10**6, 10**6, 50.756, 75.372,
+                                                   181.332, 209.175, 402.103, 553.451, name='Optimise load profile 3 (energy)', power=False))
 
 borefield.set_min_avg_fluid_temperature(-5)
 borefield.set_max_avg_fluid_temperature(25)
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 100, 100,
-                                                   536.036, 676.417, 0, 0, name='Optimise load profile 100%'))
+                                                   536.036, 676.417, 0, 0, name='Optimise load profile 100% (power)', power=True, hourly=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 100, 100,
+                                                   536.036, 676.417, 0, 0, name='Optimise load profile 100% (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 100, 100,
+                                                   536.036, 676.417, 0, 0, name='Optimise load profile 100% (energy)', power=False))
 
 borefield = Borefield()
 borefield.set_ground_parameters(data)
 borefield.set_Rb(0.2)
 borefield.set_borefield(borefield_gt)
 borefield.set_max_avg_fluid_temperature(16)
 borefield.set_min_avg_fluid_temperature(0)
 hourly_load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"), col_heating=1, col_cooling=0)
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 99.976, 66.492,
                                                    643.137, 195.331, 33.278, 340.705,
-                                                   name='Optimise load profile 1, reversed'))
+                                                   name='Optimise load profile 1, reversed (power)', power=True, hourly=False))
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 99.971, 66.424,
+                                                   639.283, 195.053, 37.132, 340.983,
+                                                   name='Optimise load profile 1, reversed (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 99.999, 71.783,
+                                                   676.415, 342.769, 22.620, 344.786,
+                                                   name='Optimise load profile 1, reversed (energy)', power=False))
 borefield.set_max_avg_fluid_temperature(20)
 borefield.set_min_avg_fluid_temperature(4)
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 97.012, 87.506,
                                                    384.204, 305.842, 292.211, 230.195,
-                                                   name='Optimise load profile 2, reversed'))
+                                                   name='Optimise load profile 2, reversed (power)', power=True, hourly=False))
 
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 87.899, 70.054,
                                                    247.186, 210.800, 429.23, 325.236,
-                                                   name='Optimise load profile 3, reversed'))
+                                                   name='Optimise load profile 3, reversed (power)', power=True, hourly=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 96.404, 87.506,
+                                                   368.463, 305.842, 307.953, 230.195,
+                                                   name='Optimise load profile 2, reversed (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 87.022, 69.662,
+                                                   239.590, 209.053, 436.826, 326.984,
+                                                   name='Optimise load profile 3, reversed (power, hourly)', power=True, hourly=True))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 150, 10**6, 10**6, 99.576, 93.039,
+                                                   661.853, 536.037, 287.343, 235.187,
+                                                   name='Optimise load profile 2, reversed (energy)', power=False))
+
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, hourly_load, 100, 10**6, 10**6, 96.304, 77.304,
+                                                   416.623, 384.529, 419.950, 318.392,
+                                                   name='Optimise load profile 3, reversed (energy)', power=False))
 
 borefield = Borefield()
 borefield.create_rectangular_borefield(3, 6, 6, 6, 146, 4)
 borefield.set_min_avg_fluid_temperature(3)
 borefield.set_max_avg_fluid_temperature(16)
-borefield.set_length_peak(6)
+borefield.load.peak_duration = 6
 load = HourlyGeothermalLoad()
 load.load_hourly_profile(FOLDER.joinpath("test\methods\hourly_data\problem_data.csv"), col_heating=0, col_cooling=1, header=True, decimal_seperator=',')
 load.simulation_period = 40
 borefield.load = load
 
 borefield.set_ground_parameters(GroundTemperatureGradient(1.9, 10, gradient=2))
 borefield.set_fluid_parameters(FluidData(0.1, 0.475, 1033, 3930, 0.001))
 borefield.set_pipe_parameters(SingleUTube(1.5, 0.016, 0.02, 0.42, 0.04))
 list_of_test_objects.add(OptimiseLoadProfileObject(borefield, load, 146, 4, 25, 81.6397, 88.1277,
                                                    22.2967, 39.52027, 55.28596, 58.400,
-                                                   name='Optimise load profile (stuck in loop)'))
+                                                   name='Optimise load profile (stuck in loop) (power)', power=True, hourly=False))
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, load, 146, 4, 25, 80.1414, 84.639,
+                                                   21.5547, 35.77766, 56.2753, 61.9987,
+                                                   name='Optimise load profile (stuck in loop) (power, hourly)', power=True, hourly=True))
+list_of_test_objects.add(OptimiseLoadProfileObject(borefield, load, 146, 4, 25, 89.242, 98.362,
+                                                   56.147, 74.421, 55.020, 56.865,
+                                                   name='Optimise load profile (stuck in loop) (energy)', power=False))
```

### Comparing `GHEtool-2.2.1/GHEtool/test/methods/test_methods.py` & `ghetool-2.2.2/GHEtool/test/methods/test_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,62 +5,56 @@
 
 
 @pytest.mark.parametrize("model,result",
                          zip(list_of_test_objects.L2_sizing_input, list_of_test_objects.L2_sizing_output),
                          ids=list_of_test_objects.names_L2)
 def test_L2(model: Borefield, result):
     if not isinstance(result[0], (int, float, str)):
-        try:
+        with pytest.raises(result[0]):
             model.size_L2(100)
-            assert False   # pragma: no cover
-        except result[0]:
-            assert True
     else:
         assert np.isclose(model.size_L2(100), result[0], atol=1e-2)
         assert model.limiting_quadrant == result[1]
 
 
 @pytest.mark.parametrize("model,result",
                          zip(list_of_test_objects.L3_sizing_input, list_of_test_objects.L3_sizing_output),
                          ids=list_of_test_objects.names_L3)
 def test_L3(model: Borefield, result):
     if not isinstance(result[0], (int, float, str)):
-        try:
+        with pytest.raises(result[0]):
             model.size_L3(100)
-            assert False   # pragma: no cover
-        except result[0]:
-            assert True
     else:
         assert np.isclose(model.size_L3(100), result[0], atol=1e-2)
         assert model.calculate_quadrant() == result[1]
 
 
 @pytest.mark.parametrize("model,result",
                          zip(list_of_test_objects.L4_sizing_input, list_of_test_objects.L4_sizing_output),
                          ids=list_of_test_objects.names_L4)
 def test_L4(model: Borefield, result):
     if not isinstance(result[0], (int, float, str)):
-        try:
+        with pytest.raises(result[0]):
             model.size_L4(100)
-            assert False   # pragma: no cover
-        except result[0]:
-            assert True
     else:
         assert np.isclose(model.size_L4(100), result[0], atol=1e-2)
         assert model.calculate_quadrant() == result[1]
 
 
 @pytest.mark.parametrize("input,result",
                          zip(list_of_test_objects.optimise_load_profile_input,
                              list_of_test_objects.optimise_load_profile_output),
                          ids=list_of_test_objects.names_optimise_load_profile)
 def test_optimise(input, result):
     model: Borefield = input[0]
-    load, depth, SCOP, SEER = input[1:]
-    model.optimise_load_profile(load, depth, SCOP, SEER)
+    load, depth, SCOP, SEER, power, hourly = input[1:]
+    if power:
+        model.optimise_load_profile_power(load, depth, SCOP, SEER, use_hourly_resolution=hourly)
+    else:
+        model.optimise_load_profile_energy(load, depth, SCOP, SEER)
     percentage_heating, percentage_cooling, peak_heating_geo, peak_cooling_geo, peak_heating_ext, peak_cooling_ext = \
         result
     assert np.isclose(model._percentage_heating, percentage_heating)
     assert np.isclose(model._percentage_cooling, percentage_cooling)
     assert np.isclose(model.load.max_peak_heating, peak_heating_geo)
     assert np.isclose(model.load.max_peak_cooling, peak_cooling_geo)
     assert np.isclose(model._external_load.max_peak_heating, peak_heating_ext)
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_baseclass.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_baseclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,19 +82,17 @@
     assert dictionary["test_bool"]
     assert dictionary["test_none"] == "None"
     assert dictionary["test_tuple"] == {'value': [12, 13, 14], 'type': 'tuple'}
     assert dictionary["test_list"] == [14, 13, 12]
     assert dictionary["test_set"] == {'value': [16, 12, 14], 'type': 'set'}
     assert dictionary["test_numpy"] == {'value': [15, 18, 16], 'type': 'np.ndarray'}
     assert dictionary["test_dictionary"] == {"a": 1, "b": 2}
-    assert dictionary["test_variable_class"] == {'k_s': 1, 'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
-                                                 '__name__': 'GroundConstantTemperature',
-                                                 'volumetric_heat_capacity': 2400000.0,
-                                                 'alpha': 4.1666666666666667e-07,
-                                                 'variable_Tg': False}
+    # assert dictionary["test_variable_class"] == {'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
+    #                                              '__name__': 'GroundConstantTemperature',
+    #                                              'variable_Tg': False}
     assert dictionary["test_pygfunction"] == {'value': [{'H': 100.0, 'D': 4.0, 'r_b': 0.075, 'x': 0.0, 'y': 0.0,
                                                         'tilt': 0.0, 'orientation': 3.141592653589793},
                                                        {'H': 100.0, 'D': 4.0, 'r_b': 0.075,
                                                         'x': 6.0, 'y': 0.0, 'tilt': 0.0, 'orientation': 0.0}],
                                               'type': 'pygfunction.Borehole'}
 
     test_class2 = TestClass()
@@ -113,19 +111,17 @@
     assert dictionary["test_bool"]
     assert dictionary["test_none"] == "None"
     assert dictionary["test_tuple"] == {'value': [12, 13, 14], 'type': 'tuple'}
     assert dictionary["test_list"] == [14, 13, 12]
     assert dictionary["test_set"] == {'value': [16, 12, 14], 'type': 'set'}
     assert dictionary["test_numpy"] == {'value': [15, 18, 16], 'type': 'np.ndarray'}
     assert dictionary["test_dictionary"] == {"a": 1, "b": 2}
-    assert dictionary["test_variable_class"] == {'k_s': 1, 'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
-                                                 '__name__': 'GroundConstantTemperature',
-                                                 'volumetric_heat_capacity': 2400000.0,
-                                                 'alpha': 4.1666666666666667e-07,
-                                                 'variable_Tg': False}
+    # assert dictionary["test_variable_class"] == {'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
+    #                                              '__name__': 'GroundConstantTemperature',
+    #                                              'variable_Tg': False}
     assert dictionary["test_pygfunction"] == {'value': [{'H': 100.0, 'D': 4.0, 'r_b': 0.075, 'x': 0.0, 'y': 0.0,
                                                         'tilt': 0.0, 'orientation': 3.141592653589793},
                                                        {'H': 100.0, 'D': 4.0, 'r_b': 0.075,
                                                         'x': 6.0, 'y': 0.0, 'tilt': 0.0, 'orientation': 0.0}], 'type': 'pygfunction.Borehole'}
 
 
 def test_with_slots():
@@ -137,19 +133,17 @@
     assert dictionary["test_bool"]
     assert dictionary["test_none"] == "None"
     assert dictionary["test_tuple"] == {'value': [12, 13, 14], 'type': 'tuple'}
     assert dictionary["test_list"] == [14, 13, 12]
     assert dictionary["test_set"] == {'value': [16, 12, 14], 'type': 'set'}
     assert dictionary["test_numpy"] == {'value': [15, 18, 16], 'type': 'np.ndarray'}
     assert dictionary["test_dictionary"] == {"a": 1, "b": 2}
-    assert dictionary["test_variable_class"] == {'k_s': 1, 'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
-                                                 '__name__': 'GroundConstantTemperature',
-                                                 'volumetric_heat_capacity': 2400000.0,
-                                                 'alpha': 4.1666666666666667e-07,
-                                                 'variable_Tg': False}
+    # assert dictionary["test_variable_class"] == {'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
+    #                                              '__name__': 'GroundConstantTemperature',
+    #                                              'variable_Tg': False}
     assert dictionary["test_pygfunction"] == {'value': [{'H': 100.0, 'D': 4.0, 'r_b': 0.075, 'x': 0.0, 'y': 0.0,
                                                         'tilt': 0.0, 'orientation': 3.141592653589793},
                                                        {'H': 100.0, 'D': 4.0, 'r_b': 0.075,
                                                         'x': 6.0, 'y': 0.0, 'tilt': 0.0, 'orientation': 0.0}], 'type': 'pygfunction.Borehole'}
 
     test_class2 = TestClassesWithSlots()
     test_class2.clear()
@@ -167,21 +161,19 @@
     assert dictionary["test_bool"]
     assert dictionary["test_none"] == "None"
     assert dictionary["test_tuple"] == {'value': [12, 13, 14], 'type': 'tuple'}
     assert dictionary["test_list"] == [14, 13, 12]
     assert dictionary["test_set"] == {'value': [16, 12, 14], 'type': 'set'}
     assert dictionary["test_numpy"] == {'value': [15, 18, 16], 'type': 'np.ndarray'}
     assert dictionary["test_dictionary"] == {"a": 1, "b": 2}
-    assert dictionary["test_variable_class"] == {'k_s': 1, 'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
-                                                 '__name__': 'GroundConstantTemperature',
-                                                 'volumetric_heat_capacity': 2400000.0,
-                                                 'alpha': 4.1666666666666667e-07,
-                                                 'variable_Tg': False}
+    # assert dictionary["test_variable_class"] == {'Tg': 2,'__module__': 'GHEtool.VariableClasses.GroundData.GroundConstantTemperature',
+    #                                              '__name__': 'GroundConstantTemperature',
+    #                                              'variable_Tg': False}
     assert dictionary["test_pygfunction"] == {'value': [{'H': 100.0, 'D': 4.0, 'r_b': 0.075, 'x': 0.0, 'y': 0.0,
                                                         'tilt': 0.0, 'orientation': 3.141592653589793},
                                                        {'H': 100.0, 'D': 4.0, 'r_b': 0.075,
                                                         'x': 6.0, 'y': 0.0, 'tilt': 0.0, 'orientation': 0.0}], 'type': 'pygfunction.Borehole'}
 
 
-def test_json_dump():
-    test_class = TestClass()
-    json.dump(test_class.to_dict(), open('test.json', 'w'))
+# def test_json_dump():
+#     test_class = TestClass()
+#     json.dump(test_class.to_dict(), open('test.json', 'w'))
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_borehole.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_borehole.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pygfunction as gt
 import numpy as np
 import pytest
 
 from GHEtool import FluidData, DoubleUTube, SingleUTube, MultipleUTube
 from GHEtool.VariableClasses import Borehole
 
+
 fluid_data = FluidData(0.2, 0.568, 998, 4180, 1e-3)
 pipe_data = DoubleUTube(1, 0.015, 0.02, 0.4, 0.05)
 
 
 def test_fluid_data_without_pipe():
     borehole = Borehole()
     assert borehole.fluid_data == FluidData()
@@ -97,20 +98,17 @@
     assert borehole.get_Rb(100, 1, 0.07, 2) == 0.12
     borehole.fluid_data = fluid_data
     assert np.isclose(borehole.calculate_Rb(100, 1, 0.075, 3), 0.09483159131195469)
 
 
 def test_calculate_Rb_no_data():
     borehole = Borehole()
-
-    try:
+    with pytest.raises(ValueError):
         borehole.calculate_Rb(100, 1, 0.075, 3)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
+
 
 def test_Rb_values():
     borehole = Borehole()
     mfr_range = np.arange(0.05, 0.55, 0.05)
     pipe_data = MultipleUTube(1, 0.015, 0.02, 0.4, 0.05, number_of_pipes=2, epsilon=1e-6)
     borehole.pipe_data = pipe_data
     Rb_list = []
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_calculation_setup.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_calculation_setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     assert test.L4_sizing
     assert not test.L3_sizing
     assert not test.L2_sizing
 
 
 def test_no_backup():
     test = CalculationSetup()
-    try:
+    with pytest.raises(ValueError):
         test.restore_backup()
-    except ValueError:
-        assert True
 
 
 def test_backup_functionality():
     test = CalculationSetup()
     test.make_backup()
     test.L3_sizing = True
     assert test.L2_sizing is False
@@ -50,49 +48,34 @@
     assert test.quadrant_sizing == 0
     test.update_variables(quadrant_sizing=1)
     assert test.quadrant_sizing == 1
 
 
 def test_more_than_one_option():
     test = CalculationSetup()
-    try:
+    with pytest.raises(ValueError):
         test._check_and_set_sizing(True, True, False)
-        assert False     # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         test._check_and_set_sizing(False, True, True)
-        assert False     # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         test._check_and_set_sizing(True, False, True)
-        assert False     # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_error_quadrant():
-    try:
+    with pytest.raises(ValueError):
         CalculationSetup(quadrant_sizing=5)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     CalculationSetup(quadrant_sizing=0)
 
 
 def test_equal_unequal():
     setup1 = CalculationSetup(2, False, True, False)
     setup2 = CalculationSetup(2, False, True, False)
     setup3 = CalculationSetup(2, True, False, False)
     assert setup1 == setup2
     assert not setup2 == setup3
     assert not setup2 == Borefield()
 
 
 def test_assign_incorrect_variable():
     setup = CalculationSetup()
-    try:
+    with pytest.raises(ValueError):
         setup.update_variables(test='test')
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_custom_gfunction.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_custom_gfunction.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_fluiddata.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_fluiddata.py`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_gfunction.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_gfunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,28 @@
     borefield2 = gt.boreholes.rectangle_field(10, 10, 6, 5, 100, 4, 0.075)
 
     gfunc = GFunction()
     gfunc.borefield = borefield1
     assert not gfunc._check_borefield(borefield2)
 
 
+def test_store_previous_values():
+    gfunc = GFunction()
+    assert gfunc.store_previous_values
+    assert gfunc._store_previous_values_backup
+
+    gfunc.store_previous_values = False
+    assert not gfunc.store_previous_values
+    assert not gfunc._store_previous_values_backup
+
+    gfunc._store_previous_values = True
+    assert gfunc.store_previous_values
+    assert not gfunc._store_previous_values_backup
+
+
 def test_equal_alpha():
     gfunc = GFunction()
     gfunc.alpha = 2
 
     assert gfunc._check_alpha(2)
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_hourly_load_data.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_hourly_load_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 import numpy as np
+import pandas as pd
 
 from GHEtool import FOLDER
 from GHEtool.VariableClasses import HourlyGeothermalLoad, HourlyGeothermalLoadMultiYear, MonthlyGeothermalLoadAbsolute
 from GHEtool.Validation.cases import load_case
 
 
 def test_load_hourly_data():
@@ -94,24 +95,53 @@
                           np.tile(np.linspace(50, 8759, 8760), load.simulation_period))
     assert np.array_equal(load.hourly_load_simulation_period,
                           np.tile(-np.linspace(0, 8759, 8760)+np.linspace(50, 8759, 8760), load.simulation_period))
 
 
 def test_set_hourly_values():
     load = HourlyGeothermalLoad()
-    try:
+    with pytest.raises(ValueError):
         load.set_hourly_heating(np.ones(10))
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.set_hourly_cooling(np.ones(10))
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
+
+
+def test_start_month_general():
+    load = HourlyGeothermalLoad()
+    assert load.start_month == 1
+    with pytest.raises(ValueError):
+        load.start_month = 1.5
+    with pytest.raises(ValueError):
+        load.start_month = 0
+    with pytest.raises(ValueError):
+        load.start_month = 13
+    load.start_month = 12
+    assert load.start_month == 12
+    assert load._start_hour == 11 * 730
+    load.start_month = 1
+    assert load.start_month == 1
+    assert load._start_hour == 0
+    load.start_month = 3
+    assert load.start_month == 3
+    assert load._start_hour == 730 * 2
+
+    load.all_months_equal = False
+    assert load._start_hour == 1416
+
+
+def test_different_start_month():
+    load = HourlyGeothermalLoad(np.arange(1, 8761, 1), np.arange(1, 8761, 1))
+    load.start_month = 3
+    assert load.start_month == 3
+    assert load.hourly_cooling_load[0] == 731 * 2 - 1
+    assert load.hourly_heating_load[0] == 731 * 2 - 1
+    load.all_months_equal = False
+    assert load.hourly_cooling_load[0] == 1417
+    assert load.hourly_heating_load[0] == 1417
+
 
 ### continue for multi year
 def test_checks_multiyear():
     load = HourlyGeothermalLoadMultiYear()
     assert not load._check_input(2)
     assert not load._check_input(np.ones(8759))
     assert not load._check_input(-1*np.ones(8760))
@@ -144,43 +174,59 @@
     assert load.imbalance == -78840
     load = HourlyGeothermalLoad(np.ones(8760), np.ones(8760)*10)
     assert load.imbalance == 78840
 
 
 def test_set_hourly_values_multi_year():
     load = HourlyGeothermalLoadMultiYear()
-    try:
+    with pytest.raises(ValueError):
         load.set_hourly_heating(np.ones(10))
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.set_hourly_cooling(np.ones(10))
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
+
+
+def test_monthly_based_on_hourly_multi_year():
+    load = HourlyGeothermalLoadMultiYear(heating_load=np.arange(0, 8760*2, 1),
+                                         cooling_load=np.arange(0, 8760*2, 1)*2)
+    heating = np.array([729, 1459, 2189, 2919, 3649, 4379, 5109, 5839, 6569, 7299, 8029, 8759, 9489,
+                        10219, 10949, 11679, 12409, 13139, 13869, 14599, 15329, 16059, 16789, 17519])
+    heating_bl = np.array([np.sum(np.arange(0, 8760*2, 1)[i-730:i]) for i in range(730, 8760*2+1, 730)])
+    assert np.allclose(load.peak_heating_simulation_period, heating)
+    assert np.allclose(load.peak_cooling_simulation_period, heating*2)
+    assert np.allclose(load.baseload_heating_simulation_period, heating_bl)
+    assert np.allclose(load.baseload_cooling_simulation_period, heating_bl * 2)
+    assert np.allclose(load.baseload_heating_power_simulation_period, heating_bl/730)
+    assert np.allclose(load.baseload_cooling_power_simulation_period, heating_bl * 2/730)
+    assert np.allclose(load.monthly_average_load_simulation_period, heating_bl/730)
+
+
+def test_resample_to_monthly_multiyear():
+    load = HourlyGeothermalLoadMultiYear()
+    load.simulation_period = 2
+    peak, baseload = load.resample_to_monthly(np.tile(np.linspace(0, 729, 730), 24))
+    assert np.array_equal(peak, np.full(24, 729))
+    assert np.array_equal(baseload, np.full(24, 266085))
+    load.all_months_equal = False
+    peak, baseload = load.resample_to_monthly(np.tile(np.linspace(0, 729, 730), 24))
+    assert np.array_equal(peak, np.tile(np.array([729., 685., 729., 729., 729., 729., 729., 729., 729., 729., 729., 729.]), 2))
+    assert np.array_equal(baseload, np.tile(np.array([266176., 234864., 275780., 259140., 275836., 259100.,
+                                              275892., 276088., 258920., 276144., 258880., 276200.]), 2))
 
 
 def test_dhw():
     load = HourlyGeothermalLoad()
     assert load.dhw == 0.
     load.add_dhw(1000)
     assert load.dhw == 1000.
     load.dhw = 200
     assert load.dhw == 200.
-    try:
+    with pytest.raises(ValueError):
         load.add_dhw('test')
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.add_dhw(-10)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
     load.dhw = 8760*10
     assert np.array_equal(np.full(12, 10), load.peak_heating)
     assert np.array_equal(np.full(8760, 10), load.hourly_heating_load)
     assert load.max_peak_heating == 10
     assert np.array_equal(np.full(8760, 10), load.hourly_heating_load)
     assert np.array_equal(np.full(12, 8760*10/12), load.baseload_heating)
@@ -245,19 +291,16 @@
                                   simulation_period=20,
                                   dhw=20000)
     load_2 = HourlyGeothermalLoad(cooling_load=np.arange(0, 8760, 1) + 1,
                                   heating_load=np.full(8760, 3),
                                   simulation_period=30,
                                   dhw=10000)
 
-    try:
+    with pytest.raises(TypeError):
         load_1 + 55
-        assert False  # pragma: no cover
-    except TypeError:
-        assert True
 
     with pytest.warns():
         result = load_1 + load_2
 
     assert result.simulation_period == 30
     assert result.dhw == 30000
     assert np.allclose(result.hourly_cooling_load, load_1.hourly_cooling_load + load_2.hourly_cooling_load)
@@ -266,15 +309,14 @@
     load_2.simulation_period = 20
     try:
         with pytest.warns():
             result = load_1 + load_2
         assert False  # pragma: no cover
     except:
         assert True
-
     assert result.simulation_period == 20
     assert result.dhw == 30000
     assert np.allclose(result.hourly_cooling_load, load_1.hourly_cooling_load + load_2.hourly_cooling_load)
     assert np.allclose(result.hourly_heating_load, load_1.hourly_heating_load + load_2.hourly_heating_load)
 
     # add with monthly load
     load_1 = MonthlyGeothermalLoadAbsolute(*load_case(2))
@@ -317,25 +359,19 @@
 
 def test_add_multiyear():
     load_1 = HourlyGeothermalLoadMultiYear(heating_load=np.arange(0, 8760, 1),
                                            cooling_load=np.full(8760, 2))
     load_2 = HourlyGeothermalLoadMultiYear(cooling_load=np.arange(0, 8760*2, 1) + 1,
                                            heating_load=np.full(8760*2, 3))
 
-    try:
+    with pytest.raises(TypeError):
         load_1 + 55
-        assert False  # pragma: no cover
-    except TypeError:
-        assert True
 
-    try:
+    with pytest.raises(ValueError):
         load_1 + load_2
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
     load_1 = HourlyGeothermalLoadMultiYear(heating_load=np.arange(0, 8760 * 2, 1),
                                            cooling_load=np.full(8760 * 2, 2))
 
     result = load_1 + load_2
 
     assert np.allclose(result._hourly_heating_load, load_1._hourly_heating_load + load_2._hourly_heating_load)
@@ -359,55 +395,9 @@
                    load_1._hourly_heating_load + np.tile(load_2._hourly_heating_load + load_2.dhw_power, load_1.simulation_period))
     assert np.allclose(result._hourly_cooling_load,
                    load_1._hourly_cooling_load + np.tile(load_2._hourly_cooling_load, load_1.simulation_period))
 
     # monthly load
     load_2 = MonthlyGeothermalLoadAbsolute(*load_case(1))
 
-    try:
+    with pytest.raises(TypeError):
         load_1 + load_2
-        assert False  # pragma: no cover
-    except TypeError:
-        assert True
-
-
-def test_start_month_general():
-    load = HourlyGeothermalLoad()
-    assert load.start_month == 1
-    try:
-        load.start_month = 1.5
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
-        load.start_month = 0
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
-        load.start_month = 13
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    load.start_month = 12
-    assert load.start_month == 12
-    assert load._start_hour == 11 * 730
-    load.start_month = 1
-    assert load.start_month == 1
-    assert load._start_hour == 0
-    load.start_month = 3
-    assert load.start_month == 3
-    assert load._start_hour == 730 * 2
-
-    load.all_months_equal = False
-    assert load._start_hour == 1416
-
-
-def test_different_start_month():
-    load = HourlyGeothermalLoad(np.arange(1, 8761, 1), np.arange(1, 8761, 1))
-    load.start_month = 3
-    assert load.start_month == 3
-    assert load.hourly_cooling_load[0] == 731 * 2 - 1
-    assert load.hourly_heating_load[0] == 731 * 2 - 1
-    load.all_months_equal = False
-    assert load.hourly_cooling_load[0] == 1417
-    assert load.hourly_heating_load[0] == 1417
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_main_class.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_main_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,43 +8,44 @@
 
 from GHEtool import GroundConstantTemperature, GroundFluxTemperature, FluidData, DoubleUTube, Borefield, CalculationSetup, FOLDER, MultipleUTube
 from GHEtool.logger import ghe_logger
 from GHEtool.Validation.cases import load_case
 from GHEtool.VariableClasses.LoadData import MonthlyGeothermalLoadAbsolute, HourlyGeothermalLoad
 from GHEtool.VariableClasses.BaseClass import UnsolvableDueToTemperatureGradient
 
+
 data = GroundConstantTemperature(3, 10)
 ground_data_constant = data
 data_ground_flux = GroundFluxTemperature(3, 10)
 fluidData = FluidData(0.2, 0.568, 998, 4180, 1e-3)
 pipeData = DoubleUTube(1, 0.015, 0.02, 0.4, 0.05)
 
 borefield_gt = gt.boreholes.rectangle_field(10, 12, 6, 6, 110, 4, 0.075)
 
 # Monthly loading values
-peakCooling = [0., 0, 34., 69., 133., 187., 213., 240., 160., 37., 0., 0.]              # Peak cooling in kW
-peakHeating = [160., 142, 102., 55., 0., 0., 0., 0., 40.4, 85., 119., 136.]             # Peak heating in kW
+peakCooling = [0.0, 0, 34.0, 69.0, 133.0, 187.0, 213.0, 240.0, 160.0, 37.0, 0.0, 0.0]  # Peak cooling in kW
+peakHeating = [160.0, 142, 102.0, 55.0, 0.0, 0.0, 0.0, 0.0, 40.4, 85.0, 119.0, 136.0]  # Peak heating in kW
 
 # annual heating and cooling load
-annualHeatingLoad = 300*10**3  # kWh
-annualCoolingLoad = 160*10**3  # kWh
+annualHeatingLoad = 300 * 10**3  # kWh
+annualCoolingLoad = 160 * 10**3  # kWh
 
 # percentage of annual load per month (15.5% for January ...)
-monthlyLoadHeatingPercentage = [0.155, 0.148, 0.125, .099, .064, 0., 0., 0., 0.061, 0.087, 0.117, 0.144]
-monthlyLoadCoolingPercentage = [0.025, 0.05, 0.05, .05, .075, .1, .2, .2, .1, .075, .05, .025]
+monthlyLoadHeatingPercentage = [0.155, 0.148, 0.125, 0.099, 0.064, 0.0, 0.0, 0.0, 0.061, 0.087, 0.117, 0.144]
+monthlyLoadCoolingPercentage = [0.025, 0.05, 0.05, 0.05, 0.075, 0.1, 0.2, 0.2, 0.1, 0.075, 0.05, 0.025]
 
 # resulting load per month
-monthlyLoadHeating = list(map(lambda x: x * annualHeatingLoad, monthlyLoadHeatingPercentage))   # kWh
-monthlyLoadCooling = list(map(lambda x: x * annualCoolingLoad, monthlyLoadCoolingPercentage))   # kWh
+monthlyLoadHeating = list(map(lambda x: x * annualHeatingLoad, monthlyLoadHeatingPercentage))  # kWh
+monthlyLoadCooling = list(map(lambda x: x * annualCoolingLoad, monthlyLoadCoolingPercentage))  # kWh
 
 
 def borefields_equal(borefield_one, borefield_two) -> bool:
     for i in range(len(borefield_one)):
         if borefield_one[i].__dict__ != borefield_two[i].__dict__:
-            return False   # pragma: no cover
+            return False  # pragma: no cover
     return True
 
 
 def test_set_investment_cost():
     borefield = Borefield()
     borefield.set_investment_cost()
     assert borefield.cost_investment == Borefield.DEFAULT_INVESTMENT
@@ -64,25 +65,25 @@
 def test_nb_of_boreholes():
     borefield = Borefield()
     assert borefield.number_of_boreholes == 0
     borefield = Borefield(borefield=copy.deepcopy(borefield_gt))
     borefield.set_ground_parameters(data_ground_flux)
     assert borefield.number_of_boreholes == 120
     borefield.set_borefield(gt.boreholes.rectangle_field(5, 5, 6, 6, 110, 0.1, 0.07))
-    assert borefield.H == 110
-    assert borefield.r_b == 0.07
-    assert borefield.D == 0.1
+    assert np.isclose(borefield.H, 110)
+    assert np.isclose(borefield.r_b, 0.07)
+    assert np.isclose(borefield.D, 0.1)
     assert borefield.number_of_boreholes == 25
     borefield.gfunction(5000, 110)
     assert np.any(borefield.gfunction_calculation_object.depth_array)
     borefield.borefield = gt.boreholes.rectangle_field(6, 5, 6, 6, 100, 1, 0.075)
     assert not np.any(borefield.gfunction_calculation_object.depth_array)
-    assert borefield.H == 100
-    assert borefield.r_b == 0.075
-    assert borefield.D == 1
+    assert np.isclose(borefield.H, 100)
+    assert np.isclose(borefield.r_b, 0.075)
+    assert np.isclose(borefield.D, 1)
     borefield.gfunction(5000, 110)
     assert np.any(borefield.gfunction_calculation_object.depth_array)
     assert borefield.number_of_boreholes == 30
     borefield.borefield = None
     assert not np.any(borefield.gfunction_calculation_object.depth_array)
     assert borefield.gfunction_calculation_object
     assert borefield.number_of_boreholes == 0
@@ -90,60 +91,102 @@
     borefield.gfunction(5000, 110)
     assert np.any(borefield.gfunction_calculation_object.depth_array)
     borefield.set_borefield(None)
     assert not np.any(borefield.gfunction_calculation_object.depth_array)
     assert borefield.number_of_boreholes == 0
 
 
+def test_set_borefield():
+    borefield = Borefield()
+    borefield.set_borefield([
+        gt.boreholes.Borehole(100, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(150, 4, 0.075, 10, 0)
+    ])
+    assert borefield.H == 125
+
+
+def test_gfunction_with_irregular_borehole_depth():
+    borefield = Borefield()
+    borefield.ground_data = ground_data_constant
+    borefield.set_borefield([
+        gt.boreholes.Borehole(150, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(100, 4, 0.075, 10, 0)
+    ])
+    borehole_irr = borefield.gfunction([3600, 3600 * 20, 3600 * 800])
+    borefield.set_borefield([
+        gt.boreholes.Borehole(125, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(125, 4, 0.075, 10, 0)
+    ])
+    borehole_reg = borefield.gfunction([3600, 3600 * 20, 3600 * 800])
+
+    # the gfunctions for those two classes should not be equal
+    assert not np.array_equal(borehole_irr, borehole_reg)
+
+
 def test_create_rectangular_field():
     borefield = Borefield()
     borefield.create_rectangular_borefield(10, 10, 6, 6, 110, 4, 0.075)
     assert borefield.number_of_boreholes == 100
     borefields_equal(borefield.borefield, gt.boreholes.rectangle_field(10, 10, 6, 6, 110, 4, 0.075))
 
 
 def test_create_circular_field():
     borefield = Borefield()
     borefield.create_circular_borefield(10, 10, 100, 1)
     assert borefield.number_of_boreholes == 10
     borefields_equal(borefield.borefield, gt.boreholes.circle_field(10, 10, 100, 1, 0.075))
 
 
+def test_create_U_shaped_field():
+    borefield = Borefield()
+    borefield.create_U_shaped_borefield(10, 9, 6, 6, 110, 4, 0.075)
+    assert borefield.number_of_boreholes == 9*2+(10-2)
+    borefields_equal(borefield.borefield, gt.boreholes.U_shaped_field(10, 10, 6, 6, 110, 4, 0.075))
+
+
+def test_create_L_shaped_field():
+    borefield = Borefield()
+    borefield.create_L_shaped_borefield(10, 9, 6, 6, 110, 4, 0.075)
+    assert borefield.number_of_boreholes == 10 + 8
+    borefields_equal(borefield.borefield, gt.boreholes.L_shaped_field(10, 10, 6, 6, 110, 4, 0.075))
+
+
+def test_create_box_shaped_field():
+    borefield = Borefield()
+    borefield.create_box_shaped_borefield(10, 8, 6, 6, 110, 4, 0.075)
+    assert borefield.number_of_boreholes == 10*2 + (8-2)*2
+    borefields_equal(borefield.borefield, gt.boreholes.box_shaped_field(10, 10, 6, 6, 110, 4, 0.075))
+
+
 def test_update_depth():
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     init_H = borefield.borefield[0].H
 
     borefield.H = init_H + 1
-    borefield._update_borefield_depth()
+    borefield._update_borefield_depth(20)
     for bor in borefield.borefield:
-        assert bor.H == init_H + 1
+        assert bor.H == 20
 
     borefield._update_borefield_depth(init_H + 2)
     for bor in borefield.borefield:
         assert bor.H == init_H + 2
 
     borefield._update_borefield_depth(init_H + 2)
     for bor in borefield.borefield:
         assert bor.H == init_H + 2
 
 
 def test_create_custom_dataset():
     borefield_test = Borefield()
-    try:
+    with pytest.raises(ValueError):
         borefield_test.create_custom_dataset([100, 1000], [50, 100])
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     borefield_test.create_rectangular_borefield(10, 10, 6, 6, 100, 1, 0.075)
-    try:
+    with pytest.raises(AssertionError):
         borefield_test.create_custom_dataset([100, 1000], [50, 100])
-        assert False  # pragma: no cover
-    except AssertionError:
-        assert True
 
 
 def test_load_custom_gfunction():
     borefield = Borefield()
     borefield.set_ground_parameters(ground_data_constant)
     borefield.borefield = copy.deepcopy(borefield_gt)
     borefield.create_custom_dataset()
@@ -154,25 +197,14 @@
     borefield.custom_gfunction = dataset
     borefield.set_borefield(None)
     assert borefield.custom_gfunction is None
     borefield.load_custom_gfunction("./test.gvalues")
     assert borefield.custom_gfunction == dataset
 
 
-def test_set_length_peak():
-    borefield = Borefield()
-    borefield.load.peak_heating_duration = 8
-    borefield.load.peak_cooling_duration = 10
-    assert borefield.load.peak_cooling_duration == 10 * 3600
-    assert borefield.load.peak_heating_duration == 8 * 3600
-    borefield.set_length_peak(12)
-    assert borefield.load.peak_cooling_duration == 12 * 3600
-    assert borefield.load.peak_heating_duration == 12 * 3600
-
-
 def test_simulation_period():
     borefield = Borefield()
     assert borefield.simulation_period == 20
     assert len(borefield.load.time_L3) == 12 * 20
     borefield.simulation_period = 25
     assert borefield.simulation_period == 25
     assert len(borefield.load.time_L3) == 12 * 25
@@ -263,75 +295,78 @@
 
 def test_set_max_temp():
     borefield = Borefield()
     borefield.set_max_avg_fluid_temperature(13)
     assert borefield.Tf_max == 13
     borefield.set_max_avg_fluid_temperature(14)
     assert borefield.Tf_max == 14
-    try:
+    with pytest.raises(ValueError):
         borefield.set_max_avg_fluid_temperature(borefield.Tf_min - 1)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_set_min_temp():
     borefield = Borefield()
     borefield.set_min_avg_fluid_temperature(3)
     assert borefield.Tf_min == 3
     borefield.set_min_avg_fluid_temperature(4)
     assert borefield.Tf_min == 4
-    try:
+    with pytest.raises(ValueError):
         borefield.set_min_avg_fluid_temperature(borefield.Tf_max + 1)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_Tg():
     borefield = Borefield()
     borefield.set_ground_parameters(ground_data_constant)
     assert borefield._Tg() == borefield.ground_data.calculate_Tg(borefield.H)
     assert borefield._Tg(20) == borefield.ground_data.calculate_Tg(20)
     borefield.set_ground_parameters(data_ground_flux)
     assert borefield._Tg() == borefield.ground_data.calculate_Tg(borefield.H)
     assert borefield._Tg(20) == borefield.ground_data.calculate_Tg(20)
 
 
-@pytest.mark.parametrize("ground_data, constant_Rb, result",
-                         zip([ground_data_constant, data_ground_flux, ground_data_constant, data_ground_flux],
-                             [True, True, False, False],
-                             [39.994203323480214, 38.70946566704161, 30.924434615896764, 30.245606119498383]))
+@pytest.mark.parametrize(
+    "ground_data, constant_Rb, result",
+    zip(
+        [ground_data_constant, data_ground_flux, ground_data_constant, data_ground_flux],
+        [True, True, False, False],
+        [39.994203323480214, 38.70946566704161, 30.924434615896764, 30.245606119498383],
+    ),
+)
 def test_Ahmadfard(ground_data, constant_Rb, result):
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     load = MonthlyGeothermalLoadAbsolute(*load_case(3))
     borefield.set_ground_parameters(ground_data)
     borefield.set_fluid_parameters(fluidData)
     borefield.set_pipe_parameters(pipeData)
     borefield.calculation_setup(use_constant_Rb=constant_Rb)
     th, qh, qm, qa = load._calculate_last_year_params(True)
-    assert np.isclose(result, borefield._Ahmadfard(th, qh, qm, qa))
+    assert np.isclose(result, borefield._Ahmadfard(th, qh, qm, qa, 0))
     assert np.isclose(result, borefield.H)
 
-@pytest.mark.parametrize("ground_data, constant_Rb, result",
-                         zip([ground_data_constant, data_ground_flux, ground_data_constant, data_ground_flux],
-                             [True, True, False, False],
-                             [48.76844845370183, 46.593433439950985, 38.53491016745154, 37.100782551185]))
+
+@pytest.mark.parametrize(
+    "ground_data, constant_Rb, result",
+    zip(
+        [ground_data_constant, data_ground_flux, ground_data_constant, data_ground_flux],
+        [True, True, False, False],
+        [48.76844845370183, 46.593433439950985, 38.53491016745154, 37.100782551185],
+    ),
+)
 def test_Carcel(ground_data, constant_Rb, result):
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     load = MonthlyGeothermalLoadAbsolute(*load_case(3))
 
     borefield.set_ground_parameters(ground_data)
     borefield.set_fluid_parameters(fluidData)
     borefield.set_pipe_parameters(pipeData)
     borefield.calculation_setup(use_constant_Rb=constant_Rb)
     th, _, tcm, qh, qpm, qm = load._calculate_first_year_params(True)
-    assert np.isclose(result, borefield._Carcel(th, tcm, qh, qpm, qm))
+    assert np.isclose(result, borefield._Carcel(th, tcm, qh, qpm, qm, 0))
     assert np.isclose(result, borefield.H)
 
 
 def test_set_sizing_setup():
     borefield = Borefield()
     sizing_setup_backup = copy.deepcopy(borefield._calculation_setup)
     borefield.calculation_setup()
@@ -349,19 +384,16 @@
     borefield.calculation_setup(atol=10)
     assert borefield._calculation_setup.atol == 10
     assert borefield._calculation_setup.rtol == 10
 
 
 def test_size():
     borefield = Borefield()
-    try:
+    with pytest.raises(ValueError):
         borefield.size()
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     borefield.borefield = copy.deepcopy(borefield_gt)
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(3))
 
     borefield.set_ground_parameters(ground_data_constant)
     sizing_setup_backup = copy.deepcopy(borefield._calculation_setup)
     borefield.size(L3_sizing=True)
     assert borefield._calculation_setup == sizing_setup_backup
@@ -378,99 +410,74 @@
     assert borefield._select_size(10, 20) == 20
 
     # with variable Tg
     borefield.set_ground_parameters(data_ground_flux)
     assert borefield._select_size(100, 20) == 100
     assert borefield._select_size(10, 80) == 80
     borefield.set_max_avg_fluid_temperature(14)
-    try:
+    with pytest.raises(UnsolvableDueToTemperatureGradient):
         borefield._select_size(10, 80)
-        assert False  # pragma: no cover
-    except UnsolvableDueToTemperatureGradient:
-        assert True
 
 
 def test_size_L2_value_errors():
     borefield = Borefield()
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L2(100)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.load = load
     borefield.set_ground_parameters(ground_data_constant)
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L2(100, 5)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
-@pytest.mark.parametrize("quadrant, result",
-                         zip([1, 2, 3, 4], [74.55862437702756, 96.85342542746277, 27.2041541800546, 21.903857780936665]))
+@pytest.mark.parametrize("quadrant, result", zip([1, 2, 3, 4], [74.55862437702756, 96.85342542746277, 27.2041541800546, 21.903857780936665]))
 def test_size_L2(quadrant, result):
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.set_ground_parameters(ground_data_constant)
     borefield.size_L2(100, quadrant_sizing=quadrant)
 
     assert np.isclose(result, borefield.size_L2(100, quadrant_sizing=quadrant))
     assert borefield.limiting_quadrant == quadrant
     assert np.isclose(result, borefield.H)
 
 
 def test_size_L3_value_errors():
     borefield = Borefield()
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L3(100)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.set_ground_parameters(ground_data_constant)
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L3(100, 5)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
-@pytest.mark.parametrize("quadrant, result",
-                         zip([1, 2, 3, 4], [56.37136629360852, 71.42698877336204, 26.722846792067735, 21.333161686968708]))
+
+@pytest.mark.parametrize("quadrant, result", zip([1, 2, 3, 4], [56.37136629360852, 71.42698877336204, 26.722846792067735, 21.333161686968708]))
 def test_size_L3(quadrant, result):
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     borefield.set_max_avg_fluid_temperature(18)
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.set_ground_parameters(ground_data_constant)
 
     assert np.isclose(result, borefield.size_L3(100, quadrant_sizing=quadrant))
     assert np.isclose(result, borefield.H)
 
 
 def test_size_L4_value_errors():
     borefield = Borefield()
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L4(100)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.set_ground_parameters(ground_data_constant)
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L4(100, 5)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         borefield.size_L4(100)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_size_L4():
     borefield = Borefield()
     borefield.set_ground_parameters(ground_data_constant)
     load = HourlyGeothermalLoad()
     # quadrant 1
@@ -586,36 +593,36 @@
         8.88514083,  9.39208797, 10.00668693, 10.68670226, 11.11560581,
        11.61858065, 11.74854509, 10.79725993, 10.08666356,  9.4767217 ,
         9.05938796,  8.66528206,  8.94801036,  9.45402141, 10.06849598,
        10.74924083, 11.1804467 , 11.68421179, 11.81471642, 10.8636843 ,
        10.15255075,  9.54096457,  9.12037341,  8.72303207,  9.00480061,
         9.51054181, 10.12547914, 10.80869029, 11.24107298, 11.74562143,
        11.87654742, 10.92504277, 10.21207583,  9.59666225,  9.17178911,
-        8.77253798,  9.0537501 ,  9.55988622, 10.17614817, 10.85968208,
+        8.77253798,  9.0537501,  9.55988622, 10.17614817, 10.85968208,
        11.29206477, 11.79661323, 11.92753922, 10.97603456, 10.26306763,
-        9.64765405,  9.2227809 ,  8.82352977,  9.1047419 ,  9.61146373,
-       10.22920734, 10.91368494, 11.34666291, 11.85119791, 11.9809148 ,
-       11.02648776, 10.30917151,  9.69046041,  9.2646135 ,  8.86532916,
+        9.64765405,  9.2227809,  8.82352977,  9.1047419,  9.61146373,
+       10.22920734, 10.91368494, 11.34666291, 11.85119791, 11.9809148,
+       11.02648776, 10.30917151,  9.69046041,  9.2646135,  8.86532916,
         9.14747171,  9.65520666, 10.27295028, 10.95742787, 11.39040584,
        11.89494084, 12.02465773, 11.07023069, 10.35291444,  9.73420334,
         9.30835643,  8.90907209,  9.19243444,  9.70106276, 10.31940964,
        11.00419406, 11.43669622, 11.93961809, 12.06604757, 11.10816011,
-       10.38957388,  9.7704954 ,  9.3450551 ,  8.9469248 ,  9.23041   ,
-        9.73903832, 10.3573852 , 11.04216962, 11.47467178, 11.97759365,
+       10.38957388,  9.7704954,  9.3450551,  8.9469248,  9.23041,
+        9.73903832, 10.3573852, 11.04216962, 11.47467178, 11.97759365,
        12.10402313, 11.14613567, 10.42754944,  9.80847096,  9.38353452,
         8.98631798,  9.27039079,  9.77937765, 10.39763925, 11.08153248,
        11.51198131, 12.01208298, 12.13659709, 11.17814528, 10.45960879,
         9.84120172,  9.41680976,  9.01959321,  9.30366603,  9.81265289,
        10.43091449, 11.11480772, 11.54525655, 12.04535822, 12.16987233,
-       11.21142051, 10.49289526,  9.87539571,  9.451568  ,  9.05473695,
+       11.21142051, 10.49289526,  9.87539571,  9.451568,  9.05473695,
         9.33898907,  9.84758987, 10.46467316, 11.14623848, 11.57437959,
        12.07379672, 12.19811941, 11.23999967, 10.52229065,  9.90479109,
         9.48096338,  9.08413234,  9.36838445,  9.87698525, 10.49406855,
-       11.17563386, 11.60377497, 12.1031921 , 12.2275148 , 11.27004561,
-       10.55323455,  9.93631861,  9.51283391,  9.1158352 ,  9.39905299,
+       11.17563386, 11.60377497, 12.1031921, 12.2275148, 11.27004561,
+       10.55323455,  9.93631861,  9.51283391,  9.1158352,  9.39905299,
         9.90536243, 10.51952398, 11.19933578, 11.62696168, 12.12650419,
        12.25159304, 11.29457142, 10.57776036,  9.96084442,  9.53735972]))
     np.testing.assert_array_almost_equal(borefield.results.peak_cooling,
                                          np.array([ 9.7265228 ,  9.87217467, 10.134688  , 10.63927884, 11.62475183,
        12.59873554, 13.28921831, 13.76520367, 12.39881805, 10.70464274,
        10.2834413 , 10.00058989,  9.91555149, 10.05871306, 10.31805035,
        10.81905145, 11.80062228, 12.77154188, 13.45848569, 13.93085698,
@@ -771,147 +778,233 @@
 
 
 def test_gfunction():
     borefield = Borefield()
     borefield.set_ground_parameters(data_ground_flux)
     borefield.create_rectangular_borefield(10, 10, 6, 6, 100, 1, 0.075)
     borefield.H = 100_000
-    try:
+    with pytest.raises(UnsolvableDueToTemperatureGradient):
         borefield.gfunction(56491)
-        assert False  # pragma: no cover
-    except UnsolvableDueToTemperatureGradient:
-        assert True
     borefield.H = 102.3
 
     np.testing.assert_array_almost_equal(borefield.gfunction([6000, 60000, 600000]), np.array([0.63751082, 1.70657847, 2.84227252]))
     borefield.create_custom_dataset()
     np.testing.assert_array_almost_equal(borefield.gfunction([6000, 60000, 600000]), np.array([0.622017, 1.703272, 2.840246]))
     borefield.calculation_setup(use_precalculated_dataset=False)
     np.testing.assert_array_almost_equal(borefield.gfunction([6000, 60000, 600000]), np.array([0.63751082, 1.70657847, 2.84227252]))
 
 
+def test_gfunction_with_irregular_depth():
+    borefield = Borefield()
+    borefield.set_ground_parameters(data_ground_flux)
+    temp = [
+        gt.boreholes.Borehole(100, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(150, 4, 0.075, 10, 0),
+        gt.boreholes.Borehole(50, 4, 0.075, 100, 0)
+    ]
+    borefield.borefield = temp
+    assert borefield.H == 100
+    g_values = borefield.gfunction([6000, 60000, 600000])
+    borefield._update_borefield_depth(100)
+    assert not np.array_equal(borefield.gfunction([6000, 60000, 600000]), g_values)
+
+    borefield = Borefield()
+    borefield.set_ground_parameters(data_ground_flux)
+    temp = [
+        gt.boreholes.Borehole(100, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(150, 4, 0.075, 10, 0),
+        gt.boreholes.Borehole(50, 4, 0.075, 100, 0)
+    ]
+    borefield.borefield = temp
+    assert borefield.H == 100
+    temp = [
+        gt.boreholes.Borehole(100, 4, 0.075, 0, 0),
+        gt.boreholes.Borehole(100, 4, 0.075, 10, 0),
+        gt.boreholes.Borehole(100, 4, 0.075, 100, 0)
+    ]
+    borefield.borefield = temp
+    assert not np.array_equal(borefield.gfunction([6000, 60000, 600000]), g_values)
+
+
 def test_load_duration(monkeypatch):
     borefield = Borefield()
-    monkeypatch.setattr(plt, 'show', lambda: None)
+    monkeypatch.setattr(plt, "show", lambda: None)
     borefield.set_ground_parameters(ground_data_constant)
     borefield.borefield = copy.deepcopy(borefield_gt)
     load = HourlyGeothermalLoad()
     load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
     borefield.load = load
     borefield.plot_load_duration(legend=True)
-    borefield.optimise_load_profile(load, 150)
+    borefield.optimise_load_profile_power(load, 150)
+    borefield.optimise_load_profile_energy(load, 150)
 
 
-def test_optimise_load_profile(monkeypatch):
+def test_optimise_load_profile_power(monkeypatch):
     borefield = Borefield()
-    monkeypatch.setattr(plt, 'show', lambda: None)
+    monkeypatch.setattr(plt, "show", lambda: None)
     borefield.set_ground_parameters(ground_data_constant)
     borefield.borefield = copy.deepcopy(borefield_gt)
     load = HourlyGeothermalLoad()
     load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
     load.simulation_period = 40
-    borefield.optimise_load_profile(load, 150)
+    borefield.optimise_load_profile_power(load, 150)
     assert borefield.load.simulation_period == 40
     assert borefield._building_load.simulation_period == 40
     assert borefield._secundary_borefield_load.simulation_period == 40
     assert borefield._external_load.simulation_period == 40
 
 
-def test_optimise_borefield_small(monkeypatch):
+def test_optimise_load_profile_energy(monkeypatch):
     borefield = Borefield()
-    monkeypatch.setattr(plt, 'show', lambda: None)
+    monkeypatch.setattr(plt, "show", lambda: None)
+    borefield.set_ground_parameters(ground_data_constant)
+    borefield.borefield = copy.deepcopy(borefield_gt)
+    load = HourlyGeothermalLoad()
+    load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
+    load.simulation_period = 40
+    borefield.optimise_load_profile_energy(load, 150)
+    assert borefield.load.simulation_period == 40
+    assert borefield._building_load.simulation_period == 40
+    assert borefield._secundary_borefield_load.simulation_period == 40
+    assert borefield._external_load.simulation_period == 40
+
+
+def test_optimise_borefield_small_power(monkeypatch):
+    borefield = Borefield()
+    monkeypatch.setattr(plt, "show", lambda: None)
+    borefield.set_ground_parameters(ground_data_constant)
+    borefield.create_rectangular_borefield(5, 1, 6, 6, 100)
+    load = HourlyGeothermalLoad()
+    load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
+    load.simulation_period = 40
+    borefield.optimise_load_profile_power(load, 150)
+    assert borefield.load.simulation_period == 40
+    assert borefield._building_load.simulation_period == 40
+    assert borefield._secundary_borefield_load.simulation_period == 40
+    assert borefield._external_load.simulation_period == 40
+
+
+def test_optimise_borefield_small_energy(monkeypatch):
+    borefield = Borefield()
+    monkeypatch.setattr(plt, "show", lambda: None)
     borefield.set_ground_parameters(ground_data_constant)
     borefield.create_rectangular_borefield(5, 1, 6, 6, 100)
     load = HourlyGeothermalLoad()
     load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
     load.simulation_period = 40
-    borefield.optimise_load_profile(load, 150, print_results=True)
+    borefield.optimise_load_profile_energy(load, 150)
     assert borefield.load.simulation_period == 40
     assert borefield._building_load.simulation_period == 40
     assert borefield._secundary_borefield_load.simulation_period == 40
     assert borefield._external_load.simulation_period == 40
 
 
-def test_optimise_borefield_wrong_threshold(monkeypatch):
+def test_optimise_borefield_wrong_threshold_power(monkeypatch):
+    borefield = Borefield()
+    monkeypatch.setattr(plt, "show", lambda: None)
+    borefield.set_ground_parameters(ground_data_constant)
+    borefield.create_rectangular_borefield(5, 1, 6, 6, 100)
+    load = HourlyGeothermalLoad()
+    load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
+    load.simulation_period = 40
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_power(load, 150, temperature_threshold=-0.5)
+
+
+def test_optimise_borefield_wrong_threshold_energy(monkeypatch):
     borefield = Borefield()
-    monkeypatch.setattr(plt, 'show', lambda: None)
+    monkeypatch.setattr(plt, "show", lambda: None)
     borefield.set_ground_parameters(ground_data_constant)
     borefield.create_rectangular_borefield(5, 1, 6, 6, 100)
     load = HourlyGeothermalLoad()
     load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
     load.simulation_period = 40
-    try:
-        borefield.optimise_load_profile(load, 150, print_results=True, temperature_threshold=-0.5)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_energy(load, 150, temperature_threshold=-0.5)
+
 
 def test_calculate_quadrants_without_data():
     borefield = Borefield()
     borefield.borefield = copy.deepcopy(borefield_gt)
     borefield.set_max_avg_fluid_temperature(18)
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     borefield.set_ground_parameters(ground_data_constant)
     borefield.calculate_quadrant()
 
 
-def test_optimise_load_profile_without_data():
+def test_optimise_load_profile_power_without_data():
     borefield = Borefield()
-    try:
-        borefield.optimise_load_profile(MonthlyGeothermalLoadAbsolute())
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_power(MonthlyGeothermalLoadAbsolute())
+
+
+def test_optimise_load_profile_energy_without_data():
+    borefield = Borefield()
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_energy(MonthlyGeothermalLoadAbsolute())
 
 
 def test_load_load():
     borefield1 = Borefield()
     borefield2 = Borefield()
 
     load = MonthlyGeothermalLoadAbsolute(*load_case(1))
     borefield2.load = load
     borefield1.set_load(load)
     assert borefield1.load is borefield2.load
 
 
 def test_calculate_temperature_profile():
     borefield = Borefield()
+    borefield.set_ground_parameters(ground_data_constant)
     load = MonthlyGeothermalLoadAbsolute(*load_case(1))
     borefield.load = load
-
-    try:
+    with pytest.raises(ValueError):
         borefield.calculate_temperatures(hourly=True)
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
 
 
-def test_optimise_load_profile_without_hourly_data():
+def test_optimise_load_profile_power_without_hourly_data():
     borefield = Borefield()
     borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(1))
-    try:
-        borefield.optimise_load_profile(borefield.load)
-        assert False   # pragma: no cover
-    except ValueError:
-        assert True
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_power(borefield.load)
     borefield.load = HourlyGeothermalLoad()
     borefield.set_ground_parameters(ground_data_constant)
     borefield.load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
     borefield.create_rectangular_borefield(10, 10, 6, 6, 150)
-    borefield.optimise_load_profile(borefield.load)
+    borefield.optimise_load_profile_power(borefield.load)
+
+
+def test_optimise_load_profile_energy_without_hourly_data():
+    borefield = Borefield()
+    borefield.load = MonthlyGeothermalLoadAbsolute(*load_case(1))
+    with pytest.raises(ValueError):
+        borefield.optimise_load_profile_energy(borefield.load)
+    borefield.load = HourlyGeothermalLoad()
+    borefield.set_ground_parameters(ground_data_constant)
+    borefield.load.load_hourly_profile(FOLDER.joinpath("Examples/hourly_profile.csv"))
+    borefield.create_rectangular_borefield(10, 10, 6, 6, 150)
+    borefield.optimise_load_profile_energy(borefield.load)
+
+
+@pytest.mark.parametrize(
+    "H, result",
+    zip(
+        range(110, 130, 1),
+        [
+            122.99210426454648, 122.99135446500962, 122.99135409065917, 122.99135403971272,
+            122.99135403719148, 122.9913540367823,  122.99135403674013, 122.99135403673134,
+            122.99221686744185, 122.99217229220649, 122.99135553171544, 122.99220727438545,
+            122.99477143007601, 122.9921794642058,  122.99220615327106, 122.99221262582992,
+            122.99221900364599, 122.9922252887964,  122.99223148329897, 122.99223758911434,
+        ],
+    ),
+)
 
 
-@pytest.mark.parametrize("H, result",
-                         zip(range(110, 130, 1), [122.99210426454648, 122.99135446500962, 122.99135409065917,
-                                                  122.99135403971272, 122.99135403719148, 122.9913540367823,
-                                                  122.99135403674013, 122.99135403673134, 122.99221686744185,
-                                                  122.99217229220649, 122.99135553171544, 122.99220727438545,
-                                                  122.99477143007601, 122.9921794642058, 122.99220615327106,
-                                                  122.99221262582992, 122.99221900364599, 122.9922252887964,
-                                                  122.99223148329897, 122.99223758911434]))
 def test_effect_H_init(H, result):
     borefield = Borefield()
     borefield.ground_data = GroundConstantTemperature(3, 11)
     borefield.create_rectangular_borefield(10, 5, 7, 7, 100, 0.75)
     load = MonthlyGeothermalLoadAbsolute(*load_case(1))
     borefield.load = load
     borefield.calculation_setup(H_init=H)
@@ -923,19 +1016,16 @@
     borefield.load = load
     assert np.isclose(borefield.size(H_init=H), result)
 
 
 def test_depth_convergence():
     borefield = Borefield()
     borefield.calculation_setup(atol=1, rtol=0.01, max_nb_of_iterations=10)
-    try:
+    with pytest.raises(RuntimeError):
         borefield._check_convergence(10, 12, 10)
-        assert False  # pragma: no cover
-    except RuntimeError:
-        assert True
 
     assert borefield._check_convergence(10, 10, 1)
     assert not borefield._check_convergence(10, 10.5, 1)
     assert borefield._check_convergence(10, 10.001, 1)
     assert not borefield._check_convergence(10000, 10002, 1)
 
 
@@ -950,17 +1040,15 @@
     assert np.isclose(borefield.calculate_next_depth_deep_sizing(75), 117.98660599828808)
     borefield.calculate_temperatures(117.98660599828808)
     assert np.isclose(borefield.calculate_next_depth_deep_sizing(117.98660599828808), 128.16618036528823)
     borefield.calculate_temperatures(128.16618036528823)
     assert np.isclose(borefield.calculate_next_depth_deep_sizing(128.16618036528823), 130.8812255630479)
 
 
-@pytest.mark.parametrize("case, result",
-                         zip((1, 2, 3, 4),
-                             [131.90418292004594, 0, 139.46239300837794, 131.90418292004594]))
+@pytest.mark.parametrize("case, result", zip((1, 2, 3, 4), [131.90418292004594, 0, 139.46239300837794, 131.90418292004594]))
 def test_deep_sizing(case, result):
     borefield = Borefield()
     borefield.ground_data = GroundFluxTemperature(3, 10)
     borefield.create_rectangular_borefield(10, 5, 7, 7, 100, 0.75)
     load = MonthlyGeothermalLoadAbsolute(*load_case(case))
     borefield.load = load
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_monthly_load_data.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_monthly_load_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 import numpy as np
 
-from GHEtool.VariableClasses import MonthlyGeothermalLoadAbsolute, HourlyGeothermalLoad
+from GHEtool.VariableClasses import MonthlyGeothermalLoadAbsolute, HourlyGeothermalLoad, MonthlyGeothermalLoadMultiYear
 from GHEtool.Validation.cases import load_case
 
 
 def test_checks():
     load = MonthlyGeothermalLoadAbsolute()
     assert not load._check_input(2)
     assert not load._check_input(np.ones(11))
@@ -14,29 +14,20 @@
     assert load._check_input([1]*12)
     assert load._check_input(np.ones(12))
 
 
 def test_start_month_general():
     load = MonthlyGeothermalLoadAbsolute()
     assert load.start_month == 1
-    try:
+    with pytest.raises(ValueError):
         load.start_month = 1.5
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.start_month = 0
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.start_month = 13
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
     load.start_month = 12
     assert load.start_month == 12
     load.start_month = 1
     assert load.start_month == 1
 
 
 def test_imbalance():
@@ -51,68 +42,56 @@
     assert np.array_equal(load.baseload_heating, np.zeros(12))
     load.baseload_heating = np.linspace(0, 11, 12)
     assert np.array_equal(load.baseload_heating, np.linspace(0, 11, 12))
     load.set_baseload_heating(np.linspace(1, 12, 12))
     assert np.array_equal(load.baseload_heating, np.linspace(1, 12, 12))
     assert np.array_equal(load.baseload_heating / 730, load.baseload_heating_power)
     assert np.array_equal(load.baseload_heating_power, load.peak_heating)
-    try:
+    with pytest.raises(ValueError):
         load.set_baseload_heating(np.ones(11))
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_baseload_cooling():
     load = MonthlyGeothermalLoadAbsolute()
     assert np.array_equal(load.baseload_cooling, np.zeros(12))
     load.baseload_cooling = np.linspace(0, 11, 12)
     assert np.array_equal(load.baseload_cooling, np.linspace(0, 11, 12))
     load.set_baseload_cooling(np.linspace(1, 12, 12))
     assert np.array_equal(load.baseload_cooling, np.linspace(1, 12, 12))
     assert np.array_equal(load.baseload_cooling / 730, load.baseload_cooling_power)
     assert np.array_equal(load.baseload_cooling_power, load.peak_cooling)
 
-    try:
+    with pytest.raises(ValueError):
         load.set_baseload_cooling(np.ones(11))
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_peak_heating():
     load = MonthlyGeothermalLoadAbsolute()
     assert np.array_equal(load.peak_heating, np.zeros(12))
     load.peak_heating = np.linspace(0, 11, 12)
     assert np.array_equal(load.peak_heating, np.linspace(0, 11, 12))
     load.set_peak_heating(np.linspace(1, 12, 12))
     assert np.array_equal(load.peak_heating, np.linspace(1, 12, 12))
     load.set_baseload_heating(np.ones(12) * 730 * 5)
     assert np.array_equal(load.peak_heating, np.array([5., 5., 5., 5., 5., 6., 7., 8., 9., 10., 11., 12.]))
-    try:
+    with pytest.raises(ValueError):
         load.set_peak_heating(np.ones(11))
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_peak_cooling():
     load = MonthlyGeothermalLoadAbsolute()
     assert np.array_equal(load.peak_cooling, np.zeros(12))
     load.peak_cooling = np.linspace(0, 11, 12)
     assert np.array_equal(load.peak_cooling, np.linspace(0, 11, 12))
     load.set_peak_cooling(np.linspace(1, 12, 12))
     assert np.array_equal(load.peak_cooling, np.linspace(1, 12, 12))
     load.set_baseload_cooling(np.ones(12) * 730 * 5)
     assert np.array_equal(load.peak_cooling, np.array([5.,  5.,  5.,  5.,  5.,  6.,  7.,  8.,  9., 10., 11., 12.]))
-    try:
+    with pytest.raises(ValueError):
         load.set_peak_cooling(np.ones(11))
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
 
 def test_times():
     load = MonthlyGeothermalLoadAbsolute()
     load.peak_cooling_duration = 6
     load.peak_heating_duration = 7
     assert load.peak_heating_duration == 7 * 3600
@@ -185,14 +164,20 @@
 
 def test_params_first_year():
     load = MonthlyGeothermalLoadAbsolute(*load_case(2))
     assert np.array_equal(load._calculate_first_year_params(False),
                           (21600.0, 18396000.0, 21024000.0, 240000.0, 6410.9589041095915, 65753.42465753425))
     assert np.array_equal(load._calculate_first_year_params(True),
                           (21600.0, 0, 2628000.0, 160000.0, 0, 25753.424657534248))
+    temp = load.peak_cooling
+    temp[0] = 250
+    load.peak_cooling = temp
+    assert np.array_equal(load._calculate_first_year_params(False),
+                          (21600, 0, 2628000, 250000.0, 0, -25753.424657534248))
+
     load.peak_heating = np.ones(12) * 160
     load.peak_cooling = np.ones(12) * 240
 
     assert np.array_equal(load._calculate_first_year_params(False),
                           (21600, 18396000.0, 21024000.0, 240000.0, 6410.9589041095915, 65753.42465753425))
     assert np.array_equal(load._calculate_first_year_params(True),
                           (21600.0, 0, 2628000.0, 160000.0, 0, 25753.424657534248))
@@ -222,24 +207,18 @@
     load = MonthlyGeothermalLoadAbsolute()
     assert load.dhw == 0.
     load.add_dhw(1000)
     assert load.dhw == 1000.
     assert np.isclose(load.dhw_power, 1000./8760)
     load.dhw = 200
     assert load.dhw == 200.
-    try:
+    with pytest.raises(ValueError):
         load.add_dhw('test')
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
-    try:
+    with pytest.raises(ValueError):
         load.add_dhw(-10)
-        assert False  # pragma: no cover
-    except ValueError:
-        assert True
 
     load.dhw = 8760*10
     assert np.array_equal(np.full(12, 10), load.peak_heating)
     assert load.max_peak_heating == 10
     assert np.array_equal(np.full(12, 8760*10/12), load.baseload_heating)
     assert load.imbalance == -8760*10
     load.all_months_equal = False
@@ -301,19 +280,16 @@
     load_1 = MonthlyGeothermalLoadAbsolute(*load_case(2))
     load_2 = MonthlyGeothermalLoadAbsolute(*load_case(1))
     load_1.dhw = 10000
     load_2.dhw = 50000
     load_1.simulation_period = 20
     load_2.simulation_period = 30
 
-    try:
+    with pytest.raises(TypeError):
         load_1 + 55
-        assert False  # pragma: no cover
-    except TypeError:
-        assert True
 
     with pytest.warns():
         result = load_1 + load_2
 
     assert result.simulation_period == 30
     assert result.dhw == 60000
     assert np.allclose(result.baseload_heating, load_1.baseload_heating + load_2.baseload_heating)
@@ -372,7 +348,24 @@
                                          peak_heating=np.arange(1, 13, 1))
     load.start_month = 2
     result = np.array([2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 1])
     assert np.array_equal(load.baseload_heating, result)
     assert np.array_equal(load.baseload_cooling, result)
     assert np.array_equal(load.peak_heating, result)
     assert np.array_equal(load.peak_cooling, result)
+
+
+### continue for multi year
+def test_checks_multiyear_monthly():
+    load = MonthlyGeothermalLoadMultiYear()
+    assert not load._check_input(2)
+    assert not load._check_input(np.ones(11))
+    assert not load._check_input(-1*np.ones(12*2))
+    assert load._check_input([1]*12*2)
+    assert load._check_input(np.ones(12))
+    assert load._check_input(np.ones(12 * 3))
+    assert not load._check_input(np.ones(30))
+    with pytest.raises(ValueError):
+        load.baseload_heating = np.ones(13)
+    with pytest.raises(ValueError):
+        load.baseload_cooling = np.ones(13)
+
```

### Comparing `GHEtool-2.2.1/GHEtool/test/unit-tests/test_pipedata.py` & `ghetool-2.2.2/GHEtool/test/unit-tests/test_pipedata.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,23 @@
     fluid = gt.media.Fluid('MPG', 20.)
     fluid = FluidData(0.5, fluid.k, fluid.rho, fluid.cp, fluid.mu)
     pipe.calculate_resistances(fluid)
     assert np.isclose(pipe.R_fp, 0.11803503887356001)
     assert np.isclose(pipe.R_ff, 0.16491519753761458)
 
 
+def test_calculate_resistance_coaxial_different_outer_conductivity():
+    pipe = CoaxialPipe(r_in_in, r_in_out, r_out_in, r_out_out, k_p, k_g, is_inner_inlet=True, k_p_out=0.2)
+    fluid = gt.media.Fluid('MPG', 20.)
+    fluid = FluidData(0.5, fluid.k, fluid.rho, fluid.cp, fluid.mu)
+    pipe.calculate_resistances(fluid)
+    assert np.isclose(pipe.R_fp, 0.1664396892206207)
+    assert np.isclose(pipe.R_ff, 0.16491519753761458)
+
+
 def test_calculate_borehole_equivalent_resistance_coaxial():
     pipe = CoaxialPipe(r_in_in, r_in_out, r_out_in, r_out_out, k_p, k_g, is_inner_inlet=True)
     fluid = gt.media.Fluid('MPG', 20.)
     fluid = FluidData(0.5, fluid.k, fluid.rho, fluid.cp, fluid.mu)
     borehole = gt.boreholes.Borehole(100, 1, 0.075, 0, 0)
     pipe.calculate_resistances(fluid)
     model = pipe.pipe_model(fluid, 2, borehole)
@@ -155,14 +164,24 @@
                          r_in=np.array([r_out_in, r_in_in]) if is_inner_inlet else
                          np.array([r_in_in, r_out_in]),
                          r_out=np.array([r_out_out, r_in_out]) if is_inner_inlet else
                          np.array([r_in_out, r_out_out]),
                          borehole=borehole, k_s=i, k_g=k_g, R_ff=pipe_ghe.R_ff, R_fp=pipe_ghe.R_fp, J=2)
 
 
+def test_calculate_borehole_equivalent_resistance_coaxial_different_outer_conductivity():
+    pipe = CoaxialPipe(r_in_in, r_in_out, r_out_in, r_out_out, k_p, k_g, is_inner_inlet=True, k_p_out=0.2)
+    fluid = gt.media.Fluid('MPG', 20.)
+    fluid = FluidData(0.5, fluid.k, fluid.rho, fluid.cp, fluid.mu)
+    borehole = gt.boreholes.Borehole(100, 1, 0.075, 0, 0)
+    pipe.calculate_resistances(fluid)
+    model = pipe.pipe_model(fluid, 2, borehole)
+    assert np.isclose(model.effective_borehole_thermal_resistance(0.5, 4180), 0.22128574562981232)
+
+
 def test_pipe_data_equal_coaxial():
     data = CoaxialPipe(r_in_in, r_in_out, r_out_in, r_out_out, k_p, k_g, is_inner_inlet=True)
     data2 = CoaxialPipe(r_in_in, r_in_out, r_out_in, r_out_out, k_p, k_g, is_inner_inlet=True)
     assert data == data2
 
 
 def test_pipe_data_unequal_coaxial():
```

### Comparing `GHEtool-2.2.1/GHEtool.egg-info/PKG-INFO` & `ghetool-2.2.2/GHEtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GHEtool
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for borefield sizing
 Home-page: https://ghetool.eu
 Author: Wouter Peere
 Author-email: wouter@ghetool.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -16,24 +16,25 @@
 Requires-Dist: pandas>=1.4.3
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: pygfunction>=2.2.1
 
 # GHEtool: An open-source tool for borefield sizing
 
 [![PyPI version](https://badge.fury.io/py/GHEtool.svg)](https://badge.fury.io/py/GHEtool)
+[![Conda version](https://anaconda.org/conda-forge/ghetool/badges/version.svg)](https://anaconda.org/conda-forge/ghetool)
 [![Tests](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml/badge.svg)](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/wouterpeere/GHEtool/branch/main/graph/badge.svg?token=I9WWHW60OD)](https://codecov.io/gh/wouterpeere/GHEtool)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04406/status.svg)](https://doi.org/10.21105/joss.04406)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/ghetool)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads%20last%20week)](https://pepy.tech/project/ghetool)
 [![Read the Docs](https://readthedocs.org/projects/ghetool/badge/?version=latest)](https://ghetool.readthedocs.io/en/latest/)
 ## What is *GHEtool*?
 <img src="https://raw.githubusercontent.com/wouterpeere/GHEtool/main/docs/Icon.png" width="110" align="left">
 
-GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen.
+GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen and is currently being maintained by Enead BV.
 The core of this package is the automated sizing of borefield under different conditions. By making use of combination of just-in-time calculations of thermal ground responses (using [pygfunction](https://github.com/MassimoCimmino/pygfunction)) with
 intelligent interpolation, this automated sizing can be done in the order of milliseconds. Please visit our website [https://GHEtool.eu](https://GHEtool.eu) for more information.
 
 ### Read The Docs
 GHEtool has an elaborate documentation were all the functionalities of the tool are explained, with examples, literature and validation.
 This can be found on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
@@ -61,15 +62,14 @@
 This code is tested with Python 3.8, 3.9, 3.10, 3.11 and 3.12 and requires the following libraries (the versions mentioned are the ones with which the code is tested)
 
 * matplotlib >= 3.5.2
 * numpy >= 1.23.1
 * pandas >= 1.4.3
 * pygfunction >= 2.2.1
 * scipy >= 1.8.1
-* scikit-optimize >= 0.9.0
 
 For the tests
 
 * Pytest >= 7.1.2
 
 For the active/passive example
 
@@ -123,14 +123,16 @@
 #### Ground properties
 Within GHEtool, there are multiple ways of setting the ground data. Currently, your options are:
 
 * _GroundConstantTemperature_: if you want to model your borefield with a constant, know ground temperature.
 * _GroundFluxTemperature_: if you want to model your ground with a varying ground temperature due to a constant geothermal heat flux.
 * _GroundTemperatureGradient_: if you want to model your ground with a varying ground temperature due to a geothermal gradient.
 
+* You can also use multiple ground layers to define your ground model. Please take a look at [our example](https://docs.ghetool.eu/en/latest/sources/code/Examples/start_in_different_month.html).
+
 Please note that it is possible to add your own ground types by inheriting the attributes from the abstract _GroundData class.
 
 #### Pipe data
 Within GHEtool, you can use different structures for the borehole internals: U-tubes or coaxial pipes.
 Concretely, the classes you can use are:
 
 * _Multiple U-tubes_
@@ -146,14 +148,16 @@
 #### Load data
 One last element which you will need in your calculations, is the load data. Currently, you can only set the primary (i.e. geothermal) load of the borefield.
 In a future version of GHEtool, also secundary building loads will be included. For now, you can use the following inputs:
 
 * _MonthlyGeothermalLoadAbsolute_: You can set one the monthly baseload and peak load for heating and cooling for one standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoad_: You can set (or load) the hourly heating and cooling load of a standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoadMultiYear_: You can set (or load) the hourly heating and cooling load for multiple years (i.e. for the whole simulation period). This way, you can use secundary loads already with GHEtool as shown in [this example](https://ghetool.readthedocs.io/en/stable/sources/code/Examples/active_passive_cooling.html).
+* _MonthlyGeothermalLoadMultiYear_: You can set the monthly heating and cooling load for multiple years (i.e. for the whole simulation period).
+
 
 All load classes also have the option to add a yearly domestic hot water usage.
 
 Please note that it is possible to add your own load types by inheriting the attributes from the abstract _LoadData class.
 
 ### Options for sizing methods
 Like always with iterative methods, there is a trade-off between speed and accuracy. Within GHEtool (using the CalculationSetup class) one can alter different parameters
@@ -255,16 +259,16 @@
 
 ## Functionalities
 GHEtool offers functionalities of value to all different disciplines working with borefields. The features are available both in the code environment and in the GUI.
 For more information about the functionalities of GHEtool, please visit the documentation on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
 ## License
 
-*GHEtool* is licensed under the terms of the 3-clause BSD-license.
-See [GHEtool license](LICENSE).
+*GHEtool* is licensed under the terms of the 3-clause BSD-license (see [GHEtool license](LICENSE)).
+For professional licenses, contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
 
 ## Contact GHEtool
 - Do you want to support GHEtool financially or by contributing to our software?
 - Do you have a great idea for a new feature?
 - Do you have a specific remark/problem?
 
 Please do contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
@@ -289,14 +293,16 @@
 
 Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021). Validated combined first and last year borefield sizing methodology. In _Proceedings of International Building Simulation Conference 2021_. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
 
 Peere, W. (2020). Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering,
 KU Leuven, Belgium.
 
 ### Applications/Mentions of GHEtool
+Meertens, L. (2024). Invloed van dynamische korte-termijneffecten op de dimensionering van geothermische boorvelden. Master thesis, Department of Mechanical Engineering, KU Lueven, Belgium.
+
 Weynjes, J. (2023). Methode voor het dimensioneren van een geothermisch systeem met regeneratie binnen verschillende ESCO-structuren. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
 
 Hermans, L., Haesen, R., Uytterhoeven, A., Peere, W., Boydens, W., Helsen, L. (2023). Pre-design of collective residential solar districts with seasonal thermal energy storage: Importance of level of detail. _Applied thermal engineering_ 226, Art.No. 120203, 10.1016/j.applthermaleng.2023.120203
 
 Cimmino, M., Cook., J. C. (2022). pygfunction 2.2 : New Features and Improvements in Accuracy and Computational Efficiency. In _Proceedings of IGSHPA Research Track 2022_. Las Vegas (USA), 6-8 December 2022. https://doi.org/10.22488/okstate.22.000015
 
 Verleyen, L., Peere, W., Michiels, E., Boydens, W., Helsen, L. (2022). The beauty of reason and insight: a story about 30 years old borefield equations. _IEA HPT Magazine 40_(3), 36-39, https://doi.org/10.23697/6q4n-3223
```

### Comparing `GHEtool-2.2.1/GHEtool.egg-info/SOURCES.txt` & `ghetool-2.2.2/GHEtool.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+GHEtool/Borefield.py
 GHEtool/__init__.py
-GHEtool/main_class.py
 GHEtool.egg-info/PKG-INFO
 GHEtool.egg-info/SOURCES.txt
 GHEtool.egg-info/dependency_links.txt
 GHEtool.egg-info/requires.txt
 GHEtool.egg-info/top_level.txt
 GHEtool/Validation/__init__.py
 GHEtool/Validation/cases.py
@@ -24,35 +24,36 @@
 GHEtool/VariableClasses/GFunction.py
 GHEtool/VariableClasses/Result.py
 GHEtool/VariableClasses/__init__.py
 GHEtool/VariableClasses/cylindrical_correction.py
 GHEtool/VariableClasses/GroundData/GroundConstantTemperature.py
 GHEtool/VariableClasses/GroundData/GroundFluxTemperature.py
 GHEtool/VariableClasses/GroundData/GroundTemperatureGradient.py
-GHEtool/VariableClasses/GroundData/Temperature_database.py
 GHEtool/VariableClasses/GroundData/_GroundData.py
 GHEtool/VariableClasses/GroundData/__init__.py
 GHEtool/VariableClasses/LoadData/_LoadData.py
 GHEtool/VariableClasses/LoadData/__init__.py
 GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoad.py
 GHEtool/VariableClasses/LoadData/GeothermalLoad/HourlyGeothermalLoadMultiYear.py
 GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadAbsolute.py
+GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadMultiYear.py
 GHEtool/VariableClasses/LoadData/GeothermalLoad/MonthlyGeothermalLoadRelative.py
 GHEtool/VariableClasses/LoadData/GeothermalLoad/__init__.py
 GHEtool/VariableClasses/PipeData/CoaxialPipe.py
 GHEtool/VariableClasses/PipeData/DoubleUTube.py
 GHEtool/VariableClasses/PipeData/MultipleUTube.py
 GHEtool/VariableClasses/PipeData/SingleUTube.py
 GHEtool/VariableClasses/PipeData/_PipeData.py
 GHEtool/VariableClasses/PipeData/__init__.py
 GHEtool/logger/__init__.py
 GHEtool/logger/ghe_logger.py
 GHEtool/test/general_tests/__init__.py
 GHEtool/test/general_tests/test_GHEtool.py
 GHEtool/test/general_tests/test_GHEtool_two.py
+GHEtool/test/general_tests/test_multiple_years.py
 GHEtool/test/methods/TestMethodClass.py
 GHEtool/test/methods/__init__.py
 GHEtool/test/methods/method_data.py
 GHEtool/test/methods/test_methods.py
 GHEtool/test/unit-tests/__init__.py
 GHEtool/test/unit-tests/test_baseclass.py
 GHEtool/test/unit-tests/test_borehole.py
@@ -60,8 +61,9 @@
 GHEtool/test/unit-tests/test_custom_gfunction.py
 GHEtool/test/unit-tests/test_fluiddata.py
 GHEtool/test/unit-tests/test_gfunction.py
 GHEtool/test/unit-tests/test_grounddata.py
 GHEtool/test/unit-tests/test_hourly_load_data.py
 GHEtool/test/unit-tests/test_main_class.py
 GHEtool/test/unit-tests/test_monthly_load_data.py
+GHEtool/test/unit-tests/test_monthly_load_multi_year.py
 GHEtool/test/unit-tests/test_pipedata.py
```

### Comparing `GHEtool-2.2.1/LICENSE.txt` & `ghetool-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GHEtool-2.2.1/PKG-INFO` & `ghetool-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GHEtool
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python package for borefield sizing
 Home-page: https://ghetool.eu
 Author: Wouter Peere
 Author-email: wouter@ghetool.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -16,24 +16,25 @@
 Requires-Dist: pandas>=1.4.3
 Requires-Dist: scipy>=1.8.1
 Requires-Dist: pygfunction>=2.2.1
 
 # GHEtool: An open-source tool for borefield sizing
 
 [![PyPI version](https://badge.fury.io/py/GHEtool.svg)](https://badge.fury.io/py/GHEtool)
+[![Conda version](https://anaconda.org/conda-forge/ghetool/badges/version.svg)](https://anaconda.org/conda-forge/ghetool)
 [![Tests](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml/badge.svg)](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/wouterpeere/GHEtool/branch/main/graph/badge.svg?token=I9WWHW60OD)](https://codecov.io/gh/wouterpeere/GHEtool)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04406/status.svg)](https://doi.org/10.21105/joss.04406)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/ghetool)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads%20last%20week)](https://pepy.tech/project/ghetool)
 [![Read the Docs](https://readthedocs.org/projects/ghetool/badge/?version=latest)](https://ghetool.readthedocs.io/en/latest/)
 ## What is *GHEtool*?
 <img src="https://raw.githubusercontent.com/wouterpeere/GHEtool/main/docs/Icon.png" width="110" align="left">
 
-GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen.
+GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen and is currently being maintained by Enead BV.
 The core of this package is the automated sizing of borefield under different conditions. By making use of combination of just-in-time calculations of thermal ground responses (using [pygfunction](https://github.com/MassimoCimmino/pygfunction)) with
 intelligent interpolation, this automated sizing can be done in the order of milliseconds. Please visit our website [https://GHEtool.eu](https://GHEtool.eu) for more information.
 
 ### Read The Docs
 GHEtool has an elaborate documentation were all the functionalities of the tool are explained, with examples, literature and validation.
 This can be found on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
@@ -61,15 +62,14 @@
 This code is tested with Python 3.8, 3.9, 3.10, 3.11 and 3.12 and requires the following libraries (the versions mentioned are the ones with which the code is tested)
 
 * matplotlib >= 3.5.2
 * numpy >= 1.23.1
 * pandas >= 1.4.3
 * pygfunction >= 2.2.1
 * scipy >= 1.8.1
-* scikit-optimize >= 0.9.0
 
 For the tests
 
 * Pytest >= 7.1.2
 
 For the active/passive example
 
@@ -123,14 +123,16 @@
 #### Ground properties
 Within GHEtool, there are multiple ways of setting the ground data. Currently, your options are:
 
 * _GroundConstantTemperature_: if you want to model your borefield with a constant, know ground temperature.
 * _GroundFluxTemperature_: if you want to model your ground with a varying ground temperature due to a constant geothermal heat flux.
 * _GroundTemperatureGradient_: if you want to model your ground with a varying ground temperature due to a geothermal gradient.
 
+* You can also use multiple ground layers to define your ground model. Please take a look at [our example](https://docs.ghetool.eu/en/latest/sources/code/Examples/start_in_different_month.html).
+
 Please note that it is possible to add your own ground types by inheriting the attributes from the abstract _GroundData class.
 
 #### Pipe data
 Within GHEtool, you can use different structures for the borehole internals: U-tubes or coaxial pipes.
 Concretely, the classes you can use are:
 
 * _Multiple U-tubes_
@@ -146,14 +148,16 @@
 #### Load data
 One last element which you will need in your calculations, is the load data. Currently, you can only set the primary (i.e. geothermal) load of the borefield.
 In a future version of GHEtool, also secundary building loads will be included. For now, you can use the following inputs:
 
 * _MonthlyGeothermalLoadAbsolute_: You can set one the monthly baseload and peak load for heating and cooling for one standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoad_: You can set (or load) the hourly heating and cooling load of a standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoadMultiYear_: You can set (or load) the hourly heating and cooling load for multiple years (i.e. for the whole simulation period). This way, you can use secundary loads already with GHEtool as shown in [this example](https://ghetool.readthedocs.io/en/stable/sources/code/Examples/active_passive_cooling.html).
+* _MonthlyGeothermalLoadMultiYear_: You can set the monthly heating and cooling load for multiple years (i.e. for the whole simulation period).
+
 
 All load classes also have the option to add a yearly domestic hot water usage.
 
 Please note that it is possible to add your own load types by inheriting the attributes from the abstract _LoadData class.
 
 ### Options for sizing methods
 Like always with iterative methods, there is a trade-off between speed and accuracy. Within GHEtool (using the CalculationSetup class) one can alter different parameters
@@ -255,16 +259,16 @@
 
 ## Functionalities
 GHEtool offers functionalities of value to all different disciplines working with borefields. The features are available both in the code environment and in the GUI.
 For more information about the functionalities of GHEtool, please visit the documentation on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
 ## License
 
-*GHEtool* is licensed under the terms of the 3-clause BSD-license.
-See [GHEtool license](LICENSE).
+*GHEtool* is licensed under the terms of the 3-clause BSD-license (see [GHEtool license](LICENSE)).
+For professional licenses, contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
 
 ## Contact GHEtool
 - Do you want to support GHEtool financially or by contributing to our software?
 - Do you have a great idea for a new feature?
 - Do you have a specific remark/problem?
 
 Please do contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
@@ -289,14 +293,16 @@
 
 Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021). Validated combined first and last year borefield sizing methodology. In _Proceedings of International Building Simulation Conference 2021_. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
 
 Peere, W. (2020). Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering,
 KU Leuven, Belgium.
 
 ### Applications/Mentions of GHEtool
+Meertens, L. (2024). Invloed van dynamische korte-termijneffecten op de dimensionering van geothermische boorvelden. Master thesis, Department of Mechanical Engineering, KU Lueven, Belgium.
+
 Weynjes, J. (2023). Methode voor het dimensioneren van een geothermisch systeem met regeneratie binnen verschillende ESCO-structuren. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
 
 Hermans, L., Haesen, R., Uytterhoeven, A., Peere, W., Boydens, W., Helsen, L. (2023). Pre-design of collective residential solar districts with seasonal thermal energy storage: Importance of level of detail. _Applied thermal engineering_ 226, Art.No. 120203, 10.1016/j.applthermaleng.2023.120203
 
 Cimmino, M., Cook., J. C. (2022). pygfunction 2.2 : New Features and Improvements in Accuracy and Computational Efficiency. In _Proceedings of IGSHPA Research Track 2022_. Las Vegas (USA), 6-8 December 2022. https://doi.org/10.22488/okstate.22.000015
 
 Verleyen, L., Peere, W., Michiels, E., Boydens, W., Helsen, L. (2022). The beauty of reason and insight: a story about 30 years old borefield equations. _IEA HPT Magazine 40_(3), 36-39, https://doi.org/10.23697/6q4n-3223
```

### Comparing `GHEtool-2.2.1/README.md` & `ghetool-2.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # GHEtool: An open-source tool for borefield sizing
 
 [![PyPI version](https://badge.fury.io/py/GHEtool.svg)](https://badge.fury.io/py/GHEtool)
+[![Conda version](https://anaconda.org/conda-forge/ghetool/badges/version.svg)](https://anaconda.org/conda-forge/ghetool)
 [![Tests](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml/badge.svg)](https://github.com/wouterpeere/GHEtool/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/wouterpeere/GHEtool/branch/main/graph/badge.svg?token=I9WWHW60OD)](https://codecov.io/gh/wouterpeere/GHEtool)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04406/status.svg)](https://doi.org/10.21105/joss.04406)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/ghetool)
 [![Downloads](https://static.pepy.tech/personalized-badge/ghetool?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads%20last%20week)](https://pepy.tech/project/ghetool)
 [![Read the Docs](https://readthedocs.org/projects/ghetool/badge/?version=latest)](https://ghetool.readthedocs.io/en/latest/)
 ## What is *GHEtool*?
 <img src="https://raw.githubusercontent.com/wouterpeere/GHEtool/main/docs/Icon.png" width="110" align="left">
 
-GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen.
+GHEtool is a Python package that contains all the functionalities needed to deal with borefield design. GHEtool has been developed as a joint effort of KU Leuven (The SySi Team), boydens engineering (part of Sweco) and FH Aachen and is currently being maintained by Enead BV.
 The core of this package is the automated sizing of borefield under different conditions. By making use of combination of just-in-time calculations of thermal ground responses (using [pygfunction](https://github.com/MassimoCimmino/pygfunction)) with
 intelligent interpolation, this automated sizing can be done in the order of milliseconds. Please visit our website [https://GHEtool.eu](https://GHEtool.eu) for more information.
 
 ### Read The Docs
 GHEtool has an elaborate documentation were all the functionalities of the tool are explained, with examples, literature and validation.
 This can be found on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
@@ -42,15 +43,14 @@
 This code is tested with Python 3.8, 3.9, 3.10, 3.11 and 3.12 and requires the following libraries (the versions mentioned are the ones with which the code is tested)
 
 * matplotlib >= 3.5.2
 * numpy >= 1.23.1
 * pandas >= 1.4.3
 * pygfunction >= 2.2.1
 * scipy >= 1.8.1
-* scikit-optimize >= 0.9.0
 
 For the tests
 
 * Pytest >= 7.1.2
 
 For the active/passive example
 
@@ -104,14 +104,16 @@
 #### Ground properties
 Within GHEtool, there are multiple ways of setting the ground data. Currently, your options are:
 
 * _GroundConstantTemperature_: if you want to model your borefield with a constant, know ground temperature.
 * _GroundFluxTemperature_: if you want to model your ground with a varying ground temperature due to a constant geothermal heat flux.
 * _GroundTemperatureGradient_: if you want to model your ground with a varying ground temperature due to a geothermal gradient.
 
+* You can also use multiple ground layers to define your ground model. Please take a look at [our example](https://docs.ghetool.eu/en/latest/sources/code/Examples/start_in_different_month.html).
+
 Please note that it is possible to add your own ground types by inheriting the attributes from the abstract _GroundData class.
 
 #### Pipe data
 Within GHEtool, you can use different structures for the borehole internals: U-tubes or coaxial pipes.
 Concretely, the classes you can use are:
 
 * _Multiple U-tubes_
@@ -127,14 +129,16 @@
 #### Load data
 One last element which you will need in your calculations, is the load data. Currently, you can only set the primary (i.e. geothermal) load of the borefield.
 In a future version of GHEtool, also secundary building loads will be included. For now, you can use the following inputs:
 
 * _MonthlyGeothermalLoadAbsolute_: You can set one the monthly baseload and peak load for heating and cooling for one standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoad_: You can set (or load) the hourly heating and cooling load of a standard year which will be used for all years within the simulation period.
 * _HourlyGeothermalLoadMultiYear_: You can set (or load) the hourly heating and cooling load for multiple years (i.e. for the whole simulation period). This way, you can use secundary loads already with GHEtool as shown in [this example](https://ghetool.readthedocs.io/en/stable/sources/code/Examples/active_passive_cooling.html).
+* _MonthlyGeothermalLoadMultiYear_: You can set the monthly heating and cooling load for multiple years (i.e. for the whole simulation period).
+
 
 All load classes also have the option to add a yearly domestic hot water usage.
 
 Please note that it is possible to add your own load types by inheriting the attributes from the abstract _LoadData class.
 
 ### Options for sizing methods
 Like always with iterative methods, there is a trade-off between speed and accuracy. Within GHEtool (using the CalculationSetup class) one can alter different parameters
@@ -236,16 +240,16 @@
 
 ## Functionalities
 GHEtool offers functionalities of value to all different disciplines working with borefields. The features are available both in the code environment and in the GUI.
 For more information about the functionalities of GHEtool, please visit the documentation on [https://docs.ghetool.eu](https://docs.ghetool.eu).
 
 ## License
 
-*GHEtool* is licensed under the terms of the 3-clause BSD-license.
-See [GHEtool license](LICENSE).
+*GHEtool* is licensed under the terms of the 3-clause BSD-license (see [GHEtool license](LICENSE)).
+For professional licenses, contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
 
 ## Contact GHEtool
 - Do you want to support GHEtool financially or by contributing to our software?
 - Do you have a great idea for a new feature?
 - Do you have a specific remark/problem?
 
 Please do contact us at [info@ghetool.eu](mailto:info@ghetool.eu).
@@ -270,14 +274,16 @@
 
 Peere, W., Picard, D., Cupeiro Figueroa, I., Boydens, W., and Helsen, L. (2021). Validated combined first and last year borefield sizing methodology. In _Proceedings of International Building Simulation Conference 2021_. Brugge (Belgium), 1-3 September 2021. https://doi.org/10.26868/25222708.2021.30180
 
 Peere, W. (2020). Methode voor economische optimalisatie van geothermische verwarmings- en koelsystemen. Master thesis, Department of Mechanical Engineering,
 KU Leuven, Belgium.
 
 ### Applications/Mentions of GHEtool
+Meertens, L. (2024). Invloed van dynamische korte-termijneffecten op de dimensionering van geothermische boorvelden. Master thesis, Department of Mechanical Engineering, KU Lueven, Belgium.
+
 Weynjes, J. (2023). Methode voor het dimensioneren van een geothermisch systeem met regeneratie binnen verschillende ESCO-structuren. Master thesis, Department of Mechanical Engineering, KU Leuven, Belgium.
 
 Hermans, L., Haesen, R., Uytterhoeven, A., Peere, W., Boydens, W., Helsen, L. (2023). Pre-design of collective residential solar districts with seasonal thermal energy storage: Importance of level of detail. _Applied thermal engineering_ 226, Art.No. 120203, 10.1016/j.applthermaleng.2023.120203
 
 Cimmino, M., Cook., J. C. (2022). pygfunction 2.2 : New Features and Improvements in Accuracy and Computational Efficiency. In _Proceedings of IGSHPA Research Track 2022_. Las Vegas (USA), 6-8 December 2022. https://doi.org/10.22488/okstate.22.000015
 
 Verleyen, L., Peere, W., Michiels, E., Boydens, W., Helsen, L. (2022). The beauty of reason and insight: a story about 30 years old borefield equations. _IEA HPT Magazine 40_(3), 36-39, https://doi.org/10.23697/6q4n-3223
```

### Comparing `GHEtool-2.2.1/setup.cfg` & `ghetool-2.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = GHEtool
-version = 2.2.1
+version = 2.2.2
 author = Wouter Peere
 author_email = wouter@ghetool.eu
 description = Python package for borefield sizing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ghetool.eu
 classifiers =
```

