# Comparing `tmp/efootprint-2.0.5.tar.gz` & `tmp/efootprint-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efootprint-2.0.5.tar", max compression
+gzip compressed data, was "efootprint-2.1.0.tar", max compression
```

## Comparing `efootprint-2.0.5.tar` & `efootprint-2.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.0.5/LICENSE
--rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.0.5/efootprint/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.0.5/efootprint/abstract_modeling_classes/__init__.py
--rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_object_base_class.py
--rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_object_dict.py
--rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_objects.py
--rw-r--r--   0        0        0    17481 2024-04-12 11:51:41.746811 efootprint-2.0.5/efootprint/abstract_modeling_classes/modeling_object.py
--rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.0.5/efootprint/abstract_modeling_classes/source_objects.py
--rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.0.5/efootprint/api_utils/__init__.py
--rw-r--r--   0        0        0     6316 2024-04-16 12:52:57.980620 efootprint-2.0.5/efootprint/api_utils/json_to_system.py
--rw-r--r--   0        0        0     1306 2024-04-06 17:14:03.492802 efootprint-2.0.5/efootprint/api_utils/system_to_json.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.0.5/efootprint/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.0.5/efootprint/builders/hardware/__init__.py
--rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.0.5/efootprint/builders/hardware/devices_defaults.py
--rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.0.5/efootprint/builders/hardware/network_defaults.py
--rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.0.5/efootprint/builders/hardware/servers_boaviztapi.py
--rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.0.5/efootprint/builders/hardware/servers_defaults.py
--rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.0.5/efootprint/builders/hardware/storage_defaults.py
--rw-r--r--   0        0        0        0 2024-04-06 17:14:03.495913 efootprint-2.0.5/efootprint/builders/usage/__init__.py
--rw-r--r--   0        0        0       39 2024-04-06 17:14:03.499539 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/.gitignore
--rw-r--r--   0        0        0        0 2024-04-06 17:14:03.500532 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-06 17:14:03.502889 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
--rw-r--r--   0        0        0     3888 2024-04-16 12:54:03.574091 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
--rw-r--r--   0        0        0     1827 2024-04-06 17:14:03.506424 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
--rw-r--r--   0        0        0    67861 2024-04-06 17:14:03.511270 efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.0.5/efootprint/constants/__init__.py
--rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.0.5/efootprint/constants/countries.py
--rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.0.5/efootprint/constants/custom_units.txt
--rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.0.5/efootprint/constants/files.py
--rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.0.5/efootprint/constants/sources.py
--rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.0.5/efootprint/constants/units.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.0.5/efootprint/core/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.0.5/efootprint/core/hardware/__init__.py
--rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.0.5/efootprint/core/hardware/device_population.py
--rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.0.5/efootprint/core/hardware/hardware_base_classes.py
--rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.0.5/efootprint/core/hardware/network.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.0.5/efootprint/core/hardware/servers/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.0.5/efootprint/core/hardware/servers/autoscaling.py
--rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.0.5/efootprint/core/hardware/servers/on_premise.py
--rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.0.5/efootprint/core/hardware/servers/server_base_class.py
--rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.0.5/efootprint/core/hardware/servers/serverless.py
--rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.0.5/efootprint/core/hardware/storage.py
--rw-r--r--   0        0        0     5312 2024-04-06 17:14:03.514666 efootprint-2.0.5/efootprint/core/service.py
--rw-r--r--   0        0        0    10359 2024-04-06 17:14:03.517635 efootprint-2.0.5/efootprint/core/system.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.0.5/efootprint/core/usage/__init__.py
--rw-r--r--   0        0        0     3995 2024-04-06 17:14:03.519960 efootprint-2.0.5/efootprint/core/usage/job.py
--rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.0.5/efootprint/core/usage/usage_pattern.py
--rw-r--r--   0        0        0     2723 2024-04-06 17:14:03.529290 efootprint-2.0.5/efootprint/core/usage/user_journey.py
--rw-r--r--   0        0        0     1510 2024-04-06 17:14:03.531224 efootprint-2.0.5/efootprint/core/usage/user_journey_step.py
--rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.0.5/efootprint/logger.py
--rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.0.5/efootprint/utils/__init__.py
--rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.0.5/efootprint/utils/calculus_graph.py
--rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.0.5/efootprint/utils/dev_utils/README.md
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.0.5/efootprint/utils/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.0.5/efootprint/utils/dev_utils/page_weights.py
--rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.0.5/efootprint/utils/dev_utils/selenium_screenshot.py
--rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.0.5/efootprint/utils/graph_tools.py
--rw-r--r--   0        0        0     2390 2024-04-06 17:14:03.536199 efootprint-2.0.5/efootprint/utils/object_relationships_graphs.py
--rw-r--r--   0        0        0     7612 2024-04-06 17:14:03.543621 efootprint-2.0.5/efootprint/utils/plot_emission_diffs.py
--rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.0.5/efootprint/utils/tools.py
--rw-r--r--   0        0        0     1258 2024-04-16 12:54:20.215067 efootprint-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-10-17 09:49:47.557993 efootprint-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3456 2024-04-06 12:40:51.663763 efootprint-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 12:40:52.150404 efootprint-2.1.0/efootprint/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.648138 efootprint-2.1.0/efootprint/abstract_modeling_classes/__init__.py
+-rw-r--r--   0        0        0    11880 2024-04-06 12:40:52.160479 efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py
+-rw-r--r--   0        0        0     2240 2024-04-06 12:40:52.168353 efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_object_dict.py
+-rw-r--r--   0        0        0    12607 2024-04-06 12:40:52.173001 efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_objects.py
+-rw-r--r--   0        0        0    17481 2024-04-12 11:51:41.746811 efootprint-2.1.0/efootprint/abstract_modeling_classes/modeling_object.py
+-rw-r--r--   0        0        0      754 2024-03-04 16:54:55.210288 efootprint-2.1.0/efootprint/abstract_modeling_classes/source_objects.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:55:00.126280 efootprint-2.1.0/efootprint/api_utils/__init__.py
+-rw-r--r--   0        0        0     6316 2024-05-06 13:11:31.690566 efootprint-2.1.0/efootprint/api_utils/json_to_system.py
+-rw-r--r--   0        0        0     1306 2024-04-06 17:14:03.492802 efootprint-2.1.0/efootprint/api_utils/system_to_json.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:53.623840 efootprint-2.1.0/efootprint/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 16:54:54.164118 efootprint-2.1.0/efootprint/builders/hardware/__init__.py
+-rw-r--r--   0        0        0     2076 2024-03-04 16:54:55.218246 efootprint-2.1.0/efootprint/builders/hardware/devices_defaults.py
+-rw-r--r--   0        0        0      743 2024-03-04 16:54:55.222924 efootprint-2.1.0/efootprint/builders/hardware/network_defaults.py
+-rw-r--r--   0        0        0     8980 2024-04-06 12:40:52.200652 efootprint-2.1.0/efootprint/builders/hardware/servers_boaviztapi.py
+-rw-r--r--   0        0        0     2898 2024-03-04 16:54:57.077899 efootprint-2.1.0/efootprint/builders/hardware/servers_defaults.py
+-rw-r--r--   0        0        0     1876 2024-03-04 16:54:55.236944 efootprint-2.1.0/efootprint/builders/hardware/storage_defaults.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.495913 efootprint-2.1.0/efootprint/builders/usage/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-06 17:14:03.499539 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-06 17:14:03.500532 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/__init__.py
+-rw-r--r--   0        0        0     2556 2024-04-06 17:14:03.502889 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py
+-rw-r--r--   0        0        0     3888 2024-05-15 13:32:03.373715 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv
+-rw-r--r--   0        0        0     1827 2024-04-06 17:14:03.506424 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py
+-rw-r--r--   0        0        0    67861 2024-04-06 17:14:03.511270 efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.656189 efootprint-2.1.0/efootprint/constants/__init__.py
+-rw-r--r--   0        0        0     4182 2024-04-06 12:40:52.207602 efootprint-2.1.0/efootprint/constants/countries.py
+-rw-r--r--   0        0        0      100 2023-10-26 17:58:06.658280 efootprint-2.1.0/efootprint/constants/custom_units.txt
+-rw-r--r--   0        0        0      284 2023-11-13 13:05:11.080734 efootprint-2.1.0/efootprint/constants/files.py
+-rw-r--r--   0        0        0     1660 2024-03-04 16:54:55.243478 efootprint-2.1.0/efootprint/constants/sources.py
+-rw-r--r--   0        0        0      173 2023-10-26 17:58:06.666143 efootprint-2.1.0/efootprint/constants/units.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.666706 efootprint-2.1.0/efootprint/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.667254 efootprint-2.1.0/efootprint/core/hardware/__init__.py
+-rw-r--r--   0        0        0     6034 2024-04-06 12:40:52.212747 efootprint-2.1.0/efootprint/core/hardware/device_population.py
+-rw-r--r--   0        0        0     5707 2024-04-06 12:40:52.215226 efootprint-2.1.0/efootprint/core/hardware/hardware_base_classes.py
+-rw-r--r--   0        0        0     3367 2024-04-06 12:40:52.219470 efootprint-2.1.0/efootprint/core/hardware/network.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.671292 efootprint-2.1.0/efootprint/core/hardware/servers/__init__.py
+-rw-r--r--   0        0        0     3135 2024-03-04 16:54:57.120650 efootprint-2.1.0/efootprint/core/hardware/servers/autoscaling.py
+-rw-r--r--   0        0        0     3766 2024-04-06 12:40:52.222595 efootprint-2.1.0/efootprint/core/hardware/servers/on_premise.py
+-rw-r--r--   0        0        0     3464 2024-03-04 16:54:59.121266 efootprint-2.1.0/efootprint/core/hardware/servers/server_base_class.py
+-rw-r--r--   0        0        0     1972 2024-03-04 16:54:57.211287 efootprint-2.1.0/efootprint/core/hardware/servers/serverless.py
+-rw-r--r--   0        0        0     5491 2024-03-04 16:54:59.146307 efootprint-2.1.0/efootprint/core/hardware/storage.py
+-rw-r--r--   0        0        0     5312 2024-04-06 17:14:03.514666 efootprint-2.1.0/efootprint/core/service.py
+-rw-r--r--   0        0        0    10750 2024-05-15 13:32:15.121297 efootprint-2.1.0/efootprint/core/system.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.688562 efootprint-2.1.0/efootprint/core/usage/__init__.py
+-rw-r--r--   0        0        0     3995 2024-04-06 17:14:03.519960 efootprint-2.1.0/efootprint/core/usage/job.py
+-rw-r--r--   0        0        0     3890 2024-04-06 12:40:52.233601 efootprint-2.1.0/efootprint/core/usage/usage_pattern.py
+-rw-r--r--   0        0        0     2723 2024-04-06 17:14:03.529290 efootprint-2.1.0/efootprint/core/usage/user_journey.py
+-rw-r--r--   0        0        0     1510 2024-04-06 17:14:03.531224 efootprint-2.1.0/efootprint/core/usage/user_journey_step.py
+-rw-r--r--   0        0        0      805 2023-11-13 13:05:11.082835 efootprint-2.1.0/efootprint/logger.py
+-rw-r--r--   0        0        0        0 2023-10-26 17:58:06.698150 efootprint-2.1.0/efootprint/utils/__init__.py
+-rw-r--r--   0        0        0     3055 2024-04-06 12:40:52.240288 efootprint-2.1.0/efootprint/utils/calculus_graph.py
+-rw-r--r--   0        0        0      146 2023-11-03 15:44:18.031433 efootprint-2.1.0/efootprint/utils/dev_utils/README.md
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.033655 efootprint-2.1.0/efootprint/utils/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-03 15:44:18.035244 efootprint-2.1.0/efootprint/utils/dev_utils/page_weights.py
+-rw-r--r--   0        0        0      830 2023-11-03 15:44:18.039040 efootprint-2.1.0/efootprint/utils/dev_utils/selenium_screenshot.py
+-rw-r--r--   0        0        0     1407 2024-04-06 12:40:52.242646 efootprint-2.1.0/efootprint/utils/graph_tools.py
+-rw-r--r--   0        0        0     2390 2024-04-06 17:14:03.536199 efootprint-2.1.0/efootprint/utils/object_relationships_graphs.py
+-rw-r--r--   0        0        0     7950 2024-05-15 13:32:15.132273 efootprint-2.1.0/efootprint/utils/plot_emission_diffs.py
+-rw-r--r--   0        0        0     1702 2024-03-04 16:54:53.701197 efootprint-2.1.0/efootprint/utils/tools.py
+-rw-r--r--   0        0        0     1258 2024-05-15 13:32:50.288617 efootprint-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 efootprint-2.1.0/PKG-INFO
```

### Comparing `efootprint-2.0.5/LICENSE` & `efootprint-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/README.md` & `efootprint-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_object_base_class.py` & `efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_object_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_object_dict.py` & `efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_object_dict.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/abstract_modeling_classes/explainable_objects.py` & `efootprint-2.1.0/efootprint/abstract_modeling_classes/explainable_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/abstract_modeling_classes/modeling_object.py` & `efootprint-2.1.0/efootprint/abstract_modeling_classes/modeling_object.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/abstract_modeling_classes/source_objects.py` & `efootprint-2.1.0/efootprint/abstract_modeling_classes/source_objects.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/api_utils/json_to_system.py` & `efootprint-2.1.0/efootprint/api_utils/json_to_system.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/api_utils/system_to_json.py` & `efootprint-2.1.0/efootprint/api_utils/system_to_json.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/hardware/devices_defaults.py` & `efootprint-2.1.0/efootprint/builders/hardware/devices_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/hardware/network_defaults.py` & `efootprint-2.1.0/efootprint/builders/hardware/network_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/hardware/servers_boaviztapi.py` & `efootprint-2.1.0/efootprint/builders/hardware/servers_boaviztapi.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/hardware/servers_defaults.py` & `efootprint-2.1.0/efootprint/builders/hardware/servers_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/hardware/storage_defaults.py` & `efootprint-2.1.0/efootprint/builders/hardware/storage_defaults.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py` & `efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_analysis.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv` & `efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_data_for_job_defaults.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py` & `efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_job_builder.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv` & `efootprint-2.1.0/efootprint/builders/usage/job_ecobenchmark/ecobenchmark_results__raw.csv`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/constants/countries.py` & `efootprint-2.1.0/efootprint/constants/countries.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/constants/sources.py` & `efootprint-2.1.0/efootprint/constants/sources.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/device_population.py` & `efootprint-2.1.0/efootprint/core/hardware/device_population.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/hardware_base_classes.py` & `efootprint-2.1.0/efootprint/core/hardware/hardware_base_classes.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/network.py` & `efootprint-2.1.0/efootprint/core/hardware/network.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/servers/autoscaling.py` & `efootprint-2.1.0/efootprint/core/hardware/servers/autoscaling.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/servers/on_premise.py` & `efootprint-2.1.0/efootprint/core/hardware/servers/on_premise.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/servers/server_base_class.py` & `efootprint-2.1.0/efootprint/core/hardware/servers/server_base_class.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/servers/serverless.py` & `efootprint-2.1.0/efootprint/core/hardware/servers/serverless.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/hardware/storage.py` & `efootprint-2.1.0/efootprint/core/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/service.py` & `efootprint-2.1.0/efootprint/core/service.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/system.py` & `efootprint-2.1.0/efootprint/core/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,22 +161,22 @@
             sum(
                 sum(
                     self.fabrication_footprints[key].values()) + sum(self.energy_footprints[key].values())
                 for key in self.fabrication_footprints.keys()
             )
         ).set_label(f"{self.name} total carbon footprint")
 
-    def plot_footprints_by_category_and_object(self, filename=None):
+    def plot_footprints_by_category_and_object(self, filename=None, height=400, width=800, return_only_html=False):
         fab_footprints = self.fabrication_footprints
         energy_footprints = self.energy_footprints
         categories = list(fab_footprints.keys())
 
         rows_as_dicts = []
 
-        value_colname = "Carbon footprints in tons CO2eq / year"
+        value_colname = "tons CO2 emissions / year"
         for category in categories:
             fab_objects = sorted(fab_footprints[category].items(), key=lambda x: x[0])
             energy_objects = sorted(energy_footprints[category].items(), key=lambda x: x[0])
 
             for objs, color in zip([energy_objects, fab_objects], ["Electricity", "Fabrication"]):
                 data_dicts = [
                     {"Type": color, "Category": category, "Object": obj[0],
@@ -186,19 +186,23 @@
                 rows_as_dicts += data_dicts
 
         df = pd.DataFrame.from_records(rows_as_dicts)
 
         total_co2 = df[value_colname].sum()
 
         fig = px.bar(
-            df, x="Category", y=value_colname, color='Type', barmode='group', height=400,
+            df, x="Category", y=value_colname, color='Type', barmode='group', height=height, width=width,
             hover_data={"Type": False, "Category": False, "Object": True, value_colname: False, "Amount": True},
-            template="plotly_white", width=800,
+            template="plotly_white",
             title=f"Total CO2 emissions from {self.name}: {display_co2_amount(format_co2_amount(total_co2 * 1000))} / year")
 
+        fig.update_layout(
+            legend={"orientation": "v", "yanchor": "top", "y": 1.02, "xanchor": "left", "x": 0.02, "title": ""},
+            title={"x": 0.5, "y": 0.9, "xanchor": 'center', "yanchor": 'top'})
+
         total_co2_per_category_and_type = df.groupby(["Category", "Type"])[value_colname].sum()
 
         for category, source_type in total_co2_per_category_and_type.keys():
             height = total_co2_per_category_and_type.loc[category, source_type]
             x_shift_direction = 1 if source_type == 'Fabrication' else -1
 
             fig.add_annotation(
@@ -206,20 +210,24 @@
                 y=height,
                 text=f"{int((height / total_co2) * 100)}%",  # Format the label as a percentage
                 showarrow=False,
                 yshift=10,  # Shift the label slightly above the stack
                 xshift=30 * x_shift_direction
             )
 
-        if filename is None:
-            filename = f"{self.name} footprints.html"
+        if return_only_html:
+            return fig.to_html(full_html=False, include_plotlyjs=False)
+
+        else:
+            if filename is None:
+                filename = f"{self.name} footprints.html"
 
-        plotly.offline.plot(fig, filename=filename, auto_open=False)
+            plotly.offline.plot(fig, filename=filename, auto_open=False)
 
-        return HTML(filename)
+            return HTML(filename)
 
     def plot_emission_diffs(self, filepath=None, figsize=(10, 5), from_start=False, plt_show=False):
         if self.previous_change is None:
             raise ValueError(
                 f"There has been no change to the system yet so no diff to plot.\n"
                 f"Use System.plot_footprints_by_category_and_object() to visualize footprints")
 
@@ -232,15 +240,15 @@
             emissions_dict__old = [self.previous_total_energy_footprints, self.previous_total_fabrication_footprints]
 
         emissions_dict__new = [self.total_energy_footprints, self.total_fabrication_footprints]
 
         fig, ax = plt.subplots(nrows=1, ncols=1, figsize=figsize)
 
         EmissionPlotter(
-            ax, emissions_dict__old, emissions_dict__new, title=self.name, rounding_value=1,
+            ax, emissions_dict__old, emissions_dict__new, title=self.name, rounding_value=0,
             timespan=ExplainableQuantity(1 * u.year, "one year")).plot_emission_diffs()
 
         if filepath is not None:
             plt.savefig(filepath, bbox_inches='tight')
 
         if plt_show:
             plt.show()
```

### Comparing `efootprint-2.0.5/efootprint/core/usage/job.py` & `efootprint-2.1.0/efootprint/core/usage/job.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/usage/usage_pattern.py` & `efootprint-2.1.0/efootprint/core/usage/usage_pattern.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/usage/user_journey.py` & `efootprint-2.1.0/efootprint/core/usage/user_journey.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/core/usage/user_journey_step.py` & `efootprint-2.1.0/efootprint/core/usage/user_journey_step.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/logger.py` & `efootprint-2.1.0/efootprint/logger.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/utils/calculus_graph.py` & `efootprint-2.1.0/efootprint/utils/calculus_graph.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/utils/dev_utils/selenium_screenshot.py` & `efootprint-2.1.0/efootprint/utils/dev_utils/selenium_screenshot.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/utils/graph_tools.py` & `efootprint-2.1.0/efootprint/utils/graph_tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/utils/object_relationships_graphs.py` & `efootprint-2.1.0/efootprint/utils/object_relationships_graphs.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/efootprint/utils/plot_emission_diffs.py` & `efootprint-2.1.0/efootprint/utils/plot_emission_diffs.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,106 +19,114 @@
         self.timespan = timespan
         self.legend_labels = legend_labels
         self.elements = ["Servers", "Storage", "Network", "Devices"]
         self.index = np.arange(len(self.elements))
         self.bar_width = 0.4
         self.total_emissions_in_kg__new = self.calculate_total_emissions(formatted_input_dicts__new)
         self.total_emissions_in_kg__old = self.calculate_total_emissions(formatted_input_dicts__old)
-        self.colors = ["#1f77b4", "#ff7f0e"]
+        self.colors = ["#6372f2", "#de5f46"]
+        if self.total_emissions_in_kg__new < 501:
+            self.unit = "kg"
+            self.dividing_number = 1
+        else:
+            self.unit = "ton"
+            self.dividing_number = 1000
 
     def calculate_total_emissions(self, formatted_input_dicts):
         total_emissions_in_kg = 0
         for input_dict in formatted_input_dicts:
             total_emissions_in_kg += (sum(input_dict.values()) * self.timespan).to(u.kg).magnitude
         return total_emissions_in_kg
 
     def get_values(self, input_dict):
-        return [(input_dict.get(element, 0 * u.kg / u.year) * self.timespan).to(u.kg).magnitude for element in self.elements]
+        return [(input_dict.get(element, 0 * u(self.unit) / u.year) * self.timespan).to(u(self.unit)).magnitude
+                for element in self.elements]
 
     def plot_common_values(self, common_values, i, color):
         return self.ax.bar(self.index + i * self.bar_width, common_values, self.bar_width, color=color, alpha=1.0)
 
     def plot_difference_values(self, diff_values, common_values, i, color):
         return self.ax.bar(
             self.index + i * self.bar_width, diff_values, self.bar_width, bottom=common_values, color=color, alpha=0.1)
 
     def plot_positive_diff(self, positive_diffs, common_values, i, color):
         return self.ax.bar(
             self.index + i * self.bar_width, positive_diffs, self.bar_width, bottom=common_values, color=color,
-            alpha=0.9)
+            alpha=0.7)
 
     def add_annotations_and_text(self, rects_common, diffs, values_old, values_new):
         arrowprops = dict(facecolor='black', shrink=0.05, width=2, headwidth=8)
 
+        figure_height = self.ax.get_ylim()[1]
         for rect, diff, value_old, value_new in zip(rects_common, diffs, values_old, values_new):
             if value_old != value_new:
-                if diff < -0.5:
-                    self.ax.annotate("", xy=(rect.get_x() + rect.get_width() / 2 - 0.06, min(value_old, value_new)),
-                                xytext=(rect.get_x() + rect.get_width() / 2 - 0.06, max(value_old, value_new)),
-                                arrowprops=arrowprops)
-                    self.ax.text(rect.get_x() + rect.get_width() / 2 + 0.06, (value_old + value_new) / 2, f"{diff:.0f}%",
-                            ha="center", va="center")
-                elif diff > 0.5:
-                    self.ax.annotate("", xy=(rect.get_x() + rect.get_width() / 2 - 0.06, max(value_old, value_new)),
-                                xytext=(rect.get_x() + rect.get_width() / 2 - 0.06, min(value_old, value_new)),
-                                arrowprops=arrowprops)
-                    self.ax.text(rect.get_x() + rect.get_width() / 2 + 0.06, (value_old + value_new) / 2, f"+{diff:.0f}%",
-                            ha="center", va="center")
+                if diff < -1:
+                    if abs(value_old - value_new) > figure_height / 10:
+                        self.ax.annotate(
+                            "", xy=(rect.get_x() + rect.get_width() / 2 - 0.06,
+                                    min(value_old, value_new) + figure_height / 20),
+                            xytext=(rect.get_x() + rect.get_width() / 2 - 0.06, max(value_old, value_new)),
+                            arrowprops=arrowprops)
+                    self.ax.text(
+                        rect.get_x() + rect.get_width() / 2 + 0.06, (value_old + value_new) / 2, f"{diff:.0f}%",
+                        ha="center", va="center")
+                elif diff > 1:
+                    if abs(value_old - value_new) > figure_height / 10:
+                        self.ax.annotate(
+                            "", xy=(rect.get_x() + rect.get_width() / 2 - 0.06, max(value_old, value_new)),
+                            xytext=(rect.get_x() + rect.get_width() / 2 - 0.06, min(value_old, value_new)),
+                            arrowprops=arrowprops)
+                    self.ax.text(
+                        rect.get_x() + rect.get_width() / 2 + 0.06, (value_old + value_new) / 2, f"+{diff:.0f}%",
+                        ha="center", va="center")
 
-            proportion = (value_new / self.total_emissions_in_kg__new) * 100
+            proportion = (value_new / (self.total_emissions_in_kg__new / self.dividing_number)) * 100
             self.ax.text(rect.get_x() + rect.get_width() / 2, value_new, f"{proportion:.0f}%", ha="center", va="bottom")
 
     def set_axes_labels(self):
-        self.ax.set_xlabel("Physical Elements")
-        self.ax.set_ylabel(f"kg CO2 emissions / {self.timespan.value}")
-        self.ax.set_title(self.title, fontsize=18, fontweight="bold", y=1.12)
+        self.ax.set_xlabel("Category")
+        self.ax.set_ylabel(f"{self.unit}s CO2 emissions / {self.timespan.value}".replace("1 ", ""))
 
         self.ax.set_xticks(self.index + self.bar_width / 2)
-        self.ax.set_xticklabels(self.elements, rotation=45, ha="right")
+        self.ax.set_xticklabels(self.elements, rotation=0, ha="center")
 
         ax2 = self.ax.twinx()
         max_value = max(
             [max(input_dict.values()) * self.timespan
-             for input_dict in self.formatted_input_dicts__new + self.formatted_input_dicts__old]).to(u.kg).magnitude
+             for input_dict in self.formatted_input_dicts__new + self.formatted_input_dicts__old]
+        ).to(u(self.unit)).magnitude
 
         max_value_margin = 1.1
-        ax2.set_ylim(0, 100 * max_value_margin * (max_value / self.total_emissions_in_kg__new))
+        ax2.set_ylim(0, 100 * max_value_margin * (max_value / (self.total_emissions_in_kg__new / self.dividing_number)))
         ax2.set_ylabel("Proportions (%)")
 
         self.ax.set_ylim(0, max_value_margin * max_value)
 
     def set_titles(self):
-        self.ax.set_title(self.title, fontsize=24, fontweight="bold", y=1.1)
-        if self.total_emissions_in_kg__new < 501:
-            unit = "kg"
-            dividing_number = 1
-        else:
-            unit = "ton"
-            dividing_number = 1000
-        rounded_total__new = round(self.total_emissions_in_kg__new / dividing_number, self.rounding_value)
+        rounded_total__new = round(self.total_emissions_in_kg__new / self.dividing_number, self.rounding_value)
         if self.rounding_value == 0:
             rounded_total__new = int(rounded_total__new)
 
         total_emissions_in_kg__old = 0
         for input_dict in self.formatted_input_dicts__old:
             total_emissions_in_kg__old += (sum(input_dict.values()) * self.timespan).to(u.kg).magnitude
 
-        rounded_total__old = round(total_emissions_in_kg__old / dividing_number, self.rounding_value)
+        rounded_total__old = round(total_emissions_in_kg__old / self.dividing_number, self.rounding_value)
         if self.rounding_value == 0:
             rounded_total__old = int(rounded_total__old)
 
         if rounded_total__old != rounded_total__new:
             plus_sign = ""
             if rounded_total__new - rounded_total__old > 0:
                 plus_sign = "+"
-            subtitle_text = f"From {rounded_total__old} to {rounded_total__new} {unit}s of CO2 emissions in" \
+            subtitle_text = f"From {rounded_total__old} to {rounded_total__new} {self.unit}s of CO2 emissions in" \
                             f" {self.timespan.value} " \
                             f"({plus_sign}{int(100 * (rounded_total__new - rounded_total__old) / rounded_total__old)}%)"
         else:
-            subtitle_text = f"{rounded_total__new} {unit}s of CO2 emissions in {self.timespan.value}"
+            subtitle_text = f"{rounded_total__new} {self.unit}s of CO2 emissions in {self.timespan.value}"
         subtitle_text = subtitle_text.replace("in 1 year", "per year")
 
         self.ax.text(
             0.5, 1.1, subtitle_text,
             transform=self.ax.transAxes, fontsize=16, va="top", ha="center")
 
     def plot_emission_diffs(self):
```

### Comparing `efootprint-2.0.5/efootprint/utils/tools.py` & `efootprint-2.1.0/efootprint/utils/tools.py`

 * *Files identical despite different names*

### Comparing `efootprint-2.0.5/pyproject.toml` & `efootprint-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "efootprint"
-version = "2.0.5"
+version = "2.1.0"
 description = "Digital service environmental footprint model"
 authors = ["Vincent Villet for Publicis Sapient"]
 readme = "README.md"
 include = ["efootprint/constants/custom_units.txt"]
 
 [tool.black]
 line-length = 120
```

### Comparing `efootprint-2.0.5/PKG-INFO` & `efootprint-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efootprint
-Version: 2.0.5
+Version: 2.1.0
 Summary: Digital service environmental footprint model
 Author: Vincent Villet for Publicis Sapient
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

