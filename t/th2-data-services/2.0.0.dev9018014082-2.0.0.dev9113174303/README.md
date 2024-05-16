# Comparing `tmp/th2_data_services-2.0.0.dev9018014082.tar.gz` & `tmp/th2_data_services-2.0.0.dev9113174303.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th2_data_services-2.0.0.dev9018014082.tar", last modified: Thu May  9 13:28:18 2024, max compression
+gzip compressed data, was "th2_data_services-2.0.0.dev9113174303.tar", last modified: Thu May 16 13:27:49 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev9018014082.tar` & `th2_data_services-2.0.0.dev9113174303.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.700000 th2_data_services-2.0.0.dev9018014082/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-09 13:28:18.700000 th2_data_services-2.0.0.dev9018014082/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 13:28:09.000000 th2_data_services-2.0.0.dev9018014082/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:28:18.700000 th2_data_services-2.0.0.dev9018014082/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.696000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.696000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.696000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.696000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.700000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.700000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-09 13:27:19.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:28:18.692000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-09 13:28:18.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-09 13:28:18.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:28:18.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 13:28:18.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 13:28:18.000000 th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42932 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35191 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 13:27:41.000000 th2_data_services-2.0.0.dev9113174303/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.927421 th2_data_services-2.0.0.dev9113174303/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.927421 th2_data_services-2.0.0.dev9113174303/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.927421 th2_data_services-2.0.0.dev9113174303/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42226 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.927421 th2_data_services-2.0.0.dev9113174303/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.931421 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.931421 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.931421 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.935421 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-16 13:26:31.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:27:49.927421 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42932 2024-05-16 13:27:49.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-16 13:27:49.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:27:49.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 13:27:49.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 13:27:49.000000 th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev9018014082/LICENSE` & `th2_data_services-2.0.0.dev9113174303/LICENSE`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/PKG-INFO` & `th2_data_services-2.0.0.dev9113174303/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3930 3138 3031 3430 3832 0a53 756d 6d61  9018014082.Summa
+00000040: 3931 3133 3137 3433 3033 0a53 756d 6d61  9113174303.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -303,2360 +303,2382 @@
 000012e0: 6c6c 6f77 696e 6720 6578 616d 706c 6520  llowing example 
 000012f0: 6173 2061 2066 696c 655d 2865 7861 6d70  as a file](examp
 00001300: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
 00001310: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
 00001320: 2020 2020 200a 2020 2020 2020 2020 3c21       .        <!
 00001330: 2d2d 2073 7461 7274 2067 6574 5f73 7461  -- start get_sta
 00001340: 7274 6564 5f65 7861 6d70 6c65 2e70 7920  rted_example.py 
-00001350: 2d2d 3e0a 2020 2020 2020 2020 6060 6070  -->.        ```p
-00001360: 7974 686f 6e0a 2020 2020 2020 2020 6672  ython.        fr
-00001370: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00001380: 2054 7570 6c65 2c20 4c69 7374 2c20 4f70   Tuple, List, Op
-00001390: 7469 6f6e 616c 2c20 4765 6e65 7261 746f  tional, Generato
-000013a0: 720a 2020 2020 2020 2020 6672 6f6d 2064  r.        from d
-000013b0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-000013c0: 6174 6574 696d 650a 2020 2020 2020 2020  atetime.        
-000013d0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-000013e0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-000013f0: 6461 7461 2069 6d70 6f72 7420 4461 7461  data import Data
-00001400: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001410: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001420: 6475 6d6d 7920 696d 706f 7274 2044 756d  dummy import Dum
-00001430: 6d79 4461 7461 536f 7572 6365 0a20 2020  myDataSource.   
-00001440: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001450: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
-00001460: 745f 7472 6565 2069 6d70 6f72 7420 280a  t_tree import (.
-00001470: 2020 2020 2020 2020 2020 2020 4576 656e              Even
-00001480: 7454 7265 652c 0a20 2020 2020 2020 2020  tTree,.         
-00001490: 2020 2045 7665 6e74 5472 6565 436f 6c6c     EventTreeColl
-000014a0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
-000014b0: 2020 2020 5061 7265 6e74 4576 656e 7454      ParentEventT
-000014c0: 7265 6543 6f6c 6c65 6374 696f 6e2c 0a20  reeCollection,. 
-000014d0: 2020 2020 2020 2020 2020 2049 4554 4344             IETCD
-000014e0: 7269 7665 722c 0a20 2020 2020 2020 2029  river,.        )
-000014f0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001500: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001510: 696e 7465 7266 6163 6573 2069 6d70 6f72  interfaces impor
-00001520: 7420 4944 6174 6153 6f75 7263 650a 2020  t IDataSource.  
-00001530: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
-00001540: 6174 615f 7365 7276 6963 6573 2e75 7469  ata_services.uti
-00001550: 6c73 2e63 6f6e 7665 7274 6572 7320 696d  ls.converters im
-00001560: 706f 7274 2028 0a20 2020 2020 2020 2020  port (.         
-00001570: 2020 2044 6174 6574 696d 6543 6f6e 7665     DatetimeConve
-00001580: 7274 6572 2c0a 2020 2020 2020 2020 2020  rter,.          
-00001590: 2020 4461 7465 7469 6d65 5374 7269 6e67    DatetimeString
-000015a0: 436f 6e76 6572 7465 722c 0a20 2020 2020  Converter,.     
-000015b0: 2020 2020 2020 2050 726f 746f 6275 6654         ProtobufT
-000015c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-000015d0: 722c 0a20 2020 2020 2020 2020 2020 2054  r,.            T
-000015e0: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
-000015f0: 7274 6572 2c0a 2020 2020 2020 2020 290a  rter,.        ).
-00001600: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001610: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00001350: 2d2d 3e0a 2020 2020 2020 2020 0a20 2020  -->.        .   
+00001360: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00001370: 2020 2020 2020 2066 726f 6d20 7479 7069         from typi
+00001380: 6e67 2069 6d70 6f72 7420 5475 706c 652c  ng import Tuple,
+00001390: 204c 6973 742c 204f 7074 696f 6e61 6c2c   List, Optional,
+000013a0: 2047 656e 6572 6174 6f72 0a20 2020 2020   Generator.     
+000013b0: 2020 2066 726f 6d20 6461 7465 7469 6d65     from datetime
+000013c0: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+000013d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000013e0: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+000013f0: 7365 7276 6963 6573 2e64 6174 6120 696d  services.data im
+00001400: 706f 7274 2044 6174 610a 2020 2020 2020  port Data.      
+00001410: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+00001420: 7365 7276 6963 6573 2e64 756d 6d79 2069  services.dummy i
+00001430: 6d70 6f72 7420 4475 6d6d 7944 6174 6153  mport DummyDataS
+00001440: 6f75 7263 650a 2020 2020 2020 2020 6672  ource.        fr
+00001450: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00001460: 6963 6573 2e65 7665 6e74 5f74 7265 6520  ices.event_tree 
+00001470: 696d 706f 7274 2028 0a20 2020 2020 2020  import (.       
+00001480: 2020 2020 2045 7665 6e74 5472 6565 2c0a       EventTree,.
+00001490: 2020 2020 2020 2020 2020 2020 4576 656e              Even
+000014a0: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+000014b0: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
+000014c0: 656e 7445 7665 6e74 5472 6565 436f 6c6c  entEventTreeColl
+000014d0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
+000014e0: 2020 2020 4945 5443 4472 6976 6572 2c0a      IETCDriver,.
+000014f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001500: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+00001510: 7365 7276 6963 6573 2e69 6e74 6572 6661  services.interfa
+00001520: 6365 7320 696d 706f 7274 2049 4461 7461  ces import IData
+00001530: 536f 7572 6365 0a20 2020 2020 2020 2066  Source.        f
+00001540: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001550: 7669 6365 732e 7574 696c 732e 636f 6e76  vices.utils.conv
+00001560: 6572 7465 7273 2069 6d70 6f72 7420 280a  erters import (.
+00001570: 2020 2020 2020 2020 2020 2020 4461 7465              Date
+00001580: 7469 6d65 436f 6e76 6572 7465 722c 0a20  timeConverter,. 
+00001590: 2020 2020 2020 2020 2020 2044 6174 6574             Datet
+000015a0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000015b0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000015c0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
+000015d0: 7043 6f6e 7665 7274 6572 2c0a 2020 2020  pConverter,.    
+000015e0: 2020 2020 2020 2020 5468 3254 696d 6573          Th2Times
+000015f0: 7461 6d70 436f 6e76 6572 7465 722c 0a20  tampConverter,. 
+00001600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00001610: 200a 2020 2020 2020 2020 2323 2323 2323   .        ######
 00001620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001630: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
-00001640: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
-00001650: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-00001660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001640: 0a20 2020 2020 2020 2023 205b 305d 204c  .        # [0] L
+00001650: 6962 2063 6f6e 6669 6775 7261 7469 6f6e  ib configuration
+00001660: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
 00001670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001680: 2323 2323 2323 0a20 2020 2020 2020 200a  ######.        .
-00001690: 2020 2020 2020 2020 2320 5b30 2e31 5d20          # [0.1] 
-000016a0: 496e 7465 7261 6374 6976 6520 6f72 2053  Interactive or S
-000016b0: 6372 6970 7420 6d6f 6465 0a20 2020 2020  cript mode.     
-000016c0: 2020 2023 2049 6620 796f 7520 7573 6520     # If you use 
-000016d0: 7468 6520 6c69 6220 696e 2069 6e74 6572  the lib in inter
-000016e0: 6163 7469 7665 206d 6f64 6520 286a 7570  active mode (jup
-000016f0: 7974 6572 2c20 6970 7974 686f 6e29 2069  yter, ipython) i
-00001700: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
-00001710: 746f 2073 6574 2074 6865 2073 7065 6369  to set the speci
-00001720: 616c 0a20 2020 2020 2020 2023 2067 6c6f  al.        # glo
-00001730: 6261 6c20 7061 7261 6d65 7465 7220 746f  bal parameter to
-00001740: 2054 7275 652e 2049 7427 6c6c 206b 6565   True. It'll kee
-00001750: 7020 6361 6368 6520 6669 6c65 7320 6966  p cache files if
-00001760: 2073 6f6d 6574 6869 6e67 2077 656e 7420   something went 
-00001770: 7772 6f6e 672e 0a20 2020 2020 2020 2066  wrong..        f
-00001780: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00001790: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
-000017a0: 6f72 7420 6f70 7469 6f6e 730a 2020 2020  ort options.    
-000017b0: 2020 2020 0a20 2020 2020 2020 206f 7074      .        opt
-000017c0: 696f 6e73 2e49 4e54 4552 4143 5449 5645  ions.INTERACTIVE
-000017d0: 5f4d 4f44 4520 3d20 5472 7565 0a20 2020  _MODE = True.   
-000017e0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-000017f0: 536f 6d65 2065 7861 6d70 6c65 2064 6174  Some example dat
-00001800: 610a 2020 2020 2020 2020 6576 656e 7473  a.        events
-00001810: 203d 2044 6174 6128 0a20 2020 2020 2020   = Data(.       
-00001820: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00001830: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00001840: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00001850: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001860: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001870: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-00001880: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-00001890: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-000018a0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2020 2020 2262 6174 6368 4964 223a 204e      "batchId": N
-000018d0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000018e0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
-000018f0: 6865 6422 3a20 4661 6c73 652c 0a20 2020  hed": False,.   
-00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001910: 2022 6576 656e 744e 616d 6522 3a20 2253   "eventName": "S
-00001920: 6574 206f 6620 6175 746f 2d67 656e 6572  et of auto-gener
-00001930: 6174 6564 2065 7665 6e74 7320 666f 7220  ated events for 
-00001940: 6473 206c 6962 2074 6573 7469 6e67 222c  ds lib testing",
-00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001960: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
-00001970: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
-00001980: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
-00001990: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
-000019a0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
-000019b0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-000019c0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
-000019d0: 3631 3735 3130 3030 7d2c 0a20 2020 2020  61751000},.     
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000019f0: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
-00001a00: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-00001a10: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
-00001a20: 6e6f 223a 2035 3630 3837 3330 3030 7d2c  no": 560873000},
-00001a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a40: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
-00001a50: 7449 6422 3a20 4e6f 6e65 2c0a 2020 2020  tId": None,.    
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
-00001a80: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001a90: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
-00001aa0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
-00001ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ac0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
-00001ad0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001af0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
-00001b00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
-00001b10: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
-00001b20: 6479 223a 205b 5d2c 0a20 2020 2020 2020  dy": [],.       
-00001b30: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001b40: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2265 7665 6e74 4964 223a 2022 6465    "eventId": "de
-00001b70: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
-00001b80: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
-00001b90: 3035 3536 3335 3232 3030 303a 3961 6462  05563522000:9adb
-00001ba0: 6233 6530 2d35 6638 622d 3463 3238 2d61  b3e0-5f8b-4c28-a
-00001bb0: 3261 632d 3733 3631 6538 6661 3730 3463  2ac-7361e8fa704c
-00001bc0: 3e64 656d 6f5f 626f 6f6b 5f31 3a74 6832  >demo_book_1:th2
-00001bd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-00001be0: 3335 3730 3535 3633 3532 3230 3030 3a64  35705563522000:d
-00001bf0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
-00001c00: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
-00001c10: 3532 645f 3222 2c0a 2020 2020 2020 2020  52d_2",.        
-00001c20: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
-00001c30: 6368 4964 223a 2022 6465 6d6f 5f62 6f6f  chId": "demo_boo
-00001c40: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
-00001c50: 3233 3031 3035 3133 3537 3035 3536 3335  2301051357055635
-00001c60: 3232 3030 303a 3961 6462 6233 6530 2d35  22000:9adbb3e0-5
-00001c70: 6638 622d 3463 3238 2d61 3261 632d 3733  f8b-4c28-a2ac-73
-00001c80: 3631 6538 6661 3730 3463 222c 0a20 2020  61e8fa704c",.   
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
-00001cb0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001cc0: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
-00001cd0: 6d65 223a 2022 506c 6169 6e20 6576 656e  me": "Plain even
-00001ce0: 7420 3122 2c0a 2020 2020 2020 2020 2020  t 1",.          
-00001cf0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00001d00: 5479 7065 223a 2022 6473 2d6c 6962 2d74  Type": "ds-lib-t
-00001d10: 6573 742d 6576 656e 7422 2c0a 2020 2020  est-event",.    
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
-00001d40: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
-00001d50: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
-00001d60: 6f22 3a20 3536 3336 3430 3030 307d 2c0a  o": 563640000},.
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2273 7461 7274 5469 6d65 7374      "startTimest
-00001d90: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
-00001da0: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
-00001db0: 2c20 226e 616e 6f22 3a20 3536 3335 3232  , "nano": 563522
-00001dc0: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
-00001dd0: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
-00001de0: 7445 7665 6e74 4964 223a 2022 6465 6d6f  tEventId": "demo
-00001df0: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00001e00: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00001e10: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
-00001e20: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
-00001e30: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
-00001e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001e50: 2020 2020 2020 2022 7375 6363 6573 7366         "successf
-00001e60: 756c 223a 2054 7275 652c 0a20 2020 2020  ul": True,.     
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001e80: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
-00001e90: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
-00001ea0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
-00001eb0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
-00001ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001ed0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
-00001ee0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
-00001f10: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
-00001f20: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
-00001f30: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
-00001f40: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001f70: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
-00001f80: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00001f90: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001fa0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
-00001fb0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
-00001fc0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
-00001fd0: 3730 3463 3e64 656d 6f5f 626f 6f6b 5f31  704c>demo_book_1
-00001fe0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001ff0: 3130 3531 3335 3730 3535 3633 3735 3730  1051357055637570
-00002000: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
-00002010: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
-00002020: 3135 3531 3532 645f 3322 2c0a 2020 2020  155152d_3",.    
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2262 6174 6368 4964 223a 2022 6465 6d6f  "batchId": "demo
-00002050: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00002060: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00002070: 3536 3335 3232 3030 303a 3961 6462 6233  563522000:9adbb3
-00002080: 6530 2d35 6638 622d 3463 3238 2d61 3261  e0-5f8b-4c28-a2a
-00002090: 632d 3733 3631 6538 6661 3730 3463 222c  c-7361e8fa704c",
-000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020b0: 2020 2020 2022 6973 4261 7463 6865 6422       "isBatched"
-000020c0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-000020d0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-000020e0: 6e74 4e61 6d65 223a 2022 506c 6169 6e20  ntName": "Plain 
-000020f0: 6576 656e 7420 3222 2c0a 2020 2020 2020  event 2",.      
-00002100: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00002110: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
-00002120: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
-00002150: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
-00002160: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
-00002170: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
-00002180: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-00002190: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
-000021a0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
-000021b0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
-000021c0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
-000021d0: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000021f0: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
-00002200: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-00002210: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-00002220: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
-00002230: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
-00002240: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
-00002250: 3264 5f31 222c 0a20 2020 2020 2020 2020  2d_1",.         
-00002260: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
-00002270: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
-000022a0: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
-000022d0: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
-000022e0: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
-000022f0: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
-00002300: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00002310: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
-00002320: 7b22 7479 7065 223a 2022 6d65 7373 6167  {"type": "messag
-00002330: 6522 2c20 2264 6174 6122 3a20 2264 732d  e", "data": "ds-
-00002340: 6c69 6220 7465 7374 2062 6f64 7922 7d2c  lib test body"},
-00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002360: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00002370: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00002380: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00002390: 4964 223a 2022 6661 6b65 2d65 7665 6e74  Id": "fake-event
-000023a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
-000023b0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-000023c0: 6422 3a20 2266 616b 652d 6261 7463 6849  d": "fake-batchI
-000023d0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-000023e0: 2020 2020 2020 2020 2269 7342 6174 6368          "isBatch
-000023f0: 6564 223a 2054 7275 652c 0a20 2020 2020  ed": True,.     
-00002400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002410: 6576 656e 744e 616d 6522 3a20 2246 616b  eventName": "Fak
-00002420: 6520 6576 656e 7422 2c0a 2020 2020 2020  e event",.      
-00002430: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00002440: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
-00002450: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
-00002480: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
-00002490: 6422 3a20 3136 3732 3932 3730 3335 2c20  d": 1672927035, 
-000024a0: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
-000024b0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-000024c0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
-000024d0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
-000024e0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
-000024f0: 3733 3235 2c20 226e 616e 6f22 3a20 3536  7325, "nano": 56
-00002500: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
-00002510: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00002520: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
-00002530: 6e6f 745f 6578 6973 7473 5f69 6e5f 7468  not_exists_in_th
-00002540: 655f 6576 656e 7473 5f73 7472 6561 6d22  e_events_stream"
-00002550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002560: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
-00002570: 6c22 3a20 4661 6c73 652c 0a20 2020 2020  l": False,.     
-00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002590: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
-000025a0: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
-000025b0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
-000025c0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
-000025d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000025e0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
-000025f0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
-00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002610: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
-00002620: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
-00002630: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
-00002640: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
-00002650: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00002660: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00002670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002680: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-00002690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000026a0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-000026b0: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
-000026c0: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
-000026d0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-000026e0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+00001680: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00001690: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000016a0: 2023 205b 302e 315d 2049 6e74 6572 6163   # [0.1] Interac
+000016b0: 7469 7665 206f 7220 5363 7269 7074 206d  tive or Script m
+000016c0: 6f64 650a 2020 2020 2020 2020 2320 4966  ode.        # If
+000016d0: 2079 6f75 2075 7365 2074 6865 206c 6962   you use the lib
+000016e0: 2069 6e20 696e 7465 7261 6374 6976 6520   in interactive 
+000016f0: 6d6f 6465 2028 6a75 7079 7465 722c 2069  mode (jupyter, i
+00001700: 7079 7468 6f6e 2920 6974 2773 2072 6563  python) it's rec
+00001710: 6f6d 6d65 6e64 6564 2074 6f20 7365 7420  ommended to set 
+00001720: 7468 6520 7370 6563 6961 6c0a 2020 2020  the special.    
+00001730: 2020 2020 2320 676c 6f62 616c 2070 6172      # global par
+00001740: 616d 6574 6572 2074 6f20 5472 7565 2e20  ameter to True. 
+00001750: 4974 276c 6c20 6b65 6570 2063 6163 6865  It'll keep cache
+00001760: 2066 696c 6573 2069 6620 736f 6d65 7468   files if someth
+00001770: 696e 6720 7765 6e74 2077 726f 6e67 2e0a  ing went wrong..
+00001780: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+00001790: 5f64 6174 615f 7365 7276 6963 6573 2e63  _data_services.c
+000017a0: 6f6e 6669 6720 696d 706f 7274 206f 7074  onfig import opt
+000017b0: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+000017c0: 2020 2020 2020 6f70 7469 6f6e 732e 494e        options.IN
+000017d0: 5445 5241 4354 4956 455f 4d4f 4445 203d  TERACTIVE_MODE =
+000017e0: 2054 7275 650a 2020 2020 2020 2020 0a20   True.        . 
+000017f0: 2020 2020 2020 2023 2053 6f6d 6520 6578         # Some ex
+00001800: 616d 706c 6520 6461 7461 0a20 2020 2020  ample data.     
+00001810: 2020 2065 7665 6e74 7320 3d20 4461 7461     events = Data
+00001820: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001850: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
+00001860: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00001870: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00001880: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00001890: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+000018a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000018b0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
+000018c0: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+000018d0: 7463 6849 6422 3a20 4e6f 6e65 2c0a 2020  tchId": None,.  
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2269 7342 6174 6368 6564 223a 2046    "isBatched": F
+00001900: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00001910: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00001920: 4e61 6d65 223a 2022 5365 7420 6f66 2061  Name": "Set of a
+00001930: 7574 6f2d 6765 6e65 7261 7465 6420 6576  uto-generated ev
+00001940: 656e 7473 2066 6f72 2064 7320 6c69 6220  ents for ds lib 
+00001950: 7465 7374 696e 6722 2c0a 2020 2020 2020  testing",.      
+00001960: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00001970: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00001980: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+000019b0: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+000019c0: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
+000019d0: 226e 616e 6f22 3a20 3536 3137 3531 3030  "nano": 56175100
+000019e0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+000019f0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+00001a00: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+00001a10: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+00001a20: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+00001a30: 3038 3733 3030 307d 2c0a 2020 2020 2020  0873000},.      
+00001a40: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00001a50: 6172 656e 7445 7665 6e74 4964 223a 204e  arentEventId": N
+00001a60: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001a70: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
+00001a80: 7366 756c 223a 2054 7275 652c 0a20 2020  sful": True,.   
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2022 626f 6f6b 4964 223a 2022 6465 6d6f   "bookId": "demo
+00001ab0: 5f62 6f6f 6b5f 3122 2c0a 2020 2020 2020  _book_1",.      
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001ad0: 636f 7065 223a 2022 7468 322d 7363 6f70  cope": "th2-scop
+00001ae0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001af0: 2020 2020 2020 2020 2261 7474 6163 6865          "attache
+00001b00: 644d 6573 7361 6765 4964 7322 3a20 5b5d  dMessageIds": []
+00001b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b20: 2020 2020 2020 2262 6f64 7922 3a20 5b5d        "body": []
+00001b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00001b50: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001b60: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00001b70: 7449 6422 3a20 2264 656d 6f5f 626f 6f6b  tId": "demo_book
+00001b80: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001b90: 3330 3130 3531 3335 3730 3535 3633 3532  3010513570556352
+00001ba0: 3230 3030 3a39 6164 6262 3365 302d 3566  2000:9adbb3e0-5f
+00001bb0: 3862 2d34 6332 382d 6132 6163 2d37 3336  8b-4c28-a2ac-736
+00001bc0: 3165 3866 6137 3034 633e 6465 6d6f 5f62  1e8fa704c>demo_b
+00001bd0: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00001be0: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+00001bf0: 3335 3232 3030 303a 6436 3165 3933 3061  3522000:d61e930a
+00001c00: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+00001c10: 6433 3461 3631 3535 3135 3264 5f32 222c  d34a6155152d_2",
+00001c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c30: 2020 2020 2022 6261 7463 6849 6422 3a20       "batchId": 
+00001c40: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
+00001c50: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+00001c60: 3335 3730 3535 3633 3532 3230 3030 3a39  35705563522000:9
+00001c70: 6164 6262 3365 302d 3566 3862 2d34 6332  adbb3e0-5f8b-4c2
+00001c80: 382d 6132 6163 2d37 3336 3165 3866 6137  8-a2ac-7361e8fa7
+00001c90: 3034 6322 2c0a 2020 2020 2020 2020 2020  04c",.          
+00001ca0: 2020 2020 2020 2020 2020 2269 7342 6174            "isBat
+00001cb0: 6368 6564 223a 2054 7275 652c 0a20 2020  ched": True,.   
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2022 6576 656e 744e 616d 6522 3a20 2250   "eventName": "P
+00001ce0: 6c61 696e 2065 7665 6e74 2031 222c 0a20  lain event 1",. 
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 2020 2022 6576 656e 7454 7970 6522 3a20     "eventType": 
+00001d10: 2264 732d 6c69 622d 7465 7374 2d65 7665  "ds-lib-test-eve
+00001d20: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+00001d30: 2020 2020 2020 2020 2022 656e 6454 696d           "endTim
+00001d40: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
+00001d50: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
+00001d60: 3032 352c 2022 6e61 6e6f 223a 2035 3633  025, "nano": 563
+00001d70: 3634 3030 3030 7d2c 0a20 2020 2020 2020  640000},.       
+00001d80: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00001d90: 6172 7454 696d 6573 7461 6d70 223a 207b  artTimestamp": {
+00001da0: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001db0: 3637 3239 3237 3032 352c 2022 6e61 6e6f  672927025, "nano
+00001dc0: 223a 2035 3633 3532 3230 3030 7d2c 0a20  ": 563522000},. 
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
+00001df0: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001e00: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001e10: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
+00001e20: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00001e30: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00001e40: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
+00001e70: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001e80: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+00001e90: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+00001ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001eb0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+00001ec0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001ee0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00001ef0: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00001f00: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00001f10: 6479 223a 207b 2274 7970 6522 3a20 226d  dy": {"type": "m
+00001f20: 6573 7361 6765 222c 2022 6461 7461 223a  essage", "data":
+00001f30: 2022 6473 2d6c 6962 2074 6573 7420 626f   "ds-lib test bo
+00001f40: 6479 227d 2c0a 2020 2020 2020 2020 2020  dy"},.          
+00001f50: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001f60: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001f80: 6576 656e 7449 6422 3a20 2264 656d 6f5f  eventId": "demo_
+00001f90: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
+00001fa0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
+00001fb0: 3633 3532 3230 3030 3a39 6164 6262 3365  63522000:9adbb3e
+00001fc0: 302d 3566 3862 2d34 6332 382d 6132 6163  0-5f8b-4c28-a2ac
+00001fd0: 2d37 3336 3165 3866 6137 3034 633e 6465  -7361e8fa704c>de
+00001fe0: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
+00001ff0: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
+00002000: 3035 3536 3337 3537 3030 303a 6436 3165  05563757000:d61e
+00002010: 3933 3061 2d38 6430 302d 3131 6564 2d61  930a-8d00-11ed-a
+00002020: 6131 612d 6433 3461 3631 3535 3135 3264  a1a-d34a6155152d
+00002030: 5f33 222c 0a20 2020 2020 2020 2020 2020  _3",.           
+00002040: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+00002050: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00002060: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00002070: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
+00002080: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
+00002090: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
+000020a0: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+000020c0: 7342 6174 6368 6564 223a 2054 7275 652c  sBatched": True,
+000020d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020e0: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
+000020f0: 3a20 2250 6c61 696e 2065 7665 6e74 2032  : "Plain event 2
+00002100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002110: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
+00002120: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
+00002130: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
+00002140: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+00002150: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
+00002160: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
+00002170: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
+00002180: 2035 3633 3739 3130 3030 7d2c 0a20 2020   563791000},.   
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
+000021b0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
+000021c0: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
+000021d0: 6e61 6e6f 223a 2035 3633 3735 3730 3030  nano": 563757000
+000021e0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000021f0: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
+00002200: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00002210: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00002220: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+00002230: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+00002240: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+00002250: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
+00002280: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+00002290: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
+000022a0: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
+000022b0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
+000022c0: 2020 2020 2020 2020 2022 7363 6f70 6522           "scope"
+000022d0: 3a20 2274 6832 2d73 636f 7065 222c 0a20  : "th2-scope",. 
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
+00002300: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2022 626f 6479 223a 207b 2274 7970 6522   "body": {"type"
+00002330: 3a20 226d 6573 7361 6765 222c 2022 6461  : "message", "da
+00002340: 7461 223a 2022 6473 2d6c 6962 2074 6573  ta": "ds-lib tes
+00002350: 7420 626f 6479 227d 2c0a 2020 2020 2020  t body"},.      
+00002360: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00002370: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2022 6576 656e 7449 6422 3a20 2266     "eventId": "f
+000023a0: 616b 652d 6576 656e 7449 6422 2c0a 2020  ake-eventId",.  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2262 6174 6368 4964 223a 2022 6661    "batchId": "fa
+000023d0: 6b65 2d62 6174 6368 4964 222c 0a20 2020  ke-batchId",.   
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
+00002400: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00002410: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
+00002420: 6d65 223a 2022 4661 6b65 2065 7665 6e74  me": "Fake event
+00002430: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002440: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
+00002450: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
+00002460: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
+00002470: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+00002480: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
+00002490: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
+000024a0: 3239 3237 3033 352c 2022 6e61 6e6f 223a  2927035, "nano":
+000024b0: 2035 3633 3739 3130 3030 7d2c 0a20 2020   563791000},.   
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
+000024e0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
+000024f0: 223a 2031 3637 3239 3237 3332 352c 2022  ": 1672927325, "
+00002500: 6e61 6e6f 223a 2035 3633 3735 3730 3030  nano": 563757000
+00002510: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00002520: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
+00002530: 656e 7449 6422 3a20 226e 6f74 5f65 7869  entId": "not_exi
+00002540: 7374 735f 696e 5f74 6865 5f65 7665 6e74  sts_in_the_event
+00002550: 735f 7374 7265 616d 222c 0a20 2020 2020  s_stream",.     
+00002560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002570: 7375 6363 6573 7366 756c 223a 2046 616c  successful": Fal
+00002580: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002590: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+000025a0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+000025b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025c0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+000025d0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000025f0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00002600: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00002610: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00002620: 6479 223a 207b 2274 7970 6522 3a20 226d  dy": {"type": "m
+00002630: 6573 7361 6765 222c 2022 6461 7461 223a  essage", "data":
+00002640: 2022 6473 2d6c 6962 2074 6573 7420 626f   "ds-lib test bo
+00002650: 6479 227d 2c0a 2020 2020 2020 2020 2020  dy"},.          
+00002660: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002670: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
+00002680: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002690: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+000026a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000026b0: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+000026c0: 2023 205b 315d 2057 6f72 6b69 6e67 2077   # [1] Working w
+000026d0: 6974 6820 6120 4461 7461 206f 626a 6563  ith a Data objec
+000026e0: 742e 0a20 2020 2020 2020 2023 2323 2323  t..        #####
 000026f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002700: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
-00002710: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
-00002720: 5d20 4669 6c74 6572 2e0a 2020 2020 2020  ] Filter..      
-00002730: 2020 6669 6c74 6572 6564 5f65 7665 6e74    filtered_event
-00002740: 733a 2044 6174 6120 3d20 6576 656e 7473  s: Data = events
-00002750: 2e66 696c 7465 7228 6c61 6d62 6461 2065  .filter(lambda e
-00002760: 3a20 655b 2262 6f64 7922 5d20 213d 205b  : e["body"] != [
-00002770: 5d29 2020 2320 4669 6c74 6572 2065 7665  ])  # Filter eve
-00002780: 6e74 7320 7769 7468 2065 6d70 7479 2062  nts with empty b
-00002790: 6f64 792e 0a20 2020 2020 2020 200a 2020  ody..        .  
-000027a0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000027b0: 205b 312e 325d 204d 6170 2e0a 2020 2020   [1.2] Map..    
-000027c0: 2020 2020 6465 6620 7472 616e 7366 6f72      def transfor
-000027d0: 6d5f 6675 6e63 7469 6f6e 2872 6563 6f72  m_function(recor
-000027e0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-000027f0: 7265 7475 726e 207b 2265 7665 6e74 4e61  return {"eventNa
-00002800: 6d65 223a 2072 6563 6f72 645b 2265 7665  me": record["eve
-00002810: 6e74 4e61 6d65 225d 2c20 2273 7563 6365  ntName"], "succe
-00002820: 7373 6675 6c22 3a20 7265 636f 7264 5b22  ssful": record["
-00002830: 7375 6363 6573 7366 756c 225d 7d0a 2020  successful"]}.  
-00002840: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-00002850: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
-00002860: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
-00002870: 7473 203d 2066 696c 7465 7265 645f 6576  ts = filtered_ev
-00002880: 656e 7473 2e6d 6170 2874 7261 6e73 666f  ents.map(transfo
-00002890: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
-000028a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-000028b0: 5b31 2e33 5d20 4461 7461 2070 6970 656c  [1.3] Data pipel
-000028c0: 696e 652e 0a20 2020 2020 2020 2023 2020  ine..        #  
-000028d0: 2020 2020 2049 6e73 7465 6164 206f 6620       Instead of 
-000028e0: 646f 696e 6720 6461 7461 2074 7261 6e73  doing data trans
-000028f0: 666f 726d 6174 696f 6e73 2073 7465 7020  formations step 
-00002900: 6279 2073 7465 7020 796f 7520 6361 6e20  by step you can 
-00002910: 646f 2069 7420 696e 206f 6e65 206c 696e  do it in one lin
-00002920: 652e 0a20 2020 2020 2020 2066 696c 7465  e..        filte
-00002930: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
-00002940: 7665 6e74 735f 6279 5f70 6970 656c 696e  vents_by_pipelin
-00002950: 6520 3d20 6576 656e 7473 2e66 696c 7465  e = events.filte
-00002960: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
-00002970: 6f64 7922 5d20 213d 205b 5d29 2e6d 6170  ody"] != []).map
-00002980: 280a 2020 2020 2020 2020 2020 2020 7472  (.            tr
-00002990: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
-000029a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000029b0: 2020 2023 2043 6f6e 7465 6e74 206f 6620     # Content of 
-000029c0: 7468 6573 6520 7477 6f20 4461 7461 206f  these two Data o
-000029d0: 626a 6563 7473 2073 686f 756c 6420 6265  bjects should be
-000029e0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
-000029f0: 6173 7365 7274 206c 6973 7428 6669 6c74  assert list(filt
-00002a00: 6572 6564 5f61 6e64 5f6d 6170 7065 645f  ered_and_mapped_
-00002a10: 6576 656e 7473 2920 3d3d 206c 6973 7428  events) == list(
-00002a20: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
-00002a30: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
-00002a40: 7065 6c69 6e65 290a 2020 2020 2020 2020  peline).        
-00002a50: 0a20 2020 2020 2020 2023 205b 312e 345d  .        # [1.4]
-00002a60: 2053 6966 742e 2053 6b69 7020 7468 6520   Sift. Skip the 
-00002a70: 6669 7273 7420 6665 7720 6974 656d 7320  first few items 
-00002a80: 6f72 206c 696d 6974 2074 6865 6d2e 0a20  or limit them.. 
-00002a90: 2020 2020 2020 2064 6174 6120 3d20 4461         data = Da
-00002aa0: 7461 285b 312c 2032 2c20 332c 2034 2c20  ta([1, 2, 3, 4, 
-00002ab0: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
-00002ac0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
-00002ad0: 342c 2031 355d 290a 2020 2020 2020 2020  4, 15]).        
-00002ae0: 6974 656d 735f 6672 6f6d 5f31 315f 746f  items_from_11_to
-00002af0: 5f65 6e64 3a20 4765 6e65 7261 746f 7220  _end: Generator 
-00002b00: 3d20 6461 7461 2e73 6966 7428 736b 6970  = data.sift(skip
-00002b10: 3d31 3029 0a20 2020 2020 2020 206f 6e6c  =10).        onl
-00002b20: 795f 6669 7273 745f 3130 5f69 7465 6d73  y_first_10_items
-00002b30: 3a20 4765 6e65 7261 746f 7220 3d20 6461  : Generator = da
-00002b40: 7461 2e73 6966 7428 6c69 6d69 743d 3130  ta.sift(limit=10
-00002b50: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002b60: 2020 2023 205b 312e 355d 2043 6861 6e67     # [1.5] Chang
-00002b70: 696e 6720 6361 6368 6520 7374 6174 7573  ing cache status
-00002b80: 2e0a 2020 2020 2020 2020 6576 656e 7473  ..        events
-00002b90: 2e75 7365 5f63 6163 6865 2854 7275 6529  .use_cache(True)
-00002ba0: 0a20 2020 2020 2020 2023 206f 7220 6a75  .        # or ju
-00002bb0: 7374 0a20 2020 2020 2020 2065 7665 6e74  st.        event
-00002bc0: 732e 7573 655f 6361 6368 6528 2920 2023  s.use_cache()  #
-00002bd0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
-00002be0: 6163 7469 7661 7465 2063 6163 6865 2e0a  activate cache..
-00002bf0: 2020 2020 2020 2020 2320 5b31 2e36 5d20          # [1.6] 
-00002c00: 5761 6c6b 2074 6872 6f75 6768 2064 6174  Walk through dat
-00002c10: 612e 0a20 2020 2020 2020 2066 6f72 2065  a..        for e
-00002c20: 7665 6e74 2069 6e20 6576 656e 7473 3a0a  vent in events:.
-00002c30: 2020 2020 2020 2020 2020 2020 2320 446f              # Do
-00002c40: 2073 6f6d 6574 6869 6e67 2077 6974 6820   something with 
-00002c50: 6576 656e 7420 2865 7665 6e74 2069 7320  event (event is 
-00002c60: 6120 6469 6374 292e 0a20 2020 2020 2020  a dict)..       
-00002c70: 2020 2020 2070 7269 6e74 2865 7665 6e74       print(event
-00002c80: 290a 2020 2020 2020 2020 2320 4166 7465  ).        # Afte
-00002c90: 7220 6669 7273 7420 6974 6572 6174 696f  r first iteratio
-00002ca0: 6e20 7468 6520 6576 656e 7473 2068 6173  n the events has
-00002cb0: 2061 2063 6163 6865 2066 696c 652e 0a20   a cache file.. 
-00002cc0: 2020 2020 2020 2023 204e 6f77 2074 6865         # Now the
-00002cd0: 7920 7769 6c6c 2062 6520 7573 6564 2069  y will be used i
-00002ce0: 6e20 7468 6520 6361 6368 6520 696e 2074  n the cache in t
-00002cf0: 6865 206e 6578 7420 6974 6572 6174 696f  he next iteratio
-00002d00: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00002d10: 2020 2020 2320 5b31 2e37 5d20 4765 7420      # [1.7] Get 
-00002d20: 6e75 6d62 6572 206f 6620 7468 6520 656c  number of the el
-00002d30: 656d 656e 7473 2069 6e20 7468 6520 4461  ements in the Da
-00002d40: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
-00002d50: 2020 206e 756d 6265 725f 6f66 5f65 7665     number_of_eve
-00002d60: 6e74 7320 3d20 6576 656e 7473 2e6c 656e  nts = events.len
-00002d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002d80: 2020 2320 5b31 2e38 5d20 4368 6563 6b20    # [1.8] Check 
-00002d90: 7468 6174 2044 6174 6120 6f62 6a65 6374  that Data object
-00002da0: 2069 736e 2774 2065 6d70 7479 2e0a 2020   isn't empty..  
-00002db0: 2020 2020 2020 2320 5468 6520 6461 7461        # The data
-00002dc0: 2073 6f75 7263 6520 7368 6f75 6c64 2062   source should b
-00002dd0: 6520 6e6f 7420 656d 7074 792e 0a20 2020  e not empty..   
-00002de0: 2020 2020 2061 7373 6572 7420 6576 656e       assert even
-00002df0: 7473 2e69 735f 656d 7074 7920 6973 2046  ts.is_empty is F
-00002e00: 616c 7365 0a20 2020 2020 2020 200a 2020  alse.        .  
-00002e10: 2020 2020 2020 2320 5b31 2e39 5d20 436f        # [1.9] Co
-00002e20: 6e76 6572 7420 4461 7461 206f 626a 6563  nvert Data objec
-00002e30: 7420 746f 2074 6865 206c 6973 7420 6f66  t to the list of
-00002e40: 2065 6c65 6d65 6e74 7328 6576 656e 7473   elements(events
-00002e50: 206f 7220 6d65 7373 6167 6573 292e 0a20   or messages).. 
-00002e60: 2020 2020 2020 2023 2042 6520 6361 7265         # Be care
-00002e70: 6675 6c2c 2074 6869 7320 6361 6e20 7461  ful, this can ta
-00002e80: 6b65 2074 6f6f 206d 7563 6820 6d65 6d6f  ke too much memo
-00002e90: 7279 2e0a 2020 2020 2020 2020 6576 656e  ry..        even
-00002ea0: 7473 5f6c 6973 7420 3d20 6c69 7374 2865  ts_list = list(e
-00002eb0: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
-00002ec0: 2020 2020 2020 2020 2320 5b31 2e31 305d          # [1.10]
-00002ed0: 2054 6865 2063 6163 6865 2069 6e68 6572   The cache inher
-00002ee0: 6974 616e 6365 2e0a 2020 2020 2020 2020  itance..        
-00002ef0: 2320 4372 6561 7465 7320 6120 6e65 7720  # Creates a new 
-00002f00: 4461 7461 206f 626a 6563 7420 7468 6174  Data object that
-00002f10: 2077 696c 6c20 7573 6520 6361 6368 6520   will use cache 
-00002f20: 6672 6f6d 2074 6865 2065 7665 6e74 7320  from the events 
-00002f30: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
-00002f40: 2020 2020 2065 7665 6e74 735f 6669 6c74       events_filt
-00002f50: 6572 6564 3a20 4461 7461 203d 2065 7665  ered: Data = eve
-00002f60: 6e74 732e 6669 6c74 6572 286c 616d 6264  nts.filter(lambd
-00002f70: 6120 7265 636f 7264 3a20 7265 636f 7264  a record: record
-00002f80: 2e67 6574 2822 6261 7463 6849 6422 2929  .get("batchId"))
-00002f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002fa0: 2020 2320 4e65 7720 4461 7461 206f 626a    # New Data obj
-00002fb0: 6563 7473 2064 6f6e 2774 2075 7365 2074  ects don't use t
-00002fc0: 6865 6972 206f 776e 2063 6163 6865 2062  heir own cache b
-00002fd0: 7920 6465 6661 756c 7420 6275 7420 7573  y default but us
-00002fe0: 6520 7468 6520 6361 6368 6520 6f66 2074  e the cache of t
-00002ff0: 6865 2070 6172 656e 7420 4461 7461 206f  he parent Data o
-00003000: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
-00003010: 2055 7365 2075 7365 5f63 6163 6865 206d   Use use_cache m
-00003020: 6574 686f 6420 746f 2061 6374 6976 6174  ethod to activat
-00003030: 6520 6361 6368 696e 672e 0a20 2020 2020  e caching..     
-00003040: 2020 2023 2041 6674 6572 2074 6861 742c     # After that,
-00003050: 2074 6865 2044 6174 6120 6f62 6a65 6374   the Data object
-00003060: 2077 696c 6c20 6372 6561 7465 2069 7473   will create its
-00003070: 206f 776e 2063 6163 6865 2066 696c 652e   own cache file.
-00003080: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
-00003090: 6669 6c74 6572 6564 2e75 7365 5f63 6163  filtered.use_cac
-000030a0: 6865 2829 0a20 2020 2020 2020 200a 2020  he().        .  
-000030b0: 2020 2020 2020 6c69 7374 2865 7665 6e74        list(event
-000030c0: 735f 6669 6c74 6572 6564 2920 2023 204a  s_filtered)  # J
-000030d0: 7573 7420 746f 2069 7465 7261 7465 2044  ust to iterate D
-000030e0: 6174 6120 6f62 6a65 6374 2028 6361 6368  ata object (cach
-000030f0: 6520 6669 6c65 2077 696c 6c20 6265 2063  e file will be c
-00003100: 7265 6174 6564 292e 0a20 2020 2020 2020  reated)..       
-00003110: 200a 2020 2020 2020 2020 6669 6c74 6572   .        filter
-00003120: 6564 5f65 7665 6e74 735f 7479 7065 7320  ed_events_types 
-00003130: 3d20 6576 656e 7473 5f66 696c 7465 7265  = events_filtere
-00003140: 642e 6d61 7028 6c61 6d62 6461 2072 6563  d.map(lambda rec
-00003150: 6f72 643a 207b 2265 7665 6e74 5479 7065  ord: {"eventType
-00003160: 223a 2072 6563 6f72 642e 6765 7428 2265  ": record.get("e
-00003170: 7665 6e74 5479 7065 2229 7d29 0a20 2020  ventType")}).   
-00003180: 2020 2020 200a 2020 2020 2020 2020 6576       .        ev
-00003190: 656e 7473 5f77 6974 686f 7574 5f74 7970  ents_without_typ
-000031a0: 6573 5f77 6974 685f 6261 7463 6820 3d20  es_with_batch = 
-000031b0: 6669 6c74 6572 6564 5f65 7665 6e74 735f  filtered_events_
-000031c0: 7479 7065 732e 6669 6c74 6572 280a 2020  types.filter(.  
-000031d0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-000031e0: 2072 6563 6f72 643a 206e 6f74 2072 6563   record: not rec
-000031f0: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
-00003200: 7065 2229 0a20 2020 2020 2020 2029 0a20  pe").        ). 
-00003210: 2020 2020 2020 2065 7665 6e74 735f 7769         events_wi
-00003220: 7468 6f75 745f 7479 7065 735f 7769 7468  thout_types_with
-00003230: 5f62 6174 6368 2e75 7365 5f63 6163 6865  _batch.use_cache
-00003240: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-00003250: 2020 2020 2320 5b31 2e31 315d 2044 6174      # [1.11] Dat
-00003260: 6120 6f62 6a65 6374 7320 6a6f 696e 696e  a objects joinin
-00003270: 672e 0a20 2020 2020 2020 2023 2059 6f75  g..        # You
-00003280: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
-00003290: 696e 6720 3320 4461 7461 206f 626a 6563  ing 3 Data objec
-000032a0: 7473 2e0a 2020 2020 2020 2020 6431 203d  ts..        d1 =
-000032b0: 2044 6174 6128 5b31 2c20 322c 2033 5d29   Data([1, 2, 3])
-000032c0: 0a20 2020 2020 2020 2064 3220 3d20 4461  .        d2 = Da
-000032d0: 7461 285b 2261 222c 207b 2269 6422 3a20  ta(["a", {"id": 
-000032e0: 3132 337d 2c20 2263 225d 290a 2020 2020  123}, "c"]).    
-000032f0: 2020 2020 6433 203d 2044 6174 6128 5b37      d3 = Data([7
-00003300: 2c20 382c 2039 5d29 0a20 2020 2020 2020  , 8, 9]).       
-00003310: 2023 2059 6f75 2063 616e 206a 6f69 6e20   # You can join 
-00003320: 4461 7461 206f 626a 6563 7473 2069 6e20  Data objects in 
-00003330: 666f 6c6c 6f77 696e 6720 7761 7973 2e0a  following ways..
-00003340: 2020 2020 2020 2020 2320 506c 6561 7365          # Please
-00003350: 206e 6f74 652c 206e 6577 2044 6174 6120   note, new Data 
-00003360: 6f62 6a65 6374 2077 696c 6c20 6861 7665  object will have
-00003370: 2063 6163 6865 2073 7461 7475 7320 3d3d   cache status ==
-00003380: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00003390: 6461 7461 5f76 6961 5f69 6e69 7420 3d20  data_via_init = 
-000033a0: 4461 7461 285b 6431 2c20 6432 2c20 6433  Data([d1, d2, d3
-000033b0: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
-000033c0: 7669 615f 6164 6420 3d20 6431 202b 2064  via_add = d1 + d
-000033d0: 3220 2b20 6433 0a20 2020 2020 2020 2064  2 + d3.        d
-000033e0: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
-000033f0: 615f 6f62 6a5f 7669 615f 696e 6974 203d  a_obj_via_init =
-00003400: 2044 6174 6128 5b64 312c 205b 2261 222c   Data([d1, ["a",
-00003410: 207b 2269 6422 3a20 3132 337d 2c20 2263   {"id": 123}, "c
-00003420: 225d 2c20 6433 5d29 0a20 2020 2020 2020  "], d3]).       
-00003430: 2064 6174 615f 7769 7468 5f6e 6f6e 5f64   data_with_non_d
-00003440: 6174 615f 6f62 6a5f 7669 615f 6164 6420  ata_obj_via_add 
-00003450: 3d20 6431 202b 205b 2261 222c 207b 2269  = d1 + ["a", {"i
-00003460: 6422 3a20 3132 337d 2c20 2263 225d 202b  d": 123}, "c"] +
-00003470: 2064 330a 2020 2020 2020 2020 2320 596f   d3.        # Yo
-00003480: 7520 6361 6e20 6a6f 696e 2063 7572 7265  u can join curre
-00003490: 6e74 2044 6174 6120 6f62 6a65 6374 206f  nt Data object o
-000034a0: 6e20 706c 6163 6520 7573 696e 6720 2b3d  n place using +=
-000034b0: 2e0a 2020 2020 2020 2020 2320 4974 2077  ..        # It w
-000034c0: 696c 6c20 6b65 6570 2063 6163 6865 2073  ill keep cache s
-000034d0: 7461 7475 732e 0a20 2020 2020 2020 2064  tatus..        d
-000034e0: 3120 2b3d 2064 3320 2023 2064 3120 7769  1 += d3  # d1 wi
-000034f0: 6c6c 2062 6563 6f6d 6520 4461 7461 285b  ll become Data([
-00003500: 312c 322c 332c 372c 382c 395d 290a 2020  1,2,3,7,8,9]).  
-00003510: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003520: 205b 312e 3132 5d20 4275 696c 6420 616e   [1.12] Build an
-00003530: 6420 7265 6164 2044 6174 6120 6f62 6a65  d read Data obje
-00003540: 6374 2063 6163 6865 2066 696c 6573 2e0a  ct cache files..
-00003550: 2020 2020 2020 2020 6576 656e 7473 2e62          events.b
-00003560: 7569 6c64 5f63 6163 6865 2822 6361 6368  uild_cache("cach
-00003570: 655f 6669 6c65 6e61 6d65 5f6f 725f 7061  e_filename_or_pa
-00003580: 7468 2229 0a20 2020 2020 2020 2064 6174  th").        dat
-00003590: 615f 6f62 6a5f 6672 6f6d 5f63 6163 6865  a_obj_from_cache
-000035a0: 203d 2044 6174 612e 6672 6f6d 5f63 6163   = Data.from_cac
-000035b0: 6865 5f66 696c 6528 2263 6163 6865 5f66  he_file("cache_f
-000035c0: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
-000035d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000035e0: 2020 2023 205b 312e 3133 5d20 4368 6563     # [1.13] Chec
-000035f0: 6b20 6966 2044 6174 6120 6973 2073 6f72  k if Data is sor
-00003600: 7465 642e 0a20 2020 2020 2020 2023 2054  ted..        # T
-00003610: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
-00003620: 616e 206f 626a 6563 7420 6069 735f 736f  an object `is_so
-00003630: 7274 6564 6020 7468 6174 2063 6f6e 7461  rted` that conta
-00003640: 696e 7320 696e 666f 726d 6174 696f 6e0a  ins information.
-00003650: 2020 2020 2020 2020 2320 2020 312e 2073          #   1. s
-00003660: 7461 7475 7320 2d2d 2073 6f72 7465 6420  tatus -- sorted 
-00003670: 6f72 206e 6f74 0a20 2020 2020 2020 2023  or not.        #
-00003680: 2020 2032 2e20 6669 7273 745f 756e 736f     2. first_unso
-00003690: 7274 6564 202d 2d20 7468 6520 696e 6465  rted -- the inde
-000036a0: 7820 6f66 2074 6865 2066 6972 7374 2075  x of the first u
-000036b0: 6e73 6f72 7465 6420 656c 656d 656e 740a  nsorted element.
-000036c0: 2020 2020 2020 2020 6973 5f73 6f72 7465          is_sorte
-000036d0: 6420 3d20 6576 656e 7473 2e69 735f 736f  d = events.is_so
-000036e0: 7274 6564 286c 616d 6264 6120 653a 2065  rted(lambda e: e
-000036f0: 5b22 7374 6172 7454 696d 6573 7461 6d70  ["startTimestamp
-00003700: 225d 5b22 6570 6f63 6853 6563 6f6e 6422  "]["epochSecond"
-00003710: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
-00003720: 2020 2020 2320 596f 7520 6361 6e20 7573      # You can us
-00003730: 6520 7468 6973 206f 626a 6563 7420 6173  e this object as
-00003740: 2075 7375 616c 2062 6f6f 6c20 7661 7269   usual bool vari
-00003750: 6162 6c65 2e0a 2020 2020 2020 2020 6966  able..        if
-00003760: 2069 735f 736f 7274 6564 3a0a 2020 2020   is_sorted:.    
-00003770: 2020 2020 2020 2020 7072 696e 7428 2265          print("e
-00003780: 7665 6e74 7320 4461 7461 206f 626a 2069  vents Data obj i
-00003790: 7320 736f 7274 6564 2122 290a 2020 2020  s sorted!").    
-000037a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000037b0: 312e 3134 5d20 5573 6520 6044 6174 612e  1.14] Use `Data.
-000037c0: 7368 6f77 2829 6020 746f 206c 6f6f 6b20  show()` to look 
-000037d0: 6174 2074 6865 2066 6972 7374 204e 206d  at the first N m
-000037e0: 6573 7361 6765 7320 696e 2074 6865 2073  essages in the s
-000037f0: 7472 6561 6d2e 0a20 2020 2020 2020 2064  tream..        d
-00003800: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
-00003810: 615f 6f62 6a5f 7669 615f 6164 642e 7368  a_obj_via_add.sh
-00003820: 6f77 286e 3d36 290a 2020 2020 2020 2020  ow(n=6).        
-00003830: 2320 5769 6c6c 2070 7269 6e74 0a20 2020  # Will print.   
-00003840: 2020 2020 2023 202d 2d2d 2d2d 2d2d 2d2d       # ---------
-00003850: 2d2d 2d2d 2050 7269 6e74 6564 2066 6972  ---- Printed fir
-00003860: 7374 2036 2072 6563 6f72 6473 202d 2d2d  st 6 records ---
-00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00003880: 2020 2023 205b 315d 202d 2d2d 2d2d 2d0a     # [1] ------.
-00003890: 2020 2020 2020 2020 2320 310a 2020 2020          # 1.    
-000038a0: 2020 2020 2320 5b32 5d20 2d2d 2d2d 2d2d      # [2] ------
-000038b0: 0a20 2020 2020 2020 2023 2032 0a20 2020  .        # 2.   
-000038c0: 2020 2020 2023 205b 335d 202d 2d2d 2d2d       # [3] -----
-000038d0: 2d0a 2020 2020 2020 2020 2320 330a 2020  -.        # 3.  
-000038e0: 2020 2020 2020 2320 5b34 5d20 2d2d 2d2d        # [4] ----
-000038f0: 2d2d 0a20 2020 2020 2020 2023 2027 6127  --.        # 'a'
-00003900: 0a20 2020 2020 2020 2023 205b 355d 202d  .        # [5] -
-00003910: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
-00003920: 7b27 6964 273a 2031 3233 7d0a 2020 2020  {'id': 123}.    
-00003930: 2020 2020 2320 5b36 5d20 2d2d 2d2d 2d2d      # [6] ------
-00003940: 0a20 2020 2020 2020 2023 2027 6327 0a20  .        # 'c'. 
-00003950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003960: 2320 5b31 2e31 355d 2059 6f75 2063 616e  # [1.15] You can
-00003970: 2072 656d 6f76 6520 7468 6520 6361 6368   remove the cach
-00003980: 6520 6669 6c65 206f 6620 7468 6520 4461  e file of the Da
-00003990: 7461 206f 626a 6563 742c 2069 6620 7265  ta object, if re
-000039a0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-000039b0: 6461 7461 5f6f 626a 5f66 726f 6d5f 6361  data_obj_from_ca
-000039c0: 6368 652e 636c 6561 725f 6361 6368 6528  che.clear_cache(
-000039d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000039e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-000039f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003a00: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
-00003a10: 2020 2320 5b32 5d20 576f 726b 696e 6720    # [2] Working 
-00003a20: 7769 7468 2063 6f6e 7665 7274 6572 732e  with converters.
-00003a30: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-00003a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003a50: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00003a60: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
-00003a70: 6172 6520 6375 7272 656e 746c 7920 7468  are currently th
-00003a80: 7265 6520 696d 706c 656d 656e 7461 7469  ree implementati
-00003a90: 6f6e 7320 6f66 2049 5469 6d65 7374 616d  ons of ITimestam
-00003aa0: 7043 6f6e 7665 7274 6572 2063 6c61 7373  pConverter class
-00003ab0: 3a20 4461 7465 7469 6d65 436f 6e76 6572  : DatetimeConver
-00003ac0: 7465 2c20 4461 7465 7469 6d65 5374 7269  te, DatetimeStri
-00003ad0: 6e67 436f 6e76 6572 7465 7220 616e 6420  ngConverter and 
-00003ae0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
-00003af0: 7043 6f6e 7665 7274 6572 2e0a 2020 2020  pConverter..    
-00003b00: 2020 2020 2320 5468 6579 2061 6c6c 2069      # They all i
-00003b10: 6d70 6c65 6d65 6e74 2073 616d 6520 6d65  mplement same me
-00003b20: 7468 6f64 7320 6672 6f6d 2062 6173 6520  thods from base 
-00003b30: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
-00003b40: 204e 6f74 6520 7468 6174 2073 6f6d 6520   Note that some 
-00003b50: 6163 6375 7261 6379 206d 6179 2062 6520  accuracy may be 
-00003b60: 6c6f 7374 2064 7572 696e 6720 636f 6e76  lost during conv
-00003b70: 6572 7369 6f6e 2e0a 2020 2020 2020 2020  ersion..        
-00003b80: 2320 4966 2066 6f72 2065 7861 6d70 6c65  # If for example
-00003b90: 2079 6f75 2075 7365 2074 6f5f 6d69 6372   you use to_micr
-00003ba0: 6f73 6563 6f6e 6473 206e 616e 6f73 6563  oseconds nanosec
-00003bb0: 6f6e 6473 2077 696c 6c20 6265 2063 7574  onds will be cut
-00003bc0: 206f 6666 2069 6e73 7465 6164 206f 6620   off instead of 
-00003bd0: 726f 756e 6469 6e67 2e0a 2020 2020 2020  rounding..      
-00003be0: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
-00003bf0: 315d 2044 6174 6574 696d 6543 6f6e 7665  1] DatetimeConve
-00003c00: 7274 6572 2e0a 2020 2020 2020 2020 2320  rter..        # 
-00003c10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
-00003c20: 7220 7461 6b65 7320 6461 7465 7469 6d65  r takes datetime
-00003c30: 2e64 6174 6574 696d 6520 6f62 6a65 6374  .datetime object
-00003c40: 2061 7320 696e 7075 742e 0a20 2020 2020   as input..     
-00003c50: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
-00003c60: 7469 6d65 5f6f 626a 203d 2064 6174 6574  time_obj = datet
-00003c70: 696d 6528 7965 6172 3d32 3032 332c 206d  ime(year=2023, m
-00003c80: 6f6e 7468 3d31 2c20 6461 793d 352c 2068  onth=1, day=5, h
-00003c90: 6f75 723d 3134 2c20 6d69 6e75 7465 3d33  our=14, minute=3
-00003ca0: 382c 2073 6563 6f6e 643d 3235 2c20 6d69  8, second=25, mi
-00003cb0: 6372 6f73 6563 6f6e 643d 3134 3630 290a  crosecond=1460).
-00003cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003cd0: 2023 2049 7420 6861 7320 6d65 7468 6f64   # It has method
-00003ce0: 7320 7468 6174 2072 6574 7572 6e20 7468  s that return th
-00003cf0: 6520 6461 7465 7469 6d65 2069 6e20 6469  e datetime in di
-00003d00: 6666 6572 656e 7420 666f 726d 6173 3a0a  fferent formas:.
-00003d10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003d20: 2064 6174 655f 6d73 203d 2044 6174 6574   date_ms = Datet
-00003d30: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
-00003d40: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
-00003d50: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
-00003d60: 2020 2064 6174 655f 7573 203d 2044 6174     date_us = Dat
-00003d70: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
-00003d80: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
-00003d90: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
-00003da0: 2020 2020 2023 2043 6f6e 7665 7274 696e       # Convertin
-00003db0: 6720 746f 206e 616e 6f73 6563 6f6e 6473  g to nanoseconds
-00003dc0: 206a 7573 7473 2061 6464 7320 7468 7265   justs adds thre
-00003dd0: 6520 7472 6169 6c69 6e67 207a 6572 6f73  e trailing zeros
-00003de0: 2061 7320 6461 7465 7469 6d65 206f 626a   as datetime obj
-00003df0: 6563 7420 646f 6573 6e27 7420 6861 7665  ect doesn't have
-00003e00: 206e 616e 6f73 6563 6f6e 6473 2e0a 2020   nanoseconds..  
-00003e10: 2020 2020 2020 6461 7465 5f6e 7320 3d20        date_ns = 
-00003e20: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
-00003e30: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
-00003e40: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
-00003e50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003e60: 2320 5b32 2e32 5d20 4461 7465 7469 6d65  # [2.2] Datetime
-00003e70: 5374 7269 6e67 436f 6e76 6572 7465 720a  StringConverter.
-00003e80: 2020 2020 2020 2020 2320 4461 7465 7469          # Dateti
-00003e90: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003ea0: 7220 7461 6b65 7320 7374 7269 6e67 2069  r takes string i
-00003eb0: 6e20 2279 7979 792d 4d4d 2d64 6454 4848  n "yyyy-MM-ddTHH
-00003ec0: 3a6d 6d3a 7373 5b2e 5353 5353 5353 5353  :mm:ss[.SSSSSSSS
-00003ed0: 535d 5a22 2066 6f72 6d61 742e 0a20 2020  S]Z" format..   
-00003ee0: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
-00003ef0: 7465 5f73 7472 696e 6720 3d20 2232 3032  te_string = "202
-00003f00: 332d 3031 2d30 3554 3134 3a33 383a 3235  3-01-05T14:38:25
-00003f10: 2e30 3031 3436 5a22 0a20 2020 2020 2020  .00146Z".       
-00003f20: 200a 2020 2020 2020 2020 2320 5765 2068   .        # We h
-00003f30: 6176 6520 7361 6d65 206d 6574 686f 6473  ave same methods
-00003f40: 2061 7320 696e 2044 6174 6574 696d 6543   as in DatetimeC
-00003f50: 6f6e 7665 7274 6572 0a20 2020 2020 2020  onverter.       
-00003f60: 2064 6174 655f 6d73 5f66 726f 6d5f 7374   date_ms_from_st
-00003f70: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
-00003f80: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
-00003f90: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
-00003fa0: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
-00003fb0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
-00003fc0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
-00003fd0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003fe0: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
-00003ff0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
-00004000: 2020 2020 2020 2064 6174 655f 6e73 5f66         date_ns_f
-00004010: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
-00004020: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
-00004030: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
-00004040: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
-00004050: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004060: 2020 2320 5765 2063 616e 2061 6c73 6f20    # We can also 
-00004070: 6765 7420 6461 7465 7469 6d65 206f 626a  get datetime obj
-00004080: 6563 7420 6672 6f6d 2073 7472 696e 670a  ect from string.
-00004090: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
-000040a0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-000040b0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-000040c0: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
-000040d0: 6d65 2864 6174 655f 7374 7269 6e67 290a  me(date_string).
-000040e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000040f0: 2023 205b 322e 335d 2050 726f 746f 6275   # [2.3] Protobu
-00004100: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
-00004110: 7465 720a 2020 2020 2020 2020 2320 5072  ter.        # Pr
-00004120: 6f74 6f62 7566 2074 696d 6573 7461 6d70  otobuf timestamp
-00004130: 7320 6d75 7374 2062 6520 696e 2066 6f72  s must be in for
-00004140: 6d20 7b22 6570 6f63 6853 6563 6f6e 6422  m {"epochSecond"
-00004150: 3a20 7365 636f 6e64 732c 2022 6e61 6e6f  : seconds, "nano
-00004160: 223a 206e 616e 6f73 6563 6f6e 6473 7d0a  ": nanoseconds}.
-00004170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004180: 2070 726f 746f 6275 665f 7469 6d65 7374   protobuf_timest
-00004190: 616d 7020 3d20 7b22 6570 6f63 6853 6563  amp = {"epochSec
-000041a0: 6f6e 6422 3a20 3136 3732 3932 3935 3035  ond": 1672929505
-000041b0: 2c20 226e 616e 6f22 3a20 315f 3436 305f  , "nano": 1_460_
-000041c0: 3030 307d 0a20 2020 2020 2020 200a 2020  000}.        .  
-000041d0: 2020 2020 2020 6461 7465 5f6d 735f 6672        date_ms_fr
-000041e0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-000041f0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004200: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
-00004210: 6c69 7365 636f 6e64 7328 7072 6f74 6f62  liseconds(protob
-00004220: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
-00004230: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
-00004240: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00004250: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004260: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
-00004270: 726f 7365 636f 6e64 7328 7072 6f74 6f62  roseconds(protob
-00004280: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
-00004290: 2020 2020 2020 6461 7465 5f6e 735f 6672        date_ns_fr
-000042a0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-000042b0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-000042c0: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
-000042d0: 6f73 6563 6f6e 6473 2870 726f 746f 6275  oseconds(protobu
-000042e0: 665f 7469 6d65 7374 616d 7029 0a20 2020  f_timestamp).   
-000042f0: 2020 2020 2064 6174 6574 696d 655f 6672       datetime_fr
-00004300: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00004310: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004320: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
-00004330: 6574 696d 6528 7072 6f74 6f62 7566 5f74  etime(protobuf_t
-00004340: 696d 6573 7461 6d70 290a 2020 2020 2020  imestamp).      
-00004350: 2020 0a20 2020 2020 2020 2023 2323 2323    .        #####
-00004360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004380: 230a 2020 2020 2020 2020 2320 5b33 5d20  #.        # [3] 
-00004390: 576f 726b 696e 6720 7769 7468 2045 7665  Working with Eve
-000043a0: 6e74 5472 6565 2061 6e64 2045 7665 6e74  ntTree and Event
-000043b0: 5472 6565 436f 6c6c 6563 7469 6f6e 2e0a  TreeCollection..
-000043c0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
-000043d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000043e0: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-000043f0: 2020 2020 2020 2023 2043 616e 2062 6520         # Can be 
-00004400: 7573 6566 756c 2069 6620 796f 7520 6861  useful if you ha
-00004410: 7665 2064 6174 612d 7374 7265 616d 2077  ve data-stream w
-00004420: 6974 6820 3c20 3130 306b 2065 6c65 6d65  ith < 100k eleme
-00004430: 6e74 732c 206f 7468 6572 7769 7365 2069  nts, otherwise i
-00004440: 740a 2020 2020 2020 2020 2320 7461 6b65  t.        # take
-00004450: 7320 746f 6f20 6d75 6368 2052 414d 2e0a  s too much RAM..
-00004460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004470: 2023 205b 332e 315d 2042 7569 6c64 2061   # [3.1] Build a
-00004480: 2063 7573 746f 6d20 4576 656e 7454 7265   custom EventTre
-00004490: 650a 2020 2020 2020 2020 2320 546f 2063  e.        # To c
-000044a0: 7265 6174 6520 616e 2045 7665 6e74 5472  reate an EventTr
-000044b0: 6565 206f 626a 6563 7420 796f 7520 6e65  ee object you ne
-000044c0: 6564 2074 6f20 7072 6f76 6964 6520 6e61  ed to provide na
-000044d0: 6d65 2c20 6964 2061 6e64 2064 6174 6120  me, id and data 
-000044e0: 6f66 2074 6865 2072 6f6f 7420 6576 656e  of the root even
-000044f0: 742e 0a20 2020 2020 2020 2074 7265 6520  t..        tree 
-00004500: 3d20 4576 656e 7454 7265 6528 6576 656e  = EventTree(even
-00004510: 745f 6e61 6d65 3d22 726f 6f74 2065 7665  t_name="root eve
-00004520: 6e74 222c 2065 7665 6e74 5f69 643d 2272  nt", event_id="r
-00004530: 6f6f 745f 6964 222c 2064 6174 613d 7b22  oot_id", data={"
-00004540: 6461 7461 223a 205b 312c 2032 2c20 332c  data": [1, 2, 3,
-00004550: 2034 2c20 355d 7d29 0a20 2020 2020 2020   4, 5]}).       
-00004560: 200a 2020 2020 2020 2020 2320 546f 2061   .        # To a
-00004570: 6464 206e 6577 206e 6f64 6520 7573 6520  dd new node use 
-00004580: 6170 7065 6e64 5f65 7665 6e74 2e20 7061  append_event. pa
-00004590: 7265 6e74 5f69 6420 6973 206e 6563 6573  rent_id is neces
-000045a0: 7361 7279 2c20 6461 7461 2069 7320 6f70  sary, data is op
-000045b0: 7469 6f6e 616c 2e0a 2020 2020 2020 2020  tional..        
-000045c0: 7472 6565 2e61 7070 656e 645f 6576 656e  tree.append_even
-000045d0: 7428 6576 656e 745f 6e61 6d65 3d22 4122  t(event_name="A"
-000045e0: 2c20 6576 656e 745f 6964 3d22 415f 6964  , event_id="A_id
-000045f0: 222c 2064 6174 613d 4e6f 6e65 2c20 7061  ", data=None, pa
-00004600: 7265 6e74 5f69 643d 2272 6f6f 745f 6964  rent_id="root_id
-00004610: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
-00004620: 2020 2020 2320 5b33 2e33 5d20 4275 696c      # [3.3] Buil
-00004630: 6469 6e67 2074 6865 2045 7665 6e74 5472  ding the EventTr
-00004640: 6565 436f 6c6c 6563 7469 6f6e 2e0a 2020  eeCollection..  
-00004650: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
-00004660: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
-00004670: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00004680: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
-00004690: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
-000046a0: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
-000046b0: 2020 2020 6461 7461 5f73 6f75 7263 6520      data_source 
-000046c0: 3d20 4475 6d6d 7944 6174 6153 6f75 7263  = DummyDataSourc
-000046d0: 6528 2920 2023 204e 6f74 6521 2057 6520  e()  # Note! We 
-000046e0: 7573 6520 6661 6b65 2044 5320 6865 7265  use fake DS here
-000046f0: 2e0a 2020 2020 2020 2020 2320 4554 4344  ..        # ETCD
-00004700: 7269 7665 7220 6865 7265 2069 7320 6120  river here is a 
-00004710: 7374 7562 2c20 6163 7475 616c 6c79 2074  stub, actually t
-00004720: 6865 206c 6962 2064 6f65 736e 2774 2068  he lib doesn't h
-00004730: 6176 6520 7375 6368 2061 2063 6c61 7373  ave such a class
-00004740: 2e0a 2020 2020 2020 2020 2320 596f 7520  ..        # You 
-00004750: 6361 6e20 7461 6b65 2069 7420 696e 204c  can take it in L
-00004760: 7744 5020 6d6f 6475 6c65 206f 7220 6372  wDP module or cr
-00004770: 6561 7465 2079 6f75 7273 656c 6620 636c  eate yourself cl
-00004780: 6173 7320 6966 2079 6f75 2068 6176 6520  ass if you have 
-00004790: 736f 6d65 2073 7065 6369 616c 2065 7665  some special eve
-000047a0: 6e74 7320 7374 7275 6374 7572 652e 0a20  nts structure.. 
-000047b0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
-000047c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
-000047d0: 7461 5f73 6f75 7263 652e 6c77 6470 2e65  ta_source.lwdp.e
-000047e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
-000047f0: 2048 7474 7045 5443 4472 6976 6572 2061   HttpETCDriver a
-00004800: 7320 4554 4344 7269 7665 720a 2020 2020  s ETCDriver.    
-00004810: 2020 2020 0a20 2020 2020 2020 2023 2049      .        # I
-00004820: 6620 796f 7520 646f 6e27 7420 7370 6563  f you don't spec
-00004830: 6966 7920 6461 7461 5f73 6f75 7263 6520  ify data_source 
-00004840: 666f 7220 7468 6520 6472 6976 6572 2074  for the driver t
-00004850: 6865 6e20 6974 2077 6f6e 2774 2072 6563  hen it won't rec
-00004860: 6f76 6572 2064 6574 6163 6865 6420 6576  over detached ev
-00004870: 656e 7473 2e0a 2020 2020 2020 2020 6472  ents..        dr
-00004880: 6976 6572 3a20 4945 5443 4472 6976 6572  iver: IETCDriver
-00004890: 2020 2320 596f 7520 7368 6f75 6c64 2069    # You should i
-000048a0: 6e69 7420 4554 4344 7269 7665 7220 6f62  nit ETCDriver ob
-000048b0: 6a65 6374 2e20 452e 672e 2066 726f 6d20  ject. E.g. from 
-000048c0: 4c77 4450 206d 6f64 756c 6520 6f72 2079  LwDP module or y
-000048d0: 6f75 7220 6375 7374 6f6d 2063 6c61 7373  our custom class
-000048e0: 2e0a 2020 2020 2020 2020 6472 6976 6572  ..        driver
-000048f0: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
-00004900: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
-00004910: 7572 6365 2c20 7573 655f 7374 7562 3d54  urce, use_stub=T
-00004920: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
-00004930: 2020 2020 2020 6574 6320 3d20 4576 656e        etc = Even
-00004940: 7454 7265 6543 6f6c 6c65 6374 696f 6e28  tTreeCollection(
-00004950: 6472 6976 6572 290a 2020 2020 2020 2020  driver).        
-00004960: 6574 632e 6275 696c 6428 6576 656e 7473  etc.build(events
-00004970: 290a 2020 2020 2020 2020 6574 632e 7368  ).        etc.sh
-00004980: 6f77 2829 0a20 2020 2020 2020 2023 2049  ow().        # I
-00004990: 7427 6c6c 2070 7269 6e74 2074 6865 2066  t'll print the f
-000049a0: 6f6c 6c6f 7769 6e67 3a0a 2020 2020 2020  ollowing:.      
-000049b0: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
-000049c0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
-000049d0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
-000049e0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
-000049f0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
-00004a00: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
-00004a10: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
-00004a20: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
-00004a30: 0a20 2020 2020 2020 2070 7269 6e74 2865  .        print(e
-00004a40: 7463 290a 2020 2020 2020 2020 2320 4576  tc).        # Ev
-00004a50: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00004a60: 6e28 7472 6565 733d 312c 2065 7665 6e74  n(trees=1, event
-00004a70: 733d 335b 7472 6565 733d 332c 2064 6574  s=3[trees=3, det
-00004a80: 6163 6865 643d 305d 290a 2020 2020 2020  ached=0]).      
-00004a90: 2020 0a20 2020 2020 2020 2023 2044 6574    .        # Det
-00004aa0: 6163 6865 6420 6576 656e 7473 2069 736e  ached events isn
-00004ab0: 2774 2065 6d70 7479 2e0a 2020 2020 2020  't empty..      
-00004ac0: 2020 6173 7365 7274 2065 7463 2e67 6574    assert etc.get
-00004ad0: 5f64 6574 6163 6865 645f 6576 656e 7473  _detached_events
-00004ae0: 2829 2020 2320 7265 7475 726e 7320 6c69  ()  # returns li
-00004af0: 7374 206f 6620 6465 7461 6368 6564 5f65  st of detached_e
-00004b00: 7665 6e74 732e 0a20 2020 2020 2020 200a  vents..        .
-00004b10: 2020 2020 2020 2020 2320 7265 636f 7665          # recove
-00004b20: 725f 756e 6b6e 6f77 6e5f 6576 656e 7473  r_unknown_events
-00004b30: 202d 2d20 7573 6564 2074 6f20 7265 636f   -- used to reco
-00004b40: 7665 7220 736f 6d65 2065 7665 6e74 7320  ver some events 
-00004b50: 7061 7265 6e74 732e 0a20 2020 2020 2020  parents..       
-00004b60: 2023 2054 6861 7420 776f 6e27 7420 776f   # That won't wo
-00004b70: 726b 2077 6974 6820 4475 6d6d 7944 6174  rk with DummyDat
-00004b80: 6153 6f75 7263 652c 2073 6f20 7761 7320  aSource, so was 
-00004b90: 636f 6d6d 656e 7465 640a 2020 2020 2020  commented.      
-00004ba0: 2020 2320 6574 632e 7265 636f 7665 725f    # etc.recover_
-00004bb0: 756e 6b6e 6f77 6e5f 6576 656e 7473 2829  unknown_events()
-00004bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004bd0: 2020 2320 4166 7465 7220 7468 6174 2074    # After that t
-00004be0: 6865 2064 6574 6163 6865 6420 6576 656e  he detached even
-00004bf0: 7473 2073 686f 756c 6420 6265 2065 6d70  ts should be emp
-00004c00: 7479 2062 6563 6175 7365 2074 6865 7920  ty because they 
-00004c10: 7765 7265 2072 6563 6f76 6572 6564 2e0a  were recovered..
-00004c20: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
-00004c30: 206e 6f74 2065 7463 2e67 6574 5f64 6574   not etc.get_det
-00004c40: 6163 6865 645f 6576 656e 7473 2829 0a20  ached_events(). 
-00004c50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004c60: 2320 2d2d 2d2d 2d0a 2020 2020 2020 2020  # -----.        
-00004c70: 0a20 2020 2020 2020 2023 2054 6865 2063  .        # The c
-00004c80: 6f6c 6c65 6374 696f 6e20 6861 7320 4576  ollection has Ev
-00004c90: 656e 7454 7265 6573 2065 6163 6820 7769  entTrees each wi
-00004ca0: 7468 2061 2074 7265 6520 6f66 2065 7665  th a tree of eve
-00004cb0: 6e74 732e 0a20 2020 2020 2020 2023 2055  nts..        # U
-00004cc0: 7369 6e67 2043 6f6c 6c65 6374 696f 6e20  sing Collection 
-00004cd0: 616e 6420 4576 656e 7454 7265 6573 2c20  and EventTrees, 
-00004ce0: 796f 7520 6361 6e20 776f 726b 2066 6c65  you can work fle
-00004cf0: 7869 626c 7920 7769 7468 2065 7665 6e74  xibly with event
-00004d00: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00004d10: 2020 2020 2320 5b33 2e33 2e31 5d20 4765      # [3.3.1] Ge
-00004d20: 7420 6c65 6176 6573 206f 6620 616c 6c20  t leaves of all 
-00004d30: 7472 6565 732e 0a20 2020 2020 2020 206c  trees..        l
-00004d40: 6561 7665 733a 2054 7570 6c65 5b64 6963  eaves: Tuple[dic
-00004d50: 745d 203d 2065 7463 2e67 6574 5f6c 6561  t] = etc.get_lea
-00004d60: 7665 7328 2920 2023 2052 6574 7572 6e73  ves()  # Returns
-00004d70: 2061 2074 7570 6c65 206f 6620 6c65 6176   a tuple of leav
-00004d80: 6573 2065 7665 6e74 730a 2020 2020 2020  es events.      
-00004d90: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004da0: 332e 325d 2047 6574 2072 6f6f 7473 2069  3.2] Get roots i
-00004db0: 6473 206f 6620 616c 6c20 7472 6565 732e  ds of all trees.
-00004dc0: 0a20 2020 2020 2020 2072 6f6f 7473 3a20  .        roots: 
-00004dd0: 4c69 7374 5b73 7472 5d20 3d20 6574 632e  List[str] = etc.
-00004de0: 6765 745f 726f 6f74 735f 6964 7328 290a  get_roots_ids().
-00004df0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00004e00: 7320 7468 6520 6c69 7374 206f 6620 726f  s the list of ro
-00004e10: 6f74 2049 6473 3a0a 2020 2020 2020 2020  ot Ids:.        
-00004e20: 2320 5b27 6465 6d6f 5f62 6f6f 6b5f 313a  # ['demo_book_1:
-00004e30: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00004e40: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
-00004e50: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
-00004e60: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
-00004e70: 3535 3135 3264 5f31 275d 0a20 2020 2020  55152d_1'].     
-00004e80: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00004e90: 2e33 2e33 5d20 4669 6e64 2061 6e20 6576  .3.3] Find an ev
-00004ea0: 656e 7420 696e 2061 6c6c 2074 7265 6573  ent in all trees
-00004eb0: 2e0a 2020 2020 2020 2020 6669 6e64 5f65  ..        find_e
-00004ec0: 7665 6e74 3a20 4f70 7469 6f6e 616c 5b64  vent: Optional[d
-00004ed0: 6963 745d 203d 2065 7463 2e66 696e 6428  ict] = etc.find(
-00004ee0: 6c61 6d62 6461 2065 7665 6e74 3a20 2253  lambda event: "S
-00004ef0: 656e 6420 6d65 7373 6167 6522 2069 6e20  end message" in 
-00004f00: 6576 656e 745b 2265 7665 6e74 5479 7065  event["eventType
-00004f10: 225d 290a 2020 2020 2020 2020 0a20 2020  "]).        .   
-00004f20: 2020 2020 2023 205b 332e 332e 345d 2046       # [3.3.4] F
-00004f30: 696e 6420 616c 6c20 6576 656e 7473 2069  ind all events i
-00004f40: 6e20 616c 6c20 7472 6565 732e 2054 6865  n all trees. The
-00004f50: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
-00004f60: 626c 6520 7665 7273 696f 6e20 2766 696e  ble version 'fin
-00004f70: 6461 6c6c 5f69 7465 7227 2e0a 2020 2020  dall_iter'..    
-00004f80: 2020 2020 6669 6e64 5f65 7665 6e74 733a      find_events:
-00004f90: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
-00004fa0: 632e 6669 6e64 616c 6c28 6c61 6d62 6461  c.findall(lambda
-00004fb0: 2065 7665 6e74 3a20 6576 656e 745b 2273   event: event["s
-00004fc0: 7563 6365 7373 6675 6c22 5d20 6973 2054  uccessful"] is T
-00004fd0: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
-00004fe0: 2020 2020 2020 2320 5b33 2e33 2e35 5d20        # [3.3.5] 
-00004ff0: 4669 6e64 2061 6e20 616e 6365 7374 6f72  Find an ancestor
-00005000: 206f 6620 7468 6520 6576 656e 742e 0a20   of the event.. 
-00005010: 2020 2020 2020 2061 6e63 6573 746f 723a         ancestor:
-00005020: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
-00005030: 3d20 6574 632e 6669 6e64 5f61 6e63 6573  = etc.find_ances
-00005040: 746f 7228 0a20 2020 2020 2020 2020 2020  tor(.           
-00005050: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00005060: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00005070: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
-00005080: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00005090: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-000050a0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
-000050b0: 2020 2020 2066 696c 7465 723d 6c61 6d62       filter=lamb
-000050c0: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
-000050d0: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
-000050e0: 6576 656e 744e 616d 6522 5d2c 0a20 2020  eventName"],.   
-000050f0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-00005100: 2020 2020 2020 2020 2320 5b33 2e33 2e36          # [3.3.6
-00005110: 5d20 4765 7420 6368 696c 6472 656e 206f  ] Get children o
-00005120: 6620 7468 6520 6576 656e 742e 2054 6865  f the event. The
-00005130: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
-00005140: 626c 6520 7665 7273 696f 6e20 2767 6574  ble version 'get
-00005150: 5f63 6869 6c64 7265 6e5f 6974 6572 272e  _children_iter'.
-00005160: 0a20 2020 2020 2020 2063 6869 6c64 7265  .        childre
-00005170: 6e3a 2054 7570 6c65 5b64 6963 745d 203d  n: Tuple[dict] =
-00005180: 2065 7463 2e67 6574 5f63 6869 6c64 7265   etc.get_childre
-00005190: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
-000051a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-000051b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-000051c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
-000051d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
-000051e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
-000051f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
-00005200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00005210: 2023 205b 332e 332e 375d 2047 6574 2073   # [3.3.7] Get s
-00005220: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
-00005230: 6669 6564 2065 7665 6e74 2e0a 2020 2020  fied event..    
-00005240: 2020 2020 7375 6274 7265 653a 2045 7665      subtree: Eve
-00005250: 6e74 5472 6565 203d 2065 7463 2e67 6574  ntTree = etc.get
-00005260: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
-00005270: 2020 2020 2020 2264 656d 6f5f 626f 6f6b        "demo_book
-00005280: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
-00005290: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
-000052a0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
-000052b0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
-000052c0: 6136 3135 3531 3532 645f 3122 0a20 2020  a6155152d_1".   
-000052d0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-000052e0: 2020 2020 2020 2020 2320 5b33 2e33 2e38          # [3.3.8
-000052f0: 5d20 4765 7420 6675 6c6c 2070 6174 6820  ] Get full path 
-00005300: 746f 2074 6865 2065 7665 6e74 2e0a 2020  to the event..  
-00005310: 2020 2020 2020 2320 4c6f 6f6b 7320 6c69        # Looks li
-00005320: 6b65 205b 616e 6365 7374 6f72 5f72 6f6f  ke [ancestor_roo
-00005330: 742c 2061 6e63 6573 746f 725f 6c65 7665  t, ancestor_leve
-00005340: 6c31 2c20 616e 6365 7374 6f72 5f6c 6576  l1, ancestor_lev
-00005350: 656c 322c 2065 7665 6e74 5d0a 2020 2020  el2, event].    
-00005360: 2020 2020 6576 656e 745f 7061 7468 3a20      event_path: 
-00005370: 4c69 7374 5b64 6963 745d 203d 2065 7463  List[dict] = etc
-00005380: 2e67 6574 5f66 756c 6c5f 7061 7468 280a  .get_full_path(.
-00005390: 2020 2020 2020 2020 2020 2020 2264 656d              "dem
-000053a0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-000053b0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-000053c0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
-000053d0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-000053e0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-000053f0: 3122 0a20 2020 2020 2020 2029 0a20 2020  1".        ).   
-00005400: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00005410: 5b33 2e33 2e39 5d20 4765 7420 7061 7265  [3.3.9] Get pare
-00005420: 6e74 206f 6620 7468 6520 6576 656e 742e  nt of the event.
-00005430: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
-00005440: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
-00005450: 280a 2020 2020 2020 2020 2020 2020 2264  (.            "d
-00005460: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-00005470: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-00005480: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
-00005490: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
-000054a0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
-000054b0: 645f 3122 0a20 2020 2020 2020 2029 0a20  d_1".        ). 
-000054c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000054d0: 2320 5b33 2e33 2e31 305d 2041 7070 656e  # [3.3.10] Appen
-000054e0: 6420 6e65 7720 6576 656e 7420 746f 2074  d new event to t
-000054f0: 6865 2063 6f6c 6c65 6374 696f 6e2e 0a20  he collection.. 
-00005500: 2020 2020 2020 2065 7463 2e61 7070 656e         etc.appen
-00005510: 645f 6576 656e 7428 0a20 2020 2020 2020  d_event(.       
-00005520: 2020 2020 2065 7665 6e74 3d7b 0a20 2020       event={.   
-00005530: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00005540: 656e 7449 6422 3a20 2261 3230 6635 6566  entId": "a20f5ef
-00005550: 342d 6333 6665 2d62 6231 302d 6132 3963  4-c3fe-bb10-a29c
-00005560: 2d64 6433 6437 3834 3930 3965 6222 2c0a  -dd3d784909eb",.
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
-00005590: 2022 3865 3235 3234 6661 2d63 6635 392d   "8e2524fa-cf59-
-000055a0: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
-000055b0: 3463 3361 3632 222c 0a20 2020 2020 2020  4c3a62",.       
-000055c0: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-000055d0: 616d 6522 3a20 2253 7475 6245 7665 6e74  ame": "StubEvent
-000055e0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
-000055f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005600: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00005610: 2e33 2e31 315d 2053 686f 7720 7468 6520  .3.11] Show the 
-00005620: 656e 7469 7265 2063 6f6c 6c65 6374 696f  entire collectio
-00005630: 6e2e 0a20 2020 2020 2020 2065 7463 2e73  n..        etc.s
-00005640: 686f 7728 290a 2020 2020 2020 2020 2320  how().        # 
-00005650: 4974 276c 6c20 7072 696e 7420 7468 6520  It'll print the 
-00005660: 666f 6c6c 6f77 696e 673a 0a20 2020 2020  following:.     
-00005670: 2020 2023 2053 6574 206f 6620 6175 746f     # Set of auto
-00005680: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
-00005690: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
-000056a0: 7469 6e67 0a20 2020 2020 2020 2023 20e2  ting.        # .
-000056b0: 949c e294 80e2 9480 2050 6c61 696e 2065  ........ Plain e
-000056c0: 7665 6e74 2031 0a20 2020 2020 2020 2023  vent 1.        #
-000056d0: 20e2 9494 e294 80e2 9480 2050 6c61 696e   ......... Plain
-000056e0: 2065 7665 6e74 2032 0a20 2020 2020 2020   event 2.       
-000056f0: 200a 2020 2020 2020 2020 2320 4173 2079   .        # As y
-00005700: 6f75 2063 616e 2073 6565 2c20 6e6f 7468  ou can see, noth
-00005710: 696e 6720 7761 7320 6368 616e 6765 642c  ing was changed,
-00005720: 2062 7574 2077 6520 6164 6465 6420 7468   but we added th
-00005730: 6520 6e65 7720 6576 656e 7421 0a20 2020  e new event!.   
-00005740: 2020 2020 2023 206c 6574 2773 206c 6f6f       # let's loo
-00005750: 6b20 6174 2074 6865 2073 756d 6d61 7279  k at the summary
-00005760: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00005770: 2020 2070 7269 6e74 2865 7463 2e73 756d     print(etc.sum
-00005780: 6d61 7279 2829 2920 2023 2074 6865 2073  mary())  # the s
-00005790: 616d 6520 6173 206a 7573 7420 7072 696e  ame as just prin
-000057a0: 7428 6574 6329 0a20 2020 2020 2020 2023  t(etc).        #
-000057b0: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
-000057c0: 7469 6f6e 2874 7265 6573 3d31 2c20 6576  tion(trees=1, ev
-000057d0: 656e 7473 3d35 5b74 7265 6573 3d33 2c20  ents=5[trees=3, 
-000057e0: 6465 7461 6368 6564 3d32 5d29 0a20 2020  detached=2]).   
-000057f0: 2020 2020 2023 2059 6f75 2063 616e 2073       # You can s
-00005800: 6565 2074 6861 7420 6974 2077 6173 2061  ee that it was a
-00005810: 6464 6564 2074 6f20 6465 7461 6368 6564  dded to detached
-00005820: 2e20 5468 6174 2773 2077 6879 2079 6f75  . That's why you
-00005830: 2064 6f6e 2774 2073 6565 2074 6865 2065   don't see the e
-00005840: 7665 6e74 0a20 2020 2020 2020 2023 2076  vent.        # v
-00005850: 6961 2060 7368 6f77 2829 602e 2060 7368  ia `show()`. `sh
-00005860: 6f77 2829 6020 7072 696e 7473 206f 6e6c  ow()` prints onl
-00005870: 7920 5472 6565 7321 0a20 2020 2020 2020  y Trees!.       
-00005880: 2023 2055 7365 2060 6574 632e 6765 745f   # Use `etc.get_
-00005890: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-000058a0: 2829 6020 746f 2063 6f6e 7665 7274 2064  ()` to convert d
-000058b0: 6574 6163 6865 6420 6576 656e 7473 2074  etached events t
-000058c0: 6f20 7472 6565 732e 0a20 2020 2020 2020  o trees..       
-000058d0: 2023 204d 6f72 6520 696e 666f 726d 6174   # More informat
-000058e0: 696f 6e20 6265 6c6f 7720 696e 2074 6865  ion below in the
-000058f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
-00005900: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00005910: 0a20 2020 2020 2020 2023 202d 2d2d 2d2d  .        # -----
-00005920: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00005930: 2020 2320 5b33 2e34 5d20 576f 726b 696e    # [3.4] Workin
-00005940: 6720 7769 7468 2074 6865 2045 7665 6e74  g with the Event
-00005950: 5472 6565 2e0a 2020 2020 2020 2020 2320  Tree..        # 
-00005960: 4576 656e 7454 7265 6520 6861 7320 7468  EventTree has th
-00005970: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
-00005980: 7320 4576 656e 7454 7265 6543 6f6c 6c65  s EventTreeColle
-00005990: 6374 696f 6e2c 2062 7574 206f 6e6c 7920  ction, but only 
-000059a0: 666f 7220 6974 7320 6f77 6e20 7472 6565  for its own tree
-000059b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000059c0: 2020 2023 205b 332e 342e 315d 2047 6574     # [3.4.1] Get
-000059d0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-000059e0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
-000059f0: 7472 6565 733a 204c 6973 745b 4576 656e  trees: List[Even
-00005a00: 7454 7265 655d 203d 2065 7463 2e67 6574  tTree] = etc.get
-00005a10: 5f74 7265 6573 2829 0a20 2020 2020 2020  _trees().       
-00005a20: 2074 7265 653a 2045 7665 6e74 5472 6565   tree: EventTree
-00005a30: 203d 2074 7265 6573 5b30 5d0a 2020 2020   = trees[0].    
-00005a40: 2020 2020 0a20 2020 2020 2020 2023 2042      .        # B
-00005a50: 7574 2045 7665 6e74 5472 6565 2070 726f  ut EventTree pro
-00005a60: 7669 6465 7320 6120 776f 726b 2077 6974  vides a work wit
-00005a70: 6820 7468 6520 7472 6565 2c20 6275 7420  h the tree, but 
-00005a80: 646f 6573 206e 6f74 206d 6f64 6966 7920  does not modify 
-00005a90: 6974 2e0a 2020 2020 2020 2020 2320 4966  it..        # If
-00005aa0: 2079 6f75 2077 616e 7420 746f 206d 6f64   you want to mod
-00005ab0: 6966 7920 7468 6520 7472 6565 2c20 7573  ify the tree, us
-00005ac0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
-00005ad0: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
-00005ae0: 0a20 2020 2020 2020 2023 205b 332e 355d  .        # [3.5]
-00005af0: 2057 6f72 6b69 6e67 2077 6974 6820 5061   Working with Pa
-00005b00: 7265 6e74 6c65 7373 5472 6565 2e0a 2020  rentlessTree..  
-00005b10: 2020 2020 2020 2320 5061 7265 6e74 6c65        # Parentle
-00005b20: 7373 5472 6565 2069 7320 616e 2045 7665  ssTree is an Eve
-00005b30: 6e74 5472 6565 2074 6861 7420 6861 7320  ntTree that has 
-00005b40: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
-00005b50: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
-00005b60: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
-00005b70: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
-00005b80: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
-00005b90: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00005ba0: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
-00005bb0: 2822 7061 7265 6e74 6c65 7373 5f74 7265  ("parentless_tre
-00005bc0: 6573 2063 6f6e 7461 696e 733a 2229 0a20  es contains:"). 
-00005bd0: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
-00005be0: 656e 746c 6573 735f 7472 6565 7329 0a20  entless_trees). 
-00005bf0: 2020 2020 2020 2023 205b 4576 656e 7454         # [EventT
-00005c00: 7265 6528 6e61 6d65 3d27 3c42 726f 6b65  ree(name='<Broke
-00005c10: 6e45 7665 6e74 3e27 2c20 726f 6f74 5f69  nEvent>', root_i
-00005c20: 643d 276e 6f74 5f65 7869 7374 735f 696e  d='not_exists_in
-00005c30: 5f74 6865 5f65 7665 6e74 735f 7374 7265  _the_events_stre
-00005c40: 616d 272c 2065 7665 6e74 733d 3229 2c0a  am', events=2),.
-00005c50: 2020 2020 2020 2020 2320 2045 7665 6e74          #  Event
-00005c60: 5472 6565 286e 616d 653d 273c 4272 6f6b  Tree(name='<Brok
-00005c70: 656e 4576 656e 743e 272c 2072 6f6f 745f  enEvent>', root_
-00005c80: 6964 3d27 3865 3235 3234 6661 2d63 6635  id='8e2524fa-cf5
-00005c90: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
-00005ca0: 3930 3463 3361 3632 272c 2065 7665 6e74  904c3a62', event
-00005cb0: 733d 3229 5d0a 2020 2020 2020 2020 0a20  s=2)].        . 
-00005cc0: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
-00005cd0: 2220 2265 7463 2061 6674 6572 2060 6765  " "etc after `ge
-00005ce0: 745f 7061 7265 6e74 6c65 7373 5f74 7265  t_parentless_tre
-00005cf0: 6573 603a 2229 0a20 2020 2020 2020 2070  es`:").        p
-00005d00: 7269 6e74 2865 7463 2e73 756d 6d61 7279  rint(etc.summary
-00005d10: 2829 290a 2020 2020 2020 2020 2320 4576  ()).        # Ev
-00005d20: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00005d30: 6e28 7472 6565 733d 335b 7265 6775 6c61  n(trees=3[regula
-00005d40: 723d 312c 2070 6172 656e 746c 6573 733d  r=1, parentless=
-00005d50: 325d 2c20 6576 656e 7473 3d37 5b74 7265  2], events=7[tre
-00005d60: 6573 3d37 2c20 6465 7461 6368 6564 3d30  es=7, detached=0
-00005d70: 5d29 270a 2020 2020 2020 2020 6574 632e  ])'.        etc.
-00005d80: 7368 6f77 2829 0a20 2020 2020 2020 2023  show().        #
-00005d90: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
-00005da0: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
-00005db0: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
-00005dc0: 0a20 2020 2020 2020 2023 20e2 949c e294  .        # .....
-00005dd0: 80e2 9480 2050 6c61 696e 2065 7665 6e74  .... Plain event
-00005de0: 2031 0a20 2020 2020 2020 2023 20e2 9494   1.        # ...
-00005df0: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
-00005e00: 6e74 2032 0a20 2020 2020 2020 2023 203c  nt 2.        # <
-00005e10: 4272 6f6b 656e 4576 656e 743e 0a20 2020  BrokenEvent>.   
-00005e20: 2020 2020 2023 20e2 9494 e294 80e2 9480       # .........
-00005e30: 2046 616b 6520 6576 656e 740a 2020 2020   Fake event.    
-00005e40: 2020 2020 2320 3c42 726f 6b65 6e45 7665      # <BrokenEve
-00005e50: 6e74 3e0a 2020 2020 2020 2020 2320 e294  nt>.        # ..
-00005e60: 94e2 9480 e294 8020 5374 7562 4576 656e  ....... StubEven
-00005e70: 7420 2020 203c 2d2d 2d20 7468 6520 6576  t    <--- the ev
-00005e80: 656e 7420 7468 6174 2077 6173 2061 6464  ent that was add
-00005e90: 6564 2061 626f 7665 0a20 2020 2020 2020  ed above.       
-00005ea0: 200a 2020 2020 2020 2020 2320 5b33 2e36   .        # [3.6
-00005eb0: 5d20 576f 726b 696e 6720 7769 7468 2050  ] Working with P
-00005ec0: 6172 656e 7445 7665 6e74 5472 6565 436f  arentEventTreeCo
-00005ed0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00005ee0: 2020 2320 5061 7265 6e74 4576 656e 7454    # ParentEventT
-00005ef0: 7265 6543 6f6c 6c65 6374 696f 6e20 6973  reeCollection is
-00005f00: 2061 2074 7265 6520 636f 6c6c 6563 7469   a tree collecti
-00005f10: 6f6e 206c 696b 6520 4576 656e 7454 7265  on like EventTre
-00005f20: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
-00005f30: 2020 2020 2023 2062 7574 2069 7420 6861       # but it ha
-00005f40: 7320 6f6e 6c79 2065 7665 6e74 7320 7468  s only events th
-00005f50: 6174 2068 6176 6520 7265 6665 7265 6e63  at have referenc
-00005f60: 6573 2e0a 2020 2020 2020 2020 6461 7461  es..        data
-00005f70: 5f73 6f75 7263 653a 2049 4461 7461 536f  _source: IDataSo
-00005f80: 7572 6365 2020 2320 596f 7520 7368 6f75  urce  # You shou
-00005f90: 6c64 2069 6e69 7420 4461 7461 536f 7572  ld init DataSour
-00005fa0: 6365 206f 626a 6563 742e 2045 2e67 2e20  ce object. E.g. 
-00005fb0: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
-00005fc0: 2e0a 2020 2020 2020 2020 6461 7461 5f73  ..        data_s
-00005fd0: 6f75 7263 6520 3d20 4475 6d6d 7944 6174  ource = DummyDat
-00005fe0: 6153 6f75 7263 6528 2920 2023 204e 6f74  aSource()  # Not
-00005ff0: 6521 2057 6520 7573 6520 6661 6b65 2044  e! We use fake D
-00006000: 5320 6865 7265 2e0a 2020 2020 2020 2020  S here..        
-00006010: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
-00006020: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
-00006030: 616c 6c79 2074 6865 206c 6962 2064 6f65  ally the lib doe
-00006040: 736e 2774 2068 6176 6520 7375 6368 2061  sn't have such a
-00006050: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
-00006060: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
-00006070: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
-00006080: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
-00006090: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
-000060a0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
-000060b0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
-000060c0: 7572 652e 0a20 2020 2020 2020 2066 726f  ure..        fro
-000060d0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-000060e0: 6365 732e 6461 7461 5f73 6f75 7263 652e  ces.data_source.
-000060f0: 6c77 6470 2e65 7665 6e74 5f74 7265 6520  lwdp.event_tree 
-00006100: 696d 706f 7274 2048 7474 7045 5443 4472  import HttpETCDr
-00006110: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
-00006120: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00006130: 2020 2064 7269 7665 7220 3d20 4554 4344     driver = ETCD
-00006140: 7269 7665 7228 6461 7461 5f73 6f75 7263  river(data_sourc
-00006150: 653d 6461 7461 5f73 6f75 7263 6529 0a20  e=data_source). 
-00006160: 2020 2020 2020 2070 6574 6320 3d20 5061         petc = Pa
-00006170: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-00006180: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
-00006190: 2020 2020 2020 2020 7065 7463 2e62 7569          petc.bui
-000061a0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
-000061b0: 2020 200a 2020 2020 2020 2020 7065 7463     .        petc
-000061c0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-000061d0: 7065 7463 2e73 756d 6d61 7279 2829 0a20  petc.summary(). 
-000061e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000061f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006210: 2323 2323 2323 0a20 2020 2020 2020 2023  ######.        #
-00006220: 205b 345d 2046 6965 6c64 2052 6573 6f6c   [4] Field Resol
-00006230: 7665 7273 0a20 2020 2020 2020 2023 2323  vers.        ###
-00006240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006260: 2323 230a 2020 2020 2020 2020 2320 506c  ###.        # Pl
-00006270: 6561 7365 2072 6561 6420 6046 6965 6c64  ease read `Field
-00006280: 2052 6573 6f6c 7665 7273 6020 626c 6f63   Resolvers` bloc
-00006290: 6b20 696e 2072 6561 646d 6520 6669 7273  k in readme firs
-000062a0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-000062b0: 2020 2020 2320 5b34 2e31 5d20 5573 6167      # [4.1] Usag
-000062c0: 6520 6578 616d 706c 6520 6672 6f6d 2063  e example from c
-000062d0: 6c69 656e 7420 636f 6465 0a20 2020 2020  lient code.     
-000062e0: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
-000062f0: 5f73 6572 7669 6365 732e 6461 7461 5f73  _services.data_s
-00006300: 6f75 7263 6520 696d 706f 7274 2028 0a20  ource import (. 
-00006310: 2020 2020 2020 2020 2020 206c 7764 702c             lwdp,
-00006320: 0a20 2020 2020 2020 2029 2020 2320 6c77  .        )  # lw
-00006330: 6470 2064 6174 615f 736f 7572 6365 2069  dp data_source i
-00006340: 6e69 7469 616c 697a 6520 7468 325f 6461  nitialize th2_da
-00006350: 7461 5f73 6572 7669 6365 732e 636f 6e66  ta_services.conf
-00006360: 6967 2064 7572 696e 6720 696d 706f 7274  ig during import
-00006370: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
-00006380: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00006390: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
-000063a0: 7074 696f 6e73 2061 7320 6f5f 0a20 2020  ptions as o_.   
-000063b0: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-000063c0: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
-000063d0: 5f73 6f75 7263 652e 6c77 6470 2e73 7475  _source.lwdp.stu
-000063e0: 625f 6275 696c 6465 7220 696d 706f 7274  b_builder import
-000063f0: 2068 7474 705f 6d65 7373 6167 655f 7374   http_message_st
-00006400: 7562 5f62 7569 6c64 6572 0a20 2020 2020  ub_builder.     
-00006410: 2020 200a 2020 2020 2020 2020 6661 6b65     .        fake
-00006420: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
-00006430: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
-00006440: 6765 5f73 7475 625f 6275 696c 6465 722e  ge_stub_builder.
-00006450: 6275 696c 6428 7b22 6d65 7373 6167 6549  build({"messageI
-00006460: 6422 3a20 2261 222c 2022 6d65 7373 6167  d": "a", "messag
-00006470: 6554 7970 6522 3a20 2252 6f6f 7422 7d29  eType": "Root"})
-00006480: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
-00006490: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
-000064a0: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
-000064b0: 6d65 7373 6167 6549 6422 3a20 2262 222c  messageId": "b",
-000064c0: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
-000064d0: 224e 6577 227d 292c 0a20 2020 2020 2020  "New"}),.       
-000064e0: 2020 2020 2068 7474 705f 6d65 7373 6167       http_messag
-000064f0: 655f 7374 7562 5f62 7569 6c64 6572 2e62  e_stub_builder.b
-00006500: 7569 6c64 287b 226d 6573 7361 6765 4964  uild({"messageId
-00006510: 223a 2022 6322 2c20 226d 6573 7361 6765  ": "c", "message
-00006520: 5479 7065 223a 2022 416d 656e 6422 7d29  Type": "Amend"})
-00006530: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
-00006540: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
-00006550: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
-00006560: 6d65 7373 6167 6549 6422 3a20 2264 222c  messageId": "d",
-00006570: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
-00006580: 2243 616e 6365 6c22 7d29 2c0a 2020 2020  "Cancel"}),.    
-00006590: 2020 2020 5d0a 2020 2020 2020 2020 6661      ].        fa
-000065a0: 6b65 5f64 6174 615f 6f62 6a20 3d20 4461  ke_data_obj = Da
-000065b0: 7461 2866 616b 655f 6461 7461 290a 2020  ta(fake_data).  
-000065c0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
-000065d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
-000065e0: 615f 6f62 6a3a 0a20 2020 2020 2020 2020  a_obj:.         
-000065f0: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
-00006600: 5f6d 6573 7361 6765 286d 2920 2023 206d  _message(m)  # m
-00006610: 6672 202d 2073 7461 6e64 7320 666f 7220  fr - stands for 
-00006620: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
-00006630: 6c76 6572 0a20 2020 2020 2020 2023 206f  lver.        # o
-00006640: 720a 2020 2020 2020 2020 666f 7220 6d20  r.        for m 
-00006650: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
-00006660: 2e6d 6170 286f 5f2e 6d66 722e 6578 7061  .map(o_.mfr.expa
-00006670: 6e64 5f6d 6573 7361 6765 293a 0a20 2020  nd_message):.   
-00006680: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-00006690: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000066a0: 205b 342e 325d 204c 6962 7261 7269 6573   [4.2] Libraries
-000066b0: 2075 7361 6765 2e0a 2020 2020 2020 2020   usage..        
-000066c0: 2320 446f 6e27 7420 696d 706f 7274 2065  # Don't import e
-000066d0: 7861 6374 2072 6573 6f6c 7665 7273 2069  xact resolvers i
-000066e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 696e  mplementation in
-000066f0: 2079 6f75 7220 636f 6465 2c20 706c 6561   your code, plea
-00006700: 7365 2e0a 2020 2020 2020 2020 2320 416c  se..        # Al
-00006710: 6c6f 7720 796f 7572 2063 6c69 656e 7420  low your client 
-00006720: 746f 2064 6f20 6974 2069 6e73 7465 6164  to do it instead
-00006730: 2e0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
-00006740: 2069 6d70 6f72 7420 606f 7074 696f 6e73   import `options
-00006750: 6020 6672 6f6d 2060 7468 325f 6461 7461  ` from `th2_data
-00006760: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
-00006770: 6020 616e 6420 7573 6520 6974 2e0a 2020  ` and use it..  
-00006780: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
-00006790: 6174 615f 7365 7276 6963 6573 2e63 6f6e  ata_services.con
-000067a0: 6669 6720 696d 706f 7274 206f 7074 696f  fig import optio
-000067b0: 6e73 2061 7320 6f5f 0a20 2020 2020 2020  ns as o_.       
-000067c0: 200a 2020 2020 2020 2020 666f 7220 6d20   .        for m 
-000067d0: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
-000067e0: 3a0a 2020 2020 2020 2020 2020 2020 6f5f  :.            o_
-000067f0: 2e6d 6672 2e65 7870 616e 645f 6d65 7373  .mfr.expand_mess
-00006800: 6167 6528 6d29 0a20 2020 2020 2020 2023  age(m).        #
-00006810: 206f 720a 2020 2020 2020 2020 666f 7220   or.        for 
-00006820: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
-00006830: 626a 2e6d 6170 286f 5f2e 6d66 722e 6578  bj.map(o_.mfr.ex
-00006840: 7061 6e64 5f6d 6573 7361 6765 293a 0a20  pand_message):. 
-00006850: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00006860: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006870: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
-00006880: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
-00006890: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
-000068a0: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
-000068b0: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
-000068c0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-000068d0: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
-000068e0: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
-000068f0: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
-00006900: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
-00006910: 7468 6520 7573 6572 2077 6869 6368 2061  the user which a
-00006920: 2064 6174 6120 736f 7572 6365 2074 6f20   data source to 
-00006930: 7573 652e 0a20 2020 2020 2020 2023 2020  use..        #  
-00006940: 2057 6520 646f 206e 6f74 206b 6e6f 7720   We do not know 
-00006950: 7768 6174 2068 6520 7769 6c6c 2063 686f  what he will cho
-00006960: 6f73 652c 2074 6865 7265 666f 7265 2c20  ose, therefore, 
-00006970: 7765 206d 7573 7420 7369 6d70 6c79 2061  we must simply a
-00006980: 6363 6573 730a 2020 2020 2020 2020 2320  ccess.        # 
-00006990: 2020 7468 6520 696e 7465 7266 6163 652c    the interface,
-000069a0: 2077 6869 6368 2077 696c 6c20 6265 2069   which will be i
-000069b0: 6e69 7469 616c 697a 6564 2062 7920 7468  nitialized by th
-000069c0: 6520 7573 6572 2e0a 2020 2020 2020 2020  e user..        
-000069d0: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000069f0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00006a00: 2020 2020 2020 2020 2320 5b35 5d20 5573          # [5] Us
-00006a10: 696e 6720 7574 696c 6974 7920 6675 6e63  ing utility func
-00006a20: 7469 6f6e 732e 0a20 2020 2020 2020 2023  tions..        #
-00006a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a50: 2323 2323 230a 2020 2020 2020 2020 6672  #####.        fr
-00006a60: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00006a70: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
-00006a80: 5f75 7469 6c73 2e66 7265 7175 656e 6369  _utils.frequenci
-00006a90: 6573 2069 6d70 6f72 7420 6765 745f 6361  es import get_ca
-00006aa0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
-00006ab0: 6573 320a 2020 2020 2020 2020 6672 6f6d  es2.        from
-00006ac0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-00006ad0: 6573 2e75 7469 6c73 2e65 7665 6e74 5f75  es.utils.event_u
-00006ae0: 7469 6c73 2e74 6f74 616c 7320 696d 706f  tils.totals impo
-00006af0: 7274 2067 6574 5f63 6174 6567 6f72 795f  rt get_category_
-00006b00: 746f 7461 6c73 320a 2020 2020 2020 2020  totals2.        
-00006b10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00006b20: 7276 6963 6573 2e75 7469 6c73 2e63 6174  rvices.utils.cat
-00006b30: 6567 6f72 7920 696d 706f 7274 2043 6174  egory import Cat
-00006b40: 6567 6f72 790a 2020 2020 2020 2020 6672  egory.        fr
-00006b50: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00006b60: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
-00006b70: 5f75 7469 6c73 2e65 7665 6e74 5f75 7469  _utils.event_uti
-00006b80: 6c73 2069 6d70 6f72 7420 6973 5f73 6f72  ls import is_sor
-00006b90: 7465 640a 2020 2020 2020 2020 0a20 2020  ted.        .   
-00006ba0: 2020 2020 2023 205b 352e 315d 2047 6574       # [5.1] Get
-00006bb0: 2074 6865 2071 7561 6e74 6974 6965 7320   the quantities 
-00006bc0: 6f66 2065 7665 6e74 7320 666f 7220 6469  of events for di
-00006bd0: 6666 6572 656e 7420 6361 7465 676f 7269  fferent categori
-00006be0: 6573 2e0a 2020 2020 2020 2020 6d65 7472  es..        metr
-00006bf0: 6963 7320 3d20 5b0a 2020 2020 2020 2020  ics = [.        
-00006c00: 2020 2020 4361 7465 676f 7279 2822 6461      Category("da
-00006c10: 7465 222c 206c 616d 6264 6120 6d3a 2054  te", lambda m: T
-00006c20: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
-00006c30: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
-00006c40: 286d 5b22 7374 6172 7454 696d 6573 7461  (m["startTimesta
-00006c50: 6d70 225d 292e 6461 7465 2829 292c 0a20  mp"]).date()),. 
-00006c60: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
-00006c70: 6f72 7928 2273 7461 7475 7322 2c20 6c61  ory("status", la
-00006c80: 6d62 6461 206d 3a20 6d5b 2273 7563 6365  mbda m: m["succe
-00006c90: 7373 6675 6c22 5d29 2c0a 2020 2020 2020  ssful"]),.      
-00006ca0: 2020 5d0a 2020 2020 2020 2020 6361 7465    ].        cate
-00006cb0: 676f 7279 5f74 6f74 616c 7320 3d20 6765  gory_totals = ge
-00006cc0: 745f 6361 7465 676f 7279 5f74 6f74 616c  t_category_total
-00006cd0: 7332 2865 7665 6e74 732c 206d 6574 7269  s2(events, metri
-00006ce0: 6373 290a 2020 2020 2020 2020 7072 696e  cs).        prin
-00006cf0: 7428 6361 7465 676f 7279 5f74 6f74 616c  t(category_total
-00006d00: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
-00006d10: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-00006d20: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
-00006d30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006d40: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
-00006d50: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
-00006d60: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
-00006d70: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
-00006d80: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
-00006d90: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00006da0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
-00006db0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-00006dc0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
-00006dd0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
-00006de0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
-00006df0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00006e00: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
-00006e10: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-00006e20: 7c20 2020 2020 2020 207c 2032 3032 332d  |        | 2023-
-00006e30: 3031 2d30 3520 7c20 4661 6c73 6520 2020  01-05 | False   
-00006e40: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
-00006e50: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
-00006e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00006e70: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00006e80: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
-00006e90: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
-00006ea0: 7c20 2020 2020 2020 2020 207c 2020 2020  |          |    
-00006eb0: 2020 2032 207c 0a20 2020 2020 2020 202b     2 |.        +
-00006ec0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006ed0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00006ee0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-00006ef0: 2020 2020 7c20 746f 7461 6c73 207c 2020      | totals |  
-00006f00: 2020 2020 2020 2020 2020 7c20 312f 3120            | 1/1 
-00006f10: 2020 2020 207c 2020 2020 2020 2034 207c       |       4 |
-00006f20: 0a20 2020 2020 2020 202b 2d2d 2d2d 2d2d  .        +------
-00006f30: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  --+------------+
-00006f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00006f50: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
-00006f60: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
-00006f70: 2020 2023 205b 352e 325d 2047 6574 2074     # [5.2] Get t
-00006f80: 6865 206e 756d 6265 7220 6f66 2065 7665  he number of eve
-00006f90: 6e74 7320 7769 7468 2073 7461 7475 7320  nts with status 
-00006fa0: 7375 6363 6573 7366 756c 2e0a 2020 2020  successful..    
-00006fb0: 2020 2020 6361 7465 676f 7279 203d 2043      category = C
-00006fc0: 6174 6567 6f72 7928 2273 7461 7475 7322  ategory("status"
-00006fd0: 2c20 6c61 6d62 6461 206d 3a20 6d5b 2273  , lambda m: m["s
-00006fe0: 7563 6365 7373 6675 6c22 5d29 0a20 2020  uccessful"]).   
-00006ff0: 2020 2020 2063 6174 6567 6f72 795f 6672       category_fr
-00007000: 6571 7565 6e63 6965 7320 3d20 6765 745f  equencies = get_
-00007010: 6361 7465 676f 7279 5f66 7265 7175 656e  category_frequen
-00007020: 6369 6573 3228 6576 656e 7473 2c20 6361  cies2(events, ca
-00007030: 7465 676f 7279 290a 2020 2020 2020 2020  tegory).        
-00007040: 7072 696e 7428 6361 7465 676f 7279 5f66  print(category_f
-00007050: 7265 7175 656e 6369 6573 290a 2020 2020  requencies).    
-00007060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007070: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
-00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000070a0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-000070b0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
-000070c0: 2020 7c20 2020 2020 2020 207c 2074 696d    |        | tim
-000070d0: 6573 7461 6d70 5f73 7461 7274 2020 2020  estamp_start    
-000070e0: 207c 2074 696d 6573 7461 6d70 5f65 6e64   | timestamp_end
-000070f0: 2020 2020 2020 207c 2046 616c 7365 2020         | False  
-00007100: 207c 2020 2054 7275 6520 7c0a 2020 2020   |   True |.    
-00007110: 2020 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d      +========+==
-00007120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007130: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
-00007140: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
-00007150: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ===+========+.  
-00007160: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-00007170: 2032 3032 332d 3031 2d30 3554 3133 3a35   2023-01-05T13:5
-00007180: 373a 3035 207c 2032 3032 332d 3031 2d30  7:05 | 2023-01-0
-00007190: 3554 3133 3a35 373a 3036 207c 2030 2020  5T13:57:06 | 0  
-000071a0: 2020 2020 207c 2020 2020 2020 3320 7c0a       |      3 |.
-000071b0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
-000071c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-000071d0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000071e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000071f0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00007200: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-00007210: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
-00007220: 3134 3a30 323a 3035 207c 2032 3032 332d  14:02:05 | 2023-
-00007230: 3031 2d30 3554 3134 3a30 323a 3036 207c  01-05T14:02:06 |
-00007240: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
-00007250: 3020 7c0a 2020 2020 2020 2020 2b2d 2d2d  0 |.        +---
-00007260: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00007270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007290: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
-000072a0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
-000072b0: 636f 756e 7420 207c 2020 2020 2020 2020  count  |        
-000072c0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 207c 2020 2020 2020 2020 207c 2020     |         |  
-000072f0: 2020 2020 3220 7c0a 2020 2020 2020 2020      2 |.        
-00007300: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
-00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007330: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-00007340: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
-00007350: 2020 7c20 746f 7461 6c73 207c 2020 2020    | totals |    
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007370: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00007380: 2020 2020 2020 207c 2031 2020 2020 2020         | 1      
-00007390: 207c 2020 2020 2020 3320 7c0a 2020 2020   |      3 |.    
-000073a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
-000073b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000073c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-000073d0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-000073e0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
-000073f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007400: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
-00007410: 335d 2043 6865 636b 2069 6620 6576 656e  3] Check if even
-00007420: 7473 2061 7265 2073 6f72 7465 642e 0a20  ts are sorted.. 
-00007430: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00007440: 6973 5f73 6f72 7465 6428 6576 656e 7473  is_sorted(events
-00007450: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00007460: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
-00007470: 6060 600a 2020 2020 2020 2020 3c21 2d2d  ```.        <!--
-00007480: 2065 6e64 2067 6574 5f73 7461 7274 6564   end get_started
-00007490: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
-000074a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000074b0: 2023 2320 322e 332e 2053 686f 7274 2074   ## 2.3. Short t
-000074c0: 6865 6f72 790a 2020 2020 2020 2020 0a20  heory.        . 
-000074d0: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
-000074e0: 7279 2070 726f 7669 6465 7320 746f 6f6c  ry provides tool
-000074f0: 7320 666f 7220 6861 6e64 6c69 6e67 2073  s for handling s
-00007500: 7472 6561 6d20 6461 7461 2e20 5768 6174  tream data. What
-00007510: 2773 2061 2073 7472 6561 6d3f 2049 7427  's a stream? It'
-00007520: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
-00007530: 656c 656d 656e 7473 2066 726f 6d20 6120  elements from a 
-00007540: 736f 7572 6365 2074 6861 740a 2020 2020  source that.    
-00007550: 2020 2020 7375 7070 6f72 7473 2061 6767      supports agg
-00007560: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
-00007570: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00007580: 2020 2020 2323 2320 5465 726d 730a 2020      ### Terms.  
-00007590: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000075a0: 202a 2a44 6174 6120 6f62 6a65 6374 2a2a   **Data object**
-000075b0: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
-000075c0: 2060 4461 7461 6020 636c 6173 7320 7768   `Data` class wh
-000075d0: 6963 6820 6973 2077 7261 7070 6572 2075  ich is wrapper u
-000075e0: 6e64 6572 2073 7472 6561 6d2e 0a20 2020  nder stream..   
-000075f0: 2020 2020 202d 202a 2a53 6571 7565 6e63       - **Sequenc
-00007600: 6520 6f66 2065 6c65 6d65 6e74 732a 2a3a  e of elements**:
-00007610: 0a20 2020 2020 2020 2020 2041 205f 4461  .          A _Da
-00007620: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
-00007630: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
-00007640: 2074 6f20 6120 7365 7175 656e 6365 6420   to a sequenced 
-00007650: 7365 7420 6f66 2076 616c 7565 7320 6f66  set of values of
-00007660: 2061 2073 7065 6369 6669 6320 656c 656d   a specific elem
-00007670: 656e 7420 7479 7065 2e20 5374 7265 616d  ent type. Stream
-00007680: 2069 6e73 6964 6520 7468 6520 5f44 6174   inside the _Dat
-00007690: 610a 2020 2020 2020 2020 2020 6f62 6a65  a.          obje
-000076a0: 6374 5f20 2a2a 646f 6e19 7420 6163 7475  ct_ **don.t actu
-000076b0: 616c 6c79 2073 746f 7265 2a2a 2065 6c65  ally store** ele
-000076c0: 6d65 6e74 733b 2074 6865 7920 6172 6520  ments; they are 
-000076d0: 636f 6d70 7574 6564 206f 6e20 6465 6d61  computed on dema
-000076e0: 6e64 2e0a 2020 2020 2020 2020 2d20 2a2a  nd..        - **
-000076f0: 6461 7461 2073 6f75 7263 652a 2a20 2865  data source** (e
-00007700: 7861 6374 6c79 2069 6e20 736d 616c 6c20  xactly in small 
-00007710: 6c65 7474 6572 7329 3a0a 2020 2020 2020  letters):.      
-00007720: 2020 2020 416e 7920 736f 7572 6365 206f      Any source o
-00007730: 6620 6461 7461 2e20 452e 672e 205b 4c69  f data. E.g. [Li
-00007740: 6768 7477 6569 6768 7420 4461 7461 2050  ghtweight Data P
-00007750: 726f 7669 6465 725d 2868 7474 7073 3a2f  rovider](https:/
-00007760: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
-00007770: 6e65 742f 7468 322d 6c77 2d64 6174 612d  net/th2-lw-data-
-00007780: 7072 6f76 6964 6572 292c 2063 6f6c 6c65  provider), colle
-00007790: 6374 696f 6e73 2c0a 2020 2020 2020 2020  ctions,.        
-000077a0: 2020 6172 7261 7973 2c20 6f72 2049 2f4f    arrays, or I/O
-000077b0: 2072 6573 6f75 7263 6573 2e0a 2020 2020   resources..    
-000077c0: 2020 2020 2d20 2a2a 4461 7461 536f 7572      - **DataSour
-000077d0: 6365 2a2a 3a0a 2020 2020 2020 2020 2020  ce**:.          
-000077e0: 4120 636c 6173 7320 7468 6174 2069 7320  A class that is 
-000077f0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
-00007800: 6c69 6e6b 2062 6574 7765 656e 2074 6865  link between the
-00007810: 2053 6f75 7263 6541 5049 2061 6e64 2043   SourceAPI and C
-00007820: 6f6d 6d61 6e64 732e 0a20 2020 2020 2020  ommands..       
-00007830: 202d 202a 2a53 6f75 7263 6541 5049 2a2a   - **SourceAPI**
-00007840: 3a0a 2020 2020 2020 2020 2020 4561 6368  :.          Each
-00007850: 2073 6f75 7263 6520 6861 7320 6974 7320   source has its 
-00007860: 6f77 6e20 4150 4920 746f 2072 6574 7269  own API to retri
-00007870: 6576 6520 6461 7461 2e20 536f 7572 6365  eve data. Source
-00007880: 4150 4920 6973 2061 2063 6c61 7373 2074  API is a class t
-00007890: 6861 7420 7072 6f76 6964 6520 4150 4920  hat provide API 
-000078a0: 666f 7220 736f 6d65 2064 6174 6120 736f  for some data so
-000078b0: 7572 6365 2e0a 2020 2020 2020 2020 2d20  urce..        - 
-000078c0: 2a2a 436f 6d6d 616e 6473 2a2a 3a0a 2020  **Commands**:.  
-000078d0: 2020 2020 2020 2020 436c 6173 7365 7320          Classes 
-000078e0: 7468 6174 2070 726f 7669 6465 2075 7365  that provide use
-000078f0: 722d 6672 6965 6e64 6c79 2069 6e74 6572  r-friendly inter
-00007900: 6661 6365 7320 666f 7220 6765 7474 696e  faces for gettin
-00007910: 6720 736f 6d65 2064 6174 6120 6672 6f6d  g some data from
-00007920: 2044 6174 6153 6f75 7263 652e 2043 6f6d   DataSource. Com
-00007930: 6d61 6e64 7320 7573 6520 5f53 6f75 7263  mands use _Sourc
-00007940: 6541 5049 5f20 746f 0a20 2020 2020 2020  eAPI_ to.       
-00007950: 2020 2061 6368 6965 7665 2069 742e 0a20     achieve it.. 
-00007960: 2020 2020 2020 202d 202a 2a41 6461 7074         - **Adapt
-00007970: 6572 732a 2a3a 0a20 2020 2020 2020 2020  ers**:.         
-00007980: 2049 7427 7320 7369 6d69 6c61 7220 746f   It's similar to
-00007990: 2066 756e 6374 696f 6e20 666f 7220 6044   function for `D
-000079a0: 6174 612e 6d61 7060 206d 6574 686f 642e  ata.map` method.
-000079b0: 2041 646f 7074 6162 6c65 2063 6f6d 6d61   Adoptable comma
-000079c0: 6e64 7320 7573 6564 2069 7420 746f 2075  nds used it to u
-000079d0: 7064 6174 6520 7468 6520 6461 7461 2073  pdate the data s
-000079e0: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
-000079f0: 202a 2a41 6767 7265 6761 7465 206f 7065   **Aggregate ope
-00007a00: 7261 7469 6f6e 732a 2a3a 0a20 2020 2020  rations**:.     
-00007a10: 2020 2020 2043 6f6d 6d6f 6e20 6f70 6572       Common oper
-00007a20: 6174 696f 6e73 2073 7563 6820 6173 2066  ations such as f
-00007a30: 696c 7465 722c 206d 6170 2c20 6c69 6d69  ilter, map, limi
-00007a40: 7420 616e 6420 736f 206f 6e2e 0a20 2020  t and so on..   
-00007a50: 2020 2020 202d 202a 2a57 6f72 6b66 6c6f       - **Workflo
-00007a60: 772a 2a3a 2041 6e20 6f72 6465 7265 6420  w**: An ordered 
-00007a70: 7365 7420 6f66 205f 4167 6772 6567 6174  set of _Aggregat
-00007a80: 6520 6f70 6572 6174 696f 6e73 5f2e 0a20  e operations_.. 
-00007a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007aa0: 2323 2320 436f 6e63 6570 740a 2020 2020  ### Concept.    
-00007ab0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
-00007ac0: 206c 6962 7261 7279 2064 6573 6372 6962   library describ
-00007ad0: 6573 2074 6865 2068 6967 682d 6c65 7665  es the high-leve
-00007ae0: 6c20 696e 7465 7266 6163 6573 2060 4953  l interfaces `IS
-00007af0: 6f75 7263 6541 5049 602c 2060 4944 6174  ourceAPI`, `IDat
-00007b00: 6153 6f75 7263 6560 2c20 6049 436f 6d6d  aSource`, `IComm
-00007b10: 616e 6460 2c20 6049 4164 6170 7465 7260  and`, `IAdapter`
-00007b20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00007b30: 2020 2041 6e79 2064 6174 6120 736f 7572     Any data sour
-00007b40: 6365 206d 7573 7420 6265 2064 6573 6372  ce must be descr
-00007b50: 6962 6564 2062 7920 7468 6520 6049 4461  ibed by the `IDa
-00007b60: 7461 536f 7572 6365 6020 6162 7374 7261  taSource` abstra
-00007b70: 6374 2063 6c61 7373 2e20 5468 6573 6520  ct class. These 
-00007b80: 6361 6e20 6265 205f 4669 6c65 4461 7461  can be _FileData
-00007b90: 536f 7572 6365 5f2c 0a20 2020 2020 2020  Source_,.       
-00007ba0: 205f 4353 5644 6174 6153 6f75 7263 655f   _CSVDataSource_
-00007bb0: 2c20 5f44 4244 6174 6153 6f75 7263 655f  , _DBDataSource_
-00007bc0: 2061 6e64 206f 7468 6572 2e0a 2020 2020   and other..    
-00007bd0: 2020 2020 0a20 2020 2020 2020 2055 7375      .        Usu
-00007be0: 616c 6c79 2c20 6461 7461 2073 6f75 7263  ally, data sourc
-00007bf0: 6573 2068 6176 6520 736f 6d65 206b 696e  es have some kin
-00007c00: 6420 6f66 2041 5049 2e20 4461 7461 6261  d of API. Databa
-00007c10: 7365 7320 2d20 7072 6f76 6964 6520 5351  ses - provide SQ
-00007c20: 4c20 6c61 6e67 7561 6765 2c20 7768 656e  L language, when
-00007c30: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
-00007c40: 6669 6c65 2c20 796f 7520 6361 6e20 7265  file, you can re
-00007c50: 6164 0a20 2020 2020 2020 206c 696e 6520  ad.        line 
-00007c60: 6279 206c 696e 652c 2065 7463 2e20 5468  by line, etc. Th
-00007c70: 6973 2041 5049 2069 7320 6465 7363 7269  is API is descri
-00007c80: 6265 6420 6279 2074 6865 2060 4953 6f75  bed by the `ISou
-00007c90: 7263 6541 5049 6020 636c 6173 732e 2042  rceAPI` class. B
-00007ca0: 6563 6175 7365 2064 6966 6665 7265 6e74  ecause different
-00007cb0: 2076 6572 7369 6f6e 7320 6f66 2074 6865   versions of the
-00007cc0: 2073 616d 6520 6461 7461 2073 6f75 7263   same data sourc
-00007cd0: 650a 2020 2020 2020 2020 6d61 7920 6861  e.        may ha
-00007ce0: 7665 2064 6966 6665 7265 6e74 2041 5049  ve different API
-00007cf0: 2c20 6974 2069 7320 6265 7474 6572 2074  , it is better t
-00007d00: 6f20 6372 6561 7465 2061 2063 6c61 7373  o create a class
-00007d10: 2066 6f72 2065 6163 6820 7665 7273 696f   for each versio
-00007d20: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00007d30: 2020 2020 4765 6e65 7261 6c6c 792c 2064      Generally, d
-00007d40: 6174 6120 736f 7572 6365 2041 5049 7320  ata source APIs 
-00007d50: 6172 6520 6869 6464 656e 2062 6568 696e  are hidden behin
-00007d60: 6420 636f 6e76 656e 6965 6e74 2069 6e74  d convenient int
-00007d70: 6572 6661 6365 732e 2054 6865 2072 6f6c  erfaces. The rol
-00007d80: 6520 6f66 2074 6865 7365 2069 6e74 6572  e of these inter
-00007d90: 6661 6365 7320 6973 2070 6c61 7965 640a  faces is played.
-00007da0: 2020 2020 2020 2020 6279 2060 4943 6f6d          by `ICom
-00007db0: 6d61 6e64 6020 636c 6173 7365 732e 0a20  mand` classes.. 
-00007dc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007dd0: 6049 4164 6170 7465 7260 2063 6c61 7373  `IAdapter` class
-00007de0: 6573 2074 7261 6e73 666f 726d 2064 6174  es transform dat
-00007df0: 6120 7374 7265 616d 206c 696b 6520 6675  a stream like fu
-00007e00: 6e63 7469 6f6e 7320 666f 7220 6044 6174  nctions for `Dat
-00007e10: 612e 6d61 7060 206d 6574 686f 642e 2045  a.map` method. E
-00007e20: 7373 656e 7469 616c 6c79 2069 7427 7320  ssentially it's 
-00007e30: 7468 6520 7361 6d65 2074 6869 6e67 2062  the same thing b
-00007e40: 7574 206d 6f72 650a 2020 2020 2020 2020  ut more.        
-00007e50: 666c 6578 6962 6c65 2e0a 2020 2020 2020  flexible..      
-00007e60: 2020 0a20 2020 2020 2020 2046 6f72 2065    .        For e
-00007e70: 7861 6d70 6c65 2c20 4c77 4450 2044 6174  xample, LwDP Dat
-00007e80: 6153 6f75 7263 6528 6874 7470 733a 2f2f  aSource(https://
-00007e90: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00007ea0: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
-00007eb0: 2d6c 7764 7029 2075 7365 7320 7468 6573  -lwdp) uses thes
-00007ec0: 6520 6162 7374 7261 6374 2063 6c61 7373  e abstract class
-00007ed0: 6573 2074 6f20 6275 696c 6420 6974 7320  es to build its 
-00007ee0: 696d 706c 656d 656e 7461 7469 6f6e 2e59  implementation.Y
-00007ef0: 6f75 2063 616e 2065 6173 696c 7920 6372  ou can easily cr
-00007f00: 6561 7465 2079 6f75 7220 6f77 6e20 756e  eate your own un
-00007f10: 6971 7565 2063 6f6d 6d61 6e64 7320 666f  ique commands fo
-00007f20: 7220 5f4c 7744 5020 4461 7461 536f 7572  r _LwDP DataSour
-00007f30: 6365 5f2c 2061 7320 7765 6c6c 2061 7320  ce_, as well as 
-00007f40: 656e 7469 7265 0a20 2020 2020 2020 205f  entire.        _
-00007f50: 4461 7461 536f 7572 6365 5f20 636c 6173  DataSource_ clas
-00007f60: 7365 732e 205b 4865 7265 2069 7320 6120  ses. [Here is a 
-00007f70: 646f 6375 6d65 6e74 6174 696f 6e5d 2864  documentation](d
-00007f80: 6f63 756d 656e 7461 7469 6f6e 2f64 6174  ocumentation/dat
-00007f90: 6173 6f75 7263 652e 6d64 2920 6f6e 2068  asource.md) on h
-00007fa0: 6f77 2074 6f20 696d 706c 656d 656e 7420  ow to implement 
-00007fb0: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
-00007fc0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00007fd0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
-00007fe0: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
-00007ff0: 656e 7461 7469 6f6e 2f69 6d67 2f63 6f6e  entation/img/con
-00008000: 6365 7074 2e70 6e67 290a 2020 2020 2020  cept.png).      
-00008010: 2020 0a20 2020 2020 2020 2023 2323 2053    .        ### S
-00008020: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
-00008030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00008040: 2020 4675 7274 6865 726d 6f72 652c 2073    Furthermore, s
-00008050: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
-00008060: 2068 6176 6520 7477 6f20 6675 6e64 616d   have two fundam
-00008070: 656e 7461 6c20 6368 6172 6163 7465 7269  ental characteri
-00008080: 7374 6963 7320 7468 6174 206d 616b 6520  stics that make 
-00008090: 7468 656d 2076 6572 7920 6469 6666 6572  them very differ
-000080a0: 656e 7420 6672 6f6d 2063 6f6c 6c65 6374  ent from collect
-000080b0: 696f 6e0a 2020 2020 2020 2020 6f70 6572  ion.        oper
-000080c0: 6174 696f 6e73 3a20 5f50 6970 656c 696e  ations: _Pipelin
-000080d0: 696e 675f 2061 6e64 205f 496e 7465 726e  ing_ and _Intern
-000080e0: 616c 2069 7465 7261 7469 6f6e 5f2e 0a20  al iteration_.. 
-000080f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008100: 2323 2323 2050 6970 656c 696e 696e 670a  #### Pipelining.
-00008110: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008120: 204d 616e 7920 7374 7265 616d 206f 7065   Many stream ope
-00008130: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
-00008140: 2073 7472 6561 6d20 7468 656d 7365 6c76   stream themselv
-00008150: 6573 2e20 5468 6973 2061 6c6c 6f77 7320  es. This allows 
-00008160: 6f70 6572 6174 696f 6e73 2074 6f20 6265  operations to be
-00008170: 2063 6861 696e 6564 2074 6f20 666f 726d   chained to form
-00008180: 2061 206c 6172 6765 7220 7069 7065 6c69   a larger pipeli
-00008190: 6e65 2e0a 2020 2020 2020 2020 0a20 2020  ne..        .   
-000081a0: 2020 2020 2021 5b44 6174 6120 7374 7265       ![Data stre
-000081b0: 616d 2070 6970 656c 696e 655d 2864 6f63  am pipeline](doc
-000081c0: 756d 656e 7461 7469 6f6e 2f69 6d67 2f64  umentation/img/d
-000081d0: 6174 615f 7374 7265 616d 5f70 6970 656c  ata_stream_pipel
-000081e0: 696e 652e 706e 6729 0a20 2020 2020 2020  ine.png).       
-000081f0: 200a 2020 2020 2020 2020 2323 2323 2049   .        #### I
-00008200: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
-00008210: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00008220: 2020 2049 6e20 636f 6e74 7261 7374 2074     In contrast t
-00008230: 6f20 636f 6c6c 6563 7469 6f6e 732c 2077  o collections, w
-00008240: 6869 6368 2061 7265 2069 7465 7261 7465  hich are iterate
-00008250: 6420 6578 706c 6963 6974 6c79 2028 6578  d explicitly (ex
-00008260: 7465 726e 616c 2069 7465 7261 7469 6f6e  ternal iteration
-00008270: 292c 2073 7472 6561 6d20 6f70 6572 6174  ), stream operat
-00008280: 696f 6e73 2064 6f20 7468 6520 6974 6572  ions do the iter
-00008290: 6174 696f 6e0a 2020 2020 2020 2020 6265  ation.        be
-000082a0: 6869 6e64 2074 6865 2073 6365 6e65 7320  hind the scenes 
-000082b0: 666f 7220 796f 752e 204e 6f74 652c 2069  for you. Note, i
-000082c0: 7420 646f 6573 6e27 7420 6d65 616e 2079  t doesn't mean y
-000082d0: 6f75 2063 616e 6e6f 7420 6974 6572 6174  ou cannot iterat
-000082e0: 6520 7468 6520 5f44 6174 6120 6f62 6a65  e the _Data obje
-000082f0: 6374 5f2e 0a20 2020 2020 2020 200a 2020  ct_..        .  
-00008300: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00008310: 2323 2044 6174 6120 6974 6572 6174 696f  ## Data iteratio
-00008320: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00008330: 2020 2054 6865 2044 6174 6120 6f62 6a65     The Data obje
-00008340: 6374 2063 6f6e 7374 7275 6374 6f72 206d  ct constructor m
-00008350: 6574 686f 6420 7461 6b65 7320 696e 2061  ethod takes in a
-00008360: 7320 6172 6775 6d65 6e74 2065 6974 6865  s argument eithe
-00008370: 7220 616e 2069 7465 7261 746f 7220 6f76  r an iterator ov
-00008380: 6572 206f 626a 6563 7473 206f 7220 6120  er objects or a 
-00008390: 6765 6e65 7261 746f 7220 6675 6e63 7469  generator functi
-000083a0: 6f6e 2e0a 2020 2020 2020 2020 5468 6520  on..        The 
-000083b0: 4461 7461 206f 626a 6563 7420 6974 6572  Data object iter
-000083c0: 6174 6f72 2068 616e 646c 6573 2065 6163  ator handles eac
-000083d0: 6820 6974 656d 2069 6e20 7468 6973 2069  h item in this i
-000083e0: 7465 7261 746f 7220 6f72 2067 656e 6572  terator or gener
-000083f0: 6174 6f72 2061 7320 7468 6579 2061 7265  ator as they are
-00008400: 2c20 6d65 616e 696e 6720 6974 2064 6f65  , meaning it doe
-00008410: 736e 2774 2074 7279 2074 6f20 7265 6164  sn't try to read
-00008420: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
-00008430: 6974 656d 206f 7220 7265 7475 726e 2074  item or return t
-00008440: 6865 6d20 6d6f 6469 6669 6564 2069 6e20  hem modified in 
-00008450: 616e 7920 7761 792c 2069 6e73 7465 6164  any way, instead
-00008460: 2072 6574 7572 6e73 2074 6865 2069 7465   returns the ite
-00008470: 6d20 6974 7365 6c66 2e0a 2020 2020 2020  m itself..      
-00008480: 2020 5468 6520 6f6e 6c79 2065 7863 6570    The only excep
-00008490: 7469 6f6e 2074 6f20 7468 6973 2069 7320  tion to this is 
-000084a0: 7768 656e 2044 6174 6120 6f62 6a65 6374  when Data object
-000084b0: 2069 7320 6275 696c 7420 7573 696e 6720   is built using 
-000084c0: 6974 6572 6174 6f72 206f 7220 6765 6e65  iterator or gene
-000084d0: 7261 746f 7220 6f76 6572 206f 7468 6572  rator over other
-000084e0: 2044 6174 6120 6f62 6a65 6374 732e 204e   Data objects. N
-000084f0: 6f74 6520 7468 6174 2074 6869 7320 6974  ote that this it
-00008500: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
-00008510: 746f 7220 6d75 7374 206f 6e6c 7920 6265  tor must only be
-00008520: 2079 6965 6c64 696e 6720 4461 7461 206f   yielding Data o
-00008530: 626a 6563 7473 2061 6e64 206e 6f74 6869  bjects and nothi
-00008540: 6e67 2065 6c73 652e 2049 6620 7765 2062  ng else. If we b
-00008550: 7569 6c64 2066 726f 6d20 6120 6d69 7820  uild from a mix 
-00008560: 6f66 2044 6174 6120 6f62 6a65 6374 7320  of Data objects 
-00008570: 616e 6420 736f 6d65 206f 7468 6572 2074  and some other t
-00008580: 7970 6573 2c20 4461 7461 206f 626a 6563  ypes, Data objec
-00008590: 7473 2720 636f 6e74 656e 7420 776f 6e27  ts' content won'
-000085a0: 7420 6265 2072 6561 6420 616e 6420 696e  t be read and in
-000085b0: 7374 6561 6420 6974 2077 696c 6c20 6265  stead it will be
-000085c0: 2072 6574 7572 6e65 6420 6173 2044 6174   returned as Dat
-000085d0: 6120 6f62 6a65 6374 2069 7473 656c 662e  a object itself.
-000085e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000085f0: 2020 536d 616c 6c20 6578 616d 706c 6520    Small example 
-00008600: 746f 2064 656d 6f6e 7374 7261 7465 3a0a  to demonstrate:.
-00008610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008620: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00008630: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
-00008640: 5f73 6572 7669 6365 732e 6461 7461 2069  _services.data i
-00008650: 6d70 6f72 7420 4461 7461 0a20 2020 2020  mport Data.     
-00008660: 2020 200a 2020 2020 2020 2020 6431 203d     .        d1 =
-00008670: 2044 6174 6128 5b31 2c32 2c33 5d29 0a20   Data([1,2,3]). 
-00008680: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
-00008690: 285b 342c 352c 365d 290a 2020 2020 2020  ([4,5,6]).      
-000086a0: 2020 0a20 2020 2020 2020 206f 6e6c 795f    .        only_
-000086b0: 6461 7461 5f6f 626a 6563 7473 203d 2044  data_objects = D
-000086c0: 6174 6128 5b64 312c 6432 5d29 2023 2057  ata([d1,d2]) # W
-000086d0: 696c 6c20 6974 6572 6174 6520 6173 2031  ill iterate as 1
-000086e0: 2c32 2c33 2c34 2c35 2c36 0a20 2020 2020  ,2,3,4,5,6.     
-000086f0: 2020 2064 6174 615f 616e 645f 6c69 7374     data_and_list
-00008700: 203d 2044 6174 6128 5b64 312c 5b34 2c35   = Data([d1,[4,5
-00008710: 2c36 5d5d 2920 2320 5769 6c6c 2069 7465  ,6]]) # Will ite
-00008720: 7261 7465 2061 7320 6431 2c20 5b34 2c35  rate as d1, [4,5
-00008730: 2c36 5d0a 2020 2020 2020 2020 6461 7461  ,6].        data
-00008740: 5f61 6e64 5f6e 756d 6265 7273 203d 2044  _and_numbers = D
-00008750: 6174 6128 5b64 312c 342c 352c 365d 2920  ata([d1,4,5,6]) 
-00008760: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
-00008770: 7320 6431 2c34 2c35 2c36 0a20 2020 2020  s d1,4,5,6.     
-00008780: 2020 206c 6973 7473 5f6f 6e6c 7920 3d20     lists_only = 
-00008790: 4461 7461 285b 312c 322c 335d 2c5b 342c  Data([1,2,3],[4,
-000087a0: 352c 365d 2920 2320 5769 6c6c 2069 7465  5,6]) # Will ite
-000087b0: 7261 7465 2061 7320 5b31 2c32 2c33 5d2c  rate as [1,2,3],
-000087c0: 5b34 2c35 2c36 5d0a 2020 2020 2020 2020  [4,5,6].        
-000087d0: 0a20 2020 2020 2020 2023 2049 6620 7765  .        # If we
-000087e0: 2077 616e 7420 746f 2069 7465 7261 7465   want to iterate
-000087f0: 206f 7665 7220 636f 6e74 656e 7420 6f66   over content of
-00008800: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
-00008810: 7765 2073 686f 756c 6420 6669 7273 7420  we should first 
-00008820: 6372 6561 7465 2044 6174 6120 6f62 6a65  create Data obje
-00008830: 6374 7320 6672 6f6d 2074 6865 6d2c 0a20  cts from them,. 
-00008840: 2020 2020 2020 2023 2074 6865 6e20 7573         # then us
-00008850: 6520 7468 656d 2074 6f20 636f 6e73 7472  e them to constr
-00008860: 7563 7420 6e65 7720 4461 7461 206f 626a  uct new Data obj
-00008870: 6563 7420 6173 2069 6e20 6361 7365 206f  ect as in case o
-00008880: 6620 6431 2061 6e64 2064 322c 2063 7265  f d1 and d2, cre
-00008890: 6174 696e 6720 276f 6e6c 795f 6461 7461  ating 'only_data
-000088a0: 5f6f 626a 6563 7473 2720 696e 2074 6869  _objects' in thi
-000088b0: 7320 6578 616d 706c 652e 0a20 2020 2020  s example..     
-000088c0: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
-000088d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000088e0: 2020 2323 2320 4461 7461 2063 6163 6869    ### Data cachi
-000088f0: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
-00008900: 2020 2020 5468 6520 5f44 6174 6120 6f62      The _Data ob
-00008910: 6a65 6374 5f20 7072 6f76 6964 6573 2074  ject_ provides t
-00008920: 6865 2061 6269 6c69 7479 2074 6f20 7573  he ability to us
-00008930: 6520 7468 6520 6361 6368 652e 2054 6865  e the cache. The
-00008940: 2063 6163 6865 2077 6f72 6b73 2066 6f72   cache works for
-00008950: 2065 6163 6820 5f44 6174 6120 6f62 6a65   each _Data obje
-00008960: 6374 5f2c 2074 6861 7420 6973 2c20 796f  ct_, that is, yo
-00008970: 7520 6368 6f6f 7365 0a20 2020 2020 2020  u choose.       
-00008980: 2077 6869 6368 205f 4461 7461 206f 626a   which _Data obj
-00008990: 6563 745f 2079 6f75 2077 616e 7420 746f  ect_ you want to
-000089a0: 2073 6176 652e 2054 6865 205f 4461 7461   save. The _Data
-000089b0: 206f 626a 6563 745f 2063 6163 6865 2069   object_ cache i
-000089c0: 7320 7361 7665 6420 6166 7465 7220 7468  s saved after th
-000089d0: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
-000089e0: 6e2c 2062 7574 2074 6865 2069 7465 7261  n, but the itera
-000089f0: 7469 6f6e 0a20 2020 2020 2020 2073 6f75  tion.        sou
-00008a00: 7263 6520 6d61 7920 6265 2064 6966 6665  rce may be diffe
-00008a10: 7265 6e74 2e0a 2020 2020 2020 2020 0a20  rent..        . 
-00008a20: 2020 2020 2020 2049 6620 796f 7520 646f         If you do
-00008a30: 6e27 7420 7573 6520 7468 6520 6361 6368  n't use the cach
-00008a40: 652c 2079 6f75 7220 736f 7572 6365 2077  e, your source w
-00008a50: 696c 6c20 6265 2074 6865 2064 6174 6120  ill be the data 
-00008a60: 736f 7572 6365 2079 6f75 2068 6176 6520  source you have 
-00008a70: 696e 2074 6865 205f 4461 7461 204f 626a  in the _Data Obj
-00008a80: 6563 745f 2e20 4275 7420 6966 2079 6f75  ect_. But if you
-00008a90: 2075 7365 2074 6865 2063 6163 6865 2c0a   use the cache,.
-00008aa0: 2020 2020 2020 2020 796f 7572 2073 6f75          your sou
-00008ab0: 7263 6520 6361 6e20 6265 2074 6865 2064  rce can be the d
-00008ac0: 6174 6120 736f 7572 6365 2c20 7468 6520  ata source, the 
-00008ad0: 7061 7265 6e74 2063 6163 6865 2c20 6f72  parent cache, or
-00008ae0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
-00008af0: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
-00008b00: 6865 2064 6174 6120 736f 7572 6365 3a0a  he data source:.
-00008b10: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-00008b20: 205f 4461 7461 204f 626a 6563 745f 2064   _Data Object_ d
-00008b30: 6f65 736e 2774 2068 6176 6520 6120 7061  oesn't have a pa
-00008b40: 7265 6e74 2063 6163 6865 2061 6e64 2069  rent cache and i
-00008b50: 7473 2063 6163 6865 2e0a 2020 2020 2020  ts cache..      
-00008b60: 2020 2a20 5468 6520 7061 7265 6e74 2063    * The parent c
-00008b70: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
-00008b80: 4966 2074 6865 205f 4461 7461 204f 626a  If the _Data Obj
-00008b90: 6563 745f 2068 6173 2061 2070 6172 656e  ect_ has a paren
-00008ba0: 7420 6361 6368 652e 2049 7420 646f 6573  t cache. It does
-00008bb0: 6e27 7420 6d61 7474 6572 2077 6861 7420  n't matter what 
-00008bc0: 706f 7369 7469 6f6e 2074 6865 2070 6172  position the par
-00008bd0: 656e 7420 6361 6368 6520 6861 7320 696e  ent cache has in
-00008be0: 2069 6e68 6572 6974 616e 6365 2e0a 2020   inheritance..  
-00008bf0: 2020 2020 2020 2020 5f44 6174 6120 4f62          _Data Ob
-00008c00: 6a65 6374 5f20 756e 6465 7273 7461 6e64  ject_ understand
-00008c10: 7320 7768 6f73 6520 6361 6368 6520 6974  s whose cache it
-00008c20: 2069 7320 616e 6420 6578 6563 7574 6573   is and executes
-00008c30: 2074 6865 2070 6172 7420 6f66 2074 6865   the part of the
-00008c40: 2077 6f72 6b66 6c6f 7720 7468 6174 2077   workflow that w
-00008c50: 6173 206e 6f74 2065 7865 6375 7465 642e  as not executed.
-00008c60: 0a20 2020 2020 2020 202a 2054 6865 206f  .        * The o
-00008c70: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
-00008c80: 2020 2020 4966 2069 7420 6973 206e 6f74      If it is not
-00008c90: 2074 6865 2066 6972 7374 2069 7465 7261   the first itera
-00008ca0: 7469 6f6e 206f 6620 7468 6973 2044 6174  tion of this Dat
-00008cb0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-00008cc0: 2020 0a20 2020 2020 2020 204e 6f74 6520    .        Note 
-00008cd0: 7468 6174 2074 6865 2063 6163 6865 2073  that the cache s
-00008ce0: 7461 7465 206f 6620 7468 6520 4461 7461  tate of the Data
-00008cf0: 206f 626a 6563 7420 6973 206e 6f74 2069   object is not i
-00008d00: 6e68 6572 6974 6564 2e0a 2020 2020 2020  nherited..      
-00008d10: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
-00008d20: 466f 7263 6564 2063 6163 6869 6e67 0a20  Forced caching. 
-00008d30: 2020 2020 2020 2059 6f75 2063 616e 2074         You can t
-00008d40: 656c 6c20 4453 2074 6f20 6361 6368 6520  ell DS to cache 
-00008d50: 6461 7461 2074 6f20 7370 6563 6966 6963  data to specific
-00008d60: 2063 6163 6865 2066 696c 652c 2077 6869   cache file, whi
-00008d70: 6368 2077 6f6e 2774 2062 6520 6465 6c65  ch won't be dele
-00008d80: 7465 6420 6166 7465 7220 7363 7269 7074  ted after script
-00008d90: 2065 6e64 2e0a 2020 2020 2020 2020 596f   end..        Yo
-00008da0: 7520 6361 6e20 7365 6520 6578 616d 706c  u can see exampl
-00008db0: 6520 696e 2031 2e31 3220 7365 6374 696f  e in 1.12 sectio
-00008dc0: 6e20 6f66 205b 6765 745f 7374 6172 7465  n of [get_starte
-00008dd0: 645f 6578 616d 706c 655d 2865 7861 6d70  d_example](examp
-00008de0: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
-00008df0: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
-00008e00: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
-00008e10: 2020 2020 2020 2023 2323 2045 7665 6e74         ### Event
-00008e20: 5472 6565 2061 6e64 2063 6f6c 6c65 6374  Tree and collect
-00008e30: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
-00008e40: 2020 2020 2020 2323 2323 2045 7665 6e74        #### Event
-00008e50: 5472 6565 0a20 2020 2020 2020 200a 2020  Tree.        .  
-00008e60: 2020 2020 2020 6045 7665 6e74 5472 6565        `EventTree
-00008e70: 6020 6973 2061 2074 7265 652d 6261 7365  ` is a tree-base
-00008e80: 6420 6461 7461 2073 7472 7563 7475 7265  d data structure
-00008e90: 206f 6620 6576 656e 7473 2e20 4974 2061   of events. It a
-00008ea0: 6c6c 6f77 7320 796f 7520 6765 7420 6368  llows you get ch
-00008eb0: 696c 6472 656e 2061 6e64 2070 6172 656e  ildren and paren
-00008ec0: 7473 206f 6620 6576 656e 742c 0a20 2020  ts of event,.   
-00008ed0: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
-00008ee0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
-00008ef0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
-00008f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008f10: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
-00008f20: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
-00008f30: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
-00008f40: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
-00008f50: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
-00008f60: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
-00008f70: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
-00008f80: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
-00008f90: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
-00008fa0: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
-00008fb0: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
-00008fc0: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
-00008fd0: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
-00008fe0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
-00008ff0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
-00009000: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
-00009010: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
-00009020: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
-00009030: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
-00009040: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
-00009050: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
-00009060: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
-00009070: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
-00009080: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
-00009090: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
-000090a0: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
-000090b0: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
-000090c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000090d0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-000090e0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
-000090f0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
-00009100: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
-00009110: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
-00009120: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00009130: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
-00009140: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
-00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009160: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
-00009170: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
-00009180: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
-00009190: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
-000091a0: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
-000091b0: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
-000091c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000091d0: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
-000091e0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
-000091f0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00009200: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
-00009210: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
-00009220: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
-00009230: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
-00009240: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
-00009250: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
-00009260: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
-00009270: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
-00009280: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
-00009290: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
-000092a0: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
-000092b0: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
-000092c0: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
-000092d0: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
-000092e0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
-000092f0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
-00009300: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
-00009310: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
-00009320: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
-00009330: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
-00009340: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
-00009350: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
-00009360: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
-00009370: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
-00009380: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
-00009390: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
-000093a0: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
-000093b0: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
-000093c0: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
-000093d0: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
-000093e0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-000093f0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
-00009400: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
-00009410: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00009420: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
-00009430: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
-00009440: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
-00009450: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
-00009460: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
-00009470: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
-00009480: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
-00009490: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
-000094a0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-000094b0: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
-000094c0: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
-000094d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000094e0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
-000094f0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
-00009500: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
-00009510: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
-00009520: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
-00009530: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
-00009540: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
-00009550: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
-00009560: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
-00009570: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
-00009580: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
-00009590: 0a20 2020 2020 2020 202a 2054 6865 2063  .        * The c
-000095a0: 6f6c 6c65 6374 696f 6e20 6861 7320 6120  ollection has a 
-000095b0: 6665 6174 7572 6520 746f 2072 6563 6f76  feature to recov
-000095c0: 6572 2065 7665 6e74 732e 2041 6c6c 2065  er events. All e
-000095d0: 7665 6e74 7320 7468 6174 2061 7265 206e  vents that are n
-000095e0: 6f74 2069 6e20 7468 6520 7265 6365 6976  ot in the receiv
-000095f0: 6564 2064 6174 6120 7374 7265 616d 2c20  ed data stream, 
-00009600: 6275 7420 7768 6963 6820 6172 650a 2020  but which are.  
-00009610: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
-00009620: 6564 2077 696c 6c20 6265 206c 6f61 6465  ed will be loade
-00009630: 6420 6672 6f6d 2074 6865 2064 6174 6120  d from the data 
-00009640: 736f 7572 6365 2e0a 2020 2020 2020 2020  source..        
-00009650: 2a20 596f 7520 6361 6e20 7461 6b65 2060  * You can take `
-00009660: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
-00009670: 2074 6f20 7365 6520 7768 6963 6820 6576   to see which ev
-00009680: 656e 7473 2061 7265 206d 6973 7369 6e67  ents are missing
-00009690: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
-000096a0: 6f75 2077 616e 742c 2079 6f75 2063 616e  ou want, you can
-000096b0: 2062 7569 6c64 2070 6172 656e 746c 6573   build parentles
-000096c0: 7320 7472 6565 7320 7768 6572 6520 7468  s trees where th
-000096d0: 6520 6d69 7373 696e 6720 6576 656e 7473  e missing events
-000096e0: 2061 7265 2073 7475 6262 6564 2069 6e73   are stubbed ins
-000096f0: 7465 6164 2e20 4a75 7374 0a20 2020 2020  tead. Just.     
-00009700: 2020 2020 2075 7365 2060 6765 745f 7061       use `get_pa
-00009710: 7265 6e74 6c65 7373 5f74 7265 6573 2829  rentless_trees()
-00009720: 602e 0a20 2020 2020 2020 200a 2020 2020  `..        .    
-00009730: 2020 2020 5265 7175 6972 656d 656e 7473      Requirements
-00009740: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00009750: 2020 2031 2e20 4576 656e 7473 2070 726f     1. Events pro
-00009760: 7669 6465 6420 746f 2045 5443 2068 6176  vided to ETC hav
-00009770: 6520 746f 2068 6176 6520 6065 7665 6e74  e to have `event
-00009780: 5f6e 616d 6560 2c20 6065 7665 6e74 5f69  _name`, `event_i
-00009790: 6460 2c20 6070 6172 656e 745f 6576 656e  d`, `parent_even
-000097a0: 745f 6964 6020 6669 656c 6473 2e20 5468  t_id` fields. Th
-000097b0: 6579 0a20 2020 2020 2020 2063 616e 2068  ey.        can h
-000097c0: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
-000097d0: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
-000097e0: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
-000097f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009800: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
-00009810: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
-00009820: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
-00009830: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
-00009840: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
-00009850: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
-00009860: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
-00009870: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
-00009880: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
-00009890: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
-000098a0: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
-000098b0: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
-000098c0: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
-000098d0: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
-000098e0: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
-000098f0: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
-00009900: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
-00009910: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
-00009920: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
-00009930: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
-00009940: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
-00009950: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
-00009960: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-00009970: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
-00009980: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
-00009990: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
-000099a0: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
-000099b0: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
-000099c0: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
-000099d0: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
-000099e0: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
-000099f0: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
-00009a00: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
-00009a10: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
-00009a20: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
-00009a30: 2020 2020 2023 2323 2046 6965 6c64 2052       ### Field R
-00009a40: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
-00009a50: 2049 6e74 6572 6661 6365 2063 616e 2062   Interface can b
-00009a60: 6520 666f 756e 6420 696e 2060 7468 325f  e found in `th2_
-00009a70: 6461 7461 5f73 6572 7669 6365 732f 696e  data_services/in
-00009a80: 7465 7266 6163 6573 2f75 7469 6c73 2f72  terfaces/utils/r
-00009a90: 6573 6f6c 7665 722e 7079 602e 2020 0a20  esolver.py`.  . 
-00009aa0: 2020 2020 2020 2041 6c6c 2064 6174 612d         All data-
-00009ab0: 736f 7572 6365 7320 7368 6f75 6c64 2069  sources should i
-00009ac0: 6d70 6c65 6d65 6e74 2074 6865 6d2e 0a20  mplement them.. 
-00009ad0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009ae0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
-00009af0: 6720 7265 736f 6c76 6572 733a 0a20 2020  g resolvers:.   
-00009b00: 2020 2020 2049 7420 736f 6c76 6573 2074       It solves t
-00009b10: 6865 2070 726f 626c 656d 206f 6620 6861  he problem of ha
-00009b20: 7669 6e67 2061 2066 6577 2044 6174 6153  ving a few DataS
-00009b30: 6f75 7263 6573 2077 6974 6820 7369 6d69  ources with simi
-00009b40: 6c61 7220 6461 7461 2c0a 2020 2020 2020  lar data,.      
-00009b50: 2020 6275 7420 7769 7468 2064 6966 6665    but with diffe
-00009b60: 7265 6e74 2077 6179 7320 746f 2067 6574  rent ways to get
-00009b70: 2069 742e 0a20 2020 2020 2020 200a 2020   it..        .  
-00009b80: 2020 2020 2020 5468 6573 6520 636c 6173        These clas
-00009b90: 7365 7320 7072 6f76 6964 6520 796f 7520  ses provide you 
-00009ba0: 6765 7474 6572 206d 6574 686f 6473 2e0a  getter methods..
-00009bb0: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
-00009bc0: 6573 6520 636c 6173 7365 7320 616c 6c6f  ese classes allo
-00009bd0: 7773 2079 6f75 2074 6f20 6672 6565 6c79  ws you to freely
-00009be0: 2073 7769 7463 6820 6265 7477 6565 6e20   switch between 
-00009bf0: 6469 6666 6572 656e 7420 6461 7461 0a20  different data. 
-00009c00: 2020 2020 2020 2066 6f72 6d61 7473 2061         formats a
-00009c10: 6e64 2064 6f6e 2774 2063 6861 6e67 6520  nd don't change 
-00009c20: 796f 7572 2063 6f64 652e 0a20 2020 2020  your code..     
-00009c30: 2020 200a 2020 2020 2020 2020 5265 736f     .        Reso
-00009c40: 6c76 6572 7320 736f 6c76 6520 7468 6520  lvers solve the 
-00009c50: 7072 6f62 6c65 6d20 6f66 2064 6174 612d  problem of data-
-00009c60: 666f 726d 6174 206d 6967 7261 7469 6f6e  format migration
-00009c70: 2e0a 2020 2020 2020 2020 2d20 6669 656c  ..        - fiel
-00009c80: 6473 2070 6c61 6365 2063 616e 2062 6520  ds place can be 
-00009c90: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
-00009ca0: 2d20 6669 656c 6473 206e 616d 6573 2063  - fields names c
-00009cb0: 616e 2062 6520 6368 616e 6765 640a 2020  an be changed.  
-00009cc0: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00009cd0: 6573 6f6c 7665 7273 2063 616e 2077 6f72  esolvers can wor
-00009ce0: 6b20 6f6e 6c79 2077 6974 6820 6f6e 6520  k only with one 
-00009cf0: 6576 656e 742f 6d65 7373 6167 652e 0a20  event/message.. 
-00009d00: 2020 2020 2020 2049 7420 6d65 616e 732c         It means,
-00009d10: 2069 6620 796f 7572 206d 6573 7361 6765   if your message
-00009d20: 2068 6173 2073 7562 2d6d 6573 7361 6765   has sub-message
-00009d30: 7320 286c 696b 6520 7468 322d 6d65 7373  s (like th2-mess
-00009d40: 6167 6573 2069 6e20 6c77 6470 2920 6974  ages in lwdp) it
-00009d50: 200a 2020 2020 2020 2020 776f 6e27 7420   .        won't 
-00009d60: 776f 726b 2c20 6265 6361 7573 6520 7265  work, because re
-00009d70: 736f 6c76 6572 2077 696c 6c20 6e6f 7420  solver will not 
-00009d80: 6b6e 6f77 2077 6974 6820 7768 6963 6820  know with which 
-00009d90: 7375 622d 6d65 7373 6167 6520 7368 6f75  sub-message shou
-00009da0: 6c64 2069 7420 776f 726b 2e20 0a20 2020  ld it work. .   
-00009db0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00009dc0: 576f 726b 6172 6f75 6e64 2a2a 2020 0a20  Workaround**  . 
-00009dd0: 2020 2020 2020 2031 2e20 4578 7061 6e64         1. Expand
-00009de0: 2061 6c6c 2079 6f75 7220 6d65 7373 6167   all your messag
-00009df0: 6573 202d 3e20 606e 6577 5f64 203d 2079  es -> `new_d = y
-00009e00: 6f75 725f 6461 7461 2e6d 6170 284d 6573  our_data.map(Mes
-00009e10: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
-00009e20: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
-00009e30: 2960 0a20 2020 2020 2020 2032 2e20 5573  )`.        2. Us
-00009e40: 6520 6045 7870 616e 6465 644d 6573 7361  e `ExpandedMessa
-00009e50: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
-00009e60: 2069 6e73 7465 6164 206f 6620 7573 7561   instead of usua
-00009e70: 6c20 604d 6573 7361 6765 4669 656c 6452  l `MessageFieldR
-00009e80: 6573 6f6c 7665 7260 2077 6865 6e20 0a20  esolver` when . 
-00009e90: 2020 2020 2020 2020 2020 2079 6f75 2074             you t
-00009ea0: 616b 6520 6669 656c 6473 2066 6f72 2065  ake fields for e
-00009eb0: 7870 616e 6465 6420 6d65 7373 6167 6573  xpanded messages
-00009ec0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00009ed0: 2020 202a 2a49 6d70 6c65 6d65 6e74 6174     **Implementat
-00009ee0: 696f 6e20 6164 7669 6365 3a2a 2a0a 2020  ion advice:**.  
-00009ef0: 2020 2020 2020 312e 2072 6169 7365 204e        1. raise N
-00009f00: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00009f10: 6f72 202d 2d20 6966 2079 6f75 7220 496d  or -- if your Im
-00009f20: 706c 656d 656e 7461 7469 6f6e 2064 6f65  plementation doe
-00009f30: 736e 2774 2073 7570 706f 7274 2074 6869  sn't support thi
-00009f40: 7320 6765 7474 6572 2e0a 2020 2020 2020  s getter..      
-00009f50: 2020 0a20 2020 2020 2020 202a 2a50 6572    .        **Per
-00009f60: 666f 726d 616e 6365 2069 6d70 6163 743a  formance impact:
-00009f70: 2a2a 0a20 2020 2020 2020 202d 2049 7420  **.        - It 
-00009f80: 6120 6269 7420 736c 6f77 6572 2074 6861  a bit slower tha
-00009f90: 6e20 7573 696e 6720 6e61 6b65 6420 6669  n using naked fi
-00009fa0: 656c 6420 6163 6365 7373 2060 6469 6374  eld access `dict
-00009fb0: 5b27 6b65 7927 5d60 2e0a 2020 2020 2020  ['key']`..      
-00009fc0: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
-00009fd0: 342e 204c 696e 6b73 0a20 2020 2020 2020  4. Links.       
-00009fe0: 200a 2020 2020 2020 2020 2d20 5b52 6570   .        - [Rep
-00009ff0: 6f72 7420 4461 7461 2050 726f 7669 6465  ort Data Provide
-0000a000: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-0000a010: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
-0000a020: 322d 7270 742d 6461 7461 2d70 726f 7669  2-rpt-data-provi
-0000a030: 6465 7229 0a20 2020 2020 2020 202d 205b  der).        - [
-0000a040: 5468 3220 4461 7461 2053 6572 7669 6365  Th2 Data Service
-0000a050: 7320 5574 696c 735d 2868 7474 7073 3a2f  s Utils](https:/
-0000a060: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
-0000a070: 6e65 742f 7468 322d 6461 7461 2d73 6572  net/th2-data-ser
-0000a080: 7669 6365 732d 7574 696c 7329 0a20 2020  vices-utils).   
-0000a090: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000a0a0: 332e 2042 6573 7420 7072 6163 7469 6365  3. Best practice
-0000a0b0: 730a 2020 2020 2020 2020 4465 7065 6e64  s.        Depend
-0000a0c0: 696e 6720 6f6e 2068 6f77 2079 6f75 2077  ing on how you w
-0000a0d0: 6f72 6b20 7769 7468 2060 4461 7461 206f  ork with `Data o
-0000a0e0: 626a 6563 7460 2c20 6974 2063 616e 2062  bject`, it can b
-0000a0f0: 6520 736c 6f77 206f 6620 6661 7374 2e0a  e slow of fast..
-0000a100: 2020 2020 2020 2020 4173 2077 6974 6820          As with 
-0000a110: 6120 7265 6c61 7469 6f6e 616c 2064 6174  a relational dat
-0000a120: 6162 6173 652c 2079 6f75 2063 616e 2077  abase, you can w
-0000a130: 7269 7465 2061 2071 7565 7279 2074 6861  rite a query tha
-0000a140: 7420 7769 6c6c 2072 6574 7572 6e20 6461  t will return da
-0000a150: 7461 2073 6c6f 776c 7920 6f72 2071 7569  ta slowly or qui
-0000a160: 636b 6c79 2c0a 2020 2020 2020 2020 7468  ckly,.        th
-0000a170: 6520 7361 6d65 2077 6865 6e20 776f 726b  e same when work
-0000a180: 696e 6720 7769 7468 2061 2060 4461 7461  ing with a `Data
-0000a190: 206f 626a 6563 7460 2e0a 2020 2020 2020   object`..      
-0000a1a0: 2020 0a20 2020 2020 2020 2046 6f6c 6c6f    .        Follo
-0000a1b0: 7720 7468 6520 7275 6c65 7320 746f 206d  w the rules to m
-0000a1c0: 616b 6520 796f 7572 2077 6f72 6b20 7769  ake your work wi
-0000a1d0: 7468 2044 6174 6120 6f62 6a65 6374 2066  th Data object f
-0000a1e0: 6173 743a 0a20 2020 2020 2020 2031 2e20  ast:.        1. 
-0000a1f0: 5573 6520 6044 6174 612e 7573 655f 6361  Use `Data.use_ca
-0000a200: 6368 6528 2960 2069 6620 796f 7520 6974  che()` if you it
-0000a210: 6572 6174 6520 6461 7461 206d 6f72 6520  erate data more 
-0000a220: 7468 616e 206f 6e65 2074 696d 652e 0a20  than one time.. 
-0000a230: 2020 2020 2020 2032 2e20 5472 7920 746f         2. Try to
-0000a240: 2064 6f6e 2774 2069 7465 7261 7465 206f   don't iterate o
-0000a250: 6e65 2060 4461 7461 206f 626a 6563 7460  ne `Data object`
-0000a260: 2069 6e73 6964 6520 7468 6520 6f74 6865   inside the othe
-0000a270: 7220 6f6e 652e 0a20 2020 2020 2020 2020  r one..         
-0000a280: 2020 4966 2079 6f75 2073 686f 756c 6420    If you should 
-0000a290: 746f 2064 6f20 6974 2c20 7573 6520 7368  to do it, use sh
-0000a2a0: 6f72 7420 6044 6174 6120 6f62 6a65 6374  ort `Data object
-0000a2b0: 6020 6669 7273 7420 616e 6420 6c6f 6e67  ` first and long
-0000a2c0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
-0000a2d0: 6e73 6964 6520 7468 6520 6c6f 6f70 2e0a  nside the loop..
-0000a2e0: 2020 2020 2020 2020 2020 2049 7427 6c6c             It'll
-0000a2f0: 2061 6c6c 6f77 2079 6f75 206f 7065 6e20   allow you open 
-0000a300: 7468 6520 6361 6368 6520 6669 6c65 206f  the cache file o
-0000a310: 7220 6372 6561 7465 2061 2072 6571 7565  r create a reque
-0000a320: 7374 2074 6f20 6044 6174 6120 736f 7572  st to `Data sour
-0000a330: 6365 6020 6c65 7373 206e 756d 6265 7220  ce` less number 
-0000a340: 6f66 2074 696d 6573 2e0a 2020 2020 2020  of times..      
-0000a350: 2020 0a20 2020 2020 2020 2023 2034 2e20    .        # 4. 
-0000a360: 4f66 6669 6369 616c 2044 6174 6153 6f75  Official DataSou
-0000a370: 7263 6520 696d 706c 656d 656e 7461 7469  rce implementati
-0000a380: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-0000a390: 2020 2020 202d 205b 4c69 6768 7477 6569       - [Lightwei
-0000a3a0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
-0000a3b0: 7220 4461 7461 2053 6f75 7263 655d 2868  r Data Source](h
-0000a3c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000a3d0: 6d2f 7468 322d 6e65 742f 7468 322d 6473  m/th2-net/th2-ds
-0000a3e0: 2d73 6f75 7263 652d 6c77 6470 290a 2020  -source-lwdp).  
-0000a3f0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-0000a400: 2020 2020 2020 2020 2320 352e 2041 5049          # 5. API
-0000a410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000a420: 2020 4966 2079 6f75 2061 7265 206c 6f6f    If you are loo
-0000a430: 6b69 6e67 2066 6f72 2063 6c61 7373 6573  king for classes
-0000a440: 2064 6573 6372 6970 7469 6f6e 2073 6565   description see
-0000a450: 2074 6865 205b 4150 4920 446f 6375 6d65   the [API Docume
-0000a460: 6e74 6174 696f 6e5d 2864 6f63 756d 656e  ntation](documen
-0000a470: 7461 7469 6f6e 2f61 7069 2f69 6e64 6578  tation/api/index
-0000a480: 2e6d 6429 2e0a 2020 2020 2020 2020 0a20  .md)..        . 
-0000a490: 2020 2020 2020 2023 2036 2e20 4578 616d         # 6. Exam
-0000a4a0: 706c 6573 0a20 2020 2020 2020 200a 2020  ples.        .  
-0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
-0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
-0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
-0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
-0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
-0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
-0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-0000a520: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
-0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
-0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
-0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
-0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
-0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
-0000a5a0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-0000a5b0: 7764 7031 0a50 726f 7669 6465 732d 4578  wdp1.Provides-Ex
-0000a5c0: 7472 613a 206c 7764 7032 0a50 726f 7669  tra: lwdp2.Provi
-0000a5d0: 6465 732d 4578 7472 613a 206c 7764 7033  des-Extra: lwdp3
-0000a5e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-0000a5f0: 206c 7764 702d 6465 760a 5072 6f76 6964   lwdp-dev.Provid
-0000a600: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
-0000a610: 7270 742d 7669 6577 6572 0a50 726f 7669  rpt-viewer.Provi
-0000a620: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
-0000a630: 2d72 7074 2d76 6965 7765 7235 0a50 726f  -rpt-viewer5.Pro
-0000a640: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-0000a650: 6c73 2d61 6476 616e 6365 640a            ls-advanced.
+00002700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002710: 230a 2020 2020 2020 2020 0a20 2020 2020  #.        .     
+00002720: 2020 2023 205b 312e 315d 2046 696c 7465     # [1.1] Filte
+00002730: 722e 0a20 2020 2020 2020 2066 696c 7465  r..        filte
+00002740: 7265 645f 6576 656e 7473 3a20 4461 7461  red_events: Data
+00002750: 203d 2065 7665 6e74 732e 6669 6c74 6572   = events.filter
+00002760: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
+00002770: 6d62 6461 2065 3a20 655b 2262 6f64 7922  mbda e: e["body"
+00002780: 5d20 213d 205b 5d29 2020 2320 4669 6c74  ] != [])  # Filt
+00002790: 6572 2065 7665 6e74 7320 7769 7468 2065  er events with e
+000027a0: 6d70 7479 2062 6f64 792e 0a20 2020 2020  mpty body..     
+000027b0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+000027c0: 2020 2020 2023 205b 312e 325d 204d 6170       # [1.2] Map
+000027d0: 2e0a 2020 2020 2020 2020 6465 6620 7472  ..        def tr
+000027e0: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+000027f0: 2872 6563 6f72 6429 3a0a 2020 2020 2020  (record):.      
+00002800: 2020 2020 2020 7265 7475 726e 207b 2265        return {"e
+00002810: 7665 6e74 4e61 6d65 223a 2072 6563 6f72  ventName": recor
+00002820: 645b 2265 7665 6e74 4e61 6d65 225d 2c0a  d["eventName"],.
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
+00002850: 3a20 7265 636f 7264 5b22 7375 6363 6573  : record["succes
+00002860: 7366 756c 225d 7d0a 2020 2020 2020 2020  sful"]}.        
+00002870: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002880: 2020 6669 6c74 6572 6564 5f61 6e64 5f6d    filtered_and_m
+00002890: 6170 7065 645f 6576 656e 7473 203d 2066  apped_events = f
+000028a0: 696c 7465 7265 645f 6576 656e 7473 2e6d  iltered_events.m
+000028b0: 6170 2874 7261 6e73 666f 726d 5f66 756e  ap(transform_fun
+000028c0: 6374 696f 6e29 0a20 2020 2020 2020 200a  ction).        .
+000028d0: 2020 2020 2020 2020 2320 5b31 2e33 5d20          # [1.3] 
+000028e0: 4461 7461 2070 6970 656c 696e 652e 0a20  Data pipeline.. 
+000028f0: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
+00002900: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
+00002910: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
+00002920: 696f 6e73 2073 7465 7020 6279 2073 7465  ions step by ste
+00002930: 7020 796f 7520 6361 6e20 646f 2069 7420  p you can do it 
+00002940: 696e 206f 6e65 206c 696e 652e 0a20 2020  in one line..   
+00002950: 2020 2020 2066 696c 7465 7265 645f 616e       filtered_an
+00002960: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
+00002970: 6279 5f70 6970 656c 696e 6520 3d20 6576  by_pipeline = ev
+00002980: 656e 7473 2e66 696c 7465 7228 0a20 2020  ents.filter(.   
+00002990: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+000029a0: 653a 2065 5b22 626f 6479 225d 2021 3d20  e: e["body"] != 
+000029b0: 5b5d 292e 6d61 7028 0a20 2020 2020 2020  []).map(.       
+000029c0: 2020 2020 2074 7261 6e73 666f 726d 5f66       transform_f
+000029d0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+000029e0: 290a 2020 2020 2020 2020 2320 436f 6e74  ).        # Cont
+000029f0: 656e 7420 6f66 2074 6865 7365 2074 776f  ent of these two
+00002a00: 2044 6174 6120 6f62 6a65 6374 7320 7368   Data objects sh
+00002a10: 6f75 6c64 2062 6520 6571 7561 6c2e 0a20  ould be equal.. 
+00002a20: 2020 2020 2020 2061 7373 6572 7420 6c69         assert li
+00002a30: 7374 2866 696c 7465 7265 645f 616e 645f  st(filtered_and_
+00002a40: 6d61 7070 6564 5f65 7665 6e74 7329 203d  mapped_events) =
+00002a50: 3d20 6c69 7374 280a 2020 2020 2020 2020  = list(.        
+00002a60: 2020 2020 6669 6c74 6572 6564 5f61 6e64      filtered_and
+00002a70: 5f6d 6170 7065 645f 6576 656e 7473 5f62  _mapped_events_b
+00002a80: 795f 7069 7065 6c69 6e65 290a 2020 2020  y_pipeline).    
+00002a90: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00002aa0: 312e 345d 2053 6966 742e 2053 6b69 7020  1.4] Sift. Skip 
+00002ab0: 7468 6520 6669 7273 7420 6665 7720 6974  the first few it
+00002ac0: 656d 7320 6f72 206c 696d 6974 2074 6865  ems or limit the
+00002ad0: 6d2e 0a20 2020 2020 2020 2064 6174 6120  m..        data 
+00002ae0: 3d20 4461 7461 285b 312c 2032 2c20 332c  = Data([1, 2, 3,
+00002af0: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
+00002b00: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
+00002b10: 332c 2031 342c 2031 355d 290a 2020 2020  3, 14, 15]).    
+00002b20: 2020 2020 6974 656d 735f 6672 6f6d 5f31      items_from_1
+00002b30: 315f 746f 5f65 6e64 3a20 4765 6e65 7261  1_to_end: Genera
+00002b40: 746f 7220 3d20 6461 7461 2e73 6966 7428  tor = data.sift(
+00002b50: 736b 6970 3d31 3029 0a20 2020 2020 2020  skip=10).       
+00002b60: 206f 6e6c 795f 6669 7273 745f 3130 5f69   only_first_10_i
+00002b70: 7465 6d73 3a20 4765 6e65 7261 746f 7220  tems: Generator 
+00002b80: 3d20 6461 7461 2e73 6966 7428 6c69 6d69  = data.sift(limi
+00002b90: 743d 3130 290a 2020 2020 2020 2020 0a20  t=10).        . 
+00002ba0: 2020 2020 2020 2023 205b 312e 355d 2043         # [1.5] C
+00002bb0: 6861 6e67 696e 6720 6361 6368 6520 7374  hanging cache st
+00002bc0: 6174 7573 2e0a 2020 2020 2020 2020 6576  atus..        ev
+00002bd0: 656e 7473 2e75 7365 5f63 6163 6865 2854  ents.use_cache(T
+00002be0: 7275 6529 0a20 2020 2020 2020 2023 206f  rue).        # o
+00002bf0: 7220 6a75 7374 0a20 2020 2020 2020 2065  r just.        e
+00002c00: 7665 6e74 732e 7573 655f 6361 6368 6528  vents.use_cache(
+00002c10: 2920 2023 2049 6620 796f 7520 7761 6e74  )  # If you want
+00002c20: 2074 6f20 6163 7469 7661 7465 2063 6163   to activate cac
+00002c30: 6865 2e0a 2020 2020 2020 2020 2320 5b31  he..        # [1
+00002c40: 2e36 5d20 5761 6c6b 2074 6872 6f75 6768  .6] Walk through
+00002c50: 2064 6174 612e 0a20 2020 2020 2020 2066   data..        f
+00002c60: 6f72 2065 7665 6e74 2069 6e20 6576 656e  or event in even
+00002c70: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00002c80: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
+00002c90: 6974 6820 6576 656e 7420 2865 7665 6e74  ith event (event
+00002ca0: 2069 7320 6120 6469 6374 292e 0a20 2020   is a dict)..   
+00002cb0: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
+00002cc0: 7665 6e74 290a 2020 2020 2020 2020 2320  vent).        # 
+00002cd0: 4166 7465 7220 6669 7273 7420 6974 6572  After first iter
+00002ce0: 6174 696f 6e20 7468 6520 6576 656e 7473  ation the events
+00002cf0: 2068 6173 2061 2063 6163 6865 2066 696c   has a cache fil
+00002d00: 652e 0a20 2020 2020 2020 2023 204e 6f77  e..        # Now
+00002d10: 2074 6865 7920 7769 6c6c 2062 6520 7573   they will be us
+00002d20: 6564 2069 6e20 7468 6520 6361 6368 6520  ed in the cache 
+00002d30: 696e 2074 6865 206e 6578 7420 6974 6572  in the next iter
+00002d40: 6174 696f 6e2e 0a20 2020 2020 2020 200a  ation..        .
+00002d50: 2020 2020 2020 2020 2320 5b31 2e37 5d20          # [1.7] 
+00002d60: 4765 7420 6e75 6d62 6572 206f 6620 7468  Get number of th
+00002d70: 6520 656c 656d 656e 7473 2069 6e20 7468  e elements in th
+00002d80: 6520 4461 7461 206f 626a 6563 742e 0a20  e Data object.. 
+00002d90: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+00002da0: 5f65 7665 6e74 7320 3d20 6576 656e 7473  _events = events
+00002db0: 2e6c 656e 0a20 2020 2020 2020 200a 2020  .len.        .  
+00002dc0: 2020 2020 2020 2320 5b31 2e38 5d20 4368        # [1.8] Ch
+00002dd0: 6563 6b20 7468 6174 2044 6174 6120 6f62  eck that Data ob
+00002de0: 6a65 6374 2069 736e 2774 2065 6d70 7479  ject isn't empty
+00002df0: 2e0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+00002e00: 6461 7461 2073 6f75 7263 6520 7368 6f75  data source shou
+00002e10: 6c64 2062 6520 6e6f 7420 656d 7074 792e  ld be not empty.
+00002e20: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002e30: 6576 656e 7473 2e69 735f 656d 7074 7920  events.is_empty 
+00002e40: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+00002e50: 200a 2020 2020 2020 2020 2320 5b31 2e39   .        # [1.9
+00002e60: 5d20 436f 6e76 6572 7420 4461 7461 206f  ] Convert Data o
+00002e70: 626a 6563 7420 746f 2074 6865 206c 6973  bject to the lis
+00002e80: 7420 6f66 2065 6c65 6d65 6e74 7328 6576  t of elements(ev
+00002e90: 656e 7473 206f 7220 6d65 7373 6167 6573  ents or messages
+00002ea0: 292e 0a20 2020 2020 2020 2023 2042 6520  )..        # Be 
+00002eb0: 6361 7265 6675 6c2c 2074 6869 7320 6361  careful, this ca
+00002ec0: 6e20 7461 6b65 2074 6f6f 206d 7563 6820  n take too much 
+00002ed0: 6d65 6d6f 7279 2e0a 2020 2020 2020 2020  memory..        
+00002ee0: 6576 656e 7473 5f6c 6973 7420 3d20 6c69  events_list = li
+00002ef0: 7374 2865 7665 6e74 7329 0a20 2020 2020  st(events).     
+00002f00: 2020 200a 2020 2020 2020 2020 2320 5b31     .        # [1
+00002f10: 2e31 305d 2054 6865 2063 6163 6865 2069  .10] The cache i
+00002f20: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
+00002f30: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
+00002f40: 6e65 7720 4461 7461 206f 626a 6563 7420  new Data object 
+00002f50: 7468 6174 2077 696c 6c20 7573 6520 6361  that will use ca
+00002f60: 6368 6520 6672 6f6d 2074 6865 2065 7665  che from the eve
+00002f70: 6e74 7320 4461 7461 206f 626a 6563 742e  nts Data object.
+00002f80: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
+00002f90: 6669 6c74 6572 6564 3a20 4461 7461 203d  filtered: Data =
+00002fa0: 2065 7665 6e74 732e 6669 6c74 6572 286c   events.filter(l
+00002fb0: 616d 6264 6120 7265 636f 7264 3a20 7265  ambda record: re
+00002fc0: 636f 7264 2e67 6574 2822 6261 7463 6849  cord.get("batchI
+00002fd0: 6422 2929 0a20 2020 2020 2020 200a 2020  d")).        .  
+00002fe0: 2020 2020 2020 2320 4e65 7720 4461 7461        # New Data
+00002ff0: 206f 626a 6563 7473 2064 6f6e 2774 2075   objects don't u
+00003000: 7365 2074 6865 6972 206f 776e 2063 6163  se their own cac
+00003010: 6865 2062 7920 6465 6661 756c 7420 6275  he by default bu
+00003020: 7420 7573 6520 7468 6520 6361 6368 6520  t use the cache 
+00003030: 6f66 2074 6865 2070 6172 656e 7420 4461  of the parent Da
+00003040: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
+00003050: 2020 2023 2055 7365 2075 7365 5f63 6163     # Use use_cac
+00003060: 6865 206d 6574 686f 6420 746f 2061 6374  he method to act
+00003070: 6976 6174 6520 6361 6368 696e 672e 0a20  ivate caching.. 
+00003080: 2020 2020 2020 2023 2041 6674 6572 2074         # After t
+00003090: 6861 742c 2074 6865 2044 6174 6120 6f62  hat, the Data ob
+000030a0: 6a65 6374 2077 696c 6c20 6372 6561 7465  ject will create
+000030b0: 2069 7473 206f 776e 2063 6163 6865 2066   its own cache f
+000030c0: 696c 652e 0a20 2020 2020 2020 2065 7665  ile..        eve
+000030d0: 6e74 735f 6669 6c74 6572 6564 2e75 7365  nts_filtered.use
+000030e0: 5f63 6163 6865 2829 0a20 2020 2020 2020  _cache().       
+000030f0: 200a 2020 2020 2020 2020 6c69 7374 280a   .        list(.
+00003100: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00003110: 7473 5f66 696c 7465 7265 6429 2020 2320  ts_filtered)  # 
+00003120: 4a75 7374 2074 6f20 6974 6572 6174 6520  Just to iterate 
+00003130: 4461 7461 206f 626a 6563 7420 2863 6163  Data object (cac
+00003140: 6865 2066 696c 6520 7769 6c6c 2062 6520  he file will be 
+00003150: 6372 6561 7465 6429 2e0a 2020 2020 2020  created)..      
+00003160: 2020 0a20 2020 2020 2020 2066 696c 7465    .        filte
+00003170: 7265 645f 6576 656e 7473 5f74 7970 6573  red_events_types
+00003180: 203d 2065 7665 6e74 735f 6669 6c74 6572   = events_filter
+00003190: 6564 2e6d 6170 280a 2020 2020 2020 2020  ed.map(.        
+000031a0: 2020 2020 6c61 6d62 6461 2072 6563 6f72      lambda recor
+000031b0: 643a 207b 2265 7665 6e74 5479 7065 223a  d: {"eventType":
+000031c0: 2072 6563 6f72 642e 6765 7428 2265 7665   record.get("eve
+000031d0: 6e74 5479 7065 2229 7d29 0a20 2020 2020  ntType")}).     
+000031e0: 2020 200a 2020 2020 2020 2020 6576 656e     .        even
+000031f0: 7473 5f77 6974 686f 7574 5f74 7970 6573  ts_without_types
+00003200: 5f77 6974 685f 6261 7463 6820 3d20 6669  _with_batch = fi
+00003210: 6c74 6572 6564 5f65 7665 6e74 735f 7479  ltered_events_ty
+00003220: 7065 732e 6669 6c74 6572 280a 2020 2020  pes.filter(.    
+00003230: 2020 2020 2020 2020 6c61 6d62 6461 2072          lambda r
+00003240: 6563 6f72 643a 206e 6f74 2072 6563 6f72  ecord: not recor
+00003250: 642e 6765 7428 2265 7665 6e74 5479 7065  d.get("eventType
+00003260: 2229 0a20 2020 2020 2020 2029 0a20 2020  ").        ).   
+00003270: 2020 2020 2065 7665 6e74 735f 7769 7468       events_with
+00003280: 6f75 745f 7479 7065 735f 7769 7468 5f62  out_types_with_b
+00003290: 6174 6368 2e75 7365 5f63 6163 6865 2829  atch.use_cache()
+000032a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000032b0: 2020 2320 5b31 2e31 315d 2044 6174 6120    # [1.11] Data 
+000032c0: 6f62 6a65 6374 7320 6a6f 696e 696e 672e  objects joining.
+000032d0: 0a20 2020 2020 2020 2023 2059 6f75 2068  .        # You h
+000032e0: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
+000032f0: 6720 3320 4461 7461 206f 626a 6563 7473  g 3 Data objects
+00003300: 2e0a 2020 2020 2020 2020 6431 203d 2044  ..        d1 = D
+00003310: 6174 6128 5b31 2c20 322c 2033 5d29 0a20  ata([1, 2, 3]). 
+00003320: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
+00003330: 285b 2261 222c 207b 2269 6422 3a20 3132  (["a", {"id": 12
+00003340: 337d 2c20 2263 225d 290a 2020 2020 2020  3}, "c"]).      
+00003350: 2020 6433 203d 2044 6174 6128 5b37 2c20    d3 = Data([7, 
+00003360: 382c 2039 5d29 0a20 2020 2020 2020 2023  8, 9]).        #
+00003370: 2059 6f75 2063 616e 206a 6f69 6e20 4461   You can join Da
+00003380: 7461 206f 626a 6563 7473 2069 6e20 666f  ta objects in fo
+00003390: 6c6c 6f77 696e 6720 7761 7973 2e0a 2020  llowing ways..  
+000033a0: 2020 2020 2020 2320 506c 6561 7365 206e        # Please n
+000033b0: 6f74 652c 206e 6577 2044 6174 6120 6f62  ote, new Data ob
+000033c0: 6a65 6374 2077 696c 6c20 6861 7665 2063  ject will have c
+000033d0: 6163 6865 2073 7461 7475 7320 3d3d 2046  ache status == F
+000033e0: 616c 7365 2e0a 2020 2020 2020 2020 6461  alse..        da
+000033f0: 7461 5f76 6961 5f69 6e69 7420 3d20 4461  ta_via_init = Da
+00003400: 7461 285b 6431 2c20 6432 2c20 6433 5d29  ta([d1, d2, d3])
+00003410: 0a20 2020 2020 2020 2064 6174 615f 7669  .        data_vi
+00003420: 615f 6164 6420 3d20 6431 202b 2064 3220  a_add = d1 + d2 
+00003430: 2b20 6433 0a20 2020 2020 2020 2064 6174  + d3.        dat
+00003440: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00003450: 6f62 6a5f 7669 615f 696e 6974 203d 2044  obj_via_init = D
+00003460: 6174 6128 5b64 312c 205b 2261 222c 207b  ata([d1, ["a", {
+00003470: 2269 6422 3a20 3132 337d 2c20 2263 225d  "id": 123}, "c"]
+00003480: 2c20 6433 5d29 0a20 2020 2020 2020 2064  , d3]).        d
+00003490: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+000034a0: 615f 6f62 6a5f 7669 615f 6164 6420 3d20  a_obj_via_add = 
+000034b0: 6431 202b 205b 2261 222c 207b 2269 6422  d1 + ["a", {"id"
+000034c0: 3a20 3132 337d 2c20 2263 225d 202b 2064  : 123}, "c"] + d
+000034d0: 330a 2020 2020 2020 2020 2320 596f 7520  3.        # You 
+000034e0: 6361 6e20 6a6f 696e 2063 7572 7265 6e74  can join current
+000034f0: 2044 6174 6120 6f62 6a65 6374 206f 6e20   Data object on 
+00003500: 706c 6163 6520 7573 696e 6720 2b3d 2e0a  place using +=..
+00003510: 2020 2020 2020 2020 2320 4974 2077 696c          # It wil
+00003520: 6c20 6b65 6570 2063 6163 6865 2073 7461  l keep cache sta
+00003530: 7475 732e 0a20 2020 2020 2020 2064 3120  tus..        d1 
+00003540: 2b3d 2064 3320 2023 2064 3120 7769 6c6c  += d3  # d1 will
+00003550: 2062 6563 6f6d 6520 4461 7461 285b 312c   become Data([1,
+00003560: 322c 332c 372c 382c 395d 290a 2020 2020  2,3,7,8,9]).    
+00003570: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00003580: 312e 3132 5d20 4275 696c 6420 616e 6420  1.12] Build and 
+00003590: 7265 6164 2044 6174 6120 6f62 6a65 6374  read Data object
+000035a0: 2063 6163 6865 2066 696c 6573 2e0a 2020   cache files..  
+000035b0: 2020 2020 2020 6576 656e 7473 2e62 7569        events.bui
+000035c0: 6c64 5f63 6163 6865 2822 6361 6368 655f  ld_cache("cache_
+000035d0: 6669 6c65 6e61 6d65 5f6f 725f 7061 7468  filename_or_path
+000035e0: 2229 0a20 2020 2020 2020 2064 6174 615f  ").        data_
+000035f0: 6f62 6a5f 6672 6f6d 5f63 6163 6865 203d  obj_from_cache =
+00003600: 2044 6174 612e 6672 6f6d 5f63 6163 6865   Data.from_cache
+00003610: 5f66 696c 6528 2263 6163 6865 5f66 696c  _file("cache_fil
+00003620: 656e 616d 655f 6f72 5f70 6174 6822 290a  ename_or_path").
+00003630: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003640: 2023 205b 312e 3133 5d20 4368 6563 6b20   # [1.13] Check 
+00003650: 6966 2044 6174 6120 6973 2073 6f72 7465  if Data is sorte
+00003660: 642e 0a20 2020 2020 2020 2023 2054 6861  d..        # Tha
+00003670: 7420 7769 6c6c 2072 6574 7572 6e20 616e  t will return an
+00003680: 206f 626a 6563 7420 6069 735f 736f 7274   object `is_sort
+00003690: 6564 6020 7468 6174 2063 6f6e 7461 696e  ed` that contain
+000036a0: 7320 696e 666f 726d 6174 696f 6e0a 2020  s information.  
+000036b0: 2020 2020 2020 2320 2020 312e 2073 7461        #   1. sta
+000036c0: 7475 7320 2d2d 2073 6f72 7465 6420 6f72  tus -- sorted or
+000036d0: 206e 6f74 0a20 2020 2020 2020 2023 2020   not.        #  
+000036e0: 2032 2e20 6669 7273 745f 756e 736f 7274   2. first_unsort
+000036f0: 6564 202d 2d20 7468 6520 696e 6465 7820  ed -- the index 
+00003700: 6f66 2074 6865 2066 6972 7374 2075 6e73  of the first uns
+00003710: 6f72 7465 6420 656c 656d 656e 740a 2020  orted element.  
+00003720: 2020 2020 2020 6973 5f73 6f72 7465 6420        is_sorted 
+00003730: 3d20 6576 656e 7473 2e69 735f 736f 7274  = events.is_sort
+00003740: 6564 286c 616d 6264 6120 653a 2065 5b22  ed(lambda e: e["
+00003750: 7374 6172 7454 696d 6573 7461 6d70 225d  startTimestamp"]
+00003760: 5b22 6570 6f63 6853 6563 6f6e 6422 5d29  ["epochSecond"])
+00003770: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003780: 2020 2320 596f 7520 6361 6e20 7573 6520    # You can use 
+00003790: 7468 6973 206f 626a 6563 7420 6173 2075  this object as u
+000037a0: 7375 616c 2062 6f6f 6c20 7661 7269 6162  sual bool variab
+000037b0: 6c65 2e0a 2020 2020 2020 2020 6966 2069  le..        if i
+000037c0: 735f 736f 7274 6564 3a0a 2020 2020 2020  s_sorted:.      
+000037d0: 2020 2020 2020 7072 696e 7428 2265 7665        print("eve
+000037e0: 6e74 7320 4461 7461 206f 626a 2069 7320  nts Data obj is 
+000037f0: 736f 7274 6564 2122 290a 2020 2020 2020  sorted!").      
+00003800: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00003810: 3134 5d20 5573 6520 6044 6174 612e 7368  14] Use `Data.sh
+00003820: 6f77 2829 6020 746f 206c 6f6f 6b20 6174  ow()` to look at
+00003830: 2074 6865 2066 6972 7374 204e 206d 6573   the first N mes
+00003840: 7361 6765 7320 696e 2074 6865 2073 7472  sages in the str
+00003850: 6561 6d2e 0a20 2020 2020 2020 2064 6174  eam..        dat
+00003860: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00003870: 6f62 6a5f 7669 615f 6164 642e 7368 6f77  obj_via_add.show
+00003880: 286e 3d36 290a 2020 2020 2020 2020 2320  (n=6).        # 
+00003890: 5769 6c6c 2070 7269 6e74 0a20 2020 2020  Will print.     
+000038a0: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+000038b0: 2d2d 2050 7269 6e74 6564 2066 6972 7374  -- Printed first
+000038c0: 2036 2072 6563 6f72 6473 202d 2d2d 2d2d   6 records -----
+000038d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000038e0: 2023 205b 315d 202d 2d2d 2d2d 2d0a 2020   # [1] ------.  
+000038f0: 2020 2020 2020 2320 310a 2020 2020 2020        # 1.      
+00003900: 2020 2320 5b32 5d20 2d2d 2d2d 2d2d 0a20    # [2] ------. 
+00003910: 2020 2020 2020 2023 2032 0a20 2020 2020         # 2.     
+00003920: 2020 2023 205b 335d 202d 2d2d 2d2d 2d0a     # [3] ------.
+00003930: 2020 2020 2020 2020 2320 330a 2020 2020          # 3.    
+00003940: 2020 2020 2320 5b34 5d20 2d2d 2d2d 2d2d      # [4] ------
+00003950: 0a20 2020 2020 2020 2023 2027 6127 0a20  .        # 'a'. 
+00003960: 2020 2020 2020 2023 205b 355d 202d 2d2d         # [5] ---
+00003970: 2d2d 2d0a 2020 2020 2020 2020 2320 7b27  ---.        # {'
+00003980: 6964 273a 2031 3233 7d0a 2020 2020 2020  id': 123}.      
+00003990: 2020 2320 5b36 5d20 2d2d 2d2d 2d2d 0a20    # [6] ------. 
+000039a0: 2020 2020 2020 2023 2027 6327 0a20 2020         # 'c'.   
+000039b0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000039c0: 5b31 2e31 355d 2059 6f75 2063 616e 2072  [1.15] You can r
+000039d0: 656d 6f76 6520 7468 6520 6361 6368 6520  emove the cache 
+000039e0: 6669 6c65 206f 6620 7468 6520 4461 7461  file of the Data
+000039f0: 206f 626a 6563 742c 2069 6620 7265 7175   object, if requ
+00003a00: 6972 6564 2e0a 2020 2020 2020 2020 6461  ired..        da
+00003a10: 7461 5f6f 626a 5f66 726f 6d5f 6361 6368  ta_obj_from_cach
+00003a20: 652e 636c 6561 725f 6361 6368 6528 290a  e.clear_cache().
+00003a30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003a40: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00003a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a60: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00003a70: 2320 5b32 5d20 576f 726b 696e 6720 7769  # [2] Working wi
+00003a80: 7468 2063 6f6e 7665 7274 6572 732e 0a20  th converters.. 
+00003a90: 2020 2020 2020 2023 2323 2323 2323 2323         #########
+00003aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003ab0: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
+00003ac0: 2020 2020 2020 2320 5468 6572 6520 6172        # There ar
+00003ad0: 6520 6375 7272 656e 746c 7920 7468 7265  e currently thre
+00003ae0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00003af0: 7320 6f66 2049 5469 6d65 7374 616d 7043  s of ITimestampC
+00003b00: 6f6e 7665 7274 6572 2063 6c61 7373 3a20  onverter class: 
+00003b10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003b20: 2c20 4461 7465 7469 6d65 5374 7269 6e67  , DatetimeString
+00003b30: 436f 6e76 6572 7465 7220 616e 6420 5072  Converter and Pr
+00003b40: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
+00003b50: 6f6e 7665 7274 6572 2e0a 2020 2020 2020  onverter..      
+00003b60: 2020 2320 5468 6579 2061 6c6c 2069 6d70    # They all imp
+00003b70: 6c65 6d65 6e74 2073 616d 6520 6d65 7468  lement same meth
+00003b80: 6f64 7320 6672 6f6d 2062 6173 6520 636c  ods from base cl
+00003b90: 6173 732e 0a20 2020 2020 2020 2023 204e  ass..        # N
+00003ba0: 6f74 6520 7468 6174 2073 6f6d 6520 6163  ote that some ac
+00003bb0: 6375 7261 6379 206d 6179 2062 6520 6c6f  curacy may be lo
+00003bc0: 7374 2064 7572 696e 6720 636f 6e76 6572  st during conver
+00003bd0: 7369 6f6e 2e0a 2020 2020 2020 2020 2320  sion..        # 
+00003be0: 4966 2066 6f72 2065 7861 6d70 6c65 2079  If for example y
+00003bf0: 6f75 2075 7365 2074 6f5f 6d69 6372 6f73  ou use to_micros
+00003c00: 6563 6f6e 6473 206e 616e 6f73 6563 6f6e  econds nanosecon
+00003c10: 6473 2077 696c 6c20 6265 2063 7574 206f  ds will be cut o
+00003c20: 6666 2069 6e73 7465 6164 206f 6620 726f  ff instead of ro
+00003c30: 756e 6469 6e67 2e0a 2020 2020 2020 2020  unding..        
+00003c40: 0a20 2020 2020 2020 2023 205b 322e 315d  .        # [2.1]
+00003c50: 2044 6174 6574 696d 6543 6f6e 7665 7274   DatetimeConvert
+00003c60: 6572 2e0a 2020 2020 2020 2020 2320 4461  er..        # Da
+00003c70: 7465 7469 6d65 436f 6e76 6572 7465 7220  tetimeConverter 
+00003c80: 7461 6b65 7320 6461 7465 7469 6d65 2e64  takes datetime.d
+00003c90: 6174 6574 696d 6520 6f62 6a65 6374 2061  atetime object a
+00003ca0: 7320 696e 7075 742e 0a20 2020 2020 2020  s input..       
+00003cb0: 200a 2020 2020 2020 2020 6461 7465 7469   .        dateti
+00003cc0: 6d65 5f6f 626a 203d 2064 6174 6574 696d  me_obj = datetim
+00003cd0: 6528 7965 6172 3d32 3032 332c 206d 6f6e  e(year=2023, mon
+00003ce0: 7468 3d31 2c20 6461 793d 352c 2068 6f75  th=1, day=5, hou
+00003cf0: 723d 3134 2c20 6d69 6e75 7465 3d33 382c  r=14, minute=38,
+00003d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d20: 2073 6563 6f6e 643d 3235 2c20 6d69 6372   second=25, micr
+00003d30: 6f73 6563 6f6e 643d 3134 3630 290a 2020  osecond=1460).  
+00003d40: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003d50: 2049 7420 6861 7320 6d65 7468 6f64 7320   It has methods 
+00003d60: 7468 6174 2072 6574 7572 6e20 7468 6520  that return the 
+00003d70: 6461 7465 7469 6d65 2069 6e20 6469 6666  datetime in diff
+00003d80: 6572 656e 7420 666f 726d 6173 3a0a 2020  erent formas:.  
+00003d90: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+00003da0: 6174 655f 6d73 203d 2044 6174 6574 696d  ate_ms = Datetim
+00003db0: 6543 6f6e 7665 7274 6572 2e74 6f5f 6d69  eConverter.to_mi
+00003dc0: 6c6c 6973 6563 6f6e 6473 2864 6174 6574  lliseconds(datet
+00003dd0: 696d 655f 6f62 6a29 0a20 2020 2020 2020  ime_obj).       
+00003de0: 2064 6174 655f 7573 203d 2044 6174 6574   date_us = Datet
+00003df0: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003e00: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
+00003e10: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003e20: 2020 2023 2043 6f6e 7665 7274 696e 6720     # Converting 
+00003e30: 746f 206e 616e 6f73 6563 6f6e 6473 206a  to nanoseconds j
+00003e40: 7573 7473 2061 6464 7320 7468 7265 6520  usts adds three 
+00003e50: 7472 6169 6c69 6e67 207a 6572 6f73 2061  trailing zeros a
+00003e60: 7320 6461 7465 7469 6d65 206f 626a 6563  s datetime objec
+00003e70: 7420 646f 6573 6e27 7420 6861 7665 206e  t doesn't have n
+00003e80: 616e 6f73 6563 6f6e 6473 2e0a 2020 2020  anoseconds..    
+00003e90: 2020 2020 6461 7465 5f6e 7320 3d20 4461      date_ns = Da
+00003ea0: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+00003eb0: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
+00003ec0: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+00003ed0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003ee0: 5b32 2e32 5d20 4461 7465 7469 6d65 5374  [2.2] DatetimeSt
+00003ef0: 7269 6e67 436f 6e76 6572 7465 720a 2020  ringConverter.  
+00003f00: 2020 2020 2020 2320 4461 7465 7469 6d65        # Datetime
+00003f10: 5374 7269 6e67 436f 6e76 6572 7465 7220  StringConverter 
+00003f20: 7461 6b65 7320 7374 7269 6e67 2069 6e20  takes string in 
+00003f30: 2279 7979 792d 4d4d 2d64 6454 4848 3a6d  "yyyy-MM-ddTHH:m
+00003f40: 6d3a 7373 5b2e 5353 5353 5353 5353 535d  m:ss[.SSSSSSSSS]
+00003f50: 5a22 2066 6f72 6d61 742e 0a20 2020 2020  Z" format..     
+00003f60: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003f70: 5f73 7472 696e 6720 3d20 2232 3032 332d  _string = "2023-
+00003f80: 3031 2d30 3554 3134 3a33 383a 3235 2e30  01-05T14:38:25.0
+00003f90: 3031 3436 5a22 0a20 2020 2020 2020 200a  0146Z".        .
+00003fa0: 2020 2020 2020 2020 2320 5765 2068 6176          # We hav
+00003fb0: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+00003fc0: 7320 696e 2044 6174 6574 696d 6543 6f6e  s in DatetimeCon
+00003fd0: 7665 7274 6572 0a20 2020 2020 2020 2064  verter.        d
+00003fe0: 6174 655f 6d73 5f66 726f 6d5f 7374 7269  ate_ms_from_stri
+00003ff0: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
+00004000: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
+00004010: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00004020: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
+00004030: 2020 6461 7465 5f75 735f 6672 6f6d 5f73    date_us_from_s
+00004040: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
+00004050: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
+00004060: 746f 5f6d 6963 726f 7365 636f 6e64 7328  to_microseconds(
+00004070: 6461 7465 5f73 7472 696e 6729 0a20 2020  date_string).   
+00004080: 2020 2020 2064 6174 655f 6e73 5f66 726f       date_ns_fro
+00004090: 6d5f 7374 7269 6e67 203d 2044 6174 6574  m_string = Datet
+000040a0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000040b0: 6572 2e74 6f5f 6e61 6e6f 7365 636f 6e64  er.to_nanosecond
+000040c0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+000040d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000040e0: 2320 5765 2063 616e 2061 6c73 6f20 6765  # We can also ge
+000040f0: 7420 6461 7465 7469 6d65 206f 626a 6563  t datetime objec
+00004100: 7420 6672 6f6d 2073 7472 696e 670a 2020  t from string.  
+00004110: 2020 2020 2020 6461 7465 7469 6d65 5f66        datetime_f
+00004120: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00004130: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00004140: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00004150: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
+00004160: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004170: 205b 322e 335d 2050 726f 746f 6275 6654   [2.3] ProtobufT
+00004180: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+00004190: 720a 2020 2020 2020 2020 2320 5072 6f74  r.        # Prot
+000041a0: 6f62 7566 2074 696d 6573 7461 6d70 7320  obuf timestamps 
+000041b0: 6d75 7374 2062 6520 696e 2066 6f72 6d20  must be in form 
+000041c0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+000041d0: 7365 636f 6e64 732c 2022 6e61 6e6f 223a  seconds, "nano":
+000041e0: 206e 616e 6f73 6563 6f6e 6473 7d0a 2020   nanoseconds}.  
+000041f0: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00004200: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+00004210: 7020 3d20 7b22 6570 6f63 6853 6563 6f6e  p = {"epochSecon
+00004220: 6422 3a20 3136 3732 3932 3935 3035 2c20  d": 1672929505, 
+00004230: 226e 616e 6f22 3a20 315f 3436 305f 3030  "nano": 1_460_00
+00004240: 307d 0a20 2020 2020 2020 200a 2020 2020  0}.        .    
+00004250: 2020 2020 6461 7465 5f6d 735f 6672 6f6d      date_ms_from
+00004260: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00004270: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00004280: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
+00004290: 7365 636f 6e64 7328 0a20 2020 2020 2020  seconds(.       
+000042a0: 2020 2020 2070 726f 746f 6275 665f 7469       protobuf_ti
+000042b0: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
+000042c0: 2064 6174 655f 7573 5f66 726f 6d5f 7469   date_us_from_ti
+000042d0: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
+000042e0: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
+000042f0: 7274 6572 2e74 6f5f 6d69 6372 6f73 6563  rter.to_microsec
+00004300: 6f6e 6473 280a 2020 2020 2020 2020 2020  onds(.          
+00004310: 2020 7072 6f74 6f62 7566 5f74 696d 6573    protobuf_times
+00004320: 7461 6d70 290a 2020 2020 2020 2020 6461  tamp).        da
+00004330: 7465 5f6e 735f 6672 6f6d 5f74 696d 6573  te_ns_from_times
+00004340: 7461 6d70 203d 2050 726f 746f 6275 6654  tamp = ProtobufT
+00004350: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+00004360: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
+00004370: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00004380: 6f74 6f62 7566 5f74 696d 6573 7461 6d70  otobuf_timestamp
+00004390: 290a 2020 2020 2020 2020 6461 7465 7469  ).        dateti
+000043a0: 6d65 5f66 726f 6d5f 7469 6d65 7374 616d  me_from_timestam
+000043b0: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
+000043c0: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
+000043d0: 6f5f 6461 7465 7469 6d65 280a 2020 2020  o_datetime(.    
+000043e0: 2020 2020 2020 2020 7072 6f74 6f62 7566          protobuf
+000043f0: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+00004400: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00004410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004430: 2323 230a 2020 2020 2020 2020 2320 5b33  ###.        # [3
+00004440: 5d20 576f 726b 696e 6720 7769 7468 2045  ] Working with E
+00004450: 7665 6e74 5472 6565 2061 6e64 2045 7665  ventTree and Eve
+00004460: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00004470: 2e0a 2020 2020 2020 2020 2323 2323 2323  ..        ######
+00004480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000044a0: 0a20 2020 2020 2020 2023 2043 616e 2062  .        # Can b
+000044b0: 6520 7573 6566 756c 2069 6620 796f 7520  e useful if you 
+000044c0: 6861 7665 2064 6174 612d 7374 7265 616d  have data-stream
+000044d0: 2077 6974 6820 3c20 3130 306b 2065 6c65   with < 100k ele
+000044e0: 6d65 6e74 732c 206f 7468 6572 7769 7365  ments, otherwise
+000044f0: 2069 740a 2020 2020 2020 2020 2320 7461   it.        # ta
+00004500: 6b65 7320 746f 6f20 6d75 6368 2052 414d  kes too much RAM
+00004510: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00004520: 2020 2023 205b 332e 315d 2042 7569 6c64     # [3.1] Build
+00004530: 2061 2063 7573 746f 6d20 4576 656e 7454   a custom EventT
+00004540: 7265 650a 2020 2020 2020 2020 2320 546f  ree.        # To
+00004550: 2063 7265 6174 6520 616e 2045 7665 6e74   create an Event
+00004560: 5472 6565 206f 626a 6563 7420 796f 7520  Tree object you 
+00004570: 6e65 6564 2074 6f20 7072 6f76 6964 6520  need to provide 
+00004580: 6e61 6d65 2c20 6964 2061 6e64 2064 6174  name, id and dat
+00004590: 6120 6f66 2074 6865 2072 6f6f 7420 6576  a of the root ev
+000045a0: 656e 742e 0a20 2020 2020 2020 2074 7265  ent..        tre
+000045b0: 6520 3d20 4576 656e 7454 7265 6528 6576  e = EventTree(ev
+000045c0: 656e 745f 6e61 6d65 3d22 726f 6f74 2065  ent_name="root e
+000045d0: 7665 6e74 222c 2065 7665 6e74 5f69 643d  vent", event_id=
+000045e0: 2272 6f6f 745f 6964 222c 0a20 2020 2020  "root_id",.     
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 6461 7461 3d7b 2264 6174 6122      data={"data"
+00004610: 3a20 5b31 2c20 322c 2033 2c20 342c 2035  : [1, 2, 3, 4, 5
+00004620: 5d7d 290a 2020 2020 2020 2020 0a20 2020  ]}).        .   
+00004630: 2020 2020 2023 2054 6f20 6164 6420 6e65       # To add ne
+00004640: 7720 6e6f 6465 2075 7365 2061 7070 656e  w node use appen
+00004650: 645f 6576 656e 742e 2070 6172 656e 745f  d_event. parent_
+00004660: 6964 2069 7320 6e65 6365 7373 6172 792c  id is necessary,
+00004670: 2064 6174 6120 6973 206f 7074 696f 6e61   data is optiona
+00004680: 6c2e 0a20 2020 2020 2020 2074 7265 652e  l..        tree.
+00004690: 6170 7065 6e64 5f65 7665 6e74 2865 7665  append_event(eve
+000046a0: 6e74 5f6e 616d 653d 2241 222c 2065 7665  nt_name="A", eve
+000046b0: 6e74 5f69 643d 2241 5f69 6422 2c20 6461  nt_id="A_id", da
+000046c0: 7461 3d4e 6f6e 652c 0a20 2020 2020 2020  ta=None,.       
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2070 6172 656e 745f 6964 3d22 726f     parent_id="ro
+000046f0: 6f74 5f69 6422 290a 2020 2020 2020 2020  ot_id").        
+00004700: 0a20 2020 2020 2020 2023 205b 332e 335d  .        # [3.3]
+00004710: 2042 7569 6c64 696e 6720 7468 6520 4576   Building the Ev
+00004720: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00004730: 6e2e 0a20 2020 2020 2020 2064 6174 615f  n..        data_
+00004740: 736f 7572 6365 3a20 4944 6174 6153 6f75  source: IDataSou
+00004750: 7263 6520 2023 2059 6f75 2073 686f 756c  rce  # You shoul
+00004760: 6420 696e 6974 2044 6174 6153 6f75 7263  d init DataSourc
+00004770: 6520 6f62 6a65 6374 2e20 452e 672e 2066  e object. E.g. f
+00004780: 726f 6d20 4c77 4450 206d 6f64 756c 652e  rom LwDP module.
+00004790: 0a20 2020 2020 2020 2064 6174 615f 736f  .        data_so
+000047a0: 7572 6365 203d 2044 756d 6d79 4461 7461  urce = DummyData
+000047b0: 536f 7572 6365 2829 2020 2320 4e6f 7465  Source()  # Note
+000047c0: 2120 5765 2075 7365 2066 616b 6520 4453  ! We use fake DS
+000047d0: 2068 6572 652e 0a20 2020 2020 2020 2023   here..        #
+000047e0: 2045 5443 4472 6976 6572 2068 6572 6520   ETCDriver here 
+000047f0: 6973 2061 2073 7475 622c 2061 6374 7561  is a stub, actua
+00004800: 6c6c 7920 7468 6520 6c69 6220 646f 6573  lly the lib does
+00004810: 6e27 7420 6861 7665 2073 7563 6820 6120  n't have such a 
+00004820: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
+00004830: 2059 6f75 2063 616e 2074 616b 6520 6974   You can take it
+00004840: 2069 6e20 4c77 4450 206d 6f64 756c 6520   in LwDP module 
+00004850: 6f72 2063 7265 6174 6520 796f 7572 7365  or create yourse
+00004860: 6c66 2063 6c61 7373 2069 6620 796f 7520  lf class if you 
+00004870: 6861 7665 2073 6f6d 6520 7370 6563 6961  have some specia
+00004880: 6c20 6576 656e 7473 2073 7472 7563 7475  l events structu
+00004890: 7265 2e0a 2020 2020 2020 2020 6672 6f6d  re..        from
+000048a0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+000048b0: 6573 2e64 6174 615f 736f 7572 6365 2e6c  es.data_source.l
+000048c0: 7764 702e 6576 656e 745f 7472 6565 2069  wdp.event_tree i
+000048d0: 6d70 6f72 740a 2020 2020 2020 2020 0a20  mport.        . 
+000048e0: 2020 2020 2020 2048 7474 7045 5443 4472         HttpETCDr
+000048f0: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
+00004900: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00004910: 2020 2023 2049 6620 796f 7520 646f 6e27     # If you don'
+00004920: 7420 7370 6563 6966 7920 6461 7461 5f73  t specify data_s
+00004930: 6f75 7263 6520 666f 7220 7468 6520 6472  ource for the dr
+00004940: 6976 6572 2074 6865 6e20 6974 2077 6f6e  iver then it won
+00004950: 2774 2072 6563 6f76 6572 2064 6574 6163  't recover detac
+00004960: 6865 6420 6576 656e 7473 2e0a 2020 2020  hed events..    
+00004970: 2020 2020 6472 6976 6572 3a20 4945 5443      driver: IETC
+00004980: 4472 6976 6572 2020 2320 596f 7520 7368  Driver  # You sh
+00004990: 6f75 6c64 2069 6e69 7420 4554 4344 7269  ould init ETCDri
+000049a0: 7665 7220 6f62 6a65 6374 2e20 452e 672e  ver object. E.g.
+000049b0: 2066 726f 6d20 4c77 4450 206d 6f64 756c   from LwDP modul
+000049c0: 6520 6f72 2079 6f75 7220 6375 7374 6f6d  e or your custom
+000049d0: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
+000049e0: 6472 6976 6572 203d 2045 5443 4472 6976  driver = ETCDriv
+000049f0: 6572 2864 6174 615f 736f 7572 6365 3d64  er(data_source=d
+00004a00: 6174 615f 736f 7572 6365 2c20 7573 655f  ata_source, use_
+00004a10: 7374 7562 3d54 7275 6529 0a20 2020 2020  stub=True).     
+00004a20: 2020 200a 2020 2020 2020 2020 6574 6320     .        etc 
+00004a30: 3d20 4576 656e 7454 7265 6543 6f6c 6c65  = EventTreeColle
+00004a40: 6374 696f 6e28 6472 6976 6572 290a 2020  ction(driver).  
+00004a50: 2020 2020 2020 6574 632e 6275 696c 6428        etc.build(
+00004a60: 6576 656e 7473 290a 2020 2020 2020 2020  events).        
+00004a70: 6574 632e 7368 6f77 2829 0a20 2020 2020  etc.show().     
+00004a80: 2020 2023 2049 7427 6c6c 2070 7269 6e74     # It'll print
+00004a90: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00004aa0: 2020 2020 2020 2020 2320 5365 7420 6f66          # Set of
+00004ab0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
+00004ac0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
+00004ad0: 6220 7465 7374 696e 670a 2020 2020 2020  b testing.      
+00004ae0: 2020 2320 e294 9ce2 9480 e294 8020 506c    # ......... Pl
+00004af0: 6169 6e20 6576 656e 7420 310a 2020 2020  ain event 1.    
+00004b00: 2020 2020 2320 e294 94e2 9480 e294 8020      # ......... 
+00004b10: 506c 6169 6e20 6576 656e 7420 320a 2020  Plain event 2.  
+00004b20: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00004b30: 7269 6e74 2865 7463 290a 2020 2020 2020  rint(etc).      
+00004b40: 2020 2320 4576 656e 7454 7265 6543 6f6c    # EventTreeCol
+00004b50: 6c65 6374 696f 6e28 7472 6565 733d 312c  lection(trees=1,
+00004b60: 2065 7665 6e74 733d 335b 7472 6565 733d   events=3[trees=
+00004b70: 332c 2064 6574 6163 6865 643d 305d 290a  3, detached=0]).
+00004b80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004b90: 2023 2044 6574 6163 6865 6420 6576 656e   # Detached even
+00004ba0: 7473 2069 736e 2774 2065 6d70 7479 2e0a  ts isn't empty..
+00004bb0: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
+00004bc0: 7463 2e67 6574 5f64 6574 6163 6865 645f  tc.get_detached_
+00004bd0: 6576 656e 7473 2829 2020 2320 7265 7475  events()  # retu
+00004be0: 726e 7320 6c69 7374 206f 6620 6465 7461  rns list of deta
+00004bf0: 6368 6564 5f65 7665 6e74 732e 0a20 2020  ched_events..   
+00004c00: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00004c10: 7265 636f 7665 725f 756e 6b6e 6f77 6e5f  recover_unknown_
+00004c20: 6576 656e 7473 202d 2d20 7573 6564 2074  events -- used t
+00004c30: 6f20 7265 636f 7665 7220 736f 6d65 2065  o recover some e
+00004c40: 7665 6e74 7320 7061 7265 6e74 732e 0a20  vents parents.. 
+00004c50: 2020 2020 2020 2023 2054 6861 7420 776f         # That wo
+00004c60: 6e27 7420 776f 726b 2077 6974 6820 4475  n't work with Du
+00004c70: 6d6d 7944 6174 6153 6f75 7263 652c 2073  mmyDataSource, s
+00004c80: 6f20 7761 7320 636f 6d6d 656e 7465 640a  o was commented.
+00004c90: 2020 2020 2020 2020 2320 6574 632e 7265          # etc.re
+00004ca0: 636f 7665 725f 756e 6b6e 6f77 6e5f 6576  cover_unknown_ev
+00004cb0: 656e 7473 2829 0a20 2020 2020 2020 200a  ents().        .
+00004cc0: 2020 2020 2020 2020 2320 4166 7465 7220          # After 
+00004cd0: 7468 6174 2074 6865 2064 6574 6163 6865  that the detache
+00004ce0: 6420 6576 656e 7473 2073 686f 756c 6420  d events should 
+00004cf0: 6265 2065 6d70 7479 2062 6563 6175 7365  be empty because
+00004d00: 2074 6865 7920 7765 7265 2072 6563 6f76   they were recov
+00004d10: 6572 6564 2e0a 2020 2020 2020 2020 2320  ered..        # 
+00004d20: 6173 7365 7274 206e 6f74 2065 7463 2e67  assert not etc.g
+00004d30: 6574 5f64 6574 6163 6865 645f 6576 656e  et_detached_even
+00004d40: 7473 2829 0a20 2020 2020 2020 200a 2020  ts().        .  
+00004d50: 2020 2020 2020 2320 2d2d 2d2d 2d0a 2020        # -----.  
+00004d60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004d70: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
+00004d80: 6861 7320 4576 656e 7454 7265 6573 2065  has EventTrees e
+00004d90: 6163 6820 7769 7468 2061 2074 7265 6520  ach with a tree 
+00004da0: 6f66 2065 7665 6e74 732e 0a20 2020 2020  of events..     
+00004db0: 2020 2023 2055 7369 6e67 2043 6f6c 6c65     # Using Colle
+00004dc0: 6374 696f 6e20 616e 6420 4576 656e 7454  ction and EventT
+00004dd0: 7265 6573 2c20 796f 7520 6361 6e20 776f  rees, you can wo
+00004de0: 726b 2066 6c65 7869 626c 7920 7769 7468  rk flexibly with
+00004df0: 2065 7665 6e74 732e 0a20 2020 2020 2020   events..       
+00004e00: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
+00004e10: 2e31 5d20 4765 7420 6c65 6176 6573 206f  .1] Get leaves o
+00004e20: 6620 616c 6c20 7472 6565 732e 0a20 2020  f all trees..   
+00004e30: 2020 2020 206c 6561 7665 733a 2054 7570       leaves: Tup
+00004e40: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
+00004e50: 6574 5f6c 6561 7665 7328 2920 2023 2052  et_leaves()  # R
+00004e60: 6574 7572 6e73 2061 2074 7570 6c65 206f  eturns a tuple o
+00004e70: 6620 6c65 6176 6573 2065 7665 6e74 730a  f leaves events.
+00004e80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004e90: 2023 205b 332e 332e 325d 2047 6574 2072   # [3.3.2] Get r
+00004ea0: 6f6f 7473 2069 6473 206f 6620 616c 6c20  oots ids of all 
+00004eb0: 7472 6565 732e 0a20 2020 2020 2020 2072  trees..        r
+00004ec0: 6f6f 7473 3a20 4c69 7374 5b73 7472 5d20  oots: List[str] 
+00004ed0: 3d20 6574 632e 6765 745f 726f 6f74 735f  = etc.get_roots_
+00004ee0: 6964 7328 290a 2020 2020 2020 2020 2320  ids().        # 
+00004ef0: 5265 7475 726e 7320 7468 6520 6c69 7374  Returns the list
+00004f00: 206f 6620 726f 6f74 2049 6473 3a0a 2020   of root Ids:.  
+00004f10: 2020 2020 2020 2320 5b27 6465 6d6f 5f62        # ['demo_b
+00004f20: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00004f30: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+00004f40: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+00004f50: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+00004f60: 6433 3461 3631 3535 3135 3264 5f31 275d  d34a6155152d_1']
+00004f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004f80: 2020 2320 5b33 2e33 2e33 5d20 4669 6e64    # [3.3.3] Find
+00004f90: 2061 6e20 6576 656e 7420 696e 2061 6c6c   an event in all
+00004fa0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+00004fb0: 6669 6e64 5f65 7665 6e74 3a20 4f70 7469  find_event: Opti
+00004fc0: 6f6e 616c 5b64 6963 745d 203d 2065 7463  onal[dict] = etc
+00004fd0: 2e66 696e 6428 0a20 2020 2020 2020 2020  .find(.         
+00004fe0: 2020 206c 616d 6264 6120 6576 656e 743a     lambda event:
+00004ff0: 2022 5365 6e64 206d 6573 7361 6765 2220   "Send message" 
+00005000: 696e 2065 7665 6e74 5b22 6576 656e 7454  in event["eventT
+00005010: 7970 6522 5d29 0a20 2020 2020 2020 200a  ype"]).        .
+00005020: 2020 2020 2020 2020 2320 5b33 2e33 2e34          # [3.3.4
+00005030: 5d20 4669 6e64 2061 6c6c 2065 7665 6e74  ] Find all event
+00005040: 7320 696e 2061 6c6c 2074 7265 6573 2e20  s in all trees. 
+00005050: 5468 6572 6520 6973 2061 6c73 6f20 6974  There is also it
+00005060: 6572 6162 6c65 2076 6572 7369 6f6e 2027  erable version '
+00005070: 6669 6e64 616c 6c5f 6974 6572 272e 0a20  findall_iter'.. 
+00005080: 2020 2020 2020 2066 696e 645f 6576 656e         find_even
+00005090: 7473 3a20 4c69 7374 5b64 6963 745d 203d  ts: List[dict] =
+000050a0: 2065 7463 2e66 696e 6461 6c6c 286c 616d   etc.findall(lam
+000050b0: 6264 6120 6576 656e 743a 2065 7665 6e74  bda event: event
+000050c0: 5b22 7375 6363 6573 7366 756c 225d 2069  ["successful"] i
+000050d0: 7320 5472 7565 290a 2020 2020 2020 2020  s True).        
+000050e0: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+000050f0: 355d 2046 696e 6420 616e 2061 6e63 6573  5] Find an ances
+00005100: 746f 7220 6f66 2074 6865 2065 7665 6e74  tor of the event
+00005110: 2e0a 2020 2020 2020 2020 616e 6365 7374  ..        ancest
+00005120: 6f72 3a20 4f70 7469 6f6e 616c 5b64 6963  or: Optional[dic
+00005130: 745d 203d 2065 7463 2e66 696e 645f 616e  t] = etc.find_an
+00005140: 6365 7374 6f72 280a 2020 2020 2020 2020  cestor(.        
+00005150: 2020 2020 2264 656d 6f5f 626f 6f6b 5f31      "demo_book_1
+00005160: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00005170: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
+00005180: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00005190: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+000051a0: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
+000051b0: 2020 2020 2020 2020 6669 6c74 6572 3d6c          filter=l
+000051c0: 616d 6264 6120 6576 656e 743a 2022 526f  ambda event: "Ro
+000051d0: 6f74 4576 656e 7422 2069 6e20 6576 656e  otEvent" in even
+000051e0: 745b 2265 7665 6e74 4e61 6d65 225d 2c0a  t["eventName"],.
+000051f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00005200: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+00005210: 332e 365d 2047 6574 2063 6869 6c64 7265  3.6] Get childre
+00005220: 6e20 6f66 2074 6865 2065 7665 6e74 2e20  n of the event. 
+00005230: 5468 6572 6520 6973 2061 6c73 6f20 6974  There is also it
+00005240: 6572 6162 6c65 2076 6572 7369 6f6e 2027  erable version '
+00005250: 6765 745f 6368 696c 6472 656e 5f69 7465  get_children_ite
+00005260: 7227 2e0a 2020 2020 2020 2020 6368 696c  r'..        chil
+00005270: 6472 656e 3a20 5475 706c 655b 6469 6374  dren: Tuple[dict
+00005280: 5d20 3d20 6574 632e 6765 745f 6368 696c  ] = etc.get_chil
+00005290: 6472 656e 280a 2020 2020 2020 2020 2020  dren(.          
+000052a0: 2020 2264 656d 6f5f 626f 6f6b 5f31 3a74    "demo_book_1:t
+000052b0: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+000052c0: 3531 3335 3730 3535 3630 3837 3330 3030  5135705560873000
+000052d0: 3a64 3631 6539 3330 612d 3864 3030 2d31  :d61e930a-8d00-1
+000052e0: 3165 642d 6161 3161 2d64 3334 6136 3135  1ed-aa1a-d34a615
+000052f0: 3531 3532 645f 3122 0a20 2020 2020 2020  5152d_1".       
+00005300: 2029 0a20 2020 2020 2020 200a 2020 2020   ).        .    
+00005310: 2020 2020 2320 5b33 2e33 2e37 5d20 4765      # [3.3.7] Ge
+00005320: 7420 7375 6274 7265 6520 666f 7220 7370  t subtree for sp
+00005330: 6563 6966 6965 6420 6576 656e 742e 0a20  ecified event.. 
+00005340: 2020 2020 2020 2073 7562 7472 6565 3a20         subtree: 
+00005350: 4576 656e 7454 7265 6520 3d20 6574 632e  EventTree = etc.
+00005360: 6765 745f 7375 6274 7265 6528 0a20 2020  get_subtree(.   
+00005370: 2020 2020 2020 2020 2022 6465 6d6f 5f62           "demo_b
+00005380: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00005390: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+000053a0: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+000053b0: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+000053c0: 6433 3461 3631 3535 3135 3264 5f31 220a  d34a6155152d_1".
+000053d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000053e0: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+000053f0: 332e 385d 2047 6574 2066 756c 6c20 7061  3.8] Get full pa
+00005400: 7468 2074 6f20 7468 6520 6576 656e 742e  th to the event.
+00005410: 0a20 2020 2020 2020 2023 204c 6f6f 6b73  .        # Looks
+00005420: 206c 696b 6520 5b61 6e63 6573 746f 725f   like [ancestor_
+00005430: 726f 6f74 2c20 616e 6365 7374 6f72 5f6c  root, ancestor_l
+00005440: 6576 656c 312c 2061 6e63 6573 746f 725f  evel1, ancestor_
+00005450: 6c65 7665 6c32 2c20 6576 656e 745d 0a20  level2, event]. 
+00005460: 2020 2020 2020 2065 7665 6e74 5f70 6174         event_pat
+00005470: 683a 204c 6973 745b 6469 6374 5d20 3d20  h: List[dict] = 
+00005480: 6574 632e 6765 745f 6675 6c6c 5f70 6174  etc.get_full_pat
+00005490: 6828 0a20 2020 2020 2020 2020 2020 2022  h(.            "
+000054a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+000054b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+000054c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+000054d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+000054e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+000054f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
+00005500: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005510: 2023 205b 332e 332e 395d 2047 6574 2070   # [3.3.9] Get p
+00005520: 6172 656e 7420 6f66 2074 6865 2065 7665  arent of the eve
+00005530: 6e74 2e0a 2020 2020 2020 2020 7061 7265  nt..        pare
+00005540: 6e74 203d 2065 7463 2e67 6574 5f70 6172  nt = etc.get_par
+00005550: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
+00005560: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00005570: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00005580: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00005590: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+000055a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000055b0: 3135 3264 5f31 220a 2020 2020 2020 2020  152d_1".        
+000055c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000055d0: 2020 2023 205b 332e 332e 3130 5d20 4170     # [3.3.10] Ap
+000055e0: 7065 6e64 206e 6577 2065 7665 6e74 2074  pend new event t
+000055f0: 6f20 7468 6520 636f 6c6c 6563 7469 6f6e  o the collection
+00005600: 2e0a 2020 2020 2020 2020 6574 632e 6170  ..        etc.ap
+00005610: 7065 6e64 5f65 7665 6e74 280a 2020 2020  pend_event(.    
+00005620: 2020 2020 2020 2020 6576 656e 743d 7b0a          event={.
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2265 7665 6e74 4964 223a 2022 6132 3066  "eventId": "a20f
+00005650: 3565 6634 2d63 3366 652d 6262 3130 2d61  5ef4-c3fe-bb10-a
+00005660: 3239 632d 6464 3364 3738 3439 3039 6562  29c-dd3d784909eb
+00005670: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005680: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
+00005690: 6422 3a20 2238 6532 3532 3466 612d 6366  d": "8e2524fa-cf
+000056a0: 3539 2d31 3165 622d 6133 6637 2d30 3934  59-11eb-a3f7-094
+000056b0: 6639 3034 6333 6136 3222 2c0a 2020 2020  f904c3a62",.    
+000056c0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000056d0: 6e74 4e61 6d65 223a 2022 5374 7562 4576  ntName": "StubEv
+000056e0: 656e 7422 2c0a 2020 2020 2020 2020 2020  ent",.          
+000056f0: 2020 7d0a 2020 2020 2020 2020 290a 2020    }.        ).  
+00005700: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005710: 205b 332e 332e 3131 5d20 5368 6f77 2074   [3.3.11] Show t
+00005720: 6865 2065 6e74 6972 6520 636f 6c6c 6563  he entire collec
+00005730: 7469 6f6e 2e0a 2020 2020 2020 2020 6574  tion..        et
+00005740: 632e 7368 6f77 2829 0a20 2020 2020 2020  c.show().       
+00005750: 2023 2049 7427 6c6c 2070 7269 6e74 2074   # It'll print t
+00005760: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2020  he following:.  
+00005770: 2020 2020 2020 2320 5365 7420 6f66 2061        # Set of a
+00005780: 7574 6f2d 6765 6e65 7261 7465 6420 6576  uto-generated ev
+00005790: 656e 7473 2066 6f72 2064 7320 6c69 6220  ents for ds lib 
+000057a0: 7465 7374 696e 670a 2020 2020 2020 2020  testing.        
+000057b0: 2320 e294 9ce2 9480 e294 8020 506c 6169  # ......... Plai
+000057c0: 6e20 6576 656e 7420 310a 2020 2020 2020  n event 1.      
+000057d0: 2020 2320 e294 94e2 9480 e294 8020 506c    # ......... Pl
+000057e0: 6169 6e20 6576 656e 7420 320a 2020 2020  ain event 2.    
+000057f0: 2020 2020 0a20 2020 2020 2020 2023 2041      .        # A
+00005800: 7320 796f 7520 6361 6e20 7365 652c 206e  s you can see, n
+00005810: 6f74 6869 6e67 2077 6173 2063 6861 6e67  othing was chang
+00005820: 6564 2c20 6275 7420 7765 2061 6464 6564  ed, but we added
+00005830: 2074 6865 206e 6577 2065 7665 6e74 210a   the new event!.
+00005840: 2020 2020 2020 2020 2320 6c65 7427 7320          # let's 
+00005850: 6c6f 6f6b 2061 7420 7468 6520 7375 6d6d  look at the summ
+00005860: 6172 792e 0a20 2020 2020 2020 200a 2020  ary..        .  
+00005870: 2020 2020 2020 7072 696e 7428 6574 632e        print(etc.
+00005880: 7375 6d6d 6172 7928 2929 2020 2320 7468  summary())  # th
+00005890: 6520 7361 6d65 2061 7320 6a75 7374 2070  e same as just p
+000058a0: 7269 6e74 2865 7463 290a 2020 2020 2020  rint(etc).      
+000058b0: 2020 2320 4576 656e 7454 7265 6543 6f6c    # EventTreeCol
+000058c0: 6c65 6374 696f 6e28 7472 6565 733d 312c  lection(trees=1,
+000058d0: 2065 7665 6e74 733d 355b 7472 6565 733d   events=5[trees=
+000058e0: 332c 2064 6574 6163 6865 643d 325d 290a  3, detached=2]).
+000058f0: 2020 2020 2020 2020 2320 596f 7520 6361          # You ca
+00005900: 6e20 7365 6520 7468 6174 2069 7420 7761  n see that it wa
+00005910: 7320 6164 6465 6420 746f 2064 6574 6163  s added to detac
+00005920: 6865 642e 2054 6861 7427 7320 7768 7920  hed. That's why 
+00005930: 796f 7520 646f 6e27 7420 7365 6520 7468  you don't see th
+00005940: 6520 6576 656e 740a 2020 2020 2020 2020  e event.        
+00005950: 2320 7669 6120 6073 686f 7728 2960 2e20  # via `show()`. 
+00005960: 6073 686f 7728 2960 2070 7269 6e74 7320  `show()` prints 
+00005970: 6f6e 6c79 2054 7265 6573 210a 2020 2020  only Trees!.    
+00005980: 2020 2020 2320 5573 6520 6065 7463 2e67      # Use `etc.g
+00005990: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+000059a0: 6565 7328 2960 2074 6f20 636f 6e76 6572  ees()` to conver
+000059b0: 7420 6465 7461 6368 6564 2065 7665 6e74  t detached event
+000059c0: 7320 746f 2074 7265 6573 2e0a 2020 2020  s to trees..    
+000059d0: 2020 2020 2320 4d6f 7265 2069 6e66 6f72      # More infor
+000059e0: 6d61 7469 6f6e 2062 656c 6f77 2069 6e20  mation below in 
+000059f0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+00005a00: 6720 7365 6374 696f 6e2e 0a20 2020 2020  g section..     
+00005a10: 2020 200a 2020 2020 2020 2020 2320 2d2d     .        # --
+00005a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00005a30: 2020 2020 2023 205b 332e 345d 2057 6f72       # [3.4] Wor
+00005a40: 6b69 6e67 2077 6974 6820 7468 6520 4576  king with the Ev
+00005a50: 656e 7454 7265 652e 0a20 2020 2020 2020  entTree..       
+00005a60: 2023 2045 7665 6e74 5472 6565 2068 6173   # EventTree has
+00005a70: 2074 6865 2073 616d 6520 6d65 7468 6f64   the same method
+00005a80: 7320 6173 2045 7665 6e74 5472 6565 436f  s as EventTreeCo
+00005a90: 6c6c 6563 7469 6f6e 2c20 6275 7420 6f6e  llection, but on
+00005aa0: 6c79 2066 6f72 2069 7473 206f 776e 2074  ly for its own t
+00005ab0: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00005ac0: 2020 2020 2020 2320 5b33 2e34 2e31 5d20        # [3.4.1] 
+00005ad0: 4765 7420 6120 636f 6c6c 6563 7469 6f6e  Get a collection
+00005ae0: 206f 6620 7472 6565 732e 0a20 2020 2020   of trees..     
+00005af0: 2020 2074 7265 6573 3a20 4c69 7374 5b45     trees: List[E
+00005b00: 7665 6e74 5472 6565 5d20 3d20 6574 632e  ventTree] = etc.
+00005b10: 6765 745f 7472 6565 7328 290a 2020 2020  get_trees().    
+00005b20: 2020 2020 7472 6565 3a20 4576 656e 7454      tree: EventT
+00005b30: 7265 6520 3d20 7472 6565 735b 305d 0a20  ree = trees[0]. 
+00005b40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005b50: 2320 4275 7420 4576 656e 7454 7265 6520  # But EventTree 
+00005b60: 7072 6f76 6964 6573 2061 2077 6f72 6b20  provides a work 
+00005b70: 7769 7468 2074 6865 2074 7265 652c 2062  with the tree, b
+00005b80: 7574 2064 6f65 7320 6e6f 7420 6d6f 6469  ut does not modi
+00005b90: 6679 2069 742e 0a20 2020 2020 2020 2023  fy it..        #
+00005ba0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00005bb0: 6d6f 6469 6679 2074 6865 2074 7265 652c  modify the tree,
+00005bc0: 2075 7365 2045 7665 6e74 5472 6565 436f   use EventTreeCo
+00005bd0: 6c6c 6563 7469 6f6e 732e 0a20 2020 2020  llections..     
+00005be0: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00005bf0: 2e35 5d20 576f 726b 696e 6720 7769 7468  .5] Working with
+00005c00: 2050 6172 656e 746c 6573 7354 7265 652e   ParentlessTree.
+00005c10: 0a20 2020 2020 2020 2023 2050 6172 656e  .        # Paren
+00005c20: 746c 6573 7354 7265 6520 6973 2061 6e20  tlessTree is an 
+00005c30: 4576 656e 7454 7265 6520 7468 6174 2068  EventTree that h
+00005c40: 6173 2064 6574 6163 6865 6420 6576 656e  as detached even
+00005c50: 7473 2077 6974 6820 7374 7562 732e 0a20  ts with stubs.. 
+00005c60: 2020 2020 2020 2070 6172 656e 746c 6573         parentles
+00005c70: 735f 7472 6565 733a 204c 6973 745b 4576  s_trees: List[Ev
+00005c80: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
+00005c90: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00005ca0: 6565 7328 290a 2020 2020 2020 2020 7072  ees().        pr
+00005cb0: 696e 7428 2270 6172 656e 746c 6573 735f  int("parentless_
+00005cc0: 7472 6565 7320 636f 6e74 6169 6e73 3a22  trees contains:"
+00005cd0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00005ce0: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+00005cf0: 290a 2020 2020 2020 2020 2320 5b45 7665  ).        # [Eve
+00005d00: 6e74 5472 6565 286e 616d 653d 273c 4272  ntTree(name='<Br
+00005d10: 6f6b 656e 4576 656e 743e 272c 2072 6f6f  okenEvent>', roo
+00005d20: 745f 6964 3d27 6e6f 745f 6578 6973 7473  t_id='not_exists
+00005d30: 5f69 6e5f 7468 655f 6576 656e 7473 5f73  _in_the_events_s
+00005d40: 7472 6561 6d27 2c20 6576 656e 7473 3d32  tream', events=2
+00005d50: 292c 0a20 2020 2020 2020 2023 2020 4576  ),.        #  Ev
+00005d60: 656e 7454 7265 6528 6e61 6d65 3d27 3c42  entTree(name='<B
+00005d70: 726f 6b65 6e45 7665 6e74 3e27 2c20 726f  rokenEvent>', ro
+00005d80: 6f74 5f69 643d 2738 6532 3532 3466 612d  ot_id='8e2524fa-
+00005d90: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
+00005da0: 3934 6639 3034 6333 6136 3227 2c20 6576  94f904c3a62', ev
+00005db0: 656e 7473 3d32 295d 0a20 2020 2020 2020  ents=2)].       
+00005dc0: 200a 2020 2020 2020 2020 7072 696e 7428   .        print(
+00005dd0: 225c 6e22 2022 6574 6320 6166 7465 7220  "\n" "etc after 
+00005de0: 6067 6574 5f70 6172 656e 746c 6573 735f  `get_parentless_
+00005df0: 7472 6565 7360 3a22 290a 2020 2020 2020  trees`:").      
+00005e00: 2020 7072 696e 7428 6574 632e 7375 6d6d    print(etc.summ
+00005e10: 6172 7928 2929 0a20 2020 2020 2020 2023  ary()).        #
+00005e20: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00005e30: 7469 6f6e 2874 7265 6573 3d33 5b72 6567  tion(trees=3[reg
+00005e40: 756c 6172 3d31 2c20 7061 7265 6e74 6c65  ular=1, parentle
+00005e50: 7373 3d32 5d2c 2065 7665 6e74 733d 375b  ss=2], events=7[
+00005e60: 7472 6565 733d 372c 2064 6574 6163 6865  trees=7, detache
+00005e70: 643d 305d 2927 0a20 2020 2020 2020 2065  d=0])'.        e
+00005e80: 7463 2e73 686f 7728 290a 2020 2020 2020  tc.show().      
+00005e90: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
+00005ea0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
+00005eb0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
+00005ec0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
+00005ed0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
+00005ee0: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
+00005ef0: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
+00005f00: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
+00005f10: 2320 3c42 726f 6b65 6e45 7665 6e74 3e0a  # <BrokenEvent>.
+00005f20: 2020 2020 2020 2020 2320 e294 94e2 9480          # ......
+00005f30: e294 8020 4661 6b65 2065 7665 6e74 0a20  ... Fake event. 
+00005f40: 2020 2020 2020 2023 203c 4272 6f6b 656e         # <Broken
+00005f50: 4576 656e 743e 0a20 2020 2020 2020 2023  Event>.        #
+00005f60: 20e2 9494 e294 80e2 9480 2053 7475 6245   ......... StubE
+00005f70: 7665 6e74 2020 2020 3c2d 2d2d 2074 6865  vent    <--- the
+00005f80: 2065 7665 6e74 2074 6861 7420 7761 7320   event that was 
+00005f90: 6164 6465 6420 6162 6f76 650a 2020 2020  added above.    
+00005fa0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00005fb0: 332e 365d 2057 6f72 6b69 6e67 2077 6974  3.6] Working wit
+00005fc0: 6820 5061 7265 6e74 4576 656e 7454 7265  h ParentEventTre
+00005fd0: 6543 6f6c 6c65 6374 696f 6e2e 0a20 2020  eCollection..   
+00005fe0: 2020 2020 2023 2050 6172 656e 7445 7665       # ParentEve
+00005ff0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00006000: 2069 7320 6120 7472 6565 2063 6f6c 6c65   is a tree colle
+00006010: 6374 696f 6e20 6c69 6b65 2045 7665 6e74  ction like Event
+00006020: 5472 6565 436f 6c6c 6563 7469 6f6e 2c0a  TreeCollection,.
+00006030: 2020 2020 2020 2020 2320 6275 7420 6974          # but it
+00006040: 2068 6173 206f 6e6c 7920 6576 656e 7473   has only events
+00006050: 2074 6861 7420 6861 7665 2072 6566 6572   that have refer
+00006060: 656e 6365 732e 0a20 2020 2020 2020 2064  ences..        d
+00006070: 6174 615f 736f 7572 6365 3a20 4944 6174  ata_source: IDat
+00006080: 6153 6f75 7263 6520 2023 2059 6f75 2073  aSource  # You s
+00006090: 686f 756c 6420 696e 6974 2044 6174 6153  hould init DataS
+000060a0: 6f75 7263 6520 6f62 6a65 6374 2e20 452e  ource object. E.
+000060b0: 672e 2066 726f 6d20 4c77 4450 206d 6f64  g. from LwDP mod
+000060c0: 756c 652e 0a20 2020 2020 2020 2064 6174  ule..        dat
+000060d0: 615f 736f 7572 6365 203d 2044 756d 6d79  a_source = Dummy
+000060e0: 4461 7461 536f 7572 6365 2829 2020 2320  DataSource()  # 
+000060f0: 4e6f 7465 2120 5765 2075 7365 2066 616b  Note! We use fak
+00006100: 6520 4453 2068 6572 652e 0a20 2020 2020  e DS here..     
+00006110: 2020 2023 2045 5443 4472 6976 6572 2068     # ETCDriver h
+00006120: 6572 6520 6973 2061 2073 7475 622c 2061  ere is a stub, a
+00006130: 6374 7561 6c6c 7920 7468 6520 6c69 6220  ctually the lib 
+00006140: 646f 6573 6e27 7420 6861 7665 2073 7563  doesn't have suc
+00006150: 6820 6120 636c 6173 732e 0a20 2020 2020  h a class..     
+00006160: 2020 2023 2059 6f75 2063 616e 2074 616b     # You can tak
+00006170: 6520 6974 2069 6e20 4c77 4450 206d 6f64  e it in LwDP mod
+00006180: 756c 6520 6f72 2063 7265 6174 6520 796f  ule or create yo
+00006190: 7572 7365 6c66 2063 6c61 7373 2069 6620  urself class if 
+000061a0: 796f 7520 6861 7665 2073 6f6d 6520 7370  you have some sp
+000061b0: 6563 6961 6c20 6576 656e 7473 2073 7472  ecial events str
+000061c0: 7563 7475 7265 2e0a 2020 2020 2020 2020  ucture..        
+000061d0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+000061e0: 7276 6963 6573 2e64 6174 615f 736f 7572  rvices.data_sour
+000061f0: 6365 2e6c 7764 702e 6576 656e 745f 7472  ce.lwdp.event_tr
+00006200: 6565 2069 6d70 6f72 740a 2020 2020 2020  ee import.      
+00006210: 2020 0a20 2020 2020 2020 2048 7474 7045    .        HttpE
+00006220: 5443 4472 6976 6572 2061 7320 4554 4344  TCDriver as ETCD
+00006230: 7269 7665 720a 2020 2020 2020 2020 0a20  river.        . 
+00006240: 2020 2020 2020 2064 7269 7665 7220 3d20         driver = 
+00006250: 4554 4344 7269 7665 7228 6461 7461 5f73  ETCDriver(data_s
+00006260: 6f75 7263 653d 6461 7461 5f73 6f75 7263  ource=data_sourc
+00006270: 6529 0a20 2020 2020 2020 2070 6574 6320  e).        petc 
+00006280: 3d20 5061 7265 6e74 4576 656e 7454 7265  = ParentEventTre
+00006290: 6543 6f6c 6c65 6374 696f 6e28 6472 6976  eCollection(driv
+000062a0: 6572 290a 2020 2020 2020 2020 7065 7463  er).        petc
+000062b0: 2e62 7569 6c64 2865 7665 6e74 7329 0a20  .build(events). 
+000062c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000062d0: 7065 7463 2e73 686f 7728 290a 2020 2020  petc.show().    
+000062e0: 2020 2020 7065 7463 2e73 756d 6d61 7279      petc.summary
+000062f0: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
+00006300: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00006310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006320: 2323 2323 2323 2323 2323 0a20 2020 2020  ##########.     
+00006330: 2020 2023 205b 345d 2046 6965 6c64 2052     # [4] Field R
+00006340: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
+00006350: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00006360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006370: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00006380: 2320 506c 6561 7365 2072 6561 6420 6046  # Please read `F
+00006390: 6965 6c64 2052 6573 6f6c 7665 7273 6020  ield Resolvers` 
+000063a0: 626c 6f63 6b20 696e 2072 6561 646d 6520  block in readme 
+000063b0: 6669 7273 742e 0a20 2020 2020 2020 200a  first..        .
+000063c0: 2020 2020 2020 2020 2320 5b34 2e31 5d20          # [4.1] 
+000063d0: 5573 6167 6520 6578 616d 706c 6520 6672  Usage example fr
+000063e0: 6f6d 2063 6c69 656e 7420 636f 6465 0a20  om client code. 
+000063f0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+00006400: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
+00006410: 7461 5f73 6f75 7263 6520 696d 706f 7274  ta_source import
+00006420: 2028 0a20 2020 2020 2020 2020 2020 206c   (.            l
+00006430: 7764 702c 0a20 2020 2020 2020 2029 2020  wdp,.        )  
+00006440: 2320 6c77 6470 2064 6174 615f 736f 7572  # lwdp data_sour
+00006450: 6365 2069 6e69 7469 616c 697a 6520 7468  ce initialize th
+00006460: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00006470: 636f 6e66 6967 2064 7572 696e 6720 696d  config during im
+00006480: 706f 7274 2e0a 2020 2020 2020 2020 6672  port..        fr
+00006490: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+000064a0: 6963 6573 2e63 6f6e 6669 6720 696d 706f  ices.config impo
+000064b0: 7274 206f 7074 696f 6e73 2061 7320 6f5f  rt options as o_
+000064c0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+000064d0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+000064e0: 6461 7461 5f73 6f75 7263 652e 6c77 6470  data_source.lwdp
+000064f0: 2e73 7475 625f 6275 696c 6465 7220 696d  .stub_builder im
+00006500: 706f 7274 0a20 2020 2020 2020 200a 2020  port.        .  
+00006510: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
+00006520: 6765 5f73 7475 625f 6275 696c 6465 720a  ge_stub_builder.
+00006530: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006540: 2066 616b 655f 6461 7461 203d 205b 0a20   fake_data = [. 
+00006550: 2020 2020 2020 2020 2020 2068 7474 705f             http_
+00006560: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
+00006570: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
+00006580: 7361 6765 4964 223a 2022 6122 2c20 226d  sageId": "a", "m
+00006590: 6573 7361 6765 5479 7065 223a 2022 526f  essageType": "Ro
+000065a0: 6f74 227d 292c 0a20 2020 2020 2020 2020  ot"}),.         
+000065b0: 2020 2068 7474 705f 6d65 7373 6167 655f     http_message_
+000065c0: 7374 7562 5f62 7569 6c64 6572 2e62 7569  stub_builder.bui
+000065d0: 6c64 287b 226d 6573 7361 6765 4964 223a  ld({"messageId":
+000065e0: 2022 6222 2c20 226d 6573 7361 6765 5479   "b", "messageTy
+000065f0: 7065 223a 2022 4e65 7722 7d29 2c0a 2020  pe": "New"}),.  
+00006600: 2020 2020 2020 2020 2020 6874 7470 5f6d            http_m
+00006610: 6573 7361 6765 5f73 7475 625f 6275 696c  essage_stub_buil
+00006620: 6465 722e 6275 696c 6428 7b22 6d65 7373  der.build({"mess
+00006630: 6167 6549 6422 3a20 2263 222c 2022 6d65  ageId": "c", "me
+00006640: 7373 6167 6554 7970 6522 3a20 2241 6d65  ssageType": "Ame
+00006650: 6e64 227d 292c 0a20 2020 2020 2020 2020  nd"}),.         
+00006660: 2020 2068 7474 705f 6d65 7373 6167 655f     http_message_
+00006670: 7374 7562 5f62 7569 6c64 6572 2e62 7569  stub_builder.bui
+00006680: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00006690: 2020 2020 7b22 6d65 7373 6167 6549 6422      {"messageId"
+000066a0: 3a20 2264 222c 2022 6d65 7373 6167 6554  : "d", "messageT
+000066b0: 7970 6522 3a20 2243 616e 6365 6c22 7d29  ype": "Cancel"})
+000066c0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+000066d0: 2020 2020 6661 6b65 5f64 6174 615f 6f62      fake_data_ob
+000066e0: 6a20 3d20 4461 7461 2866 616b 655f 6461  j = Data(fake_da
+000066f0: 7461 290a 2020 2020 2020 2020 0a20 2020  ta).        .   
+00006700: 2020 2020 2066 6f72 206d 2069 6e20 6661       for m in fa
+00006710: 6b65 5f64 6174 615f 6f62 6a3a 0a20 2020  ke_data_obj:.   
+00006720: 2020 2020 2020 2020 206f 5f2e 6d66 722e           o_.mfr.
+00006730: 6578 7061 6e64 5f6d 6573 7361 6765 286d  expand_message(m
+00006740: 2920 2023 206d 6672 202d 2073 7461 6e64  )  # mfr - stand
+00006750: 7320 666f 7220 4d65 7373 6167 6546 6965  s for MessageFie
+00006760: 6c64 5265 736f 6c76 6572 0a20 2020 2020  ldResolver.     
+00006770: 2020 2023 206f 720a 2020 2020 2020 2020     # or.        
+00006780: 666f 7220 6d20 696e 2066 616b 655f 6461  for m in fake_da
+00006790: 7461 5f6f 626a 2e6d 6170 286f 5f2e 6d66  ta_obj.map(o_.mf
+000067a0: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
+000067b0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+000067c0: 6173 730a 2020 2020 2020 2020 0a20 2020  ass.        .   
+000067d0: 2020 2020 2023 205b 342e 325d 204c 6962       # [4.2] Lib
+000067e0: 7261 7269 6573 2075 7361 6765 2e0a 2020  raries usage..  
+000067f0: 2020 2020 2020 2320 446f 6e27 7420 696d        # Don't im
+00006800: 706f 7274 2065 7861 6374 2072 6573 6f6c  port exact resol
+00006810: 7665 7273 2069 6d70 6c65 6d65 6e74 6174  vers implementat
+00006820: 696f 6e20 696e 2079 6f75 7220 636f 6465  ion in your code
+00006830: 2c20 706c 6561 7365 2e0a 2020 2020 2020  , please..      
+00006840: 2020 2320 416c 6c6f 7720 796f 7572 2063    # Allow your c
+00006850: 6c69 656e 7420 746f 2064 6f20 6974 2069  lient to do it i
+00006860: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
+00006870: 2320 4a75 7374 2069 6d70 6f72 7420 606f  # Just import `o
+00006880: 7074 696f 6e73 6020 6672 6f6d 2060 7468  ptions` from `th
+00006890: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+000068a0: 636f 6e66 6967 6020 616e 6420 7573 6520  config` and use 
+000068b0: 6974 2e0a 2020 2020 2020 2020 6672 6f6d  it..        from
+000068c0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+000068d0: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
+000068e0: 206f 7074 696f 6e73 2061 7320 6f5f 0a20   options as o_. 
+000068f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006900: 666f 7220 6d20 696e 2066 616b 655f 6461  for m in fake_da
+00006910: 7461 5f6f 626a 3a0a 2020 2020 2020 2020  ta_obj:.        
+00006920: 2020 2020 6f5f 2e6d 6672 2e65 7870 616e      o_.mfr.expan
+00006930: 645f 6d65 7373 6167 6528 6d29 0a20 2020  d_message(m).   
+00006940: 2020 2020 2023 206f 720a 2020 2020 2020       # or.      
+00006950: 2020 666f 7220 6d20 696e 2066 616b 655f    for m in fake_
+00006960: 6461 7461 5f6f 626a 2e6d 6170 286f 5f2e  data_obj.map(o_.
+00006970: 6d66 722e 6578 7061 6e64 5f6d 6573 7361  mfr.expand_messa
+00006980: 6765 293a 0a20 2020 2020 2020 2020 2020  ge):.           
+00006990: 2070 6173 730a 2020 2020 2020 2020 0a20   pass.        . 
+000069a0: 2020 2020 2020 2023 204d 6f72 6520 7465         # More te
+000069b0: 6368 2064 6574 6169 6c73 3a0a 2020 2020  ch details:.    
+000069c0: 2020 2020 2320 2020 496e 2074 6869 7320      #   In this 
+000069d0: 6361 7365 2c20 7468 6572 6520 6973 206e  case, there is n
+000069e0: 6f20 6c69 6e65 2060 6672 6f6d 2074 6832  o line `from th2
+000069f0: 5f64 6174 615f 7365 7276 6963 6573 2e64  _data_services.d
+00006a00: 6174 615f 736f 7572 6365 2069 6d70 6f72  ata_source impor
+00006a10: 7420 6c77 6470 2060 0a20 2020 2020 2020  t lwdp `.       
+00006a20: 2023 2020 2062 6563 6175 7365 2077 6520   #   because we 
+00006a30: 7368 6f75 6c64 206e 6f74 2063 686f 6f73  should not choos
+00006a40: 6520 666f 7220 7468 6520 7573 6572 2077  e for the user w
+00006a50: 6869 6368 2061 2064 6174 6120 736f 7572  hich a data sour
+00006a60: 6365 2074 6f20 7573 652e 0a20 2020 2020  ce to use..     
+00006a70: 2020 2023 2020 2057 6520 646f 206e 6f74     #   We do not
+00006a80: 206b 6e6f 7720 7768 6174 2068 6520 7769   know what he wi
+00006a90: 6c6c 2063 686f 6f73 652c 2074 6865 7265  ll choose, there
+00006aa0: 666f 7265 2c20 7765 206d 7573 7420 7369  fore, we must si
+00006ab0: 6d70 6c79 2061 6363 6573 730a 2020 2020  mply access.    
+00006ac0: 2020 2020 2320 2020 7468 6520 696e 7465      #   the inte
+00006ad0: 7266 6163 652c 2077 6869 6368 2077 696c  rface, which wil
+00006ae0: 6c20 6265 2069 6e69 7469 616c 697a 6564  l be initialized
+00006af0: 2062 7920 7468 6520 7573 6572 2e0a 2020   by the user..  
+00006b00: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00006b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b30: 2323 2323 230a 2020 2020 2020 2020 2320  #####.        # 
+00006b40: 5b35 5d20 5573 696e 6720 7574 696c 6974  [5] Using utilit
+00006b50: 7920 6675 6e63 7469 6f6e 732e 0a20 2020  y functions..   
+00006b60: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00006b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b80: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00006b90: 2020 2020 6672 6f6d 2074 6832 5f64 6174      from th2_dat
+00006ba0: 615f 7365 7276 6963 6573 2e75 7469 6c73  a_services.utils
+00006bb0: 2e65 7665 6e74 5f75 7469 6c73 2e66 7265  .event_utils.fre
+00006bc0: 7175 656e 6369 6573 2069 6d70 6f72 740a  quencies import.
+00006bd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006be0: 2067 6574 5f63 6174 6567 6f72 795f 6672   get_category_fr
+00006bf0: 6571 7565 6e63 6965 7332 0a20 2020 2020  equencies2.     
+00006c00: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+00006c10: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
+00006c20: 6576 656e 745f 7574 696c 732e 746f 7461  event_utils.tota
+00006c30: 6c73 2069 6d70 6f72 7420 6765 745f 6361  ls import get_ca
+00006c40: 7465 676f 7279 5f74 6f74 616c 7332 0a20  tegory_totals2. 
+00006c50: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+00006c60: 6461 7461 5f73 6572 7669 6365 732e 7574  data_services.ut
+00006c70: 696c 732e 6361 7465 676f 7279 2069 6d70  ils.category imp
+00006c80: 6f72 7420 4361 7465 676f 7279 0a20 2020  ort Category.   
+00006c90: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+00006ca0: 7461 5f73 6572 7669 6365 732e 7574 696c  ta_services.util
+00006cb0: 732e 6576 656e 745f 7574 696c 732e 6576  s.event_utils.ev
+00006cc0: 656e 745f 7574 696c 7320 696d 706f 7274  ent_utils import
+00006cd0: 2069 735f 736f 7274 6564 0a20 2020 2020   is_sorted.     
+00006ce0: 2020 200a 2020 2020 2020 2020 2320 5b35     .        # [5
+00006cf0: 2e31 5d20 4765 7420 7468 6520 7175 616e  .1] Get the quan
+00006d00: 7469 7469 6573 206f 6620 6576 656e 7473  tities of events
+00006d10: 2066 6f72 2064 6966 6665 7265 6e74 2063   for different c
+00006d20: 6174 6567 6f72 6965 732e 0a20 2020 2020  ategories..     
+00006d30: 2020 206d 6574 7269 6373 203d 205b 0a20     metrics = [. 
+00006d40: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
+00006d50: 6f72 7928 2264 6174 6522 2c20 6c61 6d62  ory("date", lamb
+00006d60: 6461 206d 3a20 5468 3254 696d 6573 7461  da m: Th2Timesta
+00006d70: 6d70 436f 6e76 6572 7465 722e 746f 5f64  mpConverter.to_d
+00006d80: 6174 6574 696d 6528 0a20 2020 2020 2020  atetime(.       
+00006d90: 2020 2020 2020 2020 206d 5b22 7374 6172           m["star
+00006da0: 7454 696d 6573 7461 6d70 225d 292e 6461  tTimestamp"]).da
+00006db0: 7465 2829 292c 0a20 2020 2020 2020 2020  te()),.         
+00006dc0: 2020 2043 6174 6567 6f72 7928 2273 7461     Category("sta
+00006dd0: 7475 7322 2c20 6c61 6d62 6461 206d 3a20  tus", lambda m: 
+00006de0: 6d5b 2273 7563 6365 7373 6675 6c22 5d29  m["successful"])
+00006df0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00006e00: 2020 2020 6361 7465 676f 7279 5f74 6f74      category_tot
+00006e10: 616c 7320 3d20 6765 745f 6361 7465 676f  als = get_catego
+00006e20: 7279 5f74 6f74 616c 7332 2865 7665 6e74  ry_totals2(event
+00006e30: 732c 206d 6574 7269 6373 290a 2020 2020  s, metrics).    
+00006e40: 2020 2020 7072 696e 7428 6361 7465 676f      print(catego
+00006e50: 7279 5f74 6f74 616c 7329 0a20 2020 2020  ry_totals).     
+00006e60: 2020 2022 2222 0a20 2020 2020 2020 202b     """.        +
+00006e70: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006e80: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00006e90: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
+00006ea0: 2020 2020 7c20 2020 2020 2020 207c 2064      |        | d
+00006eb0: 6174 6520 2020 2020 2020 7c20 7374 6174  ate       | stat
+00006ec0: 7573 2020 207c 2020 2063 6f75 6e74 207c  us   |   count |
+00006ed0: 0a20 2020 2020 2020 202b 3d3d 3d3d 3d3d  .        +======
+00006ee0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ==+============+
+00006ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  ==========+=====
+00006f00: 3d3d 3d3d 2b0a 2020 2020 2020 2020 7c20  ====+.        | 
+00006f10: 2020 2020 2020 207c 2032 3032 332d 3031         | 2023-01
+00006f20: 2d30 3520 7c20 5472 7565 2020 2020 207c  -05 | True     |
+00006f30: 2020 2020 2020 2033 207c 0a20 2020 2020         3 |.     
+00006f40: 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d     +--------+---
+00006f50: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00006f60: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a  ----+---------+.
+00006f70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006f80: 207c 2032 3032 332d 3031 2d30 3520 7c20   | 2023-01-05 | 
+00006f90: 4661 6c73 6520 2020 207c 2020 2020 2020  False    |      
+00006fa0: 2031 207c 0a20 2020 2020 2020 202b 2d2d   1 |.        +--
+00006fb0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00006fc0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  ---+----------+-
+00006fd0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00006fe0: 2020 7c20 636f 756e 7420 207c 2020 2020    | count  |    
+00006ff0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00007000: 2020 207c 2020 2020 2020 2032 207c 0a20     |       2 |. 
+00007010: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
+00007020: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
+00007030: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00007040: 2d2d 2b0a 2020 2020 2020 2020 7c20 746f  --+.        | to
+00007050: 7461 6c73 207c 2020 2020 2020 2020 2020  tals |          
+00007060: 2020 7c20 312f 3120 2020 2020 207c 2020    | 1/1      |  
+00007070: 2020 2020 2034 207c 0a20 2020 2020 2020       4 |.       
+00007080: 202b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d   +--------+-----
+00007090: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000070a0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020  --+---------+.  
+000070b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000070c0: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
+000070d0: 325d 2047 6574 2074 6865 206e 756d 6265  2] Get the numbe
+000070e0: 7220 6f66 2065 7665 6e74 7320 7769 7468  r of events with
+000070f0: 2073 7461 7475 7320 7375 6363 6573 7366   status successf
+00007100: 756c 2e0a 2020 2020 2020 2020 6361 7465  ul..        cate
+00007110: 676f 7279 203d 2043 6174 6567 6f72 7928  gory = Category(
+00007120: 2273 7461 7475 7322 2c20 6c61 6d62 6461  "status", lambda
+00007130: 206d 3a20 6d5b 2273 7563 6365 7373 6675   m: m["successfu
+00007140: 6c22 5d29 0a20 2020 2020 2020 2063 6174  l"]).        cat
+00007150: 6567 6f72 795f 6672 6571 7565 6e63 6965  egory_frequencie
+00007160: 7320 3d20 6765 745f 6361 7465 676f 7279  s = get_category
+00007170: 5f66 7265 7175 656e 6369 6573 3228 6576  _frequencies2(ev
+00007180: 656e 7473 2c20 6361 7465 676f 7279 290a  ents, category).
+00007190: 2020 2020 2020 2020 7072 696e 7428 6361          print(ca
+000071a0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
+000071b0: 6573 290a 2020 2020 2020 2020 2222 220a  es).        """.
+000071c0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+000071d0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+000071e0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000071f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00007200: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007210: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
+00007220: 2020 207c 2074 696d 6573 7461 6d70 5f73     | timestamp_s
+00007230: 7461 7274 2020 2020 207c 2074 696d 6573  tart     | times
+00007240: 7461 6d70 5f65 6e64 2020 2020 2020 207c  tamp_end       |
+00007250: 2046 616c 7365 2020 207c 2020 2054 7275   False   |   Tru
+00007260: 6520 7c0a 2020 2020 2020 2020 2b3d 3d3d  e |.        +===
+00007270: 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d  =====+==========
+00007280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+00007290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000072a0: 3d2b 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  =+=========+====
+000072b0: 3d3d 3d3d 2b0a 2020 2020 2020 2020 7c20  ====+.        | 
+000072c0: 2020 2020 2020 207c 2032 3032 332d 3031         | 2023-01
+000072d0: 2d30 3554 3133 3a35 373a 3035 207c 2032  -05T13:57:05 | 2
+000072e0: 3032 332d 3031 2d30 3554 3133 3a35 373a  023-01-05T13:57:
+000072f0: 3036 207c 2030 2020 2020 2020 207c 2020  06 | 0       |  
+00007300: 2020 2020 3320 7c0a 2020 2020 2020 2020      3 |.        
+00007310: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007340: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+00007350: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00007360: 2020 7c20 2020 2020 2020 207c 2032 3032    |        | 202
+00007370: 332d 3031 2d30 3554 3134 3a30 323a 3035  3-01-05T14:02:05
+00007380: 207c 2032 3032 332d 3031 2d30 3554 3134   | 2023-01-05T14
+00007390: 3a30 323a 3036 207c 2031 2020 2020 2020  :02:06 | 1      
+000073a0: 207c 2020 2020 2020 3020 7c0a 2020 2020   |      0 |.    
+000073b0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
+000073c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073d0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000073e0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000073f0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
+00007400: 2020 2020 2020 7c20 636f 756e 7420 207c        | count  |
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00007430: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00007440: 2020 2020 207c 2020 2020 2020 3220 7c0a       |      2 |.
+00007450: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+00007460: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00007470: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00007490: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000074a0: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
+000074b0: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
+000074c0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+000074d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000074e0: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
+000074f0: 3320 7c0a 2020 2020 2020 2020 2b2d 2d2d  3 |.        +---
+00007500: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007530: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
+00007540: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+00007550: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
+00007560: 2020 2023 205b 352e 335d 2043 6865 636b     # [5.3] Check
+00007570: 2069 6620 6576 656e 7473 2061 7265 2073   if events are s
+00007580: 6f72 7465 642e 0a20 2020 2020 2020 2072  orted..        r
+00007590: 6573 756c 7420 3d20 6973 5f73 6f72 7465  esult = is_sorte
+000075a0: 6428 6576 656e 7473 290a 2020 2020 2020  d(events).      
+000075b0: 2020 7072 696e 7428 7265 7375 6c74 290a    print(result).
+000075c0: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+000075d0: 2020 2020 3c21 2d2d 2065 6e64 2067 6574      <!-- end get
+000075e0: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
+000075f0: 2e70 7920 2d2d 3e0a 2020 2020 2020 2020  .py -->.        
+00007600: 0a20 2020 2020 2020 2023 2320 322e 332e  .        ## 2.3.
+00007610: 2053 686f 7274 2074 6865 6f72 790a 2020   Short theory.  
+00007620: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00007630: 6865 206c 6962 7261 7279 2070 726f 7669  he library provi
+00007640: 6465 7320 746f 6f6c 7320 666f 7220 6861  des tools for ha
+00007650: 6e64 6c69 6e67 2073 7472 6561 6d20 6461  ndling stream da
+00007660: 7461 2e20 5768 6174 2773 2061 2073 7472  ta. What's a str
+00007670: 6561 6d3f 2049 7427 7320 6120 7365 7175  eam? It's a sequ
+00007680: 656e 6365 206f 6620 656c 656d 656e 7473  ence of elements
+00007690: 2066 726f 6d20 6120 736f 7572 6365 2074   from a source t
+000076a0: 6861 740a 2020 2020 2020 2020 7375 7070  hat.        supp
+000076b0: 6f72 7473 2061 6767 7265 6761 7465 206f  orts aggregate o
+000076c0: 7065 7261 7469 6f6e 732e 0a20 2020 2020  perations..     
+000076d0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+000076e0: 5465 726d 730a 2020 2020 2020 2020 0a20  Terms.        . 
+000076f0: 2020 2020 2020 202d 202a 2a44 6174 6120         - **Data 
+00007700: 6f62 6a65 6374 2a2a 3a20 416e 2069 6e73  object**: An ins
+00007710: 7461 6e63 6520 6f66 2060 4461 7461 6020  tance of `Data` 
+00007720: 636c 6173 7320 7768 6963 6820 6973 2077  class which is w
+00007730: 7261 7070 6572 2075 6e64 6572 2073 7472  rapper under str
+00007740: 6561 6d2e 0a20 2020 2020 2020 202d 202a  eam..        - *
+00007750: 2a53 6571 7565 6e63 6520 6f66 2065 6c65  *Sequence of ele
+00007760: 6d65 6e74 732a 2a3a 0a20 2020 2020 2020  ments**:.       
+00007770: 2020 2041 205f 4461 7461 206f 626a 6563     A _Data objec
+00007780: 745f 2070 726f 7669 6465 7320 616e 2069  t_ provides an i
+00007790: 6e74 6572 6661 6365 2074 6f20 6120 7365  nterface to a se
+000077a0: 7175 656e 6365 6420 7365 7420 6f66 2076  quenced set of v
+000077b0: 616c 7565 7320 6f66 2061 2073 7065 6369  alues of a speci
+000077c0: 6669 6320 656c 656d 656e 7420 7479 7065  fic element type
+000077d0: 2e20 5374 7265 616d 2069 6e73 6964 6520  . Stream inside 
+000077e0: 7468 6520 5f44 6174 610a 2020 2020 2020  the _Data.      
+000077f0: 2020 2020 6f62 6a65 6374 5f20 2a2a 646f      object_ **do
+00007800: 6e19 7420 6163 7475 616c 6c79 2073 746f  n.t actually sto
+00007810: 7265 2a2a 2065 6c65 6d65 6e74 733b 2074  re** elements; t
+00007820: 6865 7920 6172 6520 636f 6d70 7574 6564  hey are computed
+00007830: 206f 6e20 6465 6d61 6e64 2e0a 2020 2020   on demand..    
+00007840: 2020 2020 2d20 2a2a 6461 7461 2073 6f75      - **data sou
+00007850: 7263 652a 2a20 2865 7861 6374 6c79 2069  rce** (exactly i
+00007860: 6e20 736d 616c 6c20 6c65 7474 6572 7329  n small letters)
+00007870: 3a0a 2020 2020 2020 2020 2020 416e 7920  :.          Any 
+00007880: 736f 7572 6365 206f 6620 6461 7461 2e20  source of data. 
+00007890: 452e 672e 205b 4c69 6768 7477 6569 6768  E.g. [Lightweigh
+000078a0: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
+000078b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000078c0: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+000078d0: 6c77 2d64 6174 612d 7072 6f76 6964 6572  lw-data-provider
+000078e0: 292c 2063 6f6c 6c65 6374 696f 6e73 2c0a  ), collections,.
+000078f0: 2020 2020 2020 2020 2020 6172 7261 7973            arrays
+00007900: 2c20 6f72 2049 2f4f 2072 6573 6f75 7263  , or I/O resourc
+00007910: 6573 2e0a 2020 2020 2020 2020 2d20 2a2a  es..        - **
+00007920: 4461 7461 536f 7572 6365 2a2a 3a0a 2020  DataSource**:.  
+00007930: 2020 2020 2020 2020 4120 636c 6173 7320          A class 
+00007940: 7468 6174 2069 7320 616e 2069 6e74 6572  that is an inter
+00007950: 6d65 6469 6174 6520 6c69 6e6b 2062 6574  mediate link bet
+00007960: 7765 656e 2074 6865 2053 6f75 7263 6541  ween the SourceA
+00007970: 5049 2061 6e64 2043 6f6d 6d61 6e64 732e  PI and Commands.
+00007980: 0a20 2020 2020 2020 202d 202a 2a53 6f75  .        - **Sou
+00007990: 7263 6541 5049 2a2a 3a0a 2020 2020 2020  rceAPI**:.      
+000079a0: 2020 2020 4561 6368 2073 6f75 7263 6520      Each source 
+000079b0: 6861 7320 6974 7320 6f77 6e20 4150 4920  has its own API 
+000079c0: 746f 2072 6574 7269 6576 6520 6461 7461  to retrieve data
+000079d0: 2e20 536f 7572 6365 4150 4920 6973 2061  . SourceAPI is a
+000079e0: 2063 6c61 7373 2074 6861 7420 7072 6f76   class that prov
+000079f0: 6964 6520 4150 4920 666f 7220 736f 6d65  ide API for some
+00007a00: 2064 6174 6120 736f 7572 6365 2e0a 2020   data source..  
+00007a10: 2020 2020 2020 2d20 2a2a 436f 6d6d 616e        - **Comman
+00007a20: 6473 2a2a 3a0a 2020 2020 2020 2020 2020  ds**:.          
+00007a30: 436c 6173 7365 7320 7468 6174 2070 726f  Classes that pro
+00007a40: 7669 6465 2075 7365 722d 6672 6965 6e64  vide user-friend
+00007a50: 6c79 2069 6e74 6572 6661 6365 7320 666f  ly interfaces fo
+00007a60: 7220 6765 7474 696e 6720 736f 6d65 2064  r getting some d
+00007a70: 6174 6120 6672 6f6d 2044 6174 6153 6f75  ata from DataSou
+00007a80: 7263 652e 2043 6f6d 6d61 6e64 7320 7573  rce. Commands us
+00007a90: 6520 5f53 6f75 7263 6541 5049 5f20 746f  e _SourceAPI_ to
+00007aa0: 0a20 2020 2020 2020 2020 2061 6368 6965  .          achie
+00007ab0: 7665 2069 742e 0a20 2020 2020 2020 202d  ve it..        -
+00007ac0: 202a 2a41 6461 7074 6572 732a 2a3a 0a20   **Adapters**:. 
+00007ad0: 2020 2020 2020 2020 2049 7427 7320 7369           It's si
+00007ae0: 6d69 6c61 7220 746f 2066 756e 6374 696f  milar to functio
+00007af0: 6e20 666f 7220 6044 6174 612e 6d61 7060  n for `Data.map`
+00007b00: 206d 6574 686f 642e 2041 646f 7074 6162   method. Adoptab
+00007b10: 6c65 2063 6f6d 6d61 6e64 7320 7573 6564  le commands used
+00007b20: 2069 7420 746f 2075 7064 6174 6520 7468   it to update th
+00007b30: 6520 6461 7461 2073 7472 6561 6d2e 0a20  e data stream.. 
+00007b40: 2020 2020 2020 202d 202a 2a41 6767 7265         - **Aggre
+00007b50: 6761 7465 206f 7065 7261 7469 6f6e 732a  gate operations*
+00007b60: 2a3a 0a20 2020 2020 2020 2020 2043 6f6d  *:.          Com
+00007b70: 6d6f 6e20 6f70 6572 6174 696f 6e73 2073  mon operations s
+00007b80: 7563 6820 6173 2066 696c 7465 722c 206d  uch as filter, m
+00007b90: 6170 2c20 6c69 6d69 7420 616e 6420 736f  ap, limit and so
+00007ba0: 206f 6e2e 0a20 2020 2020 2020 202d 202a   on..        - *
+00007bb0: 2a57 6f72 6b66 6c6f 772a 2a3a 2041 6e20  *Workflow**: An 
+00007bc0: 6f72 6465 7265 6420 7365 7420 6f66 205f  ordered set of _
+00007bd0: 4167 6772 6567 6174 6520 6f70 6572 6174  Aggregate operat
+00007be0: 696f 6e73 5f2e 0a20 2020 2020 2020 200a  ions_..        .
+00007bf0: 2020 2020 2020 2020 2323 2320 436f 6e63          ### Conc
+00007c00: 6570 740a 2020 2020 2020 2020 0a20 2020  ept.        .   
+00007c10: 2020 2020 2054 6865 206c 6962 7261 7279       The library
+00007c20: 2064 6573 6372 6962 6573 2074 6865 2068   describes the h
+00007c30: 6967 682d 6c65 7665 6c20 696e 7465 7266  igh-level interf
+00007c40: 6163 6573 2060 4953 6f75 7263 6541 5049  aces `ISourceAPI
+00007c50: 602c 2060 4944 6174 6153 6f75 7263 6560  `, `IDataSource`
+00007c60: 2c20 6049 436f 6d6d 616e 6460 2c20 6049  , `ICommand`, `I
+00007c70: 4164 6170 7465 7260 2e0a 2020 2020 2020  Adapter`..      
+00007c80: 2020 0a20 2020 2020 2020 2041 6e79 2064    .        Any d
+00007c90: 6174 6120 736f 7572 6365 206d 7573 7420  ata source must 
+00007ca0: 6265 2064 6573 6372 6962 6564 2062 7920  be described by 
+00007cb0: 7468 6520 6049 4461 7461 536f 7572 6365  the `IDataSource
+00007cc0: 6020 6162 7374 7261 6374 2063 6c61 7373  ` abstract class
+00007cd0: 2e20 5468 6573 6520 6361 6e20 6265 205f  . These can be _
+00007ce0: 4669 6c65 4461 7461 536f 7572 6365 5f2c  FileDataSource_,
+00007cf0: 0a20 2020 2020 2020 205f 4353 5644 6174  .        _CSVDat
+00007d00: 6153 6f75 7263 655f 2c20 5f44 4244 6174  aSource_, _DBDat
+00007d10: 6153 6f75 7263 655f 2061 6e64 206f 7468  aSource_ and oth
+00007d20: 6572 2e0a 2020 2020 2020 2020 0a20 2020  er..        .   
+00007d30: 2020 2020 2055 7375 616c 6c79 2c20 6461       Usually, da
+00007d40: 7461 2073 6f75 7263 6573 2068 6176 6520  ta sources have 
+00007d50: 736f 6d65 206b 696e 6420 6f66 2041 5049  some kind of API
+00007d60: 2e20 4461 7461 6261 7365 7320 2d20 7072  . Databases - pr
+00007d70: 6f76 6964 6520 5351 4c20 6c61 6e67 7561  ovide SQL langua
+00007d80: 6765 2c20 7768 656e 2077 6f72 6b69 6e67  ge, when working
+00007d90: 2077 6974 6820 6120 6669 6c65 2c20 796f   with a file, yo
+00007da0: 7520 6361 6e20 7265 6164 0a20 2020 2020  u can read.     
+00007db0: 2020 206c 696e 6520 6279 206c 696e 652c     line by line,
+00007dc0: 2065 7463 2e20 5468 6973 2041 5049 2069   etc. This API i
+00007dd0: 7320 6465 7363 7269 6265 6420 6279 2074  s described by t
+00007de0: 6865 2060 4953 6f75 7263 6541 5049 6020  he `ISourceAPI` 
+00007df0: 636c 6173 732e 2042 6563 6175 7365 2064  class. Because d
+00007e00: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
+00007e10: 7320 6f66 2074 6865 2073 616d 6520 6461  s of the same da
+00007e20: 7461 2073 6f75 7263 650a 2020 2020 2020  ta source.      
+00007e30: 2020 6d61 7920 6861 7665 2064 6966 6665    may have diffe
+00007e40: 7265 6e74 2041 5049 2c20 6974 2069 7320  rent API, it is 
+00007e50: 6265 7474 6572 2074 6f20 6372 6561 7465  better to create
+00007e60: 2061 2063 6c61 7373 2066 6f72 2065 6163   a class for eac
+00007e70: 6820 7665 7273 696f 6e2e 0a20 2020 2020  h version..     
+00007e80: 2020 200a 2020 2020 2020 2020 4765 6e65     .        Gene
+00007e90: 7261 6c6c 792c 2064 6174 6120 736f 7572  rally, data sour
+00007ea0: 6365 2041 5049 7320 6172 6520 6869 6464  ce APIs are hidd
+00007eb0: 656e 2062 6568 696e 6420 636f 6e76 656e  en behind conven
+00007ec0: 6965 6e74 2069 6e74 6572 6661 6365 732e  ient interfaces.
+00007ed0: 2054 6865 2072 6f6c 6520 6f66 2074 6865   The role of the
+00007ee0: 7365 2069 6e74 6572 6661 6365 7320 6973  se interfaces is
+00007ef0: 2070 6c61 7965 640a 2020 2020 2020 2020   played.        
+00007f00: 6279 2060 4943 6f6d 6d61 6e64 6020 636c  by `ICommand` cl
+00007f10: 6173 7365 732e 0a20 2020 2020 2020 200a  asses..        .
+00007f20: 2020 2020 2020 2020 6049 4164 6170 7465          `IAdapte
+00007f30: 7260 2063 6c61 7373 6573 2074 7261 6e73  r` classes trans
+00007f40: 666f 726d 2064 6174 6120 7374 7265 616d  form data stream
+00007f50: 206c 696b 6520 6675 6e63 7469 6f6e 7320   like functions 
+00007f60: 666f 7220 6044 6174 612e 6d61 7060 206d  for `Data.map` m
+00007f70: 6574 686f 642e 2045 7373 656e 7469 616c  ethod. Essential
+00007f80: 6c79 2069 7427 7320 7468 6520 7361 6d65  ly it's the same
+00007f90: 2074 6869 6e67 2062 7574 206d 6f72 650a   thing but more.
+00007fa0: 2020 2020 2020 2020 666c 6578 6962 6c65          flexible
+00007fb0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007fc0: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
+00007fd0: 4c77 4450 2044 6174 6153 6f75 7263 6528  LwDP DataSource(
+00007fe0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007ff0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
+00008000: 732d 736f 7572 6365 2d6c 7764 7029 2075  s-source-lwdp) u
+00008010: 7365 7320 7468 6573 6520 6162 7374 7261  ses these abstra
+00008020: 6374 2063 6c61 7373 6573 2074 6f20 6275  ct classes to bu
+00008030: 696c 6420 6974 7320 696d 706c 656d 656e  ild its implemen
+00008040: 7461 7469 6f6e 2e59 6f75 2063 616e 2065  tation.You can e
+00008050: 6173 696c 7920 6372 6561 7465 2079 6f75  asily create you
+00008060: 7220 6f77 6e20 756e 6971 7565 2063 6f6d  r own unique com
+00008070: 6d61 6e64 7320 666f 7220 5f4c 7744 5020  mands for _LwDP 
+00008080: 4461 7461 536f 7572 6365 5f2c 2061 7320  DataSource_, as 
+00008090: 7765 6c6c 2061 7320 656e 7469 7265 0a20  well as entire. 
+000080a0: 2020 2020 2020 205f 4461 7461 536f 7572         _DataSour
+000080b0: 6365 5f20 636c 6173 7365 732e 205b 4865  ce_ classes. [He
+000080c0: 7265 2069 7320 6120 646f 6375 6d65 6e74  re is a document
+000080d0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
+000080e0: 7469 6f6e 2f64 6174 6173 6f75 7263 652e  tion/datasource.
+000080f0: 6d64 2920 6f6e 2068 6f77 2074 6f20 696d  md) on how to im
+00008100: 706c 656d 656e 7420 7468 6573 6520 696e  plement these in
+00008110: 7465 7266 6163 6573 2e0a 2020 2020 2020  terfaces..      
+00008120: 2020 0a20 2020 2020 2020 2021 5b44 6174    .        ![Dat
+00008130: 6120 7374 7265 616d 2070 6970 656c 696e  a stream pipelin
+00008140: 655d 2864 6f63 756d 656e 7461 7469 6f6e  e](documentation
+00008150: 2f69 6d67 2f63 6f6e 6365 7074 2e70 6e67  /img/concept.png
+00008160: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00008170: 2020 2023 2323 2053 7472 6561 6d20 6f70     ### Stream op
+00008180: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
+00008190: 200a 2020 2020 2020 2020 4675 7274 6865   .        Furthe
+000081a0: 726d 6f72 652c 2073 7472 6561 6d20 6f70  rmore, stream op
+000081b0: 6572 6174 696f 6e73 2068 6176 6520 7477  erations have tw
+000081c0: 6f20 6675 6e64 616d 656e 7461 6c20 6368  o fundamental ch
+000081d0: 6172 6163 7465 7269 7374 6963 7320 7468  aracteristics th
+000081e0: 6174 206d 616b 6520 7468 656d 2076 6572  at make them ver
+000081f0: 7920 6469 6666 6572 656e 7420 6672 6f6d  y different from
+00008200: 2063 6f6c 6c65 6374 696f 6e0a 2020 2020   collection.    
+00008210: 2020 2020 6f70 6572 6174 696f 6e73 3a20      operations: 
+00008220: 5f50 6970 656c 696e 696e 675f 2061 6e64  _Pipelining_ and
+00008230: 205f 496e 7465 726e 616c 2069 7465 7261   _Internal itera
+00008240: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
+00008250: 2020 2020 2020 2020 2323 2323 2050 6970          #### Pip
+00008260: 656c 696e 696e 670a 2020 2020 2020 2020  elining.        
+00008270: 0a20 2020 2020 2020 204d 616e 7920 7374  .        Many st
+00008280: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
+00008290: 7265 7475 726e 2061 2073 7472 6561 6d20  return a stream 
+000082a0: 7468 656d 7365 6c76 6573 2e20 5468 6973  themselves. This
+000082b0: 2061 6c6c 6f77 7320 6f70 6572 6174 696f   allows operatio
+000082c0: 6e73 2074 6f20 6265 2063 6861 696e 6564  ns to be chained
+000082d0: 2074 6f20 666f 726d 2061 206c 6172 6765   to form a large
+000082e0: 7220 7069 7065 6c69 6e65 2e0a 2020 2020  r pipeline..    
+000082f0: 2020 2020 0a20 2020 2020 2020 2021 5b44      .        ![D
+00008300: 6174 6120 7374 7265 616d 2070 6970 656c  ata stream pipel
+00008310: 696e 655d 2864 6f63 756d 656e 7461 7469  ine](documentati
+00008320: 6f6e 2f69 6d67 2f64 6174 615f 7374 7265  on/img/data_stre
+00008330: 616d 5f70 6970 656c 696e 652e 706e 6729  am_pipeline.png)
+00008340: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00008350: 2020 2323 2323 2049 6e74 6572 6e61 6c20    #### Internal 
+00008360: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
+00008370: 2020 0a20 2020 2020 2020 2049 6e20 636f    .        In co
+00008380: 6e74 7261 7374 2074 6f20 636f 6c6c 6563  ntrast to collec
+00008390: 7469 6f6e 732c 2077 6869 6368 2061 7265  tions, which are
+000083a0: 2069 7465 7261 7465 6420 6578 706c 6963   iterated explic
+000083b0: 6974 6c79 2028 6578 7465 726e 616c 2069  itly (external i
+000083c0: 7465 7261 7469 6f6e 292c 2073 7472 6561  teration), strea
+000083d0: 6d20 6f70 6572 6174 696f 6e73 2064 6f20  m operations do 
+000083e0: 7468 6520 6974 6572 6174 696f 6e0a 2020  the iteration.  
+000083f0: 2020 2020 2020 6265 6869 6e64 2074 6865        behind the
+00008400: 2073 6365 6e65 7320 666f 7220 796f 752e   scenes for you.
+00008410: 204e 6f74 652c 2069 7420 646f 6573 6e27   Note, it doesn'
+00008420: 7420 6d65 616e 2079 6f75 2063 616e 6e6f  t mean you canno
+00008430: 7420 6974 6572 6174 6520 7468 6520 5f44  t iterate the _D
+00008440: 6174 6120 6f62 6a65 6374 5f2e 0a20 2020  ata object_..   
+00008450: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00008460: 2020 2020 2020 2023 2323 2044 6174 6120         ### Data 
+00008470: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
+00008480: 2020 0a20 2020 2020 2020 2054 6865 2044    .        The D
+00008490: 6174 6120 6f62 6a65 6374 2063 6f6e 7374  ata object const
+000084a0: 7275 6374 6f72 206d 6574 686f 6420 7461  ructor method ta
+000084b0: 6b65 7320 696e 2061 7320 6172 6775 6d65  kes in as argume
+000084c0: 6e74 2065 6974 6865 7220 616e 2069 7465  nt either an ite
+000084d0: 7261 746f 7220 6f76 6572 206f 626a 6563  rator over objec
+000084e0: 7473 206f 7220 6120 6765 6e65 7261 746f  ts or a generato
+000084f0: 7220 6675 6e63 7469 6f6e 2e0a 2020 2020  r function..    
+00008500: 2020 2020 5468 6520 4461 7461 206f 626a      The Data obj
+00008510: 6563 7420 6974 6572 6174 6f72 2068 616e  ect iterator han
+00008520: 646c 6573 2065 6163 6820 6974 656d 2069  dles each item i
+00008530: 6e20 7468 6973 2069 7465 7261 746f 7220  n this iterator 
+00008540: 6f72 2067 656e 6572 6174 6f72 2061 7320  or generator as 
+00008550: 7468 6579 2061 7265 2c20 6d65 616e 696e  they are, meanin
+00008560: 6720 6974 2064 6f65 736e 2774 2074 7279  g it doesn't try
+00008570: 2074 6f20 7265 6164 2074 6865 2063 6f6e   to read the con
+00008580: 7465 6e74 206f 6620 6974 656d 206f 7220  tent of item or 
+00008590: 7265 7475 726e 2074 6865 6d20 6d6f 6469  return them modi
+000085a0: 6669 6564 2069 6e20 616e 7920 7761 792c  fied in any way,
+000085b0: 2069 6e73 7465 6164 2072 6574 7572 6e73   instead returns
+000085c0: 2074 6865 2069 7465 6d20 6974 7365 6c66   the item itself
+000085d0: 2e0a 2020 2020 2020 2020 5468 6520 6f6e  ..        The on
+000085e0: 6c79 2065 7863 6570 7469 6f6e 2074 6f20  ly exception to 
+000085f0: 7468 6973 2069 7320 7768 656e 2044 6174  this is when Dat
+00008600: 6120 6f62 6a65 6374 2069 7320 6275 696c  a object is buil
+00008610: 7420 7573 696e 6720 6974 6572 6174 6f72  t using iterator
+00008620: 206f 7220 6765 6e65 7261 746f 7220 6f76   or generator ov
+00008630: 6572 206f 7468 6572 2044 6174 6120 6f62  er other Data ob
+00008640: 6a65 6374 732e 204e 6f74 6520 7468 6174  jects. Note that
+00008650: 2074 6869 7320 6974 6572 6174 6f72 206f   this iterator o
+00008660: 7220 6765 6e65 7261 746f 7220 6d75 7374  r generator must
+00008670: 206f 6e6c 7920 6265 2079 6965 6c64 696e   only be yieldin
+00008680: 6720 4461 7461 206f 626a 6563 7473 2061  g Data objects a
+00008690: 6e64 206e 6f74 6869 6e67 2065 6c73 652e  nd nothing else.
+000086a0: 2049 6620 7765 2062 7569 6c64 2066 726f   If we build fro
+000086b0: 6d20 6120 6d69 7820 6f66 2044 6174 6120  m a mix of Data 
+000086c0: 6f62 6a65 6374 7320 616e 6420 736f 6d65  objects and some
+000086d0: 206f 7468 6572 2074 7970 6573 2c20 4461   other types, Da
+000086e0: 7461 206f 626a 6563 7473 2720 636f 6e74  ta objects' cont
+000086f0: 656e 7420 776f 6e27 7420 6265 2072 6561  ent won't be rea
+00008700: 6420 616e 6420 696e 7374 6561 6420 6974  d and instead it
+00008710: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00008720: 6420 6173 2044 6174 6120 6f62 6a65 6374  d as Data object
+00008730: 2069 7473 656c 662e 0a20 2020 2020 2020   itself..       
+00008740: 200a 2020 2020 2020 2020 536d 616c 6c20   .        Small 
+00008750: 6578 616d 706c 6520 746f 2064 656d 6f6e  example to demon
+00008760: 7374 7261 7465 3a0a 2020 2020 2020 2020  strate:.        
+00008770: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
+00008780: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
+00008790: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
+000087a0: 732e 6461 7461 2069 6d70 6f72 7420 4461  s.data import Da
+000087b0: 7461 0a20 2020 2020 2020 200a 2020 2020  ta.        .    
+000087c0: 2020 2020 6431 203d 2044 6174 6128 5b31      d1 = Data([1
+000087d0: 2c32 2c33 5d29 0a20 2020 2020 2020 2064  ,2,3]).        d
+000087e0: 3220 3d20 4461 7461 285b 342c 352c 365d  2 = Data([4,5,6]
+000087f0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00008800: 2020 206f 6e6c 795f 6461 7461 5f6f 626a     only_data_obj
+00008810: 6563 7473 203d 2044 6174 6128 5b64 312c  ects = Data([d1,
+00008820: 6432 5d29 2023 2057 696c 6c20 6974 6572  d2]) # Will iter
+00008830: 6174 6520 6173 2031 2c32 2c33 2c34 2c35  ate as 1,2,3,4,5
+00008840: 2c36 0a20 2020 2020 2020 2064 6174 615f  ,6.        data_
+00008850: 616e 645f 6c69 7374 203d 2044 6174 6128  and_list = Data(
+00008860: 5b64 312c 5b34 2c35 2c36 5d5d 2920 2320  [d1,[4,5,6]]) # 
+00008870: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00008880: 6431 2c20 5b34 2c35 2c36 5d0a 2020 2020  d1, [4,5,6].    
+00008890: 2020 2020 6461 7461 5f61 6e64 5f6e 756d      data_and_num
+000088a0: 6265 7273 203d 2044 6174 6128 5b64 312c  bers = Data([d1,
+000088b0: 342c 352c 365d 2920 2320 5769 6c6c 2069  4,5,6]) # Will i
+000088c0: 7465 7261 7465 2061 7320 6431 2c34 2c35  terate as d1,4,5
+000088d0: 2c36 0a20 2020 2020 2020 206c 6973 7473  ,6.        lists
+000088e0: 5f6f 6e6c 7920 3d20 4461 7461 285b 312c  _only = Data([1,
+000088f0: 322c 335d 2c5b 342c 352c 365d 2920 2320  2,3],[4,5,6]) # 
+00008900: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00008910: 5b31 2c32 2c33 5d2c 5b34 2c35 2c36 5d0a  [1,2,3],[4,5,6].
+00008920: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008930: 2023 2049 6620 7765 2077 616e 7420 746f   # If we want to
+00008940: 2069 7465 7261 7465 206f 7665 7220 636f   iterate over co
+00008950: 6e74 656e 7420 6f66 206c 6973 7420 6f66  ntent of list of
+00008960: 206c 6973 7473 2c20 7765 2073 686f 756c   lists, we shoul
+00008970: 6420 6669 7273 7420 6372 6561 7465 2044  d first create D
+00008980: 6174 6120 6f62 6a65 6374 7320 6672 6f6d  ata objects from
+00008990: 2074 6865 6d2c 0a20 2020 2020 2020 2023   them,.        #
+000089a0: 2074 6865 6e20 7573 6520 7468 656d 2074   then use them t
+000089b0: 6f20 636f 6e73 7472 7563 7420 6e65 7720  o construct new 
+000089c0: 4461 7461 206f 626a 6563 7420 6173 2069  Data object as i
+000089d0: 6e20 6361 7365 206f 6620 6431 2061 6e64  n case of d1 and
+000089e0: 2064 322c 2063 7265 6174 696e 6720 276f   d2, creating 'o
+000089f0: 6e6c 795f 6461 7461 5f6f 626a 6563 7473  nly_data_objects
+00008a00: 2720 696e 2074 6869 7320 6578 616d 706c  ' in this exampl
+00008a10: 652e 0a20 2020 2020 2020 2060 6060 0a20  e..        ```. 
+00008a20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008a30: 200a 2020 2020 2020 2020 2323 2320 4461   .        ### Da
+00008a40: 7461 2063 6163 6869 6e67 0a20 2020 2020  ta caching.     
+00008a50: 2020 200a 2020 2020 2020 2020 5468 6520     .        The 
+00008a60: 5f44 6174 6120 6f62 6a65 6374 5f20 7072  _Data object_ pr
+00008a70: 6f76 6964 6573 2074 6865 2061 6269 6c69  ovides the abili
+00008a80: 7479 2074 6f20 7573 6520 7468 6520 6361  ty to use the ca
+00008a90: 6368 652e 2054 6865 2063 6163 6865 2077  che. The cache w
+00008aa0: 6f72 6b73 2066 6f72 2065 6163 6820 5f44  orks for each _D
+00008ab0: 6174 6120 6f62 6a65 6374 5f2c 2074 6861  ata object_, tha
+00008ac0: 7420 6973 2c20 796f 7520 6368 6f6f 7365  t is, you choose
+00008ad0: 0a20 2020 2020 2020 2077 6869 6368 205f  .        which _
+00008ae0: 4461 7461 206f 626a 6563 745f 2079 6f75  Data object_ you
+00008af0: 2077 616e 7420 746f 2073 6176 652e 2054   want to save. T
+00008b00: 6865 205f 4461 7461 206f 626a 6563 745f  he _Data object_
+00008b10: 2063 6163 6865 2069 7320 7361 7665 6420   cache is saved 
+00008b20: 6166 7465 7220 7468 6520 6669 7273 7420  after the first 
+00008b30: 6974 6572 6174 696f 6e2c 2062 7574 2074  iteration, but t
+00008b40: 6865 2069 7465 7261 7469 6f6e 0a20 2020  he iteration.   
+00008b50: 2020 2020 2073 6f75 7263 6520 6d61 7920       source may 
+00008b60: 6265 2064 6966 6665 7265 6e74 2e0a 2020  be different..  
+00008b70: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
+00008b80: 6620 796f 7520 646f 6e27 7420 7573 6520  f you don't use 
+00008b90: 7468 6520 6361 6368 652c 2079 6f75 7220  the cache, your 
+00008ba0: 736f 7572 6365 2077 696c 6c20 6265 2074  source will be t
+00008bb0: 6865 2064 6174 6120 736f 7572 6365 2079  he data source y
+00008bc0: 6f75 2068 6176 6520 696e 2074 6865 205f  ou have in the _
+00008bd0: 4461 7461 204f 626a 6563 745f 2e20 4275  Data Object_. Bu
+00008be0: 7420 6966 2079 6f75 2075 7365 2074 6865  t if you use the
+00008bf0: 2063 6163 6865 2c0a 2020 2020 2020 2020   cache,.        
+00008c00: 796f 7572 2073 6f75 7263 6520 6361 6e20  your source can 
+00008c10: 6265 2074 6865 2064 6174 6120 736f 7572  be the data sour
+00008c20: 6365 2c20 7468 6520 7061 7265 6e74 2063  ce, the parent c
+00008c30: 6163 6865 2c20 6f72 206f 776e 2063 6163  ache, or own cac
+00008c40: 6865 3a0a 2020 2020 2020 2020 0a20 2020  he:.        .   
+00008c50: 2020 2020 202a 2054 6865 2064 6174 6120       * The data 
+00008c60: 736f 7572 6365 3a0a 2020 2020 2020 2020  source:.        
+00008c70: 2020 4966 2074 6865 205f 4461 7461 204f    If the _Data O
+00008c80: 626a 6563 745f 2064 6f65 736e 2774 2068  bject_ doesn't h
+00008c90: 6176 6520 6120 7061 7265 6e74 2063 6163  ave a parent cac
+00008ca0: 6865 2061 6e64 2069 7473 2063 6163 6865  he and its cache
+00008cb0: 2e0a 2020 2020 2020 2020 2a20 5468 6520  ..        * The 
+00008cc0: 7061 7265 6e74 2063 6163 6865 3a0a 2020  parent cache:.  
+00008cd0: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
+00008ce0: 4461 7461 204f 626a 6563 745f 2068 6173  Data Object_ has
+00008cf0: 2061 2070 6172 656e 7420 6361 6368 652e   a parent cache.
+00008d00: 2049 7420 646f 6573 6e27 7420 6d61 7474   It doesn't matt
+00008d10: 6572 2077 6861 7420 706f 7369 7469 6f6e  er what position
+00008d20: 2074 6865 2070 6172 656e 7420 6361 6368   the parent cach
+00008d30: 6520 6861 7320 696e 2069 6e68 6572 6974  e has in inherit
+00008d40: 616e 6365 2e0a 2020 2020 2020 2020 2020  ance..          
+00008d50: 5f44 6174 6120 4f62 6a65 6374 5f20 756e  _Data Object_ un
+00008d60: 6465 7273 7461 6e64 7320 7768 6f73 6520  derstands whose 
+00008d70: 6361 6368 6520 6974 2069 7320 616e 6420  cache it is and 
+00008d80: 6578 6563 7574 6573 2074 6865 2070 6172  executes the par
+00008d90: 7420 6f66 2074 6865 2077 6f72 6b66 6c6f  t of the workflo
+00008da0: 7720 7468 6174 2077 6173 206e 6f74 2065  w that was not e
+00008db0: 7865 6375 7465 642e 0a20 2020 2020 2020  xecuted..       
+00008dc0: 202a 2054 6865 206f 776e 2063 6163 6865   * The own cache
+00008dd0: 3a0a 2020 2020 2020 2020 2020 4966 2069  :.          If i
+00008de0: 7420 6973 206e 6f74 2074 6865 2066 6972  t is not the fir
+00008df0: 7374 2069 7465 7261 7469 6f6e 206f 6620  st iteration of 
+00008e00: 7468 6973 2044 6174 6120 6f62 6a65 6374  this Data object
+00008e10: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008e20: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
+00008e30: 2063 6163 6865 2073 7461 7465 206f 6620   cache state of 
+00008e40: 7468 6520 4461 7461 206f 626a 6563 7420  the Data object 
+00008e50: 6973 206e 6f74 2069 6e68 6572 6974 6564  is not inherited
+00008e60: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008e70: 2020 2023 2323 2320 466f 7263 6564 2063     #### Forced c
+00008e80: 6163 6869 6e67 0a20 2020 2020 2020 2059  aching.        Y
+00008e90: 6f75 2063 616e 2074 656c 6c20 4453 2074  ou can tell DS t
+00008ea0: 6f20 6361 6368 6520 6461 7461 2074 6f20  o cache data to 
+00008eb0: 7370 6563 6966 6963 2063 6163 6865 2066  specific cache f
+00008ec0: 696c 652c 2077 6869 6368 2077 6f6e 2774  ile, which won't
+00008ed0: 2062 6520 6465 6c65 7465 6420 6166 7465   be deleted afte
+00008ee0: 7220 7363 7269 7074 2065 6e64 2e0a 2020  r script end..  
+00008ef0: 2020 2020 2020 596f 7520 6361 6e20 7365        You can se
+00008f00: 6520 6578 616d 706c 6520 696e 2031 2e31  e example in 1.1
+00008f10: 3220 7365 6374 696f 6e20 6f66 205b 6765  2 section of [ge
+00008f20: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
+00008f30: 655d 2865 7861 6d70 6c65 732f 6765 745f  e](examples/get_
+00008f40: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
+00008f50: 7079 292e 0a20 2020 2020 2020 200a 2020  py)..        .  
+00008f60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00008f70: 2323 2045 7665 6e74 5472 6565 2061 6e64  ## EventTree and
+00008f80: 2063 6f6c 6c65 6374 696f 6e73 0a20 2020   collections.   
+00008f90: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00008fa0: 2323 2045 7665 6e74 5472 6565 0a20 2020  ## EventTree.   
+00008fb0: 2020 2020 200a 2020 2020 2020 2020 6045       .        `E
+00008fc0: 7665 6e74 5472 6565 6020 6973 2061 2074  ventTree` is a t
+00008fd0: 7265 652d 6261 7365 6420 6461 7461 2073  ree-based data s
+00008fe0: 7472 7563 7475 7265 206f 6620 6576 656e  tructure of even
+00008ff0: 7473 2e20 4974 2061 6c6c 6f77 7320 796f  ts. It allows yo
+00009000: 7520 6765 7420 6368 696c 6472 656e 2061  u get children a
+00009010: 6e64 2070 6172 656e 7473 206f 6620 6576  nd parents of ev
+00009020: 656e 742c 0a20 2020 2020 2020 2064 6973  ent,.        dis
+00009030: 706c 6179 2074 7265 652c 2067 6574 2066  play tree, get f
+00009040: 756c 6c20 7061 7468 2074 6f20 6576 656e  ull path to even
+00009050: 7420 6574 632e 0a20 2020 2020 2020 200a  t etc..        .
+00009060: 2020 2020 2020 2020 4465 7461 696c 733a          Details:
+00009070: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00009080: 2020 2a20 6045 7665 6e74 5472 6565 6020    * `EventTree` 
+00009090: 636f 6e74 6169 6e73 2061 6c6c 2065 7665  contains all eve
+000090a0: 6e74 7320 696e 206d 656d 6f72 792e 0a20  nts in memory.. 
+000090b0: 2020 2020 2020 202a 2054 7265 6520 6861         * Tree ha
+000090c0: 7320 736f 6d65 2069 6d70 6f72 7461 6e74  s some important
+000090d0: 2074 6572 6d73 3a0a 2020 2020 2020 2020   terms:.        
+000090e0: 2020 2020 312e 205f 416e 6365 7374 6f72      1. _Ancestor
+000090f0: 5f20 6973 2061 6e79 2072 656c 6174 6976  _ is any relativ
+00009100: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+00009110: 7020 7468 6520 7472 6565 2028 6772 616e  p the tree (gran
+00009120: 6470 6172 656e 742c 2070 6172 656e 7420  dparent, parent 
+00009130: 6574 632e 292e 0a20 2020 2020 2020 2020  etc.)..         
+00009140: 2020 2032 2e20 5f50 6172 656e 745f 2069     2. _Parent_ i
+00009150: 7320 6f6e 6c79 2074 6865 2066 6972 7374  s only the first
+00009160: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00009170: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00009180: 6565 2e0a 2020 2020 2020 2020 2020 2020  ee..            
+00009190: 332e 205f 4368 696c 645f 2069 7320 7468  3. _Child_ is th
+000091a0: 6520 6669 7273 7420 7265 6c61 7469 7665  e first relative
+000091b0: 206f 6620 7468 6520 6576 656e 7420 646f   of the event do
+000091c0: 776e 2074 6865 2074 7265 652e 0a20 2020  wn the tree..   
+000091d0: 2020 2020 200a 2020 2020 2020 2020 5461       .        Ta
+000091e0: 6b65 2061 206c 6f6f 6b20 6174 2074 6865  ke a look at the
+000091f0: 2066 6f6c 6c6f 7769 6e67 2048 544d 4c20   following HTML 
+00009200: 7472 6565 2074 6f20 756e 6465 7273 7461  tree to understa
+00009210: 6e64 2074 6865 6d2e 0a20 2020 2020 2020  nd them..       
+00009220: 200a 2020 2020 2020 2020 2020 2060 6060   .           ```
+00009230: 0a20 2020 2020 2020 2020 2020 203c 626f  .            <bo
+00009240: 6479 3e20 3c21 2d2d 2061 6e63 6573 746f  dy> <!-- ancesto
+00009250: 7220 2867 7261 6e64 7061 7265 6e74 292c  r (grandparent),
+00009260: 2062 7574 206e 6f74 2070 6172 656e 7420   but not parent 
+00009270: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
+00009280: 2020 2020 3c64 6976 3e20 3c21 2d2d 2070      <div> <!-- p
+00009290: 6172 656e 7420 2620 616e 6365 7374 6f72  arent & ancestor
+000092a0: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+000092b0: 2020 2020 2020 2020 203c 703e 4865 6c6c           <p>Hell
+000092c0: 6f2c 2077 6f72 6c64 213c 2f70 3e20 3c21  o, world!</p> <!
+000092d0: 2d2d 2063 6869 6c64 202d 2d3e 0a20 2020  -- child -->.   
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 203c 703e 476f 6f64 6279 6521 3c2f 703e   <p>Goodbye!</p>
+00009300: 203c 212d 2d20 7369 626c 696e 6720 2d2d   <!-- sibling --
+00009310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00009320: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00009330: 2020 2020 203c 2f62 6f64 793e 0a20 2020       </body>.   
+00009340: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00009350: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00009360: 2320 436f 6c6c 6563 7469 6f6e 730a 2020  # Collections.  
+00009370: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+00009380: 2a45 7665 6e74 5472 6565 436f 6c6c 6563  *EventTreeCollec
+00009390: 7469 6f6e 2a2a 2069 7320 6120 636f 6c6c  tion** is a coll
+000093a0: 6563 7469 6f6e 206f 6620 4576 656e 7454  ection of EventT
+000093b0: 7265 6573 2e20 5468 6520 636f 6c6c 6563  rees. The collec
+000093c0: 7469 6f6e 2062 7569 6c64 7320 6120 6665  tion builds a fe
+000093d0: 7720 5f45 7665 6e74 5472 6565 5f20 6279  w _EventTree_ by
+000093e0: 2070 6173 7365 6420 5f44 6174 610a 2020   passed _Data.  
+000093f0: 2020 2020 2020 6f62 6a65 6374 5f2e 2041        object_. A
+00009400: 6c74 686f 7567 6820 796f 7520 6361 6e20  lthough you can 
+00009410: 6368 616e 6765 2074 6865 2074 7265 6520  change the tree 
+00009420: 6469 7265 6374 6c79 2c20 6974 2773 2062  directly, it's b
+00009430: 6574 7465 7220 746f 2064 6f20 6974 2074  etter to do it t
+00009440: 6872 6f75 6768 2063 6f6c 6c65 6374 696f  hrough collectio
+00009450: 6e73 2062 6563 6175 7365 2074 6865 7920  ns because they 
+00009460: 6172 6520 6177 6172 6520 6f66 0a20 2020  are aware of.   
+00009470: 2020 2020 2060 6465 7461 6368 6564 5f65       `detached_e
+00009480: 7665 6e74 7360 2061 6e64 2063 616e 2073  vents` and can s
+00009490: 6f6c 7665 2073 6f6d 6520 6576 656e 7473  olve some events
+000094a0: 2064 6570 656e 6465 6e63 6965 732e 2054   dependencies. T
+000094b0: 6865 2063 6f6c 6c65 6374 696f 6e20 6861  he collection ha
+000094c0: 7320 7369 6d69 6c61 7220 6665 6174 7572  s similar featur
+000094d0: 6573 206c 696b 6520 6120 7369 6e67 6c65  es like a single
+000094e0: 205f 4576 656e 7454 7265 655f 0a20 2020   _EventTree_.   
+000094f0: 2020 2020 2062 7574 2061 7070 6c79 696e       but applyin
+00009500: 6720 7468 656d 2066 6f72 2061 6c6c 205f  g them for all _
+00009510: 4576 656e 7454 7265 6573 5f2e 0a20 2020  EventTrees_..   
+00009520: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+00009530: 5061 7265 6e74 4576 656e 7454 7265 6543  ParentEventTreeC
+00009540: 6f6c 6c65 6374 696f 6e2a 2a20 6973 2061  ollection** is a
+00009550: 2063 6f6c 6c65 6374 696f 6e20 7369 6d69   collection simi
+00009560: 6c61 7220 746f 205f 4576 656e 7454 7265  lar to _EventTre
+00009570: 6543 6f6c 6c65 6374 696f 6e5f 2062 7574  eCollection_ but
+00009580: 2063 6f6e 7461 696e 696e 6720 6f6e 6c79   containing only
+00009590: 2070 6172 656e 7420 6576 656e 7473 2074   parent events t
+000095a0: 6861 740a 2020 2020 2020 2020 6172 6520  hat.        are 
+000095b0: 7265 6665 7265 6e63 6564 2069 6e20 7468  referenced in th
+000095c0: 6520 6461 7461 2073 7472 6561 6d2e 2054  e data stream. T
+000095d0: 6865 2063 6f6c 6c65 6374 696f 6e20 6861  he collection ha
+000095e0: 7320 6665 6174 7572 6573 2073 696d 696c  s features simil
+000095f0: 6172 2074 6f20 5f45 7665 6e74 5472 6565  ar to _EventTree
+00009600: 436f 6c6c 6563 7469 6f6e 5f2e 0a20 2020  Collection_..   
+00009610: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
+00009620: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
+00009630: 2020 2020 2020 2020 2a20 546f 2075 7365          * To use
+00009640: 2045 5420 636f 6c6c 6563 7469 6f6e 7320   ET collections 
+00009650: 796f 7520 6e65 6564 2074 6f20 696e 6974  you need to init
+00009660: 6961 6c69 7a65 2074 6865 6d20 6279 205f  ialize them by _
+00009670: 4554 4344 7269 7665 725f 2e20 4461 7461  ETCDriver_. Data
+00009680: 2073 6f75 7263 6573 2075 7375 616c 6c79   sources usually
+00009690: 2070 726f 7669 6465 2074 6865 6d2e 0a20   provide them.. 
+000096a0: 2020 2020 2020 2020 2059 6f75 2063 616e           You can
+000096b0: 2063 7265 6174 6520 6974 2062 7920 796f   create it by yo
+000096c0: 7572 7365 6c66 2064 6570 656e 6469 6e67  urself depending
+000096d0: 206f 6e20 796f 7572 2064 6174 6120 7374   on your data st
+000096e0: 7275 6374 7572 652e 0a20 2020 2020 2020  ructure..       
+000096f0: 202a 2054 6865 2063 6f6c 6c65 6374 696f   * The collectio
+00009700: 6e20 6861 7320 6120 6665 6174 7572 6520  n has a feature 
+00009710: 746f 2072 6563 6f76 6572 2065 7665 6e74  to recover event
+00009720: 732e 2041 6c6c 2065 7665 6e74 7320 7468  s. All events th
+00009730: 6174 2061 7265 206e 6f74 2069 6e20 7468  at are not in th
+00009740: 6520 7265 6365 6976 6564 2064 6174 6120  e received data 
+00009750: 7374 7265 616d 2c20 6275 7420 7768 6963  stream, but whic
+00009760: 6820 6172 650a 2020 2020 2020 2020 2020  h are.          
+00009770: 7265 6665 7265 6e63 6564 2077 696c 6c20  referenced will 
+00009780: 6265 206c 6f61 6465 6420 6672 6f6d 2074  be loaded from t
+00009790: 6865 2064 6174 6120 736f 7572 6365 2e0a  he data source..
+000097a0: 2020 2020 2020 2020 2a20 596f 7520 6361          * You ca
+000097b0: 6e20 7461 6b65 2060 6465 7461 6368 6564  n take `detached
+000097c0: 5f65 7665 6e74 7360 2074 6f20 7365 6520  _events` to see 
+000097d0: 7768 6963 6820 6576 656e 7473 2061 7265  which events are
+000097e0: 206d 6973 7369 6e67 2e0a 2020 2020 2020   missing..      
+000097f0: 2020 2a20 4966 2079 6f75 2077 616e 742c    * If you want,
+00009800: 2079 6f75 2063 616e 2062 7569 6c64 2070   you can build p
+00009810: 6172 656e 746c 6573 7320 7472 6565 7320  arentless trees 
+00009820: 7768 6572 6520 7468 6520 6d69 7373 696e  where the missin
+00009830: 6720 6576 656e 7473 2061 7265 2073 7475  g events are stu
+00009840: 6262 6564 2069 6e73 7465 6164 2e20 4a75  bbed instead. Ju
+00009850: 7374 0a20 2020 2020 2020 2020 2075 7365  st.          use
+00009860: 2060 6765 745f 7061 7265 6e74 6c65 7373   `get_parentless
+00009870: 5f74 7265 6573 2829 602e 0a20 2020 2020  _trees()`..     
+00009880: 2020 200a 2020 2020 2020 2020 5265 7175     .        Requ
+00009890: 6972 656d 656e 7473 3a0a 2020 2020 2020  irements:.      
+000098a0: 2020 0a20 2020 2020 2020 2031 2e20 4576    .        1. Ev
+000098b0: 656e 7473 2070 726f 7669 6465 6420 746f  ents provided to
+000098c0: 2045 5443 2068 6176 6520 746f 2068 6176   ETC have to hav
+000098d0: 6520 6065 7665 6e74 5f6e 616d 6560 2c20  e `event_name`, 
+000098e0: 6065 7665 6e74 5f69 6460 2c20 6070 6172  `event_id`, `par
+000098f0: 656e 745f 6576 656e 745f 6964 6020 6669  ent_event_id` fi
+00009900: 656c 6473 2e20 5468 6579 0a20 2020 2020  elds. They.     
+00009910: 2020 2063 616e 2068 6176 6520 616e 6f74     can have anot
+00009920: 6865 7220 6e61 6d65 7320 2869 7420 7265  her names (it re
+00009930: 736f 6c76 6573 2069 6e20 7468 6520 6472  solves in the dr
+00009940: 6976 6572 292e 0a20 2020 2020 2020 200a  iver)..        .
+00009950: 2020 2020 2020 2020 2323 2323 2048 696e          #### Hin
+00009960: 7473 0a20 2020 2020 2020 200a 2020 2020  ts.        .    
+00009970: 2020 2020 2a20 5265 6d6f 7665 2061 6c6c      * Remove all
+00009980: 2075 6e6e 6563 6573 7361 7279 2066 6965   unnecessary fie
+00009990: 6c64 7320 6672 6f6d 2065 7665 6e74 7320  lds from events 
+000099a0: 6265 666f 7265 2070 6173 7369 6e67 2074  before passing t
+000099b0: 6f20 6120 5f63 6f6c 6c65 6374 696f 6e5f  o a _collection_
+000099c0: 2074 6f20 7265 6475 6365 206d 656d 6f72   to reduce memor
+000099d0: 7920 7573 6167 652e 0a20 2020 2020 2020  y usage..       
+000099e0: 202a 2055 7365 2060 7368 6f77 2829 6020   * Use `show()` 
+000099f0: 6d65 7468 6f64 2074 6f20 7072 696e 7420  method to print 
+00009a00: 7468 6520 7472 6565 2069 6e20 7472 6565  the tree in tree
+00009a10: 2d6c 696b 6520 7669 6577 2e0a 2020 2020  -like view..    
+00009a20: 2020 2020 2a20 4e6f 7465 2074 6861 7420      * Note that 
+00009a30: 7468 6520 6067 6574 5f78 6020 6d65 7468  the `get_x` meth
+00009a40: 6f64 7320 7769 6c6c 2072 6169 7365 2061  ods will raise a
+00009a50: 6e20 6578 6365 7074 696f 6e20 6966 2079  n exception if y
+00009a60: 6f75 2070 6173 7320 616e 2075 6e6b 6e6f  ou pass an unkno
+00009a70: 776e 2065 7665 6e74 2069 642c 2075 6e6c  wn event id, unl
+00009a80: 696b 6520 7468 6520 6066 696e 645f 7860  ike the `find_x`
+00009a90: 206d 6574 686f 6473 2028 0a20 2020 2020   methods (.     
+00009aa0: 2020 2020 2074 6865 7920 7265 7475 726e       they return
+00009ab0: 204e 6f6e 6529 2e0a 2020 2020 2020 2020   None)..        
+00009ac0: 2a20 4966 2079 6f75 2077 616e 7420 746f  * If you want to
+00009ad0: 206b 6e6f 7720 7468 6174 2073 7065 6369   know that speci
+00009ae0: 6669 6564 2065 7665 6e74 2065 7869 7374  fied event exist
+00009af0: 732c 2075 7365 2074 6865 2070 7974 686f  s, use the pytho
+00009b00: 6e20 6069 6e60 206b 6579 776f 7264 2028  n `in` keyword (
+00009b10: 652e 672e 2060 2765 7665 6e74 2d69 6427  e.g. `'event-id'
+00009b20: 2069 6e20 6576 656e 7473 5f74 7265 6560   in events_tree`
+00009b30: 292e 0a20 2020 2020 2020 202a 2055 7365  )..        * Use
+00009b40: 2074 6865 2070 7974 686f 6e20 606c 656e   the python `len
+00009b50: 6020 6b65 7977 6f72 6420 746f 2067 6574  ` keyword to get
+00009b60: 2065 7665 6e74 7320 6e75 6d62 6572 2069   events number i
+00009b70: 6e20 7468 6520 7472 6565 2e0a 2020 2020  n the tree..    
+00009b80: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00009b90: 2046 6965 6c64 2052 6573 6f6c 7665 7273   Field Resolvers
+00009ba0: 0a20 2020 2020 2020 2049 6e74 6572 6661  .        Interfa
+00009bb0: 6365 2063 616e 2062 6520 666f 756e 6420  ce can be found 
+00009bc0: 696e 2060 7468 325f 6461 7461 5f73 6572  in `th2_data_ser
+00009bd0: 7669 6365 732f 696e 7465 7266 6163 6573  vices/interfaces
+00009be0: 2f75 7469 6c73 2f72 6573 6f6c 7665 722e  /utils/resolver.
+00009bf0: 7079 602e 2020 0a20 2020 2020 2020 2041  py`.  .        A
+00009c00: 6c6c 2064 6174 612d 736f 7572 6365 7320  ll data-sources 
+00009c10: 7368 6f75 6c64 2069 6d70 6c65 6d65 6e74  should implement
+00009c20: 2074 6865 6d2e 0a20 2020 2020 2020 200a   them..        .
+00009c30: 2020 2020 2020 2020 5468 6520 6964 6561          The idea
+00009c40: 206f 6620 7573 696e 6720 7265 736f 6c76   of using resolv
+00009c50: 6572 733a 0a20 2020 2020 2020 2049 7420  ers:.        It 
+00009c60: 736f 6c76 6573 2074 6865 2070 726f 626c  solves the probl
+00009c70: 656d 206f 6620 6861 7669 6e67 2061 2066  em of having a f
+00009c80: 6577 2044 6174 6153 6f75 7263 6573 2077  ew DataSources w
+00009c90: 6974 6820 7369 6d69 6c61 7220 6461 7461  ith similar data
+00009ca0: 2c0a 2020 2020 2020 2020 6275 7420 7769  ,.        but wi
+00009cb0: 7468 2064 6966 6665 7265 6e74 2077 6179  th different way
+00009cc0: 7320 746f 2067 6574 2069 742e 0a20 2020  s to get it..   
+00009cd0: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00009ce0: 6573 6520 636c 6173 7365 7320 7072 6f76  ese classes prov
+00009cf0: 6964 6520 796f 7520 6765 7474 6572 206d  ide you getter m
+00009d00: 6574 686f 6473 2e0a 2020 2020 2020 2020  ethods..        
+00009d10: 5573 696e 6720 7468 6573 6520 636c 6173  Using these clas
+00009d20: 7365 7320 616c 6c6f 7773 2079 6f75 2074  ses allows you t
+00009d30: 6f20 6672 6565 6c79 2073 7769 7463 6820  o freely switch 
+00009d40: 6265 7477 6565 6e20 6469 6666 6572 656e  between differen
+00009d50: 7420 6461 7461 0a20 2020 2020 2020 2066  t data.        f
+00009d60: 6f72 6d61 7473 2061 6e64 2064 6f6e 2774  ormats and don't
+00009d70: 2063 6861 6e67 6520 796f 7572 2063 6f64   change your cod
+00009d80: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+00009d90: 2020 2020 5265 736f 6c76 6572 7320 736f      Resolvers so
+00009da0: 6c76 6520 7468 6520 7072 6f62 6c65 6d20  lve the problem 
+00009db0: 6f66 2064 6174 612d 666f 726d 6174 206d  of data-format m
+00009dc0: 6967 7261 7469 6f6e 2e0a 2020 2020 2020  igration..      
+00009dd0: 2020 2d20 6669 656c 6473 2070 6c61 6365    - fields place
+00009de0: 2063 616e 2062 6520 6368 616e 6765 640a   can be changed.
+00009df0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
+00009e00: 206e 616d 6573 2063 616e 2062 6520 6368   names can be ch
+00009e10: 616e 6765 640a 2020 2020 2020 2020 0a20  anged.        . 
+00009e20: 2020 2020 2020 2052 6573 6f6c 7665 7273         Resolvers
+00009e30: 2063 616e 2077 6f72 6b20 6f6e 6c79 2077   can work only w
+00009e40: 6974 6820 6f6e 6520 6576 656e 742f 6d65  ith one event/me
+00009e50: 7373 6167 652e 0a20 2020 2020 2020 2049  ssage..        I
+00009e60: 7420 6d65 616e 732c 2069 6620 796f 7572  t means, if your
+00009e70: 206d 6573 7361 6765 2068 6173 2073 7562   message has sub
+00009e80: 2d6d 6573 7361 6765 7320 286c 696b 6520  -messages (like 
+00009e90: 7468 322d 6d65 7373 6167 6573 2069 6e20  th2-messages in 
+00009ea0: 6c77 6470 2920 6974 200a 2020 2020 2020  lwdp) it .      
+00009eb0: 2020 776f 6e27 7420 776f 726b 2c20 6265    won't work, be
+00009ec0: 6361 7573 6520 7265 736f 6c76 6572 2077  cause resolver w
+00009ed0: 696c 6c20 6e6f 7420 6b6e 6f77 2077 6974  ill not know wit
+00009ee0: 6820 7768 6963 6820 7375 622d 6d65 7373  h which sub-mess
+00009ef0: 6167 6520 7368 6f75 6c64 2069 7420 776f  age should it wo
+00009f00: 726b 2e20 0a20 2020 2020 2020 200a 2020  rk. .        .  
+00009f10: 2020 2020 2020 2a2a 576f 726b 6172 6f75        **Workarou
+00009f20: 6e64 2a2a 2020 0a20 2020 2020 2020 2031  nd**  .        1
+00009f30: 2e20 4578 7061 6e64 2061 6c6c 2079 6f75  . Expand all you
+00009f40: 7220 6d65 7373 6167 6573 202d 3e20 606e  r messages -> `n
+00009f50: 6577 5f64 203d 2079 6f75 725f 6461 7461  ew_d = your_data
+00009f60: 2e6d 6170 284d 6573 7361 6765 4669 656c  .map(MessageFiel
+00009f70: 6452 6573 6f6c 7665 722e 6578 7061 6e64  dResolver.expand
+00009f80: 5f6d 6573 7361 6765 2960 0a20 2020 2020  _message)`.     
+00009f90: 2020 2032 2e20 5573 6520 6045 7870 616e     2. Use `Expan
+00009fa0: 6465 644d 6573 7361 6765 4669 656c 6452  dedMessageFieldR
+00009fb0: 6573 6f6c 7665 7260 2069 6e73 7465 6164  esolver` instead
+00009fc0: 206f 6620 7573 7561 6c20 604d 6573 7361   of usual `Messa
+00009fd0: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
+00009fe0: 2077 6865 6e20 0a20 2020 2020 2020 2020   when .         
+00009ff0: 2020 2079 6f75 2074 616b 6520 6669 656c     you take fiel
+0000a000: 6473 2066 6f72 2065 7870 616e 6465 6420  ds for expanded 
+0000a010: 6d65 7373 6167 6573 2e0a 2020 2020 2020  messages..      
+0000a020: 2020 0a20 2020 2020 2020 202a 2a49 6d70    .        **Imp
+0000a030: 6c65 6d65 6e74 6174 696f 6e20 6164 7669  lementation advi
+0000a040: 6365 3a2a 2a0a 2020 2020 2020 2020 312e  ce:**.        1.
+0000a050: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000a060: 656e 7465 6445 7272 6f72 202d 2d20 6966  entedError -- if
+0000a070: 2079 6f75 7220 496d 706c 656d 656e 7461   your Implementa
+0000a080: 7469 6f6e 2064 6f65 736e 2774 2073 7570  tion doesn't sup
+0000a090: 706f 7274 2074 6869 7320 6765 7474 6572  port this getter
+0000a0a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a0b0: 2020 202a 2a50 6572 666f 726d 616e 6365     **Performance
+0000a0c0: 2069 6d70 6163 743a 2a2a 0a20 2020 2020   impact:**.     
+0000a0d0: 2020 202d 2049 7420 6120 6269 7420 736c     - It a bit sl
+0000a0e0: 6f77 6572 2074 6861 6e20 7573 696e 6720  ower than using 
+0000a0f0: 6e61 6b65 6420 6669 656c 6420 6163 6365  naked field acce
+0000a100: 7373 2060 6469 6374 5b27 6b65 7927 5d60  ss `dict['key']`
+0000a110: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a120: 2020 2023 2320 322e 342e 204c 696e 6b73     ## 2.4. Links
+0000a130: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a140: 2020 2d20 5b52 6570 6f72 7420 4461 7461    - [Report Data
+0000a150: 2050 726f 7669 6465 725d 2868 7474 7073   Provider](https
+0000a160: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+0000a170: 322d 6e65 742f 7468 322d 7270 742d 6461  2-net/th2-rpt-da
+0000a180: 7461 2d70 726f 7669 6465 7229 0a20 2020  ta-provider).   
+0000a190: 2020 2020 202d 205b 5468 3220 4461 7461       - [Th2 Data
+0000a1a0: 2053 6572 7669 6365 7320 5574 696c 735d   Services Utils]
+0000a1b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a1c0: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+0000a1d0: 6461 7461 2d73 6572 7669 6365 732d 7574  data-services-ut
+0000a1e0: 696c 7329 0a20 2020 2020 2020 200a 2020  ils).        .  
+0000a1f0: 2020 2020 2020 2320 332e 2042 6573 7420        # 3. Best 
+0000a200: 7072 6163 7469 6365 730a 2020 2020 2020  practices.      
+0000a210: 2020 4465 7065 6e64 696e 6720 6f6e 2068    Depending on h
+0000a220: 6f77 2079 6f75 2077 6f72 6b20 7769 7468  ow you work with
+0000a230: 2060 4461 7461 206f 626a 6563 7460 2c20   `Data object`, 
+0000a240: 6974 2063 616e 2062 6520 736c 6f77 206f  it can be slow o
+0000a250: 6620 6661 7374 2e0a 2020 2020 2020 2020  f fast..        
+0000a260: 4173 2077 6974 6820 6120 7265 6c61 7469  As with a relati
+0000a270: 6f6e 616c 2064 6174 6162 6173 652c 2079  onal database, y
+0000a280: 6f75 2063 616e 2077 7269 7465 2061 2071  ou can write a q
+0000a290: 7565 7279 2074 6861 7420 7769 6c6c 2072  uery that will r
+0000a2a0: 6574 7572 6e20 6461 7461 2073 6c6f 776c  eturn data slowl
+0000a2b0: 7920 6f72 2071 7569 636b 6c79 2c0a 2020  y or quickly,.  
+0000a2c0: 2020 2020 2020 7468 6520 7361 6d65 2077        the same w
+0000a2d0: 6865 6e20 776f 726b 696e 6720 7769 7468  hen working with
+0000a2e0: 2061 2060 4461 7461 206f 626a 6563 7460   a `Data object`
+0000a2f0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a300: 2020 2046 6f6c 6c6f 7720 7468 6520 7275     Follow the ru
+0000a310: 6c65 7320 746f 206d 616b 6520 796f 7572  les to make your
+0000a320: 2077 6f72 6b20 7769 7468 2044 6174 6120   work with Data 
+0000a330: 6f62 6a65 6374 2066 6173 743a 0a20 2020  object fast:.   
+0000a340: 2020 2020 2031 2e20 5573 6520 6044 6174       1. Use `Dat
+0000a350: 612e 7573 655f 6361 6368 6528 2960 2069  a.use_cache()` i
+0000a360: 6620 796f 7520 6974 6572 6174 6520 6461  f you iterate da
+0000a370: 7461 206d 6f72 6520 7468 616e 206f 6e65  ta more than one
+0000a380: 2074 696d 652e 0a20 2020 2020 2020 2032   time..        2
+0000a390: 2e20 5472 7920 746f 2064 6f6e 2774 2069  . Try to don't i
+0000a3a0: 7465 7261 7465 206f 6e65 2060 4461 7461  terate one `Data
+0000a3b0: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+0000a3c0: 7468 6520 6f74 6865 7220 6f6e 652e 0a20  the other one.. 
+0000a3d0: 2020 2020 2020 2020 2020 4966 2079 6f75            If you
+0000a3e0: 2073 686f 756c 6420 746f 2064 6f20 6974   should to do it
+0000a3f0: 2c20 7573 6520 7368 6f72 7420 6044 6174  , use short `Dat
+0000a400: 6120 6f62 6a65 6374 6020 6669 7273 7420  a object` first 
+0000a410: 616e 6420 6c6f 6e67 2060 4461 7461 206f  and long `Data o
+0000a420: 626a 6563 7460 2069 6e73 6964 6520 7468  bject` inside th
+0000a430: 6520 6c6f 6f70 2e0a 2020 2020 2020 2020  e loop..        
+0000a440: 2020 2049 7427 6c6c 2061 6c6c 6f77 2079     It'll allow y
+0000a450: 6f75 206f 7065 6e20 7468 6520 6361 6368  ou open the cach
+0000a460: 6520 6669 6c65 206f 7220 6372 6561 7465  e file or create
+0000a470: 2061 2072 6571 7565 7374 2074 6f20 6044   a request to `D
+0000a480: 6174 6120 736f 7572 6365 6020 6c65 7373  ata source` less
+0000a490: 206e 756d 6265 7220 6f66 2074 696d 6573   number of times
+0000a4a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a4b0: 2020 2023 2034 2e20 4f66 6669 6369 616c     # 4. Official
+0000a4c0: 2044 6174 6153 6f75 7263 6520 696d 706c   DataSource impl
+0000a4d0: 656d 656e 7461 7469 6f6e 730a 2020 2020  ementations.    
+0000a4e0: 2020 2020 0a20 2020 2020 2020 202d 205b      .        - [
+0000a4f0: 4c69 6768 7477 6569 6768 7420 4461 7461  Lightweight Data
+0000a500: 2050 726f 7669 6465 7220 4461 7461 2053   Provider Data S
+0000a510: 6f75 7263 655d 2868 7474 7073 3a2f 2f67  ource](https://g
+0000a520: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
+0000a530: 742f 7468 322d 6473 2d73 6f75 7263 652d  t/th2-ds-source-
+0000a540: 6c77 6470 290a 2020 2020 2020 2020 0a20  lwdp).        . 
+0000a550: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a560: 2320 352e 2041 5049 0a20 2020 2020 2020  # 5. API.       
+0000a570: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+0000a580: 2061 7265 206c 6f6f 6b69 6e67 2066 6f72   are looking for
+0000a590: 2063 6c61 7373 6573 2064 6573 6372 6970   classes descrip
+0000a5a0: 7469 6f6e 2073 6565 2074 6865 205b 4150  tion see the [AP
+0000a5b0: 4920 446f 6375 6d65 6e74 6174 696f 6e5d  I Documentation]
+0000a5c0: 2864 6f63 756d 656e 7461 7469 6f6e 2f61  (documentation/a
+0000a5d0: 7069 2f69 6e64 6578 2e6d 6429 2e0a 2020  pi/index.md)..  
+0000a5e0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000a5f0: 2036 2e20 4578 616d 706c 6573 0a20 2020   6. Examples.   
+0000a600: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+0000a610: 5b67 6574 5f73 7461 7274 6564 5f65 7861  [get_started_exa
+0000a620: 6d70 6c65 2e70 795d 2865 7861 6d70 6c65  mple.py](example
+0000a630: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
+0000a640: 616d 706c 652e 7079 290a 2020 2020 2020  ample.py).      
+0000a650: 2020 0a50 6c61 7466 6f72 6d3a 2055 4e4b    .Platform: UNK
+0000a660: 4e4f 574e 0a52 6571 7569 7265 732d 5079  NOWN.Requires-Py
+0000a670: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
+0000a680: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+0000a690: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+0000a6a0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
+0000a6b0: 7261 3a20 7264 700a 5072 6f76 6964 6573  ra: rdp.Provides
+0000a6c0: 2d45 7874 7261 3a20 7264 7035 0a50 726f  -Extra: rdp5.Pro
+0000a6d0: 7669 6465 732d 4578 7472 613a 2072 6470  vides-Extra: rdp
+0000a6e0: 360a 5072 6f76 6964 6573 2d45 7874 7261  6.Provides-Extra
+0000a6f0: 3a20 6c77 6470 0a50 726f 7669 6465 732d  : lwdp.Provides-
+0000a700: 4578 7472 613a 206c 7764 7031 0a50 726f  Extra: lwdp1.Pro
+0000a710: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
+0000a720: 7032 0a50 726f 7669 6465 732d 4578 7472  p2.Provides-Extr
+0000a730: 613a 206c 7764 7033 0a50 726f 7669 6465  a: lwdp3.Provide
+0000a740: 732d 4578 7472 613a 206c 7764 702d 6465  s-Extra: lwdp-de
+0000a750: 760a 5072 6f76 6964 6573 2d45 7874 7261  v.Provides-Extra
+0000a760: 3a20 7574 696c 732d 7270 742d 7669 6577  : utils-rpt-view
+0000a770: 6572 0a50 726f 7669 6465 732d 4578 7472  er.Provides-Extr
+0000a780: 613a 2075 7469 6c73 2d72 7074 2d76 6965  a: utils-rpt-vie
+0000a790: 7765 7235 0a50 726f 7669 6465 732d 4578  wer5.Provides-Ex
+0000a7a0: 7472 613a 2075 7469 6c73 2d61 6476 616e  tra: utils-advan
+0000a7b0: 6365 640a                                ced.
```

### Comparing `th2_data_services-2.0.0.dev9018014082/README.md` & `th2_data_services-2.0.0.dev9113174303/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -230,1962 +230,1971 @@
 00000e50: 7265 732e 0a0a 5b54 6865 2066 6f6c 6c6f  res...[The follo
 00000e60: 7769 6e67 2065 7861 6d70 6c65 2061 7320  wing example as 
 00000e70: 6120 6669 6c65 5d28 6578 616d 706c 6573  a file](examples
 00000e80: 2f67 6574 5f73 7461 7274 6564 5f65 7861  /get_started_exa
 00000e90: 6d70 6c65 2e70 7929 2e0a 0a3c 212d 2d20  mple.py)...<!-- 
 00000ea0: 7374 6172 7420 6765 745f 7374 6172 7465  start get_starte
 00000eb0: 645f 6578 616d 706c 652e 7079 202d 2d3e  d_example.py -->
-00000ec0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00000ed0: 7479 7069 6e67 2069 6d70 6f72 7420 5475  typing import Tu
-00000ee0: 706c 652c 204c 6973 742c 204f 7074 696f  ple, List, Optio
-00000ef0: 6e61 6c2c 2047 656e 6572 6174 6f72 0a66  nal, Generator.f
-00000f00: 726f 6d20 6461 7465 7469 6d65 2069 6d70  rom datetime imp
-00000f10: 6f72 7420 6461 7465 7469 6d65 0a0a 6672  ort datetime..fr
-00000f20: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00000f30: 6963 6573 2e64 6174 6120 696d 706f 7274  ices.data import
-00000f40: 2044 6174 610a 6672 6f6d 2074 6832 5f64   Data.from th2_d
-00000f50: 6174 615f 7365 7276 6963 6573 2e64 756d  ata_services.dum
-00000f60: 6d79 2069 6d70 6f72 7420 4475 6d6d 7944  my import DummyD
-00000f70: 6174 6153 6f75 7263 650a 6672 6f6d 2074  ataSource.from t
-00000f80: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00000f90: 2e65 7665 6e74 5f74 7265 6520 696d 706f  .event_tree impo
-00000fa0: 7274 2028 0a20 2020 2045 7665 6e74 5472  rt (.    EventTr
-00000fb0: 6565 2c0a 2020 2020 4576 656e 7454 7265  ee,.    EventTre
-00000fc0: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
-00000fd0: 2050 6172 656e 7445 7665 6e74 5472 6565   ParentEventTree
-00000fe0: 436f 6c6c 6563 7469 6f6e 2c0a 2020 2020  Collection,.    
-00000ff0: 4945 5443 4472 6976 6572 2c0a 290a 6672  IETCDriver,.).fr
-00001000: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00001010: 6963 6573 2e69 6e74 6572 6661 6365 7320  ices.interfaces 
-00001020: 696d 706f 7274 2049 4461 7461 536f 7572  import IDataSour
-00001030: 6365 0a66 726f 6d20 7468 325f 6461 7461  ce.from th2_data
-00001040: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
-00001050: 636f 6e76 6572 7465 7273 2069 6d70 6f72  converters impor
-00001060: 7420 280a 2020 2020 4461 7465 7469 6d65  t (.    Datetime
-00001070: 436f 6e76 6572 7465 722c 0a20 2020 2044  Converter,.    D
-00001080: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-00001090: 7665 7274 6572 2c0a 2020 2020 5072 6f74  verter,.    Prot
-000010a0: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
-000010b0: 7665 7274 6572 2c0a 2020 2020 5468 3254  verter,.    Th2T
-000010c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-000010d0: 722c 0a29 0a0a 2323 2323 2323 2323 2323  r,.)..##########
+00000ec0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000ed0: 2074 7970 696e 6720 696d 706f 7274 2054   typing import T
+00000ee0: 7570 6c65 2c20 4c69 7374 2c20 4f70 7469  uple, List, Opti
+00000ef0: 6f6e 616c 2c20 4765 6e65 7261 746f 720a  onal, Generator.
+00000f00: 6672 6f6d 2064 6174 6574 696d 6520 696d  from datetime im
+00000f10: 706f 7274 2064 6174 6574 696d 650a 0a66  port datetime..f
+00000f20: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00000f30: 7669 6365 732e 6461 7461 2069 6d70 6f72  vices.data impor
+00000f40: 7420 4461 7461 0a66 726f 6d20 7468 325f  t Data.from th2_
+00000f50: 6461 7461 5f73 6572 7669 6365 732e 6475  data_services.du
+00000f60: 6d6d 7920 696d 706f 7274 2044 756d 6d79  mmy import Dummy
+00000f70: 4461 7461 536f 7572 6365 0a66 726f 6d20  DataSource.from 
+00000f80: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
+00000f90: 732e 6576 656e 745f 7472 6565 2069 6d70  s.event_tree imp
+00000fa0: 6f72 7420 280a 2020 2020 4576 656e 7454  ort (.    EventT
+00000fb0: 7265 652c 0a20 2020 2045 7665 6e74 5472  ree,.    EventTr
+00000fc0: 6565 436f 6c6c 6563 7469 6f6e 2c0a 2020  eeCollection,.  
+00000fd0: 2020 5061 7265 6e74 4576 656e 7454 7265    ParentEventTre
+00000fe0: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
+00000ff0: 2049 4554 4344 7269 7665 722c 0a29 0a66   IETCDriver,.).f
+00001000: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001010: 7669 6365 732e 696e 7465 7266 6163 6573  vices.interfaces
+00001020: 2069 6d70 6f72 7420 4944 6174 6153 6f75   import IDataSou
+00001030: 7263 650a 6672 6f6d 2074 6832 5f64 6174  rce.from th2_dat
+00001040: 615f 7365 7276 6963 6573 2e75 7469 6c73  a_services.utils
+00001050: 2e63 6f6e 7665 7274 6572 7320 696d 706f  .converters impo
+00001060: 7274 2028 0a20 2020 2044 6174 6574 696d  rt (.    Datetim
+00001070: 6543 6f6e 7665 7274 6572 2c0a 2020 2020  eConverter,.    
+00001080: 4461 7465 7469 6d65 5374 7269 6e67 436f  DatetimeStringCo
+00001090: 6e76 6572 7465 722c 0a20 2020 2050 726f  nverter,.    Pro
+000010a0: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+000010b0: 6e76 6572 7465 722c 0a20 2020 2054 6832  nverter,.    Th2
+000010c0: 5469 6d65 7374 616d 7043 6f6e 7665 7274  TimestampConvert
+000010d0: 6572 2c0a 290a 0a23 2323 2323 2323 2323  er,.)..#########
 000010e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000010f0: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
-00001100: 305d 204c 6962 2063 6f6e 6669 6775 7261  0] Lib configura
-00001110: 7469 6f6e 0a23 2323 2323 2323 2323 2323  tion.###########
+000010f0: 2323 2323 2323 2323 2323 2323 230a 2320  #############.# 
+00001100: 5b30 5d20 4c69 6220 636f 6e66 6967 7572  [0] Lib configur
+00001110: 6174 696f 6e0a 2323 2323 2323 2323 2323  ation.##########
 00001120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001130: 2323 2323 2323 2323 2323 230a 0a23 205b  ###########..# [
-00001140: 302e 315d 2049 6e74 6572 6163 7469 7665  0.1] Interactive
-00001150: 206f 7220 5363 7269 7074 206d 6f64 650a   or Script mode.
-00001160: 2320 4966 2079 6f75 2075 7365 2074 6865  # If you use the
-00001170: 206c 6962 2069 6e20 696e 7465 7261 6374   lib in interact
-00001180: 6976 6520 6d6f 6465 2028 6a75 7079 7465  ive mode (jupyte
-00001190: 722c 2069 7079 7468 6f6e 2920 6974 2773  r, ipython) it's
-000011a0: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-000011b0: 7365 7420 7468 6520 7370 6563 6961 6c0a  set the special.
-000011c0: 2320 676c 6f62 616c 2070 6172 616d 6574  # global paramet
-000011d0: 6572 2074 6f20 5472 7565 2e20 4974 276c  er to True. It'l
-000011e0: 6c20 6b65 6570 2063 6163 6865 2066 696c  l keep cache fil
-000011f0: 6573 2069 6620 736f 6d65 7468 696e 6720  es if something 
-00001200: 7765 6e74 2077 726f 6e67 2e0a 6672 6f6d  went wrong..from
-00001210: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-00001220: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
-00001230: 206f 7074 696f 6e73 0a0a 6f70 7469 6f6e   options..option
-00001240: 732e 494e 5445 5241 4354 4956 455f 4d4f  s.INTERACTIVE_MO
-00001250: 4445 203d 2054 7275 650a 0a23 2053 6f6d  DE = True..# Som
-00001260: 6520 6578 616d 706c 6520 6461 7461 0a65  e example data.e
-00001270: 7665 6e74 7320 3d20 4461 7461 280a 2020  vents = Data(.  
-00001280: 2020 5b0a 2020 2020 2020 2020 7b0a 2020    [.        {.  
-00001290: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-000012a0: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
-000012b0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000012c0: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
-000012d0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-000012e0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-000012f0: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
-00001300: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-00001310: 6422 3a20 4e6f 6e65 2c0a 2020 2020 2020  d": None,.      
-00001320: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-00001330: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00001340: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
-00001350: 223a 2022 5365 7420 6f66 2061 7574 6f2d  ": "Set of auto-
-00001360: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
-00001370: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
-00001380: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
-00001390: 2020 2265 7665 6e74 5479 7065 223a 2022    "eventType": "
-000013a0: 6473 2d6c 6962 2d74 6573 742d 6576 656e  ds-lib-test-even
-000013b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000013c0: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
-000013d0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
-000013e0: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
-000013f0: 6f22 3a20 3536 3137 3531 3030 307d 2c0a  o": 561751000},.
-00001400: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00001410: 7274 5469 6d65 7374 616d 7022 3a20 7b22  rtTimestamp": {"
-00001420: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
-00001430: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
-00001440: 3a20 3536 3038 3733 3030 307d 2c0a 2020  : 560873000},.  
-00001450: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
-00001460: 7445 7665 6e74 4964 223a 204e 6f6e 652c  tEventId": None,
-00001470: 0a20 2020 2020 2020 2020 2020 2022 7375  .            "su
-00001480: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
-00001490: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
-000014a0: 6f6b 4964 223a 2022 6465 6d6f 5f62 6f6f  okId": "demo_boo
-000014b0: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
-000014c0: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
-000014d0: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
-000014e0: 2020 2020 2261 7474 6163 6865 644d 6573      "attachedMes
-000014f0: 7361 6765 4964 7322 3a20 5b5d 2c0a 2020  sageIds": [],.  
-00001500: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
-00001510: 3a20 5b5d 2c0a 2020 2020 2020 2020 7d2c  : [],.        },
-00001520: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00001530: 2020 2020 2020 2022 6576 656e 7449 6422         "eventId"
-00001540: 3a20 2264 656d 6f5f 626f 6f6b 5f31 3a74  : "demo_book_1:t
-00001550: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
-00001560: 3531 3335 3730 3535 3633 3532 3230 3030  5135705563522000
-00001570: 3a39 6164 6262 3365 302d 3566 3862 2d34  :9adbb3e0-5f8b-4
-00001580: 6332 382d 6132 6163 2d37 3336 3165 3866  c28-a2ac-7361e8f
-00001590: 6137 3034 633e 6465 6d6f 5f62 6f6f 6b5f  a704c>demo_book_
-000015a0: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
-000015b0: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
-000015c0: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
-000015d0: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
-000015e0: 3631 3535 3135 3264 5f32 222c 0a20 2020  6155152d_2",.   
-000015f0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-00001600: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-00001610: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001620: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
-00001630: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
-00001640: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
-00001650: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
-00001660: 2020 2020 2020 2269 7342 6174 6368 6564        "isBatched
-00001670: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00001680: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
-00001690: 3a20 2250 6c61 696e 2065 7665 6e74 2031  : "Plain event 1
-000016a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000016b0: 6576 656e 7454 7970 6522 3a20 2264 732d  eventType": "ds-
-000016c0: 6c69 622d 7465 7374 2d65 7665 6e74 222c  lib-test-event",
-000016d0: 0a20 2020 2020 2020 2020 2020 2022 656e  .            "en
-000016e0: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
-000016f0: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
-00001700: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
-00001710: 2035 3633 3634 3030 3030 7d2c 0a20 2020   563640000},.   
-00001720: 2020 2020 2020 2020 2022 7374 6172 7454           "startT
-00001730: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
-00001740: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-00001750: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
-00001760: 3633 3532 3230 3030 7d2c 0a20 2020 2020  63522000},.     
-00001770: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
-00001780: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001790: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-000017a0: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-000017b0: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-000017c0: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-000017d0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-000017e0: 2020 2020 2020 2020 2020 2020 2273 7563              "suc
-000017f0: 6365 7373 6675 6c22 3a20 5472 7565 2c0a  cessful": True,.
-00001800: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
-00001810: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
-00001820: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
-00001830: 2022 7363 6f70 6522 3a20 2274 6832 2d73   "scope": "th2-s
-00001840: 636f 7065 222c 0a20 2020 2020 2020 2020  cope",.         
-00001850: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
-00001860: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
-00001870: 2020 2020 2020 2020 2022 626f 6479 223a           "body":
-00001880: 207b 2274 7970 6522 3a20 226d 6573 7361   {"type": "messa
-00001890: 6765 222c 2022 6461 7461 223a 2022 6473  ge", "data": "ds
-000018a0: 2d6c 6962 2074 6573 7420 626f 6479 227d  -lib test body"}
-000018b0: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
-000018c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-000018d0: 2020 2022 6576 656e 7449 6422 3a20 2264     "eventId": "d
-000018e0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-000018f0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-00001900: 3730 3535 3633 3532 3230 3030 3a39 6164  705563522000:9ad
-00001910: 6262 3365 302d 3566 3862 2d34 6332 382d  bb3e0-5f8b-4c28-
-00001920: 6132 6163 2d37 3336 3165 3866 6137 3034  a2ac-7361e8fa704
-00001930: 633e 6465 6d6f 5f62 6f6f 6b5f 313a 7468  c>demo_book_1:th
-00001940: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001950: 3133 3537 3035 3536 3337 3537 3030 303a  135705563757000:
-00001960: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00001970: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-00001980: 3135 3264 5f33 222c 0a20 2020 2020 2020  152d_3",.       
-00001990: 2020 2020 2022 6261 7463 6849 6422 3a20       "batchId": 
-000019a0: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
-000019b0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-000019c0: 3335 3730 3535 3633 3532 3230 3030 3a39  35705563522000:9
-000019d0: 6164 6262 3365 302d 3566 3862 2d34 6332  adbb3e0-5f8b-4c2
-000019e0: 382d 6132 6163 2d37 3336 3165 3866 6137  8-a2ac-7361e8fa7
-000019f0: 3034 6322 2c0a 2020 2020 2020 2020 2020  04c",.          
-00001a00: 2020 2269 7342 6174 6368 6564 223a 2054    "isBatched": T
-00001a10: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00001a20: 2022 6576 656e 744e 616d 6522 3a20 2250   "eventName": "P
-00001a30: 6c61 696e 2065 7665 6e74 2032 222c 0a20  lain event 2",. 
-00001a40: 2020 2020 2020 2020 2020 2022 6576 656e             "even
-00001a50: 7454 7970 6522 3a20 2264 732d 6c69 622d  tType": "ds-lib-
-00001a60: 7465 7374 2d65 7665 6e74 222c 0a20 2020  test-event",.   
-00001a70: 2020 2020 2020 2020 2022 656e 6454 696d           "endTim
-00001a80: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
-00001a90: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
-00001aa0: 3032 352c 2022 6e61 6e6f 223a 2035 3633  025, "nano": 563
-00001ab0: 3739 3130 3030 7d2c 0a20 2020 2020 2020  791000},.       
-00001ac0: 2020 2020 2022 7374 6172 7454 696d 6573       "startTimes
-00001ad0: 7461 6d70 223a 207b 2265 706f 6368 5365  tamp": {"epochSe
-00001ae0: 636f 6e64 223a 2031 3637 3239 3237 3032  cond": 167292702
-00001af0: 352c 2022 6e61 6e6f 223a 2035 3633 3735  5, "nano": 56375
-00001b00: 3730 3030 7d2c 0a20 2020 2020 2020 2020  7000},.         
-00001b10: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
-00001b20: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
-00001b30: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001b40: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
-00001b50: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
-00001b60: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
-00001b70: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
-00001b80: 2020 2020 2020 2020 2273 7563 6365 7373          "success
-00001b90: 6675 6c22 3a20 5472 7565 2c0a 2020 2020  ful": True,.    
-00001ba0: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
-00001bb0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
-00001bc0: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
-00001bd0: 6f70 6522 3a20 2274 6832 2d73 636f 7065  ope": "th2-scope
-00001be0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001bf0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
-00001c00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
-00001c10: 2020 2020 2022 626f 6479 223a 207b 2274       "body": {"t
-00001c20: 7970 6522 3a20 226d 6573 7361 6765 222c  ype": "message",
-00001c30: 2022 6461 7461 223a 2022 6473 2d6c 6962   "data": "ds-lib
-00001c40: 2074 6573 7420 626f 6479 227d 2c0a 2020   test body"},.  
-00001c50: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001c60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00001c70: 6576 656e 7449 6422 3a20 2266 616b 652d  eventId": "fake-
-00001c80: 6576 656e 7449 6422 2c0a 2020 2020 2020  eventId",.      
-00001c90: 2020 2020 2020 2262 6174 6368 4964 223a        "batchId":
-00001ca0: 2022 6661 6b65 2d62 6174 6368 4964 222c   "fake-batchId",
-00001cb0: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
-00001cc0: 4261 7463 6865 6422 3a20 5472 7565 2c0a  Batched": True,.
-00001cd0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00001ce0: 6e74 4e61 6d65 223a 2022 4661 6b65 2065  ntName": "Fake e
-00001cf0: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
-00001d00: 2020 2022 6576 656e 7454 7970 6522 3a20     "eventType": 
-00001d10: 2264 732d 6c69 622d 7465 7374 2d65 7665  "ds-lib-test-eve
-00001d20: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-00001d30: 2022 656e 6454 696d 6573 7461 6d70 223a   "endTimestamp":
-00001d40: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-00001d50: 2031 3637 3239 3237 3033 352c 2022 6e61   1672927035, "na
-00001d60: 6e6f 223a 2035 3633 3739 3130 3030 7d2c  no": 563791000},
-00001d70: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
-00001d80: 6172 7454 696d 6573 7461 6d70 223a 207b  artTimestamp": {
-00001d90: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
-00001da0: 3637 3239 3237 3332 352c 2022 6e61 6e6f  672927325, "nano
-00001db0: 223a 2035 3633 3735 3730 3030 7d2c 0a20  ": 563757000},. 
-00001dc0: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
-00001dd0: 6e74 4576 656e 7449 6422 3a20 226e 6f74  ntEventId": "not
-00001de0: 5f65 7869 7374 735f 696e 5f74 6865 5f65  _exists_in_the_e
-00001df0: 7665 6e74 735f 7374 7265 616d 222c 0a20  vents_stream",. 
-00001e00: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
-00001e10: 6573 7366 756c 223a 2046 616c 7365 2c0a  essful": False,.
-00001e20: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
-00001e30: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
-00001e40: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
-00001e50: 2022 7363 6f70 6522 3a20 2274 6832 2d73   "scope": "th2-s
-00001e60: 636f 7065 222c 0a20 2020 2020 2020 2020  cope",.         
-00001e70: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
-00001e80: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
-00001e90: 2020 2020 2020 2020 2022 626f 6479 223a           "body":
-00001ea0: 207b 2274 7970 6522 3a20 226d 6573 7361   {"type": "messa
-00001eb0: 6765 222c 2022 6461 7461 223a 2022 6473  ge", "data": "ds
-00001ec0: 2d6c 6962 2074 6573 7420 626f 6479 227d  -lib test body"}
-00001ed0: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
-00001ee0: 205d 0a29 0a0a 2323 2323 2323 2323 2323   ].)..##########
+00001130: 2323 2323 2323 2323 2323 2323 0a0a 2320  ############..# 
+00001140: 5b30 2e31 5d20 496e 7465 7261 6374 6976  [0.1] Interactiv
+00001150: 6520 6f72 2053 6372 6970 7420 6d6f 6465  e or Script mode
+00001160: 0a23 2049 6620 796f 7520 7573 6520 7468  .# If you use th
+00001170: 6520 6c69 6220 696e 2069 6e74 6572 6163  e lib in interac
+00001180: 7469 7665 206d 6f64 6520 286a 7570 7974  tive mode (jupyt
+00001190: 6572 2c20 6970 7974 686f 6e29 2069 7427  er, ipython) it'
+000011a0: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
+000011b0: 2073 6574 2074 6865 2073 7065 6369 616c   set the special
+000011c0: 0a23 2067 6c6f 6261 6c20 7061 7261 6d65  .# global parame
+000011d0: 7465 7220 746f 2054 7275 652e 2049 7427  ter to True. It'
+000011e0: 6c6c 206b 6565 7020 6361 6368 6520 6669  ll keep cache fi
+000011f0: 6c65 7320 6966 2073 6f6d 6574 6869 6e67  les if something
+00001200: 2077 656e 7420 7772 6f6e 672e 0a66 726f   went wrong..fro
+00001210: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+00001220: 6365 732e 636f 6e66 6967 2069 6d70 6f72  ces.config impor
+00001230: 7420 6f70 7469 6f6e 730a 0a6f 7074 696f  t options..optio
+00001240: 6e73 2e49 4e54 4552 4143 5449 5645 5f4d  ns.INTERACTIVE_M
+00001250: 4f44 4520 3d20 5472 7565 0a0a 2320 536f  ODE = True..# So
+00001260: 6d65 2065 7861 6d70 6c65 2064 6174 610a  me example data.
+00001270: 6576 656e 7473 203d 2044 6174 6128 0a20  events = Data(. 
+00001280: 2020 205b 0a20 2020 2020 2020 207b 0a20     [.        {. 
+00001290: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+000012a0: 7449 6422 3a20 2264 656d 6f5f 626f 6f6b  tId": "demo_book
+000012b0: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+000012c0: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+000012d0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+000012e0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+000012f0: 6136 3135 3531 3532 645f 3122 2c0a 2020  a6155152d_1",.  
+00001300: 2020 2020 2020 2020 2020 2262 6174 6368            "batch
+00001310: 4964 223a 204e 6f6e 652c 0a20 2020 2020  Id": None,.     
+00001320: 2020 2020 2020 2022 6973 4261 7463 6865         "isBatche
+00001330: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
+00001340: 2020 2020 2020 2022 6576 656e 744e 616d         "eventNam
+00001350: 6522 3a20 2253 6574 206f 6620 6175 746f  e": "Set of auto
+00001360: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
+00001370: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
+00001380: 7469 6e67 222c 0a20 2020 2020 2020 2020  ting",.         
+00001390: 2020 2022 6576 656e 7454 7970 6522 3a20     "eventType": 
+000013a0: 2264 732d 6c69 622d 7465 7374 2d65 7665  "ds-lib-test-eve
+000013b0: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+000013c0: 2022 656e 6454 696d 6573 7461 6d70 223a   "endTimestamp":
+000013d0: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
+000013e0: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
+000013f0: 6e6f 223a 2035 3631 3735 3130 3030 7d2c  no": 561751000},
+00001400: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
+00001410: 6172 7454 696d 6573 7461 6d70 223a 207b  artTimestamp": {
+00001420: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001430: 3637 3239 3237 3032 352c 2022 6e61 6e6f  672927025, "nano
+00001440: 223a 2035 3630 3837 3330 3030 7d2c 0a20  ": 560873000},. 
+00001450: 2020 2020 2020 2020 2020 2022 7061 7265             "pare
+00001460: 6e74 4576 656e 7449 6422 3a20 4e6f 6e65  ntEventId": None
+00001470: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00001480: 7563 6365 7373 6675 6c22 3a20 5472 7565  uccessful": True
+00001490: 2c0a 2020 2020 2020 2020 2020 2020 2262  ,.            "b
+000014a0: 6f6f 6b49 6422 3a20 2264 656d 6f5f 626f  ookId": "demo_bo
+000014b0: 6f6b 5f31 222c 0a20 2020 2020 2020 2020  ok_1",.         
+000014c0: 2020 2022 7363 6f70 6522 3a20 2274 6832     "scope": "th2
+000014d0: 2d73 636f 7065 222c 0a20 2020 2020 2020  -scope",.       
+000014e0: 2020 2020 2022 6174 7461 6368 6564 4d65       "attachedMe
+000014f0: 7373 6167 6549 6473 223a 205b 5d2c 0a20  ssageIds": [],. 
+00001500: 2020 2020 2020 2020 2020 2022 626f 6479             "body
+00001510: 223a 205b 5d2c 0a20 2020 2020 2020 207d  ": [],.        }
+00001520: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+00001530: 2020 2020 2020 2020 2265 7665 6e74 4964          "eventId
+00001540: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 313a  ": "demo_book_1:
+00001550: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
+00001560: 3035 3133 3537 3035 3536 3335 3232 3030  0513570556352200
+00001570: 303a 3961 6462 6233 6530 2d35 6638 622d  0:9adbb3e0-5f8b-
+00001580: 3463 3238 2d61 3261 632d 3733 3631 6538  4c28-a2ac-7361e8
+00001590: 6661 3730 3463 3e64 656d 6f5f 626f 6f6b  fa704c>demo_book
+000015a0: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+000015b0: 3330 3130 3531 3335 3730 3535 3633 3532  3010513570556352
+000015c0: 3230 3030 3a64 3631 6539 3330 612d 3864  2000:d61e930a-8d
+000015d0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+000015e0: 6136 3135 3531 3532 645f 3222 2c0a 2020  a6155152d_2",.  
+000015f0: 2020 2020 2020 2020 2020 2262 6174 6368            "batch
+00001600: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
+00001610: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
+00001620: 3031 3035 3133 3537 3035 3536 3335 3232  0105135705563522
+00001630: 3030 303a 3961 6462 6233 6530 2d35 6638  000:9adbb3e0-5f8
+00001640: 622d 3463 3238 2d61 3261 632d 3733 3631  b-4c28-a2ac-7361
+00001650: 6538 6661 3730 3463 222c 0a20 2020 2020  e8fa704c",.     
+00001660: 2020 2020 2020 2022 6973 4261 7463 6865         "isBatche
+00001670: 6422 3a20 5472 7565 2c0a 2020 2020 2020  d": True,.      
+00001680: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
+00001690: 223a 2022 506c 6169 6e20 6576 656e 7420  ": "Plain event 
+000016a0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+000016b0: 2265 7665 6e74 5479 7065 223a 2022 6473  "eventType": "ds
+000016c0: 2d6c 6962 2d74 6573 742d 6576 656e 7422  -lib-test-event"
+000016d0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+000016e0: 6e64 5469 6d65 7374 616d 7022 3a20 7b22  ndTimestamp": {"
+000016f0: 6570 6f63 6853 6563 6f6e 6422 3a20 3136  epochSecond": 16
+00001700: 3732 3932 3730 3235 2c20 226e 616e 6f22  72927025, "nano"
+00001710: 3a20 3536 3336 3430 3030 307d 2c0a 2020  : 563640000},.  
+00001720: 2020 2020 2020 2020 2020 2273 7461 7274            "start
+00001730: 5469 6d65 7374 616d 7022 3a20 7b22 6570  Timestamp": {"ep
+00001740: 6f63 6853 6563 6f6e 6422 3a20 3136 3732  ochSecond": 1672
+00001750: 3932 3730 3235 2c20 226e 616e 6f22 3a20  927025, "nano": 
+00001760: 3536 3335 3232 3030 307d 2c0a 2020 2020  563522000},.    
+00001770: 2020 2020 2020 2020 2270 6172 656e 7445          "parentE
+00001780: 7665 6e74 4964 223a 2022 6465 6d6f 5f62  ventId": "demo_b
+00001790: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+000017a0: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+000017b0: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+000017c0: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+000017d0: 6433 3461 3631 3535 3135 3264 5f31 222c  d34a6155152d_1",
+000017e0: 0a20 2020 2020 2020 2020 2020 2022 7375  .            "su
+000017f0: 6363 6573 7366 756c 223a 2054 7275 652c  ccessful": True,
+00001800: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
+00001810: 6f6b 4964 223a 2022 6465 6d6f 5f62 6f6f  okId": "demo_boo
+00001820: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
+00001830: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
+00001840: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
+00001850: 2020 2020 2261 7474 6163 6865 644d 6573      "attachedMes
+00001860: 7361 6765 4964 7322 3a20 5b5d 2c0a 2020  sageIds": [],.  
+00001870: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
+00001880: 3a20 7b22 7479 7065 223a 2022 6d65 7373  : {"type": "mess
+00001890: 6167 6522 2c20 2264 6174 6122 3a20 2264  age", "data": "d
+000018a0: 732d 6c69 6220 7465 7374 2062 6f64 7922  s-lib test body"
+000018b0: 7d2c 0a20 2020 2020 2020 207d 2c0a 2020  },.        },.  
+000018c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000018d0: 2020 2020 2265 7665 6e74 4964 223a 2022      "eventId": "
+000018e0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+000018f0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+00001900: 3537 3035 3536 3335 3232 3030 303a 3961  5705563522000:9a
+00001910: 6462 6233 6530 2d35 6638 622d 3463 3238  dbb3e0-5f8b-4c28
+00001920: 2d61 3261 632d 3733 3631 6538 6661 3730  -a2ac-7361e8fa70
+00001930: 3463 3e64 656d 6f5f 626f 6f6b 5f31 3a74  4c>demo_book_1:t
+00001940: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+00001950: 3531 3335 3730 3535 3633 3735 3730 3030  5135705563757000
+00001960: 3a64 3631 6539 3330 612d 3864 3030 2d31  :d61e930a-8d00-1
+00001970: 3165 642d 6161 3161 2d64 3334 6136 3135  1ed-aa1a-d34a615
+00001980: 3531 3532 645f 3322 2c0a 2020 2020 2020  5152d_3",.      
+00001990: 2020 2020 2020 2262 6174 6368 4964 223a        "batchId":
+000019a0: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+000019b0: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+000019c0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
+000019d0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
+000019e0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
+000019f0: 3730 3463 222c 0a20 2020 2020 2020 2020  704c",.         
+00001a00: 2020 2022 6973 4261 7463 6865 6422 3a20     "isBatched": 
+00001a10: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00001a20: 2020 2265 7665 6e74 4e61 6d65 223a 2022    "eventName": "
+00001a30: 506c 6169 6e20 6576 656e 7420 3222 2c0a  Plain event 2",.
+00001a40: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00001a50: 6e74 5479 7065 223a 2022 6473 2d6c 6962  ntType": "ds-lib
+00001a60: 2d74 6573 742d 6576 656e 7422 2c0a 2020  -test-event",.  
+00001a70: 2020 2020 2020 2020 2020 2265 6e64 5469            "endTi
+00001a80: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+00001a90: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+00001aa0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+00001ab0: 3337 3931 3030 307d 2c0a 2020 2020 2020  3791000},.      
+00001ac0: 2020 2020 2020 2273 7461 7274 5469 6d65        "startTime
+00001ad0: 7374 616d 7022 3a20 7b22 6570 6f63 6853  stamp": {"epochS
+00001ae0: 6563 6f6e 6422 3a20 3136 3732 3932 3730  econd": 16729270
+00001af0: 3235 2c20 226e 616e 6f22 3a20 3536 3337  25, "nano": 5637
+00001b00: 3537 3030 307d 2c0a 2020 2020 2020 2020  57000},.        
+00001b10: 2020 2020 2270 6172 656e 7445 7665 6e74      "parentEvent
+00001b20: 4964 223a 2022 6465 6d6f 5f62 6f6f 6b5f  Id": "demo_book_
+00001b30: 313a 7468 322d 7363 6f70 653a 3230 3233  1:th2-scope:2023
+00001b40: 3031 3035 3133 3537 3035 3536 3038 3733  0105135705560873
+00001b50: 3030 303a 6436 3165 3933 3061 2d38 6430  000:d61e930a-8d0
+00001b60: 302d 3131 6564 2d61 6131 612d 6433 3461  0-11ed-aa1a-d34a
+00001b70: 3631 3535 3135 3264 5f31 222c 0a20 2020  6155152d_1",.   
+00001b80: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
+00001b90: 7366 756c 223a 2054 7275 652c 0a20 2020  sful": True,.   
+00001ba0: 2020 2020 2020 2020 2022 626f 6f6b 4964           "bookId
+00001bb0: 223a 2022 6465 6d6f 5f62 6f6f 6b5f 3122  ": "demo_book_1"
+00001bc0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00001bd0: 636f 7065 223a 2022 7468 322d 7363 6f70  cope": "th2-scop
+00001be0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001bf0: 2261 7474 6163 6865 644d 6573 7361 6765  "attachedMessage
+00001c00: 4964 7322 3a20 5b5d 2c0a 2020 2020 2020  Ids": [],.      
+00001c10: 2020 2020 2020 2262 6f64 7922 3a20 7b22        "body": {"
+00001c20: 7479 7065 223a 2022 6d65 7373 6167 6522  type": "message"
+00001c30: 2c20 2264 6174 6122 3a20 2264 732d 6c69  , "data": "ds-li
+00001c40: 6220 7465 7374 2062 6f64 7922 7d2c 0a20  b test body"},. 
+00001c50: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001c60: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00001c70: 2265 7665 6e74 4964 223a 2022 6661 6b65  "eventId": "fake
+00001c80: 2d65 7665 6e74 4964 222c 0a20 2020 2020  -eventId",.     
+00001c90: 2020 2020 2020 2022 6261 7463 6849 6422         "batchId"
+00001ca0: 3a20 2266 616b 652d 6261 7463 6849 6422  : "fake-batchId"
+00001cb0: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+00001cc0: 7342 6174 6368 6564 223a 2054 7275 652c  sBatched": True,
+00001cd0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00001ce0: 656e 744e 616d 6522 3a20 2246 616b 6520  entName": "Fake 
+00001cf0: 6576 656e 7422 2c0a 2020 2020 2020 2020  event",.        
+00001d00: 2020 2020 2265 7665 6e74 5479 7065 223a      "eventType":
+00001d10: 2022 6473 2d6c 6962 2d74 6573 742d 6576   "ds-lib-test-ev
+00001d20: 656e 7422 2c0a 2020 2020 2020 2020 2020  ent",.          
+00001d30: 2020 2265 6e64 5469 6d65 7374 616d 7022    "endTimestamp"
+00001d40: 3a20 7b22 6570 6f63 6853 6563 6f6e 6422  : {"epochSecond"
+00001d50: 3a20 3136 3732 3932 3730 3335 2c20 226e  : 1672927035, "n
+00001d60: 616e 6f22 3a20 3536 3337 3931 3030 307d  ano": 563791000}
+00001d70: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00001d80: 7461 7274 5469 6d65 7374 616d 7022 3a20  tartTimestamp": 
+00001d90: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+00001da0: 3136 3732 3932 3733 3235 2c20 226e 616e  1672927325, "nan
+00001db0: 6f22 3a20 3536 3337 3537 3030 307d 2c0a  o": 563757000},.
+00001dc0: 2020 2020 2020 2020 2020 2020 2270 6172              "par
+00001dd0: 656e 7445 7665 6e74 4964 223a 2022 6e6f  entEventId": "no
+00001de0: 745f 6578 6973 7473 5f69 6e5f 7468 655f  t_exists_in_the_
+00001df0: 6576 656e 7473 5f73 7472 6561 6d22 2c0a  events_stream",.
+00001e00: 2020 2020 2020 2020 2020 2020 2273 7563              "suc
+00001e10: 6365 7373 6675 6c22 3a20 4661 6c73 652c  cessful": False,
+00001e20: 0a20 2020 2020 2020 2020 2020 2022 626f  .            "bo
+00001e30: 6f6b 4964 223a 2022 6465 6d6f 5f62 6f6f  okId": "demo_boo
+00001e40: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
+00001e50: 2020 2273 636f 7065 223a 2022 7468 322d    "scope": "th2-
+00001e60: 7363 6f70 6522 2c0a 2020 2020 2020 2020  scope",.        
+00001e70: 2020 2020 2261 7474 6163 6865 644d 6573      "attachedMes
+00001e80: 7361 6765 4964 7322 3a20 5b5d 2c0a 2020  sageIds": [],.  
+00001e90: 2020 2020 2020 2020 2020 2262 6f64 7922            "body"
+00001ea0: 3a20 7b22 7479 7065 223a 2022 6d65 7373  : {"type": "mess
+00001eb0: 6167 6522 2c20 2264 6174 6122 3a20 2264  age", "data": "d
+00001ec0: 732d 6c69 6220 7465 7374 2062 6f64 7922  s-lib test body"
+00001ed0: 7d2c 0a20 2020 2020 2020 207d 2c0a 2020  },.        },.  
+00001ee0: 2020 5d0a 290a 0a23 2323 2323 2323 2323    ].)..#########
 00001ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001f00: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
-00001f10: 315d 2057 6f72 6b69 6e67 2077 6974 6820  1] Working with 
-00001f20: 6120 4461 7461 206f 626a 6563 742e 0a23  a Data object..#
+00001f00: 2323 2323 2323 2323 2323 2323 230a 2320  #############.# 
+00001f10: 5b31 5d20 576f 726b 696e 6720 7769 7468  [1] Working with
+00001f20: 2061 2044 6174 6120 6f62 6a65 6374 2e0a   a Data object..
 00001f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00001f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001f50: 2323 2323 230a 0a23 205b 312e 315d 2046  #####..# [1.1] F
-00001f60: 696c 7465 722e 0a66 696c 7465 7265 645f  ilter..filtered_
-00001f70: 6576 656e 7473 3a20 4461 7461 203d 2065  events: Data = e
-00001f80: 7665 6e74 732e 6669 6c74 6572 286c 616d  vents.filter(lam
-00001f90: 6264 6120 653a 2065 5b22 626f 6479 225d  bda e: e["body"]
-00001fa0: 2021 3d20 5b5d 2920 2023 2046 696c 7465   != [])  # Filte
-00001fb0: 7220 6576 656e 7473 2077 6974 6820 656d  r events with em
-00001fc0: 7074 7920 626f 6479 2e0a 0a0a 2320 5b31  pty body....# [1
-00001fd0: 2e32 5d20 4d61 702e 0a64 6566 2074 7261  .2] Map..def tra
-00001fe0: 6e73 666f 726d 5f66 756e 6374 696f 6e28  nsform_function(
-00001ff0: 7265 636f 7264 293a 0a20 2020 2072 6574  record):.    ret
-00002000: 7572 6e20 7b22 6576 656e 744e 616d 6522  urn {"eventName"
-00002010: 3a20 7265 636f 7264 5b22 6576 656e 744e  : record["eventN
-00002020: 616d 6522 5d2c 2022 7375 6363 6573 7366  ame"], "successf
-00002030: 756c 223a 2072 6563 6f72 645b 2273 7563  ul": record["suc
-00002040: 6365 7373 6675 6c22 5d7d 0a0a 0a66 696c  cessful"]}...fil
-00002050: 7465 7265 645f 616e 645f 6d61 7070 6564  tered_and_mapped
-00002060: 5f65 7665 6e74 7320 3d20 6669 6c74 6572  _events = filter
-00002070: 6564 5f65 7665 6e74 732e 6d61 7028 7472  ed_events.map(tr
-00002080: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
-00002090: 290a 0a23 205b 312e 335d 2044 6174 6120  )..# [1.3] Data 
-000020a0: 7069 7065 6c69 6e65 2e0a 2320 2020 2020  pipeline..#     
-000020b0: 2020 496e 7374 6561 6420 6f66 2064 6f69    Instead of doi
-000020c0: 6e67 2064 6174 6120 7472 616e 7366 6f72  ng data transfor
-000020d0: 6d61 7469 6f6e 7320 7374 6570 2062 7920  mations step by 
-000020e0: 7374 6570 2079 6f75 2063 616e 2064 6f20  step you can do 
-000020f0: 6974 2069 6e20 6f6e 6520 6c69 6e65 2e0a  it in one line..
-00002100: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
-00002110: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
-00002120: 7065 6c69 6e65 203d 2065 7665 6e74 732e  peline = events.
-00002130: 6669 6c74 6572 286c 616d 6264 6120 653a  filter(lambda e:
-00002140: 2065 5b22 626f 6479 225d 2021 3d20 5b5d   e["body"] != []
-00002150: 292e 6d61 7028 0a20 2020 2074 7261 6e73  ).map(.    trans
-00002160: 666f 726d 5f66 756e 6374 696f 6e0a 290a  form_function.).
-00002170: 2320 436f 6e74 656e 7420 6f66 2074 6865  # Content of the
-00002180: 7365 2074 776f 2044 6174 6120 6f62 6a65  se two Data obje
-00002190: 6374 7320 7368 6f75 6c64 2062 6520 6571  cts should be eq
-000021a0: 7561 6c2e 0a61 7373 6572 7420 6c69 7374  ual..assert list
-000021b0: 2866 696c 7465 7265 645f 616e 645f 6d61  (filtered_and_ma
-000021c0: 7070 6564 5f65 7665 6e74 7329 203d 3d20  pped_events) == 
-000021d0: 6c69 7374 2866 696c 7465 7265 645f 616e  list(filtered_an
-000021e0: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
-000021f0: 6279 5f70 6970 656c 696e 6529 0a0a 2320  by_pipeline)..# 
-00002200: 5b31 2e34 5d20 5369 6674 2e20 536b 6970  [1.4] Sift. Skip
-00002210: 2074 6865 2066 6972 7374 2066 6577 2069   the first few i
-00002220: 7465 6d73 206f 7220 6c69 6d69 7420 7468  tems or limit th
-00002230: 656d 2e0a 6461 7461 203d 2044 6174 6128  em..data = Data(
-00002240: 5b31 2c20 322c 2033 2c20 342c 2035 2c20  [1, 2, 3, 4, 5, 
-00002250: 362c 2037 2c20 382c 2039 2c20 3130 2c20  6, 7, 8, 9, 10, 
-00002260: 3131 2c20 3132 2c20 3133 2c20 3134 2c20  11, 12, 13, 14, 
-00002270: 3135 5d29 0a69 7465 6d73 5f66 726f 6d5f  15]).items_from_
-00002280: 3131 5f74 6f5f 656e 643a 2047 656e 6572  11_to_end: Gener
-00002290: 6174 6f72 203d 2064 6174 612e 7369 6674  ator = data.sift
-000022a0: 2873 6b69 703d 3130 290a 6f6e 6c79 5f66  (skip=10).only_f
-000022b0: 6972 7374 5f31 305f 6974 656d 733a 2047  irst_10_items: G
-000022c0: 656e 6572 6174 6f72 203d 2064 6174 612e  enerator = data.
-000022d0: 7369 6674 286c 696d 6974 3d31 3029 0a0a  sift(limit=10)..
-000022e0: 2320 5b31 2e35 5d20 4368 616e 6769 6e67  # [1.5] Changing
-000022f0: 2063 6163 6865 2073 7461 7475 732e 0a65   cache status..e
-00002300: 7665 6e74 732e 7573 655f 6361 6368 6528  vents.use_cache(
-00002310: 5472 7565 290a 2320 6f72 206a 7573 740a  True).# or just.
-00002320: 6576 656e 7473 2e75 7365 5f63 6163 6865  events.use_cache
-00002330: 2829 2020 2320 4966 2079 6f75 2077 616e  ()  # If you wan
-00002340: 7420 746f 2061 6374 6976 6174 6520 6361  t to activate ca
-00002350: 6368 652e 0a23 205b 312e 365d 2057 616c  che..# [1.6] Wal
-00002360: 6b20 7468 726f 7567 6820 6461 7461 2e0a  k through data..
-00002370: 666f 7220 6576 656e 7420 696e 2065 7665  for event in eve
-00002380: 6e74 733a 0a20 2020 2023 2044 6f20 736f  nts:.    # Do so
-00002390: 6d65 7468 696e 6720 7769 7468 2065 7665  mething with eve
-000023a0: 6e74 2028 6576 656e 7420 6973 2061 2064  nt (event is a d
-000023b0: 6963 7429 2e0a 2020 2020 7072 696e 7428  ict)..    print(
-000023c0: 6576 656e 7429 0a23 2041 6674 6572 2066  event).# After f
-000023d0: 6972 7374 2069 7465 7261 7469 6f6e 2074  irst iteration t
-000023e0: 6865 2065 7665 6e74 7320 6861 7320 6120  he events has a 
-000023f0: 6361 6368 6520 6669 6c65 2e0a 2320 4e6f  cache file..# No
-00002400: 7720 7468 6579 2077 696c 6c20 6265 2075  w they will be u
-00002410: 7365 6420 696e 2074 6865 2063 6163 6865  sed in the cache
-00002420: 2069 6e20 7468 6520 6e65 7874 2069 7465   in the next ite
-00002430: 7261 7469 6f6e 2e0a 0a23 205b 312e 375d  ration...# [1.7]
-00002440: 2047 6574 206e 756d 6265 7220 6f66 2074   Get number of t
-00002450: 6865 2065 6c65 6d65 6e74 7320 696e 2074  he elements in t
-00002460: 6865 2044 6174 6120 6f62 6a65 6374 2e0a  he Data object..
-00002470: 6e75 6d62 6572 5f6f 665f 6576 656e 7473  number_of_events
-00002480: 203d 2065 7665 6e74 732e 6c65 6e0a 0a23   = events.len..#
-00002490: 205b 312e 385d 2043 6865 636b 2074 6861   [1.8] Check tha
-000024a0: 7420 4461 7461 206f 626a 6563 7420 6973  t Data object is
-000024b0: 6e27 7420 656d 7074 792e 0a23 2054 6865  n't empty..# The
-000024c0: 2064 6174 6120 736f 7572 6365 2073 686f   data source sho
-000024d0: 756c 6420 6265 206e 6f74 2065 6d70 7479  uld be not empty
-000024e0: 2e0a 6173 7365 7274 2065 7665 6e74 732e  ..assert events.
-000024f0: 6973 5f65 6d70 7479 2069 7320 4661 6c73  is_empty is Fals
-00002500: 650a 0a23 205b 312e 395d 2043 6f6e 7665  e..# [1.9] Conve
-00002510: 7274 2044 6174 6120 6f62 6a65 6374 2074  rt Data object t
-00002520: 6f20 7468 6520 6c69 7374 206f 6620 656c  o the list of el
-00002530: 656d 656e 7473 2865 7665 6e74 7320 6f72  ements(events or
-00002540: 206d 6573 7361 6765 7329 2e0a 2320 4265   messages)..# Be
-00002550: 2063 6172 6566 756c 2c20 7468 6973 2063   careful, this c
-00002560: 616e 2074 616b 6520 746f 6f20 6d75 6368  an take too much
-00002570: 206d 656d 6f72 792e 0a65 7665 6e74 735f   memory..events_
-00002580: 6c69 7374 203d 206c 6973 7428 6576 656e  list = list(even
-00002590: 7473 290a 0a23 205b 312e 3130 5d20 5468  ts)..# [1.10] Th
-000025a0: 6520 6361 6368 6520 696e 6865 7269 7461  e cache inherita
-000025b0: 6e63 652e 0a23 2043 7265 6174 6573 2061  nce..# Creates a
-000025c0: 206e 6577 2044 6174 6120 6f62 6a65 6374   new Data object
-000025d0: 2074 6861 7420 7769 6c6c 2075 7365 2063   that will use c
-000025e0: 6163 6865 2066 726f 6d20 7468 6520 6576  ache from the ev
-000025f0: 656e 7473 2044 6174 6120 6f62 6a65 6374  ents Data object
-00002600: 2e0a 6576 656e 7473 5f66 696c 7465 7265  ..events_filtere
-00002610: 643a 2044 6174 6120 3d20 6576 656e 7473  d: Data = events
-00002620: 2e66 696c 7465 7228 6c61 6d62 6461 2072  .filter(lambda r
-00002630: 6563 6f72 643a 2072 6563 6f72 642e 6765  ecord: record.ge
-00002640: 7428 2262 6174 6368 4964 2229 290a 0a23  t("batchId"))..#
-00002650: 204e 6577 2044 6174 6120 6f62 6a65 6374   New Data object
-00002660: 7320 646f 6e27 7420 7573 6520 7468 6569  s don't use thei
-00002670: 7220 6f77 6e20 6361 6368 6520 6279 2064  r own cache by d
-00002680: 6566 6175 6c74 2062 7574 2075 7365 2074  efault but use t
-00002690: 6865 2063 6163 6865 206f 6620 7468 6520  he cache of the 
-000026a0: 7061 7265 6e74 2044 6174 6120 6f62 6a65  parent Data obje
-000026b0: 6374 2e0a 2320 5573 6520 7573 655f 6361  ct..# Use use_ca
-000026c0: 6368 6520 6d65 7468 6f64 2074 6f20 6163  che method to ac
-000026d0: 7469 7661 7465 2063 6163 6869 6e67 2e0a  tivate caching..
-000026e0: 2320 4166 7465 7220 7468 6174 2c20 7468  # After that, th
-000026f0: 6520 4461 7461 206f 626a 6563 7420 7769  e Data object wi
-00002700: 6c6c 2063 7265 6174 6520 6974 7320 6f77  ll create its ow
-00002710: 6e20 6361 6368 6520 6669 6c65 2e0a 6576  n cache file..ev
-00002720: 656e 7473 5f66 696c 7465 7265 642e 7573  ents_filtered.us
-00002730: 655f 6361 6368 6528 290a 0a6c 6973 7428  e_cache()..list(
-00002740: 6576 656e 7473 5f66 696c 7465 7265 6429  events_filtered)
-00002750: 2020 2320 4a75 7374 2074 6f20 6974 6572    # Just to iter
-00002760: 6174 6520 4461 7461 206f 626a 6563 7420  ate Data object 
-00002770: 2863 6163 6865 2066 696c 6520 7769 6c6c  (cache file will
-00002780: 2062 6520 6372 6561 7465 6429 2e0a 0a66   be created)...f
-00002790: 696c 7465 7265 645f 6576 656e 7473 5f74  iltered_events_t
-000027a0: 7970 6573 203d 2065 7665 6e74 735f 6669  ypes = events_fi
-000027b0: 6c74 6572 6564 2e6d 6170 286c 616d 6264  ltered.map(lambd
-000027c0: 6120 7265 636f 7264 3a20 7b22 6576 656e  a record: {"even
-000027d0: 7454 7970 6522 3a20 7265 636f 7264 2e67  tType": record.g
-000027e0: 6574 2822 6576 656e 7454 7970 6522 297d  et("eventType")}
-000027f0: 290a 0a65 7665 6e74 735f 7769 7468 6f75  )..events_withou
-00002800: 745f 7479 7065 735f 7769 7468 5f62 6174  t_types_with_bat
-00002810: 6368 203d 2066 696c 7465 7265 645f 6576  ch = filtered_ev
-00002820: 656e 7473 5f74 7970 6573 2e66 696c 7465  ents_types.filte
-00002830: 7228 0a20 2020 206c 616d 6264 6120 7265  r(.    lambda re
-00002840: 636f 7264 3a20 6e6f 7420 7265 636f 7264  cord: not record
-00002850: 2e67 6574 2822 6576 656e 7454 7970 6522  .get("eventType"
-00002860: 290a 290a 6576 656e 7473 5f77 6974 686f  ).).events_witho
-00002870: 7574 5f74 7970 6573 5f77 6974 685f 6261  ut_types_with_ba
-00002880: 7463 682e 7573 655f 6361 6368 6528 290a  tch.use_cache().
-00002890: 0a23 205b 312e 3131 5d20 4461 7461 206f  .# [1.11] Data o
-000028a0: 626a 6563 7473 206a 6f69 6e69 6e67 2e0a  bjects joining..
-000028b0: 2320 596f 7520 6861 7665 2074 6865 2066  # You have the f
-000028c0: 6f6c 6c6f 7769 6e67 2033 2044 6174 6120  ollowing 3 Data 
-000028d0: 6f62 6a65 6374 732e 0a64 3120 3d20 4461  objects..d1 = Da
-000028e0: 7461 285b 312c 2032 2c20 335d 290a 6432  ta([1, 2, 3]).d2
-000028f0: 203d 2044 6174 6128 5b22 6122 2c20 7b22   = Data(["a", {"
-00002900: 6964 223a 2031 3233 7d2c 2022 6322 5d29  id": 123}, "c"])
-00002910: 0a64 3320 3d20 4461 7461 285b 372c 2038  .d3 = Data([7, 8
-00002920: 2c20 395d 290a 2320 596f 7520 6361 6e20  , 9]).# You can 
-00002930: 6a6f 696e 2044 6174 6120 6f62 6a65 6374  join Data object
-00002940: 7320 696e 2066 6f6c 6c6f 7769 6e67 2077  s in following w
-00002950: 6179 732e 0a23 2050 6c65 6173 6520 6e6f  ays..# Please no
-00002960: 7465 2c20 6e65 7720 4461 7461 206f 626a  te, new Data obj
-00002970: 6563 7420 7769 6c6c 2068 6176 6520 6361  ect will have ca
-00002980: 6368 6520 7374 6174 7573 203d 3d20 4661  che status == Fa
-00002990: 6c73 652e 0a64 6174 615f 7669 615f 696e  lse..data_via_in
-000029a0: 6974 203d 2044 6174 6128 5b64 312c 2064  it = Data([d1, d
-000029b0: 322c 2064 335d 290a 6461 7461 5f76 6961  2, d3]).data_via
-000029c0: 5f61 6464 203d 2064 3120 2b20 6432 202b  _add = d1 + d2 +
-000029d0: 2064 330a 6461 7461 5f77 6974 685f 6e6f   d3.data_with_no
-000029e0: 6e5f 6461 7461 5f6f 626a 5f76 6961 5f69  n_data_obj_via_i
-000029f0: 6e69 7420 3d20 4461 7461 285b 6431 2c20  nit = Data([d1, 
-00002a00: 5b22 6122 2c20 7b22 6964 223a 2031 3233  ["a", {"id": 123
-00002a10: 7d2c 2022 6322 5d2c 2064 335d 290a 6461  }, "c"], d3]).da
-00002a20: 7461 5f77 6974 685f 6e6f 6e5f 6461 7461  ta_with_non_data
-00002a30: 5f6f 626a 5f76 6961 5f61 6464 203d 2064  _obj_via_add = d
-00002a40: 3120 2b20 5b22 6122 2c20 7b22 6964 223a  1 + ["a", {"id":
-00002a50: 2031 3233 7d2c 2022 6322 5d20 2b20 6433   123}, "c"] + d3
-00002a60: 0a23 2059 6f75 2063 616e 206a 6f69 6e20  .# You can join 
-00002a70: 6375 7272 656e 7420 4461 7461 206f 626a  current Data obj
-00002a80: 6563 7420 6f6e 2070 6c61 6365 2075 7369  ect on place usi
-00002a90: 6e67 202b 3d2e 0a23 2049 7420 7769 6c6c  ng +=..# It will
-00002aa0: 206b 6565 7020 6361 6368 6520 7374 6174   keep cache stat
-00002ab0: 7573 2e0a 6431 202b 3d20 6433 2020 2320  us..d1 += d3  # 
-00002ac0: 6431 2077 696c 6c20 6265 636f 6d65 2044  d1 will become D
-00002ad0: 6174 6128 5b31 2c32 2c33 2c37 2c38 2c39  ata([1,2,3,7,8,9
-00002ae0: 5d29 0a0a 2320 5b31 2e31 325d 2042 7569  ])..# [1.12] Bui
-00002af0: 6c64 2061 6e64 2072 6561 6420 4461 7461  ld and read Data
-00002b00: 206f 626a 6563 7420 6361 6368 6520 6669   object cache fi
-00002b10: 6c65 732e 0a65 7665 6e74 732e 6275 696c  les..events.buil
-00002b20: 645f 6361 6368 6528 2263 6163 6865 5f66  d_cache("cache_f
-00002b30: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
-00002b40: 290a 6461 7461 5f6f 626a 5f66 726f 6d5f  ).data_obj_from_
-00002b50: 6361 6368 6520 3d20 4461 7461 2e66 726f  cache = Data.fro
-00002b60: 6d5f 6361 6368 655f 6669 6c65 2822 6361  m_cache_file("ca
-00002b70: 6368 655f 6669 6c65 6e61 6d65 5f6f 725f  che_filename_or_
-00002b80: 7061 7468 2229 0a0a 2320 5b31 2e31 335d  path")..# [1.13]
-00002b90: 2043 6865 636b 2069 6620 4461 7461 2069   Check if Data i
-00002ba0: 7320 736f 7274 6564 2e0a 2320 5468 6174  s sorted..# That
-00002bb0: 2077 696c 6c20 7265 7475 726e 2061 6e20   will return an 
-00002bc0: 6f62 6a65 6374 2060 6973 5f73 6f72 7465  object `is_sorte
-00002bd0: 6460 2074 6861 7420 636f 6e74 6169 6e73  d` that contains
-00002be0: 2069 6e66 6f72 6d61 7469 6f6e 0a23 2020   information.#  
-00002bf0: 2031 2e20 7374 6174 7573 202d 2d20 736f   1. status -- so
-00002c00: 7274 6564 206f 7220 6e6f 740a 2320 2020  rted or not.#   
-00002c10: 322e 2066 6972 7374 5f75 6e73 6f72 7465  2. first_unsorte
-00002c20: 6420 2d2d 2074 6865 2069 6e64 6578 206f  d -- the index o
-00002c30: 6620 7468 6520 6669 7273 7420 756e 736f  f the first unso
-00002c40: 7274 6564 2065 6c65 6d65 6e74 0a69 735f  rted element.is_
-00002c50: 736f 7274 6564 203d 2065 7665 6e74 732e  sorted = events.
-00002c60: 6973 5f73 6f72 7465 6428 6c61 6d62 6461  is_sorted(lambda
-00002c70: 2065 3a20 655b 2273 7461 7274 5469 6d65   e: e["startTime
-00002c80: 7374 616d 7022 5d5b 2265 706f 6368 5365  stamp"]["epochSe
-00002c90: 636f 6e64 225d 290a 0a23 2059 6f75 2063  cond"])..# You c
-00002ca0: 616e 2075 7365 2074 6869 7320 6f62 6a65  an use this obje
-00002cb0: 6374 2061 7320 7573 7561 6c20 626f 6f6c  ct as usual bool
-00002cc0: 2076 6172 6961 626c 652e 0a69 6620 6973   variable..if is
-00002cd0: 5f73 6f72 7465 643a 0a20 2020 2070 7269  _sorted:.    pri
-00002ce0: 6e74 2822 6576 656e 7473 2044 6174 6120  nt("events Data 
-00002cf0: 6f62 6a20 6973 2073 6f72 7465 6421 2229  obj is sorted!")
-00002d00: 0a0a 2320 5b31 2e31 345d 2055 7365 2060  ..# [1.14] Use `
-00002d10: 4461 7461 2e73 686f 7728 2960 2074 6f20  Data.show()` to 
-00002d20: 6c6f 6f6b 2061 7420 7468 6520 6669 7273  look at the firs
-00002d30: 7420 4e20 6d65 7373 6167 6573 2069 6e20  t N messages in 
-00002d40: 7468 6520 7374 7265 616d 2e0a 6461 7461  the stream..data
-00002d50: 5f77 6974 685f 6e6f 6e5f 6461 7461 5f6f  _with_non_data_o
-00002d60: 626a 5f76 6961 5f61 6464 2e73 686f 7728  bj_via_add.show(
-00002d70: 6e3d 3629 0a23 2057 696c 6c20 7072 696e  n=6).# Will prin
-00002d80: 740a 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  t.# ------------
-00002d90: 2d20 5072 696e 7465 6420 6669 7273 7420  - Printed first 
-00002da0: 3620 7265 636f 7264 7320 2d2d 2d2d 2d2d  6 records ------
-00002db0: 2d2d 2d2d 2d2d 2d0a 2320 5b31 5d20 2d2d  -------.# [1] --
-00002dc0: 2d2d 2d2d 0a23 2031 0a23 205b 325d 202d  ----.# 1.# [2] -
-00002dd0: 2d2d 2d2d 2d0a 2320 320a 2320 5b33 5d20  -----.# 2.# [3] 
-00002de0: 2d2d 2d2d 2d2d 0a23 2033 0a23 205b 345d  ------.# 3.# [4]
-00002df0: 202d 2d2d 2d2d 2d0a 2320 2761 270a 2320   ------.# 'a'.# 
-00002e00: 5b35 5d20 2d2d 2d2d 2d2d 0a23 207b 2769  [5] ------.# {'i
-00002e10: 6427 3a20 3132 337d 0a23 205b 365d 202d  d': 123}.# [6] -
-00002e20: 2d2d 2d2d 2d0a 2320 2763 270a 0a23 205b  -----.# 'c'..# [
-00002e30: 312e 3135 5d20 596f 7520 6361 6e20 7265  1.15] You can re
-00002e40: 6d6f 7665 2074 6865 2063 6163 6865 2066  move the cache f
-00002e50: 696c 6520 6f66 2074 6865 2044 6174 6120  ile of the Data 
-00002e60: 6f62 6a65 6374 2c20 6966 2072 6571 7569  object, if requi
-00002e70: 7265 642e 0a64 6174 615f 6f62 6a5f 6672  red..data_obj_fr
-00002e80: 6f6d 5f63 6163 6865 2e63 6c65 6172 5f63  om_cache.clear_c
-00002e90: 6163 6865 2829 0a0a 2323 2323 2323 2323  ache()..########
-00002ea0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002eb0: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-00002ec0: 205b 325d 2057 6f72 6b69 6e67 2077 6974   [2] Working wit
-00002ed0: 6820 636f 6e76 6572 7465 7273 2e0a 2323  h converters..##
-00002ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002f00: 2323 2323 0a23 2054 6865 7265 2061 7265  ####.# There are
-00002f10: 2063 7572 7265 6e74 6c79 2074 6872 6565   currently three
-00002f20: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00002f30: 206f 6620 4954 696d 6573 7461 6d70 436f   of ITimestampCo
-00002f40: 6e76 6572 7465 7220 636c 6173 733a 2044  nverter class: D
-00002f50: 6174 6574 696d 6543 6f6e 7665 7274 652c  atetimeConverte,
-00002f60: 2044 6174 6574 696d 6553 7472 696e 6743   DatetimeStringC
-00002f70: 6f6e 7665 7274 6572 2061 6e64 2050 726f  onverter and Pro
-00002f80: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
-00002f90: 6e76 6572 7465 722e 0a23 2054 6865 7920  nverter..# They 
-00002fa0: 616c 6c20 696d 706c 656d 656e 7420 7361  all implement sa
-00002fb0: 6d65 206d 6574 686f 6473 2066 726f 6d20  me methods from 
-00002fc0: 6261 7365 2063 6c61 7373 2e0a 2320 4e6f  base class..# No
-00002fd0: 7465 2074 6861 7420 736f 6d65 2061 6363  te that some acc
-00002fe0: 7572 6163 7920 6d61 7920 6265 206c 6f73  uracy may be los
-00002ff0: 7420 6475 7269 6e67 2063 6f6e 7665 7273  t during convers
-00003000: 696f 6e2e 0a23 2049 6620 666f 7220 6578  ion..# If for ex
-00003010: 616d 706c 6520 796f 7520 7573 6520 746f  ample you use to
-00003020: 5f6d 6963 726f 7365 636f 6e64 7320 6e61  _microseconds na
-00003030: 6e6f 7365 636f 6e64 7320 7769 6c6c 2062  noseconds will b
-00003040: 6520 6375 7420 6f66 6620 696e 7374 6561  e cut off instea
-00003050: 6420 6f66 2072 6f75 6e64 696e 672e 0a0a  d of rounding...
-00003060: 2320 5b32 2e31 5d20 4461 7465 7469 6d65  # [2.1] Datetime
-00003070: 436f 6e76 6572 7465 722e 0a23 2044 6174  Converter..# Dat
-00003080: 6574 696d 6543 6f6e 7665 7274 6572 2074  etimeConverter t
-00003090: 616b 6573 2064 6174 6574 696d 652e 6461  akes datetime.da
-000030a0: 7465 7469 6d65 206f 626a 6563 7420 6173  tetime object as
-000030b0: 2069 6e70 7574 2e0a 0a64 6174 6574 696d   input...datetim
-000030c0: 655f 6f62 6a20 3d20 6461 7465 7469 6d65  e_obj = datetime
-000030d0: 2879 6561 723d 3230 3233 2c20 6d6f 6e74  (year=2023, mont
-000030e0: 683d 312c 2064 6179 3d35 2c20 686f 7572  h=1, day=5, hour
-000030f0: 3d31 342c 206d 696e 7574 653d 3338 2c20  =14, minute=38, 
-00003100: 7365 636f 6e64 3d32 352c 206d 6963 726f  second=25, micro
-00003110: 7365 636f 6e64 3d31 3436 3029 0a0a 2320  second=1460)..# 
-00003120: 4974 2068 6173 206d 6574 686f 6473 2074  It has methods t
-00003130: 6861 7420 7265 7475 726e 2074 6865 2064  hat return the d
-00003140: 6174 6574 696d 6520 696e 2064 6966 6665  atetime in diffe
-00003150: 7265 6e74 2066 6f72 6d61 733a 0a0a 6461  rent formas:..da
-00003160: 7465 5f6d 7320 3d20 4461 7465 7469 6d65  te_ms = Datetime
-00003170: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
-00003180: 6c69 7365 636f 6e64 7328 6461 7465 7469  liseconds(dateti
-00003190: 6d65 5f6f 626a 290a 6461 7465 5f75 7320  me_obj).date_us 
-000031a0: 3d20 4461 7465 7469 6d65 436f 6e76 6572  = DatetimeConver
-000031b0: 7465 722e 746f 5f6d 6963 726f 7365 636f  ter.to_microseco
-000031c0: 6e64 7328 6461 7465 7469 6d65 5f6f 626a  nds(datetime_obj
-000031d0: 290a 2320 436f 6e76 6572 7469 6e67 2074  ).# Converting t
-000031e0: 6f20 6e61 6e6f 7365 636f 6e64 7320 6a75  o nanoseconds ju
-000031f0: 7374 7320 6164 6473 2074 6872 6565 2074  sts adds three t
-00003200: 7261 696c 696e 6720 7a65 726f 7320 6173  railing zeros as
-00003210: 2064 6174 6574 696d 6520 6f62 6a65 6374   datetime object
-00003220: 2064 6f65 736e 2774 2068 6176 6520 6e61   doesn't have na
-00003230: 6e6f 7365 636f 6e64 732e 0a64 6174 655f  noseconds..date_
-00003240: 6e73 203d 2044 6174 6574 696d 6543 6f6e  ns = DatetimeCon
-00003250: 7665 7274 6572 2e74 6f5f 6e61 6e6f 7365  verter.to_nanose
-00003260: 636f 6e64 7328 6461 7465 7469 6d65 5f6f  conds(datetime_o
-00003270: 626a 290a 0a23 205b 322e 325d 2044 6174  bj)..# [2.2] Dat
-00003280: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
-00003290: 7274 6572 0a23 2044 6174 6574 696d 6553  rter.# DatetimeS
-000032a0: 7472 696e 6743 6f6e 7665 7274 6572 2074  tringConverter t
-000032b0: 616b 6573 2073 7472 696e 6720 696e 2022  akes string in "
-000032c0: 7979 7979 2d4d 4d2d 6464 5448 483a 6d6d  yyyy-MM-ddTHH:mm
-000032d0: 3a73 735b 2e53 5353 5353 5353 5353 5d5a  :ss[.SSSSSSSSS]Z
-000032e0: 2220 666f 726d 6174 2e0a 0a64 6174 655f  " format...date_
-000032f0: 7374 7269 6e67 203d 2022 3230 3233 2d30  string = "2023-0
-00003300: 312d 3035 5431 343a 3338 3a32 352e 3030  1-05T14:38:25.00
-00003310: 3134 365a 220a 0a23 2057 6520 6861 7665  146Z"..# We have
-00003320: 2073 616d 6520 6d65 7468 6f64 7320 6173   same methods as
-00003330: 2069 6e20 4461 7465 7469 6d65 436f 6e76   in DatetimeConv
-00003340: 6572 7465 720a 6461 7465 5f6d 735f 6672  erter.date_ms_fr
-00003350: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
-00003360: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-00003370: 7465 722e 746f 5f6d 696c 6c69 7365 636f  ter.to_milliseco
-00003380: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
-00003390: 0a64 6174 655f 7573 5f66 726f 6d5f 7374  .date_us_from_st
-000033a0: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
-000033b0: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
-000033c0: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
-000033d0: 6174 655f 7374 7269 6e67 290a 6461 7465  ate_string).date
-000033e0: 5f6e 735f 6672 6f6d 5f73 7472 696e 6720  _ns_from_string 
-000033f0: 3d20 4461 7465 7469 6d65 5374 7269 6e67  = DatetimeString
-00003400: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
-00003410: 6f73 6563 6f6e 6473 2864 6174 655f 7374  oseconds(date_st
-00003420: 7269 6e67 290a 0a23 2057 6520 6361 6e20  ring)..# We can 
-00003430: 616c 736f 2067 6574 2064 6174 6574 696d  also get datetim
-00003440: 6520 6f62 6a65 6374 2066 726f 6d20 7374  e object from st
-00003450: 7269 6e67 0a64 6174 6574 696d 655f 6672  ring.datetime_fr
-00003460: 6f6d 5f73 7472 696e 6720 3d20 4461 7465  om_string = Date
-00003470: 7469 6d65 5374 7269 6e67 436f 6e76 6572  timeStringConver
-00003480: 7465 722e 746f 5f64 6174 6574 696d 6528  ter.to_datetime(
-00003490: 6461 7465 5f73 7472 696e 6729 0a0a 2320  date_string)..# 
-000034a0: 5b32 2e33 5d20 5072 6f74 6f62 7566 5469  [2.3] ProtobufTi
-000034b0: 6d65 7374 616d 7043 6f6e 7665 7274 6572  mestampConverter
-000034c0: 0a23 2050 726f 746f 6275 6620 7469 6d65  .# Protobuf time
-000034d0: 7374 616d 7073 206d 7573 7420 6265 2069  stamps must be i
-000034e0: 6e20 666f 726d 207b 2265 706f 6368 5365  n form {"epochSe
-000034f0: 636f 6e64 223a 2073 6563 6f6e 6473 2c20  cond": seconds, 
-00003500: 226e 616e 6f22 3a20 6e61 6e6f 7365 636f  "nano": nanoseco
-00003510: 6e64 737d 0a0a 7072 6f74 6f62 7566 5f74  nds}..protobuf_t
-00003520: 696d 6573 7461 6d70 203d 207b 2265 706f  imestamp = {"epo
-00003530: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-00003540: 3239 3530 352c 2022 6e61 6e6f 223a 2031  29505, "nano": 1
-00003550: 5f34 3630 5f30 3030 7d0a 0a64 6174 655f  _460_000}..date_
-00003560: 6d73 5f66 726f 6d5f 7469 6d65 7374 616d  ms_from_timestam
-00003570: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
-00003580: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
-00003590: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2870  o_milliseconds(p
-000035a0: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
-000035b0: 7029 0a64 6174 655f 7573 5f66 726f 6d5f  p).date_us_from_
-000035c0: 7469 6d65 7374 616d 7020 3d20 5072 6f74  timestamp = Prot
-000035d0: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
-000035e0: 7665 7274 6572 2e74 6f5f 6d69 6372 6f73  verter.to_micros
-000035f0: 6563 6f6e 6473 2870 726f 746f 6275 665f  econds(protobuf_
-00003600: 7469 6d65 7374 616d 7029 0a64 6174 655f  timestamp).date_
-00003610: 6e73 5f66 726f 6d5f 7469 6d65 7374 616d  ns_from_timestam
-00003620: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
-00003630: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
-00003640: 6f5f 6e61 6e6f 7365 636f 6e64 7328 7072  o_nanoseconds(pr
-00003650: 6f74 6f62 7566 5f74 696d 6573 7461 6d70  otobuf_timestamp
-00003660: 290a 6461 7465 7469 6d65 5f66 726f 6d5f  ).datetime_from_
-00003670: 7469 6d65 7374 616d 7020 3d20 5072 6f74  timestamp = Prot
-00003680: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
-00003690: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
-000036a0: 6d65 2870 726f 746f 6275 665f 7469 6d65  me(protobuf_time
-000036b0: 7374 616d 7029 0a0a 2323 2323 2323 2323  stamp)..########
-000036c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000036d0: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-000036e0: 205b 335d 2057 6f72 6b69 6e67 2077 6974   [3] Working wit
-000036f0: 6820 4576 656e 7454 7265 6520 616e 6420  h EventTree and 
-00003700: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00003710: 696f 6e2e 0a23 2323 2323 2323 2323 2323  ion..###########
+00001f50: 2323 2323 2323 0a0a 2320 5b31 2e31 5d20  ######..# [1.1] 
+00001f60: 4669 6c74 6572 2e0a 6669 6c74 6572 6564  Filter..filtered
+00001f70: 5f65 7665 6e74 733a 2044 6174 6120 3d20  _events: Data = 
+00001f80: 6576 656e 7473 2e66 696c 7465 7228 0a20  events.filter(. 
+00001f90: 2020 206c 616d 6264 6120 653a 2065 5b22     lambda e: e["
+00001fa0: 626f 6479 225d 2021 3d20 5b5d 2920 2023  body"] != [])  #
+00001fb0: 2046 696c 7465 7220 6576 656e 7473 2077   Filter events w
+00001fc0: 6974 6820 656d 7074 7920 626f 6479 2e0a  ith empty body..
+00001fd0: 0a0a 2320 5b31 2e32 5d20 4d61 702e 0a64  ..# [1.2] Map..d
+00001fe0: 6566 2074 7261 6e73 666f 726d 5f66 756e  ef transform_fun
+00001ff0: 6374 696f 6e28 7265 636f 7264 293a 0a20  ction(record):. 
+00002000: 2020 2072 6574 7572 6e20 7b22 6576 656e     return {"even
+00002010: 744e 616d 6522 3a20 7265 636f 7264 5b22  tName": record["
+00002020: 6576 656e 744e 616d 6522 5d2c 0a20 2020  eventName"],.   
+00002030: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
+00002040: 7366 756c 223a 2072 6563 6f72 645b 2273  sful": record["s
+00002050: 7563 6365 7373 6675 6c22 5d7d 0a0a 0a66  uccessful"]}...f
+00002060: 696c 7465 7265 645f 616e 645f 6d61 7070  iltered_and_mapp
+00002070: 6564 5f65 7665 6e74 7320 3d20 6669 6c74  ed_events = filt
+00002080: 6572 6564 5f65 7665 6e74 732e 6d61 7028  ered_events.map(
+00002090: 7472 616e 7366 6f72 6d5f 6675 6e63 7469  transform_functi
+000020a0: 6f6e 290a 0a23 205b 312e 335d 2044 6174  on)..# [1.3] Dat
+000020b0: 6120 7069 7065 6c69 6e65 2e0a 2320 2020  a pipeline..#   
+000020c0: 2020 2020 496e 7374 6561 6420 6f66 2064      Instead of d
+000020d0: 6f69 6e67 2064 6174 6120 7472 616e 7366  oing data transf
+000020e0: 6f72 6d61 7469 6f6e 7320 7374 6570 2062  ormations step b
+000020f0: 7920 7374 6570 2079 6f75 2063 616e 2064  y step you can d
+00002100: 6f20 6974 2069 6e20 6f6e 6520 6c69 6e65  o it in one line
+00002110: 2e0a 6669 6c74 6572 6564 5f61 6e64 5f6d  ..filtered_and_m
+00002120: 6170 7065 645f 6576 656e 7473 5f62 795f  apped_events_by_
+00002130: 7069 7065 6c69 6e65 203d 2065 7665 6e74  pipeline = event
+00002140: 732e 6669 6c74 6572 280a 2020 2020 6c61  s.filter(.    la
+00002150: 6d62 6461 2065 3a20 655b 2262 6f64 7922  mbda e: e["body"
+00002160: 5d20 213d 205b 5d29 2e6d 6170 280a 2020  ] != []).map(.  
+00002170: 2020 7472 616e 7366 6f72 6d5f 6675 6e63    transform_func
+00002180: 7469 6f6e 0a29 0a23 2043 6f6e 7465 6e74  tion.).# Content
+00002190: 206f 6620 7468 6573 6520 7477 6f20 4461   of these two Da
+000021a0: 7461 206f 626a 6563 7473 2073 686f 756c  ta objects shoul
+000021b0: 6420 6265 2065 7175 616c 2e0a 6173 7365  d be equal..asse
+000021c0: 7274 206c 6973 7428 6669 6c74 6572 6564  rt list(filtered
+000021d0: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
+000021e0: 7473 2920 3d3d 206c 6973 7428 0a20 2020  ts) == list(.   
+000021f0: 2066 696c 7465 7265 645f 616e 645f 6d61   filtered_and_ma
+00002200: 7070 6564 5f65 7665 6e74 735f 6279 5f70  pped_events_by_p
+00002210: 6970 656c 696e 6529 0a0a 2320 5b31 2e34  ipeline)..# [1.4
+00002220: 5d20 5369 6674 2e20 536b 6970 2074 6865  ] Sift. Skip the
+00002230: 2066 6972 7374 2066 6577 2069 7465 6d73   first few items
+00002240: 206f 7220 6c69 6d69 7420 7468 656d 2e0a   or limit them..
+00002250: 6461 7461 203d 2044 6174 6128 5b31 2c20  data = Data([1, 
+00002260: 322c 2033 2c20 342c 2035 2c20 362c 2037  2, 3, 4, 5, 6, 7
+00002270: 2c20 382c 2039 2c20 3130 2c20 3131 2c20  , 8, 9, 10, 11, 
+00002280: 3132 2c20 3133 2c20 3134 2c20 3135 5d29  12, 13, 14, 15])
+00002290: 0a69 7465 6d73 5f66 726f 6d5f 3131 5f74  .items_from_11_t
+000022a0: 6f5f 656e 643a 2047 656e 6572 6174 6f72  o_end: Generator
+000022b0: 203d 2064 6174 612e 7369 6674 2873 6b69   = data.sift(ski
+000022c0: 703d 3130 290a 6f6e 6c79 5f66 6972 7374  p=10).only_first
+000022d0: 5f31 305f 6974 656d 733a 2047 656e 6572  _10_items: Gener
+000022e0: 6174 6f72 203d 2064 6174 612e 7369 6674  ator = data.sift
+000022f0: 286c 696d 6974 3d31 3029 0a0a 2320 5b31  (limit=10)..# [1
+00002300: 2e35 5d20 4368 616e 6769 6e67 2063 6163  .5] Changing cac
+00002310: 6865 2073 7461 7475 732e 0a65 7665 6e74  he status..event
+00002320: 732e 7573 655f 6361 6368 6528 5472 7565  s.use_cache(True
+00002330: 290a 2320 6f72 206a 7573 740a 6576 656e  ).# or just.even
+00002340: 7473 2e75 7365 5f63 6163 6865 2829 2020  ts.use_cache()  
+00002350: 2320 4966 2079 6f75 2077 616e 7420 746f  # If you want to
+00002360: 2061 6374 6976 6174 6520 6361 6368 652e   activate cache.
+00002370: 0a23 205b 312e 365d 2057 616c 6b20 7468  .# [1.6] Walk th
+00002380: 726f 7567 6820 6461 7461 2e0a 666f 7220  rough data..for 
+00002390: 6576 656e 7420 696e 2065 7665 6e74 733a  event in events:
+000023a0: 0a20 2020 2023 2044 6f20 736f 6d65 7468  .    # Do someth
+000023b0: 696e 6720 7769 7468 2065 7665 6e74 2028  ing with event (
+000023c0: 6576 656e 7420 6973 2061 2064 6963 7429  event is a dict)
+000023d0: 2e0a 2020 2020 7072 696e 7428 6576 656e  ..    print(even
+000023e0: 7429 0a23 2041 6674 6572 2066 6972 7374  t).# After first
+000023f0: 2069 7465 7261 7469 6f6e 2074 6865 2065   iteration the e
+00002400: 7665 6e74 7320 6861 7320 6120 6361 6368  vents has a cach
+00002410: 6520 6669 6c65 2e0a 2320 4e6f 7720 7468  e file..# Now th
+00002420: 6579 2077 696c 6c20 6265 2075 7365 6420  ey will be used 
+00002430: 696e 2074 6865 2063 6163 6865 2069 6e20  in the cache in 
+00002440: 7468 6520 6e65 7874 2069 7465 7261 7469  the next iterati
+00002450: 6f6e 2e0a 0a23 205b 312e 375d 2047 6574  on...# [1.7] Get
+00002460: 206e 756d 6265 7220 6f66 2074 6865 2065   number of the e
+00002470: 6c65 6d65 6e74 7320 696e 2074 6865 2044  lements in the D
+00002480: 6174 6120 6f62 6a65 6374 2e0a 6e75 6d62  ata object..numb
+00002490: 6572 5f6f 665f 6576 656e 7473 203d 2065  er_of_events = e
+000024a0: 7665 6e74 732e 6c65 6e0a 0a23 205b 312e  vents.len..# [1.
+000024b0: 385d 2043 6865 636b 2074 6861 7420 4461  8] Check that Da
+000024c0: 7461 206f 626a 6563 7420 6973 6e27 7420  ta object isn't 
+000024d0: 656d 7074 792e 0a23 2054 6865 2064 6174  empty..# The dat
+000024e0: 6120 736f 7572 6365 2073 686f 756c 6420  a source should 
+000024f0: 6265 206e 6f74 2065 6d70 7479 2e0a 6173  be not empty..as
+00002500: 7365 7274 2065 7665 6e74 732e 6973 5f65  sert events.is_e
+00002510: 6d70 7479 2069 7320 4661 6c73 650a 0a23  mpty is False..#
+00002520: 205b 312e 395d 2043 6f6e 7665 7274 2044   [1.9] Convert D
+00002530: 6174 6120 6f62 6a65 6374 2074 6f20 7468  ata object to th
+00002540: 6520 6c69 7374 206f 6620 656c 656d 656e  e list of elemen
+00002550: 7473 2865 7665 6e74 7320 6f72 206d 6573  ts(events or mes
+00002560: 7361 6765 7329 2e0a 2320 4265 2063 6172  sages)..# Be car
+00002570: 6566 756c 2c20 7468 6973 2063 616e 2074  eful, this can t
+00002580: 616b 6520 746f 6f20 6d75 6368 206d 656d  ake too much mem
+00002590: 6f72 792e 0a65 7665 6e74 735f 6c69 7374  ory..events_list
+000025a0: 203d 206c 6973 7428 6576 656e 7473 290a   = list(events).
+000025b0: 0a23 205b 312e 3130 5d20 5468 6520 6361  .# [1.10] The ca
+000025c0: 6368 6520 696e 6865 7269 7461 6e63 652e  che inheritance.
+000025d0: 0a23 2043 7265 6174 6573 2061 206e 6577  .# Creates a new
+000025e0: 2044 6174 6120 6f62 6a65 6374 2074 6861   Data object tha
+000025f0: 7420 7769 6c6c 2075 7365 2063 6163 6865  t will use cache
+00002600: 2066 726f 6d20 7468 6520 6576 656e 7473   from the events
+00002610: 2044 6174 6120 6f62 6a65 6374 2e0a 6576   Data object..ev
+00002620: 656e 7473 5f66 696c 7465 7265 643a 2044  ents_filtered: D
+00002630: 6174 6120 3d20 6576 656e 7473 2e66 696c  ata = events.fil
+00002640: 7465 7228 6c61 6d62 6461 2072 6563 6f72  ter(lambda recor
+00002650: 643a 2072 6563 6f72 642e 6765 7428 2262  d: record.get("b
+00002660: 6174 6368 4964 2229 290a 0a23 204e 6577  atchId"))..# New
+00002670: 2044 6174 6120 6f62 6a65 6374 7320 646f   Data objects do
+00002680: 6e27 7420 7573 6520 7468 6569 7220 6f77  n't use their ow
+00002690: 6e20 6361 6368 6520 6279 2064 6566 6175  n cache by defau
+000026a0: 6c74 2062 7574 2075 7365 2074 6865 2063  lt but use the c
+000026b0: 6163 6865 206f 6620 7468 6520 7061 7265  ache of the pare
+000026c0: 6e74 2044 6174 6120 6f62 6a65 6374 2e0a  nt Data object..
+000026d0: 2320 5573 6520 7573 655f 6361 6368 6520  # Use use_cache 
+000026e0: 6d65 7468 6f64 2074 6f20 6163 7469 7661  method to activa
+000026f0: 7465 2063 6163 6869 6e67 2e0a 2320 4166  te caching..# Af
+00002700: 7465 7220 7468 6174 2c20 7468 6520 4461  ter that, the Da
+00002710: 7461 206f 626a 6563 7420 7769 6c6c 2063  ta object will c
+00002720: 7265 6174 6520 6974 7320 6f77 6e20 6361  reate its own ca
+00002730: 6368 6520 6669 6c65 2e0a 6576 656e 7473  che file..events
+00002740: 5f66 696c 7465 7265 642e 7573 655f 6361  _filtered.use_ca
+00002750: 6368 6528 290a 0a6c 6973 7428 0a20 2020  che()..list(.   
+00002760: 2065 7665 6e74 735f 6669 6c74 6572 6564   events_filtered
+00002770: 2920 2023 204a 7573 7420 746f 2069 7465  )  # Just to ite
+00002780: 7261 7465 2044 6174 6120 6f62 6a65 6374  rate Data object
+00002790: 2028 6361 6368 6520 6669 6c65 2077 696c   (cache file wil
+000027a0: 6c20 6265 2063 7265 6174 6564 292e 0a0a  l be created)...
+000027b0: 6669 6c74 6572 6564 5f65 7665 6e74 735f  filtered_events_
+000027c0: 7479 7065 7320 3d20 6576 656e 7473 5f66  types = events_f
+000027d0: 696c 7465 7265 642e 6d61 7028 0a20 2020  iltered.map(.   
+000027e0: 206c 616d 6264 6120 7265 636f 7264 3a20   lambda record: 
+000027f0: 7b22 6576 656e 7454 7970 6522 3a20 7265  {"eventType": re
+00002800: 636f 7264 2e67 6574 2822 6576 656e 7454  cord.get("eventT
+00002810: 7970 6522 297d 290a 0a65 7665 6e74 735f  ype")})..events_
+00002820: 7769 7468 6f75 745f 7479 7065 735f 7769  without_types_wi
+00002830: 7468 5f62 6174 6368 203d 2066 696c 7465  th_batch = filte
+00002840: 7265 645f 6576 656e 7473 5f74 7970 6573  red_events_types
+00002850: 2e66 696c 7465 7228 0a20 2020 206c 616d  .filter(.    lam
+00002860: 6264 6120 7265 636f 7264 3a20 6e6f 7420  bda record: not 
+00002870: 7265 636f 7264 2e67 6574 2822 6576 656e  record.get("even
+00002880: 7454 7970 6522 290a 290a 6576 656e 7473  tType").).events
+00002890: 5f77 6974 686f 7574 5f74 7970 6573 5f77  _without_types_w
+000028a0: 6974 685f 6261 7463 682e 7573 655f 6361  ith_batch.use_ca
+000028b0: 6368 6528 290a 0a23 205b 312e 3131 5d20  che()..# [1.11] 
+000028c0: 4461 7461 206f 626a 6563 7473 206a 6f69  Data objects joi
+000028d0: 6e69 6e67 2e0a 2320 596f 7520 6861 7665  ning..# You have
+000028e0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2033   the following 3
+000028f0: 2044 6174 6120 6f62 6a65 6374 732e 0a64   Data objects..d
+00002900: 3120 3d20 4461 7461 285b 312c 2032 2c20  1 = Data([1, 2, 
+00002910: 335d 290a 6432 203d 2044 6174 6128 5b22  3]).d2 = Data(["
+00002920: 6122 2c20 7b22 6964 223a 2031 3233 7d2c  a", {"id": 123},
+00002930: 2022 6322 5d29 0a64 3320 3d20 4461 7461   "c"]).d3 = Data
+00002940: 285b 372c 2038 2c20 395d 290a 2320 596f  ([7, 8, 9]).# Yo
+00002950: 7520 6361 6e20 6a6f 696e 2044 6174 6120  u can join Data 
+00002960: 6f62 6a65 6374 7320 696e 2066 6f6c 6c6f  objects in follo
+00002970: 7769 6e67 2077 6179 732e 0a23 2050 6c65  wing ways..# Ple
+00002980: 6173 6520 6e6f 7465 2c20 6e65 7720 4461  ase note, new Da
+00002990: 7461 206f 626a 6563 7420 7769 6c6c 2068  ta object will h
+000029a0: 6176 6520 6361 6368 6520 7374 6174 7573  ave cache status
+000029b0: 203d 3d20 4661 6c73 652e 0a64 6174 615f   == False..data_
+000029c0: 7669 615f 696e 6974 203d 2044 6174 6128  via_init = Data(
+000029d0: 5b64 312c 2064 322c 2064 335d 290a 6461  [d1, d2, d3]).da
+000029e0: 7461 5f76 6961 5f61 6464 203d 2064 3120  ta_via_add = d1 
+000029f0: 2b20 6432 202b 2064 330a 6461 7461 5f77  + d2 + d3.data_w
+00002a00: 6974 685f 6e6f 6e5f 6461 7461 5f6f 626a  ith_non_data_obj
+00002a10: 5f76 6961 5f69 6e69 7420 3d20 4461 7461  _via_init = Data
+00002a20: 285b 6431 2c20 5b22 6122 2c20 7b22 6964  ([d1, ["a", {"id
+00002a30: 223a 2031 3233 7d2c 2022 6322 5d2c 2064  ": 123}, "c"], d
+00002a40: 335d 290a 6461 7461 5f77 6974 685f 6e6f  3]).data_with_no
+00002a50: 6e5f 6461 7461 5f6f 626a 5f76 6961 5f61  n_data_obj_via_a
+00002a60: 6464 203d 2064 3120 2b20 5b22 6122 2c20  dd = d1 + ["a", 
+00002a70: 7b22 6964 223a 2031 3233 7d2c 2022 6322  {"id": 123}, "c"
+00002a80: 5d20 2b20 6433 0a23 2059 6f75 2063 616e  ] + d3.# You can
+00002a90: 206a 6f69 6e20 6375 7272 656e 7420 4461   join current Da
+00002aa0: 7461 206f 626a 6563 7420 6f6e 2070 6c61  ta object on pla
+00002ab0: 6365 2075 7369 6e67 202b 3d2e 0a23 2049  ce using +=..# I
+00002ac0: 7420 7769 6c6c 206b 6565 7020 6361 6368  t will keep cach
+00002ad0: 6520 7374 6174 7573 2e0a 6431 202b 3d20  e status..d1 += 
+00002ae0: 6433 2020 2320 6431 2077 696c 6c20 6265  d3  # d1 will be
+00002af0: 636f 6d65 2044 6174 6128 5b31 2c32 2c33  come Data([1,2,3
+00002b00: 2c37 2c38 2c39 5d29 0a0a 2320 5b31 2e31  ,7,8,9])..# [1.1
+00002b10: 325d 2042 7569 6c64 2061 6e64 2072 6561  2] Build and rea
+00002b20: 6420 4461 7461 206f 626a 6563 7420 6361  d Data object ca
+00002b30: 6368 6520 6669 6c65 732e 0a65 7665 6e74  che files..event
+00002b40: 732e 6275 696c 645f 6361 6368 6528 2263  s.build_cache("c
+00002b50: 6163 6865 5f66 696c 656e 616d 655f 6f72  ache_filename_or
+00002b60: 5f70 6174 6822 290a 6461 7461 5f6f 626a  _path").data_obj
+00002b70: 5f66 726f 6d5f 6361 6368 6520 3d20 4461  _from_cache = Da
+00002b80: 7461 2e66 726f 6d5f 6361 6368 655f 6669  ta.from_cache_fi
+00002b90: 6c65 2822 6361 6368 655f 6669 6c65 6e61  le("cache_filena
+00002ba0: 6d65 5f6f 725f 7061 7468 2229 0a0a 2320  me_or_path")..# 
+00002bb0: 5b31 2e31 335d 2043 6865 636b 2069 6620  [1.13] Check if 
+00002bc0: 4461 7461 2069 7320 736f 7274 6564 2e0a  Data is sorted..
+00002bd0: 2320 5468 6174 2077 696c 6c20 7265 7475  # That will retu
+00002be0: 726e 2061 6e20 6f62 6a65 6374 2060 6973  rn an object `is
+00002bf0: 5f73 6f72 7465 6460 2074 6861 7420 636f  _sorted` that co
+00002c00: 6e74 6169 6e73 2069 6e66 6f72 6d61 7469  ntains informati
+00002c10: 6f6e 0a23 2020 2031 2e20 7374 6174 7573  on.#   1. status
+00002c20: 202d 2d20 736f 7274 6564 206f 7220 6e6f   -- sorted or no
+00002c30: 740a 2320 2020 322e 2066 6972 7374 5f75  t.#   2. first_u
+00002c40: 6e73 6f72 7465 6420 2d2d 2074 6865 2069  nsorted -- the i
+00002c50: 6e64 6578 206f 6620 7468 6520 6669 7273  ndex of the firs
+00002c60: 7420 756e 736f 7274 6564 2065 6c65 6d65  t unsorted eleme
+00002c70: 6e74 0a69 735f 736f 7274 6564 203d 2065  nt.is_sorted = e
+00002c80: 7665 6e74 732e 6973 5f73 6f72 7465 6428  vents.is_sorted(
+00002c90: 6c61 6d62 6461 2065 3a20 655b 2273 7461  lambda e: e["sta
+00002ca0: 7274 5469 6d65 7374 616d 7022 5d5b 2265  rtTimestamp"]["e
+00002cb0: 706f 6368 5365 636f 6e64 225d 290a 0a23  pochSecond"])..#
+00002cc0: 2059 6f75 2063 616e 2075 7365 2074 6869   You can use thi
+00002cd0: 7320 6f62 6a65 6374 2061 7320 7573 7561  s object as usua
+00002ce0: 6c20 626f 6f6c 2076 6172 6961 626c 652e  l bool variable.
+00002cf0: 0a69 6620 6973 5f73 6f72 7465 643a 0a20  .if is_sorted:. 
+00002d00: 2020 2070 7269 6e74 2822 6576 656e 7473     print("events
+00002d10: 2044 6174 6120 6f62 6a20 6973 2073 6f72   Data obj is sor
+00002d20: 7465 6421 2229 0a0a 2320 5b31 2e31 345d  ted!")..# [1.14]
+00002d30: 2055 7365 2060 4461 7461 2e73 686f 7728   Use `Data.show(
+00002d40: 2960 2074 6f20 6c6f 6f6b 2061 7420 7468  )` to look at th
+00002d50: 6520 6669 7273 7420 4e20 6d65 7373 6167  e first N messag
+00002d60: 6573 2069 6e20 7468 6520 7374 7265 616d  es in the stream
+00002d70: 2e0a 6461 7461 5f77 6974 685f 6e6f 6e5f  ..data_with_non_
+00002d80: 6461 7461 5f6f 626a 5f76 6961 5f61 6464  data_obj_via_add
+00002d90: 2e73 686f 7728 6e3d 3629 0a23 2057 696c  .show(n=6).# Wil
+00002da0: 6c20 7072 696e 740a 2320 2d2d 2d2d 2d2d  l print.# ------
+00002db0: 2d2d 2d2d 2d2d 2d20 5072 696e 7465 6420  ------- Printed 
+00002dc0: 6669 7273 7420 3620 7265 636f 7264 7320  first 6 records 
+00002dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2320  -------------.# 
+00002de0: 5b31 5d20 2d2d 2d2d 2d2d 0a23 2031 0a23  [1] ------.# 1.#
+00002df0: 205b 325d 202d 2d2d 2d2d 2d0a 2320 320a   [2] ------.# 2.
+00002e00: 2320 5b33 5d20 2d2d 2d2d 2d2d 0a23 2033  # [3] ------.# 3
+00002e10: 0a23 205b 345d 202d 2d2d 2d2d 2d0a 2320  .# [4] ------.# 
+00002e20: 2761 270a 2320 5b35 5d20 2d2d 2d2d 2d2d  'a'.# [5] ------
+00002e30: 0a23 207b 2769 6427 3a20 3132 337d 0a23  .# {'id': 123}.#
+00002e40: 205b 365d 202d 2d2d 2d2d 2d0a 2320 2763   [6] ------.# 'c
+00002e50: 270a 0a23 205b 312e 3135 5d20 596f 7520  '..# [1.15] You 
+00002e60: 6361 6e20 7265 6d6f 7665 2074 6865 2063  can remove the c
+00002e70: 6163 6865 2066 696c 6520 6f66 2074 6865  ache file of the
+00002e80: 2044 6174 6120 6f62 6a65 6374 2c20 6966   Data object, if
+00002e90: 2072 6571 7569 7265 642e 0a64 6174 615f   required..data_
+00002ea0: 6f62 6a5f 6672 6f6d 5f63 6163 6865 2e63  obj_from_cache.c
+00002eb0: 6c65 6172 5f63 6163 6865 2829 0a0a 2323  lear_cache()..##
+00002ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002ee0: 2323 2323 0a23 205b 325d 2057 6f72 6b69  ####.# [2] Worki
+00002ef0: 6e67 2077 6974 6820 636f 6e76 6572 7465  ng with converte
+00002f00: 7273 2e0a 2323 2323 2323 2323 2323 2323  rs..############
+00002f10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002f20: 2323 2323 2323 2323 2323 0a23 2054 6865  ##########.# The
+00002f30: 7265 2061 7265 2063 7572 7265 6e74 6c79  re are currently
+00002f40: 2074 6872 6565 2069 6d70 6c65 6d65 6e74   three implement
+00002f50: 6174 696f 6e73 206f 6620 4954 696d 6573  ations of ITimes
+00002f60: 7461 6d70 436f 6e76 6572 7465 7220 636c  tampConverter cl
+00002f70: 6173 733a 2044 6174 6574 696d 6543 6f6e  ass: DatetimeCon
+00002f80: 7665 7274 652c 2044 6174 6574 696d 6553  verte, DatetimeS
+00002f90: 7472 696e 6743 6f6e 7665 7274 6572 2061  tringConverter a
+00002fa0: 6e64 2050 726f 746f 6275 6654 696d 6573  nd ProtobufTimes
+00002fb0: 7461 6d70 436f 6e76 6572 7465 722e 0a23  tampConverter..#
+00002fc0: 2054 6865 7920 616c 6c20 696d 706c 656d   They all implem
+00002fd0: 656e 7420 7361 6d65 206d 6574 686f 6473  ent same methods
+00002fe0: 2066 726f 6d20 6261 7365 2063 6c61 7373   from base class
+00002ff0: 2e0a 2320 4e6f 7465 2074 6861 7420 736f  ..# Note that so
+00003000: 6d65 2061 6363 7572 6163 7920 6d61 7920  me accuracy may 
+00003010: 6265 206c 6f73 7420 6475 7269 6e67 2063  be lost during c
+00003020: 6f6e 7665 7273 696f 6e2e 0a23 2049 6620  onversion..# If 
+00003030: 666f 7220 6578 616d 706c 6520 796f 7520  for example you 
+00003040: 7573 6520 746f 5f6d 6963 726f 7365 636f  use to_microseco
+00003050: 6e64 7320 6e61 6e6f 7365 636f 6e64 7320  nds nanoseconds 
+00003060: 7769 6c6c 2062 6520 6375 7420 6f66 6620  will be cut off 
+00003070: 696e 7374 6561 6420 6f66 2072 6f75 6e64  instead of round
+00003080: 696e 672e 0a0a 2320 5b32 2e31 5d20 4461  ing...# [2.1] Da
+00003090: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+000030a0: 0a23 2044 6174 6574 696d 6543 6f6e 7665  .# DatetimeConve
+000030b0: 7274 6572 2074 616b 6573 2064 6174 6574  rter takes datet
+000030c0: 696d 652e 6461 7465 7469 6d65 206f 626a  ime.datetime obj
+000030d0: 6563 7420 6173 2069 6e70 7574 2e0a 0a64  ect as input...d
+000030e0: 6174 6574 696d 655f 6f62 6a20 3d20 6461  atetime_obj = da
+000030f0: 7465 7469 6d65 2879 6561 723d 3230 3233  tetime(year=2023
+00003100: 2c20 6d6f 6e74 683d 312c 2064 6179 3d35  , month=1, day=5
+00003110: 2c20 686f 7572 3d31 342c 206d 696e 7574  , hour=14, minut
+00003120: 653d 3338 2c0a 2020 2020 2020 2020 2020  e=38,.          
+00003130: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003140: 636f 6e64 3d32 352c 206d 6963 726f 7365  cond=25, microse
+00003150: 636f 6e64 3d31 3436 3029 0a0a 2320 4974  cond=1460)..# It
+00003160: 2068 6173 206d 6574 686f 6473 2074 6861   has methods tha
+00003170: 7420 7265 7475 726e 2074 6865 2064 6174  t return the dat
+00003180: 6574 696d 6520 696e 2064 6966 6665 7265  etime in differe
+00003190: 6e74 2066 6f72 6d61 733a 0a0a 6461 7465  nt formas:..date
+000031a0: 5f6d 7320 3d20 4461 7465 7469 6d65 436f  _ms = DatetimeCo
+000031b0: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
+000031c0: 7365 636f 6e64 7328 6461 7465 7469 6d65  seconds(datetime
+000031d0: 5f6f 626a 290a 6461 7465 5f75 7320 3d20  _obj).date_us = 
+000031e0: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+000031f0: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
+00003200: 7328 6461 7465 7469 6d65 5f6f 626a 290a  s(datetime_obj).
+00003210: 2320 436f 6e76 6572 7469 6e67 2074 6f20  # Converting to 
+00003220: 6e61 6e6f 7365 636f 6e64 7320 6a75 7374  nanoseconds just
+00003230: 7320 6164 6473 2074 6872 6565 2074 7261  s adds three tra
+00003240: 696c 696e 6720 7a65 726f 7320 6173 2064  iling zeros as d
+00003250: 6174 6574 696d 6520 6f62 6a65 6374 2064  atetime object d
+00003260: 6f65 736e 2774 2068 6176 6520 6e61 6e6f  oesn't have nano
+00003270: 7365 636f 6e64 732e 0a64 6174 655f 6e73  seconds..date_ns
+00003280: 203d 2044 6174 6574 696d 6543 6f6e 7665   = DatetimeConve
+00003290: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
+000032a0: 6e64 7328 6461 7465 7469 6d65 5f6f 626a  nds(datetime_obj
+000032b0: 290a 0a23 205b 322e 325d 2044 6174 6574  )..# [2.2] Datet
+000032c0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000032d0: 6572 0a23 2044 6174 6574 696d 6553 7472  er.# DatetimeStr
+000032e0: 696e 6743 6f6e 7665 7274 6572 2074 616b  ingConverter tak
+000032f0: 6573 2073 7472 696e 6720 696e 2022 7979  es string in "yy
+00003300: 7979 2d4d 4d2d 6464 5448 483a 6d6d 3a73  yy-MM-ddTHH:mm:s
+00003310: 735b 2e53 5353 5353 5353 5353 5d5a 2220  s[.SSSSSSSSS]Z" 
+00003320: 666f 726d 6174 2e0a 0a64 6174 655f 7374  format...date_st
+00003330: 7269 6e67 203d 2022 3230 3233 2d30 312d  ring = "2023-01-
+00003340: 3035 5431 343a 3338 3a32 352e 3030 3134  05T14:38:25.0014
+00003350: 365a 220a 0a23 2057 6520 6861 7665 2073  6Z"..# We have s
+00003360: 616d 6520 6d65 7468 6f64 7320 6173 2069  ame methods as i
+00003370: 6e20 4461 7465 7469 6d65 436f 6e76 6572  n DatetimeConver
+00003380: 7465 720a 6461 7465 5f6d 735f 6672 6f6d  ter.date_ms_from
+00003390: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
+000033a0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+000033b0: 722e 746f 5f6d 696c 6c69 7365 636f 6e64  r.to_millisecond
+000033c0: 7328 6461 7465 5f73 7472 696e 6729 0a64  s(date_string).d
+000033d0: 6174 655f 7573 5f66 726f 6d5f 7374 7269  ate_us_from_stri
+000033e0: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
+000033f0: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
+00003400: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
+00003410: 655f 7374 7269 6e67 290a 6461 7465 5f6e  e_string).date_n
+00003420: 735f 6672 6f6d 5f73 7472 696e 6720 3d20  s_from_string = 
+00003430: 4461 7465 7469 6d65 5374 7269 6e67 436f  DatetimeStringCo
+00003440: 6e76 6572 7465 722e 746f 5f6e 616e 6f73  nverter.to_nanos
+00003450: 6563 6f6e 6473 2864 6174 655f 7374 7269  econds(date_stri
+00003460: 6e67 290a 0a23 2057 6520 6361 6e20 616c  ng)..# We can al
+00003470: 736f 2067 6574 2064 6174 6574 696d 6520  so get datetime 
+00003480: 6f62 6a65 6374 2066 726f 6d20 7374 7269  object from stri
+00003490: 6e67 0a64 6174 6574 696d 655f 6672 6f6d  ng.datetime_from
+000034a0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
+000034b0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
+000034c0: 722e 746f 5f64 6174 6574 696d 6528 6461  r.to_datetime(da
+000034d0: 7465 5f73 7472 696e 6729 0a0a 2320 5b32  te_string)..# [2
+000034e0: 2e33 5d20 5072 6f74 6f62 7566 5469 6d65  .3] ProtobufTime
+000034f0: 7374 616d 7043 6f6e 7665 7274 6572 0a23  stampConverter.#
+00003500: 2050 726f 746f 6275 6620 7469 6d65 7374   Protobuf timest
+00003510: 616d 7073 206d 7573 7420 6265 2069 6e20  amps must be in 
+00003520: 666f 726d 207b 2265 706f 6368 5365 636f  form {"epochSeco
+00003530: 6e64 223a 2073 6563 6f6e 6473 2c20 226e  nd": seconds, "n
+00003540: 616e 6f22 3a20 6e61 6e6f 7365 636f 6e64  ano": nanosecond
+00003550: 737d 0a0a 7072 6f74 6f62 7566 5f74 696d  s}..protobuf_tim
+00003560: 6573 7461 6d70 203d 207b 2265 706f 6368  estamp = {"epoch
+00003570: 5365 636f 6e64 223a 2031 3637 3239 3239  Second": 1672929
+00003580: 3530 352c 2022 6e61 6e6f 223a 2031 5f34  505, "nano": 1_4
+00003590: 3630 5f30 3030 7d0a 0a64 6174 655f 6d73  60_000}..date_ms
+000035a0: 5f66 726f 6d5f 7469 6d65 7374 616d 7020  _from_timestamp 
+000035b0: 3d20 5072 6f74 6f62 7566 5469 6d65 7374  = ProtobufTimest
+000035c0: 616d 7043 6f6e 7665 7274 6572 2e74 6f5f  ampConverter.to_
+000035d0: 6d69 6c6c 6973 6563 6f6e 6473 280a 2020  milliseconds(.  
+000035e0: 2020 7072 6f74 6f62 7566 5f74 696d 6573    protobuf_times
+000035f0: 7461 6d70 290a 6461 7465 5f75 735f 6672  tamp).date_us_fr
+00003600: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
+00003610: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
+00003620: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
+00003630: 726f 7365 636f 6e64 7328 0a20 2020 2070  roseconds(.    p
+00003640: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+00003650: 7029 0a64 6174 655f 6e73 5f66 726f 6d5f  p).date_ns_from_
+00003660: 7469 6d65 7374 616d 7020 3d20 5072 6f74  timestamp = Prot
+00003670: 6f62 7566 5469 6d65 7374 616d 7043 6f6e  obufTimestampCon
+00003680: 7665 7274 6572 2e74 6f5f 6e61 6e6f 7365  verter.to_nanose
+00003690: 636f 6e64 7328 0a20 2020 2070 726f 746f  conds(.    proto
+000036a0: 6275 665f 7469 6d65 7374 616d 7029 0a64  buf_timestamp).d
+000036b0: 6174 6574 696d 655f 6672 6f6d 5f74 696d  atetime_from_tim
+000036c0: 6573 7461 6d70 203d 2050 726f 746f 6275  estamp = Protobu
+000036d0: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
+000036e0: 7465 722e 746f 5f64 6174 6574 696d 6528  ter.to_datetime(
+000036f0: 0a20 2020 2070 726f 746f 6275 665f 7469  .    protobuf_ti
+00003700: 6d65 7374 616d 7029 0a0a 2323 2323 2323  mestamp)..######
+00003710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00003720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003730: 2323 2323 2323 2323 2323 230a 2320 4361  ###########.# Ca
-00003740: 6e20 6265 2075 7365 6675 6c20 6966 2079  n be useful if y
-00003750: 6f75 2068 6176 6520 6461 7461 2d73 7472  ou have data-str
-00003760: 6561 6d20 7769 7468 203c 2031 3030 6b20  eam with < 100k 
-00003770: 656c 656d 656e 7473 2c20 6f74 6865 7277  elements, otherw
-00003780: 6973 6520 6974 0a23 2074 616b 6573 2074  ise it.# takes t
-00003790: 6f6f 206d 7563 6820 5241 4d2e 0a0a 2320  oo much RAM...# 
-000037a0: 5b33 2e31 5d20 4275 696c 6420 6120 6375  [3.1] Build a cu
-000037b0: 7374 6f6d 2045 7665 6e74 5472 6565 0a23  stom EventTree.#
-000037c0: 2054 6f20 6372 6561 7465 2061 6e20 4576   To create an Ev
-000037d0: 656e 7454 7265 6520 6f62 6a65 6374 2079  entTree object y
-000037e0: 6f75 206e 6565 6420 746f 2070 726f 7669  ou need to provi
-000037f0: 6465 206e 616d 652c 2069 6420 616e 6420  de name, id and 
-00003800: 6461 7461 206f 6620 7468 6520 726f 6f74  data of the root
-00003810: 2065 7665 6e74 2e0a 7472 6565 203d 2045   event..tree = E
-00003820: 7665 6e74 5472 6565 2865 7665 6e74 5f6e  ventTree(event_n
-00003830: 616d 653d 2272 6f6f 7420 6576 656e 7422  ame="root event"
-00003840: 2c20 6576 656e 745f 6964 3d22 726f 6f74  , event_id="root
-00003850: 5f69 6422 2c20 6461 7461 3d7b 2264 6174  _id", data={"dat
-00003860: 6122 3a20 5b31 2c20 322c 2033 2c20 342c  a": [1, 2, 3, 4,
-00003870: 2035 5d7d 290a 0a23 2054 6f20 6164 6420   5]})..# To add 
-00003880: 6e65 7720 6e6f 6465 2075 7365 2061 7070  new node use app
-00003890: 656e 645f 6576 656e 742e 2070 6172 656e  end_event. paren
-000038a0: 745f 6964 2069 7320 6e65 6365 7373 6172  t_id is necessar
-000038b0: 792c 2064 6174 6120 6973 206f 7074 696f  y, data is optio
-000038c0: 6e61 6c2e 0a74 7265 652e 6170 7065 6e64  nal..tree.append
-000038d0: 5f65 7665 6e74 2865 7665 6e74 5f6e 616d  _event(event_nam
-000038e0: 653d 2241 222c 2065 7665 6e74 5f69 643d  e="A", event_id=
-000038f0: 2241 5f69 6422 2c20 6461 7461 3d4e 6f6e  "A_id", data=Non
-00003900: 652c 2070 6172 656e 745f 6964 3d22 726f  e, parent_id="ro
-00003910: 6f74 5f69 6422 290a 0a23 205b 332e 335d  ot_id")..# [3.3]
-00003920: 2042 7569 6c64 696e 6720 7468 6520 4576   Building the Ev
-00003930: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00003940: 6e2e 0a64 6174 615f 736f 7572 6365 3a20  n..data_source: 
-00003950: 4944 6174 6153 6f75 7263 6520 2023 2059  IDataSource  # Y
-00003960: 6f75 2073 686f 756c 6420 696e 6974 2044  ou should init D
-00003970: 6174 6153 6f75 7263 6520 6f62 6a65 6374  ataSource object
-00003980: 2e20 452e 672e 2066 726f 6d20 4c77 4450  . E.g. from LwDP
-00003990: 206d 6f64 756c 652e 0a64 6174 615f 736f   module..data_so
-000039a0: 7572 6365 203d 2044 756d 6d79 4461 7461  urce = DummyData
-000039b0: 536f 7572 6365 2829 2020 2320 4e6f 7465  Source()  # Note
-000039c0: 2120 5765 2075 7365 2066 616b 6520 4453  ! We use fake DS
-000039d0: 2068 6572 652e 0a23 2045 5443 4472 6976   here..# ETCDriv
-000039e0: 6572 2068 6572 6520 6973 2061 2073 7475  er here is a stu
-000039f0: 622c 2061 6374 7561 6c6c 7920 7468 6520  b, actually the 
-00003a00: 6c69 6220 646f 6573 6e27 7420 6861 7665  lib doesn't have
-00003a10: 2073 7563 6820 6120 636c 6173 732e 0a23   such a class..#
-00003a20: 2059 6f75 2063 616e 2074 616b 6520 6974   You can take it
-00003a30: 2069 6e20 4c77 4450 206d 6f64 756c 6520   in LwDP module 
-00003a40: 6f72 2063 7265 6174 6520 796f 7572 7365  or create yourse
-00003a50: 6c66 2063 6c61 7373 2069 6620 796f 7520  lf class if you 
-00003a60: 6861 7665 2073 6f6d 6520 7370 6563 6961  have some specia
-00003a70: 6c20 6576 656e 7473 2073 7472 7563 7475  l events structu
-00003a80: 7265 2e0a 6672 6f6d 2074 6832 5f64 6174  re..from th2_dat
-00003a90: 615f 7365 7276 6963 6573 2e64 6174 615f  a_services.data_
-00003aa0: 736f 7572 6365 2e6c 7764 702e 6576 656e  source.lwdp.even
-00003ab0: 745f 7472 6565 2069 6d70 6f72 7420 4874  t_tree import Ht
-00003ac0: 7470 4554 4344 7269 7665 7220 6173 2045  tpETCDriver as E
-00003ad0: 5443 4472 6976 6572 0a0a 2320 4966 2079  TCDriver..# If y
-00003ae0: 6f75 2064 6f6e 2774 2073 7065 6369 6679  ou don't specify
-00003af0: 2064 6174 615f 736f 7572 6365 2066 6f72   data_source for
-00003b00: 2074 6865 2064 7269 7665 7220 7468 656e   the driver then
-00003b10: 2069 7420 776f 6e27 7420 7265 636f 7665   it won't recove
-00003b20: 7220 6465 7461 6368 6564 2065 7665 6e74  r detached event
-00003b30: 732e 0a64 7269 7665 723a 2049 4554 4344  s..driver: IETCD
-00003b40: 7269 7665 7220 2023 2059 6f75 2073 686f  river  # You sho
-00003b50: 756c 6420 696e 6974 2045 5443 4472 6976  uld init ETCDriv
-00003b60: 6572 206f 626a 6563 742e 2045 2e67 2e20  er object. E.g. 
-00003b70: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
-00003b80: 206f 7220 796f 7572 2063 7573 746f 6d20   or your custom 
-00003b90: 636c 6173 732e 0a64 7269 7665 7220 3d20  class..driver = 
-00003ba0: 4554 4344 7269 7665 7228 6461 7461 5f73  ETCDriver(data_s
-00003bb0: 6f75 7263 653d 6461 7461 5f73 6f75 7263  ource=data_sourc
-00003bc0: 652c 2075 7365 5f73 7475 623d 5472 7565  e, use_stub=True
-00003bd0: 290a 0a65 7463 203d 2045 7665 6e74 5472  )..etc = EventTr
-00003be0: 6565 436f 6c6c 6563 7469 6f6e 2864 7269  eeCollection(dri
-00003bf0: 7665 7229 0a65 7463 2e62 7569 6c64 2865  ver).etc.build(e
-00003c00: 7665 6e74 7329 0a65 7463 2e73 686f 7728  vents).etc.show(
-00003c10: 290a 2320 4974 276c 6c20 7072 696e 7420  ).# It'll print 
-00003c20: 7468 6520 666f 6c6c 6f77 696e 673a 0a23  the following:.#
-00003c30: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
-00003c40: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
-00003c50: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
-00003c60: 0a23 20e2 949c e294 80e2 9480 2050 6c61  .# ......... Pla
-00003c70: 696e 2065 7665 6e74 2031 0a23 20e2 9494  in event 1.# ...
-00003c80: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
-00003c90: 6e74 2032 0a0a 7072 696e 7428 6574 6329  nt 2..print(etc)
-00003ca0: 0a23 2045 7665 6e74 5472 6565 436f 6c6c  .# EventTreeColl
-00003cb0: 6563 7469 6f6e 2874 7265 6573 3d31 2c20  ection(trees=1, 
-00003cc0: 6576 656e 7473 3d33 5b74 7265 6573 3d33  events=3[trees=3
-00003cd0: 2c20 6465 7461 6368 6564 3d30 5d29 0a0a  , detached=0])..
-00003ce0: 2320 4465 7461 6368 6564 2065 7665 6e74  # Detached event
-00003cf0: 7320 6973 6e27 7420 656d 7074 792e 0a61  s isn't empty..a
-00003d00: 7373 6572 7420 6574 632e 6765 745f 6465  ssert etc.get_de
-00003d10: 7461 6368 6564 5f65 7665 6e74 7328 2920  tached_events() 
-00003d20: 2023 2072 6574 7572 6e73 206c 6973 7420   # returns list 
-00003d30: 6f66 2064 6574 6163 6865 645f 6576 656e  of detached_even
-00003d40: 7473 2e0a 0a23 2072 6563 6f76 6572 5f75  ts...# recover_u
-00003d50: 6e6b 6e6f 776e 5f65 7665 6e74 7320 2d2d  nknown_events --
-00003d60: 2075 7365 6420 746f 2072 6563 6f76 6572   used to recover
-00003d70: 2073 6f6d 6520 6576 656e 7473 2070 6172   some events par
-00003d80: 656e 7473 2e0a 2320 5468 6174 2077 6f6e  ents..# That won
-00003d90: 2774 2077 6f72 6b20 7769 7468 2044 756d  't work with Dum
-00003da0: 6d79 4461 7461 536f 7572 6365 2c20 736f  myDataSource, so
-00003db0: 2077 6173 2063 6f6d 6d65 6e74 6564 0a23   was commented.#
-00003dc0: 2065 7463 2e72 6563 6f76 6572 5f75 6e6b   etc.recover_unk
-00003dd0: 6e6f 776e 5f65 7665 6e74 7328 290a 0a23  nown_events()..#
-00003de0: 2041 6674 6572 2074 6861 7420 7468 6520   After that the 
-00003df0: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
-00003e00: 7368 6f75 6c64 2062 6520 656d 7074 7920  should be empty 
-00003e10: 6265 6361 7573 6520 7468 6579 2077 6572  because they wer
-00003e20: 6520 7265 636f 7665 7265 642e 0a23 2061  e recovered..# a
-00003e30: 7373 6572 7420 6e6f 7420 6574 632e 6765  ssert not etc.ge
-00003e40: 745f 6465 7461 6368 6564 5f65 7665 6e74  t_detached_event
-00003e50: 7328 290a 0a23 202d 2d2d 2d2d 0a0a 2320  s()..# -----..# 
-00003e60: 5468 6520 636f 6c6c 6563 7469 6f6e 2068  The collection h
-00003e70: 6173 2045 7665 6e74 5472 6565 7320 6561  as EventTrees ea
-00003e80: 6368 2077 6974 6820 6120 7472 6565 206f  ch with a tree o
-00003e90: 6620 6576 656e 7473 2e0a 2320 5573 696e  f events..# Usin
-00003ea0: 6720 436f 6c6c 6563 7469 6f6e 2061 6e64  g Collection and
-00003eb0: 2045 7665 6e74 5472 6565 732c 2079 6f75   EventTrees, you
-00003ec0: 2063 616e 2077 6f72 6b20 666c 6578 6962   can work flexib
-00003ed0: 6c79 2077 6974 6820 6576 656e 7473 2e0a  ly with events..
-00003ee0: 0a23 205b 332e 332e 315d 2047 6574 206c  .# [3.3.1] Get l
-00003ef0: 6561 7665 7320 6f66 2061 6c6c 2074 7265  eaves of all tre
-00003f00: 6573 2e0a 6c65 6176 6573 3a20 5475 706c  es..leaves: Tupl
-00003f10: 655b 6469 6374 5d20 3d20 6574 632e 6765  e[dict] = etc.ge
-00003f20: 745f 6c65 6176 6573 2829 2020 2320 5265  t_leaves()  # Re
-00003f30: 7475 726e 7320 6120 7475 706c 6520 6f66  turns a tuple of
-00003f40: 206c 6561 7665 7320 6576 656e 7473 0a0a   leaves events..
-00003f50: 2320 5b33 2e33 2e32 5d20 4765 7420 726f  # [3.3.2] Get ro
-00003f60: 6f74 7320 6964 7320 6f66 2061 6c6c 2074  ots ids of all t
-00003f70: 7265 6573 2e0a 726f 6f74 733a 204c 6973  rees..roots: Lis
-00003f80: 745b 7374 725d 203d 2065 7463 2e67 6574  t[str] = etc.get
-00003f90: 5f72 6f6f 7473 5f69 6473 2829 0a23 2052  _roots_ids().# R
-00003fa0: 6574 7572 6e73 2074 6865 206c 6973 7420  eturns the list 
-00003fb0: 6f66 2072 6f6f 7420 4964 733a 0a23 205b  of root Ids:.# [
-00003fc0: 2764 656d 6f5f 626f 6f6b 5f31 3a74 6832  'demo_book_1:th2
-00003fd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-00003fe0: 3335 3730 3535 3630 3837 3330 3030 3a64  35705560873000:d
-00003ff0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
-00004000: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
-00004010: 3532 645f 3127 5d0a 0a23 205b 332e 332e  52d_1']..# [3.3.
-00004020: 335d 2046 696e 6420 616e 2065 7665 6e74  3] Find an event
-00004030: 2069 6e20 616c 6c20 7472 6565 732e 0a66   in all trees..f
-00004040: 696e 645f 6576 656e 743a 204f 7074 696f  ind_event: Optio
-00004050: 6e61 6c5b 6469 6374 5d20 3d20 6574 632e  nal[dict] = etc.
-00004060: 6669 6e64 286c 616d 6264 6120 6576 656e  find(lambda even
-00004070: 743a 2022 5365 6e64 206d 6573 7361 6765  t: "Send message
-00004080: 2220 696e 2065 7665 6e74 5b22 6576 656e  " in event["even
-00004090: 7454 7970 6522 5d29 0a0a 2320 5b33 2e33  tType"])..# [3.3
-000040a0: 2e34 5d20 4669 6e64 2061 6c6c 2065 7665  .4] Find all eve
-000040b0: 6e74 7320 696e 2061 6c6c 2074 7265 6573  nts in all trees
-000040c0: 2e20 5468 6572 6520 6973 2061 6c73 6f20  . There is also 
-000040d0: 6974 6572 6162 6c65 2076 6572 7369 6f6e  iterable version
-000040e0: 2027 6669 6e64 616c 6c5f 6974 6572 272e   'findall_iter'.
-000040f0: 0a66 696e 645f 6576 656e 7473 3a20 4c69  .find_events: Li
-00004100: 7374 5b64 6963 745d 203d 2065 7463 2e66  st[dict] = etc.f
-00004110: 696e 6461 6c6c 286c 616d 6264 6120 6576  indall(lambda ev
-00004120: 656e 743a 2065 7665 6e74 5b22 7375 6363  ent: event["succ
-00004130: 6573 7366 756c 225d 2069 7320 5472 7565  essful"] is True
-00004140: 290a 0a23 205b 332e 332e 355d 2046 696e  )..# [3.3.5] Fin
-00004150: 6420 616e 2061 6e63 6573 746f 7220 6f66  d an ancestor of
-00004160: 2074 6865 2065 7665 6e74 2e0a 616e 6365   the event..ance
-00004170: 7374 6f72 3a20 4f70 7469 6f6e 616c 5b64  stor: Optional[d
-00004180: 6963 745d 203d 2065 7463 2e66 696e 645f  ict] = etc.find_
-00004190: 616e 6365 7374 6f72 280a 2020 2020 2264  ancestor(.    "d
-000041a0: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-000041b0: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-000041c0: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
-000041d0: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
-000041e0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
-000041f0: 645f 3122 2c0a 2020 2020 6669 6c74 6572  d_1",.    filter
-00004200: 3d6c 616d 6264 6120 6576 656e 743a 2022  =lambda event: "
-00004210: 526f 6f74 4576 656e 7422 2069 6e20 6576  RootEvent" in ev
-00004220: 656e 745b 2265 7665 6e74 4e61 6d65 225d  ent["eventName"]
-00004230: 2c0a 290a 0a23 205b 332e 332e 365d 2047  ,.)..# [3.3.6] G
-00004240: 6574 2063 6869 6c64 7265 6e20 6f66 2074  et children of t
-00004250: 6865 2065 7665 6e74 2e20 5468 6572 6520  he event. There 
-00004260: 6973 2061 6c73 6f20 6974 6572 6162 6c65  is also iterable
-00004270: 2076 6572 7369 6f6e 2027 6765 745f 6368   version 'get_ch
-00004280: 696c 6472 656e 5f69 7465 7227 2e0a 6368  ildren_iter'..ch
-00004290: 696c 6472 656e 3a20 5475 706c 655b 6469  ildren: Tuple[di
-000042a0: 6374 5d20 3d20 6574 632e 6765 745f 6368  ct] = etc.get_ch
-000042b0: 696c 6472 656e 280a 2020 2020 2264 656d  ildren(.    "dem
-000042c0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-000042d0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-000042e0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
-000042f0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-00004300: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-00004310: 3122 0a29 0a0a 2320 5b33 2e33 2e37 5d20  1".)..# [3.3.7] 
-00004320: 4765 7420 7375 6274 7265 6520 666f 7220  Get subtree for 
-00004330: 7370 6563 6966 6965 6420 6576 656e 742e  specified event.
-00004340: 0a73 7562 7472 6565 3a20 4576 656e 7454  .subtree: EventT
-00004350: 7265 6520 3d20 6574 632e 6765 745f 7375  ree = etc.get_su
-00004360: 6274 7265 6528 0a20 2020 2022 6465 6d6f  btree(.    "demo
-00004370: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00004380: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00004390: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
-000043a0: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
-000043b0: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
-000043c0: 220a 290a 0a23 205b 332e 332e 385d 2047  ".)..# [3.3.8] G
-000043d0: 6574 2066 756c 6c20 7061 7468 2074 6f20  et full path to 
-000043e0: 7468 6520 6576 656e 742e 0a23 204c 6f6f  the event..# Loo
-000043f0: 6b73 206c 696b 6520 5b61 6e63 6573 746f  ks like [ancesto
-00004400: 725f 726f 6f74 2c20 616e 6365 7374 6f72  r_root, ancestor
-00004410: 5f6c 6576 656c 312c 2061 6e63 6573 746f  _level1, ancesto
-00004420: 725f 6c65 7665 6c32 2c20 6576 656e 745d  r_level2, event]
-00004430: 0a65 7665 6e74 5f70 6174 683a 204c 6973  .event_path: Lis
-00004440: 745b 6469 6374 5d20 3d20 6574 632e 6765  t[dict] = etc.ge
-00004450: 745f 6675 6c6c 5f70 6174 6828 0a20 2020  t_full_path(.   
-00004460: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00004470: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00004480: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
-00004490: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-000044a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-000044b0: 3135 3264 5f31 220a 290a 0a23 205b 332e  152d_1".)..# [3.
-000044c0: 332e 395d 2047 6574 2070 6172 656e 7420  3.9] Get parent 
-000044d0: 6f66 2074 6865 2065 7665 6e74 2e0a 7061  of the event..pa
-000044e0: 7265 6e74 203d 2065 7463 2e67 6574 5f70  rent = etc.get_p
-000044f0: 6172 656e 7428 0a20 2020 2022 6465 6d6f  arent(.    "demo
-00004500: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00004510: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00004520: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
-00004530: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
-00004540: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
-00004550: 220a 290a 0a23 205b 332e 332e 3130 5d20  ".)..# [3.3.10] 
-00004560: 4170 7065 6e64 206e 6577 2065 7665 6e74  Append new event
-00004570: 2074 6f20 7468 6520 636f 6c6c 6563 7469   to the collecti
-00004580: 6f6e 2e0a 6574 632e 6170 7065 6e64 5f65  on..etc.append_e
-00004590: 7665 6e74 280a 2020 2020 6576 656e 743d  vent(.    event=
-000045a0: 7b0a 2020 2020 2020 2020 2265 7665 6e74  {.        "event
-000045b0: 4964 223a 2022 6132 3066 3565 6634 2d63  Id": "a20f5ef4-c
-000045c0: 3366 652d 6262 3130 2d61 3239 632d 6464  3fe-bb10-a29c-dd
-000045d0: 3364 3738 3439 3039 6562 222c 0a20 2020  3d784909eb",.   
-000045e0: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
-000045f0: 7449 6422 3a20 2238 6532 3532 3466 612d  tId": "8e2524fa-
-00004600: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
-00004610: 3934 6639 3034 6333 6136 3222 2c0a 2020  94f904c3a62",.  
-00004620: 2020 2020 2020 2265 7665 6e74 4e61 6d65        "eventName
-00004630: 223a 2022 5374 7562 4576 656e 7422 2c0a  ": "StubEvent",.
-00004640: 2020 2020 7d0a 290a 0a23 205b 332e 332e      }.)..# [3.3.
-00004650: 3131 5d20 5368 6f77 2074 6865 2065 6e74  11] Show the ent
-00004660: 6972 6520 636f 6c6c 6563 7469 6f6e 2e0a  ire collection..
-00004670: 6574 632e 7368 6f77 2829 0a23 2049 7427  etc.show().# It'
-00004680: 6c6c 2070 7269 6e74 2074 6865 2066 6f6c  ll print the fol
-00004690: 6c6f 7769 6e67 3a0a 2320 5365 7420 6f66  lowing:.# Set of
-000046a0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
-000046b0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
-000046c0: 6220 7465 7374 696e 670a 2320 e294 9ce2  b testing.# ....
-000046d0: 9480 e294 8020 506c 6169 6e20 6576 656e  ..... Plain even
-000046e0: 7420 310a 2320 e294 94e2 9480 e294 8020  t 1.# ......... 
-000046f0: 506c 6169 6e20 6576 656e 7420 320a 0a23  Plain event 2..#
-00004700: 2041 7320 796f 7520 6361 6e20 7365 652c   As you can see,
-00004710: 206e 6f74 6869 6e67 2077 6173 2063 6861   nothing was cha
-00004720: 6e67 6564 2c20 6275 7420 7765 2061 6464  nged, but we add
-00004730: 6564 2074 6865 206e 6577 2065 7665 6e74  ed the new event
-00004740: 210a 2320 6c65 7427 7320 6c6f 6f6b 2061  !.# let's look a
-00004750: 7420 7468 6520 7375 6d6d 6172 792e 0a0a  t the summary...
-00004760: 7072 696e 7428 6574 632e 7375 6d6d 6172  print(etc.summar
-00004770: 7928 2929 2020 2320 7468 6520 7361 6d65  y())  # the same
-00004780: 2061 7320 6a75 7374 2070 7269 6e74 2865   as just print(e
-00004790: 7463 290a 2320 4576 656e 7454 7265 6543  tc).# EventTreeC
-000047a0: 6f6c 6c65 6374 696f 6e28 7472 6565 733d  ollection(trees=
-000047b0: 312c 2065 7665 6e74 733d 355b 7472 6565  1, events=5[tree
-000047c0: 733d 332c 2064 6574 6163 6865 643d 325d  s=3, detached=2]
-000047d0: 290a 2320 596f 7520 6361 6e20 7365 6520  ).# You can see 
-000047e0: 7468 6174 2069 7420 7761 7320 6164 6465  that it was adde
-000047f0: 6420 746f 2064 6574 6163 6865 642e 2054  d to detached. T
-00004800: 6861 7427 7320 7768 7920 796f 7520 646f  hat's why you do
-00004810: 6e27 7420 7365 6520 7468 6520 6576 656e  n't see the even
-00004820: 740a 2320 7669 6120 6073 686f 7728 2960  t.# via `show()`
-00004830: 2e20 6073 686f 7728 2960 2070 7269 6e74  . `show()` print
-00004840: 7320 6f6e 6c79 2054 7265 6573 210a 2320  s only Trees!.# 
-00004850: 5573 6520 6065 7463 2e67 6574 5f70 6172  Use `etc.get_par
-00004860: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
-00004870: 2074 6f20 636f 6e76 6572 7420 6465 7461   to convert deta
-00004880: 6368 6564 2065 7665 6e74 7320 746f 2074  ched events to t
-00004890: 7265 6573 2e0a 2320 4d6f 7265 2069 6e66  rees..# More inf
-000048a0: 6f72 6d61 7469 6f6e 2062 656c 6f77 2069  ormation below i
-000048b0: 6e20 7468 6520 636f 7272 6573 706f 6e64  n the correspond
-000048c0: 696e 6720 7365 6374 696f 6e2e 0a0a 2320  ing section...# 
-000048d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a23  --------------.#
-000048e0: 205b 332e 345d 2057 6f72 6b69 6e67 2077   [3.4] Working w
-000048f0: 6974 6820 7468 6520 4576 656e 7454 7265  ith the EventTre
-00004900: 652e 0a23 2045 7665 6e74 5472 6565 2068  e..# EventTree h
-00004910: 6173 2074 6865 2073 616d 6520 6d65 7468  as the same meth
-00004920: 6f64 7320 6173 2045 7665 6e74 5472 6565  ods as EventTree
-00004930: 436f 6c6c 6563 7469 6f6e 2c20 6275 7420  Collection, but 
-00004940: 6f6e 6c79 2066 6f72 2069 7473 206f 776e  only for its own
-00004950: 2074 7265 652e 0a0a 2320 5b33 2e34 2e31   tree...# [3.4.1
-00004960: 5d20 4765 7420 6120 636f 6c6c 6563 7469  ] Get a collecti
-00004970: 6f6e 206f 6620 7472 6565 732e 0a74 7265  on of trees..tre
-00004980: 6573 3a20 4c69 7374 5b45 7665 6e74 5472  es: List[EventTr
-00004990: 6565 5d20 3d20 6574 632e 6765 745f 7472  ee] = etc.get_tr
-000049a0: 6565 7328 290a 7472 6565 3a20 4576 656e  ees().tree: Even
-000049b0: 7454 7265 6520 3d20 7472 6565 735b 305d  tTree = trees[0]
-000049c0: 0a0a 2320 4275 7420 4576 656e 7454 7265  ..# But EventTre
-000049d0: 6520 7072 6f76 6964 6573 2061 2077 6f72  e provides a wor
-000049e0: 6b20 7769 7468 2074 6865 2074 7265 652c  k with the tree,
-000049f0: 2062 7574 2064 6f65 7320 6e6f 7420 6d6f   but does not mo
-00004a00: 6469 6679 2069 742e 0a23 2049 6620 796f  dify it..# If yo
-00004a10: 7520 7761 6e74 2074 6f20 6d6f 6469 6679  u want to modify
-00004a20: 2074 6865 2074 7265 652c 2075 7365 2045   the tree, use E
-00004a30: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-00004a40: 6f6e 732e 0a0a 2320 5b33 2e35 5d20 576f  ons...# [3.5] Wo
-00004a50: 726b 696e 6720 7769 7468 2050 6172 656e  rking with Paren
-00004a60: 746c 6573 7354 7265 652e 0a23 2050 6172  tlessTree..# Par
-00004a70: 656e 746c 6573 7354 7265 6520 6973 2061  entlessTree is a
-00004a80: 6e20 4576 656e 7454 7265 6520 7468 6174  n EventTree that
-00004a90: 2068 6173 2064 6574 6163 6865 6420 6576   has detached ev
-00004aa0: 656e 7473 2077 6974 6820 7374 7562 732e  ents with stubs.
-00004ab0: 0a70 6172 656e 746c 6573 735f 7472 6565  .parentless_tree
-00004ac0: 733a 204c 6973 745b 4576 656e 7454 7265  s: List[EventTre
-00004ad0: 655d 203d 2065 7463 2e67 6574 5f70 6172  e] = etc.get_par
-00004ae0: 656e 746c 6573 735f 7472 6565 7328 290a  entless_trees().
-00004af0: 7072 696e 7428 2270 6172 656e 746c 6573  print("parentles
-00004b00: 735f 7472 6565 7320 636f 6e74 6169 6e73  s_trees contains
-00004b10: 3a22 290a 7072 696e 7428 7061 7265 6e74  :").print(parent
-00004b20: 6c65 7373 5f74 7265 6573 290a 2320 5b45  less_trees).# [E
-00004b30: 7665 6e74 5472 6565 286e 616d 653d 273c  ventTree(name='<
-00004b40: 4272 6f6b 656e 4576 656e 743e 272c 2072  BrokenEvent>', r
-00004b50: 6f6f 745f 6964 3d27 6e6f 745f 6578 6973  oot_id='not_exis
-00004b60: 7473 5f69 6e5f 7468 655f 6576 656e 7473  ts_in_the_events
-00004b70: 5f73 7472 6561 6d27 2c20 6576 656e 7473  _stream', events
-00004b80: 3d32 292c 0a23 2020 4576 656e 7454 7265  =2),.#  EventTre
-00004b90: 6528 6e61 6d65 3d27 3c42 726f 6b65 6e45  e(name='<BrokenE
-00004ba0: 7665 6e74 3e27 2c20 726f 6f74 5f69 643d  vent>', root_id=
-00004bb0: 2738 6532 3532 3466 612d 6366 3539 2d31  '8e2524fa-cf59-1
-00004bc0: 3165 622d 6133 6637 2d30 3934 6639 3034  1eb-a3f7-094f904
-00004bd0: 6333 6136 3227 2c20 6576 656e 7473 3d32  c3a62', events=2
-00004be0: 295d 0a0a 7072 696e 7428 225c 6e22 2022  )]..print("\n" "
-00004bf0: 6574 6320 6166 7465 7220 6067 6574 5f70  etc after `get_p
-00004c00: 6172 656e 746c 6573 735f 7472 6565 7360  arentless_trees`
-00004c10: 3a22 290a 7072 696e 7428 6574 632e 7375  :").print(etc.su
-00004c20: 6d6d 6172 7928 2929 0a23 2045 7665 6e74  mmary()).# Event
-00004c30: 5472 6565 436f 6c6c 6563 7469 6f6e 2874  TreeCollection(t
-00004c40: 7265 6573 3d33 5b72 6567 756c 6172 3d31  rees=3[regular=1
-00004c50: 2c20 7061 7265 6e74 6c65 7373 3d32 5d2c  , parentless=2],
-00004c60: 2065 7665 6e74 733d 375b 7472 6565 733d   events=7[trees=
-00004c70: 372c 2064 6574 6163 6865 643d 305d 2927  7, detached=0])'
-00004c80: 0a65 7463 2e73 686f 7728 290a 2320 5365  .etc.show().# Se
-00004c90: 7420 6f66 2061 7574 6f2d 6765 6e65 7261  t of auto-genera
-00004ca0: 7465 6420 6576 656e 7473 2066 6f72 2064  ted events for d
-00004cb0: 7320 6c69 6220 7465 7374 696e 670a 2320  s lib testing.# 
-00004cc0: e294 9ce2 9480 e294 8020 506c 6169 6e20  ......... Plain 
-00004cd0: 6576 656e 7420 310a 2320 e294 94e2 9480  event 1.# ......
-00004ce0: e294 8020 506c 6169 6e20 6576 656e 7420  ... Plain event 
-00004cf0: 320a 2320 3c42 726f 6b65 6e45 7665 6e74  2.# <BrokenEvent
-00004d00: 3e0a 2320 e294 94e2 9480 e294 8020 4661  >.# ......... Fa
-00004d10: 6b65 2065 7665 6e74 0a23 203c 4272 6f6b  ke event.# <Brok
-00004d20: 656e 4576 656e 743e 0a23 20e2 9494 e294  enEvent>.# .....
-00004d30: 80e2 9480 2053 7475 6245 7665 6e74 2020  .... StubEvent  
-00004d40: 2020 3c2d 2d2d 2074 6865 2065 7665 6e74    <--- the event
-00004d50: 2074 6861 7420 7761 7320 6164 6465 6420   that was added 
-00004d60: 6162 6f76 650a 0a23 205b 332e 365d 2057  above..# [3.6] W
-00004d70: 6f72 6b69 6e67 2077 6974 6820 5061 7265  orking with Pare
-00004d80: 6e74 4576 656e 7454 7265 6543 6f6c 6c65  ntEventTreeColle
-00004d90: 6374 696f 6e2e 0a23 2050 6172 656e 7445  ction..# ParentE
-00004da0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-00004db0: 6f6e 2069 7320 6120 7472 6565 2063 6f6c  on is a tree col
-00004dc0: 6c65 6374 696f 6e20 6c69 6b65 2045 7665  lection like Eve
-00004dd0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00004de0: 2c0a 2320 6275 7420 6974 2068 6173 206f  ,.# but it has o
-00004df0: 6e6c 7920 6576 656e 7473 2074 6861 7420  nly events that 
-00004e00: 6861 7665 2072 6566 6572 656e 6365 732e  have references.
-00004e10: 0a64 6174 615f 736f 7572 6365 3a20 4944  .data_source: ID
-00004e20: 6174 6153 6f75 7263 6520 2023 2059 6f75  ataSource  # You
-00004e30: 2073 686f 756c 6420 696e 6974 2044 6174   should init Dat
-00004e40: 6153 6f75 7263 6520 6f62 6a65 6374 2e20  aSource object. 
-00004e50: 452e 672e 2066 726f 6d20 4c77 4450 206d  E.g. from LwDP m
-00004e60: 6f64 756c 652e 0a64 6174 615f 736f 7572  odule..data_sour
-00004e70: 6365 203d 2044 756d 6d79 4461 7461 536f  ce = DummyDataSo
-00004e80: 7572 6365 2829 2020 2320 4e6f 7465 2120  urce()  # Note! 
-00004e90: 5765 2075 7365 2066 616b 6520 4453 2068  We use fake DS h
-00004ea0: 6572 652e 0a23 2045 5443 4472 6976 6572  ere..# ETCDriver
-00004eb0: 2068 6572 6520 6973 2061 2073 7475 622c   here is a stub,
-00004ec0: 2061 6374 7561 6c6c 7920 7468 6520 6c69   actually the li
-00004ed0: 6220 646f 6573 6e27 7420 6861 7665 2073  b doesn't have s
-00004ee0: 7563 6820 6120 636c 6173 732e 0a23 2059  uch a class..# Y
-00004ef0: 6f75 2063 616e 2074 616b 6520 6974 2069  ou can take it i
-00004f00: 6e20 4c77 4450 206d 6f64 756c 6520 6f72  n LwDP module or
-00004f10: 2063 7265 6174 6520 796f 7572 7365 6c66   create yourself
-00004f20: 2063 6c61 7373 2069 6620 796f 7520 6861   class if you ha
-00004f30: 7665 2073 6f6d 6520 7370 6563 6961 6c20  ve some special 
-00004f40: 6576 656e 7473 2073 7472 7563 7475 7265  events structure
-00004f50: 2e0a 6672 6f6d 2074 6832 5f64 6174 615f  ..from th2_data_
-00004f60: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-00004f70: 7572 6365 2e6c 7764 702e 6576 656e 745f  urce.lwdp.event_
-00004f80: 7472 6565 2069 6d70 6f72 7420 4874 7470  tree import Http
-00004f90: 4554 4344 7269 7665 7220 6173 2045 5443  ETCDriver as ETC
-00004fa0: 4472 6976 6572 0a0a 6472 6976 6572 203d  Driver..driver =
-00004fb0: 2045 5443 4472 6976 6572 2864 6174 615f   ETCDriver(data_
-00004fc0: 736f 7572 6365 3d64 6174 615f 736f 7572  source=data_sour
-00004fd0: 6365 290a 7065 7463 203d 2050 6172 656e  ce).petc = Paren
-00004fe0: 7445 7665 6e74 5472 6565 436f 6c6c 6563  tEventTreeCollec
-00004ff0: 7469 6f6e 2864 7269 7665 7229 0a70 6574  tion(driver).pet
-00005000: 632e 6275 696c 6428 6576 656e 7473 290a  c.build(events).
-00005010: 0a70 6574 632e 7368 6f77 2829 0a70 6574  .petc.show().pet
-00005020: 632e 7375 6d6d 6172 7928 290a 0a23 2323  c.summary()..###
-00005030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005050: 2323 230a 2320 5b34 5d20 4669 656c 6420  ###.# [4] Field 
-00005060: 5265 736f 6c76 6572 730a 2323 2323 2323  Resolvers.######
-00005070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005090: 0a23 2050 6c65 6173 6520 7265 6164 2060  .# Please read `
-000050a0: 4669 656c 6420 5265 736f 6c76 6572 7360  Field Resolvers`
-000050b0: 2062 6c6f 636b 2069 6e20 7265 6164 6d65   block in readme
-000050c0: 2066 6972 7374 2e0a 0a23 205b 342e 315d   first...# [4.1]
-000050d0: 2055 7361 6765 2065 7861 6d70 6c65 2066   Usage example f
-000050e0: 726f 6d20 636c 6965 6e74 2063 6f64 650a  rom client code.
-000050f0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00005100: 7276 6963 6573 2e64 6174 615f 736f 7572  rvices.data_sour
-00005110: 6365 2069 6d70 6f72 7420 280a 2020 2020  ce import (.    
-00005120: 6c77 6470 2c0a 2920 2023 206c 7764 7020  lwdp,.)  # lwdp 
-00005130: 6461 7461 5f73 6f75 7263 6520 696e 6974  data_source init
-00005140: 6961 6c69 7a65 2074 6832 5f64 6174 615f  ialize th2_data_
-00005150: 7365 7276 6963 6573 2e63 6f6e 6669 6720  services.config 
-00005160: 6475 7269 6e67 2069 6d70 6f72 742e 0a66  during import..f
-00005170: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00005180: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
-00005190: 6f72 7420 6f70 7469 6f6e 7320 6173 206f  ort options as o
-000051a0: 5f0a 6672 6f6d 2074 6832 5f64 6174 615f  _.from th2_data_
-000051b0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-000051c0: 7572 6365 2e6c 7764 702e 7374 7562 5f62  urce.lwdp.stub_b
-000051d0: 7569 6c64 6572 2069 6d70 6f72 7420 6874  uilder import ht
-000051e0: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
-000051f0: 6275 696c 6465 720a 0a66 616b 655f 6461  builder..fake_da
-00005200: 7461 203d 205b 0a20 2020 2068 7474 705f  ta = [.    http_
-00005210: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
-00005220: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
-00005230: 7361 6765 4964 223a 2022 6122 2c20 226d  sageId": "a", "m
-00005240: 6573 7361 6765 5479 7065 223a 2022 526f  essageType": "Ro
-00005250: 6f74 227d 292c 0a20 2020 2068 7474 705f  ot"}),.    http_
+00003730: 0a23 205b 335d 2057 6f72 6b69 6e67 2077  .# [3] Working w
+00003740: 6974 6820 4576 656e 7454 7265 6520 616e  ith EventTree an
+00003750: 6420 4576 656e 7454 7265 6543 6f6c 6c65  d EventTreeColle
+00003760: 6374 696f 6e2e 0a23 2323 2323 2323 2323  ction..#########
+00003770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003780: 2323 2323 2323 2323 2323 2323 230a 2320  #############.# 
+00003790: 4361 6e20 6265 2075 7365 6675 6c20 6966  Can be useful if
+000037a0: 2079 6f75 2068 6176 6520 6461 7461 2d73   you have data-s
+000037b0: 7472 6561 6d20 7769 7468 203c 2031 3030  tream with < 100
+000037c0: 6b20 656c 656d 656e 7473 2c20 6f74 6865  k elements, othe
+000037d0: 7277 6973 6520 6974 0a23 2074 616b 6573  rwise it.# takes
+000037e0: 2074 6f6f 206d 7563 6820 5241 4d2e 0a0a   too much RAM...
+000037f0: 2320 5b33 2e31 5d20 4275 696c 6420 6120  # [3.1] Build a 
+00003800: 6375 7374 6f6d 2045 7665 6e74 5472 6565  custom EventTree
+00003810: 0a23 2054 6f20 6372 6561 7465 2061 6e20  .# To create an 
+00003820: 4576 656e 7454 7265 6520 6f62 6a65 6374  EventTree object
+00003830: 2079 6f75 206e 6565 6420 746f 2070 726f   you need to pro
+00003840: 7669 6465 206e 616d 652c 2069 6420 616e  vide name, id an
+00003850: 6420 6461 7461 206f 6620 7468 6520 726f  d data of the ro
+00003860: 6f74 2065 7665 6e74 2e0a 7472 6565 203d  ot event..tree =
+00003870: 2045 7665 6e74 5472 6565 2865 7665 6e74   EventTree(event
+00003880: 5f6e 616d 653d 2272 6f6f 7420 6576 656e  _name="root even
+00003890: 7422 2c20 6576 656e 745f 6964 3d22 726f  t", event_id="ro
+000038a0: 6f74 5f69 6422 2c0a 2020 2020 2020 2020  ot_id",.        
+000038b0: 2020 2020 2020 2020 2064 6174 613d 7b22           data={"
+000038c0: 6461 7461 223a 205b 312c 2032 2c20 332c  data": [1, 2, 3,
+000038d0: 2034 2c20 355d 7d29 0a0a 2320 546f 2061   4, 5]})..# To a
+000038e0: 6464 206e 6577 206e 6f64 6520 7573 6520  dd new node use 
+000038f0: 6170 7065 6e64 5f65 7665 6e74 2e20 7061  append_event. pa
+00003900: 7265 6e74 5f69 6420 6973 206e 6563 6573  rent_id is neces
+00003910: 7361 7279 2c20 6461 7461 2069 7320 6f70  sary, data is op
+00003920: 7469 6f6e 616c 2e0a 7472 6565 2e61 7070  tional..tree.app
+00003930: 656e 645f 6576 656e 7428 6576 656e 745f  end_event(event_
+00003940: 6e61 6d65 3d22 4122 2c20 6576 656e 745f  name="A", event_
+00003950: 6964 3d22 415f 6964 222c 2064 6174 613d  id="A_id", data=
+00003960: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00003970: 2020 2020 2020 2020 7061 7265 6e74 5f69          parent_i
+00003980: 643d 2272 6f6f 745f 6964 2229 0a0a 2320  d="root_id")..# 
+00003990: 5b33 2e33 5d20 4275 696c 6469 6e67 2074  [3.3] Building t
+000039a0: 6865 2045 7665 6e74 5472 6565 436f 6c6c  he EventTreeColl
+000039b0: 6563 7469 6f6e 2e0a 6461 7461 5f73 6f75  ection..data_sou
+000039c0: 7263 653a 2049 4461 7461 536f 7572 6365  rce: IDataSource
+000039d0: 2020 2320 596f 7520 7368 6f75 6c64 2069    # You should i
+000039e0: 6e69 7420 4461 7461 536f 7572 6365 206f  nit DataSource o
+000039f0: 626a 6563 742e 2045 2e67 2e20 6672 6f6d  bject. E.g. from
+00003a00: 204c 7744 5020 6d6f 6475 6c65 2e0a 6461   LwDP module..da
+00003a10: 7461 5f73 6f75 7263 6520 3d20 4475 6d6d  ta_source = Dumm
+00003a20: 7944 6174 6153 6f75 7263 6528 2920 2023  yDataSource()  #
+00003a30: 204e 6f74 6521 2057 6520 7573 6520 6661   Note! We use fa
+00003a40: 6b65 2044 5320 6865 7265 2e0a 2320 4554  ke DS here..# ET
+00003a50: 4344 7269 7665 7220 6865 7265 2069 7320  CDriver here is 
+00003a60: 6120 7374 7562 2c20 6163 7475 616c 6c79  a stub, actually
+00003a70: 2074 6865 206c 6962 2064 6f65 736e 2774   the lib doesn't
+00003a80: 2068 6176 6520 7375 6368 2061 2063 6c61   have such a cla
+00003a90: 7373 2e0a 2320 596f 7520 6361 6e20 7461  ss..# You can ta
+00003aa0: 6b65 2069 7420 696e 204c 7744 5020 6d6f  ke it in LwDP mo
+00003ab0: 6475 6c65 206f 7220 6372 6561 7465 2079  dule or create y
+00003ac0: 6f75 7273 656c 6620 636c 6173 7320 6966  ourself class if
+00003ad0: 2079 6f75 2068 6176 6520 736f 6d65 2073   you have some s
+00003ae0: 7065 6369 616c 2065 7665 6e74 7320 7374  pecial events st
+00003af0: 7275 6374 7572 652e 0a66 726f 6d20 7468  ructure..from th
+00003b00: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00003b10: 6461 7461 5f73 6f75 7263 652e 6c77 6470  data_source.lwdp
+00003b20: 2e65 7665 6e74 5f74 7265 6520 696d 706f  .event_tree impo
+00003b30: 7274 0a0a 4874 7470 4554 4344 7269 7665  rt..HttpETCDrive
+00003b40: 7220 6173 2045 5443 4472 6976 6572 0a0a  r as ETCDriver..
+00003b50: 2320 4966 2079 6f75 2064 6f6e 2774 2073  # If you don't s
+00003b60: 7065 6369 6679 2064 6174 615f 736f 7572  pecify data_sour
+00003b70: 6365 2066 6f72 2074 6865 2064 7269 7665  ce for the drive
+00003b80: 7220 7468 656e 2069 7420 776f 6e27 7420  r then it won't 
+00003b90: 7265 636f 7665 7220 6465 7461 6368 6564  recover detached
+00003ba0: 2065 7665 6e74 732e 0a64 7269 7665 723a   events..driver:
+00003bb0: 2049 4554 4344 7269 7665 7220 2023 2059   IETCDriver  # Y
+00003bc0: 6f75 2073 686f 756c 6420 696e 6974 2045  ou should init E
+00003bd0: 5443 4472 6976 6572 206f 626a 6563 742e  TCDriver object.
+00003be0: 2045 2e67 2e20 6672 6f6d 204c 7744 5020   E.g. from LwDP 
+00003bf0: 6d6f 6475 6c65 206f 7220 796f 7572 2063  module or your c
+00003c00: 7573 746f 6d20 636c 6173 732e 0a64 7269  ustom class..dri
+00003c10: 7665 7220 3d20 4554 4344 7269 7665 7228  ver = ETCDriver(
+00003c20: 6461 7461 5f73 6f75 7263 653d 6461 7461  data_source=data
+00003c30: 5f73 6f75 7263 652c 2075 7365 5f73 7475  _source, use_stu
+00003c40: 623d 5472 7565 290a 0a65 7463 203d 2045  b=True)..etc = E
+00003c50: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
+00003c60: 6f6e 2864 7269 7665 7229 0a65 7463 2e62  on(driver).etc.b
+00003c70: 7569 6c64 2865 7665 6e74 7329 0a65 7463  uild(events).etc
+00003c80: 2e73 686f 7728 290a 2320 4974 276c 6c20  .show().# It'll 
+00003c90: 7072 696e 7420 7468 6520 666f 6c6c 6f77  print the follow
+00003ca0: 696e 673a 0a23 2053 6574 206f 6620 6175  ing:.# Set of au
+00003cb0: 746f 2d67 656e 6572 6174 6564 2065 7665  to-generated eve
+00003cc0: 6e74 7320 666f 7220 6473 206c 6962 2074  nts for ds lib t
+00003cd0: 6573 7469 6e67 0a23 20e2 949c e294 80e2  esting.# .......
+00003ce0: 9480 2050 6c61 696e 2065 7665 6e74 2031  .. Plain event 1
+00003cf0: 0a23 20e2 9494 e294 80e2 9480 2050 6c61  .# ......... Pla
+00003d00: 696e 2065 7665 6e74 2032 0a0a 7072 696e  in event 2..prin
+00003d10: 7428 6574 6329 0a23 2045 7665 6e74 5472  t(etc).# EventTr
+00003d20: 6565 436f 6c6c 6563 7469 6f6e 2874 7265  eeCollection(tre
+00003d30: 6573 3d31 2c20 6576 656e 7473 3d33 5b74  es=1, events=3[t
+00003d40: 7265 6573 3d33 2c20 6465 7461 6368 6564  rees=3, detached
+00003d50: 3d30 5d29 0a0a 2320 4465 7461 6368 6564  =0])..# Detached
+00003d60: 2065 7665 6e74 7320 6973 6e27 7420 656d   events isn't em
+00003d70: 7074 792e 0a61 7373 6572 7420 6574 632e  pty..assert etc.
+00003d80: 6765 745f 6465 7461 6368 6564 5f65 7665  get_detached_eve
+00003d90: 6e74 7328 2920 2023 2072 6574 7572 6e73  nts()  # returns
+00003da0: 206c 6973 7420 6f66 2064 6574 6163 6865   list of detache
+00003db0: 645f 6576 656e 7473 2e0a 0a23 2072 6563  d_events...# rec
+00003dc0: 6f76 6572 5f75 6e6b 6e6f 776e 5f65 7665  over_unknown_eve
+00003dd0: 6e74 7320 2d2d 2075 7365 6420 746f 2072  nts -- used to r
+00003de0: 6563 6f76 6572 2073 6f6d 6520 6576 656e  ecover some even
+00003df0: 7473 2070 6172 656e 7473 2e0a 2320 5468  ts parents..# Th
+00003e00: 6174 2077 6f6e 2774 2077 6f72 6b20 7769  at won't work wi
+00003e10: 7468 2044 756d 6d79 4461 7461 536f 7572  th DummyDataSour
+00003e20: 6365 2c20 736f 2077 6173 2063 6f6d 6d65  ce, so was comme
+00003e30: 6e74 6564 0a23 2065 7463 2e72 6563 6f76  nted.# etc.recov
+00003e40: 6572 5f75 6e6b 6e6f 776e 5f65 7665 6e74  er_unknown_event
+00003e50: 7328 290a 0a23 2041 6674 6572 2074 6861  s()..# After tha
+00003e60: 7420 7468 6520 6465 7461 6368 6564 2065  t the detached e
+00003e70: 7665 6e74 7320 7368 6f75 6c64 2062 6520  vents should be 
+00003e80: 656d 7074 7920 6265 6361 7573 6520 7468  empty because th
+00003e90: 6579 2077 6572 6520 7265 636f 7665 7265  ey were recovere
+00003ea0: 642e 0a23 2061 7373 6572 7420 6e6f 7420  d..# assert not 
+00003eb0: 6574 632e 6765 745f 6465 7461 6368 6564  etc.get_detached
+00003ec0: 5f65 7665 6e74 7328 290a 0a23 202d 2d2d  _events()..# ---
+00003ed0: 2d2d 0a0a 2320 5468 6520 636f 6c6c 6563  --..# The collec
+00003ee0: 7469 6f6e 2068 6173 2045 7665 6e74 5472  tion has EventTr
+00003ef0: 6565 7320 6561 6368 2077 6974 6820 6120  ees each with a 
+00003f00: 7472 6565 206f 6620 6576 656e 7473 2e0a  tree of events..
+00003f10: 2320 5573 696e 6720 436f 6c6c 6563 7469  # Using Collecti
+00003f20: 6f6e 2061 6e64 2045 7665 6e74 5472 6565  on and EventTree
+00003f30: 732c 2079 6f75 2063 616e 2077 6f72 6b20  s, you can work 
+00003f40: 666c 6578 6962 6c79 2077 6974 6820 6576  flexibly with ev
+00003f50: 656e 7473 2e0a 0a23 205b 332e 332e 315d  ents...# [3.3.1]
+00003f60: 2047 6574 206c 6561 7665 7320 6f66 2061   Get leaves of a
+00003f70: 6c6c 2074 7265 6573 2e0a 6c65 6176 6573  ll trees..leaves
+00003f80: 3a20 5475 706c 655b 6469 6374 5d20 3d20  : Tuple[dict] = 
+00003f90: 6574 632e 6765 745f 6c65 6176 6573 2829  etc.get_leaves()
+00003fa0: 2020 2320 5265 7475 726e 7320 6120 7475    # Returns a tu
+00003fb0: 706c 6520 6f66 206c 6561 7665 7320 6576  ple of leaves ev
+00003fc0: 656e 7473 0a0a 2320 5b33 2e33 2e32 5d20  ents..# [3.3.2] 
+00003fd0: 4765 7420 726f 6f74 7320 6964 7320 6f66  Get roots ids of
+00003fe0: 2061 6c6c 2074 7265 6573 2e0a 726f 6f74   all trees..root
+00003ff0: 733a 204c 6973 745b 7374 725d 203d 2065  s: List[str] = e
+00004000: 7463 2e67 6574 5f72 6f6f 7473 5f69 6473  tc.get_roots_ids
+00004010: 2829 0a23 2052 6574 7572 6e73 2074 6865  ().# Returns the
+00004020: 206c 6973 7420 6f66 2072 6f6f 7420 4964   list of root Id
+00004030: 733a 0a23 205b 2764 656d 6f5f 626f 6f6b  s:.# ['demo_book
+00004040: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00004050: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+00004060: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+00004070: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+00004080: 6136 3135 3531 3532 645f 3127 5d0a 0a23  a6155152d_1']..#
+00004090: 205b 332e 332e 335d 2046 696e 6420 616e   [3.3.3] Find an
+000040a0: 2065 7665 6e74 2069 6e20 616c 6c20 7472   event in all tr
+000040b0: 6565 732e 0a66 696e 645f 6576 656e 743a  ees..find_event:
+000040c0: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
+000040d0: 3d20 6574 632e 6669 6e64 280a 2020 2020  = etc.find(.    
+000040e0: 6c61 6d62 6461 2065 7665 6e74 3a20 2253  lambda event: "S
+000040f0: 656e 6420 6d65 7373 6167 6522 2069 6e20  end message" in 
+00004100: 6576 656e 745b 2265 7665 6e74 5479 7065  event["eventType
+00004110: 225d 290a 0a23 205b 332e 332e 345d 2046  "])..# [3.3.4] F
+00004120: 696e 6420 616c 6c20 6576 656e 7473 2069  ind all events i
+00004130: 6e20 616c 6c20 7472 6565 732e 2054 6865  n all trees. The
+00004140: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
+00004150: 626c 6520 7665 7273 696f 6e20 2766 696e  ble version 'fin
+00004160: 6461 6c6c 5f69 7465 7227 2e0a 6669 6e64  dall_iter'..find
+00004170: 5f65 7665 6e74 733a 204c 6973 745b 6469  _events: List[di
+00004180: 6374 5d20 3d20 6574 632e 6669 6e64 616c  ct] = etc.findal
+00004190: 6c28 6c61 6d62 6461 2065 7665 6e74 3a20  l(lambda event: 
+000041a0: 6576 656e 745b 2273 7563 6365 7373 6675  event["successfu
+000041b0: 6c22 5d20 6973 2054 7275 6529 0a0a 2320  l"] is True)..# 
+000041c0: 5b33 2e33 2e35 5d20 4669 6e64 2061 6e20  [3.3.5] Find an 
+000041d0: 616e 6365 7374 6f72 206f 6620 7468 6520  ancestor of the 
+000041e0: 6576 656e 742e 0a61 6e63 6573 746f 723a  event..ancestor:
+000041f0: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
+00004200: 3d20 6574 632e 6669 6e64 5f61 6e63 6573  = etc.find_ances
+00004210: 746f 7228 0a20 2020 2022 6465 6d6f 5f62  tor(.    "demo_b
+00004220: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00004230: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+00004240: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+00004250: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+00004260: 6433 3461 3631 3535 3135 3264 5f31 222c  d34a6155152d_1",
+00004270: 0a20 2020 2066 696c 7465 723d 6c61 6d62  .    filter=lamb
+00004280: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
+00004290: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
+000042a0: 6576 656e 744e 616d 6522 5d2c 0a29 0a0a  eventName"],.)..
+000042b0: 2320 5b33 2e33 2e36 5d20 4765 7420 6368  # [3.3.6] Get ch
+000042c0: 696c 6472 656e 206f 6620 7468 6520 6576  ildren of the ev
+000042d0: 656e 742e 2054 6865 7265 2069 7320 616c  ent. There is al
+000042e0: 736f 2069 7465 7261 626c 6520 7665 7273  so iterable vers
+000042f0: 696f 6e20 2767 6574 5f63 6869 6c64 7265  ion 'get_childre
+00004300: 6e5f 6974 6572 272e 0a63 6869 6c64 7265  n_iter'..childre
+00004310: 6e3a 2054 7570 6c65 5b64 6963 745d 203d  n: Tuple[dict] =
+00004320: 2065 7463 2e67 6574 5f63 6869 6c64 7265   etc.get_childre
+00004330: 6e28 0a20 2020 2022 6465 6d6f 5f62 6f6f  n(.    "demo_boo
+00004340: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
+00004350: 3233 3031 3035 3133 3537 3035 3536 3038  2301051357055608
+00004360: 3733 3030 303a 6436 3165 3933 3061 2d38  73000:d61e930a-8
+00004370: 6430 302d 3131 6564 2d61 6131 612d 6433  d00-11ed-aa1a-d3
+00004380: 3461 3631 3535 3135 3264 5f31 220a 290a  4a6155152d_1".).
+00004390: 0a23 205b 332e 332e 375d 2047 6574 2073  .# [3.3.7] Get s
+000043a0: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
+000043b0: 6669 6564 2065 7665 6e74 2e0a 7375 6274  fied event..subt
+000043c0: 7265 653a 2045 7665 6e74 5472 6565 203d  ree: EventTree =
+000043d0: 2065 7463 2e67 6574 5f73 7562 7472 6565   etc.get_subtree
+000043e0: 280a 2020 2020 2264 656d 6f5f 626f 6f6b  (.    "demo_book
+000043f0: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00004400: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+00004410: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+00004420: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+00004430: 6136 3135 3531 3532 645f 3122 0a29 0a0a  a6155152d_1".)..
+00004440: 2320 5b33 2e33 2e38 5d20 4765 7420 6675  # [3.3.8] Get fu
+00004450: 6c6c 2070 6174 6820 746f 2074 6865 2065  ll path to the e
+00004460: 7665 6e74 2e0a 2320 4c6f 6f6b 7320 6c69  vent..# Looks li
+00004470: 6b65 205b 616e 6365 7374 6f72 5f72 6f6f  ke [ancestor_roo
+00004480: 742c 2061 6e63 6573 746f 725f 6c65 7665  t, ancestor_leve
+00004490: 6c31 2c20 616e 6365 7374 6f72 5f6c 6576  l1, ancestor_lev
+000044a0: 656c 322c 2065 7665 6e74 5d0a 6576 656e  el2, event].even
+000044b0: 745f 7061 7468 3a20 4c69 7374 5b64 6963  t_path: List[dic
+000044c0: 745d 203d 2065 7463 2e67 6574 5f66 756c  t] = etc.get_ful
+000044d0: 6c5f 7061 7468 280a 2020 2020 2264 656d  l_path(.    "dem
+000044e0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
+000044f0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
+00004500: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
+00004510: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
+00004520: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
+00004530: 3122 0a29 0a0a 2320 5b33 2e33 2e39 5d20  1".)..# [3.3.9] 
+00004540: 4765 7420 7061 7265 6e74 206f 6620 7468  Get parent of th
+00004550: 6520 6576 656e 742e 0a70 6172 656e 7420  e event..parent 
+00004560: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
+00004570: 280a 2020 2020 2264 656d 6f5f 626f 6f6b  (.    "demo_book
+00004580: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00004590: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
+000045a0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
+000045b0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
+000045c0: 6136 3135 3531 3532 645f 3122 0a29 0a0a  a6155152d_1".)..
+000045d0: 2320 5b33 2e33 2e31 305d 2041 7070 656e  # [3.3.10] Appen
+000045e0: 6420 6e65 7720 6576 656e 7420 746f 2074  d new event to t
+000045f0: 6865 2063 6f6c 6c65 6374 696f 6e2e 0a65  he collection..e
+00004600: 7463 2e61 7070 656e 645f 6576 656e 7428  tc.append_event(
+00004610: 0a20 2020 2065 7665 6e74 3d7b 0a20 2020  .    event={.   
+00004620: 2020 2020 2022 6576 656e 7449 6422 3a20       "eventId": 
+00004630: 2261 3230 6635 6566 342d 6333 6665 2d62  "a20f5ef4-c3fe-b
+00004640: 6231 302d 6132 3963 2d64 6433 6437 3834  b10-a29c-dd3d784
+00004650: 3930 3965 6222 2c0a 2020 2020 2020 2020  909eb",.        
+00004660: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
+00004670: 2022 3865 3235 3234 6661 2d63 6635 392d   "8e2524fa-cf59-
+00004680: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
+00004690: 3463 3361 3632 222c 0a20 2020 2020 2020  4c3a62",.       
+000046a0: 2022 6576 656e 744e 616d 6522 3a20 2253   "eventName": "S
+000046b0: 7475 6245 7665 6e74 222c 0a20 2020 207d  tubEvent",.    }
+000046c0: 0a29 0a0a 2320 5b33 2e33 2e31 315d 2053  .)..# [3.3.11] S
+000046d0: 686f 7720 7468 6520 656e 7469 7265 2063  how the entire c
+000046e0: 6f6c 6c65 6374 696f 6e2e 0a65 7463 2e73  ollection..etc.s
+000046f0: 686f 7728 290a 2320 4974 276c 6c20 7072  how().# It'll pr
+00004700: 696e 7420 7468 6520 666f 6c6c 6f77 696e  int the followin
+00004710: 673a 0a23 2053 6574 206f 6620 6175 746f  g:.# Set of auto
+00004720: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
+00004730: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
+00004740: 7469 6e67 0a23 20e2 949c e294 80e2 9480  ting.# .........
+00004750: 2050 6c61 696e 2065 7665 6e74 2031 0a23   Plain event 1.#
+00004760: 20e2 9494 e294 80e2 9480 2050 6c61 696e   ......... Plain
+00004770: 2065 7665 6e74 2032 0a0a 2320 4173 2079   event 2..# As y
+00004780: 6f75 2063 616e 2073 6565 2c20 6e6f 7468  ou can see, noth
+00004790: 696e 6720 7761 7320 6368 616e 6765 642c  ing was changed,
+000047a0: 2062 7574 2077 6520 6164 6465 6420 7468   but we added th
+000047b0: 6520 6e65 7720 6576 656e 7421 0a23 206c  e new event!.# l
+000047c0: 6574 2773 206c 6f6f 6b20 6174 2074 6865  et's look at the
+000047d0: 2073 756d 6d61 7279 2e0a 0a70 7269 6e74   summary...print
+000047e0: 2865 7463 2e73 756d 6d61 7279 2829 2920  (etc.summary()) 
+000047f0: 2023 2074 6865 2073 616d 6520 6173 206a   # the same as j
+00004800: 7573 7420 7072 696e 7428 6574 6329 0a23  ust print(etc).#
+00004810: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00004820: 7469 6f6e 2874 7265 6573 3d31 2c20 6576  tion(trees=1, ev
+00004830: 656e 7473 3d35 5b74 7265 6573 3d33 2c20  ents=5[trees=3, 
+00004840: 6465 7461 6368 6564 3d32 5d29 0a23 2059  detached=2]).# Y
+00004850: 6f75 2063 616e 2073 6565 2074 6861 7420  ou can see that 
+00004860: 6974 2077 6173 2061 6464 6564 2074 6f20  it was added to 
+00004870: 6465 7461 6368 6564 2e20 5468 6174 2773  detached. That's
+00004880: 2077 6879 2079 6f75 2064 6f6e 2774 2073   why you don't s
+00004890: 6565 2074 6865 2065 7665 6e74 0a23 2076  ee the event.# v
+000048a0: 6961 2060 7368 6f77 2829 602e 2060 7368  ia `show()`. `sh
+000048b0: 6f77 2829 6020 7072 696e 7473 206f 6e6c  ow()` prints onl
+000048c0: 7920 5472 6565 7321 0a23 2055 7365 2060  y Trees!.# Use `
+000048d0: 6574 632e 6765 745f 7061 7265 6e74 6c65  etc.get_parentle
+000048e0: 7373 5f74 7265 6573 2829 6020 746f 2063  ss_trees()` to c
+000048f0: 6f6e 7665 7274 2064 6574 6163 6865 6420  onvert detached 
+00004900: 6576 656e 7473 2074 6f20 7472 6565 732e  events to trees.
+00004910: 0a23 204d 6f72 6520 696e 666f 726d 6174  .# More informat
+00004920: 696f 6e20 6265 6c6f 7720 696e 2074 6865  ion below in the
+00004930: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
+00004940: 6563 7469 6f6e 2e0a 0a23 202d 2d2d 2d2d  ection...# -----
+00004950: 2d2d 2d2d 2d2d 2d2d 2d0a 2320 5b33 2e34  ---------.# [3.4
+00004960: 5d20 576f 726b 696e 6720 7769 7468 2074  ] Working with t
+00004970: 6865 2045 7665 6e74 5472 6565 2e0a 2320  he EventTree..# 
+00004980: 4576 656e 7454 7265 6520 6861 7320 7468  EventTree has th
+00004990: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+000049a0: 7320 4576 656e 7454 7265 6543 6f6c 6c65  s EventTreeColle
+000049b0: 6374 696f 6e2c 2062 7574 206f 6e6c 7920  ction, but only 
+000049c0: 666f 7220 6974 7320 6f77 6e20 7472 6565  for its own tree
+000049d0: 2e0a 0a23 205b 332e 342e 315d 2047 6574  ...# [3.4.1] Get
+000049e0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
+000049f0: 2074 7265 6573 2e0a 7472 6565 733a 204c   trees..trees: L
+00004a00: 6973 745b 4576 656e 7454 7265 655d 203d  ist[EventTree] =
+00004a10: 2065 7463 2e67 6574 5f74 7265 6573 2829   etc.get_trees()
+00004a20: 0a74 7265 653a 2045 7665 6e74 5472 6565  .tree: EventTree
+00004a30: 203d 2074 7265 6573 5b30 5d0a 0a23 2042   = trees[0]..# B
+00004a40: 7574 2045 7665 6e74 5472 6565 2070 726f  ut EventTree pro
+00004a50: 7669 6465 7320 6120 776f 726b 2077 6974  vides a work wit
+00004a60: 6820 7468 6520 7472 6565 2c20 6275 7420  h the tree, but 
+00004a70: 646f 6573 206e 6f74 206d 6f64 6966 7920  does not modify 
+00004a80: 6974 2e0a 2320 4966 2079 6f75 2077 616e  it..# If you wan
+00004a90: 7420 746f 206d 6f64 6966 7920 7468 6520  t to modify the 
+00004aa0: 7472 6565 2c20 7573 6520 4576 656e 7454  tree, use EventT
+00004ab0: 7265 6543 6f6c 6c65 6374 696f 6e73 2e0a  reeCollections..
+00004ac0: 0a23 205b 332e 355d 2057 6f72 6b69 6e67  .# [3.5] Working
+00004ad0: 2077 6974 6820 5061 7265 6e74 6c65 7373   with Parentless
+00004ae0: 5472 6565 2e0a 2320 5061 7265 6e74 6c65  Tree..# Parentle
+00004af0: 7373 5472 6565 2069 7320 616e 2045 7665  ssTree is an Eve
+00004b00: 6e74 5472 6565 2074 6861 7420 6861 7320  ntTree that has 
+00004b10: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
+00004b20: 7769 7468 2073 7475 6273 2e0a 7061 7265  with stubs..pare
+00004b30: 6e74 6c65 7373 5f74 7265 6573 3a20 4c69  ntless_trees: Li
+00004b40: 7374 5b45 7665 6e74 5472 6565 5d20 3d20  st[EventTree] = 
+00004b50: 6574 632e 6765 745f 7061 7265 6e74 6c65  etc.get_parentle
+00004b60: 7373 5f74 7265 6573 2829 0a70 7269 6e74  ss_trees().print
+00004b70: 2822 7061 7265 6e74 6c65 7373 5f74 7265  ("parentless_tre
+00004b80: 6573 2063 6f6e 7461 696e 733a 2229 0a70  es contains:").p
+00004b90: 7269 6e74 2870 6172 656e 746c 6573 735f  rint(parentless_
+00004ba0: 7472 6565 7329 0a23 205b 4576 656e 7454  trees).# [EventT
+00004bb0: 7265 6528 6e61 6d65 3d27 3c42 726f 6b65  ree(name='<Broke
+00004bc0: 6e45 7665 6e74 3e27 2c20 726f 6f74 5f69  nEvent>', root_i
+00004bd0: 643d 276e 6f74 5f65 7869 7374 735f 696e  d='not_exists_in
+00004be0: 5f74 6865 5f65 7665 6e74 735f 7374 7265  _the_events_stre
+00004bf0: 616d 272c 2065 7665 6e74 733d 3229 2c0a  am', events=2),.
+00004c00: 2320 2045 7665 6e74 5472 6565 286e 616d  #  EventTree(nam
+00004c10: 653d 273c 4272 6f6b 656e 4576 656e 743e  e='<BrokenEvent>
+00004c20: 272c 2072 6f6f 745f 6964 3d27 3865 3235  ', root_id='8e25
+00004c30: 3234 6661 2d63 6635 392d 3131 6562 2d61  24fa-cf59-11eb-a
+00004c40: 3366 372d 3039 3466 3930 3463 3361 3632  3f7-094f904c3a62
+00004c50: 272c 2065 7665 6e74 733d 3229 5d0a 0a70  ', events=2)]..p
+00004c60: 7269 6e74 2822 5c6e 2220 2265 7463 2061  rint("\n" "etc a
+00004c70: 6674 6572 2060 6765 745f 7061 7265 6e74  fter `get_parent
+00004c80: 6c65 7373 5f74 7265 6573 603a 2229 0a70  less_trees`:").p
+00004c90: 7269 6e74 2865 7463 2e73 756d 6d61 7279  rint(etc.summary
+00004ca0: 2829 290a 2320 4576 656e 7454 7265 6543  ()).# EventTreeC
+00004cb0: 6f6c 6c65 6374 696f 6e28 7472 6565 733d  ollection(trees=
+00004cc0: 335b 7265 6775 6c61 723d 312c 2070 6172  3[regular=1, par
+00004cd0: 656e 746c 6573 733d 325d 2c20 6576 656e  entless=2], even
+00004ce0: 7473 3d37 5b74 7265 6573 3d37 2c20 6465  ts=7[trees=7, de
+00004cf0: 7461 6368 6564 3d30 5d29 270a 6574 632e  tached=0])'.etc.
+00004d00: 7368 6f77 2829 0a23 2053 6574 206f 6620  show().# Set of 
+00004d10: 6175 746f 2d67 656e 6572 6174 6564 2065  auto-generated e
+00004d20: 7665 6e74 7320 666f 7220 6473 206c 6962  vents for ds lib
+00004d30: 2074 6573 7469 6e67 0a23 20e2 949c e294   testing.# .....
+00004d40: 80e2 9480 2050 6c61 696e 2065 7665 6e74  .... Plain event
+00004d50: 2031 0a23 20e2 9494 e294 80e2 9480 2050   1.# ......... P
+00004d60: 6c61 696e 2065 7665 6e74 2032 0a23 203c  lain event 2.# <
+00004d70: 4272 6f6b 656e 4576 656e 743e 0a23 20e2  BrokenEvent>.# .
+00004d80: 9494 e294 80e2 9480 2046 616b 6520 6576  ........ Fake ev
+00004d90: 656e 740a 2320 3c42 726f 6b65 6e45 7665  ent.# <BrokenEve
+00004da0: 6e74 3e0a 2320 e294 94e2 9480 e294 8020  nt>.# ......... 
+00004db0: 5374 7562 4576 656e 7420 2020 203c 2d2d  StubEvent    <--
+00004dc0: 2d20 7468 6520 6576 656e 7420 7468 6174  - the event that
+00004dd0: 2077 6173 2061 6464 6564 2061 626f 7665   was added above
+00004de0: 0a0a 2320 5b33 2e36 5d20 576f 726b 696e  ..# [3.6] Workin
+00004df0: 6720 7769 7468 2050 6172 656e 7445 7665  g with ParentEve
+00004e00: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00004e10: 2e0a 2320 5061 7265 6e74 4576 656e 7454  ..# ParentEventT
+00004e20: 7265 6543 6f6c 6c65 6374 696f 6e20 6973  reeCollection is
+00004e30: 2061 2074 7265 6520 636f 6c6c 6563 7469   a tree collecti
+00004e40: 6f6e 206c 696b 6520 4576 656e 7454 7265  on like EventTre
+00004e50: 6543 6f6c 6c65 6374 696f 6e2c 0a23 2062  eCollection,.# b
+00004e60: 7574 2069 7420 6861 7320 6f6e 6c79 2065  ut it has only e
+00004e70: 7665 6e74 7320 7468 6174 2068 6176 6520  vents that have 
+00004e80: 7265 6665 7265 6e63 6573 2e0a 6461 7461  references..data
+00004e90: 5f73 6f75 7263 653a 2049 4461 7461 536f  _source: IDataSo
+00004ea0: 7572 6365 2020 2320 596f 7520 7368 6f75  urce  # You shou
+00004eb0: 6c64 2069 6e69 7420 4461 7461 536f 7572  ld init DataSour
+00004ec0: 6365 206f 626a 6563 742e 2045 2e67 2e20  ce object. E.g. 
+00004ed0: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
+00004ee0: 2e0a 6461 7461 5f73 6f75 7263 6520 3d20  ..data_source = 
+00004ef0: 4475 6d6d 7944 6174 6153 6f75 7263 6528  DummyDataSource(
+00004f00: 2920 2023 204e 6f74 6521 2057 6520 7573  )  # Note! We us
+00004f10: 6520 6661 6b65 2044 5320 6865 7265 2e0a  e fake DS here..
+00004f20: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
+00004f30: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
+00004f40: 616c 6c79 2074 6865 206c 6962 2064 6f65  ally the lib doe
+00004f50: 736e 2774 2068 6176 6520 7375 6368 2061  sn't have such a
+00004f60: 2063 6c61 7373 2e0a 2320 596f 7520 6361   class..# You ca
+00004f70: 6e20 7461 6b65 2069 7420 696e 204c 7744  n take it in LwD
+00004f80: 5020 6d6f 6475 6c65 206f 7220 6372 6561  P module or crea
+00004f90: 7465 2079 6f75 7273 656c 6620 636c 6173  te yourself clas
+00004fa0: 7320 6966 2079 6f75 2068 6176 6520 736f  s if you have so
+00004fb0: 6d65 2073 7065 6369 616c 2065 7665 6e74  me special event
+00004fc0: 7320 7374 7275 6374 7572 652e 0a66 726f  s structure..fro
+00004fd0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+00004fe0: 6365 732e 6461 7461 5f73 6f75 7263 652e  ces.data_source.
+00004ff0: 6c77 6470 2e65 7665 6e74 5f74 7265 6520  lwdp.event_tree 
+00005000: 696d 706f 7274 0a0a 4874 7470 4554 4344  import..HttpETCD
+00005010: 7269 7665 7220 6173 2045 5443 4472 6976  river as ETCDriv
+00005020: 6572 0a0a 6472 6976 6572 203d 2045 5443  er..driver = ETC
+00005030: 4472 6976 6572 2864 6174 615f 736f 7572  Driver(data_sour
+00005040: 6365 3d64 6174 615f 736f 7572 6365 290a  ce=data_source).
+00005050: 7065 7463 203d 2050 6172 656e 7445 7665  petc = ParentEve
+00005060: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00005070: 2864 7269 7665 7229 0a70 6574 632e 6275  (driver).petc.bu
+00005080: 696c 6428 6576 656e 7473 290a 0a70 6574  ild(events)..pet
+00005090: 632e 7368 6f77 2829 0a70 6574 632e 7375  c.show().petc.su
+000050a0: 6d6d 6172 7928 290a 0a23 2323 2323 2323  mmary()..#######
+000050b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000050c0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000050d0: 2320 5b34 5d20 4669 656c 6420 5265 736f  # [4] Field Reso
+000050e0: 6c76 6572 730a 2323 2323 2323 2323 2323  lvers.##########
+000050f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005100: 2323 2323 2323 2323 2323 2323 0a23 2050  ############.# P
+00005110: 6c65 6173 6520 7265 6164 2060 4669 656c  lease read `Fiel
+00005120: 6420 5265 736f 6c76 6572 7360 2062 6c6f  d Resolvers` blo
+00005130: 636b 2069 6e20 7265 6164 6d65 2066 6972  ck in readme fir
+00005140: 7374 2e0a 0a23 205b 342e 315d 2055 7361  st...# [4.1] Usa
+00005150: 6765 2065 7861 6d70 6c65 2066 726f 6d20  ge example from 
+00005160: 636c 6965 6e74 2063 6f64 650a 6672 6f6d  client code.from
+00005170: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00005180: 6573 2e64 6174 615f 736f 7572 6365 2069  es.data_source i
+00005190: 6d70 6f72 7420 280a 2020 2020 6c77 6470  mport (.    lwdp
+000051a0: 2c0a 2920 2023 206c 7764 7020 6461 7461  ,.)  # lwdp data
+000051b0: 5f73 6f75 7263 6520 696e 6974 6961 6c69  _source initiali
+000051c0: 7a65 2074 6832 5f64 6174 615f 7365 7276  ze th2_data_serv
+000051d0: 6963 6573 2e63 6f6e 6669 6720 6475 7269  ices.config duri
+000051e0: 6e67 2069 6d70 6f72 742e 0a66 726f 6d20  ng import..from 
+000051f0: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
+00005200: 732e 636f 6e66 6967 2069 6d70 6f72 7420  s.config import 
+00005210: 6f70 7469 6f6e 7320 6173 206f 5f0a 6672  options as o_.fr
+00005220: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00005230: 6963 6573 2e64 6174 615f 736f 7572 6365  ices.data_source
+00005240: 2e6c 7764 702e 7374 7562 5f62 7569 6c64  .lwdp.stub_build
+00005250: 6572 2069 6d70 6f72 740a 0a68 7474 705f  er import..http_
 00005260: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
-00005270: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
-00005280: 7361 6765 4964 223a 2022 6222 2c20 226d  sageId": "b", "m
-00005290: 6573 7361 6765 5479 7065 223a 2022 4e65  essageType": "Ne
-000052a0: 7722 7d29 2c0a 2020 2020 6874 7470 5f6d  w"}),.    http_m
-000052b0: 6573 7361 6765 5f73 7475 625f 6275 696c  essage_stub_buil
-000052c0: 6465 722e 6275 696c 6428 7b22 6d65 7373  der.build({"mess
-000052d0: 6167 6549 6422 3a20 2263 222c 2022 6d65  ageId": "c", "me
-000052e0: 7373 6167 6554 7970 6522 3a20 2241 6d65  ssageType": "Ame
-000052f0: 6e64 227d 292c 0a20 2020 2068 7474 705f  nd"}),.    http_
-00005300: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
-00005310: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
-00005320: 7361 6765 4964 223a 2022 6422 2c20 226d  sageId": "d", "m
-00005330: 6573 7361 6765 5479 7065 223a 2022 4361  essageType": "Ca
-00005340: 6e63 656c 227d 292c 0a5d 0a66 616b 655f  ncel"}),.].fake_
-00005350: 6461 7461 5f6f 626a 203d 2044 6174 6128  data_obj = Data(
-00005360: 6661 6b65 5f64 6174 6129 0a0a 666f 7220  fake_data)..for 
-00005370: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
-00005380: 626a 3a0a 2020 2020 6f5f 2e6d 6672 2e65  bj:.    o_.mfr.e
-00005390: 7870 616e 645f 6d65 7373 6167 6528 6d29  xpand_message(m)
-000053a0: 2020 2320 6d66 7220 2d20 7374 616e 6473    # mfr - stands
-000053b0: 2066 6f72 204d 6573 7361 6765 4669 656c   for MessageFiel
-000053c0: 6452 6573 6f6c 7665 720a 2320 6f72 0a66  dResolver.# or.f
-000053d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
-000053e0: 615f 6f62 6a2e 6d61 7028 6f5f 2e6d 6672  a_obj.map(o_.mfr
-000053f0: 2e65 7870 616e 645f 6d65 7373 6167 6529  .expand_message)
-00005400: 3a0a 2020 2020 7061 7373 0a0a 2320 5b34  :.    pass..# [4
-00005410: 2e32 5d20 4c69 6272 6172 6965 7320 7573  .2] Libraries us
-00005420: 6167 652e 0a23 2044 6f6e 2774 2069 6d70  age..# Don't imp
-00005430: 6f72 7420 6578 6163 7420 7265 736f 6c76  ort exact resolv
-00005440: 6572 7320 696d 706c 656d 656e 7461 7469  ers implementati
-00005450: 6f6e 2069 6e20 796f 7572 2063 6f64 652c  on in your code,
-00005460: 2070 6c65 6173 652e 0a23 2041 6c6c 6f77   please..# Allow
-00005470: 2079 6f75 7220 636c 6965 6e74 2074 6f20   your client to 
-00005480: 646f 2069 7420 696e 7374 6561 642e 0a23  do it instead..#
-00005490: 204a 7573 7420 696d 706f 7274 2060 6f70   Just import `op
-000054a0: 7469 6f6e 7360 2066 726f 6d20 6074 6832  tions` from `th2
-000054b0: 5f64 6174 615f 7365 7276 6963 6573 2e63  _data_services.c
-000054c0: 6f6e 6669 6760 2061 6e64 2075 7365 2069  onfig` and use i
-000054d0: 742e 0a66 726f 6d20 7468 325f 6461 7461  t..from th2_data
-000054e0: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
-000054f0: 2069 6d70 6f72 7420 6f70 7469 6f6e 7320   import options 
-00005500: 6173 206f 5f0a 0a66 6f72 206d 2069 6e20  as o_..for m in 
-00005510: 6661 6b65 5f64 6174 615f 6f62 6a3a 0a20  fake_data_obj:. 
-00005520: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
-00005530: 5f6d 6573 7361 6765 286d 290a 2320 6f72  _message(m).# or
-00005540: 0a66 6f72 206d 2069 6e20 6661 6b65 5f64  .for m in fake_d
-00005550: 6174 615f 6f62 6a2e 6d61 7028 6f5f 2e6d  ata_obj.map(o_.m
-00005560: 6672 2e65 7870 616e 645f 6d65 7373 6167  fr.expand_messag
-00005570: 6529 3a0a 2020 2020 7061 7373 0a0a 2320  e):.    pass..# 
-00005580: 4d6f 7265 2074 6563 6820 6465 7461 696c  More tech detail
-00005590: 733a 0a23 2020 2049 6e20 7468 6973 2063  s:.#   In this c
-000055a0: 6173 652c 2074 6865 7265 2069 7320 6e6f  ase, there is no
-000055b0: 206c 696e 6520 6066 726f 6d20 7468 325f   line `from th2_
-000055c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
-000055d0: 7461 5f73 6f75 7263 6520 696d 706f 7274  ta_source import
-000055e0: 206c 7764 7020 600a 2320 2020 6265 6361   lwdp `.#   beca
-000055f0: 7573 6520 7765 2073 686f 756c 6420 6e6f  use we should no
-00005600: 7420 6368 6f6f 7365 2066 6f72 2074 6865  t choose for the
-00005610: 2075 7365 7220 7768 6963 6820 6120 6461   user which a da
-00005620: 7461 2073 6f75 7263 6520 746f 2075 7365  ta source to use
-00005630: 2e0a 2320 2020 5765 2064 6f20 6e6f 7420  ..#   We do not 
-00005640: 6b6e 6f77 2077 6861 7420 6865 2077 696c  know what he wil
-00005650: 6c20 6368 6f6f 7365 2c20 7468 6572 6566  l choose, theref
-00005660: 6f72 652c 2077 6520 6d75 7374 2073 696d  ore, we must sim
-00005670: 706c 7920 6163 6365 7373 0a23 2020 2074  ply access.#   t
-00005680: 6865 2069 6e74 6572 6661 6365 2c20 7768  he interface, wh
-00005690: 6963 6820 7769 6c6c 2062 6520 696e 6974  ich will be init
-000056a0: 6961 6c69 7a65 6420 6279 2074 6865 2075  ialized by the u
-000056b0: 7365 722e 0a0a 2323 2323 2323 2323 2323  ser...##########
-000056c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000056d0: 2323 2323 2323 2323 2323 2323 0a23 205b  ############.# [
-000056e0: 355d 2055 7369 6e67 2075 7469 6c69 7479  5] Using utility
-000056f0: 2066 756e 6374 696f 6e73 2e0a 2323 2323   functions..####
-00005700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005710: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00005720: 2323 0a66 726f 6d20 7468 325f 6461 7461  ##.from th2_data
-00005730: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
-00005740: 6576 656e 745f 7574 696c 732e 6672 6571  event_utils.freq
-00005750: 7565 6e63 6965 7320 696d 706f 7274 2067  uencies import g
-00005760: 6574 5f63 6174 6567 6f72 795f 6672 6571  et_category_freq
-00005770: 7565 6e63 6965 7332 0a66 726f 6d20 7468  uencies2.from th
-00005780: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00005790: 7574 696c 732e 6576 656e 745f 7574 696c  utils.event_util
-000057a0: 732e 746f 7461 6c73 2069 6d70 6f72 7420  s.totals import 
-000057b0: 6765 745f 6361 7465 676f 7279 5f74 6f74  get_category_tot
-000057c0: 616c 7332 0a66 726f 6d20 7468 325f 6461  als2.from th2_da
-000057d0: 7461 5f73 6572 7669 6365 732e 7574 696c  ta_services.util
-000057e0: 732e 6361 7465 676f 7279 2069 6d70 6f72  s.category impor
-000057f0: 7420 4361 7465 676f 7279 0a66 726f 6d20  t Category.from 
-00005800: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
-00005810: 732e 7574 696c 732e 6576 656e 745f 7574  s.utils.event_ut
-00005820: 696c 732e 6576 656e 745f 7574 696c 7320  ils.event_utils 
-00005830: 696d 706f 7274 2069 735f 736f 7274 6564  import is_sorted
-00005840: 0a0a 2320 5b35 2e31 5d20 4765 7420 7468  ..# [5.1] Get th
-00005850: 6520 7175 616e 7469 7469 6573 206f 6620  e quantities of 
-00005860: 6576 656e 7473 2066 6f72 2064 6966 6665  events for diffe
-00005870: 7265 6e74 2063 6174 6567 6f72 6965 732e  rent categories.
-00005880: 0a6d 6574 7269 6373 203d 205b 0a20 2020  .metrics = [.   
-00005890: 2043 6174 6567 6f72 7928 2264 6174 6522   Category("date"
-000058a0: 2c20 6c61 6d62 6461 206d 3a20 5468 3254  , lambda m: Th2T
-000058b0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-000058c0: 722e 746f 5f64 6174 6574 696d 6528 6d5b  r.to_datetime(m[
-000058d0: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
-000058e0: 5d29 2e64 6174 6528 2929 2c0a 2020 2020  ]).date()),.    
-000058f0: 4361 7465 676f 7279 2822 7374 6174 7573  Category("status
-00005900: 222c 206c 616d 6264 6120 6d3a 206d 5b22  ", lambda m: m["
-00005910: 7375 6363 6573 7366 756c 225d 292c 0a5d  successful"]),.]
-00005920: 0a63 6174 6567 6f72 795f 746f 7461 6c73  .category_totals
-00005930: 203d 2067 6574 5f63 6174 6567 6f72 795f   = get_category_
-00005940: 746f 7461 6c73 3228 6576 656e 7473 2c20  totals2(events, 
-00005950: 6d65 7472 6963 7329 0a70 7269 6e74 2863  metrics).print(c
-00005960: 6174 6567 6f72 795f 746f 7461 6c73 290a  ategory_totals).
-00005970: 2222 220a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d  """.+--------+--
-00005980: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00005990: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-000059a0: 0a7c 2020 2020 2020 2020 7c20 6461 7465  .|        | date
-000059b0: 2020 2020 2020 207c 2073 7461 7475 7320         | status 
-000059c0: 2020 7c20 2020 636f 756e 7420 7c0a 2b3d    |   count |.+=
-000059d0: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-000059e0: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d2b  ====+==========+
-000059f0: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  =========+.|    
-00005a00: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
-00005a10: 207c 2054 7275 6520 2020 2020 7c20 2020   | True     |   
-00005a20: 2020 2020 3320 7c0a 2b2d 2d2d 2d2d 2d2d      3 |.+-------
-00005a30: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  -+------------+-
-00005a40: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00005a50: 2d2d 2d2b 0a7c 2020 2020 2020 2020 7c20  ---+.|        | 
-00005a60: 3230 3233 2d30 312d 3035 207c 2046 616c  2023-01-05 | Fal
-00005a70: 7365 2020 2020 7c20 2020 2020 2020 3120  se    |       1 
-00005a80: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  |.+--------+----
-00005a90: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00005aa0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  ---+---------+.|
-00005ab0: 2063 6f75 6e74 2020 7c20 2020 2020 2020   count  |       
-00005ac0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00005ad0: 7c20 2020 2020 2020 3220 7c0a 2b2d 2d2d  |       2 |.+---
-00005ae0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00005af0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  --+----------+--
-00005b00: 2d2d 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c  -------+.| total
-00005b10: 7320 7c20 2020 2020 2020 2020 2020 207c  s |            |
-00005b20: 2031 2f31 2020 2020 2020 7c20 2020 2020   1/1      |     
-00005b30: 2020 3420 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b    4 |.+--------+
-00005b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00005b50: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00005b60: 2d2b 0a22 2222 0a0a 2320 5b35 2e32 5d20  -+."""..# [5.2] 
-00005b70: 4765 7420 7468 6520 6e75 6d62 6572 206f  Get the number o
-00005b80: 6620 6576 656e 7473 2077 6974 6820 7374  f events with st
-00005b90: 6174 7573 2073 7563 6365 7373 6675 6c2e  atus successful.
-00005ba0: 0a63 6174 6567 6f72 7920 3d20 4361 7465  .category = Cate
-00005bb0: 676f 7279 2822 7374 6174 7573 222c 206c  gory("status", l
-00005bc0: 616d 6264 6120 6d3a 206d 5b22 7375 6363  ambda m: m["succ
-00005bd0: 6573 7366 756c 225d 290a 6361 7465 676f  essful"]).catego
-00005be0: 7279 5f66 7265 7175 656e 6369 6573 203d  ry_frequencies =
-00005bf0: 2067 6574 5f63 6174 6567 6f72 795f 6672   get_category_fr
-00005c00: 6571 7565 6e63 6965 7332 2865 7665 6e74  equencies2(event
-00005c10: 732c 2063 6174 6567 6f72 7929 0a70 7269  s, category).pri
-00005c20: 6e74 2863 6174 6567 6f72 795f 6672 6571  nt(category_freq
-00005c30: 7565 6e63 6965 7329 0a22 2222 0a2b 2d2d  uencies).""".+--
-00005c40: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00005c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00005c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005c70: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
-00005c80: 2d2d 2d2d 2d2b 0a7c 2020 2020 2020 2020  -----+.|        
-00005c90: 7c20 7469 6d65 7374 616d 705f 7374 6172  | timestamp_star
-00005ca0: 7420 2020 2020 7c20 7469 6d65 7374 616d  t     | timestam
-00005cb0: 705f 656e 6420 2020 2020 2020 7c20 4661  p_end       | Fa
-00005cc0: 6c73 6520 2020 7c20 2020 5472 7565 207c  lse   |   True |
-00005cd0: 0a2b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  .+========+=====
-00005ce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005cf0: 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  +===============
-00005d00: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
-00005d10: 2b3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  +========+.|    
-00005d20: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
-00005d30: 5431 333a 3537 3a30 3520 7c20 3230 3233  T13:57:05 | 2023
-00005d40: 2d30 312d 3035 5431 333a 3537 3a30 3620  -01-05T13:57:06 
-00005d50: 7c20 3020 2020 2020 2020 7c20 2020 2020  | 0       |     
-00005d60: 2033 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d   3 |.+--------+-
-00005d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005d80: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00005d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00005da0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2b 0a7c  ----+--------+.|
-00005db0: 2020 2020 2020 2020 7c20 3230 3233 2d30          | 2023-0
-00005dc0: 312d 3035 5431 343a 3032 3a30 3520 7c20  1-05T14:02:05 | 
-00005dd0: 3230 3233 2d30 312d 3035 5431 343a 3032  2023-01-05T14:02
-00005de0: 3a30 3620 7c20 3120 2020 2020 2020 7c20  :06 | 1       | 
-00005df0: 2020 2020 2030 207c 0a2b 2d2d 2d2d 2d2d       0 |.+------
-00005e00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00005e10: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00005e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00005e30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00005e40: 2d2b 0a7c 2063 6f75 6e74 2020 7c20 2020  -+.| count  |   
-00005e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e60: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00005e70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00005e80: 2020 7c20 2020 2020 2032 207c 0a2b 2d2d    |      2 |.+--
-00005e90: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00005ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00005eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005ec0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
-00005ed0: 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c 7320  -----+.| totals 
-00005ee0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00005ef0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00005f00: 2020 2020 2020 2020 2020 2020 7c20 3120              | 1 
-00005f10: 2020 2020 2020 7c20 2020 2020 2033 207c        |      3 |
-00005f20: 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  .+--------+-----
-00005f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f40: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00005f50: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00005f60: 2b2d 2d2d 2d2d 2d2d 2d2b 0a22 2222 0a0a  +--------+."""..
-00005f70: 2320 5b35 2e33 5d20 4368 6563 6b20 6966  # [5.3] Check if
-00005f80: 2065 7665 6e74 7320 6172 6520 736f 7274   events are sort
-00005f90: 6564 2e0a 7265 7375 6c74 203d 2069 735f  ed..result = is_
-00005fa0: 736f 7274 6564 2865 7665 6e74 7329 0a70  sorted(events).p
-00005fb0: 7269 6e74 2872 6573 756c 7429 0a60 6060  rint(result).```
-00005fc0: 0a3c 212d 2d20 656e 6420 6765 745f 7374  .<!-- end get_st
-00005fd0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
-00005fe0: 202d 2d3e 0a0a 2323 2032 2e33 2e20 5368   -->..## 2.3. Sh
-00005ff0: 6f72 7420 7468 656f 7279 0a0a 5468 6520  ort theory..The 
-00006000: 6c69 6272 6172 7920 7072 6f76 6964 6573  library provides
-00006010: 2074 6f6f 6c73 2066 6f72 2068 616e 646c   tools for handl
-00006020: 696e 6720 7374 7265 616d 2064 6174 612e  ing stream data.
-00006030: 2057 6861 7427 7320 6120 7374 7265 616d   What's a stream
-00006040: 3f20 4974 2773 2061 2073 6571 7565 6e63  ? It's a sequenc
-00006050: 6520 6f66 2065 6c65 6d65 6e74 7320 6672  e of elements fr
-00006060: 6f6d 2061 2073 6f75 7263 6520 7468 6174  om a source that
-00006070: 0a73 7570 706f 7274 7320 6167 6772 6567  .supports aggreg
-00006080: 6174 6520 6f70 6572 6174 696f 6e73 2e0a  ate operations..
-00006090: 0a23 2323 2054 6572 6d73 0a0a 2d20 2a2a  .### Terms..- **
-000060a0: 4461 7461 206f 626a 6563 742a 2a3a 2041  Data object**: A
-000060b0: 6e20 696e 7374 616e 6365 206f 6620 6044  n instance of `D
-000060c0: 6174 6160 2063 6c61 7373 2077 6869 6368  ata` class which
-000060d0: 2069 7320 7772 6170 7065 7220 756e 6465   is wrapper unde
-000060e0: 7220 7374 7265 616d 2e0a 2d20 2a2a 5365  r stream..- **Se
-000060f0: 7175 656e 6365 206f 6620 656c 656d 656e  quence of elemen
-00006100: 7473 2a2a 3a0a 2020 4120 5f44 6174 6120  ts**:.  A _Data 
-00006110: 6f62 6a65 6374 5f20 7072 6f76 6964 6573  object_ provides
-00006120: 2061 6e20 696e 7465 7266 6163 6520 746f   an interface to
-00006130: 2061 2073 6571 7565 6e63 6564 2073 6574   a sequenced set
-00006140: 206f 6620 7661 6c75 6573 206f 6620 6120   of values of a 
-00006150: 7370 6563 6966 6963 2065 6c65 6d65 6e74  specific element
-00006160: 2074 7970 652e 2053 7472 6561 6d20 696e   type. Stream in
-00006170: 7369 6465 2074 6865 205f 4461 7461 0a20  side the _Data. 
-00006180: 206f 626a 6563 745f 202a 2a64 6f6e 1974   object_ **don.t
-00006190: 2061 6374 7561 6c6c 7920 7374 6f72 652a   actually store*
-000061a0: 2a20 656c 656d 656e 7473 3b20 7468 6579  * elements; they
-000061b0: 2061 7265 2063 6f6d 7075 7465 6420 6f6e   are computed on
-000061c0: 2064 656d 616e 642e 0a2d 202a 2a64 6174   demand..- **dat
-000061d0: 6120 736f 7572 6365 2a2a 2028 6578 6163  a source** (exac
-000061e0: 746c 7920 696e 2073 6d61 6c6c 206c 6574  tly in small let
-000061f0: 7465 7273 293a 0a20 2041 6e79 2073 6f75  ters):.  Any sou
-00006200: 7263 6520 6f66 2064 6174 612e 2045 2e67  rce of data. E.g
-00006210: 2e20 5b4c 6967 6874 7765 6967 6874 2044  . [Lightweight D
-00006220: 6174 6120 5072 6f76 6964 6572 5d28 6874  ata Provider](ht
-00006230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006240: 2f74 6832 2d6e 6574 2f74 6832 2d6c 772d  /th2-net/th2-lw-
-00006250: 6461 7461 2d70 726f 7669 6465 7229 2c20  data-provider), 
-00006260: 636f 6c6c 6563 7469 6f6e 732c 0a20 2061  collections,.  a
-00006270: 7272 6179 732c 206f 7220 492f 4f20 7265  rrays, or I/O re
-00006280: 736f 7572 6365 732e 0a2d 202a 2a44 6174  sources..- **Dat
-00006290: 6153 6f75 7263 652a 2a3a 0a20 2041 2063  aSource**:.  A c
-000062a0: 6c61 7373 2074 6861 7420 6973 2061 6e20  lass that is an 
-000062b0: 696e 7465 726d 6564 6961 7465 206c 696e  intermediate lin
-000062c0: 6b20 6265 7477 6565 6e20 7468 6520 536f  k between the So
-000062d0: 7572 6365 4150 4920 616e 6420 436f 6d6d  urceAPI and Comm
-000062e0: 616e 6473 2e0a 2d20 2a2a 536f 7572 6365  ands..- **Source
-000062f0: 4150 492a 2a3a 0a20 2045 6163 6820 736f  API**:.  Each so
-00006300: 7572 6365 2068 6173 2069 7473 206f 776e  urce has its own
-00006310: 2041 5049 2074 6f20 7265 7472 6965 7665   API to retrieve
-00006320: 2064 6174 612e 2053 6f75 7263 6541 5049   data. SourceAPI
-00006330: 2069 7320 6120 636c 6173 7320 7468 6174   is a class that
-00006340: 2070 726f 7669 6465 2041 5049 2066 6f72   provide API for
-00006350: 2073 6f6d 6520 6461 7461 2073 6f75 7263   some data sourc
-00006360: 652e 0a2d 202a 2a43 6f6d 6d61 6e64 732a  e..- **Commands*
-00006370: 2a3a 0a20 2043 6c61 7373 6573 2074 6861  *:.  Classes tha
-00006380: 7420 7072 6f76 6964 6520 7573 6572 2d66  t provide user-f
-00006390: 7269 656e 646c 7920 696e 7465 7266 6163  riendly interfac
-000063a0: 6573 2066 6f72 2067 6574 7469 6e67 2073  es for getting s
-000063b0: 6f6d 6520 6461 7461 2066 726f 6d20 4461  ome data from Da
-000063c0: 7461 536f 7572 6365 2e20 436f 6d6d 616e  taSource. Comman
-000063d0: 6473 2075 7365 205f 536f 7572 6365 4150  ds use _SourceAP
-000063e0: 495f 2074 6f0a 2020 6163 6869 6576 6520  I_ to.  achieve 
-000063f0: 6974 2e0a 2d20 2a2a 4164 6170 7465 7273  it..- **Adapters
-00006400: 2a2a 3a0a 2020 4974 2773 2073 696d 696c  **:.  It's simil
-00006410: 6172 2074 6f20 6675 6e63 7469 6f6e 2066  ar to function f
-00006420: 6f72 2060 4461 7461 2e6d 6170 6020 6d65  or `Data.map` me
-00006430: 7468 6f64 2e20 4164 6f70 7461 626c 6520  thod. Adoptable 
-00006440: 636f 6d6d 616e 6473 2075 7365 6420 6974  commands used it
-00006450: 2074 6f20 7570 6461 7465 2074 6865 2064   to update the d
-00006460: 6174 6120 7374 7265 616d 2e0a 2d20 2a2a  ata stream..- **
-00006470: 4167 6772 6567 6174 6520 6f70 6572 6174  Aggregate operat
-00006480: 696f 6e73 2a2a 3a0a 2020 436f 6d6d 6f6e  ions**:.  Common
-00006490: 206f 7065 7261 7469 6f6e 7320 7375 6368   operations such
-000064a0: 2061 7320 6669 6c74 6572 2c20 6d61 702c   as filter, map,
-000064b0: 206c 696d 6974 2061 6e64 2073 6f20 6f6e   limit and so on
-000064c0: 2e0a 2d20 2a2a 576f 726b 666c 6f77 2a2a  ..- **Workflow**
-000064d0: 3a20 416e 206f 7264 6572 6564 2073 6574  : An ordered set
-000064e0: 206f 6620 5f41 6767 7265 6761 7465 206f   of _Aggregate o
-000064f0: 7065 7261 7469 6f6e 735f 2e0a 0a23 2323  perations_...###
-00006500: 2043 6f6e 6365 7074 0a0a 5468 6520 6c69   Concept..The li
-00006510: 6272 6172 7920 6465 7363 7269 6265 7320  brary describes 
-00006520: 7468 6520 6869 6768 2d6c 6576 656c 2069  the high-level i
-00006530: 6e74 6572 6661 6365 7320 6049 536f 7572  nterfaces `ISour
-00006540: 6365 4150 4960 2c20 6049 4461 7461 536f  ceAPI`, `IDataSo
-00006550: 7572 6365 602c 2060 4943 6f6d 6d61 6e64  urce`, `ICommand
-00006560: 602c 2060 4941 6461 7074 6572 602e 0a0a  `, `IAdapter`...
-00006570: 416e 7920 6461 7461 2073 6f75 7263 6520  Any data source 
-00006580: 6d75 7374 2062 6520 6465 7363 7269 6265  must be describe
-00006590: 6420 6279 2074 6865 2060 4944 6174 6153  d by the `IDataS
-000065a0: 6f75 7263 6560 2061 6273 7472 6163 7420  ource` abstract 
-000065b0: 636c 6173 732e 2054 6865 7365 2063 616e  class. These can
-000065c0: 2062 6520 5f46 696c 6544 6174 6153 6f75   be _FileDataSou
-000065d0: 7263 655f 2c0a 5f43 5356 4461 7461 536f  rce_,._CSVDataSo
-000065e0: 7572 6365 5f2c 205f 4442 4461 7461 536f  urce_, _DBDataSo
-000065f0: 7572 6365 5f20 616e 6420 6f74 6865 722e  urce_ and other.
-00006600: 0a0a 5573 7561 6c6c 792c 2064 6174 6120  ..Usually, data 
-00006610: 736f 7572 6365 7320 6861 7665 2073 6f6d  sources have som
-00006620: 6520 6b69 6e64 206f 6620 4150 492e 2044  e kind of API. D
-00006630: 6174 6162 6173 6573 202d 2070 726f 7669  atabases - provi
-00006640: 6465 2053 514c 206c 616e 6775 6167 652c  de SQL language,
-00006650: 2077 6865 6e20 776f 726b 696e 6720 7769   when working wi
-00006660: 7468 2061 2066 696c 652c 2079 6f75 2063  th a file, you c
-00006670: 616e 2072 6561 640a 6c69 6e65 2062 7920  an read.line by 
-00006680: 6c69 6e65 2c20 6574 632e 2054 6869 7320  line, etc. This 
-00006690: 4150 4920 6973 2064 6573 6372 6962 6564  API is described
-000066a0: 2062 7920 7468 6520 6049 536f 7572 6365   by the `ISource
-000066b0: 4150 4960 2063 6c61 7373 2e20 4265 6361  API` class. Beca
-000066c0: 7573 6520 6469 6666 6572 656e 7420 7665  use different ve
-000066d0: 7273 696f 6e73 206f 6620 7468 6520 7361  rsions of the sa
-000066e0: 6d65 2064 6174 6120 736f 7572 6365 0a6d  me data source.m
-000066f0: 6179 2068 6176 6520 6469 6666 6572 656e  ay have differen
-00006700: 7420 4150 492c 2069 7420 6973 2062 6574  t API, it is bet
-00006710: 7465 7220 746f 2063 7265 6174 6520 6120  ter to create a 
-00006720: 636c 6173 7320 666f 7220 6561 6368 2076  class for each v
-00006730: 6572 7369 6f6e 2e0a 0a47 656e 6572 616c  ersion...General
-00006740: 6c79 2c20 6461 7461 2073 6f75 7263 6520  ly, data source 
-00006750: 4150 4973 2061 7265 2068 6964 6465 6e20  APIs are hidden 
-00006760: 6265 6869 6e64 2063 6f6e 7665 6e69 656e  behind convenien
-00006770: 7420 696e 7465 7266 6163 6573 2e20 5468  t interfaces. Th
-00006780: 6520 726f 6c65 206f 6620 7468 6573 6520  e role of these 
-00006790: 696e 7465 7266 6163 6573 2069 7320 706c  interfaces is pl
-000067a0: 6179 6564 0a62 7920 6049 436f 6d6d 616e  ayed.by `IComman
-000067b0: 6460 2063 6c61 7373 6573 2e0a 0a60 4941  d` classes...`IA
-000067c0: 6461 7074 6572 6020 636c 6173 7365 7320  dapter` classes 
-000067d0: 7472 616e 7366 6f72 6d20 6461 7461 2073  transform data s
-000067e0: 7472 6561 6d20 6c69 6b65 2066 756e 6374  tream like funct
-000067f0: 696f 6e73 2066 6f72 2060 4461 7461 2e6d  ions for `Data.m
-00006800: 6170 6020 6d65 7468 6f64 2e20 4573 7365  ap` method. Esse
-00006810: 6e74 6961 6c6c 7920 6974 2773 2074 6865  ntially it's the
-00006820: 2073 616d 6520 7468 696e 6720 6275 7420   same thing but 
-00006830: 6d6f 7265 0a66 6c65 7869 626c 652e 0a0a  more.flexible...
-00006840: 466f 7220 6578 616d 706c 652c 204c 7744  For example, LwD
-00006850: 5020 4461 7461 536f 7572 6365 2868 7474  P DataSource(htt
-00006860: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00006870: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
-00006880: 6f75 7263 652d 6c77 6470 2920 7573 6573  ource-lwdp) uses
-00006890: 2074 6865 7365 2061 6273 7472 6163 7420   these abstract 
-000068a0: 636c 6173 7365 7320 746f 2062 7569 6c64  classes to build
-000068b0: 2069 7473 2069 6d70 6c65 6d65 6e74 6174   its implementat
-000068c0: 696f 6e2e 596f 7520 6361 6e20 6561 7369  ion.You can easi
-000068d0: 6c79 2063 7265 6174 6520 796f 7572 206f  ly create your o
-000068e0: 776e 2075 6e69 7175 6520 636f 6d6d 616e  wn unique comman
-000068f0: 6473 2066 6f72 205f 4c77 4450 2044 6174  ds for _LwDP Dat
-00006900: 6153 6f75 7263 655f 2c20 6173 2077 656c  aSource_, as wel
-00006910: 6c20 6173 2065 6e74 6972 650a 5f44 6174  l as entire._Dat
-00006920: 6153 6f75 7263 655f 2063 6c61 7373 6573  aSource_ classes
-00006930: 2e20 5b48 6572 6520 6973 2061 2064 6f63  . [Here is a doc
-00006940: 756d 656e 7461 7469 6f6e 5d28 646f 6375  umentation](docu
-00006950: 6d65 6e74 6174 696f 6e2f 6461 7461 736f  mentation/dataso
-00006960: 7572 6365 2e6d 6429 206f 6e20 686f 7720  urce.md) on how 
-00006970: 746f 2069 6d70 6c65 6d65 6e74 2074 6865  to implement the
-00006980: 7365 2069 6e74 6572 6661 6365 732e 0a0a  se interfaces...
-00006990: 215b 4461 7461 2073 7472 6561 6d20 7069  ![Data stream pi
-000069a0: 7065 6c69 6e65 5d28 646f 6375 6d65 6e74  peline](document
-000069b0: 6174 696f 6e2f 696d 672f 636f 6e63 6570  ation/img/concep
-000069c0: 742e 706e 6729 0a0a 2323 2320 5374 7265  t.png)..### Stre
-000069d0: 616d 206f 7065 7261 7469 6f6e 730a 0a46  am operations..F
-000069e0: 7572 7468 6572 6d6f 7265 2c20 7374 7265  urthermore, stre
-000069f0: 616d 206f 7065 7261 7469 6f6e 7320 6861  am operations ha
-00006a00: 7665 2074 776f 2066 756e 6461 6d65 6e74  ve two fundament
-00006a10: 616c 2063 6861 7261 6374 6572 6973 7469  al characteristi
-00006a20: 6373 2074 6861 7420 6d61 6b65 2074 6865  cs that make the
-00006a30: 6d20 7665 7279 2064 6966 6665 7265 6e74  m very different
-00006a40: 2066 726f 6d20 636f 6c6c 6563 7469 6f6e   from collection
-00006a50: 0a6f 7065 7261 7469 6f6e 733a 205f 5069  .operations: _Pi
-00006a60: 7065 6c69 6e69 6e67 5f20 616e 6420 5f49  pelining_ and _I
-00006a70: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
-00006a80: 6e5f 2e0a 0a23 2323 2320 5069 7065 6c69  n_...#### Pipeli
-00006a90: 6e69 6e67 0a0a 4d61 6e79 2073 7472 6561  ning..Many strea
-00006aa0: 6d20 6f70 6572 6174 696f 6e73 2072 6574  m operations ret
-00006ab0: 7572 6e20 6120 7374 7265 616d 2074 6865  urn a stream the
-00006ac0: 6d73 656c 7665 732e 2054 6869 7320 616c  mselves. This al
-00006ad0: 6c6f 7773 206f 7065 7261 7469 6f6e 7320  lows operations 
-00006ae0: 746f 2062 6520 6368 6169 6e65 6420 746f  to be chained to
-00006af0: 2066 6f72 6d20 6120 6c61 7267 6572 2070   form a larger p
-00006b00: 6970 656c 696e 652e 0a0a 215b 4461 7461  ipeline...![Data
-00006b10: 2073 7472 6561 6d20 7069 7065 6c69 6e65   stream pipeline
-00006b20: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
-00006b30: 696d 672f 6461 7461 5f73 7472 6561 6d5f  img/data_stream_
-00006b40: 7069 7065 6c69 6e65 2e70 6e67 290a 0a23  pipeline.png)..#
-00006b50: 2323 2320 496e 7465 726e 616c 2069 7465  ### Internal ite
-00006b60: 7261 7469 6f6e 0a0a 496e 2063 6f6e 7472  ration..In contr
-00006b70: 6173 7420 746f 2063 6f6c 6c65 6374 696f  ast to collectio
-00006b80: 6e73 2c20 7768 6963 6820 6172 6520 6974  ns, which are it
-00006b90: 6572 6174 6564 2065 7870 6c69 6369 746c  erated explicitl
-00006ba0: 7920 2865 7874 6572 6e61 6c20 6974 6572  y (external iter
-00006bb0: 6174 696f 6e29 2c20 7374 7265 616d 206f  ation), stream o
-00006bc0: 7065 7261 7469 6f6e 7320 646f 2074 6865  perations do the
-00006bd0: 2069 7465 7261 7469 6f6e 0a62 6568 696e   iteration.behin
-00006be0: 6420 7468 6520 7363 656e 6573 2066 6f72  d the scenes for
-00006bf0: 2079 6f75 2e20 4e6f 7465 2c20 6974 2064   you. Note, it d
-00006c00: 6f65 736e 2774 206d 6561 6e20 796f 7520  oesn't mean you 
-00006c10: 6361 6e6e 6f74 2069 7465 7261 7465 2074  cannot iterate t
-00006c20: 6865 205f 4461 7461 206f 626a 6563 745f  he _Data object_
-00006c30: 2e0a 0a0a 2323 2320 4461 7461 2069 7465  ....### Data ite
-00006c40: 7261 7469 6f6e 0a0a 5468 6520 4461 7461  ration..The Data
-00006c50: 206f 626a 6563 7420 636f 6e73 7472 7563   object construc
-00006c60: 746f 7220 6d65 7468 6f64 2074 616b 6573  tor method takes
-00006c70: 2069 6e20 6173 2061 7267 756d 656e 7420   in as argument 
-00006c80: 6569 7468 6572 2061 6e20 6974 6572 6174  either an iterat
-00006c90: 6f72 206f 7665 7220 6f62 6a65 6374 7320  or over objects 
-00006ca0: 6f72 2061 2067 656e 6572 6174 6f72 2066  or a generator f
-00006cb0: 756e 6374 696f 6e2e 0a54 6865 2044 6174  unction..The Dat
-00006cc0: 6120 6f62 6a65 6374 2069 7465 7261 746f  a object iterato
-00006cd0: 7220 6861 6e64 6c65 7320 6561 6368 2069  r handles each i
-00006ce0: 7465 6d20 696e 2074 6869 7320 6974 6572  tem in this iter
-00006cf0: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
-00006d00: 7220 6173 2074 6865 7920 6172 652c 206d  r as they are, m
-00006d10: 6561 6e69 6e67 2069 7420 646f 6573 6e27  eaning it doesn'
-00006d20: 7420 7472 7920 746f 2072 6561 6420 7468  t try to read th
-00006d30: 6520 636f 6e74 656e 7420 6f66 2069 7465  e content of ite
-00006d40: 6d20 6f72 2072 6574 7572 6e20 7468 656d  m or return them
-00006d50: 206d 6f64 6966 6965 6420 696e 2061 6e79   modified in any
-00006d60: 2077 6179 2c20 696e 7374 6561 6420 7265   way, instead re
-00006d70: 7475 726e 7320 7468 6520 6974 656d 2069  turns the item i
-00006d80: 7473 656c 662e 0a54 6865 206f 6e6c 7920  tself..The only 
-00006d90: 6578 6365 7074 696f 6e20 746f 2074 6869  exception to thi
-00006da0: 7320 6973 2077 6865 6e20 4461 7461 206f  s is when Data o
-00006db0: 626a 6563 7420 6973 2062 7569 6c74 2075  bject is built u
-00006dc0: 7369 6e67 2069 7465 7261 746f 7220 6f72  sing iterator or
-00006dd0: 2067 656e 6572 6174 6f72 206f 7665 7220   generator over 
-00006de0: 6f74 6865 7220 4461 7461 206f 626a 6563  other Data objec
-00006df0: 7473 2e20 4e6f 7465 2074 6861 7420 7468  ts. Note that th
-00006e00: 6973 2069 7465 7261 746f 7220 6f72 2067  is iterator or g
-00006e10: 656e 6572 6174 6f72 206d 7573 7420 6f6e  enerator must on
-00006e20: 6c79 2062 6520 7969 656c 6469 6e67 2044  ly be yielding D
-00006e30: 6174 6120 6f62 6a65 6374 7320 616e 6420  ata objects and 
-00006e40: 6e6f 7468 696e 6720 656c 7365 2e20 4966  nothing else. If
-00006e50: 2077 6520 6275 696c 6420 6672 6f6d 2061   we build from a
-00006e60: 206d 6978 206f 6620 4461 7461 206f 626a   mix of Data obj
-00006e70: 6563 7473 2061 6e64 2073 6f6d 6520 6f74  ects and some ot
-00006e80: 6865 7220 7479 7065 732c 2044 6174 6120  her types, Data 
-00006e90: 6f62 6a65 6374 7327 2063 6f6e 7465 6e74  objects' content
-00006ea0: 2077 6f6e 2774 2062 6520 7265 6164 2061   won't be read a
-00006eb0: 6e64 2069 6e73 7465 6164 2069 7420 7769  nd instead it wi
-00006ec0: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
-00006ed0: 7320 4461 7461 206f 626a 6563 7420 6974  s Data object it
-00006ee0: 7365 6c66 2e0a 0a53 6d61 6c6c 2065 7861  self...Small exa
-00006ef0: 6d70 6c65 2074 6f20 6465 6d6f 6e73 7472  mple to demonstr
-00006f00: 6174 653a 0a0a 6060 6070 7974 686f 6e0a  ate:..```python.
-00006f10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00006f20: 7276 6963 6573 2e64 6174 6120 696d 706f  rvices.data impo
-00006f30: 7274 2044 6174 610a 0a64 3120 3d20 4461  rt Data..d1 = Da
-00006f40: 7461 285b 312c 322c 335d 290a 6432 203d  ta([1,2,3]).d2 =
-00006f50: 2044 6174 6128 5b34 2c35 2c36 5d29 0a0a   Data([4,5,6])..
-00006f60: 6f6e 6c79 5f64 6174 615f 6f62 6a65 6374  only_data_object
-00006f70: 7320 3d20 4461 7461 285b 6431 2c64 325d  s = Data([d1,d2]
-00006f80: 2920 2320 5769 6c6c 2069 7465 7261 7465  ) # Will iterate
-00006f90: 2061 7320 312c 322c 332c 342c 352c 360a   as 1,2,3,4,5,6.
-00006fa0: 6461 7461 5f61 6e64 5f6c 6973 7420 3d20  data_and_list = 
-00006fb0: 4461 7461 285b 6431 2c5b 342c 352c 365d  Data([d1,[4,5,6]
-00006fc0: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
-00006fd0: 6520 6173 2064 312c 205b 342c 352c 365d  e as d1, [4,5,6]
-00006fe0: 0a64 6174 615f 616e 645f 6e75 6d62 6572  .data_and_number
-00006ff0: 7320 3d20 4461 7461 285b 6431 2c34 2c35  s = Data([d1,4,5
-00007000: 2c36 5d29 2023 2057 696c 6c20 6974 6572  ,6]) # Will iter
-00007010: 6174 6520 6173 2064 312c 342c 352c 360a  ate as d1,4,5,6.
-00007020: 6c69 7374 735f 6f6e 6c79 203d 2044 6174  lists_only = Dat
-00007030: 6128 5b31 2c32 2c33 5d2c 5b34 2c35 2c36  a([1,2,3],[4,5,6
-00007040: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
-00007050: 6520 6173 205b 312c 322c 335d 2c5b 342c  e as [1,2,3],[4,
-00007060: 352c 365d 0a0a 2320 4966 2077 6520 7761  5,6]..# If we wa
-00007070: 6e74 2074 6f20 6974 6572 6174 6520 6f76  nt to iterate ov
-00007080: 6572 2063 6f6e 7465 6e74 206f 6620 6c69  er content of li
-00007090: 7374 206f 6620 6c69 7374 732c 2077 6520  st of lists, we 
-000070a0: 7368 6f75 6c64 2066 6972 7374 2063 7265  should first cre
-000070b0: 6174 6520 4461 7461 206f 626a 6563 7473  ate Data objects
-000070c0: 2066 726f 6d20 7468 656d 2c0a 2320 7468   from them,.# th
-000070d0: 656e 2075 7365 2074 6865 6d20 746f 2063  en use them to c
-000070e0: 6f6e 7374 7275 6374 206e 6577 2044 6174  onstruct new Dat
-000070f0: 6120 6f62 6a65 6374 2061 7320 696e 2063  a object as in c
-00007100: 6173 6520 6f66 2064 3120 616e 6420 6432  ase of d1 and d2
-00007110: 2c20 6372 6561 7469 6e67 2027 6f6e 6c79  , creating 'only
-00007120: 5f64 6174 615f 6f62 6a65 6374 7327 2069  _data_objects' i
-00007130: 6e20 7468 6973 2065 7861 6d70 6c65 2e0a  n this example..
-00007140: 6060 600a 200a 0a23 2323 2044 6174 6120  ```. ..### Data 
-00007150: 6361 6368 696e 670a 0a54 6865 205f 4461  caching..The _Da
-00007160: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
-00007170: 6465 7320 7468 6520 6162 696c 6974 7920  des the ability 
-00007180: 746f 2075 7365 2074 6865 2063 6163 6865  to use the cache
-00007190: 2e20 5468 6520 6361 6368 6520 776f 726b  . The cache work
-000071a0: 7320 666f 7220 6561 6368 205f 4461 7461  s for each _Data
-000071b0: 206f 626a 6563 745f 2c20 7468 6174 2069   object_, that i
-000071c0: 732c 2079 6f75 2063 686f 6f73 650a 7768  s, you choose.wh
-000071d0: 6963 6820 5f44 6174 6120 6f62 6a65 6374  ich _Data object
-000071e0: 5f20 796f 7520 7761 6e74 2074 6f20 7361  _ you want to sa
-000071f0: 7665 2e20 5468 6520 5f44 6174 6120 6f62  ve. The _Data ob
-00007200: 6a65 6374 5f20 6361 6368 6520 6973 2073  ject_ cache is s
-00007210: 6176 6564 2061 6674 6572 2074 6865 2066  aved after the f
-00007220: 6972 7374 2069 7465 7261 7469 6f6e 2c20  irst iteration, 
-00007230: 6275 7420 7468 6520 6974 6572 6174 696f  but the iteratio
-00007240: 6e0a 736f 7572 6365 206d 6179 2062 6520  n.source may be 
-00007250: 6469 6666 6572 656e 742e 0a0a 4966 2079  different...If y
-00007260: 6f75 2064 6f6e 2774 2075 7365 2074 6865  ou don't use the
-00007270: 2063 6163 6865 2c20 796f 7572 2073 6f75   cache, your sou
-00007280: 7263 6520 7769 6c6c 2062 6520 7468 6520  rce will be the 
-00007290: 6461 7461 2073 6f75 7263 6520 796f 7520  data source you 
-000072a0: 6861 7665 2069 6e20 7468 6520 5f44 6174  have in the _Dat
-000072b0: 6120 4f62 6a65 6374 5f2e 2042 7574 2069  a Object_. But i
-000072c0: 6620 796f 7520 7573 6520 7468 6520 6361  f you use the ca
-000072d0: 6368 652c 0a79 6f75 7220 736f 7572 6365  che,.your source
-000072e0: 2063 616e 2062 6520 7468 6520 6461 7461   can be the data
-000072f0: 2073 6f75 7263 652c 2074 6865 2070 6172   source, the par
-00007300: 656e 7420 6361 6368 652c 206f 7220 6f77  ent cache, or ow
-00007310: 6e20 6361 6368 653a 0a0a 2a20 5468 6520  n cache:..* The 
-00007320: 6461 7461 2073 6f75 7263 653a 0a20 2049  data source:.  I
-00007330: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
-00007340: 6374 5f20 646f 6573 6e27 7420 6861 7665  ct_ doesn't have
-00007350: 2061 2070 6172 656e 7420 6361 6368 6520   a parent cache 
-00007360: 616e 6420 6974 7320 6361 6368 652e 0a2a  and its cache..*
-00007370: 2054 6865 2070 6172 656e 7420 6361 6368   The parent cach
-00007380: 653a 0a20 2049 6620 7468 6520 5f44 6174  e:.  If the _Dat
-00007390: 6120 4f62 6a65 6374 5f20 6861 7320 6120  a Object_ has a 
-000073a0: 7061 7265 6e74 2063 6163 6865 2e20 4974  parent cache. It
-000073b0: 2064 6f65 736e 2774 206d 6174 7465 7220   doesn't matter 
-000073c0: 7768 6174 2070 6f73 6974 696f 6e20 7468  what position th
-000073d0: 6520 7061 7265 6e74 2063 6163 6865 2068  e parent cache h
-000073e0: 6173 2069 6e20 696e 6865 7269 7461 6e63  as in inheritanc
-000073f0: 652e 0a20 205f 4461 7461 204f 626a 6563  e..  _Data Objec
-00007400: 745f 2075 6e64 6572 7374 616e 6473 2077  t_ understands w
-00007410: 686f 7365 2063 6163 6865 2069 7420 6973  hose cache it is
-00007420: 2061 6e64 2065 7865 6375 7465 7320 7468   and executes th
-00007430: 6520 7061 7274 206f 6620 7468 6520 776f  e part of the wo
-00007440: 726b 666c 6f77 2074 6861 7420 7761 7320  rkflow that was 
-00007450: 6e6f 7420 6578 6563 7574 6564 2e0a 2a20  not executed..* 
-00007460: 5468 6520 6f77 6e20 6361 6368 653a 0a20  The own cache:. 
-00007470: 2049 6620 6974 2069 7320 6e6f 7420 7468   If it is not th
-00007480: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
-00007490: 6e20 6f66 2074 6869 7320 4461 7461 206f  n of this Data o
-000074a0: 626a 6563 742e 0a0a 4e6f 7465 2074 6861  bject...Note tha
-000074b0: 7420 7468 6520 6361 6368 6520 7374 6174  t the cache stat
-000074c0: 6520 6f66 2074 6865 2044 6174 6120 6f62  e of the Data ob
-000074d0: 6a65 6374 2069 7320 6e6f 7420 696e 6865  ject is not inhe
-000074e0: 7269 7465 642e 0a0a 2323 2323 2046 6f72  rited...#### For
-000074f0: 6365 6420 6361 6368 696e 670a 596f 7520  ced caching.You 
-00007500: 6361 6e20 7465 6c6c 2044 5320 746f 2063  can tell DS to c
-00007510: 6163 6865 2064 6174 6120 746f 2073 7065  ache data to spe
-00007520: 6369 6669 6320 6361 6368 6520 6669 6c65  cific cache file
-00007530: 2c20 7768 6963 6820 776f 6e27 7420 6265  , which won't be
-00007540: 2064 656c 6574 6564 2061 6674 6572 2073   deleted after s
-00007550: 6372 6970 7420 656e 642e 0a59 6f75 2063  cript end..You c
-00007560: 616e 2073 6565 2065 7861 6d70 6c65 2069  an see example i
-00007570: 6e20 312e 3132 2073 6563 7469 6f6e 206f  n 1.12 section o
-00007580: 6620 5b67 6574 5f73 7461 7274 6564 5f65  f [get_started_e
-00007590: 7861 6d70 6c65 5d28 6578 616d 706c 6573  xample](examples
-000075a0: 2f67 6574 5f73 7461 7274 6564 5f65 7861  /get_started_exa
-000075b0: 6d70 6c65 2e70 7929 2e0a 0a0a 2323 2320  mple.py)....### 
-000075c0: 4576 656e 7454 7265 6520 616e 6420 636f  EventTree and co
-000075d0: 6c6c 6563 7469 6f6e 730a 0a23 2323 2320  llections..#### 
-000075e0: 4576 656e 7454 7265 650a 0a60 4576 656e  EventTree..`Even
-000075f0: 7454 7265 6560 2069 7320 6120 7472 6565  tTree` is a tree
-00007600: 2d62 6173 6564 2064 6174 6120 7374 7275  -based data stru
-00007610: 6374 7572 6520 6f66 2065 7665 6e74 732e  cture of events.
-00007620: 2049 7420 616c 6c6f 7773 2079 6f75 2067   It allows you g
-00007630: 6574 2063 6869 6c64 7265 6e20 616e 6420  et children and 
-00007640: 7061 7265 6e74 7320 6f66 2065 7665 6e74  parents of event
-00007650: 2c0a 6469 7370 6c61 7920 7472 6565 2c20  ,.display tree, 
-00007660: 6765 7420 6675 6c6c 2070 6174 6820 746f  get full path to
-00007670: 2065 7665 6e74 2065 7463 2e0a 0a44 6574   event etc...Det
-00007680: 6169 6c73 3a0a 0a2a 2060 4576 656e 7454  ails:..* `EventT
-00007690: 7265 6560 2063 6f6e 7461 696e 7320 616c  ree` contains al
-000076a0: 6c20 6576 656e 7473 2069 6e20 6d65 6d6f  l events in memo
-000076b0: 7279 2e0a 2a20 5472 6565 2068 6173 2073  ry..* Tree has s
-000076c0: 6f6d 6520 696d 706f 7274 616e 7420 7465  ome important te
-000076d0: 726d 733a 0a20 2020 2031 2e20 5f41 6e63  rms:.    1. _Anc
-000076e0: 6573 746f 725f 2069 7320 616e 7920 7265  estor_ is any re
-000076f0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-00007700: 656e 7420 7570 2074 6865 2074 7265 6520  ent up the tree 
-00007710: 2867 7261 6e64 7061 7265 6e74 2c20 7061  (grandparent, pa
-00007720: 7265 6e74 2065 7463 2e29 2e0a 2020 2020  rent etc.)..    
-00007730: 322e 205f 5061 7265 6e74 5f20 6973 206f  2. _Parent_ is o
-00007740: 6e6c 7920 7468 6520 6669 7273 7420 7265  nly the first re
-00007750: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
-00007760: 656e 7420 7570 2074 6865 2074 7265 652e  ent up the tree.
-00007770: 0a20 2020 2033 2e20 5f43 6869 6c64 5f20  .    3. _Child_ 
-00007780: 6973 2074 6865 2066 6972 7374 2072 656c  is the first rel
-00007790: 6174 6976 6520 6f66 2074 6865 2065 7665  ative of the eve
-000077a0: 6e74 2064 6f77 6e20 7468 6520 7472 6565  nt down the tree
-000077b0: 2e0a 0a54 616b 6520 6120 6c6f 6f6b 2061  ...Take a look a
-000077c0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
-000077d0: 4854 4d4c 2074 7265 6520 746f 2075 6e64  HTML tree to und
-000077e0: 6572 7374 616e 6420 7468 656d 2e0a 0a20  erstand them... 
-000077f0: 2020 6060 600a 2020 2020 3c62 6f64 793e    ```.    <body>
-00007800: 203c 212d 2d20 616e 6365 7374 6f72 2028   <!-- ancestor (
-00007810: 6772 616e 6470 6172 656e 7429 2c20 6275  grandparent), bu
-00007820: 7420 6e6f 7420 7061 7265 6e74 202d 2d3e  t not parent -->
-00007830: 0a20 2020 2020 2020 203c 6469 763e 203c  .        <div> <
-00007840: 212d 2d20 7061 7265 6e74 2026 2061 6e63  !-- parent & anc
-00007850: 6573 746f 7220 2d2d 3e0a 2020 2020 2020  estor -->.      
-00007860: 2020 2020 2020 3c70 3e48 656c 6c6f 2c20        <p>Hello, 
-00007870: 776f 726c 6421 3c2f 703e 203c 212d 2d20  world!</p> <!-- 
-00007880: 6368 696c 6420 2d2d 3e0a 2020 2020 2020  child -->.      
-00007890: 2020 2020 2020 3c70 3e47 6f6f 6462 7965        <p>Goodbye
-000078a0: 213c 2f70 3e20 3c21 2d2d 2073 6962 6c69  !</p> <!-- sibli
-000078b0: 6e67 202d 2d3e 0a20 2020 2020 2020 203c  ng -->.        <
-000078c0: 2f64 6976 3e0a 2020 2020 3c2f 626f 6479  /div>.    </body
-000078d0: 3e0a 2020 2060 6060 0a0a 2323 2323 2043  >.   ```..#### C
-000078e0: 6f6c 6c65 6374 696f 6e73 0a0a 2a2a 4576  ollections..**Ev
-000078f0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00007900: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
-00007910: 696f 6e20 6f66 2045 7665 6e74 5472 6565  ion of EventTree
-00007920: 732e 2054 6865 2063 6f6c 6c65 6374 696f  s. The collectio
-00007930: 6e20 6275 696c 6473 2061 2066 6577 205f  n builds a few _
-00007940: 4576 656e 7454 7265 655f 2062 7920 7061  EventTree_ by pa
-00007950: 7373 6564 205f 4461 7461 0a6f 626a 6563  ssed _Data.objec
-00007960: 745f 2e20 416c 7468 6f75 6768 2079 6f75  t_. Although you
-00007970: 2063 616e 2063 6861 6e67 6520 7468 6520   can change the 
-00007980: 7472 6565 2064 6972 6563 746c 792c 2069  tree directly, i
-00007990: 7427 7320 6265 7474 6572 2074 6f20 646f  t's better to do
-000079a0: 2069 7420 7468 726f 7567 6820 636f 6c6c   it through coll
-000079b0: 6563 7469 6f6e 7320 6265 6361 7573 6520  ections because 
-000079c0: 7468 6579 2061 7265 2061 7761 7265 206f  they are aware o
-000079d0: 660a 6064 6574 6163 6865 645f 6576 656e  f.`detached_even
-000079e0: 7473 6020 616e 6420 6361 6e20 736f 6c76  ts` and can solv
-000079f0: 6520 736f 6d65 2065 7665 6e74 7320 6465  e some events de
-00007a00: 7065 6e64 656e 6369 6573 2e20 5468 6520  pendencies. The 
-00007a10: 636f 6c6c 6563 7469 6f6e 2068 6173 2073  collection has s
-00007a20: 696d 696c 6172 2066 6561 7475 7265 7320  imilar features 
-00007a30: 6c69 6b65 2061 2073 696e 676c 6520 5f45  like a single _E
-00007a40: 7665 6e74 5472 6565 5f0a 6275 7420 6170  ventTree_.but ap
-00007a50: 706c 7969 6e67 2074 6865 6d20 666f 7220  plying them for 
-00007a60: 616c 6c20 5f45 7665 6e74 5472 6565 735f  all _EventTrees_
-00007a70: 2e0a 0a2a 2a50 6172 656e 7445 7665 6e74  ...**ParentEvent
-00007a80: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
-00007a90: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
-00007aa0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
-00007ab0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
-00007ac0: 5f20 6275 7420 636f 6e74 6169 6e69 6e67  _ but containing
-00007ad0: 206f 6e6c 7920 7061 7265 6e74 2065 7665   only parent eve
-00007ae0: 6e74 7320 7468 6174 0a61 7265 2072 6566  nts that.are ref
-00007af0: 6572 656e 6365 6420 696e 2074 6865 2064  erenced in the d
-00007b00: 6174 6120 7374 7265 616d 2e20 5468 6520  ata stream. The 
-00007b10: 636f 6c6c 6563 7469 6f6e 2068 6173 2066  collection has f
-00007b20: 6561 7475 7265 7320 7369 6d69 6c61 7220  eatures similar 
-00007b30: 746f 205f 4576 656e 7454 7265 6543 6f6c  to _EventTreeCol
-00007b40: 6c65 6374 696f 6e5f 2e0a 0a44 6574 6169  lection_...Detai
-00007b50: 6c73 3a0a 0a2a 2054 6f20 7573 6520 4554  ls:..* To use ET
-00007b60: 2063 6f6c 6c65 6374 696f 6e73 2079 6f75   collections you
-00007b70: 206e 6565 6420 746f 2069 6e69 7469 616c   need to initial
-00007b80: 697a 6520 7468 656d 2062 7920 5f45 5443  ize them by _ETC
-00007b90: 4472 6976 6572 5f2e 2044 6174 6120 736f  Driver_. Data so
-00007ba0: 7572 6365 7320 7573 7561 6c6c 7920 7072  urces usually pr
-00007bb0: 6f76 6964 6520 7468 656d 2e0a 2020 596f  ovide them..  Yo
-00007bc0: 7520 6361 6e20 6372 6561 7465 2069 7420  u can create it 
-00007bd0: 6279 2079 6f75 7273 656c 6620 6465 7065  by yourself depe
-00007be0: 6e64 696e 6720 6f6e 2079 6f75 7220 6461  nding on your da
-00007bf0: 7461 2073 7472 7563 7475 7265 2e0a 2a20  ta structure..* 
-00007c00: 5468 6520 636f 6c6c 6563 7469 6f6e 2068  The collection h
-00007c10: 6173 2061 2066 6561 7475 7265 2074 6f20  as a feature to 
-00007c20: 7265 636f 7665 7220 6576 656e 7473 2e20  recover events. 
-00007c30: 416c 6c20 6576 656e 7473 2074 6861 7420  All events that 
-00007c40: 6172 6520 6e6f 7420 696e 2074 6865 2072  are not in the r
-00007c50: 6563 6569 7665 6420 6461 7461 2073 7472  eceived data str
-00007c60: 6561 6d2c 2062 7574 2077 6869 6368 2061  eam, but which a
-00007c70: 7265 0a20 2072 6566 6572 656e 6365 6420  re.  referenced 
-00007c80: 7769 6c6c 2062 6520 6c6f 6164 6564 2066  will be loaded f
-00007c90: 726f 6d20 7468 6520 6461 7461 2073 6f75  rom the data sou
-00007ca0: 7263 652e 0a2a 2059 6f75 2063 616e 2074  rce..* You can t
-00007cb0: 616b 6520 6064 6574 6163 6865 645f 6576  ake `detached_ev
-00007cc0: 656e 7473 6020 746f 2073 6565 2077 6869  ents` to see whi
-00007cd0: 6368 2065 7665 6e74 7320 6172 6520 6d69  ch events are mi
-00007ce0: 7373 696e 672e 0a2a 2049 6620 796f 7520  ssing..* If you 
-00007cf0: 7761 6e74 2c20 796f 7520 6361 6e20 6275  want, you can bu
-00007d00: 696c 6420 7061 7265 6e74 6c65 7373 2074  ild parentless t
-00007d10: 7265 6573 2077 6865 7265 2074 6865 206d  rees where the m
-00007d20: 6973 7369 6e67 2065 7665 6e74 7320 6172  issing events ar
-00007d30: 6520 7374 7562 6265 6420 696e 7374 6561  e stubbed instea
-00007d40: 642e 204a 7573 740a 2020 7573 6520 6067  d. Just.  use `g
-00007d50: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
-00007d60: 6565 7328 2960 2e0a 0a52 6571 7569 7265  ees()`...Require
-00007d70: 6d65 6e74 733a 0a0a 312e 2045 7665 6e74  ments:..1. Event
-00007d80: 7320 7072 6f76 6964 6564 2074 6f20 4554  s provided to ET
-00007d90: 4320 6861 7665 2074 6f20 6861 7665 2060  C have to have `
-00007da0: 6576 656e 745f 6e61 6d65 602c 2060 6576  event_name`, `ev
-00007db0: 656e 745f 6964 602c 2060 7061 7265 6e74  ent_id`, `parent
-00007dc0: 5f65 7665 6e74 5f69 6460 2066 6965 6c64  _event_id` field
-00007dd0: 732e 2054 6865 790a 6361 6e20 6861 7665  s. They.can have
-00007de0: 2061 6e6f 7468 6572 206e 616d 6573 2028   another names (
-00007df0: 6974 2072 6573 6f6c 7665 7320 696e 2074  it resolves in t
-00007e00: 6865 2064 7269 7665 7229 2e0a 0a23 2323  he driver)...###
-00007e10: 2320 4869 6e74 730a 0a2a 2052 656d 6f76  # Hints..* Remov
-00007e20: 6520 616c 6c20 756e 6e65 6365 7373 6172  e all unnecessar
-00007e30: 7920 6669 656c 6473 2066 726f 6d20 6576  y fields from ev
-00007e40: 656e 7473 2062 6566 6f72 6520 7061 7373  ents before pass
-00007e50: 696e 6720 746f 2061 205f 636f 6c6c 6563  ing to a _collec
-00007e60: 7469 6f6e 5f20 746f 2072 6564 7563 6520  tion_ to reduce 
-00007e70: 6d65 6d6f 7279 2075 7361 6765 2e0a 2a20  memory usage..* 
-00007e80: 5573 6520 6073 686f 7728 2960 206d 6574  Use `show()` met
-00007e90: 686f 6420 746f 2070 7269 6e74 2074 6865  hod to print the
-00007ea0: 2074 7265 6520 696e 2074 7265 652d 6c69   tree in tree-li
-00007eb0: 6b65 2076 6965 772e 0a2a 204e 6f74 6520  ke view..* Note 
-00007ec0: 7468 6174 2074 6865 2060 6765 745f 7860  that the `get_x`
-00007ed0: 206d 6574 686f 6473 2077 696c 6c20 7261   methods will ra
-00007ee0: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
-00007ef0: 2069 6620 796f 7520 7061 7373 2061 6e20   if you pass an 
-00007f00: 756e 6b6e 6f77 6e20 6576 656e 7420 6964  unknown event id
-00007f10: 2c20 756e 6c69 6b65 2074 6865 2060 6669  , unlike the `fi
-00007f20: 6e64 5f78 6020 6d65 7468 6f64 7320 280a  nd_x` methods (.
-00007f30: 2020 7468 6579 2072 6574 7572 6e20 4e6f    they return No
-00007f40: 6e65 292e 0a2a 2049 6620 796f 7520 7761  ne)..* If you wa
-00007f50: 6e74 2074 6f20 6b6e 6f77 2074 6861 7420  nt to know that 
-00007f60: 7370 6563 6966 6965 6420 6576 656e 7420  specified event 
-00007f70: 6578 6973 7473 2c20 7573 6520 7468 6520  exists, use the 
-00007f80: 7079 7468 6f6e 2060 696e 6020 6b65 7977  python `in` keyw
-00007f90: 6f72 6420 2865 2e67 2e20 6027 6576 656e  ord (e.g. `'even
-00007fa0: 742d 6964 2720 696e 2065 7665 6e74 735f  t-id' in events_
-00007fb0: 7472 6565 6029 2e0a 2a20 5573 6520 7468  tree`)..* Use th
-00007fc0: 6520 7079 7468 6f6e 2060 6c65 6e60 206b  e python `len` k
-00007fd0: 6579 776f 7264 2074 6f20 6765 7420 6576  eyword to get ev
-00007fe0: 656e 7473 206e 756d 6265 7220 696e 2074  ents number in t
-00007ff0: 6865 2074 7265 652e 0a0a 2323 2320 4669  he tree...### Fi
-00008000: 656c 6420 5265 736f 6c76 6572 730a 496e  eld Resolvers.In
-00008010: 7465 7266 6163 6520 6361 6e20 6265 2066  terface can be f
-00008020: 6f75 6e64 2069 6e20 6074 6832 5f64 6174  ound in `th2_dat
-00008030: 615f 7365 7276 6963 6573 2f69 6e74 6572  a_services/inter
-00008040: 6661 6365 732f 7574 696c 732f 7265 736f  faces/utils/reso
-00008050: 6c76 6572 2e70 7960 2e20 200a 416c 6c20  lver.py`.  .All 
-00008060: 6461 7461 2d73 6f75 7263 6573 2073 686f  data-sources sho
-00008070: 756c 6420 696d 706c 656d 656e 7420 7468  uld implement th
-00008080: 656d 2e0a 0a54 6865 2069 6465 6120 6f66  em...The idea of
-00008090: 2075 7369 6e67 2072 6573 6f6c 7665 7273   using resolvers
-000080a0: 3a0a 4974 2073 6f6c 7665 7320 7468 6520  :.It solves the 
-000080b0: 7072 6f62 6c65 6d20 6f66 2068 6176 696e  problem of havin
-000080c0: 6720 6120 6665 7720 4461 7461 536f 7572  g a few DataSour
-000080d0: 6365 7320 7769 7468 2073 696d 696c 6172  ces with similar
-000080e0: 2064 6174 612c 0a62 7574 2077 6974 6820   data,.but with 
-000080f0: 6469 6666 6572 656e 7420 7761 7973 2074  different ways t
-00008100: 6f20 6765 7420 6974 2e0a 0a54 6865 7365  o get it...These
-00008110: 2063 6c61 7373 6573 2070 726f 7669 6465   classes provide
-00008120: 2079 6f75 2067 6574 7465 7220 6d65 7468   you getter meth
-00008130: 6f64 732e 0a55 7369 6e67 2074 6865 7365  ods..Using these
-00008140: 2063 6c61 7373 6573 2061 6c6c 6f77 7320   classes allows 
-00008150: 796f 7520 746f 2066 7265 656c 7920 7377  you to freely sw
-00008160: 6974 6368 2062 6574 7765 656e 2064 6966  itch between dif
-00008170: 6665 7265 6e74 2064 6174 610a 666f 726d  ferent data.form
-00008180: 6174 7320 616e 6420 646f 6e27 7420 6368  ats and don't ch
-00008190: 616e 6765 2079 6f75 7220 636f 6465 2e0a  ange your code..
-000081a0: 0a52 6573 6f6c 7665 7273 2073 6f6c 7665  .Resolvers solve
-000081b0: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
-000081c0: 6461 7461 2d66 6f72 6d61 7420 6d69 6772  data-format migr
-000081d0: 6174 696f 6e2e 0a2d 2066 6965 6c64 7320  ation..- fields 
-000081e0: 706c 6163 6520 6361 6e20 6265 2063 6861  place can be cha
-000081f0: 6e67 6564 0a2d 2066 6965 6c64 7320 6e61  nged.- fields na
-00008200: 6d65 7320 6361 6e20 6265 2063 6861 6e67  mes can be chang
-00008210: 6564 0a0a 5265 736f 6c76 6572 7320 6361  ed..Resolvers ca
-00008220: 6e20 776f 726b 206f 6e6c 7920 7769 7468  n work only with
-00008230: 206f 6e65 2065 7665 6e74 2f6d 6573 7361   one event/messa
-00008240: 6765 2e0a 4974 206d 6561 6e73 2c20 6966  ge..It means, if
-00008250: 2079 6f75 7220 6d65 7373 6167 6520 6861   your message ha
-00008260: 7320 7375 622d 6d65 7373 6167 6573 2028  s sub-messages (
-00008270: 6c69 6b65 2074 6832 2d6d 6573 7361 6765  like th2-message
-00008280: 7320 696e 206c 7764 7029 2069 7420 0a77  s in lwdp) it .w
-00008290: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
-000082a0: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
-000082b0: 206e 6f74 206b 6e6f 7720 7769 7468 2077   not know with w
-000082c0: 6869 6368 2073 7562 2d6d 6573 7361 6765  hich sub-message
-000082d0: 2073 686f 756c 6420 6974 2077 6f72 6b2e   should it work.
-000082e0: 200a 0a2a 2a57 6f72 6b61 726f 756e 642a   ..**Workaround*
-000082f0: 2a20 200a 312e 2045 7870 616e 6420 616c  *  .1. Expand al
-00008300: 6c20 796f 7572 206d 6573 7361 6765 7320  l your messages 
-00008310: 2d3e 2060 6e65 775f 6420 3d20 796f 7572  -> `new_d = your
-00008320: 5f64 6174 612e 6d61 7028 4d65 7373 6167  _data.map(Messag
-00008330: 6546 6965 6c64 5265 736f 6c76 6572 2e65  eFieldResolver.e
-00008340: 7870 616e 645f 6d65 7373 6167 6529 600a  xpand_message)`.
-00008350: 322e 2055 7365 2060 4578 7061 6e64 6564  2. Use `Expanded
-00008360: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
-00008370: 6c76 6572 6020 696e 7374 6561 6420 6f66  lver` instead of
-00008380: 2075 7375 616c 2060 4d65 7373 6167 6546   usual `MessageF
-00008390: 6965 6c64 5265 736f 6c76 6572 6020 7768  ieldResolver` wh
-000083a0: 656e 200a 2020 2020 796f 7520 7461 6b65  en .    you take
-000083b0: 2066 6965 6c64 7320 666f 7220 6578 7061   fields for expa
-000083c0: 6e64 6564 206d 6573 7361 6765 732e 0a0a  nded messages...
-000083d0: 2a2a 496d 706c 656d 656e 7461 7469 6f6e  **Implementation
-000083e0: 2061 6476 6963 653a 2a2a 0a31 2e20 7261   advice:**.1. ra
-000083f0: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
-00008400: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
-00008410: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
-00008420: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
-00008430: 7420 7468 6973 2067 6574 7465 722e 0a0a  t this getter...
-00008440: 2a2a 5065 7266 6f72 6d61 6e63 6520 696d  **Performance im
-00008450: 7061 6374 3a2a 2a0a 2d20 4974 2061 2062  pact:**.- It a b
-00008460: 6974 2073 6c6f 7765 7220 7468 616e 2075  it slower than u
-00008470: 7369 6e67 206e 616b 6564 2066 6965 6c64  sing naked field
-00008480: 2061 6363 6573 7320 6064 6963 745b 276b   access `dict['k
-00008490: 6579 275d 602e 0a0a 2323 2032 2e34 2e20  ey']`...## 2.4. 
-000084a0: 4c69 6e6b 730a 0a2d 205b 5265 706f 7274  Links..- [Report
-000084b0: 2044 6174 6120 5072 6f76 6964 6572 5d28   Data Provider](
-000084c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000084d0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d72  om/th2-net/th2-r
-000084e0: 7074 2d64 6174 612d 7072 6f76 6964 6572  pt-data-provider
-000084f0: 290a 2d20 5b54 6832 2044 6174 6120 5365  ).- [Th2 Data Se
-00008500: 7276 6963 6573 2055 7469 6c73 5d28 6874  rvices Utils](ht
-00008510: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00008520: 2f74 6832 2d6e 6574 2f74 6832 2d64 6174  /th2-net/th2-dat
-00008530: 612d 7365 7276 6963 6573 2d75 7469 6c73  a-services-utils
-00008540: 290a 0a23 2033 2e20 4265 7374 2070 7261  )..# 3. Best pra
-00008550: 6374 6963 6573 0a44 6570 656e 6469 6e67  ctices.Depending
-00008560: 206f 6e20 686f 7720 796f 7520 776f 726b   on how you work
-00008570: 2077 6974 6820 6044 6174 6120 6f62 6a65   with `Data obje
-00008580: 6374 602c 2069 7420 6361 6e20 6265 2073  ct`, it can be s
-00008590: 6c6f 7720 6f66 2066 6173 742e 0a41 7320  low of fast..As 
-000085a0: 7769 7468 2061 2072 656c 6174 696f 6e61  with a relationa
-000085b0: 6c20 6461 7461 6261 7365 2c20 796f 7520  l database, you 
-000085c0: 6361 6e20 7772 6974 6520 6120 7175 6572  can write a quer
-000085d0: 7920 7468 6174 2077 696c 6c20 7265 7475  y that will retu
-000085e0: 726e 2064 6174 6120 736c 6f77 6c79 206f  rn data slowly o
-000085f0: 7220 7175 6963 6b6c 792c 0a74 6865 2073  r quickly,.the s
-00008600: 616d 6520 7768 656e 2077 6f72 6b69 6e67  ame when working
-00008610: 2077 6974 6820 6120 6044 6174 6120 6f62   with a `Data ob
-00008620: 6a65 6374 602e 0a0a 466f 6c6c 6f77 2074  ject`...Follow t
-00008630: 6865 2072 756c 6573 2074 6f20 6d61 6b65  he rules to make
-00008640: 2079 6f75 7220 776f 726b 2077 6974 6820   your work with 
-00008650: 4461 7461 206f 626a 6563 7420 6661 7374  Data object fast
-00008660: 3a0a 312e 2055 7365 2060 4461 7461 2e75  :.1. Use `Data.u
-00008670: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
-00008680: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
-00008690: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
-000086a0: 6d65 2e0a 322e 2054 7279 2074 6f20 646f  me..2. Try to do
-000086b0: 6e27 7420 6974 6572 6174 6520 6f6e 6520  n't iterate one 
-000086c0: 6044 6174 6120 6f62 6a65 6374 6020 696e  `Data object` in
-000086d0: 7369 6465 2074 6865 206f 7468 6572 206f  side the other o
-000086e0: 6e65 2e0a 2020 2049 6620 796f 7520 7368  ne..   If you sh
-000086f0: 6f75 6c64 2074 6f20 646f 2069 742c 2075  ould to do it, u
-00008700: 7365 2073 686f 7274 2060 4461 7461 206f  se short `Data o
-00008710: 626a 6563 7460 2066 6972 7374 2061 6e64  bject` first and
-00008720: 206c 6f6e 6720 6044 6174 6120 6f62 6a65   long `Data obje
-00008730: 6374 6020 696e 7369 6465 2074 6865 206c  ct` inside the l
-00008740: 6f6f 702e 0a20 2020 4974 276c 6c20 616c  oop..   It'll al
-00008750: 6c6f 7720 796f 7520 6f70 656e 2074 6865  low you open the
-00008760: 2063 6163 6865 2066 696c 6520 6f72 2063   cache file or c
-00008770: 7265 6174 6520 6120 7265 7175 6573 7420  reate a request 
-00008780: 746f 2060 4461 7461 2073 6f75 7263 6560  to `Data source`
-00008790: 206c 6573 7320 6e75 6d62 6572 206f 6620   less number of 
-000087a0: 7469 6d65 732e 0a0a 2320 342e 204f 6666  times...# 4. Off
-000087b0: 6963 6961 6c20 4461 7461 536f 7572 6365  icial DataSource
-000087c0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-000087d0: 0a0a 2d20 5b4c 6967 6874 7765 6967 6874  ..- [Lightweight
-000087e0: 2044 6174 6120 5072 6f76 6964 6572 2044   Data Provider D
-000087f0: 6174 6120 536f 7572 6365 5d28 6874 7470  ata Source](http
-00008800: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00008810: 6832 2d6e 6574 2f74 6832 2d64 732d 736f  h2-net/th2-ds-so
-00008820: 7572 6365 2d6c 7764 7029 0a0a 0a23 2035  urce-lwdp)...# 5
-00008830: 2e20 4150 490a 0a49 6620 796f 7520 6172  . API..If you ar
-00008840: 6520 6c6f 6f6b 696e 6720 666f 7220 636c  e looking for cl
-00008850: 6173 7365 7320 6465 7363 7269 7074 696f  asses descriptio
-00008860: 6e20 7365 6520 7468 6520 5b41 5049 2044  n see the [API D
-00008870: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
-00008880: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
-00008890: 696e 6465 782e 6d64 292e 0a0a 2320 362e  index.md)...# 6.
-000088a0: 2045 7861 6d70 6c65 730a 0a2d 205b 6765   Examples..- [ge
-000088b0: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
-000088c0: 652e 7079 5d28 6578 616d 706c 6573 2f67  e.py](examples/g
-000088d0: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
-000088e0: 6c65 2e70 7929 0a                        le.py).
+00005270: 6c64 6572 0a0a 6661 6b65 5f64 6174 6120  lder..fake_data 
+00005280: 3d20 5b0a 2020 2020 6874 7470 5f6d 6573  = [.    http_mes
+00005290: 7361 6765 5f73 7475 625f 6275 696c 6465  sage_stub_builde
+000052a0: 722e 6275 696c 6428 7b22 6d65 7373 6167  r.build({"messag
+000052b0: 6549 6422 3a20 2261 222c 2022 6d65 7373  eId": "a", "mess
+000052c0: 6167 6554 7970 6522 3a20 2252 6f6f 7422  ageType": "Root"
+000052d0: 7d29 2c0a 2020 2020 6874 7470 5f6d 6573  }),.    http_mes
+000052e0: 7361 6765 5f73 7475 625f 6275 696c 6465  sage_stub_builde
+000052f0: 722e 6275 696c 6428 7b22 6d65 7373 6167  r.build({"messag
+00005300: 6549 6422 3a20 2262 222c 2022 6d65 7373  eId": "b", "mess
+00005310: 6167 6554 7970 6522 3a20 224e 6577 227d  ageType": "New"}
+00005320: 292c 0a20 2020 2068 7474 705f 6d65 7373  ),.    http_mess
+00005330: 6167 655f 7374 7562 5f62 7569 6c64 6572  age_stub_builder
+00005340: 2e62 7569 6c64 287b 226d 6573 7361 6765  .build({"message
+00005350: 4964 223a 2022 6322 2c20 226d 6573 7361  Id": "c", "messa
+00005360: 6765 5479 7065 223a 2022 416d 656e 6422  geType": "Amend"
+00005370: 7d29 2c0a 2020 2020 6874 7470 5f6d 6573  }),.    http_mes
+00005380: 7361 6765 5f73 7475 625f 6275 696c 6465  sage_stub_builde
+00005390: 722e 6275 696c 6428 0a20 2020 2020 2020  r.build(.       
+000053a0: 207b 226d 6573 7361 6765 4964 223a 2022   {"messageId": "
+000053b0: 6422 2c20 226d 6573 7361 6765 5479 7065  d", "messageType
+000053c0: 223a 2022 4361 6e63 656c 227d 292c 0a5d  ": "Cancel"}),.]
+000053d0: 0a66 616b 655f 6461 7461 5f6f 626a 203d  .fake_data_obj =
+000053e0: 2044 6174 6128 6661 6b65 5f64 6174 6129   Data(fake_data)
+000053f0: 0a0a 666f 7220 6d20 696e 2066 616b 655f  ..for m in fake_
+00005400: 6461 7461 5f6f 626a 3a0a 2020 2020 6f5f  data_obj:.    o_
+00005410: 2e6d 6672 2e65 7870 616e 645f 6d65 7373  .mfr.expand_mess
+00005420: 6167 6528 6d29 2020 2320 6d66 7220 2d20  age(m)  # mfr - 
+00005430: 7374 616e 6473 2066 6f72 204d 6573 7361  stands for Messa
+00005440: 6765 4669 656c 6452 6573 6f6c 7665 720a  geFieldResolver.
+00005450: 2320 6f72 0a66 6f72 206d 2069 6e20 6661  # or.for m in fa
+00005460: 6b65 5f64 6174 615f 6f62 6a2e 6d61 7028  ke_data_obj.map(
+00005470: 6f5f 2e6d 6672 2e65 7870 616e 645f 6d65  o_.mfr.expand_me
+00005480: 7373 6167 6529 3a0a 2020 2020 7061 7373  ssage):.    pass
+00005490: 0a0a 2320 5b34 2e32 5d20 4c69 6272 6172  ..# [4.2] Librar
+000054a0: 6965 7320 7573 6167 652e 0a23 2044 6f6e  ies usage..# Don
+000054b0: 2774 2069 6d70 6f72 7420 6578 6163 7420  't import exact 
+000054c0: 7265 736f 6c76 6572 7320 696d 706c 656d  resolvers implem
+000054d0: 656e 7461 7469 6f6e 2069 6e20 796f 7572  entation in your
+000054e0: 2063 6f64 652c 2070 6c65 6173 652e 0a23   code, please..#
+000054f0: 2041 6c6c 6f77 2079 6f75 7220 636c 6965   Allow your clie
+00005500: 6e74 2074 6f20 646f 2069 7420 696e 7374  nt to do it inst
+00005510: 6561 642e 0a23 204a 7573 7420 696d 706f  ead..# Just impo
+00005520: 7274 2060 6f70 7469 6f6e 7360 2066 726f  rt `options` fro
+00005530: 6d20 6074 6832 5f64 6174 615f 7365 7276  m `th2_data_serv
+00005540: 6963 6573 2e63 6f6e 6669 6760 2061 6e64  ices.config` and
+00005550: 2075 7365 2069 742e 0a66 726f 6d20 7468   use it..from th
+00005560: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00005570: 636f 6e66 6967 2069 6d70 6f72 7420 6f70  config import op
+00005580: 7469 6f6e 7320 6173 206f 5f0a 0a66 6f72  tions as o_..for
+00005590: 206d 2069 6e20 6661 6b65 5f64 6174 615f   m in fake_data_
+000055a0: 6f62 6a3a 0a20 2020 206f 5f2e 6d66 722e  obj:.    o_.mfr.
+000055b0: 6578 7061 6e64 5f6d 6573 7361 6765 286d  expand_message(m
+000055c0: 290a 2320 6f72 0a66 6f72 206d 2069 6e20  ).# or.for m in 
+000055d0: 6661 6b65 5f64 6174 615f 6f62 6a2e 6d61  fake_data_obj.ma
+000055e0: 7028 6f5f 2e6d 6672 2e65 7870 616e 645f  p(o_.mfr.expand_
+000055f0: 6d65 7373 6167 6529 3a0a 2020 2020 7061  message):.    pa
+00005600: 7373 0a0a 2320 4d6f 7265 2074 6563 6820  ss..# More tech 
+00005610: 6465 7461 696c 733a 0a23 2020 2049 6e20  details:.#   In 
+00005620: 7468 6973 2063 6173 652c 2074 6865 7265  this case, there
+00005630: 2069 7320 6e6f 206c 696e 6520 6066 726f   is no line `fro
+00005640: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
+00005650: 6365 732e 6461 7461 5f73 6f75 7263 6520  ces.data_source 
+00005660: 696d 706f 7274 206c 7764 7020 600a 2320  import lwdp `.# 
+00005670: 2020 6265 6361 7573 6520 7765 2073 686f    because we sho
+00005680: 756c 6420 6e6f 7420 6368 6f6f 7365 2066  uld not choose f
+00005690: 6f72 2074 6865 2075 7365 7220 7768 6963  or the user whic
+000056a0: 6820 6120 6461 7461 2073 6f75 7263 6520  h a data source 
+000056b0: 746f 2075 7365 2e0a 2320 2020 5765 2064  to use..#   We d
+000056c0: 6f20 6e6f 7420 6b6e 6f77 2077 6861 7420  o not know what 
+000056d0: 6865 2077 696c 6c20 6368 6f6f 7365 2c20  he will choose, 
+000056e0: 7468 6572 6566 6f72 652c 2077 6520 6d75  therefore, we mu
+000056f0: 7374 2073 696d 706c 7920 6163 6365 7373  st simply access
+00005700: 0a23 2020 2074 6865 2069 6e74 6572 6661  .#   the interfa
+00005710: 6365 2c20 7768 6963 6820 7769 6c6c 2062  ce, which will b
+00005720: 6520 696e 6974 6961 6c69 7a65 6420 6279  e initialized by
+00005730: 2074 6865 2075 7365 722e 0a0a 2323 2323   the user...####
+00005740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005760: 2323 0a23 205b 355d 2055 7369 6e67 2075  ##.# [5] Using u
+00005770: 7469 6c69 7479 2066 756e 6374 696f 6e73  tility functions
+00005780: 2e0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00005790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000057a0: 2323 2323 2323 2323 0a66 726f 6d20 7468  ########.from th
+000057b0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+000057c0: 7574 696c 732e 6576 656e 745f 7574 696c  utils.event_util
+000057d0: 732e 6672 6571 7565 6e63 6965 7320 696d  s.frequencies im
+000057e0: 706f 7274 0a0a 6765 745f 6361 7465 676f  port..get_catego
+000057f0: 7279 5f66 7265 7175 656e 6369 6573 320a  ry_frequencies2.
+00005800: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00005810: 7276 6963 6573 2e75 7469 6c73 2e65 7665  rvices.utils.eve
+00005820: 6e74 5f75 7469 6c73 2e74 6f74 616c 7320  nt_utils.totals 
+00005830: 696d 706f 7274 2067 6574 5f63 6174 6567  import get_categ
+00005840: 6f72 795f 746f 7461 6c73 320a 6672 6f6d  ory_totals2.from
+00005850: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+00005860: 6573 2e75 7469 6c73 2e63 6174 6567 6f72  es.utils.categor
+00005870: 7920 696d 706f 7274 2043 6174 6567 6f72  y import Categor
+00005880: 790a 6672 6f6d 2074 6832 5f64 6174 615f  y.from th2_data_
+00005890: 7365 7276 6963 6573 2e75 7469 6c73 2e65  services.utils.e
+000058a0: 7665 6e74 5f75 7469 6c73 2e65 7665 6e74  vent_utils.event
+000058b0: 5f75 7469 6c73 2069 6d70 6f72 7420 6973  _utils import is
+000058c0: 5f73 6f72 7465 640a 0a23 205b 352e 315d  _sorted..# [5.1]
+000058d0: 2047 6574 2074 6865 2071 7561 6e74 6974   Get the quantit
+000058e0: 6965 7320 6f66 2065 7665 6e74 7320 666f  ies of events fo
+000058f0: 7220 6469 6666 6572 656e 7420 6361 7465  r different cate
+00005900: 676f 7269 6573 2e0a 6d65 7472 6963 7320  gories..metrics 
+00005910: 3d20 5b0a 2020 2020 4361 7465 676f 7279  = [.    Category
+00005920: 2822 6461 7465 222c 206c 616d 6264 6120  ("date", lambda 
+00005930: 6d3a 2054 6832 5469 6d65 7374 616d 7043  m: Th2TimestampC
+00005940: 6f6e 7665 7274 6572 2e74 6f5f 6461 7465  onverter.to_date
+00005950: 7469 6d65 280a 2020 2020 2020 2020 6d5b  time(.        m[
+00005960: 2273 7461 7274 5469 6d65 7374 616d 7022  "startTimestamp"
+00005970: 5d29 2e64 6174 6528 2929 2c0a 2020 2020  ]).date()),.    
+00005980: 4361 7465 676f 7279 2822 7374 6174 7573  Category("status
+00005990: 222c 206c 616d 6264 6120 6d3a 206d 5b22  ", lambda m: m["
+000059a0: 7375 6363 6573 7366 756c 225d 292c 0a5d  successful"]),.]
+000059b0: 0a63 6174 6567 6f72 795f 746f 7461 6c73  .category_totals
+000059c0: 203d 2067 6574 5f63 6174 6567 6f72 795f   = get_category_
+000059d0: 746f 7461 6c73 3228 6576 656e 7473 2c20  totals2(events, 
+000059e0: 6d65 7472 6963 7329 0a70 7269 6e74 2863  metrics).print(c
+000059f0: 6174 6567 6f72 795f 746f 7461 6c73 290a  ategory_totals).
+00005a00: 2222 220a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d  """.+--------+--
+00005a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00005a20: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+00005a30: 0a7c 2020 2020 2020 2020 7c20 6461 7465  .|        | date
+00005a40: 2020 2020 2020 207c 2073 7461 7475 7320         | status 
+00005a50: 2020 7c20 2020 636f 756e 7420 7c0a 2b3d    |   count |.+=
+00005a60: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+00005a70: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d2b  ====+==========+
+00005a80: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  =========+.|    
+00005a90: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
+00005aa0: 207c 2054 7275 6520 2020 2020 7c20 2020   | True     |   
+00005ab0: 2020 2020 3320 7c0a 2b2d 2d2d 2d2d 2d2d      3 |.+-------
+00005ac0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  -+------------+-
+00005ad0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00005ae0: 2d2d 2d2b 0a7c 2020 2020 2020 2020 7c20  ---+.|        | 
+00005af0: 3230 3233 2d30 312d 3035 207c 2046 616c  2023-01-05 | Fal
+00005b00: 7365 2020 2020 7c20 2020 2020 2020 3120  se    |       1 
+00005b10: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  |.+--------+----
+00005b20: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005b30: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  ---+---------+.|
+00005b40: 2063 6f75 6e74 2020 7c20 2020 2020 2020   count  |       
+00005b50: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00005b60: 7c20 2020 2020 2020 3220 7c0a 2b2d 2d2d  |       2 |.+---
+00005b70: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00005b80: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  --+----------+--
+00005b90: 2d2d 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c  -------+.| total
+00005ba0: 7320 7c20 2020 2020 2020 2020 2020 207c  s |            |
+00005bb0: 2031 2f31 2020 2020 2020 7c20 2020 2020   1/1      |     
+00005bc0: 2020 3420 7c0a 2b2d 2d2d 2d2d 2d2d 2d2b    4 |.+--------+
+00005bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005be0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00005bf0: 2d2b 0a22 2222 0a0a 2320 5b35 2e32 5d20  -+."""..# [5.2] 
+00005c00: 4765 7420 7468 6520 6e75 6d62 6572 206f  Get the number o
+00005c10: 6620 6576 656e 7473 2077 6974 6820 7374  f events with st
+00005c20: 6174 7573 2073 7563 6365 7373 6675 6c2e  atus successful.
+00005c30: 0a63 6174 6567 6f72 7920 3d20 4361 7465  .category = Cate
+00005c40: 676f 7279 2822 7374 6174 7573 222c 206c  gory("status", l
+00005c50: 616d 6264 6120 6d3a 206d 5b22 7375 6363  ambda m: m["succ
+00005c60: 6573 7366 756c 225d 290a 6361 7465 676f  essful"]).catego
+00005c70: 7279 5f66 7265 7175 656e 6369 6573 203d  ry_frequencies =
+00005c80: 2067 6574 5f63 6174 6567 6f72 795f 6672   get_category_fr
+00005c90: 6571 7565 6e63 6965 7332 2865 7665 6e74  equencies2(event
+00005ca0: 732c 2063 6174 6567 6f72 7929 0a70 7269  s, category).pri
+00005cb0: 6e74 2863 6174 6567 6f72 795f 6672 6571  nt(category_freq
+00005cc0: 7565 6e63 6965 7329 0a22 2222 0a2b 2d2d  uencies).""".+--
+00005cd0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
+00005d10: 2d2d 2d2d 2d2b 0a7c 2020 2020 2020 2020  -----+.|        
+00005d20: 7c20 7469 6d65 7374 616d 705f 7374 6172  | timestamp_star
+00005d30: 7420 2020 2020 7c20 7469 6d65 7374 616d  t     | timestam
+00005d40: 705f 656e 6420 2020 2020 2020 7c20 4661  p_end       | Fa
+00005d50: 6c73 6520 2020 7c20 2020 5472 7565 207c  lse   |   True |
+00005d60: 0a2b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  .+========+=====
+00005d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005d80: 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  +===============
+00005d90: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
+00005da0: 2b3d 3d3d 3d3d 3d3d 3d2b 0a7c 2020 2020  +========+.|    
+00005db0: 2020 2020 7c20 3230 3233 2d30 312d 3035      | 2023-01-05
+00005dc0: 5431 333a 3537 3a30 3520 7c20 3230 3233  T13:57:05 | 2023
+00005dd0: 2d30 312d 3035 5431 333a 3537 3a30 3620  -01-05T13:57:06 
+00005de0: 7c20 3020 2020 2020 2020 7c20 2020 2020  | 0       |     
+00005df0: 2033 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d   3 |.+--------+-
+00005e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005e10: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00005e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00005e30: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2b 0a7c  ----+--------+.|
+00005e40: 2020 2020 2020 2020 7c20 3230 3233 2d30          | 2023-0
+00005e50: 312d 3035 5431 343a 3032 3a30 3520 7c20  1-05T14:02:05 | 
+00005e60: 3230 3233 2d30 312d 3035 5431 343a 3032  2023-01-05T14:02
+00005e70: 3a30 3620 7c20 3120 2020 2020 2020 7c20  :06 | 1       | 
+00005e80: 2020 2020 2030 207c 0a2b 2d2d 2d2d 2d2d       0 |.+------
+00005e90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00005ea0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00005ec0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00005ed0: 2d2b 0a7c 2063 6f75 6e74 2020 7c20 2020  -+.| count  |   
+00005ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ef0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00005f00: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00005f10: 2020 7c20 2020 2020 2032 207c 0a2b 2d2d    |      2 |.+--
+00005f20: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005f50: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  --+---------+---
+00005f60: 2d2d 2d2d 2d2b 0a7c 2074 6f74 616c 7320  -----+.| totals 
+00005f70: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00005f80: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00005f90: 2020 2020 2020 2020 2020 2020 7c20 3120              | 1 
+00005fa0: 2020 2020 2020 7c20 2020 2020 2033 207c        |      3 |
+00005fb0: 0a2b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  .+--------+-----
+00005fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005fd0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00005fe0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00005ff0: 2b2d 2d2d 2d2d 2d2d 2d2b 0a22 2222 0a0a  +--------+."""..
+00006000: 2320 5b35 2e33 5d20 4368 6563 6b20 6966  # [5.3] Check if
+00006010: 2065 7665 6e74 7320 6172 6520 736f 7274   events are sort
+00006020: 6564 2e0a 7265 7375 6c74 203d 2069 735f  ed..result = is_
+00006030: 736f 7274 6564 2865 7665 6e74 7329 0a70  sorted(events).p
+00006040: 7269 6e74 2872 6573 756c 7429 0a60 6060  rint(result).```
+00006050: 0a3c 212d 2d20 656e 6420 6765 745f 7374  .<!-- end get_st
+00006060: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
+00006070: 202d 2d3e 0a0a 2323 2032 2e33 2e20 5368   -->..## 2.3. Sh
+00006080: 6f72 7420 7468 656f 7279 0a0a 5468 6520  ort theory..The 
+00006090: 6c69 6272 6172 7920 7072 6f76 6964 6573  library provides
+000060a0: 2074 6f6f 6c73 2066 6f72 2068 616e 646c   tools for handl
+000060b0: 696e 6720 7374 7265 616d 2064 6174 612e  ing stream data.
+000060c0: 2057 6861 7427 7320 6120 7374 7265 616d   What's a stream
+000060d0: 3f20 4974 2773 2061 2073 6571 7565 6e63  ? It's a sequenc
+000060e0: 6520 6f66 2065 6c65 6d65 6e74 7320 6672  e of elements fr
+000060f0: 6f6d 2061 2073 6f75 7263 6520 7468 6174  om a source that
+00006100: 0a73 7570 706f 7274 7320 6167 6772 6567  .supports aggreg
+00006110: 6174 6520 6f70 6572 6174 696f 6e73 2e0a  ate operations..
+00006120: 0a23 2323 2054 6572 6d73 0a0a 2d20 2a2a  .### Terms..- **
+00006130: 4461 7461 206f 626a 6563 742a 2a3a 2041  Data object**: A
+00006140: 6e20 696e 7374 616e 6365 206f 6620 6044  n instance of `D
+00006150: 6174 6160 2063 6c61 7373 2077 6869 6368  ata` class which
+00006160: 2069 7320 7772 6170 7065 7220 756e 6465   is wrapper unde
+00006170: 7220 7374 7265 616d 2e0a 2d20 2a2a 5365  r stream..- **Se
+00006180: 7175 656e 6365 206f 6620 656c 656d 656e  quence of elemen
+00006190: 7473 2a2a 3a0a 2020 4120 5f44 6174 6120  ts**:.  A _Data 
+000061a0: 6f62 6a65 6374 5f20 7072 6f76 6964 6573  object_ provides
+000061b0: 2061 6e20 696e 7465 7266 6163 6520 746f   an interface to
+000061c0: 2061 2073 6571 7565 6e63 6564 2073 6574   a sequenced set
+000061d0: 206f 6620 7661 6c75 6573 206f 6620 6120   of values of a 
+000061e0: 7370 6563 6966 6963 2065 6c65 6d65 6e74  specific element
+000061f0: 2074 7970 652e 2053 7472 6561 6d20 696e   type. Stream in
+00006200: 7369 6465 2074 6865 205f 4461 7461 0a20  side the _Data. 
+00006210: 206f 626a 6563 745f 202a 2a64 6f6e 1974   object_ **don.t
+00006220: 2061 6374 7561 6c6c 7920 7374 6f72 652a   actually store*
+00006230: 2a20 656c 656d 656e 7473 3b20 7468 6579  * elements; they
+00006240: 2061 7265 2063 6f6d 7075 7465 6420 6f6e   are computed on
+00006250: 2064 656d 616e 642e 0a2d 202a 2a64 6174   demand..- **dat
+00006260: 6120 736f 7572 6365 2a2a 2028 6578 6163  a source** (exac
+00006270: 746c 7920 696e 2073 6d61 6c6c 206c 6574  tly in small let
+00006280: 7465 7273 293a 0a20 2041 6e79 2073 6f75  ters):.  Any sou
+00006290: 7263 6520 6f66 2064 6174 612e 2045 2e67  rce of data. E.g
+000062a0: 2e20 5b4c 6967 6874 7765 6967 6874 2044  . [Lightweight D
+000062b0: 6174 6120 5072 6f76 6964 6572 5d28 6874  ata Provider](ht
+000062c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000062d0: 2f74 6832 2d6e 6574 2f74 6832 2d6c 772d  /th2-net/th2-lw-
+000062e0: 6461 7461 2d70 726f 7669 6465 7229 2c20  data-provider), 
+000062f0: 636f 6c6c 6563 7469 6f6e 732c 0a20 2061  collections,.  a
+00006300: 7272 6179 732c 206f 7220 492f 4f20 7265  rrays, or I/O re
+00006310: 736f 7572 6365 732e 0a2d 202a 2a44 6174  sources..- **Dat
+00006320: 6153 6f75 7263 652a 2a3a 0a20 2041 2063  aSource**:.  A c
+00006330: 6c61 7373 2074 6861 7420 6973 2061 6e20  lass that is an 
+00006340: 696e 7465 726d 6564 6961 7465 206c 696e  intermediate lin
+00006350: 6b20 6265 7477 6565 6e20 7468 6520 536f  k between the So
+00006360: 7572 6365 4150 4920 616e 6420 436f 6d6d  urceAPI and Comm
+00006370: 616e 6473 2e0a 2d20 2a2a 536f 7572 6365  ands..- **Source
+00006380: 4150 492a 2a3a 0a20 2045 6163 6820 736f  API**:.  Each so
+00006390: 7572 6365 2068 6173 2069 7473 206f 776e  urce has its own
+000063a0: 2041 5049 2074 6f20 7265 7472 6965 7665   API to retrieve
+000063b0: 2064 6174 612e 2053 6f75 7263 6541 5049   data. SourceAPI
+000063c0: 2069 7320 6120 636c 6173 7320 7468 6174   is a class that
+000063d0: 2070 726f 7669 6465 2041 5049 2066 6f72   provide API for
+000063e0: 2073 6f6d 6520 6461 7461 2073 6f75 7263   some data sourc
+000063f0: 652e 0a2d 202a 2a43 6f6d 6d61 6e64 732a  e..- **Commands*
+00006400: 2a3a 0a20 2043 6c61 7373 6573 2074 6861  *:.  Classes tha
+00006410: 7420 7072 6f76 6964 6520 7573 6572 2d66  t provide user-f
+00006420: 7269 656e 646c 7920 696e 7465 7266 6163  riendly interfac
+00006430: 6573 2066 6f72 2067 6574 7469 6e67 2073  es for getting s
+00006440: 6f6d 6520 6461 7461 2066 726f 6d20 4461  ome data from Da
+00006450: 7461 536f 7572 6365 2e20 436f 6d6d 616e  taSource. Comman
+00006460: 6473 2075 7365 205f 536f 7572 6365 4150  ds use _SourceAP
+00006470: 495f 2074 6f0a 2020 6163 6869 6576 6520  I_ to.  achieve 
+00006480: 6974 2e0a 2d20 2a2a 4164 6170 7465 7273  it..- **Adapters
+00006490: 2a2a 3a0a 2020 4974 2773 2073 696d 696c  **:.  It's simil
+000064a0: 6172 2074 6f20 6675 6e63 7469 6f6e 2066  ar to function f
+000064b0: 6f72 2060 4461 7461 2e6d 6170 6020 6d65  or `Data.map` me
+000064c0: 7468 6f64 2e20 4164 6f70 7461 626c 6520  thod. Adoptable 
+000064d0: 636f 6d6d 616e 6473 2075 7365 6420 6974  commands used it
+000064e0: 2074 6f20 7570 6461 7465 2074 6865 2064   to update the d
+000064f0: 6174 6120 7374 7265 616d 2e0a 2d20 2a2a  ata stream..- **
+00006500: 4167 6772 6567 6174 6520 6f70 6572 6174  Aggregate operat
+00006510: 696f 6e73 2a2a 3a0a 2020 436f 6d6d 6f6e  ions**:.  Common
+00006520: 206f 7065 7261 7469 6f6e 7320 7375 6368   operations such
+00006530: 2061 7320 6669 6c74 6572 2c20 6d61 702c   as filter, map,
+00006540: 206c 696d 6974 2061 6e64 2073 6f20 6f6e   limit and so on
+00006550: 2e0a 2d20 2a2a 576f 726b 666c 6f77 2a2a  ..- **Workflow**
+00006560: 3a20 416e 206f 7264 6572 6564 2073 6574  : An ordered set
+00006570: 206f 6620 5f41 6767 7265 6761 7465 206f   of _Aggregate o
+00006580: 7065 7261 7469 6f6e 735f 2e0a 0a23 2323  perations_...###
+00006590: 2043 6f6e 6365 7074 0a0a 5468 6520 6c69   Concept..The li
+000065a0: 6272 6172 7920 6465 7363 7269 6265 7320  brary describes 
+000065b0: 7468 6520 6869 6768 2d6c 6576 656c 2069  the high-level i
+000065c0: 6e74 6572 6661 6365 7320 6049 536f 7572  nterfaces `ISour
+000065d0: 6365 4150 4960 2c20 6049 4461 7461 536f  ceAPI`, `IDataSo
+000065e0: 7572 6365 602c 2060 4943 6f6d 6d61 6e64  urce`, `ICommand
+000065f0: 602c 2060 4941 6461 7074 6572 602e 0a0a  `, `IAdapter`...
+00006600: 416e 7920 6461 7461 2073 6f75 7263 6520  Any data source 
+00006610: 6d75 7374 2062 6520 6465 7363 7269 6265  must be describe
+00006620: 6420 6279 2074 6865 2060 4944 6174 6153  d by the `IDataS
+00006630: 6f75 7263 6560 2061 6273 7472 6163 7420  ource` abstract 
+00006640: 636c 6173 732e 2054 6865 7365 2063 616e  class. These can
+00006650: 2062 6520 5f46 696c 6544 6174 6153 6f75   be _FileDataSou
+00006660: 7263 655f 2c0a 5f43 5356 4461 7461 536f  rce_,._CSVDataSo
+00006670: 7572 6365 5f2c 205f 4442 4461 7461 536f  urce_, _DBDataSo
+00006680: 7572 6365 5f20 616e 6420 6f74 6865 722e  urce_ and other.
+00006690: 0a0a 5573 7561 6c6c 792c 2064 6174 6120  ..Usually, data 
+000066a0: 736f 7572 6365 7320 6861 7665 2073 6f6d  sources have som
+000066b0: 6520 6b69 6e64 206f 6620 4150 492e 2044  e kind of API. D
+000066c0: 6174 6162 6173 6573 202d 2070 726f 7669  atabases - provi
+000066d0: 6465 2053 514c 206c 616e 6775 6167 652c  de SQL language,
+000066e0: 2077 6865 6e20 776f 726b 696e 6720 7769   when working wi
+000066f0: 7468 2061 2066 696c 652c 2079 6f75 2063  th a file, you c
+00006700: 616e 2072 6561 640a 6c69 6e65 2062 7920  an read.line by 
+00006710: 6c69 6e65 2c20 6574 632e 2054 6869 7320  line, etc. This 
+00006720: 4150 4920 6973 2064 6573 6372 6962 6564  API is described
+00006730: 2062 7920 7468 6520 6049 536f 7572 6365   by the `ISource
+00006740: 4150 4960 2063 6c61 7373 2e20 4265 6361  API` class. Beca
+00006750: 7573 6520 6469 6666 6572 656e 7420 7665  use different ve
+00006760: 7273 696f 6e73 206f 6620 7468 6520 7361  rsions of the sa
+00006770: 6d65 2064 6174 6120 736f 7572 6365 0a6d  me data source.m
+00006780: 6179 2068 6176 6520 6469 6666 6572 656e  ay have differen
+00006790: 7420 4150 492c 2069 7420 6973 2062 6574  t API, it is bet
+000067a0: 7465 7220 746f 2063 7265 6174 6520 6120  ter to create a 
+000067b0: 636c 6173 7320 666f 7220 6561 6368 2076  class for each v
+000067c0: 6572 7369 6f6e 2e0a 0a47 656e 6572 616c  ersion...General
+000067d0: 6c79 2c20 6461 7461 2073 6f75 7263 6520  ly, data source 
+000067e0: 4150 4973 2061 7265 2068 6964 6465 6e20  APIs are hidden 
+000067f0: 6265 6869 6e64 2063 6f6e 7665 6e69 656e  behind convenien
+00006800: 7420 696e 7465 7266 6163 6573 2e20 5468  t interfaces. Th
+00006810: 6520 726f 6c65 206f 6620 7468 6573 6520  e role of these 
+00006820: 696e 7465 7266 6163 6573 2069 7320 706c  interfaces is pl
+00006830: 6179 6564 0a62 7920 6049 436f 6d6d 616e  ayed.by `IComman
+00006840: 6460 2063 6c61 7373 6573 2e0a 0a60 4941  d` classes...`IA
+00006850: 6461 7074 6572 6020 636c 6173 7365 7320  dapter` classes 
+00006860: 7472 616e 7366 6f72 6d20 6461 7461 2073  transform data s
+00006870: 7472 6561 6d20 6c69 6b65 2066 756e 6374  tream like funct
+00006880: 696f 6e73 2066 6f72 2060 4461 7461 2e6d  ions for `Data.m
+00006890: 6170 6020 6d65 7468 6f64 2e20 4573 7365  ap` method. Esse
+000068a0: 6e74 6961 6c6c 7920 6974 2773 2074 6865  ntially it's the
+000068b0: 2073 616d 6520 7468 696e 6720 6275 7420   same thing but 
+000068c0: 6d6f 7265 0a66 6c65 7869 626c 652e 0a0a  more.flexible...
+000068d0: 466f 7220 6578 616d 706c 652c 204c 7744  For example, LwD
+000068e0: 5020 4461 7461 536f 7572 6365 2868 7474  P DataSource(htt
+000068f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00006900: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
+00006910: 6f75 7263 652d 6c77 6470 2920 7573 6573  ource-lwdp) uses
+00006920: 2074 6865 7365 2061 6273 7472 6163 7420   these abstract 
+00006930: 636c 6173 7365 7320 746f 2062 7569 6c64  classes to build
+00006940: 2069 7473 2069 6d70 6c65 6d65 6e74 6174   its implementat
+00006950: 696f 6e2e 596f 7520 6361 6e20 6561 7369  ion.You can easi
+00006960: 6c79 2063 7265 6174 6520 796f 7572 206f  ly create your o
+00006970: 776e 2075 6e69 7175 6520 636f 6d6d 616e  wn unique comman
+00006980: 6473 2066 6f72 205f 4c77 4450 2044 6174  ds for _LwDP Dat
+00006990: 6153 6f75 7263 655f 2c20 6173 2077 656c  aSource_, as wel
+000069a0: 6c20 6173 2065 6e74 6972 650a 5f44 6174  l as entire._Dat
+000069b0: 6153 6f75 7263 655f 2063 6c61 7373 6573  aSource_ classes
+000069c0: 2e20 5b48 6572 6520 6973 2061 2064 6f63  . [Here is a doc
+000069d0: 756d 656e 7461 7469 6f6e 5d28 646f 6375  umentation](docu
+000069e0: 6d65 6e74 6174 696f 6e2f 6461 7461 736f  mentation/dataso
+000069f0: 7572 6365 2e6d 6429 206f 6e20 686f 7720  urce.md) on how 
+00006a00: 746f 2069 6d70 6c65 6d65 6e74 2074 6865  to implement the
+00006a10: 7365 2069 6e74 6572 6661 6365 732e 0a0a  se interfaces...
+00006a20: 215b 4461 7461 2073 7472 6561 6d20 7069  ![Data stream pi
+00006a30: 7065 6c69 6e65 5d28 646f 6375 6d65 6e74  peline](document
+00006a40: 6174 696f 6e2f 696d 672f 636f 6e63 6570  ation/img/concep
+00006a50: 742e 706e 6729 0a0a 2323 2320 5374 7265  t.png)..### Stre
+00006a60: 616d 206f 7065 7261 7469 6f6e 730a 0a46  am operations..F
+00006a70: 7572 7468 6572 6d6f 7265 2c20 7374 7265  urthermore, stre
+00006a80: 616d 206f 7065 7261 7469 6f6e 7320 6861  am operations ha
+00006a90: 7665 2074 776f 2066 756e 6461 6d65 6e74  ve two fundament
+00006aa0: 616c 2063 6861 7261 6374 6572 6973 7469  al characteristi
+00006ab0: 6373 2074 6861 7420 6d61 6b65 2074 6865  cs that make the
+00006ac0: 6d20 7665 7279 2064 6966 6665 7265 6e74  m very different
+00006ad0: 2066 726f 6d20 636f 6c6c 6563 7469 6f6e   from collection
+00006ae0: 0a6f 7065 7261 7469 6f6e 733a 205f 5069  .operations: _Pi
+00006af0: 7065 6c69 6e69 6e67 5f20 616e 6420 5f49  pelining_ and _I
+00006b00: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
+00006b10: 6e5f 2e0a 0a23 2323 2320 5069 7065 6c69  n_...#### Pipeli
+00006b20: 6e69 6e67 0a0a 4d61 6e79 2073 7472 6561  ning..Many strea
+00006b30: 6d20 6f70 6572 6174 696f 6e73 2072 6574  m operations ret
+00006b40: 7572 6e20 6120 7374 7265 616d 2074 6865  urn a stream the
+00006b50: 6d73 656c 7665 732e 2054 6869 7320 616c  mselves. This al
+00006b60: 6c6f 7773 206f 7065 7261 7469 6f6e 7320  lows operations 
+00006b70: 746f 2062 6520 6368 6169 6e65 6420 746f  to be chained to
+00006b80: 2066 6f72 6d20 6120 6c61 7267 6572 2070   form a larger p
+00006b90: 6970 656c 696e 652e 0a0a 215b 4461 7461  ipeline...![Data
+00006ba0: 2073 7472 6561 6d20 7069 7065 6c69 6e65   stream pipeline
+00006bb0: 5d28 646f 6375 6d65 6e74 6174 696f 6e2f  ](documentation/
+00006bc0: 696d 672f 6461 7461 5f73 7472 6561 6d5f  img/data_stream_
+00006bd0: 7069 7065 6c69 6e65 2e70 6e67 290a 0a23  pipeline.png)..#
+00006be0: 2323 2320 496e 7465 726e 616c 2069 7465  ### Internal ite
+00006bf0: 7261 7469 6f6e 0a0a 496e 2063 6f6e 7472  ration..In contr
+00006c00: 6173 7420 746f 2063 6f6c 6c65 6374 696f  ast to collectio
+00006c10: 6e73 2c20 7768 6963 6820 6172 6520 6974  ns, which are it
+00006c20: 6572 6174 6564 2065 7870 6c69 6369 746c  erated explicitl
+00006c30: 7920 2865 7874 6572 6e61 6c20 6974 6572  y (external iter
+00006c40: 6174 696f 6e29 2c20 7374 7265 616d 206f  ation), stream o
+00006c50: 7065 7261 7469 6f6e 7320 646f 2074 6865  perations do the
+00006c60: 2069 7465 7261 7469 6f6e 0a62 6568 696e   iteration.behin
+00006c70: 6420 7468 6520 7363 656e 6573 2066 6f72  d the scenes for
+00006c80: 2079 6f75 2e20 4e6f 7465 2c20 6974 2064   you. Note, it d
+00006c90: 6f65 736e 2774 206d 6561 6e20 796f 7520  oesn't mean you 
+00006ca0: 6361 6e6e 6f74 2069 7465 7261 7465 2074  cannot iterate t
+00006cb0: 6865 205f 4461 7461 206f 626a 6563 745f  he _Data object_
+00006cc0: 2e0a 0a0a 2323 2320 4461 7461 2069 7465  ....### Data ite
+00006cd0: 7261 7469 6f6e 0a0a 5468 6520 4461 7461  ration..The Data
+00006ce0: 206f 626a 6563 7420 636f 6e73 7472 7563   object construc
+00006cf0: 746f 7220 6d65 7468 6f64 2074 616b 6573  tor method takes
+00006d00: 2069 6e20 6173 2061 7267 756d 656e 7420   in as argument 
+00006d10: 6569 7468 6572 2061 6e20 6974 6572 6174  either an iterat
+00006d20: 6f72 206f 7665 7220 6f62 6a65 6374 7320  or over objects 
+00006d30: 6f72 2061 2067 656e 6572 6174 6f72 2066  or a generator f
+00006d40: 756e 6374 696f 6e2e 0a54 6865 2044 6174  unction..The Dat
+00006d50: 6120 6f62 6a65 6374 2069 7465 7261 746f  a object iterato
+00006d60: 7220 6861 6e64 6c65 7320 6561 6368 2069  r handles each i
+00006d70: 7465 6d20 696e 2074 6869 7320 6974 6572  tem in this iter
+00006d80: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
+00006d90: 7220 6173 2074 6865 7920 6172 652c 206d  r as they are, m
+00006da0: 6561 6e69 6e67 2069 7420 646f 6573 6e27  eaning it doesn'
+00006db0: 7420 7472 7920 746f 2072 6561 6420 7468  t try to read th
+00006dc0: 6520 636f 6e74 656e 7420 6f66 2069 7465  e content of ite
+00006dd0: 6d20 6f72 2072 6574 7572 6e20 7468 656d  m or return them
+00006de0: 206d 6f64 6966 6965 6420 696e 2061 6e79   modified in any
+00006df0: 2077 6179 2c20 696e 7374 6561 6420 7265   way, instead re
+00006e00: 7475 726e 7320 7468 6520 6974 656d 2069  turns the item i
+00006e10: 7473 656c 662e 0a54 6865 206f 6e6c 7920  tself..The only 
+00006e20: 6578 6365 7074 696f 6e20 746f 2074 6869  exception to thi
+00006e30: 7320 6973 2077 6865 6e20 4461 7461 206f  s is when Data o
+00006e40: 626a 6563 7420 6973 2062 7569 6c74 2075  bject is built u
+00006e50: 7369 6e67 2069 7465 7261 746f 7220 6f72  sing iterator or
+00006e60: 2067 656e 6572 6174 6f72 206f 7665 7220   generator over 
+00006e70: 6f74 6865 7220 4461 7461 206f 626a 6563  other Data objec
+00006e80: 7473 2e20 4e6f 7465 2074 6861 7420 7468  ts. Note that th
+00006e90: 6973 2069 7465 7261 746f 7220 6f72 2067  is iterator or g
+00006ea0: 656e 6572 6174 6f72 206d 7573 7420 6f6e  enerator must on
+00006eb0: 6c79 2062 6520 7969 656c 6469 6e67 2044  ly be yielding D
+00006ec0: 6174 6120 6f62 6a65 6374 7320 616e 6420  ata objects and 
+00006ed0: 6e6f 7468 696e 6720 656c 7365 2e20 4966  nothing else. If
+00006ee0: 2077 6520 6275 696c 6420 6672 6f6d 2061   we build from a
+00006ef0: 206d 6978 206f 6620 4461 7461 206f 626a   mix of Data obj
+00006f00: 6563 7473 2061 6e64 2073 6f6d 6520 6f74  ects and some ot
+00006f10: 6865 7220 7479 7065 732c 2044 6174 6120  her types, Data 
+00006f20: 6f62 6a65 6374 7327 2063 6f6e 7465 6e74  objects' content
+00006f30: 2077 6f6e 2774 2062 6520 7265 6164 2061   won't be read a
+00006f40: 6e64 2069 6e73 7465 6164 2069 7420 7769  nd instead it wi
+00006f50: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
+00006f60: 7320 4461 7461 206f 626a 6563 7420 6974  s Data object it
+00006f70: 7365 6c66 2e0a 0a53 6d61 6c6c 2065 7861  self...Small exa
+00006f80: 6d70 6c65 2074 6f20 6465 6d6f 6e73 7472  mple to demonstr
+00006f90: 6174 653a 0a0a 6060 6070 7974 686f 6e0a  ate:..```python.
+00006fa0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+00006fb0: 7276 6963 6573 2e64 6174 6120 696d 706f  rvices.data impo
+00006fc0: 7274 2044 6174 610a 0a64 3120 3d20 4461  rt Data..d1 = Da
+00006fd0: 7461 285b 312c 322c 335d 290a 6432 203d  ta([1,2,3]).d2 =
+00006fe0: 2044 6174 6128 5b34 2c35 2c36 5d29 0a0a   Data([4,5,6])..
+00006ff0: 6f6e 6c79 5f64 6174 615f 6f62 6a65 6374  only_data_object
+00007000: 7320 3d20 4461 7461 285b 6431 2c64 325d  s = Data([d1,d2]
+00007010: 2920 2320 5769 6c6c 2069 7465 7261 7465  ) # Will iterate
+00007020: 2061 7320 312c 322c 332c 342c 352c 360a   as 1,2,3,4,5,6.
+00007030: 6461 7461 5f61 6e64 5f6c 6973 7420 3d20  data_and_list = 
+00007040: 4461 7461 285b 6431 2c5b 342c 352c 365d  Data([d1,[4,5,6]
+00007050: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
+00007060: 6520 6173 2064 312c 205b 342c 352c 365d  e as d1, [4,5,6]
+00007070: 0a64 6174 615f 616e 645f 6e75 6d62 6572  .data_and_number
+00007080: 7320 3d20 4461 7461 285b 6431 2c34 2c35  s = Data([d1,4,5
+00007090: 2c36 5d29 2023 2057 696c 6c20 6974 6572  ,6]) # Will iter
+000070a0: 6174 6520 6173 2064 312c 342c 352c 360a  ate as d1,4,5,6.
+000070b0: 6c69 7374 735f 6f6e 6c79 203d 2044 6174  lists_only = Dat
+000070c0: 6128 5b31 2c32 2c33 5d2c 5b34 2c35 2c36  a([1,2,3],[4,5,6
+000070d0: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
+000070e0: 6520 6173 205b 312c 322c 335d 2c5b 342c  e as [1,2,3],[4,
+000070f0: 352c 365d 0a0a 2320 4966 2077 6520 7761  5,6]..# If we wa
+00007100: 6e74 2074 6f20 6974 6572 6174 6520 6f76  nt to iterate ov
+00007110: 6572 2063 6f6e 7465 6e74 206f 6620 6c69  er content of li
+00007120: 7374 206f 6620 6c69 7374 732c 2077 6520  st of lists, we 
+00007130: 7368 6f75 6c64 2066 6972 7374 2063 7265  should first cre
+00007140: 6174 6520 4461 7461 206f 626a 6563 7473  ate Data objects
+00007150: 2066 726f 6d20 7468 656d 2c0a 2320 7468   from them,.# th
+00007160: 656e 2075 7365 2074 6865 6d20 746f 2063  en use them to c
+00007170: 6f6e 7374 7275 6374 206e 6577 2044 6174  onstruct new Dat
+00007180: 6120 6f62 6a65 6374 2061 7320 696e 2063  a object as in c
+00007190: 6173 6520 6f66 2064 3120 616e 6420 6432  ase of d1 and d2
+000071a0: 2c20 6372 6561 7469 6e67 2027 6f6e 6c79  , creating 'only
+000071b0: 5f64 6174 615f 6f62 6a65 6374 7327 2069  _data_objects' i
+000071c0: 6e20 7468 6973 2065 7861 6d70 6c65 2e0a  n this example..
+000071d0: 6060 600a 200a 0a23 2323 2044 6174 6120  ```. ..### Data 
+000071e0: 6361 6368 696e 670a 0a54 6865 205f 4461  caching..The _Da
+000071f0: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
+00007200: 6465 7320 7468 6520 6162 696c 6974 7920  des the ability 
+00007210: 746f 2075 7365 2074 6865 2063 6163 6865  to use the cache
+00007220: 2e20 5468 6520 6361 6368 6520 776f 726b  . The cache work
+00007230: 7320 666f 7220 6561 6368 205f 4461 7461  s for each _Data
+00007240: 206f 626a 6563 745f 2c20 7468 6174 2069   object_, that i
+00007250: 732c 2079 6f75 2063 686f 6f73 650a 7768  s, you choose.wh
+00007260: 6963 6820 5f44 6174 6120 6f62 6a65 6374  ich _Data object
+00007270: 5f20 796f 7520 7761 6e74 2074 6f20 7361  _ you want to sa
+00007280: 7665 2e20 5468 6520 5f44 6174 6120 6f62  ve. The _Data ob
+00007290: 6a65 6374 5f20 6361 6368 6520 6973 2073  ject_ cache is s
+000072a0: 6176 6564 2061 6674 6572 2074 6865 2066  aved after the f
+000072b0: 6972 7374 2069 7465 7261 7469 6f6e 2c20  irst iteration, 
+000072c0: 6275 7420 7468 6520 6974 6572 6174 696f  but the iteratio
+000072d0: 6e0a 736f 7572 6365 206d 6179 2062 6520  n.source may be 
+000072e0: 6469 6666 6572 656e 742e 0a0a 4966 2079  different...If y
+000072f0: 6f75 2064 6f6e 2774 2075 7365 2074 6865  ou don't use the
+00007300: 2063 6163 6865 2c20 796f 7572 2073 6f75   cache, your sou
+00007310: 7263 6520 7769 6c6c 2062 6520 7468 6520  rce will be the 
+00007320: 6461 7461 2073 6f75 7263 6520 796f 7520  data source you 
+00007330: 6861 7665 2069 6e20 7468 6520 5f44 6174  have in the _Dat
+00007340: 6120 4f62 6a65 6374 5f2e 2042 7574 2069  a Object_. But i
+00007350: 6620 796f 7520 7573 6520 7468 6520 6361  f you use the ca
+00007360: 6368 652c 0a79 6f75 7220 736f 7572 6365  che,.your source
+00007370: 2063 616e 2062 6520 7468 6520 6461 7461   can be the data
+00007380: 2073 6f75 7263 652c 2074 6865 2070 6172   source, the par
+00007390: 656e 7420 6361 6368 652c 206f 7220 6f77  ent cache, or ow
+000073a0: 6e20 6361 6368 653a 0a0a 2a20 5468 6520  n cache:..* The 
+000073b0: 6461 7461 2073 6f75 7263 653a 0a20 2049  data source:.  I
+000073c0: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
+000073d0: 6374 5f20 646f 6573 6e27 7420 6861 7665  ct_ doesn't have
+000073e0: 2061 2070 6172 656e 7420 6361 6368 6520   a parent cache 
+000073f0: 616e 6420 6974 7320 6361 6368 652e 0a2a  and its cache..*
+00007400: 2054 6865 2070 6172 656e 7420 6361 6368   The parent cach
+00007410: 653a 0a20 2049 6620 7468 6520 5f44 6174  e:.  If the _Dat
+00007420: 6120 4f62 6a65 6374 5f20 6861 7320 6120  a Object_ has a 
+00007430: 7061 7265 6e74 2063 6163 6865 2e20 4974  parent cache. It
+00007440: 2064 6f65 736e 2774 206d 6174 7465 7220   doesn't matter 
+00007450: 7768 6174 2070 6f73 6974 696f 6e20 7468  what position th
+00007460: 6520 7061 7265 6e74 2063 6163 6865 2068  e parent cache h
+00007470: 6173 2069 6e20 696e 6865 7269 7461 6e63  as in inheritanc
+00007480: 652e 0a20 205f 4461 7461 204f 626a 6563  e..  _Data Objec
+00007490: 745f 2075 6e64 6572 7374 616e 6473 2077  t_ understands w
+000074a0: 686f 7365 2063 6163 6865 2069 7420 6973  hose cache it is
+000074b0: 2061 6e64 2065 7865 6375 7465 7320 7468   and executes th
+000074c0: 6520 7061 7274 206f 6620 7468 6520 776f  e part of the wo
+000074d0: 726b 666c 6f77 2074 6861 7420 7761 7320  rkflow that was 
+000074e0: 6e6f 7420 6578 6563 7574 6564 2e0a 2a20  not executed..* 
+000074f0: 5468 6520 6f77 6e20 6361 6368 653a 0a20  The own cache:. 
+00007500: 2049 6620 6974 2069 7320 6e6f 7420 7468   If it is not th
+00007510: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
+00007520: 6e20 6f66 2074 6869 7320 4461 7461 206f  n of this Data o
+00007530: 626a 6563 742e 0a0a 4e6f 7465 2074 6861  bject...Note tha
+00007540: 7420 7468 6520 6361 6368 6520 7374 6174  t the cache stat
+00007550: 6520 6f66 2074 6865 2044 6174 6120 6f62  e of the Data ob
+00007560: 6a65 6374 2069 7320 6e6f 7420 696e 6865  ject is not inhe
+00007570: 7269 7465 642e 0a0a 2323 2323 2046 6f72  rited...#### For
+00007580: 6365 6420 6361 6368 696e 670a 596f 7520  ced caching.You 
+00007590: 6361 6e20 7465 6c6c 2044 5320 746f 2063  can tell DS to c
+000075a0: 6163 6865 2064 6174 6120 746f 2073 7065  ache data to spe
+000075b0: 6369 6669 6320 6361 6368 6520 6669 6c65  cific cache file
+000075c0: 2c20 7768 6963 6820 776f 6e27 7420 6265  , which won't be
+000075d0: 2064 656c 6574 6564 2061 6674 6572 2073   deleted after s
+000075e0: 6372 6970 7420 656e 642e 0a59 6f75 2063  cript end..You c
+000075f0: 616e 2073 6565 2065 7861 6d70 6c65 2069  an see example i
+00007600: 6e20 312e 3132 2073 6563 7469 6f6e 206f  n 1.12 section o
+00007610: 6620 5b67 6574 5f73 7461 7274 6564 5f65  f [get_started_e
+00007620: 7861 6d70 6c65 5d28 6578 616d 706c 6573  xample](examples
+00007630: 2f67 6574 5f73 7461 7274 6564 5f65 7861  /get_started_exa
+00007640: 6d70 6c65 2e70 7929 2e0a 0a0a 2323 2320  mple.py)....### 
+00007650: 4576 656e 7454 7265 6520 616e 6420 636f  EventTree and co
+00007660: 6c6c 6563 7469 6f6e 730a 0a23 2323 2320  llections..#### 
+00007670: 4576 656e 7454 7265 650a 0a60 4576 656e  EventTree..`Even
+00007680: 7454 7265 6560 2069 7320 6120 7472 6565  tTree` is a tree
+00007690: 2d62 6173 6564 2064 6174 6120 7374 7275  -based data stru
+000076a0: 6374 7572 6520 6f66 2065 7665 6e74 732e  cture of events.
+000076b0: 2049 7420 616c 6c6f 7773 2079 6f75 2067   It allows you g
+000076c0: 6574 2063 6869 6c64 7265 6e20 616e 6420  et children and 
+000076d0: 7061 7265 6e74 7320 6f66 2065 7665 6e74  parents of event
+000076e0: 2c0a 6469 7370 6c61 7920 7472 6565 2c20  ,.display tree, 
+000076f0: 6765 7420 6675 6c6c 2070 6174 6820 746f  get full path to
+00007700: 2065 7665 6e74 2065 7463 2e0a 0a44 6574   event etc...Det
+00007710: 6169 6c73 3a0a 0a2a 2060 4576 656e 7454  ails:..* `EventT
+00007720: 7265 6560 2063 6f6e 7461 696e 7320 616c  ree` contains al
+00007730: 6c20 6576 656e 7473 2069 6e20 6d65 6d6f  l events in memo
+00007740: 7279 2e0a 2a20 5472 6565 2068 6173 2073  ry..* Tree has s
+00007750: 6f6d 6520 696d 706f 7274 616e 7420 7465  ome important te
+00007760: 726d 733a 0a20 2020 2031 2e20 5f41 6e63  rms:.    1. _Anc
+00007770: 6573 746f 725f 2069 7320 616e 7920 7265  estor_ is any re
+00007780: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+00007790: 656e 7420 7570 2074 6865 2074 7265 6520  ent up the tree 
+000077a0: 2867 7261 6e64 7061 7265 6e74 2c20 7061  (grandparent, pa
+000077b0: 7265 6e74 2065 7463 2e29 2e0a 2020 2020  rent etc.)..    
+000077c0: 322e 205f 5061 7265 6e74 5f20 6973 206f  2. _Parent_ is o
+000077d0: 6e6c 7920 7468 6520 6669 7273 7420 7265  nly the first re
+000077e0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+000077f0: 656e 7420 7570 2074 6865 2074 7265 652e  ent up the tree.
+00007800: 0a20 2020 2033 2e20 5f43 6869 6c64 5f20  .    3. _Child_ 
+00007810: 6973 2074 6865 2066 6972 7374 2072 656c  is the first rel
+00007820: 6174 6976 6520 6f66 2074 6865 2065 7665  ative of the eve
+00007830: 6e74 2064 6f77 6e20 7468 6520 7472 6565  nt down the tree
+00007840: 2e0a 0a54 616b 6520 6120 6c6f 6f6b 2061  ...Take a look a
+00007850: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
+00007860: 4854 4d4c 2074 7265 6520 746f 2075 6e64  HTML tree to und
+00007870: 6572 7374 616e 6420 7468 656d 2e0a 0a20  erstand them... 
+00007880: 2020 6060 600a 2020 2020 3c62 6f64 793e    ```.    <body>
+00007890: 203c 212d 2d20 616e 6365 7374 6f72 2028   <!-- ancestor (
+000078a0: 6772 616e 6470 6172 656e 7429 2c20 6275  grandparent), bu
+000078b0: 7420 6e6f 7420 7061 7265 6e74 202d 2d3e  t not parent -->
+000078c0: 0a20 2020 2020 2020 203c 6469 763e 203c  .        <div> <
+000078d0: 212d 2d20 7061 7265 6e74 2026 2061 6e63  !-- parent & anc
+000078e0: 6573 746f 7220 2d2d 3e0a 2020 2020 2020  estor -->.      
+000078f0: 2020 2020 2020 3c70 3e48 656c 6c6f 2c20        <p>Hello, 
+00007900: 776f 726c 6421 3c2f 703e 203c 212d 2d20  world!</p> <!-- 
+00007910: 6368 696c 6420 2d2d 3e0a 2020 2020 2020  child -->.      
+00007920: 2020 2020 2020 3c70 3e47 6f6f 6462 7965        <p>Goodbye
+00007930: 213c 2f70 3e20 3c21 2d2d 2073 6962 6c69  !</p> <!-- sibli
+00007940: 6e67 202d 2d3e 0a20 2020 2020 2020 203c  ng -->.        <
+00007950: 2f64 6976 3e0a 2020 2020 3c2f 626f 6479  /div>.    </body
+00007960: 3e0a 2020 2060 6060 0a0a 2323 2323 2043  >.   ```..#### C
+00007970: 6f6c 6c65 6374 696f 6e73 0a0a 2a2a 4576  ollections..**Ev
+00007980: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00007990: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
+000079a0: 696f 6e20 6f66 2045 7665 6e74 5472 6565  ion of EventTree
+000079b0: 732e 2054 6865 2063 6f6c 6c65 6374 696f  s. The collectio
+000079c0: 6e20 6275 696c 6473 2061 2066 6577 205f  n builds a few _
+000079d0: 4576 656e 7454 7265 655f 2062 7920 7061  EventTree_ by pa
+000079e0: 7373 6564 205f 4461 7461 0a6f 626a 6563  ssed _Data.objec
+000079f0: 745f 2e20 416c 7468 6f75 6768 2079 6f75  t_. Although you
+00007a00: 2063 616e 2063 6861 6e67 6520 7468 6520   can change the 
+00007a10: 7472 6565 2064 6972 6563 746c 792c 2069  tree directly, i
+00007a20: 7427 7320 6265 7474 6572 2074 6f20 646f  t's better to do
+00007a30: 2069 7420 7468 726f 7567 6820 636f 6c6c   it through coll
+00007a40: 6563 7469 6f6e 7320 6265 6361 7573 6520  ections because 
+00007a50: 7468 6579 2061 7265 2061 7761 7265 206f  they are aware o
+00007a60: 660a 6064 6574 6163 6865 645f 6576 656e  f.`detached_even
+00007a70: 7473 6020 616e 6420 6361 6e20 736f 6c76  ts` and can solv
+00007a80: 6520 736f 6d65 2065 7665 6e74 7320 6465  e some events de
+00007a90: 7065 6e64 656e 6369 6573 2e20 5468 6520  pendencies. The 
+00007aa0: 636f 6c6c 6563 7469 6f6e 2068 6173 2073  collection has s
+00007ab0: 696d 696c 6172 2066 6561 7475 7265 7320  imilar features 
+00007ac0: 6c69 6b65 2061 2073 696e 676c 6520 5f45  like a single _E
+00007ad0: 7665 6e74 5472 6565 5f0a 6275 7420 6170  ventTree_.but ap
+00007ae0: 706c 7969 6e67 2074 6865 6d20 666f 7220  plying them for 
+00007af0: 616c 6c20 5f45 7665 6e74 5472 6565 735f  all _EventTrees_
+00007b00: 2e0a 0a2a 2a50 6172 656e 7445 7665 6e74  ...**ParentEvent
+00007b10: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
+00007b20: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
+00007b30: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
+00007b40: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00007b50: 5f20 6275 7420 636f 6e74 6169 6e69 6e67  _ but containing
+00007b60: 206f 6e6c 7920 7061 7265 6e74 2065 7665   only parent eve
+00007b70: 6e74 7320 7468 6174 0a61 7265 2072 6566  nts that.are ref
+00007b80: 6572 656e 6365 6420 696e 2074 6865 2064  erenced in the d
+00007b90: 6174 6120 7374 7265 616d 2e20 5468 6520  ata stream. The 
+00007ba0: 636f 6c6c 6563 7469 6f6e 2068 6173 2066  collection has f
+00007bb0: 6561 7475 7265 7320 7369 6d69 6c61 7220  eatures similar 
+00007bc0: 746f 205f 4576 656e 7454 7265 6543 6f6c  to _EventTreeCol
+00007bd0: 6c65 6374 696f 6e5f 2e0a 0a44 6574 6169  lection_...Detai
+00007be0: 6c73 3a0a 0a2a 2054 6f20 7573 6520 4554  ls:..* To use ET
+00007bf0: 2063 6f6c 6c65 6374 696f 6e73 2079 6f75   collections you
+00007c00: 206e 6565 6420 746f 2069 6e69 7469 616c   need to initial
+00007c10: 697a 6520 7468 656d 2062 7920 5f45 5443  ize them by _ETC
+00007c20: 4472 6976 6572 5f2e 2044 6174 6120 736f  Driver_. Data so
+00007c30: 7572 6365 7320 7573 7561 6c6c 7920 7072  urces usually pr
+00007c40: 6f76 6964 6520 7468 656d 2e0a 2020 596f  ovide them..  Yo
+00007c50: 7520 6361 6e20 6372 6561 7465 2069 7420  u can create it 
+00007c60: 6279 2079 6f75 7273 656c 6620 6465 7065  by yourself depe
+00007c70: 6e64 696e 6720 6f6e 2079 6f75 7220 6461  nding on your da
+00007c80: 7461 2073 7472 7563 7475 7265 2e0a 2a20  ta structure..* 
+00007c90: 5468 6520 636f 6c6c 6563 7469 6f6e 2068  The collection h
+00007ca0: 6173 2061 2066 6561 7475 7265 2074 6f20  as a feature to 
+00007cb0: 7265 636f 7665 7220 6576 656e 7473 2e20  recover events. 
+00007cc0: 416c 6c20 6576 656e 7473 2074 6861 7420  All events that 
+00007cd0: 6172 6520 6e6f 7420 696e 2074 6865 2072  are not in the r
+00007ce0: 6563 6569 7665 6420 6461 7461 2073 7472  eceived data str
+00007cf0: 6561 6d2c 2062 7574 2077 6869 6368 2061  eam, but which a
+00007d00: 7265 0a20 2072 6566 6572 656e 6365 6420  re.  referenced 
+00007d10: 7769 6c6c 2062 6520 6c6f 6164 6564 2066  will be loaded f
+00007d20: 726f 6d20 7468 6520 6461 7461 2073 6f75  rom the data sou
+00007d30: 7263 652e 0a2a 2059 6f75 2063 616e 2074  rce..* You can t
+00007d40: 616b 6520 6064 6574 6163 6865 645f 6576  ake `detached_ev
+00007d50: 656e 7473 6020 746f 2073 6565 2077 6869  ents` to see whi
+00007d60: 6368 2065 7665 6e74 7320 6172 6520 6d69  ch events are mi
+00007d70: 7373 696e 672e 0a2a 2049 6620 796f 7520  ssing..* If you 
+00007d80: 7761 6e74 2c20 796f 7520 6361 6e20 6275  want, you can bu
+00007d90: 696c 6420 7061 7265 6e74 6c65 7373 2074  ild parentless t
+00007da0: 7265 6573 2077 6865 7265 2074 6865 206d  rees where the m
+00007db0: 6973 7369 6e67 2065 7665 6e74 7320 6172  issing events ar
+00007dc0: 6520 7374 7562 6265 6420 696e 7374 6561  e stubbed instea
+00007dd0: 642e 204a 7573 740a 2020 7573 6520 6067  d. Just.  use `g
+00007de0: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00007df0: 6565 7328 2960 2e0a 0a52 6571 7569 7265  ees()`...Require
+00007e00: 6d65 6e74 733a 0a0a 312e 2045 7665 6e74  ments:..1. Event
+00007e10: 7320 7072 6f76 6964 6564 2074 6f20 4554  s provided to ET
+00007e20: 4320 6861 7665 2074 6f20 6861 7665 2060  C have to have `
+00007e30: 6576 656e 745f 6e61 6d65 602c 2060 6576  event_name`, `ev
+00007e40: 656e 745f 6964 602c 2060 7061 7265 6e74  ent_id`, `parent
+00007e50: 5f65 7665 6e74 5f69 6460 2066 6965 6c64  _event_id` field
+00007e60: 732e 2054 6865 790a 6361 6e20 6861 7665  s. They.can have
+00007e70: 2061 6e6f 7468 6572 206e 616d 6573 2028   another names (
+00007e80: 6974 2072 6573 6f6c 7665 7320 696e 2074  it resolves in t
+00007e90: 6865 2064 7269 7665 7229 2e0a 0a23 2323  he driver)...###
+00007ea0: 2320 4869 6e74 730a 0a2a 2052 656d 6f76  # Hints..* Remov
+00007eb0: 6520 616c 6c20 756e 6e65 6365 7373 6172  e all unnecessar
+00007ec0: 7920 6669 656c 6473 2066 726f 6d20 6576  y fields from ev
+00007ed0: 656e 7473 2062 6566 6f72 6520 7061 7373  ents before pass
+00007ee0: 696e 6720 746f 2061 205f 636f 6c6c 6563  ing to a _collec
+00007ef0: 7469 6f6e 5f20 746f 2072 6564 7563 6520  tion_ to reduce 
+00007f00: 6d65 6d6f 7279 2075 7361 6765 2e0a 2a20  memory usage..* 
+00007f10: 5573 6520 6073 686f 7728 2960 206d 6574  Use `show()` met
+00007f20: 686f 6420 746f 2070 7269 6e74 2074 6865  hod to print the
+00007f30: 2074 7265 6520 696e 2074 7265 652d 6c69   tree in tree-li
+00007f40: 6b65 2076 6965 772e 0a2a 204e 6f74 6520  ke view..* Note 
+00007f50: 7468 6174 2074 6865 2060 6765 745f 7860  that the `get_x`
+00007f60: 206d 6574 686f 6473 2077 696c 6c20 7261   methods will ra
+00007f70: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+00007f80: 2069 6620 796f 7520 7061 7373 2061 6e20   if you pass an 
+00007f90: 756e 6b6e 6f77 6e20 6576 656e 7420 6964  unknown event id
+00007fa0: 2c20 756e 6c69 6b65 2074 6865 2060 6669  , unlike the `fi
+00007fb0: 6e64 5f78 6020 6d65 7468 6f64 7320 280a  nd_x` methods (.
+00007fc0: 2020 7468 6579 2072 6574 7572 6e20 4e6f    they return No
+00007fd0: 6e65 292e 0a2a 2049 6620 796f 7520 7761  ne)..* If you wa
+00007fe0: 6e74 2074 6f20 6b6e 6f77 2074 6861 7420  nt to know that 
+00007ff0: 7370 6563 6966 6965 6420 6576 656e 7420  specified event 
+00008000: 6578 6973 7473 2c20 7573 6520 7468 6520  exists, use the 
+00008010: 7079 7468 6f6e 2060 696e 6020 6b65 7977  python `in` keyw
+00008020: 6f72 6420 2865 2e67 2e20 6027 6576 656e  ord (e.g. `'even
+00008030: 742d 6964 2720 696e 2065 7665 6e74 735f  t-id' in events_
+00008040: 7472 6565 6029 2e0a 2a20 5573 6520 7468  tree`)..* Use th
+00008050: 6520 7079 7468 6f6e 2060 6c65 6e60 206b  e python `len` k
+00008060: 6579 776f 7264 2074 6f20 6765 7420 6576  eyword to get ev
+00008070: 656e 7473 206e 756d 6265 7220 696e 2074  ents number in t
+00008080: 6865 2074 7265 652e 0a0a 2323 2320 4669  he tree...### Fi
+00008090: 656c 6420 5265 736f 6c76 6572 730a 496e  eld Resolvers.In
+000080a0: 7465 7266 6163 6520 6361 6e20 6265 2066  terface can be f
+000080b0: 6f75 6e64 2069 6e20 6074 6832 5f64 6174  ound in `th2_dat
+000080c0: 615f 7365 7276 6963 6573 2f69 6e74 6572  a_services/inter
+000080d0: 6661 6365 732f 7574 696c 732f 7265 736f  faces/utils/reso
+000080e0: 6c76 6572 2e70 7960 2e20 200a 416c 6c20  lver.py`.  .All 
+000080f0: 6461 7461 2d73 6f75 7263 6573 2073 686f  data-sources sho
+00008100: 756c 6420 696d 706c 656d 656e 7420 7468  uld implement th
+00008110: 656d 2e0a 0a54 6865 2069 6465 6120 6f66  em...The idea of
+00008120: 2075 7369 6e67 2072 6573 6f6c 7665 7273   using resolvers
+00008130: 3a0a 4974 2073 6f6c 7665 7320 7468 6520  :.It solves the 
+00008140: 7072 6f62 6c65 6d20 6f66 2068 6176 696e  problem of havin
+00008150: 6720 6120 6665 7720 4461 7461 536f 7572  g a few DataSour
+00008160: 6365 7320 7769 7468 2073 696d 696c 6172  ces with similar
+00008170: 2064 6174 612c 0a62 7574 2077 6974 6820   data,.but with 
+00008180: 6469 6666 6572 656e 7420 7761 7973 2074  different ways t
+00008190: 6f20 6765 7420 6974 2e0a 0a54 6865 7365  o get it...These
+000081a0: 2063 6c61 7373 6573 2070 726f 7669 6465   classes provide
+000081b0: 2079 6f75 2067 6574 7465 7220 6d65 7468   you getter meth
+000081c0: 6f64 732e 0a55 7369 6e67 2074 6865 7365  ods..Using these
+000081d0: 2063 6c61 7373 6573 2061 6c6c 6f77 7320   classes allows 
+000081e0: 796f 7520 746f 2066 7265 656c 7920 7377  you to freely sw
+000081f0: 6974 6368 2062 6574 7765 656e 2064 6966  itch between dif
+00008200: 6665 7265 6e74 2064 6174 610a 666f 726d  ferent data.form
+00008210: 6174 7320 616e 6420 646f 6e27 7420 6368  ats and don't ch
+00008220: 616e 6765 2079 6f75 7220 636f 6465 2e0a  ange your code..
+00008230: 0a52 6573 6f6c 7665 7273 2073 6f6c 7665  .Resolvers solve
+00008240: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
+00008250: 6461 7461 2d66 6f72 6d61 7420 6d69 6772  data-format migr
+00008260: 6174 696f 6e2e 0a2d 2066 6965 6c64 7320  ation..- fields 
+00008270: 706c 6163 6520 6361 6e20 6265 2063 6861  place can be cha
+00008280: 6e67 6564 0a2d 2066 6965 6c64 7320 6e61  nged.- fields na
+00008290: 6d65 7320 6361 6e20 6265 2063 6861 6e67  mes can be chang
+000082a0: 6564 0a0a 5265 736f 6c76 6572 7320 6361  ed..Resolvers ca
+000082b0: 6e20 776f 726b 206f 6e6c 7920 7769 7468  n work only with
+000082c0: 206f 6e65 2065 7665 6e74 2f6d 6573 7361   one event/messa
+000082d0: 6765 2e0a 4974 206d 6561 6e73 2c20 6966  ge..It means, if
+000082e0: 2079 6f75 7220 6d65 7373 6167 6520 6861   your message ha
+000082f0: 7320 7375 622d 6d65 7373 6167 6573 2028  s sub-messages (
+00008300: 6c69 6b65 2074 6832 2d6d 6573 7361 6765  like th2-message
+00008310: 7320 696e 206c 7764 7029 2069 7420 0a77  s in lwdp) it .w
+00008320: 6f6e 2774 2077 6f72 6b2c 2062 6563 6175  on't work, becau
+00008330: 7365 2072 6573 6f6c 7665 7220 7769 6c6c  se resolver will
+00008340: 206e 6f74 206b 6e6f 7720 7769 7468 2077   not know with w
+00008350: 6869 6368 2073 7562 2d6d 6573 7361 6765  hich sub-message
+00008360: 2073 686f 756c 6420 6974 2077 6f72 6b2e   should it work.
+00008370: 200a 0a2a 2a57 6f72 6b61 726f 756e 642a   ..**Workaround*
+00008380: 2a20 200a 312e 2045 7870 616e 6420 616c  *  .1. Expand al
+00008390: 6c20 796f 7572 206d 6573 7361 6765 7320  l your messages 
+000083a0: 2d3e 2060 6e65 775f 6420 3d20 796f 7572  -> `new_d = your
+000083b0: 5f64 6174 612e 6d61 7028 4d65 7373 6167  _data.map(Messag
+000083c0: 6546 6965 6c64 5265 736f 6c76 6572 2e65  eFieldResolver.e
+000083d0: 7870 616e 645f 6d65 7373 6167 6529 600a  xpand_message)`.
+000083e0: 322e 2055 7365 2060 4578 7061 6e64 6564  2. Use `Expanded
+000083f0: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
+00008400: 6c76 6572 6020 696e 7374 6561 6420 6f66  lver` instead of
+00008410: 2075 7375 616c 2060 4d65 7373 6167 6546   usual `MessageF
+00008420: 6965 6c64 5265 736f 6c76 6572 6020 7768  ieldResolver` wh
+00008430: 656e 200a 2020 2020 796f 7520 7461 6b65  en .    you take
+00008440: 2066 6965 6c64 7320 666f 7220 6578 7061   fields for expa
+00008450: 6e64 6564 206d 6573 7361 6765 732e 0a0a  nded messages...
+00008460: 2a2a 496d 706c 656d 656e 7461 7469 6f6e  **Implementation
+00008470: 2061 6476 6963 653a 2a2a 0a31 2e20 7261   advice:**.1. ra
+00008480: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00008490: 6564 4572 726f 7220 2d2d 2069 6620 796f  edError -- if yo
+000084a0: 7572 2049 6d70 6c65 6d65 6e74 6174 696f  ur Implementatio
+000084b0: 6e20 646f 6573 6e27 7420 7375 7070 6f72  n doesn't suppor
+000084c0: 7420 7468 6973 2067 6574 7465 722e 0a0a  t this getter...
+000084d0: 2a2a 5065 7266 6f72 6d61 6e63 6520 696d  **Performance im
+000084e0: 7061 6374 3a2a 2a0a 2d20 4974 2061 2062  pact:**.- It a b
+000084f0: 6974 2073 6c6f 7765 7220 7468 616e 2075  it slower than u
+00008500: 7369 6e67 206e 616b 6564 2066 6965 6c64  sing naked field
+00008510: 2061 6363 6573 7320 6064 6963 745b 276b   access `dict['k
+00008520: 6579 275d 602e 0a0a 2323 2032 2e34 2e20  ey']`...## 2.4. 
+00008530: 4c69 6e6b 730a 0a2d 205b 5265 706f 7274  Links..- [Report
+00008540: 2044 6174 6120 5072 6f76 6964 6572 5d28   Data Provider](
+00008550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00008560: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d72  om/th2-net/th2-r
+00008570: 7074 2d64 6174 612d 7072 6f76 6964 6572  pt-data-provider
+00008580: 290a 2d20 5b54 6832 2044 6174 6120 5365  ).- [Th2 Data Se
+00008590: 7276 6963 6573 2055 7469 6c73 5d28 6874  rvices Utils](ht
+000085a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000085b0: 2f74 6832 2d6e 6574 2f74 6832 2d64 6174  /th2-net/th2-dat
+000085c0: 612d 7365 7276 6963 6573 2d75 7469 6c73  a-services-utils
+000085d0: 290a 0a23 2033 2e20 4265 7374 2070 7261  )..# 3. Best pra
+000085e0: 6374 6963 6573 0a44 6570 656e 6469 6e67  ctices.Depending
+000085f0: 206f 6e20 686f 7720 796f 7520 776f 726b   on how you work
+00008600: 2077 6974 6820 6044 6174 6120 6f62 6a65   with `Data obje
+00008610: 6374 602c 2069 7420 6361 6e20 6265 2073  ct`, it can be s
+00008620: 6c6f 7720 6f66 2066 6173 742e 0a41 7320  low of fast..As 
+00008630: 7769 7468 2061 2072 656c 6174 696f 6e61  with a relationa
+00008640: 6c20 6461 7461 6261 7365 2c20 796f 7520  l database, you 
+00008650: 6361 6e20 7772 6974 6520 6120 7175 6572  can write a quer
+00008660: 7920 7468 6174 2077 696c 6c20 7265 7475  y that will retu
+00008670: 726e 2064 6174 6120 736c 6f77 6c79 206f  rn data slowly o
+00008680: 7220 7175 6963 6b6c 792c 0a74 6865 2073  r quickly,.the s
+00008690: 616d 6520 7768 656e 2077 6f72 6b69 6e67  ame when working
+000086a0: 2077 6974 6820 6120 6044 6174 6120 6f62   with a `Data ob
+000086b0: 6a65 6374 602e 0a0a 466f 6c6c 6f77 2074  ject`...Follow t
+000086c0: 6865 2072 756c 6573 2074 6f20 6d61 6b65  he rules to make
+000086d0: 2079 6f75 7220 776f 726b 2077 6974 6820   your work with 
+000086e0: 4461 7461 206f 626a 6563 7420 6661 7374  Data object fast
+000086f0: 3a0a 312e 2055 7365 2060 4461 7461 2e75  :.1. Use `Data.u
+00008700: 7365 5f63 6163 6865 2829 6020 6966 2079  se_cache()` if y
+00008710: 6f75 2069 7465 7261 7465 2064 6174 6120  ou iterate data 
+00008720: 6d6f 7265 2074 6861 6e20 6f6e 6520 7469  more than one ti
+00008730: 6d65 2e0a 322e 2054 7279 2074 6f20 646f  me..2. Try to do
+00008740: 6e27 7420 6974 6572 6174 6520 6f6e 6520  n't iterate one 
+00008750: 6044 6174 6120 6f62 6a65 6374 6020 696e  `Data object` in
+00008760: 7369 6465 2074 6865 206f 7468 6572 206f  side the other o
+00008770: 6e65 2e0a 2020 2049 6620 796f 7520 7368  ne..   If you sh
+00008780: 6f75 6c64 2074 6f20 646f 2069 742c 2075  ould to do it, u
+00008790: 7365 2073 686f 7274 2060 4461 7461 206f  se short `Data o
+000087a0: 626a 6563 7460 2066 6972 7374 2061 6e64  bject` first and
+000087b0: 206c 6f6e 6720 6044 6174 6120 6f62 6a65   long `Data obje
+000087c0: 6374 6020 696e 7369 6465 2074 6865 206c  ct` inside the l
+000087d0: 6f6f 702e 0a20 2020 4974 276c 6c20 616c  oop..   It'll al
+000087e0: 6c6f 7720 796f 7520 6f70 656e 2074 6865  low you open the
+000087f0: 2063 6163 6865 2066 696c 6520 6f72 2063   cache file or c
+00008800: 7265 6174 6520 6120 7265 7175 6573 7420  reate a request 
+00008810: 746f 2060 4461 7461 2073 6f75 7263 6560  to `Data source`
+00008820: 206c 6573 7320 6e75 6d62 6572 206f 6620   less number of 
+00008830: 7469 6d65 732e 0a0a 2320 342e 204f 6666  times...# 4. Off
+00008840: 6963 6961 6c20 4461 7461 536f 7572 6365  icial DataSource
+00008850: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
+00008860: 0a0a 2d20 5b4c 6967 6874 7765 6967 6874  ..- [Lightweight
+00008870: 2044 6174 6120 5072 6f76 6964 6572 2044   Data Provider D
+00008880: 6174 6120 536f 7572 6365 5d28 6874 7470  ata Source](http
+00008890: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000088a0: 6832 2d6e 6574 2f74 6832 2d64 732d 736f  h2-net/th2-ds-so
+000088b0: 7572 6365 2d6c 7764 7029 0a0a 0a23 2035  urce-lwdp)...# 5
+000088c0: 2e20 4150 490a 0a49 6620 796f 7520 6172  . API..If you ar
+000088d0: 6520 6c6f 6f6b 696e 6720 666f 7220 636c  e looking for cl
+000088e0: 6173 7365 7320 6465 7363 7269 7074 696f  asses descriptio
+000088f0: 6e20 7365 6520 7468 6520 5b41 5049 2044  n see the [API D
+00008900: 6f63 756d 656e 7461 7469 6f6e 5d28 646f  ocumentation](do
+00008910: 6375 6d65 6e74 6174 696f 6e2f 6170 692f  cumentation/api/
+00008920: 696e 6465 782e 6d64 292e 0a0a 2320 362e  index.md)...# 6.
+00008930: 2045 7861 6d70 6c65 730a 0a2d 205b 6765   Examples..- [ge
+00008940: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
+00008950: 652e 7079 5d28 6578 616d 706c 6573 2f67  e.py](examples/g
+00008960: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+00008970: 6c65 2e70 7929 0a                        le.py).
```

### Comparing `th2_data_services-2.0.0.dev9018014082/setup.py` & `th2_data_services-2.0.0.dev9113174303/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/data.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,39 +68,32 @@
         If your timestamp has nanoseconds, they will be just cut (not rounded).
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
             datetime: Timestamp in python datetime format.
-
-        Speed test:
-            AMD Ryzen 7 6800H with Radeon Graphics 3.20 GHz
-            ~ 987 ns per iteration  ~= 1000000 iterations per second
         """
         seconds, nanoseconds = cls.parse_timestamp_int(timestamp)
-        nanoseconds_str = f"{nanoseconds:0>9}"
-        microseconds = nanoseconds_str[:-3]
-        ts = float(str(seconds) + "." + microseconds)
-        return datetime.utcfromtimestamp(ts)
+        return datetime.utcfromtimestamp(seconds + nanoseconds // 1000 / 1_000_000)
 
     @classmethod
     def to_seconds(cls, timestamp: TimestampType):
         """Converts timestamp to seconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
             int: Timestamp in seconds format.
         """
-        seconds, nanoseconds = cls.parse_timestamp(timestamp)
-        return int(seconds)
+        seconds, nanoseconds = cls.parse_timestamp_int(timestamp)
+        return seconds
 
     @classmethod
     def to_milliseconds(cls, timestamp: TimestampType) -> int:
         """Converts timestamp to milliseconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
```

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/converters.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,105 +9,134 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
-from collections import namedtuple
 from datetime import datetime, timezone
 import shutil
 import gzip
+import ciso8601
 
 import flatdict as _flatdict
 
 from th2_data_services.interfaces.utils.converter import ITimestampConverter, TimestampType
 
-_DatetimeTuple = namedtuple("DatetimeTuple", ["datetime", "mantissa"])
-
 
 class DatetimeStringConverter(ITimestampConverter[str]):
     """Converts datetime strings.
 
     Works with ISO_8601 datetime strings.
 
     If you request microseconds but your timestamp has nanoseconds,
     they will be just cut (not rounding).
 
-    Expected timestamp format "yyyy-MM-ddTHH:mm:ss[.SSSSSSSSS]Z".
-    If you don't provide 'Z' in the end, it can return wrong results.
+    Expected timestamp format "yyyy-MM-ddTHH:mm:ss[.SSSSSSSSS][Z]".
+    'Z' in the end is optional.
     """
 
     @classmethod
     def parse_timestamp(cls, datetime_string: str) -> (str, str):
-        # Exception handling works faster than using `if`.
+        # Note:
+        #   we have similar code here (not the separate function)
+        #   to improve performance.
         try:
-            # Handles "yyyy-MM-ddTHH:mm:ss.SSSSSSSSSZ"
-            dt_tuple = _DatetimeTuple(*datetime_string.rsplit("."))
-            timestamp = datetime.strptime(dt_tuple.datetime, "%Y-%m-%dT%H:%M:%S").replace(
-                tzinfo=timezone.utc
-            )
-        except TypeError:
-            # Handles "yyyy-MM-ddTHH:mm:ssZ"
-            timestamp = datetime.strptime(datetime_string, "%Y-%m-%dT%H:%M:%SZ").replace(
-                tzinfo=timezone.utc
-            )
-            dt_tuple = _DatetimeTuple("", "")  # ('2022-03-05T23:56:44', '0Z')
-
-        mantissa_wo_z = dt_tuple.mantissa[:-1]
-        nanoseconds = f"{mantissa_wo_z:0<9}"  # Add zeros on right.
-        seconds = str(int(timestamp.timestamp()))
+            if datetime_string[19] == ".":
+                datetime_part, mantissa = datetime_string.rsplit(".")
+                if mantissa[-1] == "Z":
+                    mantissa = mantissa[:-1]
+            else:
+                datetime_part, mantissa = datetime_string, ""
+        except:
+            datetime_part, mantissa = datetime_string, ""
+
+        dt = ciso8601.parse_datetime(datetime_part).replace(tzinfo=timezone.utc)
+
+        nanoseconds = f"{mantissa:0<9}"  # Add zeros on right.
+        seconds = str(int(dt.timestamp()))
 
         return seconds, nanoseconds
 
     @classmethod
     def parse_timestamp_int(cls, datetime_string: str) -> (int, int):
-        # TODO - there should be better solution
-        seconds, nanoseconds = cls.parse_timestamp(datetime_string)
-        return int(seconds), int(nanoseconds)
+        # Note:
+        #   we have similar code here (not the separate function)
+        #   to improve performance.
+        try:
+            if datetime_string[19] == ".":
+                datetime_part, mantissa = datetime_string.rsplit(".")
+                if mantissa[-1] == "Z":
+                    mantissa = mantissa[:-1]
+            else:
+                datetime_part, mantissa = datetime_string, ""
+        except:
+            datetime_part, mantissa = datetime_string, ""
+
+        dt = ciso8601.parse_datetime_as_naive(datetime_part).replace(tzinfo=timezone.utc)
+
+        return int(dt.timestamp()), int(f"{mantissa:0<9}")
+
+    @classmethod
+    def to_datetime(cls, datetime_string: str) -> datetime:
+        return ciso8601.parse_datetime_as_naive(datetime_string)
 
 
 class UniversalDatetimeStringConverter(ITimestampConverter[str]):
     """Converts datetime strings.
 
     If you request microseconds but your timestamp has nanoseconds,
     they will be just cut (not rounding).
 
     Expected timestamp format "yyyy-MM-ddTHH:mm:ss[.SSSSSSSSS]Z" or without Z or T as separators.
     """
 
     @classmethod
     def parse_timestamp(cls, datetime_string: str) -> (str, str):
-        if datetime_string.endswith("Z"):
-            datetime_string = datetime_string[:-1]
-        datetime_string = datetime_string.replace("T", " ")
-        # Exception handling works faster than using `if`.
         try:
-            # Handles "yyyy-MM-ddTHH:mm:ss.SSSSSSSSSZ"
-            dt_tuple = _DatetimeTuple(*datetime_string.rsplit("."))
-            timestamp = datetime.strptime(dt_tuple.datetime, "%Y-%m-%d %H:%M:%S").replace(
-                tzinfo=timezone.utc
-            )
-        except TypeError:
-            # Handles "yyyy-MM-ddTHH:mm:ssZ"
-            timestamp = datetime.strptime(datetime_string, "%Y-%m-%d %H:%M:%S").replace(
-                tzinfo=timezone.utc
-            )
-            dt_tuple = _DatetimeTuple("", "")  # ('2022-03-05T23:56:44', '0')
+            datetime_string = datetime_string.replace("T", " ")
+            if datetime_string[19] == ".":
+                datetime_part, mantissa = datetime_string.rsplit(".")
+                if mantissa[-1] == "Z":
+                    mantissa = mantissa[:-1]
+            else:
+                datetime_part, mantissa = datetime_string, ""
+        except:
+            datetime_part, mantissa = datetime_string, ""
+
+        dt = ciso8601.parse_datetime(datetime_part).replace(tzinfo=timezone.utc)
 
-        nanoseconds = f"{dt_tuple.mantissa:0<9}"  # Add zeros on right.
-        seconds = str(int(timestamp.timestamp()))
+        nanoseconds = f"{mantissa:0<9}"  # Add zeros on right.
+        seconds = str(int(dt.timestamp()))
 
         return seconds, nanoseconds
 
     @classmethod
     def parse_timestamp_int(cls, datetime_string: str) -> (int, int):
-        # TODO - there should be better solution
-        seconds, nanoseconds = cls.parse_timestamp(datetime_string)
-        return int(seconds), int(nanoseconds)
+        # Note:
+        #   we have similar code here (not the separate function)
+        #   to improve performance.
+        try:
+            datetime_string = datetime_string.replace("T", " ")
+            if datetime_string[19] == ".":
+                datetime_part, mantissa = datetime_string.rsplit(".")
+                if mantissa[-1] == "Z":
+                    mantissa = mantissa[:-1]
+            else:
+                datetime_part, mantissa = datetime_string, ""
+        except:
+            datetime_part, mantissa = datetime_string, ""
+
+        dt = ciso8601.parse_datetime(datetime_part).replace(tzinfo=timezone.utc)
+
+        return int(dt.timestamp()), int(f"{mantissa:0<9}")
+
+    @classmethod
+    def to_datetime(cls, datetime_string: str) -> datetime:
+        return ciso8601.parse_datetime_as_naive(datetime_string)
 
 
 class DatetimeConverter(ITimestampConverter[datetime]):
     """Converts datetime objects to timestamp.
 
     If you request milliseconds but your timestamp has microseconds, they will
     be just cut (not rounding).
@@ -187,16 +216,15 @@
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
             int: Timestamp in seconds format.
         """
-        seconds, nanoseconds = cls.parse_timestamp_int(timestamp)
-        return seconds
+        return timestamp["epochSecond"]
 
     @classmethod
     def to_microseconds(cls, timestamp: TimestampType) -> int:
         """Converts timestamp to microseconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
```

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/data_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev9113174303/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3930 3138 3031 3430 3832 0a53 756d 6d61  9018014082.Summa
+00000040: 3931 3133 3137 3433 3033 0a53 756d 6d61  9113174303.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -303,2360 +303,2382 @@
 000012e0: 6c6c 6f77 696e 6720 6578 616d 706c 6520  llowing example 
 000012f0: 6173 2061 2066 696c 655d 2865 7861 6d70  as a file](examp
 00001300: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
 00001310: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
 00001320: 2020 2020 200a 2020 2020 2020 2020 3c21       .        <!
 00001330: 2d2d 2073 7461 7274 2067 6574 5f73 7461  -- start get_sta
 00001340: 7274 6564 5f65 7861 6d70 6c65 2e70 7920  rted_example.py 
-00001350: 2d2d 3e0a 2020 2020 2020 2020 6060 6070  -->.        ```p
-00001360: 7974 686f 6e0a 2020 2020 2020 2020 6672  ython.        fr
-00001370: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00001380: 2054 7570 6c65 2c20 4c69 7374 2c20 4f70   Tuple, List, Op
-00001390: 7469 6f6e 616c 2c20 4765 6e65 7261 746f  tional, Generato
-000013a0: 720a 2020 2020 2020 2020 6672 6f6d 2064  r.        from d
-000013b0: 6174 6574 696d 6520 696d 706f 7274 2064  atetime import d
-000013c0: 6174 6574 696d 650a 2020 2020 2020 2020  atetime.        
-000013d0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-000013e0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-000013f0: 6461 7461 2069 6d70 6f72 7420 4461 7461  data import Data
-00001400: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001410: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001420: 6475 6d6d 7920 696d 706f 7274 2044 756d  dummy import Dum
-00001430: 6d79 4461 7461 536f 7572 6365 0a20 2020  myDataSource.   
-00001440: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-00001450: 7461 5f73 6572 7669 6365 732e 6576 656e  ta_services.even
-00001460: 745f 7472 6565 2069 6d70 6f72 7420 280a  t_tree import (.
-00001470: 2020 2020 2020 2020 2020 2020 4576 656e              Even
-00001480: 7454 7265 652c 0a20 2020 2020 2020 2020  tTree,.         
-00001490: 2020 2045 7665 6e74 5472 6565 436f 6c6c     EventTreeColl
-000014a0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
-000014b0: 2020 2020 5061 7265 6e74 4576 656e 7454      ParentEventT
-000014c0: 7265 6543 6f6c 6c65 6374 696f 6e2c 0a20  reeCollection,. 
-000014d0: 2020 2020 2020 2020 2020 2049 4554 4344             IETCD
-000014e0: 7269 7665 722c 0a20 2020 2020 2020 2029  river,.        )
-000014f0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
-00001500: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
-00001510: 696e 7465 7266 6163 6573 2069 6d70 6f72  interfaces impor
-00001520: 7420 4944 6174 6153 6f75 7263 650a 2020  t IDataSource.  
-00001530: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
-00001540: 6174 615f 7365 7276 6963 6573 2e75 7469  ata_services.uti
-00001550: 6c73 2e63 6f6e 7665 7274 6572 7320 696d  ls.converters im
-00001560: 706f 7274 2028 0a20 2020 2020 2020 2020  port (.         
-00001570: 2020 2044 6174 6574 696d 6543 6f6e 7665     DatetimeConve
-00001580: 7274 6572 2c0a 2020 2020 2020 2020 2020  rter,.          
-00001590: 2020 4461 7465 7469 6d65 5374 7269 6e67    DatetimeString
-000015a0: 436f 6e76 6572 7465 722c 0a20 2020 2020  Converter,.     
-000015b0: 2020 2020 2020 2050 726f 746f 6275 6654         ProtobufT
-000015c0: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
-000015d0: 722c 0a20 2020 2020 2020 2020 2020 2054  r,.            T
-000015e0: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
-000015f0: 7274 6572 2c0a 2020 2020 2020 2020 290a  rter,.        ).
-00001600: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001610: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00001350: 2d2d 3e0a 2020 2020 2020 2020 0a20 2020  -->.        .   
+00001360: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00001370: 2020 2020 2020 2066 726f 6d20 7479 7069         from typi
+00001380: 6e67 2069 6d70 6f72 7420 5475 706c 652c  ng import Tuple,
+00001390: 204c 6973 742c 204f 7074 696f 6e61 6c2c   List, Optional,
+000013a0: 2047 656e 6572 6174 6f72 0a20 2020 2020   Generator.     
+000013b0: 2020 2066 726f 6d20 6461 7465 7469 6d65     from datetime
+000013c0: 2069 6d70 6f72 7420 6461 7465 7469 6d65   import datetime
+000013d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000013e0: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+000013f0: 7365 7276 6963 6573 2e64 6174 6120 696d  services.data im
+00001400: 706f 7274 2044 6174 610a 2020 2020 2020  port Data.      
+00001410: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+00001420: 7365 7276 6963 6573 2e64 756d 6d79 2069  services.dummy i
+00001430: 6d70 6f72 7420 4475 6d6d 7944 6174 6153  mport DummyDataS
+00001440: 6f75 7263 650a 2020 2020 2020 2020 6672  ource.        fr
+00001450: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+00001460: 6963 6573 2e65 7665 6e74 5f74 7265 6520  ices.event_tree 
+00001470: 696d 706f 7274 2028 0a20 2020 2020 2020  import (.       
+00001480: 2020 2020 2045 7665 6e74 5472 6565 2c0a       EventTree,.
+00001490: 2020 2020 2020 2020 2020 2020 4576 656e              Even
+000014a0: 7454 7265 6543 6f6c 6c65 6374 696f 6e2c  tTreeCollection,
+000014b0: 0a20 2020 2020 2020 2020 2020 2050 6172  .            Par
+000014c0: 656e 7445 7665 6e74 5472 6565 436f 6c6c  entEventTreeColl
+000014d0: 6563 7469 6f6e 2c0a 2020 2020 2020 2020  ection,.        
+000014e0: 2020 2020 4945 5443 4472 6976 6572 2c0a      IETCDriver,.
+000014f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001500: 2020 6672 6f6d 2074 6832 5f64 6174 615f    from th2_data_
+00001510: 7365 7276 6963 6573 2e69 6e74 6572 6661  services.interfa
+00001520: 6365 7320 696d 706f 7274 2049 4461 7461  ces import IData
+00001530: 536f 7572 6365 0a20 2020 2020 2020 2066  Source.        f
+00001540: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
+00001550: 7669 6365 732e 7574 696c 732e 636f 6e76  vices.utils.conv
+00001560: 6572 7465 7273 2069 6d70 6f72 7420 280a  erters import (.
+00001570: 2020 2020 2020 2020 2020 2020 4461 7465              Date
+00001580: 7469 6d65 436f 6e76 6572 7465 722c 0a20  timeConverter,. 
+00001590: 2020 2020 2020 2020 2020 2044 6174 6574             Datet
+000015a0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000015b0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000015c0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
+000015d0: 7043 6f6e 7665 7274 6572 2c0a 2020 2020  pConverter,.    
+000015e0: 2020 2020 2020 2020 5468 3254 696d 6573          Th2Times
+000015f0: 7461 6d70 436f 6e76 6572 7465 722c 0a20  tampConverter,. 
+00001600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00001610: 200a 2020 2020 2020 2020 2323 2323 2323   .        ######
 00001620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001630: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
-00001640: 2320 5b30 5d20 4c69 6220 636f 6e66 6967  # [0] Lib config
-00001650: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-00001660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001640: 0a20 2020 2020 2020 2023 205b 305d 204c  .        # [0] L
+00001650: 6962 2063 6f6e 6669 6775 7261 7469 6f6e  ib configuration
+00001660: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
 00001670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001680: 2323 2323 2323 0a20 2020 2020 2020 200a  ######.        .
-00001690: 2020 2020 2020 2020 2320 5b30 2e31 5d20          # [0.1] 
-000016a0: 496e 7465 7261 6374 6976 6520 6f72 2053  Interactive or S
-000016b0: 6372 6970 7420 6d6f 6465 0a20 2020 2020  cript mode.     
-000016c0: 2020 2023 2049 6620 796f 7520 7573 6520     # If you use 
-000016d0: 7468 6520 6c69 6220 696e 2069 6e74 6572  the lib in inter
-000016e0: 6163 7469 7665 206d 6f64 6520 286a 7570  active mode (jup
-000016f0: 7974 6572 2c20 6970 7974 686f 6e29 2069  yter, ipython) i
-00001700: 7427 7320 7265 636f 6d6d 656e 6465 6420  t's recommended 
-00001710: 746f 2073 6574 2074 6865 2073 7065 6369  to set the speci
-00001720: 616c 0a20 2020 2020 2020 2023 2067 6c6f  al.        # glo
-00001730: 6261 6c20 7061 7261 6d65 7465 7220 746f  bal parameter to
-00001740: 2054 7275 652e 2049 7427 6c6c 206b 6565   True. It'll kee
-00001750: 7020 6361 6368 6520 6669 6c65 7320 6966  p cache files if
-00001760: 2073 6f6d 6574 6869 6e67 2077 656e 7420   something went 
-00001770: 7772 6f6e 672e 0a20 2020 2020 2020 2066  wrong..        f
-00001780: 726f 6d20 7468 325f 6461 7461 5f73 6572  rom th2_data_ser
-00001790: 7669 6365 732e 636f 6e66 6967 2069 6d70  vices.config imp
-000017a0: 6f72 7420 6f70 7469 6f6e 730a 2020 2020  ort options.    
-000017b0: 2020 2020 0a20 2020 2020 2020 206f 7074      .        opt
-000017c0: 696f 6e73 2e49 4e54 4552 4143 5449 5645  ions.INTERACTIVE
-000017d0: 5f4d 4f44 4520 3d20 5472 7565 0a20 2020  _MODE = True.   
-000017e0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-000017f0: 536f 6d65 2065 7861 6d70 6c65 2064 6174  Some example dat
-00001800: 610a 2020 2020 2020 2020 6576 656e 7473  a.        events
-00001810: 203d 2044 6174 6128 0a20 2020 2020 2020   = Data(.       
-00001820: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00001830: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00001840: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00001850: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
-00001860: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
-00001870: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
-00001880: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
-00001890: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
-000018a0: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
-000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018c0: 2020 2020 2262 6174 6368 4964 223a 204e      "batchId": N
-000018d0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000018e0: 2020 2020 2020 2020 2022 6973 4261 7463           "isBatc
-000018f0: 6865 6422 3a20 4661 6c73 652c 0a20 2020  hed": False,.   
-00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001910: 2022 6576 656e 744e 616d 6522 3a20 2253   "eventName": "S
-00001920: 6574 206f 6620 6175 746f 2d67 656e 6572  et of auto-gener
-00001930: 6174 6564 2065 7665 6e74 7320 666f 7220  ated events for 
-00001940: 6473 206c 6962 2074 6573 7469 6e67 222c  ds lib testing",
-00001950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001960: 2020 2020 2022 6576 656e 7454 7970 6522       "eventType"
-00001970: 3a20 2264 732d 6c69 622d 7465 7374 2d65  : "ds-lib-test-e
-00001980: 7665 6e74 222c 0a20 2020 2020 2020 2020  vent",.         
-00001990: 2020 2020 2020 2020 2020 2022 656e 6454             "endT
-000019a0: 696d 6573 7461 6d70 223a 207b 2265 706f  imestamp": {"epo
-000019b0: 6368 5365 636f 6e64 223a 2031 3637 3239  chSecond": 16729
-000019c0: 3237 3032 352c 2022 6e61 6e6f 223a 2035  27025, "nano": 5
-000019d0: 3631 3735 3130 3030 7d2c 0a20 2020 2020  61751000},.     
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000019f0: 7374 6172 7454 696d 6573 7461 6d70 223a  startTimestamp":
-00001a00: 207b 2265 706f 6368 5365 636f 6e64 223a   {"epochSecond":
-00001a10: 2031 3637 3239 3237 3032 352c 2022 6e61   1672927025, "na
-00001a20: 6e6f 223a 2035 3630 3837 3330 3030 7d2c  no": 560873000},
-00001a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a40: 2020 2020 2022 7061 7265 6e74 4576 656e       "parentEven
-00001a50: 7449 6422 3a20 4e6f 6e65 2c0a 2020 2020  tId": None,.    
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
-00001a80: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001a90: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
-00001aa0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
-00001ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ac0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
-00001ad0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001af0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
-00001b00: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
-00001b10: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
-00001b20: 6479 223a 205b 5d2c 0a20 2020 2020 2020  dy": [],.       
-00001b30: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001b40: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2265 7665 6e74 4964 223a 2022 6465    "eventId": "de
-00001b70: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
-00001b80: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
-00001b90: 3035 3536 3335 3232 3030 303a 3961 6462  05563522000:9adb
-00001ba0: 6233 6530 2d35 6638 622d 3463 3238 2d61  b3e0-5f8b-4c28-a
-00001bb0: 3261 632d 3733 3631 6538 6661 3730 3463  2ac-7361e8fa704c
-00001bc0: 3e64 656d 6f5f 626f 6f6b 5f31 3a74 6832  >demo_book_1:th2
-00001bd0: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
-00001be0: 3335 3730 3535 3633 3532 3230 3030 3a64  35705563522000:d
-00001bf0: 3631 6539 3330 612d 3864 3030 2d31 3165  61e930a-8d00-11e
-00001c00: 642d 6161 3161 2d64 3334 6136 3135 3531  d-aa1a-d34a61551
-00001c10: 3532 645f 3222 2c0a 2020 2020 2020 2020  52d_2",.        
-00001c20: 2020 2020 2020 2020 2020 2020 2262 6174              "bat
-00001c30: 6368 4964 223a 2022 6465 6d6f 5f62 6f6f  chId": "demo_boo
-00001c40: 6b5f 313a 7468 322d 7363 6f70 653a 3230  k_1:th2-scope:20
-00001c50: 3233 3031 3035 3133 3537 3035 3536 3335  2301051357055635
-00001c60: 3232 3030 303a 3961 6462 6233 6530 2d35  22000:9adbb3e0-5
-00001c70: 6638 622d 3463 3238 2d61 3261 632d 3733  f8b-4c28-a2ac-73
-00001c80: 3631 6538 6661 3730 3463 222c 0a20 2020  61e8fa704c",.   
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
-00001cb0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001cc0: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
-00001cd0: 6d65 223a 2022 506c 6169 6e20 6576 656e  me": "Plain even
-00001ce0: 7420 3122 2c0a 2020 2020 2020 2020 2020  t 1",.          
-00001cf0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00001d00: 5479 7065 223a 2022 6473 2d6c 6962 2d74  Type": "ds-lib-t
-00001d10: 6573 742d 6576 656e 7422 2c0a 2020 2020  est-event",.    
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d30: 2265 6e64 5469 6d65 7374 616d 7022 3a20  "endTimestamp": 
-00001d40: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
-00001d50: 3136 3732 3932 3730 3235 2c20 226e 616e  1672927025, "nan
-00001d60: 6f22 3a20 3536 3336 3430 3030 307d 2c0a  o": 563640000},.
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 2020 2020 2273 7461 7274 5469 6d65 7374      "startTimest
-00001d90: 616d 7022 3a20 7b22 6570 6f63 6853 6563  amp": {"epochSec
-00001da0: 6f6e 6422 3a20 3136 3732 3932 3730 3235  ond": 1672927025
-00001db0: 2c20 226e 616e 6f22 3a20 3536 3335 3232  , "nano": 563522
-00001dc0: 3030 307d 2c0a 2020 2020 2020 2020 2020  000},.          
-00001dd0: 2020 2020 2020 2020 2020 2270 6172 656e            "paren
-00001de0: 7445 7665 6e74 4964 223a 2022 6465 6d6f  tEventId": "demo
-00001df0: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00001e00: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00001e10: 3536 3038 3733 3030 303a 6436 3165 3933  560873000:d61e93
-00001e20: 3061 2d38 6430 302d 3131 6564 2d61 6131  0a-8d00-11ed-aa1
-00001e30: 612d 6433 3461 3631 3535 3135 3264 5f31  a-d34a6155152d_1
-00001e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001e50: 2020 2020 2020 2022 7375 6363 6573 7366         "successf
-00001e60: 756c 223a 2054 7275 652c 0a20 2020 2020  ul": True,.     
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001e80: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
-00001e90: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
-00001ea0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
-00001eb0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
-00001ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001ed0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
-00001ee0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f00: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
-00001f10: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
-00001f20: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
-00001f30: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
-00001f40: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001f70: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
-00001f80: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00001f90: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00001fa0: 3133 3537 3035 3536 3335 3232 3030 303a  135705563522000:
-00001fb0: 3961 6462 6233 6530 2d35 6638 622d 3463  9adbb3e0-5f8b-4c
-00001fc0: 3238 2d61 3261 632d 3733 3631 6538 6661  28-a2ac-7361e8fa
-00001fd0: 3730 3463 3e64 656d 6f5f 626f 6f6b 5f31  704c>demo_book_1
-00001fe0: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
-00001ff0: 3130 3531 3335 3730 3535 3633 3735 3730  1051357055637570
-00002000: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
-00002010: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
-00002020: 3135 3531 3532 645f 3322 2c0a 2020 2020  155152d_3",.    
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2262 6174 6368 4964 223a 2022 6465 6d6f  "batchId": "demo
-00002050: 5f62 6f6f 6b5f 313a 7468 322d 7363 6f70  _book_1:th2-scop
-00002060: 653a 3230 3233 3031 3035 3133 3537 3035  e:20230105135705
-00002070: 3536 3335 3232 3030 303a 3961 6462 6233  563522000:9adbb3
-00002080: 6530 2d35 6638 622d 3463 3238 2d61 3261  e0-5f8b-4c28-a2a
-00002090: 632d 3733 3631 6538 6661 3730 3463 222c  c-7361e8fa704c",
-000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000020b0: 2020 2020 2022 6973 4261 7463 6865 6422       "isBatched"
-000020c0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-000020d0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-000020e0: 6e74 4e61 6d65 223a 2022 506c 6169 6e20  ntName": "Plain 
-000020f0: 6576 656e 7420 3222 2c0a 2020 2020 2020  event 2",.      
-00002100: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00002110: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
-00002120: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
-00002150: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
-00002160: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
-00002170: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
-00002180: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-00002190: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
-000021a0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
-000021b0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
-000021c0: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
-000021d0: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000021f0: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
-00002200: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-00002210: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-00002220: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
-00002230: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
-00002240: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
-00002250: 3264 5f31 222c 0a20 2020 2020 2020 2020  2d_1",.         
-00002260: 2020 2020 2020 2020 2020 2022 7375 6363             "succ
-00002270: 6573 7366 756c 223a 2054 7275 652c 0a20  essful": True,. 
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2022 626f 6f6b 4964 223a 2022 6465     "bookId": "de
-000022a0: 6d6f 5f62 6f6f 6b5f 3122 2c0a 2020 2020  mo_book_1",.    
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2273 636f 7065 223a 2022 7468 322d 7363  "scope": "th2-sc
-000022d0: 6f70 6522 2c0a 2020 2020 2020 2020 2020  ope",.          
-000022e0: 2020 2020 2020 2020 2020 2261 7474 6163            "attac
-000022f0: 6865 644d 6573 7361 6765 4964 7322 3a20  hedMessageIds": 
-00002300: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
-00002310: 2020 2020 2020 2020 2262 6f64 7922 3a20          "body": 
-00002320: 7b22 7479 7065 223a 2022 6d65 7373 6167  {"type": "messag
-00002330: 6522 2c20 2264 6174 6122 3a20 2264 732d  e", "data": "ds-
-00002340: 6c69 6220 7465 7374 2062 6f64 7922 7d2c  lib test body"},
-00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002360: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00002370: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00002380: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00002390: 4964 223a 2022 6661 6b65 2d65 7665 6e74  Id": "fake-event
-000023a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
-000023b0: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
-000023c0: 6422 3a20 2266 616b 652d 6261 7463 6849  d": "fake-batchI
-000023d0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-000023e0: 2020 2020 2020 2020 2269 7342 6174 6368          "isBatch
-000023f0: 6564 223a 2054 7275 652c 0a20 2020 2020  ed": True,.     
-00002400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002410: 6576 656e 744e 616d 6522 3a20 2246 616b  eventName": "Fak
-00002420: 6520 6576 656e 7422 2c0a 2020 2020 2020  e event",.      
-00002430: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00002440: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
-00002450: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
-00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002470: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
-00002480: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
-00002490: 6422 3a20 3136 3732 3932 3730 3335 2c20  d": 1672927035, 
-000024a0: 226e 616e 6f22 3a20 3536 3337 3931 3030  "nano": 56379100
-000024b0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
-000024c0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
-000024d0: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
-000024e0: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
-000024f0: 3733 3235 2c20 226e 616e 6f22 3a20 3536  7325, "nano": 56
-00002500: 3337 3537 3030 307d 2c0a 2020 2020 2020  3757000},.      
-00002510: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00002520: 6172 656e 7445 7665 6e74 4964 223a 2022  arentEventId": "
-00002530: 6e6f 745f 6578 6973 7473 5f69 6e5f 7468  not_exists_in_th
-00002540: 655f 6576 656e 7473 5f73 7472 6561 6d22  e_events_stream"
-00002550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002560: 2020 2020 2020 2273 7563 6365 7373 6675        "successfu
-00002570: 6c22 3a20 4661 6c73 652c 0a20 2020 2020  l": False,.     
-00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002590: 626f 6f6b 4964 223a 2022 6465 6d6f 5f62  bookId": "demo_b
-000025a0: 6f6f 6b5f 3122 2c0a 2020 2020 2020 2020  ook_1",.        
-000025b0: 2020 2020 2020 2020 2020 2020 2273 636f              "sco
-000025c0: 7065 223a 2022 7468 322d 7363 6f70 6522  pe": "th2-scope"
-000025d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000025e0: 2020 2020 2020 2261 7474 6163 6865 644d        "attachedM
-000025f0: 6573 7361 6765 4964 7322 3a20 5b5d 2c0a  essageIds": [],.
-00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002610: 2020 2020 2262 6f64 7922 3a20 7b22 7479      "body": {"ty
-00002620: 7065 223a 2022 6d65 7373 6167 6522 2c20  pe": "message", 
-00002630: 2264 6174 6122 3a20 2264 732d 6c69 6220  "data": "ds-lib 
-00002640: 7465 7374 2062 6f64 7922 7d2c 0a20 2020  test body"},.   
-00002650: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00002660: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00002670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002680: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-00002690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000026a0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-000026b0: 2020 2020 2020 2020 2320 5b31 5d20 576f          # [1] Wo
-000026c0: 726b 696e 6720 7769 7468 2061 2044 6174  rking with a Dat
-000026d0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-000026e0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+00001680: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00001690: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000016a0: 2023 205b 302e 315d 2049 6e74 6572 6163   # [0.1] Interac
+000016b0: 7469 7665 206f 7220 5363 7269 7074 206d  tive or Script m
+000016c0: 6f64 650a 2020 2020 2020 2020 2320 4966  ode.        # If
+000016d0: 2079 6f75 2075 7365 2074 6865 206c 6962   you use the lib
+000016e0: 2069 6e20 696e 7465 7261 6374 6976 6520   in interactive 
+000016f0: 6d6f 6465 2028 6a75 7079 7465 722c 2069  mode (jupyter, i
+00001700: 7079 7468 6f6e 2920 6974 2773 2072 6563  python) it's rec
+00001710: 6f6d 6d65 6e64 6564 2074 6f20 7365 7420  ommended to set 
+00001720: 7468 6520 7370 6563 6961 6c0a 2020 2020  the special.    
+00001730: 2020 2020 2320 676c 6f62 616c 2070 6172      # global par
+00001740: 616d 6574 6572 2074 6f20 5472 7565 2e20  ameter to True. 
+00001750: 4974 276c 6c20 6b65 6570 2063 6163 6865  It'll keep cache
+00001760: 2066 696c 6573 2069 6620 736f 6d65 7468   files if someth
+00001770: 696e 6720 7765 6e74 2077 726f 6e67 2e0a  ing went wrong..
+00001780: 2020 2020 2020 2020 6672 6f6d 2074 6832          from th2
+00001790: 5f64 6174 615f 7365 7276 6963 6573 2e63  _data_services.c
+000017a0: 6f6e 6669 6720 696d 706f 7274 206f 7074  onfig import opt
+000017b0: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
+000017c0: 2020 2020 2020 6f70 7469 6f6e 732e 494e        options.IN
+000017d0: 5445 5241 4354 4956 455f 4d4f 4445 203d  TERACTIVE_MODE =
+000017e0: 2054 7275 650a 2020 2020 2020 2020 0a20   True.        . 
+000017f0: 2020 2020 2020 2023 2053 6f6d 6520 6578         # Some ex
+00001800: 616d 706c 6520 6461 7461 0a20 2020 2020  ample data.     
+00001810: 2020 2065 7665 6e74 7320 3d20 4461 7461     events = Data
+00001820: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001850: 2020 2020 2020 2265 7665 6e74 4964 223a        "eventId":
+00001860: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00001870: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00001880: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00001890: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+000018a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000018b0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
+000018c0: 2020 2020 2020 2020 2020 2020 2022 6261               "ba
+000018d0: 7463 6849 6422 3a20 4e6f 6e65 2c0a 2020  tchId": None,.  
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 2020 2269 7342 6174 6368 6564 223a 2046    "isBatched": F
+00001900: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00001910: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00001920: 4e61 6d65 223a 2022 5365 7420 6f66 2061  Name": "Set of a
+00001930: 7574 6f2d 6765 6e65 7261 7465 6420 6576  uto-generated ev
+00001940: 656e 7473 2066 6f72 2064 7320 6c69 6220  ents for ds lib 
+00001950: 7465 7374 696e 6722 2c0a 2020 2020 2020  testing",.      
+00001960: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00001970: 7665 6e74 5479 7065 223a 2022 6473 2d6c  ventType": "ds-l
+00001980: 6962 2d74 6573 742d 6576 656e 7422 2c0a  ib-test-event",.
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2020 2265 6e64 5469 6d65 7374 616d      "endTimestam
+000019b0: 7022 3a20 7b22 6570 6f63 6853 6563 6f6e  p": {"epochSecon
+000019c0: 6422 3a20 3136 3732 3932 3730 3235 2c20  d": 1672927025, 
+000019d0: 226e 616e 6f22 3a20 3536 3137 3531 3030  "nano": 56175100
+000019e0: 307d 2c0a 2020 2020 2020 2020 2020 2020  0},.            
+000019f0: 2020 2020 2020 2020 2273 7461 7274 5469          "startTi
+00001a00: 6d65 7374 616d 7022 3a20 7b22 6570 6f63  mestamp": {"epoc
+00001a10: 6853 6563 6f6e 6422 3a20 3136 3732 3932  hSecond": 167292
+00001a20: 3730 3235 2c20 226e 616e 6f22 3a20 3536  7025, "nano": 56
+00001a30: 3038 3733 3030 307d 2c0a 2020 2020 2020  0873000},.      
+00001a40: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00001a50: 6172 656e 7445 7665 6e74 4964 223a 204e  arentEventId": N
+00001a60: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001a70: 2020 2020 2020 2020 2022 7375 6363 6573           "succes
+00001a80: 7366 756c 223a 2054 7275 652c 0a20 2020  sful": True,.   
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2022 626f 6f6b 4964 223a 2022 6465 6d6f   "bookId": "demo
+00001ab0: 5f62 6f6f 6b5f 3122 2c0a 2020 2020 2020  _book_1",.      
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00001ad0: 636f 7065 223a 2022 7468 322d 7363 6f70  cope": "th2-scop
+00001ae0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00001af0: 2020 2020 2020 2020 2261 7474 6163 6865          "attache
+00001b00: 644d 6573 7361 6765 4964 7322 3a20 5b5d  dMessageIds": []
+00001b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b20: 2020 2020 2020 2262 6f64 7922 3a20 5b5d        "body": []
+00001b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00001b50: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001b60: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00001b70: 7449 6422 3a20 2264 656d 6f5f 626f 6f6b  tId": "demo_book
+00001b80: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
+00001b90: 3330 3130 3531 3335 3730 3535 3633 3532  3010513570556352
+00001ba0: 3230 3030 3a39 6164 6262 3365 302d 3566  2000:9adbb3e0-5f
+00001bb0: 3862 2d34 6332 382d 6132 6163 2d37 3336  8b-4c28-a2ac-736
+00001bc0: 3165 3866 6137 3034 633e 6465 6d6f 5f62  1e8fa704c>demo_b
+00001bd0: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00001be0: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+00001bf0: 3335 3232 3030 303a 6436 3165 3933 3061  3522000:d61e930a
+00001c00: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+00001c10: 6433 3461 3631 3535 3135 3264 5f32 222c  d34a6155152d_2",
+00001c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c30: 2020 2020 2022 6261 7463 6849 6422 3a20       "batchId": 
+00001c40: 2264 656d 6f5f 626f 6f6b 5f31 3a74 6832  "demo_book_1:th2
+00001c50: 2d73 636f 7065 3a32 3032 3330 3130 3531  -scope:202301051
+00001c60: 3335 3730 3535 3633 3532 3230 3030 3a39  35705563522000:9
+00001c70: 6164 6262 3365 302d 3566 3862 2d34 6332  adbb3e0-5f8b-4c2
+00001c80: 382d 6132 6163 2d37 3336 3165 3866 6137  8-a2ac-7361e8fa7
+00001c90: 3034 6322 2c0a 2020 2020 2020 2020 2020  04c",.          
+00001ca0: 2020 2020 2020 2020 2020 2269 7342 6174            "isBat
+00001cb0: 6368 6564 223a 2054 7275 652c 0a20 2020  ched": True,.   
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2022 6576 656e 744e 616d 6522 3a20 2250   "eventName": "P
+00001ce0: 6c61 696e 2065 7665 6e74 2031 222c 0a20  lain event 1",. 
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 2020 2022 6576 656e 7454 7970 6522 3a20     "eventType": 
+00001d10: 2264 732d 6c69 622d 7465 7374 2d65 7665  "ds-lib-test-eve
+00001d20: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+00001d30: 2020 2020 2020 2020 2022 656e 6454 696d           "endTim
+00001d40: 6573 7461 6d70 223a 207b 2265 706f 6368  estamp": {"epoch
+00001d50: 5365 636f 6e64 223a 2031 3637 3239 3237  Second": 1672927
+00001d60: 3032 352c 2022 6e61 6e6f 223a 2035 3633  025, "nano": 563
+00001d70: 3634 3030 3030 7d2c 0a20 2020 2020 2020  640000},.       
+00001d80: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00001d90: 6172 7454 696d 6573 7461 6d70 223a 207b  artTimestamp": {
+00001da0: 2265 706f 6368 5365 636f 6e64 223a 2031  "epochSecond": 1
+00001db0: 3637 3239 3237 3032 352c 2022 6e61 6e6f  672927025, "nano
+00001dc0: 223a 2035 3633 3532 3230 3030 7d2c 0a20  ": 563522000},. 
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
+00001df0: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00001e00: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00001e10: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
+00001e20: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00001e30: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+00001e40: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2273 7563 6365 7373 6675 6c22 3a20 5472  "successful": Tr
+00001e70: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001e80: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+00001e90: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+00001ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001eb0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+00001ec0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001ee0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00001ef0: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00001f00: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00001f10: 6479 223a 207b 2274 7970 6522 3a20 226d  dy": {"type": "m
+00001f20: 6573 7361 6765 222c 2022 6461 7461 223a  essage", "data":
+00001f30: 2022 6473 2d6c 6962 2074 6573 7420 626f   "ds-lib test bo
+00001f40: 6479 227d 2c0a 2020 2020 2020 2020 2020  dy"},.          
+00001f50: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001f60: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001f80: 6576 656e 7449 6422 3a20 2264 656d 6f5f  eventId": "demo_
+00001f90: 626f 6f6b 5f31 3a74 6832 2d73 636f 7065  book_1:th2-scope
+00001fa0: 3a32 3032 3330 3130 3531 3335 3730 3535  :202301051357055
+00001fb0: 3633 3532 3230 3030 3a39 6164 6262 3365  63522000:9adbb3e
+00001fc0: 302d 3566 3862 2d34 6332 382d 6132 6163  0-5f8b-4c28-a2ac
+00001fd0: 2d37 3336 3165 3866 6137 3034 633e 6465  -7361e8fa704c>de
+00001fe0: 6d6f 5f62 6f6f 6b5f 313a 7468 322d 7363  mo_book_1:th2-sc
+00001ff0: 6f70 653a 3230 3233 3031 3035 3133 3537  ope:202301051357
+00002000: 3035 3536 3337 3537 3030 303a 6436 3165  05563757000:d61e
+00002010: 3933 3061 2d38 6430 302d 3131 6564 2d61  930a-8d00-11ed-a
+00002020: 6131 612d 6433 3461 3631 3535 3135 3264  a1a-d34a6155152d
+00002030: 5f33 222c 0a20 2020 2020 2020 2020 2020  _3",.           
+00002040: 2020 2020 2020 2020 2022 6261 7463 6849           "batchI
+00002050: 6422 3a20 2264 656d 6f5f 626f 6f6b 5f31  d": "demo_book_1
+00002060: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00002070: 3130 3531 3335 3730 3535 3633 3532 3230  1051357055635220
+00002080: 3030 3a39 6164 6262 3365 302d 3566 3862  00:9adbb3e0-5f8b
+00002090: 2d34 6332 382d 6132 6163 2d37 3336 3165  -4c28-a2ac-7361e
+000020a0: 3866 6137 3034 6322 2c0a 2020 2020 2020  8fa704c",.      
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+000020c0: 7342 6174 6368 6564 223a 2054 7275 652c  sBatched": True,
+000020d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020e0: 2020 2020 2022 6576 656e 744e 616d 6522       "eventName"
+000020f0: 3a20 2250 6c61 696e 2065 7665 6e74 2032  : "Plain event 2
+00002100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002110: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
+00002120: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
+00002130: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
+00002140: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+00002150: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
+00002160: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
+00002170: 3239 3237 3032 352c 2022 6e61 6e6f 223a  2927025, "nano":
+00002180: 2035 3633 3739 3130 3030 7d2c 0a20 2020   563791000},.   
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
+000021b0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
+000021c0: 223a 2031 3637 3239 3237 3032 352c 2022  ": 1672927025, "
+000021d0: 6e61 6e6f 223a 2035 3633 3735 3730 3030  nano": 563757000
+000021e0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000021f0: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
+00002200: 656e 7449 6422 3a20 2264 656d 6f5f 626f  entId": "demo_bo
+00002210: 6f6b 5f31 3a74 6832 2d73 636f 7065 3a32  ok_1:th2-scope:2
+00002220: 3032 3330 3130 3531 3335 3730 3535 3630  0230105135705560
+00002230: 3837 3330 3030 3a64 3631 6539 3330 612d  873000:d61e930a-
+00002240: 3864 3030 2d31 3165 642d 6161 3161 2d64  8d00-11ed-aa1a-d
+00002250: 3334 6136 3135 3531 3532 645f 3122 2c0a  34a6155152d_1",.
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
+00002280: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+00002290: 2020 2020 2020 2020 2020 2020 2262 6f6f              "boo
+000022a0: 6b49 6422 3a20 2264 656d 6f5f 626f 6f6b  kId": "demo_book
+000022b0: 5f31 222c 0a20 2020 2020 2020 2020 2020  _1",.           
+000022c0: 2020 2020 2020 2020 2022 7363 6f70 6522           "scope"
+000022d0: 3a20 2274 6832 2d73 636f 7065 222c 0a20  : "th2-scope",. 
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 2020 2022 6174 7461 6368 6564 4d65 7373     "attachedMess
+00002300: 6167 6549 6473 223a 205b 5d2c 0a20 2020  ageIds": [],.   
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2022 626f 6479 223a 207b 2274 7970 6522   "body": {"type"
+00002330: 3a20 226d 6573 7361 6765 222c 2022 6461  : "message", "da
+00002340: 7461 223a 2022 6473 2d6c 6962 2074 6573  ta": "ds-lib tes
+00002350: 7420 626f 6479 227d 2c0a 2020 2020 2020  t body"},.      
+00002360: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00002370: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 2022 6576 656e 7449 6422 3a20 2266     "eventId": "f
+000023a0: 616b 652d 6576 656e 7449 6422 2c0a 2020  ake-eventId",.  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2262 6174 6368 4964 223a 2022 6661    "batchId": "fa
+000023d0: 6b65 2d62 6174 6368 4964 222c 0a20 2020  ke-batchId",.   
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2022 6973 4261 7463 6865 6422 3a20 5472   "isBatched": Tr
+00002400: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00002410: 2020 2020 2020 2020 2265 7665 6e74 4e61          "eventNa
+00002420: 6d65 223a 2022 4661 6b65 2065 7665 6e74  me": "Fake event
+00002430: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002440: 2020 2020 2020 2022 6576 656e 7454 7970         "eventTyp
+00002450: 6522 3a20 2264 732d 6c69 622d 7465 7374  e": "ds-lib-test
+00002460: 2d65 7665 6e74 222c 0a20 2020 2020 2020  -event",.       
+00002470: 2020 2020 2020 2020 2020 2020 2022 656e               "en
+00002480: 6454 696d 6573 7461 6d70 223a 207b 2265  dTimestamp": {"e
+00002490: 706f 6368 5365 636f 6e64 223a 2031 3637  pochSecond": 167
+000024a0: 3239 3237 3033 352c 2022 6e61 6e6f 223a  2927035, "nano":
+000024b0: 2035 3633 3739 3130 3030 7d2c 0a20 2020   563791000},.   
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2022 7374 6172 7454 696d 6573 7461 6d70   "startTimestamp
+000024e0: 223a 207b 2265 706f 6368 5365 636f 6e64  ": {"epochSecond
+000024f0: 223a 2031 3637 3239 3237 3332 352c 2022  ": 1672927325, "
+00002500: 6e61 6e6f 223a 2035 3633 3735 3730 3030  nano": 563757000
+00002510: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00002520: 2020 2020 2020 2022 7061 7265 6e74 4576         "parentEv
+00002530: 656e 7449 6422 3a20 226e 6f74 5f65 7869  entId": "not_exi
+00002540: 7374 735f 696e 5f74 6865 5f65 7665 6e74  sts_in_the_event
+00002550: 735f 7374 7265 616d 222c 0a20 2020 2020  s_stream",.     
+00002560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002570: 7375 6363 6573 7366 756c 223a 2046 616c  successful": Fal
+00002580: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002590: 2020 2020 2020 2020 2262 6f6f 6b49 6422          "bookId"
+000025a0: 3a20 2264 656d 6f5f 626f 6f6b 5f31 222c  : "demo_book_1",
+000025b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025c0: 2020 2020 2022 7363 6f70 6522 3a20 2274       "scope": "t
+000025d0: 6832 2d73 636f 7065 222c 0a20 2020 2020  h2-scope",.     
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000025f0: 6174 7461 6368 6564 4d65 7373 6167 6549  attachedMessageI
+00002600: 6473 223a 205b 5d2c 0a20 2020 2020 2020  ds": [],.       
+00002610: 2020 2020 2020 2020 2020 2020 2022 626f               "bo
+00002620: 6479 223a 207b 2274 7970 6522 3a20 226d  dy": {"type": "m
+00002630: 6573 7361 6765 222c 2022 6461 7461 223a  essage", "data":
+00002640: 2022 6473 2d6c 6962 2074 6573 7420 626f   "ds-lib test bo
+00002650: 6479 227d 2c0a 2020 2020 2020 2020 2020  dy"},.          
+00002660: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002670: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
+00002680: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002690: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+000026a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000026b0: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
+000026c0: 2023 205b 315d 2057 6f72 6b69 6e67 2077   # [1] Working w
+000026d0: 6974 6820 6120 4461 7461 206f 626a 6563  ith a Data objec
+000026e0: 742e 0a20 2020 2020 2020 2023 2323 2323  t..        #####
 000026f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002700: 2323 2323 2323 2323 0a20 2020 2020 2020  ########.       
-00002710: 200a 2020 2020 2020 2020 2320 5b31 2e31   .        # [1.1
-00002720: 5d20 4669 6c74 6572 2e0a 2020 2020 2020  ] Filter..      
-00002730: 2020 6669 6c74 6572 6564 5f65 7665 6e74    filtered_event
-00002740: 733a 2044 6174 6120 3d20 6576 656e 7473  s: Data = events
-00002750: 2e66 696c 7465 7228 6c61 6d62 6461 2065  .filter(lambda e
-00002760: 3a20 655b 2262 6f64 7922 5d20 213d 205b  : e["body"] != [
-00002770: 5d29 2020 2320 4669 6c74 6572 2065 7665  ])  # Filter eve
-00002780: 6e74 7320 7769 7468 2065 6d70 7479 2062  nts with empty b
-00002790: 6f64 792e 0a20 2020 2020 2020 200a 2020  ody..        .  
-000027a0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000027b0: 205b 312e 325d 204d 6170 2e0a 2020 2020   [1.2] Map..    
-000027c0: 2020 2020 6465 6620 7472 616e 7366 6f72      def transfor
-000027d0: 6d5f 6675 6e63 7469 6f6e 2872 6563 6f72  m_function(recor
-000027e0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-000027f0: 7265 7475 726e 207b 2265 7665 6e74 4e61  return {"eventNa
-00002800: 6d65 223a 2072 6563 6f72 645b 2265 7665  me": record["eve
-00002810: 6e74 4e61 6d65 225d 2c20 2273 7563 6365  ntName"], "succe
-00002820: 7373 6675 6c22 3a20 7265 636f 7264 5b22  ssful": record["
-00002830: 7375 6363 6573 7366 756c 225d 7d0a 2020  successful"]}.  
-00002840: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-00002850: 2020 2020 2020 2020 6669 6c74 6572 6564          filtered
-00002860: 5f61 6e64 5f6d 6170 7065 645f 6576 656e  _and_mapped_even
-00002870: 7473 203d 2066 696c 7465 7265 645f 6576  ts = filtered_ev
-00002880: 656e 7473 2e6d 6170 2874 7261 6e73 666f  ents.map(transfo
-00002890: 726d 5f66 756e 6374 696f 6e29 0a20 2020  rm_function).   
-000028a0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-000028b0: 5b31 2e33 5d20 4461 7461 2070 6970 656c  [1.3] Data pipel
-000028c0: 696e 652e 0a20 2020 2020 2020 2023 2020  ine..        #  
-000028d0: 2020 2020 2049 6e73 7465 6164 206f 6620       Instead of 
-000028e0: 646f 696e 6720 6461 7461 2074 7261 6e73  doing data trans
-000028f0: 666f 726d 6174 696f 6e73 2073 7465 7020  formations step 
-00002900: 6279 2073 7465 7020 796f 7520 6361 6e20  by step you can 
-00002910: 646f 2069 7420 696e 206f 6e65 206c 696e  do it in one lin
-00002920: 652e 0a20 2020 2020 2020 2066 696c 7465  e..        filte
-00002930: 7265 645f 616e 645f 6d61 7070 6564 5f65  red_and_mapped_e
-00002940: 7665 6e74 735f 6279 5f70 6970 656c 696e  vents_by_pipelin
-00002950: 6520 3d20 6576 656e 7473 2e66 696c 7465  e = events.filte
-00002960: 7228 6c61 6d62 6461 2065 3a20 655b 2262  r(lambda e: e["b
-00002970: 6f64 7922 5d20 213d 205b 5d29 2e6d 6170  ody"] != []).map
-00002980: 280a 2020 2020 2020 2020 2020 2020 7472  (.            tr
-00002990: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
-000029a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000029b0: 2020 2023 2043 6f6e 7465 6e74 206f 6620     # Content of 
-000029c0: 7468 6573 6520 7477 6f20 4461 7461 206f  these two Data o
-000029d0: 626a 6563 7473 2073 686f 756c 6420 6265  bjects should be
-000029e0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
-000029f0: 6173 7365 7274 206c 6973 7428 6669 6c74  assert list(filt
-00002a00: 6572 6564 5f61 6e64 5f6d 6170 7065 645f  ered_and_mapped_
-00002a10: 6576 656e 7473 2920 3d3d 206c 6973 7428  events) == list(
-00002a20: 6669 6c74 6572 6564 5f61 6e64 5f6d 6170  filtered_and_map
-00002a30: 7065 645f 6576 656e 7473 5f62 795f 7069  ped_events_by_pi
-00002a40: 7065 6c69 6e65 290a 2020 2020 2020 2020  peline).        
-00002a50: 0a20 2020 2020 2020 2023 205b 312e 345d  .        # [1.4]
-00002a60: 2053 6966 742e 2053 6b69 7020 7468 6520   Sift. Skip the 
-00002a70: 6669 7273 7420 6665 7720 6974 656d 7320  first few items 
-00002a80: 6f72 206c 696d 6974 2074 6865 6d2e 0a20  or limit them.. 
-00002a90: 2020 2020 2020 2064 6174 6120 3d20 4461         data = Da
-00002aa0: 7461 285b 312c 2032 2c20 332c 2034 2c20  ta([1, 2, 3, 4, 
-00002ab0: 352c 2036 2c20 372c 2038 2c20 392c 2031  5, 6, 7, 8, 9, 1
-00002ac0: 302c 2031 312c 2031 322c 2031 332c 2031  0, 11, 12, 13, 1
-00002ad0: 342c 2031 355d 290a 2020 2020 2020 2020  4, 15]).        
-00002ae0: 6974 656d 735f 6672 6f6d 5f31 315f 746f  items_from_11_to
-00002af0: 5f65 6e64 3a20 4765 6e65 7261 746f 7220  _end: Generator 
-00002b00: 3d20 6461 7461 2e73 6966 7428 736b 6970  = data.sift(skip
-00002b10: 3d31 3029 0a20 2020 2020 2020 206f 6e6c  =10).        onl
-00002b20: 795f 6669 7273 745f 3130 5f69 7465 6d73  y_first_10_items
-00002b30: 3a20 4765 6e65 7261 746f 7220 3d20 6461  : Generator = da
-00002b40: 7461 2e73 6966 7428 6c69 6d69 743d 3130  ta.sift(limit=10
-00002b50: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00002b60: 2020 2023 205b 312e 355d 2043 6861 6e67     # [1.5] Chang
-00002b70: 696e 6720 6361 6368 6520 7374 6174 7573  ing cache status
-00002b80: 2e0a 2020 2020 2020 2020 6576 656e 7473  ..        events
-00002b90: 2e75 7365 5f63 6163 6865 2854 7275 6529  .use_cache(True)
-00002ba0: 0a20 2020 2020 2020 2023 206f 7220 6a75  .        # or ju
-00002bb0: 7374 0a20 2020 2020 2020 2065 7665 6e74  st.        event
-00002bc0: 732e 7573 655f 6361 6368 6528 2920 2023  s.use_cache()  #
-00002bd0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
-00002be0: 6163 7469 7661 7465 2063 6163 6865 2e0a  activate cache..
-00002bf0: 2020 2020 2020 2020 2320 5b31 2e36 5d20          # [1.6] 
-00002c00: 5761 6c6b 2074 6872 6f75 6768 2064 6174  Walk through dat
-00002c10: 612e 0a20 2020 2020 2020 2066 6f72 2065  a..        for e
-00002c20: 7665 6e74 2069 6e20 6576 656e 7473 3a0a  vent in events:.
-00002c30: 2020 2020 2020 2020 2020 2020 2320 446f              # Do
-00002c40: 2073 6f6d 6574 6869 6e67 2077 6974 6820   something with 
-00002c50: 6576 656e 7420 2865 7665 6e74 2069 7320  event (event is 
-00002c60: 6120 6469 6374 292e 0a20 2020 2020 2020  a dict)..       
-00002c70: 2020 2020 2070 7269 6e74 2865 7665 6e74       print(event
-00002c80: 290a 2020 2020 2020 2020 2320 4166 7465  ).        # Afte
-00002c90: 7220 6669 7273 7420 6974 6572 6174 696f  r first iteratio
-00002ca0: 6e20 7468 6520 6576 656e 7473 2068 6173  n the events has
-00002cb0: 2061 2063 6163 6865 2066 696c 652e 0a20   a cache file.. 
-00002cc0: 2020 2020 2020 2023 204e 6f77 2074 6865         # Now the
-00002cd0: 7920 7769 6c6c 2062 6520 7573 6564 2069  y will be used i
-00002ce0: 6e20 7468 6520 6361 6368 6520 696e 2074  n the cache in t
-00002cf0: 6865 206e 6578 7420 6974 6572 6174 696f  he next iteratio
-00002d00: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00002d10: 2020 2020 2320 5b31 2e37 5d20 4765 7420      # [1.7] Get 
-00002d20: 6e75 6d62 6572 206f 6620 7468 6520 656c  number of the el
-00002d30: 656d 656e 7473 2069 6e20 7468 6520 4461  ements in the Da
-00002d40: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
-00002d50: 2020 206e 756d 6265 725f 6f66 5f65 7665     number_of_eve
-00002d60: 6e74 7320 3d20 6576 656e 7473 2e6c 656e  nts = events.len
-00002d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002d80: 2020 2320 5b31 2e38 5d20 4368 6563 6b20    # [1.8] Check 
-00002d90: 7468 6174 2044 6174 6120 6f62 6a65 6374  that Data object
-00002da0: 2069 736e 2774 2065 6d70 7479 2e0a 2020   isn't empty..  
-00002db0: 2020 2020 2020 2320 5468 6520 6461 7461        # The data
-00002dc0: 2073 6f75 7263 6520 7368 6f75 6c64 2062   source should b
-00002dd0: 6520 6e6f 7420 656d 7074 792e 0a20 2020  e not empty..   
-00002de0: 2020 2020 2061 7373 6572 7420 6576 656e       assert even
-00002df0: 7473 2e69 735f 656d 7074 7920 6973 2046  ts.is_empty is F
-00002e00: 616c 7365 0a20 2020 2020 2020 200a 2020  alse.        .  
-00002e10: 2020 2020 2020 2320 5b31 2e39 5d20 436f        # [1.9] Co
-00002e20: 6e76 6572 7420 4461 7461 206f 626a 6563  nvert Data objec
-00002e30: 7420 746f 2074 6865 206c 6973 7420 6f66  t to the list of
-00002e40: 2065 6c65 6d65 6e74 7328 6576 656e 7473   elements(events
-00002e50: 206f 7220 6d65 7373 6167 6573 292e 0a20   or messages).. 
-00002e60: 2020 2020 2020 2023 2042 6520 6361 7265         # Be care
-00002e70: 6675 6c2c 2074 6869 7320 6361 6e20 7461  ful, this can ta
-00002e80: 6b65 2074 6f6f 206d 7563 6820 6d65 6d6f  ke too much memo
-00002e90: 7279 2e0a 2020 2020 2020 2020 6576 656e  ry..        even
-00002ea0: 7473 5f6c 6973 7420 3d20 6c69 7374 2865  ts_list = list(e
-00002eb0: 7665 6e74 7329 0a20 2020 2020 2020 200a  vents).        .
-00002ec0: 2020 2020 2020 2020 2320 5b31 2e31 305d          # [1.10]
-00002ed0: 2054 6865 2063 6163 6865 2069 6e68 6572   The cache inher
-00002ee0: 6974 616e 6365 2e0a 2020 2020 2020 2020  itance..        
-00002ef0: 2320 4372 6561 7465 7320 6120 6e65 7720  # Creates a new 
-00002f00: 4461 7461 206f 626a 6563 7420 7468 6174  Data object that
-00002f10: 2077 696c 6c20 7573 6520 6361 6368 6520   will use cache 
-00002f20: 6672 6f6d 2074 6865 2065 7665 6e74 7320  from the events 
-00002f30: 4461 7461 206f 626a 6563 742e 0a20 2020  Data object..   
-00002f40: 2020 2020 2065 7665 6e74 735f 6669 6c74       events_filt
-00002f50: 6572 6564 3a20 4461 7461 203d 2065 7665  ered: Data = eve
-00002f60: 6e74 732e 6669 6c74 6572 286c 616d 6264  nts.filter(lambd
-00002f70: 6120 7265 636f 7264 3a20 7265 636f 7264  a record: record
-00002f80: 2e67 6574 2822 6261 7463 6849 6422 2929  .get("batchId"))
-00002f90: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00002fa0: 2020 2320 4e65 7720 4461 7461 206f 626a    # New Data obj
-00002fb0: 6563 7473 2064 6f6e 2774 2075 7365 2074  ects don't use t
-00002fc0: 6865 6972 206f 776e 2063 6163 6865 2062  heir own cache b
-00002fd0: 7920 6465 6661 756c 7420 6275 7420 7573  y default but us
-00002fe0: 6520 7468 6520 6361 6368 6520 6f66 2074  e the cache of t
-00002ff0: 6865 2070 6172 656e 7420 4461 7461 206f  he parent Data o
-00003000: 626a 6563 742e 0a20 2020 2020 2020 2023  bject..        #
-00003010: 2055 7365 2075 7365 5f63 6163 6865 206d   Use use_cache m
-00003020: 6574 686f 6420 746f 2061 6374 6976 6174  ethod to activat
-00003030: 6520 6361 6368 696e 672e 0a20 2020 2020  e caching..     
-00003040: 2020 2023 2041 6674 6572 2074 6861 742c     # After that,
-00003050: 2074 6865 2044 6174 6120 6f62 6a65 6374   the Data object
-00003060: 2077 696c 6c20 6372 6561 7465 2069 7473   will create its
-00003070: 206f 776e 2063 6163 6865 2066 696c 652e   own cache file.
-00003080: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
-00003090: 6669 6c74 6572 6564 2e75 7365 5f63 6163  filtered.use_cac
-000030a0: 6865 2829 0a20 2020 2020 2020 200a 2020  he().        .  
-000030b0: 2020 2020 2020 6c69 7374 2865 7665 6e74        list(event
-000030c0: 735f 6669 6c74 6572 6564 2920 2023 204a  s_filtered)  # J
-000030d0: 7573 7420 746f 2069 7465 7261 7465 2044  ust to iterate D
-000030e0: 6174 6120 6f62 6a65 6374 2028 6361 6368  ata object (cach
-000030f0: 6520 6669 6c65 2077 696c 6c20 6265 2063  e file will be c
-00003100: 7265 6174 6564 292e 0a20 2020 2020 2020  reated)..       
-00003110: 200a 2020 2020 2020 2020 6669 6c74 6572   .        filter
-00003120: 6564 5f65 7665 6e74 735f 7479 7065 7320  ed_events_types 
-00003130: 3d20 6576 656e 7473 5f66 696c 7465 7265  = events_filtere
-00003140: 642e 6d61 7028 6c61 6d62 6461 2072 6563  d.map(lambda rec
-00003150: 6f72 643a 207b 2265 7665 6e74 5479 7065  ord: {"eventType
-00003160: 223a 2072 6563 6f72 642e 6765 7428 2265  ": record.get("e
-00003170: 7665 6e74 5479 7065 2229 7d29 0a20 2020  ventType")}).   
-00003180: 2020 2020 200a 2020 2020 2020 2020 6576       .        ev
-00003190: 656e 7473 5f77 6974 686f 7574 5f74 7970  ents_without_typ
-000031a0: 6573 5f77 6974 685f 6261 7463 6820 3d20  es_with_batch = 
-000031b0: 6669 6c74 6572 6564 5f65 7665 6e74 735f  filtered_events_
-000031c0: 7479 7065 732e 6669 6c74 6572 280a 2020  types.filter(.  
-000031d0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-000031e0: 2072 6563 6f72 643a 206e 6f74 2072 6563   record: not rec
-000031f0: 6f72 642e 6765 7428 2265 7665 6e74 5479  ord.get("eventTy
-00003200: 7065 2229 0a20 2020 2020 2020 2029 0a20  pe").        ). 
-00003210: 2020 2020 2020 2065 7665 6e74 735f 7769         events_wi
-00003220: 7468 6f75 745f 7479 7065 735f 7769 7468  thout_types_with
-00003230: 5f62 6174 6368 2e75 7365 5f63 6163 6865  _batch.use_cache
-00003240: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
-00003250: 2020 2020 2320 5b31 2e31 315d 2044 6174      # [1.11] Dat
-00003260: 6120 6f62 6a65 6374 7320 6a6f 696e 696e  a objects joinin
-00003270: 672e 0a20 2020 2020 2020 2023 2059 6f75  g..        # You
-00003280: 2068 6176 6520 7468 6520 666f 6c6c 6f77   have the follow
-00003290: 696e 6720 3320 4461 7461 206f 626a 6563  ing 3 Data objec
-000032a0: 7473 2e0a 2020 2020 2020 2020 6431 203d  ts..        d1 =
-000032b0: 2044 6174 6128 5b31 2c20 322c 2033 5d29   Data([1, 2, 3])
-000032c0: 0a20 2020 2020 2020 2064 3220 3d20 4461  .        d2 = Da
-000032d0: 7461 285b 2261 222c 207b 2269 6422 3a20  ta(["a", {"id": 
-000032e0: 3132 337d 2c20 2263 225d 290a 2020 2020  123}, "c"]).    
-000032f0: 2020 2020 6433 203d 2044 6174 6128 5b37      d3 = Data([7
-00003300: 2c20 382c 2039 5d29 0a20 2020 2020 2020  , 8, 9]).       
-00003310: 2023 2059 6f75 2063 616e 206a 6f69 6e20   # You can join 
-00003320: 4461 7461 206f 626a 6563 7473 2069 6e20  Data objects in 
-00003330: 666f 6c6c 6f77 696e 6720 7761 7973 2e0a  following ways..
-00003340: 2020 2020 2020 2020 2320 506c 6561 7365          # Please
-00003350: 206e 6f74 652c 206e 6577 2044 6174 6120   note, new Data 
-00003360: 6f62 6a65 6374 2077 696c 6c20 6861 7665  object will have
-00003370: 2063 6163 6865 2073 7461 7475 7320 3d3d   cache status ==
-00003380: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
-00003390: 6461 7461 5f76 6961 5f69 6e69 7420 3d20  data_via_init = 
-000033a0: 4461 7461 285b 6431 2c20 6432 2c20 6433  Data([d1, d2, d3
-000033b0: 5d29 0a20 2020 2020 2020 2064 6174 615f  ]).        data_
-000033c0: 7669 615f 6164 6420 3d20 6431 202b 2064  via_add = d1 + d
-000033d0: 3220 2b20 6433 0a20 2020 2020 2020 2064  2 + d3.        d
-000033e0: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
-000033f0: 615f 6f62 6a5f 7669 615f 696e 6974 203d  a_obj_via_init =
-00003400: 2044 6174 6128 5b64 312c 205b 2261 222c   Data([d1, ["a",
-00003410: 207b 2269 6422 3a20 3132 337d 2c20 2263   {"id": 123}, "c
-00003420: 225d 2c20 6433 5d29 0a20 2020 2020 2020  "], d3]).       
-00003430: 2064 6174 615f 7769 7468 5f6e 6f6e 5f64   data_with_non_d
-00003440: 6174 615f 6f62 6a5f 7669 615f 6164 6420  ata_obj_via_add 
-00003450: 3d20 6431 202b 205b 2261 222c 207b 2269  = d1 + ["a", {"i
-00003460: 6422 3a20 3132 337d 2c20 2263 225d 202b  d": 123}, "c"] +
-00003470: 2064 330a 2020 2020 2020 2020 2320 596f   d3.        # Yo
-00003480: 7520 6361 6e20 6a6f 696e 2063 7572 7265  u can join curre
-00003490: 6e74 2044 6174 6120 6f62 6a65 6374 206f  nt Data object o
-000034a0: 6e20 706c 6163 6520 7573 696e 6720 2b3d  n place using +=
-000034b0: 2e0a 2020 2020 2020 2020 2320 4974 2077  ..        # It w
-000034c0: 696c 6c20 6b65 6570 2063 6163 6865 2073  ill keep cache s
-000034d0: 7461 7475 732e 0a20 2020 2020 2020 2064  tatus..        d
-000034e0: 3120 2b3d 2064 3320 2023 2064 3120 7769  1 += d3  # d1 wi
-000034f0: 6c6c 2062 6563 6f6d 6520 4461 7461 285b  ll become Data([
-00003500: 312c 322c 332c 372c 382c 395d 290a 2020  1,2,3,7,8,9]).  
-00003510: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003520: 205b 312e 3132 5d20 4275 696c 6420 616e   [1.12] Build an
-00003530: 6420 7265 6164 2044 6174 6120 6f62 6a65  d read Data obje
-00003540: 6374 2063 6163 6865 2066 696c 6573 2e0a  ct cache files..
-00003550: 2020 2020 2020 2020 6576 656e 7473 2e62          events.b
-00003560: 7569 6c64 5f63 6163 6865 2822 6361 6368  uild_cache("cach
-00003570: 655f 6669 6c65 6e61 6d65 5f6f 725f 7061  e_filename_or_pa
-00003580: 7468 2229 0a20 2020 2020 2020 2064 6174  th").        dat
-00003590: 615f 6f62 6a5f 6672 6f6d 5f63 6163 6865  a_obj_from_cache
-000035a0: 203d 2044 6174 612e 6672 6f6d 5f63 6163   = Data.from_cac
-000035b0: 6865 5f66 696c 6528 2263 6163 6865 5f66  he_file("cache_f
-000035c0: 696c 656e 616d 655f 6f72 5f70 6174 6822  ilename_or_path"
-000035d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000035e0: 2020 2023 205b 312e 3133 5d20 4368 6563     # [1.13] Chec
-000035f0: 6b20 6966 2044 6174 6120 6973 2073 6f72  k if Data is sor
-00003600: 7465 642e 0a20 2020 2020 2020 2023 2054  ted..        # T
-00003610: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
-00003620: 616e 206f 626a 6563 7420 6069 735f 736f  an object `is_so
-00003630: 7274 6564 6020 7468 6174 2063 6f6e 7461  rted` that conta
-00003640: 696e 7320 696e 666f 726d 6174 696f 6e0a  ins information.
-00003650: 2020 2020 2020 2020 2320 2020 312e 2073          #   1. s
-00003660: 7461 7475 7320 2d2d 2073 6f72 7465 6420  tatus -- sorted 
-00003670: 6f72 206e 6f74 0a20 2020 2020 2020 2023  or not.        #
-00003680: 2020 2032 2e20 6669 7273 745f 756e 736f     2. first_unso
-00003690: 7274 6564 202d 2d20 7468 6520 696e 6465  rted -- the inde
-000036a0: 7820 6f66 2074 6865 2066 6972 7374 2075  x of the first u
-000036b0: 6e73 6f72 7465 6420 656c 656d 656e 740a  nsorted element.
-000036c0: 2020 2020 2020 2020 6973 5f73 6f72 7465          is_sorte
-000036d0: 6420 3d20 6576 656e 7473 2e69 735f 736f  d = events.is_so
-000036e0: 7274 6564 286c 616d 6264 6120 653a 2065  rted(lambda e: e
-000036f0: 5b22 7374 6172 7454 696d 6573 7461 6d70  ["startTimestamp
-00003700: 225d 5b22 6570 6f63 6853 6563 6f6e 6422  "]["epochSecond"
-00003710: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
-00003720: 2020 2020 2320 596f 7520 6361 6e20 7573      # You can us
-00003730: 6520 7468 6973 206f 626a 6563 7420 6173  e this object as
-00003740: 2075 7375 616c 2062 6f6f 6c20 7661 7269   usual bool vari
-00003750: 6162 6c65 2e0a 2020 2020 2020 2020 6966  able..        if
-00003760: 2069 735f 736f 7274 6564 3a0a 2020 2020   is_sorted:.    
-00003770: 2020 2020 2020 2020 7072 696e 7428 2265          print("e
-00003780: 7665 6e74 7320 4461 7461 206f 626a 2069  vents Data obj i
-00003790: 7320 736f 7274 6564 2122 290a 2020 2020  s sorted!").    
-000037a0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
-000037b0: 312e 3134 5d20 5573 6520 6044 6174 612e  1.14] Use `Data.
-000037c0: 7368 6f77 2829 6020 746f 206c 6f6f 6b20  show()` to look 
-000037d0: 6174 2074 6865 2066 6972 7374 204e 206d  at the first N m
-000037e0: 6573 7361 6765 7320 696e 2074 6865 2073  essages in the s
-000037f0: 7472 6561 6d2e 0a20 2020 2020 2020 2064  tream..        d
-00003800: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
-00003810: 615f 6f62 6a5f 7669 615f 6164 642e 7368  a_obj_via_add.sh
-00003820: 6f77 286e 3d36 290a 2020 2020 2020 2020  ow(n=6).        
-00003830: 2320 5769 6c6c 2070 7269 6e74 0a20 2020  # Will print.   
-00003840: 2020 2020 2023 202d 2d2d 2d2d 2d2d 2d2d       # ---------
-00003850: 2d2d 2d2d 2050 7269 6e74 6564 2066 6972  ---- Printed fir
-00003860: 7374 2036 2072 6563 6f72 6473 202d 2d2d  st 6 records ---
-00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00003880: 2020 2023 205b 315d 202d 2d2d 2d2d 2d0a     # [1] ------.
-00003890: 2020 2020 2020 2020 2320 310a 2020 2020          # 1.    
-000038a0: 2020 2020 2320 5b32 5d20 2d2d 2d2d 2d2d      # [2] ------
-000038b0: 0a20 2020 2020 2020 2023 2032 0a20 2020  .        # 2.   
-000038c0: 2020 2020 2023 205b 335d 202d 2d2d 2d2d       # [3] -----
-000038d0: 2d0a 2020 2020 2020 2020 2320 330a 2020  -.        # 3.  
-000038e0: 2020 2020 2020 2320 5b34 5d20 2d2d 2d2d        # [4] ----
-000038f0: 2d2d 0a20 2020 2020 2020 2023 2027 6127  --.        # 'a'
-00003900: 0a20 2020 2020 2020 2023 205b 355d 202d  .        # [5] -
-00003910: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
-00003920: 7b27 6964 273a 2031 3233 7d0a 2020 2020  {'id': 123}.    
-00003930: 2020 2020 2320 5b36 5d20 2d2d 2d2d 2d2d      # [6] ------
-00003940: 0a20 2020 2020 2020 2023 2027 6327 0a20  .        # 'c'. 
-00003950: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003960: 2320 5b31 2e31 355d 2059 6f75 2063 616e  # [1.15] You can
-00003970: 2072 656d 6f76 6520 7468 6520 6361 6368   remove the cach
-00003980: 6520 6669 6c65 206f 6620 7468 6520 4461  e file of the Da
-00003990: 7461 206f 626a 6563 742c 2069 6620 7265  ta object, if re
-000039a0: 7175 6972 6564 2e0a 2020 2020 2020 2020  quired..        
-000039b0: 6461 7461 5f6f 626a 5f66 726f 6d5f 6361  data_obj_from_ca
-000039c0: 6368 652e 636c 6561 725f 6361 6368 6528  che.clear_cache(
-000039d0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000039e0: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-000039f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003a00: 2323 2323 2323 2323 230a 2020 2020 2020  #########.      
-00003a10: 2020 2320 5b32 5d20 576f 726b 696e 6720    # [2] Working 
-00003a20: 7769 7468 2063 6f6e 7665 7274 6572 732e  with converters.
-00003a30: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-00003a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003a50: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00003a60: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
-00003a70: 6172 6520 6375 7272 656e 746c 7920 7468  are currently th
-00003a80: 7265 6520 696d 706c 656d 656e 7461 7469  ree implementati
-00003a90: 6f6e 7320 6f66 2049 5469 6d65 7374 616d  ons of ITimestam
-00003aa0: 7043 6f6e 7665 7274 6572 2063 6c61 7373  pConverter class
-00003ab0: 3a20 4461 7465 7469 6d65 436f 6e76 6572  : DatetimeConver
-00003ac0: 7465 2c20 4461 7465 7469 6d65 5374 7269  te, DatetimeStri
-00003ad0: 6e67 436f 6e76 6572 7465 7220 616e 6420  ngConverter and 
-00003ae0: 5072 6f74 6f62 7566 5469 6d65 7374 616d  ProtobufTimestam
-00003af0: 7043 6f6e 7665 7274 6572 2e0a 2020 2020  pConverter..    
-00003b00: 2020 2020 2320 5468 6579 2061 6c6c 2069      # They all i
-00003b10: 6d70 6c65 6d65 6e74 2073 616d 6520 6d65  mplement same me
-00003b20: 7468 6f64 7320 6672 6f6d 2062 6173 6520  thods from base 
-00003b30: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
-00003b40: 204e 6f74 6520 7468 6174 2073 6f6d 6520   Note that some 
-00003b50: 6163 6375 7261 6379 206d 6179 2062 6520  accuracy may be 
-00003b60: 6c6f 7374 2064 7572 696e 6720 636f 6e76  lost during conv
-00003b70: 6572 7369 6f6e 2e0a 2020 2020 2020 2020  ersion..        
-00003b80: 2320 4966 2066 6f72 2065 7861 6d70 6c65  # If for example
-00003b90: 2079 6f75 2075 7365 2074 6f5f 6d69 6372   you use to_micr
-00003ba0: 6f73 6563 6f6e 6473 206e 616e 6f73 6563  oseconds nanosec
-00003bb0: 6f6e 6473 2077 696c 6c20 6265 2063 7574  onds will be cut
-00003bc0: 206f 6666 2069 6e73 7465 6164 206f 6620   off instead of 
-00003bd0: 726f 756e 6469 6e67 2e0a 2020 2020 2020  rounding..      
-00003be0: 2020 0a20 2020 2020 2020 2023 205b 322e    .        # [2.
-00003bf0: 315d 2044 6174 6574 696d 6543 6f6e 7665  1] DatetimeConve
-00003c00: 7274 6572 2e0a 2020 2020 2020 2020 2320  rter..        # 
-00003c10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
-00003c20: 7220 7461 6b65 7320 6461 7465 7469 6d65  r takes datetime
-00003c30: 2e64 6174 6574 696d 6520 6f62 6a65 6374  .datetime object
-00003c40: 2061 7320 696e 7075 742e 0a20 2020 2020   as input..     
-00003c50: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
-00003c60: 7469 6d65 5f6f 626a 203d 2064 6174 6574  time_obj = datet
-00003c70: 696d 6528 7965 6172 3d32 3032 332c 206d  ime(year=2023, m
-00003c80: 6f6e 7468 3d31 2c20 6461 793d 352c 2068  onth=1, day=5, h
-00003c90: 6f75 723d 3134 2c20 6d69 6e75 7465 3d33  our=14, minute=3
-00003ca0: 382c 2073 6563 6f6e 643d 3235 2c20 6d69  8, second=25, mi
-00003cb0: 6372 6f73 6563 6f6e 643d 3134 3630 290a  crosecond=1460).
-00003cc0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003cd0: 2023 2049 7420 6861 7320 6d65 7468 6f64   # It has method
-00003ce0: 7320 7468 6174 2072 6574 7572 6e20 7468  s that return th
-00003cf0: 6520 6461 7465 7469 6d65 2069 6e20 6469  e datetime in di
-00003d00: 6666 6572 656e 7420 666f 726d 6173 3a0a  fferent formas:.
-00003d10: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003d20: 2064 6174 655f 6d73 203d 2044 6174 6574   date_ms = Datet
-00003d30: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
-00003d40: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
-00003d50: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
-00003d60: 2020 2064 6174 655f 7573 203d 2044 6174     date_us = Dat
-00003d70: 6574 696d 6543 6f6e 7665 7274 6572 2e74  etimeConverter.t
-00003d80: 6f5f 6d69 6372 6f73 6563 6f6e 6473 2864  o_microseconds(d
-00003d90: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
-00003da0: 2020 2020 2023 2043 6f6e 7665 7274 696e       # Convertin
-00003db0: 6720 746f 206e 616e 6f73 6563 6f6e 6473  g to nanoseconds
-00003dc0: 206a 7573 7473 2061 6464 7320 7468 7265   justs adds thre
-00003dd0: 6520 7472 6169 6c69 6e67 207a 6572 6f73  e trailing zeros
-00003de0: 2061 7320 6461 7465 7469 6d65 206f 626a   as datetime obj
-00003df0: 6563 7420 646f 6573 6e27 7420 6861 7665  ect doesn't have
-00003e00: 206e 616e 6f73 6563 6f6e 6473 2e0a 2020   nanoseconds..  
-00003e10: 2020 2020 2020 6461 7465 5f6e 7320 3d20        date_ns = 
-00003e20: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
-00003e30: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
-00003e40: 2864 6174 6574 696d 655f 6f62 6a29 0a20  (datetime_obj). 
-00003e50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00003e60: 2320 5b32 2e32 5d20 4461 7465 7469 6d65  # [2.2] Datetime
-00003e70: 5374 7269 6e67 436f 6e76 6572 7465 720a  StringConverter.
-00003e80: 2020 2020 2020 2020 2320 4461 7465 7469          # Dateti
-00003e90: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003ea0: 7220 7461 6b65 7320 7374 7269 6e67 2069  r takes string i
-00003eb0: 6e20 2279 7979 792d 4d4d 2d64 6454 4848  n "yyyy-MM-ddTHH
-00003ec0: 3a6d 6d3a 7373 5b2e 5353 5353 5353 5353  :mm:ss[.SSSSSSSS
-00003ed0: 535d 5a22 2066 6f72 6d61 742e 0a20 2020  S]Z" format..   
-00003ee0: 2020 2020 200a 2020 2020 2020 2020 6461       .        da
-00003ef0: 7465 5f73 7472 696e 6720 3d20 2232 3032  te_string = "202
-00003f00: 332d 3031 2d30 3554 3134 3a33 383a 3235  3-01-05T14:38:25
-00003f10: 2e30 3031 3436 5a22 0a20 2020 2020 2020  .00146Z".       
-00003f20: 200a 2020 2020 2020 2020 2320 5765 2068   .        # We h
-00003f30: 6176 6520 7361 6d65 206d 6574 686f 6473  ave same methods
-00003f40: 2061 7320 696e 2044 6174 6574 696d 6543   as in DatetimeC
-00003f50: 6f6e 7665 7274 6572 0a20 2020 2020 2020  onverter.       
-00003f60: 2064 6174 655f 6d73 5f66 726f 6d5f 7374   date_ms_from_st
-00003f70: 7269 6e67 203d 2044 6174 6574 696d 6553  ring = DatetimeS
-00003f80: 7472 696e 6743 6f6e 7665 7274 6572 2e74  tringConverter.t
-00003f90: 6f5f 6d69 6c6c 6973 6563 6f6e 6473 2864  o_milliseconds(d
-00003fa0: 6174 655f 7374 7269 6e67 290a 2020 2020  ate_string).    
-00003fb0: 2020 2020 6461 7465 5f75 735f 6672 6f6d      date_us_from
-00003fc0: 5f73 7472 696e 6720 3d20 4461 7465 7469  _string = Dateti
-00003fd0: 6d65 5374 7269 6e67 436f 6e76 6572 7465  meStringConverte
-00003fe0: 722e 746f 5f6d 6963 726f 7365 636f 6e64  r.to_microsecond
-00003ff0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
-00004000: 2020 2020 2020 2064 6174 655f 6e73 5f66         date_ns_f
-00004010: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
-00004020: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
-00004030: 7274 6572 2e74 6f5f 6e61 6e6f 7365 636f  rter.to_nanoseco
-00004040: 6e64 7328 6461 7465 5f73 7472 696e 6729  nds(date_string)
-00004050: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004060: 2020 2320 5765 2063 616e 2061 6c73 6f20    # We can also 
-00004070: 6765 7420 6461 7465 7469 6d65 206f 626a  get datetime obj
-00004080: 6563 7420 6672 6f6d 2073 7472 696e 670a  ect from string.
-00004090: 2020 2020 2020 2020 6461 7465 7469 6d65          datetime
-000040a0: 5f66 726f 6d5f 7374 7269 6e67 203d 2044  _from_string = D
-000040b0: 6174 6574 696d 6553 7472 696e 6743 6f6e  atetimeStringCon
-000040c0: 7665 7274 6572 2e74 6f5f 6461 7465 7469  verter.to_dateti
-000040d0: 6d65 2864 6174 655f 7374 7269 6e67 290a  me(date_string).
-000040e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000040f0: 2023 205b 322e 335d 2050 726f 746f 6275   # [2.3] Protobu
-00004100: 6654 696d 6573 7461 6d70 436f 6e76 6572  fTimestampConver
-00004110: 7465 720a 2020 2020 2020 2020 2320 5072  ter.        # Pr
-00004120: 6f74 6f62 7566 2074 696d 6573 7461 6d70  otobuf timestamp
-00004130: 7320 6d75 7374 2062 6520 696e 2066 6f72  s must be in for
-00004140: 6d20 7b22 6570 6f63 6853 6563 6f6e 6422  m {"epochSecond"
-00004150: 3a20 7365 636f 6e64 732c 2022 6e61 6e6f  : seconds, "nano
-00004160: 223a 206e 616e 6f73 6563 6f6e 6473 7d0a  ": nanoseconds}.
-00004170: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004180: 2070 726f 746f 6275 665f 7469 6d65 7374   protobuf_timest
-00004190: 616d 7020 3d20 7b22 6570 6f63 6853 6563  amp = {"epochSec
-000041a0: 6f6e 6422 3a20 3136 3732 3932 3935 3035  ond": 1672929505
-000041b0: 2c20 226e 616e 6f22 3a20 315f 3436 305f  , "nano": 1_460_
-000041c0: 3030 307d 0a20 2020 2020 2020 200a 2020  000}.        .  
-000041d0: 2020 2020 2020 6461 7465 5f6d 735f 6672        date_ms_fr
-000041e0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-000041f0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004200: 436f 6e76 6572 7465 722e 746f 5f6d 696c  Converter.to_mil
-00004210: 6c69 7365 636f 6e64 7328 7072 6f74 6f62  liseconds(protob
-00004220: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
-00004230: 2020 2020 2020 6461 7465 5f75 735f 6672        date_us_fr
-00004240: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00004250: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004260: 436f 6e76 6572 7465 722e 746f 5f6d 6963  Converter.to_mic
-00004270: 726f 7365 636f 6e64 7328 7072 6f74 6f62  roseconds(protob
-00004280: 7566 5f74 696d 6573 7461 6d70 290a 2020  uf_timestamp).  
-00004290: 2020 2020 2020 6461 7465 5f6e 735f 6672        date_ns_fr
-000042a0: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-000042b0: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-000042c0: 436f 6e76 6572 7465 722e 746f 5f6e 616e  Converter.to_nan
-000042d0: 6f73 6563 6f6e 6473 2870 726f 746f 6275  oseconds(protobu
-000042e0: 665f 7469 6d65 7374 616d 7029 0a20 2020  f_timestamp).   
-000042f0: 2020 2020 2064 6174 6574 696d 655f 6672       datetime_fr
-00004300: 6f6d 5f74 696d 6573 7461 6d70 203d 2050  om_timestamp = P
-00004310: 726f 746f 6275 6654 696d 6573 7461 6d70  rotobufTimestamp
-00004320: 436f 6e76 6572 7465 722e 746f 5f64 6174  Converter.to_dat
-00004330: 6574 696d 6528 7072 6f74 6f62 7566 5f74  etime(protobuf_t
-00004340: 696d 6573 7461 6d70 290a 2020 2020 2020  imestamp).      
-00004350: 2020 0a20 2020 2020 2020 2023 2323 2323    .        #####
-00004360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004380: 230a 2020 2020 2020 2020 2320 5b33 5d20  #.        # [3] 
-00004390: 576f 726b 696e 6720 7769 7468 2045 7665  Working with Eve
-000043a0: 6e74 5472 6565 2061 6e64 2045 7665 6e74  ntTree and Event
-000043b0: 5472 6565 436f 6c6c 6563 7469 6f6e 2e0a  TreeCollection..
-000043c0: 2020 2020 2020 2020 2323 2323 2323 2323          ########
-000043d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000043e0: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
-000043f0: 2020 2020 2020 2023 2043 616e 2062 6520         # Can be 
-00004400: 7573 6566 756c 2069 6620 796f 7520 6861  useful if you ha
-00004410: 7665 2064 6174 612d 7374 7265 616d 2077  ve data-stream w
-00004420: 6974 6820 3c20 3130 306b 2065 6c65 6d65  ith < 100k eleme
-00004430: 6e74 732c 206f 7468 6572 7769 7365 2069  nts, otherwise i
-00004440: 740a 2020 2020 2020 2020 2320 7461 6b65  t.        # take
-00004450: 7320 746f 6f20 6d75 6368 2052 414d 2e0a  s too much RAM..
-00004460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00004470: 2023 205b 332e 315d 2042 7569 6c64 2061   # [3.1] Build a
-00004480: 2063 7573 746f 6d20 4576 656e 7454 7265   custom EventTre
-00004490: 650a 2020 2020 2020 2020 2320 546f 2063  e.        # To c
-000044a0: 7265 6174 6520 616e 2045 7665 6e74 5472  reate an EventTr
-000044b0: 6565 206f 626a 6563 7420 796f 7520 6e65  ee object you ne
-000044c0: 6564 2074 6f20 7072 6f76 6964 6520 6e61  ed to provide na
-000044d0: 6d65 2c20 6964 2061 6e64 2064 6174 6120  me, id and data 
-000044e0: 6f66 2074 6865 2072 6f6f 7420 6576 656e  of the root even
-000044f0: 742e 0a20 2020 2020 2020 2074 7265 6520  t..        tree 
-00004500: 3d20 4576 656e 7454 7265 6528 6576 656e  = EventTree(even
-00004510: 745f 6e61 6d65 3d22 726f 6f74 2065 7665  t_name="root eve
-00004520: 6e74 222c 2065 7665 6e74 5f69 643d 2272  nt", event_id="r
-00004530: 6f6f 745f 6964 222c 2064 6174 613d 7b22  oot_id", data={"
-00004540: 6461 7461 223a 205b 312c 2032 2c20 332c  data": [1, 2, 3,
-00004550: 2034 2c20 355d 7d29 0a20 2020 2020 2020   4, 5]}).       
-00004560: 200a 2020 2020 2020 2020 2320 546f 2061   .        # To a
-00004570: 6464 206e 6577 206e 6f64 6520 7573 6520  dd new node use 
-00004580: 6170 7065 6e64 5f65 7665 6e74 2e20 7061  append_event. pa
-00004590: 7265 6e74 5f69 6420 6973 206e 6563 6573  rent_id is neces
-000045a0: 7361 7279 2c20 6461 7461 2069 7320 6f70  sary, data is op
-000045b0: 7469 6f6e 616c 2e0a 2020 2020 2020 2020  tional..        
-000045c0: 7472 6565 2e61 7070 656e 645f 6576 656e  tree.append_even
-000045d0: 7428 6576 656e 745f 6e61 6d65 3d22 4122  t(event_name="A"
-000045e0: 2c20 6576 656e 745f 6964 3d22 415f 6964  , event_id="A_id
-000045f0: 222c 2064 6174 613d 4e6f 6e65 2c20 7061  ", data=None, pa
-00004600: 7265 6e74 5f69 643d 2272 6f6f 745f 6964  rent_id="root_id
-00004610: 2229 0a20 2020 2020 2020 200a 2020 2020  ").        .    
-00004620: 2020 2020 2320 5b33 2e33 5d20 4275 696c      # [3.3] Buil
-00004630: 6469 6e67 2074 6865 2045 7665 6e74 5472  ding the EventTr
-00004640: 6565 436f 6c6c 6563 7469 6f6e 2e0a 2020  eeCollection..  
-00004650: 2020 2020 2020 6461 7461 5f73 6f75 7263        data_sourc
-00004660: 653a 2049 4461 7461 536f 7572 6365 2020  e: IDataSource  
-00004670: 2320 596f 7520 7368 6f75 6c64 2069 6e69  # You should ini
-00004680: 7420 4461 7461 536f 7572 6365 206f 626a  t DataSource obj
-00004690: 6563 742e 2045 2e67 2e20 6672 6f6d 204c  ect. E.g. from L
-000046a0: 7744 5020 6d6f 6475 6c65 2e0a 2020 2020  wDP module..    
-000046b0: 2020 2020 6461 7461 5f73 6f75 7263 6520      data_source 
-000046c0: 3d20 4475 6d6d 7944 6174 6153 6f75 7263  = DummyDataSourc
-000046d0: 6528 2920 2023 204e 6f74 6521 2057 6520  e()  # Note! We 
-000046e0: 7573 6520 6661 6b65 2044 5320 6865 7265  use fake DS here
-000046f0: 2e0a 2020 2020 2020 2020 2320 4554 4344  ..        # ETCD
-00004700: 7269 7665 7220 6865 7265 2069 7320 6120  river here is a 
-00004710: 7374 7562 2c20 6163 7475 616c 6c79 2074  stub, actually t
-00004720: 6865 206c 6962 2064 6f65 736e 2774 2068  he lib doesn't h
-00004730: 6176 6520 7375 6368 2061 2063 6c61 7373  ave such a class
-00004740: 2e0a 2020 2020 2020 2020 2320 596f 7520  ..        # You 
-00004750: 6361 6e20 7461 6b65 2069 7420 696e 204c  can take it in L
-00004760: 7744 5020 6d6f 6475 6c65 206f 7220 6372  wDP module or cr
-00004770: 6561 7465 2079 6f75 7273 656c 6620 636c  eate yourself cl
-00004780: 6173 7320 6966 2079 6f75 2068 6176 6520  ass if you have 
-00004790: 736f 6d65 2073 7065 6369 616c 2065 7665  some special eve
-000047a0: 6e74 7320 7374 7275 6374 7572 652e 0a20  nts structure.. 
-000047b0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
-000047c0: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
-000047d0: 7461 5f73 6f75 7263 652e 6c77 6470 2e65  ta_source.lwdp.e
-000047e0: 7665 6e74 5f74 7265 6520 696d 706f 7274  vent_tree import
-000047f0: 2048 7474 7045 5443 4472 6976 6572 2061   HttpETCDriver a
-00004800: 7320 4554 4344 7269 7665 720a 2020 2020  s ETCDriver.    
-00004810: 2020 2020 0a20 2020 2020 2020 2023 2049      .        # I
-00004820: 6620 796f 7520 646f 6e27 7420 7370 6563  f you don't spec
-00004830: 6966 7920 6461 7461 5f73 6f75 7263 6520  ify data_source 
-00004840: 666f 7220 7468 6520 6472 6976 6572 2074  for the driver t
-00004850: 6865 6e20 6974 2077 6f6e 2774 2072 6563  hen it won't rec
-00004860: 6f76 6572 2064 6574 6163 6865 6420 6576  over detached ev
-00004870: 656e 7473 2e0a 2020 2020 2020 2020 6472  ents..        dr
-00004880: 6976 6572 3a20 4945 5443 4472 6976 6572  iver: IETCDriver
-00004890: 2020 2320 596f 7520 7368 6f75 6c64 2069    # You should i
-000048a0: 6e69 7420 4554 4344 7269 7665 7220 6f62  nit ETCDriver ob
-000048b0: 6a65 6374 2e20 452e 672e 2066 726f 6d20  ject. E.g. from 
-000048c0: 4c77 4450 206d 6f64 756c 6520 6f72 2079  LwDP module or y
-000048d0: 6f75 7220 6375 7374 6f6d 2063 6c61 7373  our custom class
-000048e0: 2e0a 2020 2020 2020 2020 6472 6976 6572  ..        driver
-000048f0: 203d 2045 5443 4472 6976 6572 2864 6174   = ETCDriver(dat
-00004900: 615f 736f 7572 6365 3d64 6174 615f 736f  a_source=data_so
-00004910: 7572 6365 2c20 7573 655f 7374 7562 3d54  urce, use_stub=T
-00004920: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
-00004930: 2020 2020 2020 6574 6320 3d20 4576 656e        etc = Even
-00004940: 7454 7265 6543 6f6c 6c65 6374 696f 6e28  tTreeCollection(
-00004950: 6472 6976 6572 290a 2020 2020 2020 2020  driver).        
-00004960: 6574 632e 6275 696c 6428 6576 656e 7473  etc.build(events
-00004970: 290a 2020 2020 2020 2020 6574 632e 7368  ).        etc.sh
-00004980: 6f77 2829 0a20 2020 2020 2020 2023 2049  ow().        # I
-00004990: 7427 6c6c 2070 7269 6e74 2074 6865 2066  t'll print the f
-000049a0: 6f6c 6c6f 7769 6e67 3a0a 2020 2020 2020  ollowing:.      
-000049b0: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
-000049c0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
-000049d0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
-000049e0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
-000049f0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
-00004a00: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
-00004a10: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
-00004a20: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
-00004a30: 0a20 2020 2020 2020 2070 7269 6e74 2865  .        print(e
-00004a40: 7463 290a 2020 2020 2020 2020 2320 4576  tc).        # Ev
-00004a50: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00004a60: 6e28 7472 6565 733d 312c 2065 7665 6e74  n(trees=1, event
-00004a70: 733d 335b 7472 6565 733d 332c 2064 6574  s=3[trees=3, det
-00004a80: 6163 6865 643d 305d 290a 2020 2020 2020  ached=0]).      
-00004a90: 2020 0a20 2020 2020 2020 2023 2044 6574    .        # Det
-00004aa0: 6163 6865 6420 6576 656e 7473 2069 736e  ached events isn
-00004ab0: 2774 2065 6d70 7479 2e0a 2020 2020 2020  't empty..      
-00004ac0: 2020 6173 7365 7274 2065 7463 2e67 6574    assert etc.get
-00004ad0: 5f64 6574 6163 6865 645f 6576 656e 7473  _detached_events
-00004ae0: 2829 2020 2320 7265 7475 726e 7320 6c69  ()  # returns li
-00004af0: 7374 206f 6620 6465 7461 6368 6564 5f65  st of detached_e
-00004b00: 7665 6e74 732e 0a20 2020 2020 2020 200a  vents..        .
-00004b10: 2020 2020 2020 2020 2320 7265 636f 7665          # recove
-00004b20: 725f 756e 6b6e 6f77 6e5f 6576 656e 7473  r_unknown_events
-00004b30: 202d 2d20 7573 6564 2074 6f20 7265 636f   -- used to reco
-00004b40: 7665 7220 736f 6d65 2065 7665 6e74 7320  ver some events 
-00004b50: 7061 7265 6e74 732e 0a20 2020 2020 2020  parents..       
-00004b60: 2023 2054 6861 7420 776f 6e27 7420 776f   # That won't wo
-00004b70: 726b 2077 6974 6820 4475 6d6d 7944 6174  rk with DummyDat
-00004b80: 6153 6f75 7263 652c 2073 6f20 7761 7320  aSource, so was 
-00004b90: 636f 6d6d 656e 7465 640a 2020 2020 2020  commented.      
-00004ba0: 2020 2320 6574 632e 7265 636f 7665 725f    # etc.recover_
-00004bb0: 756e 6b6e 6f77 6e5f 6576 656e 7473 2829  unknown_events()
-00004bc0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00004bd0: 2020 2320 4166 7465 7220 7468 6174 2074    # After that t
-00004be0: 6865 2064 6574 6163 6865 6420 6576 656e  he detached even
-00004bf0: 7473 2073 686f 756c 6420 6265 2065 6d70  ts should be emp
-00004c00: 7479 2062 6563 6175 7365 2074 6865 7920  ty because they 
-00004c10: 7765 7265 2072 6563 6f76 6572 6564 2e0a  were recovered..
-00004c20: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
-00004c30: 206e 6f74 2065 7463 2e67 6574 5f64 6574   not etc.get_det
-00004c40: 6163 6865 645f 6576 656e 7473 2829 0a20  ached_events(). 
-00004c50: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004c60: 2320 2d2d 2d2d 2d0a 2020 2020 2020 2020  # -----.        
-00004c70: 0a20 2020 2020 2020 2023 2054 6865 2063  .        # The c
-00004c80: 6f6c 6c65 6374 696f 6e20 6861 7320 4576  ollection has Ev
-00004c90: 656e 7454 7265 6573 2065 6163 6820 7769  entTrees each wi
-00004ca0: 7468 2061 2074 7265 6520 6f66 2065 7665  th a tree of eve
-00004cb0: 6e74 732e 0a20 2020 2020 2020 2023 2055  nts..        # U
-00004cc0: 7369 6e67 2043 6f6c 6c65 6374 696f 6e20  sing Collection 
-00004cd0: 616e 6420 4576 656e 7454 7265 6573 2c20  and EventTrees, 
-00004ce0: 796f 7520 6361 6e20 776f 726b 2066 6c65  you can work fle
-00004cf0: 7869 626c 7920 7769 7468 2065 7665 6e74  xibly with event
-00004d00: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00004d10: 2020 2020 2320 5b33 2e33 2e31 5d20 4765      # [3.3.1] Ge
-00004d20: 7420 6c65 6176 6573 206f 6620 616c 6c20  t leaves of all 
-00004d30: 7472 6565 732e 0a20 2020 2020 2020 206c  trees..        l
-00004d40: 6561 7665 733a 2054 7570 6c65 5b64 6963  eaves: Tuple[dic
-00004d50: 745d 203d 2065 7463 2e67 6574 5f6c 6561  t] = etc.get_lea
-00004d60: 7665 7328 2920 2023 2052 6574 7572 6e73  ves()  # Returns
-00004d70: 2061 2074 7570 6c65 206f 6620 6c65 6176   a tuple of leav
-00004d80: 6573 2065 7665 6e74 730a 2020 2020 2020  es events.      
-00004d90: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
-00004da0: 332e 325d 2047 6574 2072 6f6f 7473 2069  3.2] Get roots i
-00004db0: 6473 206f 6620 616c 6c20 7472 6565 732e  ds of all trees.
-00004dc0: 0a20 2020 2020 2020 2072 6f6f 7473 3a20  .        roots: 
-00004dd0: 4c69 7374 5b73 7472 5d20 3d20 6574 632e  List[str] = etc.
-00004de0: 6765 745f 726f 6f74 735f 6964 7328 290a  get_roots_ids().
-00004df0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00004e00: 7320 7468 6520 6c69 7374 206f 6620 726f  s the list of ro
-00004e10: 6f74 2049 6473 3a0a 2020 2020 2020 2020  ot Ids:.        
-00004e20: 2320 5b27 6465 6d6f 5f62 6f6f 6b5f 313a  # ['demo_book_1:
-00004e30: 7468 322d 7363 6f70 653a 3230 3233 3031  th2-scope:202301
-00004e40: 3035 3133 3537 3035 3536 3038 3733 3030  0513570556087300
-00004e50: 303a 6436 3165 3933 3061 2d38 6430 302d  0:d61e930a-8d00-
-00004e60: 3131 6564 2d61 6131 612d 6433 3461 3631  11ed-aa1a-d34a61
-00004e70: 3535 3135 3264 5f31 275d 0a20 2020 2020  55152d_1'].     
-00004e80: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00004e90: 2e33 2e33 5d20 4669 6e64 2061 6e20 6576  .3.3] Find an ev
-00004ea0: 656e 7420 696e 2061 6c6c 2074 7265 6573  ent in all trees
-00004eb0: 2e0a 2020 2020 2020 2020 6669 6e64 5f65  ..        find_e
-00004ec0: 7665 6e74 3a20 4f70 7469 6f6e 616c 5b64  vent: Optional[d
-00004ed0: 6963 745d 203d 2065 7463 2e66 696e 6428  ict] = etc.find(
-00004ee0: 6c61 6d62 6461 2065 7665 6e74 3a20 2253  lambda event: "S
-00004ef0: 656e 6420 6d65 7373 6167 6522 2069 6e20  end message" in 
-00004f00: 6576 656e 745b 2265 7665 6e74 5479 7065  event["eventType
-00004f10: 225d 290a 2020 2020 2020 2020 0a20 2020  "]).        .   
-00004f20: 2020 2020 2023 205b 332e 332e 345d 2046       # [3.3.4] F
-00004f30: 696e 6420 616c 6c20 6576 656e 7473 2069  ind all events i
-00004f40: 6e20 616c 6c20 7472 6565 732e 2054 6865  n all trees. The
-00004f50: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
-00004f60: 626c 6520 7665 7273 696f 6e20 2766 696e  ble version 'fin
-00004f70: 6461 6c6c 5f69 7465 7227 2e0a 2020 2020  dall_iter'..    
-00004f80: 2020 2020 6669 6e64 5f65 7665 6e74 733a      find_events:
-00004f90: 204c 6973 745b 6469 6374 5d20 3d20 6574   List[dict] = et
-00004fa0: 632e 6669 6e64 616c 6c28 6c61 6d62 6461  c.findall(lambda
-00004fb0: 2065 7665 6e74 3a20 6576 656e 745b 2273   event: event["s
-00004fc0: 7563 6365 7373 6675 6c22 5d20 6973 2054  uccessful"] is T
-00004fd0: 7275 6529 0a20 2020 2020 2020 200a 2020  rue).        .  
-00004fe0: 2020 2020 2020 2320 5b33 2e33 2e35 5d20        # [3.3.5] 
-00004ff0: 4669 6e64 2061 6e20 616e 6365 7374 6f72  Find an ancestor
-00005000: 206f 6620 7468 6520 6576 656e 742e 0a20   of the event.. 
-00005010: 2020 2020 2020 2061 6e63 6573 746f 723a         ancestor:
-00005020: 204f 7074 696f 6e61 6c5b 6469 6374 5d20   Optional[dict] 
-00005030: 3d20 6574 632e 6669 6e64 5f61 6e63 6573  = etc.find_ances
-00005040: 746f 7228 0a20 2020 2020 2020 2020 2020  tor(.           
-00005050: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
-00005060: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
-00005070: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
-00005080: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
-00005090: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
-000050a0: 3135 3264 5f31 222c 0a20 2020 2020 2020  152d_1",.       
-000050b0: 2020 2020 2066 696c 7465 723d 6c61 6d62       filter=lamb
-000050c0: 6461 2065 7665 6e74 3a20 2252 6f6f 7445  da event: "RootE
-000050d0: 7665 6e74 2220 696e 2065 7665 6e74 5b22  vent" in event["
-000050e0: 6576 656e 744e 616d 6522 5d2c 0a20 2020  eventName"],.   
-000050f0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-00005100: 2020 2020 2020 2020 2320 5b33 2e33 2e36          # [3.3.6
-00005110: 5d20 4765 7420 6368 696c 6472 656e 206f  ] Get children o
-00005120: 6620 7468 6520 6576 656e 742e 2054 6865  f the event. The
-00005130: 7265 2069 7320 616c 736f 2069 7465 7261  re is also itera
-00005140: 626c 6520 7665 7273 696f 6e20 2767 6574  ble version 'get
-00005150: 5f63 6869 6c64 7265 6e5f 6974 6572 272e  _children_iter'.
-00005160: 0a20 2020 2020 2020 2063 6869 6c64 7265  .        childre
-00005170: 6e3a 2054 7570 6c65 5b64 6963 745d 203d  n: Tuple[dict] =
-00005180: 2065 7463 2e67 6574 5f63 6869 6c64 7265   etc.get_childre
-00005190: 6e28 0a20 2020 2020 2020 2020 2020 2022  n(.            "
-000051a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
-000051b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
-000051c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
-000051d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
-000051e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
-000051f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
-00005200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00005210: 2023 205b 332e 332e 375d 2047 6574 2073   # [3.3.7] Get s
-00005220: 7562 7472 6565 2066 6f72 2073 7065 6369  ubtree for speci
-00005230: 6669 6564 2065 7665 6e74 2e0a 2020 2020  fied event..    
-00005240: 2020 2020 7375 6274 7265 653a 2045 7665      subtree: Eve
-00005250: 6e74 5472 6565 203d 2065 7463 2e67 6574  ntTree = etc.get
-00005260: 5f73 7562 7472 6565 280a 2020 2020 2020  _subtree(.      
-00005270: 2020 2020 2020 2264 656d 6f5f 626f 6f6b        "demo_book
-00005280: 5f31 3a74 6832 2d73 636f 7065 3a32 3032  _1:th2-scope:202
-00005290: 3330 3130 3531 3335 3730 3535 3630 3837  3010513570556087
-000052a0: 3330 3030 3a64 3631 6539 3330 612d 3864  3000:d61e930a-8d
-000052b0: 3030 2d31 3165 642d 6161 3161 2d64 3334  00-11ed-aa1a-d34
-000052c0: 6136 3135 3531 3532 645f 3122 0a20 2020  a6155152d_1".   
-000052d0: 2020 2020 2029 0a20 2020 2020 2020 200a       ).        .
-000052e0: 2020 2020 2020 2020 2320 5b33 2e33 2e38          # [3.3.8
-000052f0: 5d20 4765 7420 6675 6c6c 2070 6174 6820  ] Get full path 
-00005300: 746f 2074 6865 2065 7665 6e74 2e0a 2020  to the event..  
-00005310: 2020 2020 2020 2320 4c6f 6f6b 7320 6c69        # Looks li
-00005320: 6b65 205b 616e 6365 7374 6f72 5f72 6f6f  ke [ancestor_roo
-00005330: 742c 2061 6e63 6573 746f 725f 6c65 7665  t, ancestor_leve
-00005340: 6c31 2c20 616e 6365 7374 6f72 5f6c 6576  l1, ancestor_lev
-00005350: 656c 322c 2065 7665 6e74 5d0a 2020 2020  el2, event].    
-00005360: 2020 2020 6576 656e 745f 7061 7468 3a20      event_path: 
-00005370: 4c69 7374 5b64 6963 745d 203d 2065 7463  List[dict] = etc
-00005380: 2e67 6574 5f66 756c 6c5f 7061 7468 280a  .get_full_path(.
-00005390: 2020 2020 2020 2020 2020 2020 2264 656d              "dem
-000053a0: 6f5f 626f 6f6b 5f31 3a74 6832 2d73 636f  o_book_1:th2-sco
-000053b0: 7065 3a32 3032 3330 3130 3531 3335 3730  pe:2023010513570
-000053c0: 3535 3630 3837 3330 3030 3a64 3631 6539  5560873000:d61e9
-000053d0: 3330 612d 3864 3030 2d31 3165 642d 6161  30a-8d00-11ed-aa
-000053e0: 3161 2d64 3334 6136 3135 3531 3532 645f  1a-d34a6155152d_
-000053f0: 3122 0a20 2020 2020 2020 2029 0a20 2020  1".        ).   
-00005400: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00005410: 5b33 2e33 2e39 5d20 4765 7420 7061 7265  [3.3.9] Get pare
-00005420: 6e74 206f 6620 7468 6520 6576 656e 742e  nt of the event.
-00005430: 0a20 2020 2020 2020 2070 6172 656e 7420  .        parent 
-00005440: 3d20 6574 632e 6765 745f 7061 7265 6e74  = etc.get_parent
-00005450: 280a 2020 2020 2020 2020 2020 2020 2264  (.            "d
-00005460: 656d 6f5f 626f 6f6b 5f31 3a74 6832 2d73  emo_book_1:th2-s
-00005470: 636f 7065 3a32 3032 3330 3130 3531 3335  cope:20230105135
-00005480: 3730 3535 3630 3837 3330 3030 3a64 3631  705560873000:d61
-00005490: 6539 3330 612d 3864 3030 2d31 3165 642d  e930a-8d00-11ed-
-000054a0: 6161 3161 2d64 3334 6136 3135 3531 3532  aa1a-d34a6155152
-000054b0: 645f 3122 0a20 2020 2020 2020 2029 0a20  d_1".        ). 
-000054c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000054d0: 2320 5b33 2e33 2e31 305d 2041 7070 656e  # [3.3.10] Appen
-000054e0: 6420 6e65 7720 6576 656e 7420 746f 2074  d new event to t
-000054f0: 6865 2063 6f6c 6c65 6374 696f 6e2e 0a20  he collection.. 
-00005500: 2020 2020 2020 2065 7463 2e61 7070 656e         etc.appen
-00005510: 645f 6576 656e 7428 0a20 2020 2020 2020  d_event(.       
-00005520: 2020 2020 2065 7665 6e74 3d7b 0a20 2020       event={.   
-00005530: 2020 2020 2020 2020 2020 2020 2022 6576               "ev
-00005540: 656e 7449 6422 3a20 2261 3230 6635 6566  entId": "a20f5ef
-00005550: 342d 6333 6665 2d62 6231 302d 6132 3963  4-c3fe-bb10-a29c
-00005560: 2d64 6433 6437 3834 3930 3965 6222 2c0a  -dd3d784909eb",.
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2270 6172 656e 7445 7665 6e74 4964 223a  "parentEventId":
-00005590: 2022 3865 3235 3234 6661 2d63 6635 392d   "8e2524fa-cf59-
-000055a0: 3131 6562 2d61 3366 372d 3039 3466 3930  11eb-a3f7-094f90
-000055b0: 3463 3361 3632 222c 0a20 2020 2020 2020  4c3a62",.       
-000055c0: 2020 2020 2020 2020 2022 6576 656e 744e           "eventN
-000055d0: 616d 6522 3a20 2253 7475 6245 7665 6e74  ame": "StubEvent
-000055e0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
-000055f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005600: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
-00005610: 2e33 2e31 315d 2053 686f 7720 7468 6520  .3.11] Show the 
-00005620: 656e 7469 7265 2063 6f6c 6c65 6374 696f  entire collectio
-00005630: 6e2e 0a20 2020 2020 2020 2065 7463 2e73  n..        etc.s
-00005640: 686f 7728 290a 2020 2020 2020 2020 2320  how().        # 
-00005650: 4974 276c 6c20 7072 696e 7420 7468 6520  It'll print the 
-00005660: 666f 6c6c 6f77 696e 673a 0a20 2020 2020  following:.     
-00005670: 2020 2023 2053 6574 206f 6620 6175 746f     # Set of auto
-00005680: 2d67 656e 6572 6174 6564 2065 7665 6e74  -generated event
-00005690: 7320 666f 7220 6473 206c 6962 2074 6573  s for ds lib tes
-000056a0: 7469 6e67 0a20 2020 2020 2020 2023 20e2  ting.        # .
-000056b0: 949c e294 80e2 9480 2050 6c61 696e 2065  ........ Plain e
-000056c0: 7665 6e74 2031 0a20 2020 2020 2020 2023  vent 1.        #
-000056d0: 20e2 9494 e294 80e2 9480 2050 6c61 696e   ......... Plain
-000056e0: 2065 7665 6e74 2032 0a20 2020 2020 2020   event 2.       
-000056f0: 200a 2020 2020 2020 2020 2320 4173 2079   .        # As y
-00005700: 6f75 2063 616e 2073 6565 2c20 6e6f 7468  ou can see, noth
-00005710: 696e 6720 7761 7320 6368 616e 6765 642c  ing was changed,
-00005720: 2062 7574 2077 6520 6164 6465 6420 7468   but we added th
-00005730: 6520 6e65 7720 6576 656e 7421 0a20 2020  e new event!.   
-00005740: 2020 2020 2023 206c 6574 2773 206c 6f6f       # let's loo
-00005750: 6b20 6174 2074 6865 2073 756d 6d61 7279  k at the summary
-00005760: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00005770: 2020 2070 7269 6e74 2865 7463 2e73 756d     print(etc.sum
-00005780: 6d61 7279 2829 2920 2023 2074 6865 2073  mary())  # the s
-00005790: 616d 6520 6173 206a 7573 7420 7072 696e  ame as just prin
-000057a0: 7428 6574 6329 0a20 2020 2020 2020 2023  t(etc).        #
-000057b0: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
-000057c0: 7469 6f6e 2874 7265 6573 3d31 2c20 6576  tion(trees=1, ev
-000057d0: 656e 7473 3d35 5b74 7265 6573 3d33 2c20  ents=5[trees=3, 
-000057e0: 6465 7461 6368 6564 3d32 5d29 0a20 2020  detached=2]).   
-000057f0: 2020 2020 2023 2059 6f75 2063 616e 2073       # You can s
-00005800: 6565 2074 6861 7420 6974 2077 6173 2061  ee that it was a
-00005810: 6464 6564 2074 6f20 6465 7461 6368 6564  dded to detached
-00005820: 2e20 5468 6174 2773 2077 6879 2079 6f75  . That's why you
-00005830: 2064 6f6e 2774 2073 6565 2074 6865 2065   don't see the e
-00005840: 7665 6e74 0a20 2020 2020 2020 2023 2076  vent.        # v
-00005850: 6961 2060 7368 6f77 2829 602e 2060 7368  ia `show()`. `sh
-00005860: 6f77 2829 6020 7072 696e 7473 206f 6e6c  ow()` prints onl
-00005870: 7920 5472 6565 7321 0a20 2020 2020 2020  y Trees!.       
-00005880: 2023 2055 7365 2060 6574 632e 6765 745f   # Use `etc.get_
-00005890: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-000058a0: 2829 6020 746f 2063 6f6e 7665 7274 2064  ()` to convert d
-000058b0: 6574 6163 6865 6420 6576 656e 7473 2074  etached events t
-000058c0: 6f20 7472 6565 732e 0a20 2020 2020 2020  o trees..       
-000058d0: 2023 204d 6f72 6520 696e 666f 726d 6174   # More informat
-000058e0: 696f 6e20 6265 6c6f 7720 696e 2074 6865  ion below in the
-000058f0: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
-00005900: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-00005910: 0a20 2020 2020 2020 2023 202d 2d2d 2d2d  .        # -----
-00005920: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00005930: 2020 2320 5b33 2e34 5d20 576f 726b 696e    # [3.4] Workin
-00005940: 6720 7769 7468 2074 6865 2045 7665 6e74  g with the Event
-00005950: 5472 6565 2e0a 2020 2020 2020 2020 2320  Tree..        # 
-00005960: 4576 656e 7454 7265 6520 6861 7320 7468  EventTree has th
-00005970: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
-00005980: 7320 4576 656e 7454 7265 6543 6f6c 6c65  s EventTreeColle
-00005990: 6374 696f 6e2c 2062 7574 206f 6e6c 7920  ction, but only 
-000059a0: 666f 7220 6974 7320 6f77 6e20 7472 6565  for its own tree
-000059b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000059c0: 2020 2023 205b 332e 342e 315d 2047 6574     # [3.4.1] Get
-000059d0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-000059e0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
-000059f0: 7472 6565 733a 204c 6973 745b 4576 656e  trees: List[Even
-00005a00: 7454 7265 655d 203d 2065 7463 2e67 6574  tTree] = etc.get
-00005a10: 5f74 7265 6573 2829 0a20 2020 2020 2020  _trees().       
-00005a20: 2074 7265 653a 2045 7665 6e74 5472 6565   tree: EventTree
-00005a30: 203d 2074 7265 6573 5b30 5d0a 2020 2020   = trees[0].    
-00005a40: 2020 2020 0a20 2020 2020 2020 2023 2042      .        # B
-00005a50: 7574 2045 7665 6e74 5472 6565 2070 726f  ut EventTree pro
-00005a60: 7669 6465 7320 6120 776f 726b 2077 6974  vides a work wit
-00005a70: 6820 7468 6520 7472 6565 2c20 6275 7420  h the tree, but 
-00005a80: 646f 6573 206e 6f74 206d 6f64 6966 7920  does not modify 
-00005a90: 6974 2e0a 2020 2020 2020 2020 2320 4966  it..        # If
-00005aa0: 2079 6f75 2077 616e 7420 746f 206d 6f64   you want to mod
-00005ab0: 6966 7920 7468 6520 7472 6565 2c20 7573  ify the tree, us
-00005ac0: 6520 4576 656e 7454 7265 6543 6f6c 6c65  e EventTreeColle
-00005ad0: 6374 696f 6e73 2e0a 2020 2020 2020 2020  ctions..        
-00005ae0: 0a20 2020 2020 2020 2023 205b 332e 355d  .        # [3.5]
-00005af0: 2057 6f72 6b69 6e67 2077 6974 6820 5061   Working with Pa
-00005b00: 7265 6e74 6c65 7373 5472 6565 2e0a 2020  rentlessTree..  
-00005b10: 2020 2020 2020 2320 5061 7265 6e74 6c65        # Parentle
-00005b20: 7373 5472 6565 2069 7320 616e 2045 7665  ssTree is an Eve
-00005b30: 6e74 5472 6565 2074 6861 7420 6861 7320  ntTree that has 
-00005b40: 6465 7461 6368 6564 2065 7665 6e74 7320  detached events 
-00005b50: 7769 7468 2073 7475 6273 2e0a 2020 2020  with stubs..    
-00005b60: 2020 2020 7061 7265 6e74 6c65 7373 5f74      parentless_t
-00005b70: 7265 6573 3a20 4c69 7374 5b45 7665 6e74  rees: List[Event
-00005b80: 5472 6565 5d20 3d20 6574 632e 6765 745f  Tree] = etc.get_
-00005b90: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00005ba0: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
-00005bb0: 2822 7061 7265 6e74 6c65 7373 5f74 7265  ("parentless_tre
-00005bc0: 6573 2063 6f6e 7461 696e 733a 2229 0a20  es contains:"). 
-00005bd0: 2020 2020 2020 2070 7269 6e74 2870 6172         print(par
-00005be0: 656e 746c 6573 735f 7472 6565 7329 0a20  entless_trees). 
-00005bf0: 2020 2020 2020 2023 205b 4576 656e 7454         # [EventT
-00005c00: 7265 6528 6e61 6d65 3d27 3c42 726f 6b65  ree(name='<Broke
-00005c10: 6e45 7665 6e74 3e27 2c20 726f 6f74 5f69  nEvent>', root_i
-00005c20: 643d 276e 6f74 5f65 7869 7374 735f 696e  d='not_exists_in
-00005c30: 5f74 6865 5f65 7665 6e74 735f 7374 7265  _the_events_stre
-00005c40: 616d 272c 2065 7665 6e74 733d 3229 2c0a  am', events=2),.
-00005c50: 2020 2020 2020 2020 2320 2045 7665 6e74          #  Event
-00005c60: 5472 6565 286e 616d 653d 273c 4272 6f6b  Tree(name='<Brok
-00005c70: 656e 4576 656e 743e 272c 2072 6f6f 745f  enEvent>', root_
-00005c80: 6964 3d27 3865 3235 3234 6661 2d63 6635  id='8e2524fa-cf5
-00005c90: 392d 3131 6562 2d61 3366 372d 3039 3466  9-11eb-a3f7-094f
-00005ca0: 3930 3463 3361 3632 272c 2065 7665 6e74  904c3a62', event
-00005cb0: 733d 3229 5d0a 2020 2020 2020 2020 0a20  s=2)].        . 
-00005cc0: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
-00005cd0: 2220 2265 7463 2061 6674 6572 2060 6765  " "etc after `ge
-00005ce0: 745f 7061 7265 6e74 6c65 7373 5f74 7265  t_parentless_tre
-00005cf0: 6573 603a 2229 0a20 2020 2020 2020 2070  es`:").        p
-00005d00: 7269 6e74 2865 7463 2e73 756d 6d61 7279  rint(etc.summary
-00005d10: 2829 290a 2020 2020 2020 2020 2320 4576  ()).        # Ev
-00005d20: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-00005d30: 6e28 7472 6565 733d 335b 7265 6775 6c61  n(trees=3[regula
-00005d40: 723d 312c 2070 6172 656e 746c 6573 733d  r=1, parentless=
-00005d50: 325d 2c20 6576 656e 7473 3d37 5b74 7265  2], events=7[tre
-00005d60: 6573 3d37 2c20 6465 7461 6368 6564 3d30  es=7, detached=0
-00005d70: 5d29 270a 2020 2020 2020 2020 6574 632e  ])'.        etc.
-00005d80: 7368 6f77 2829 0a20 2020 2020 2020 2023  show().        #
-00005d90: 2053 6574 206f 6620 6175 746f 2d67 656e   Set of auto-gen
-00005da0: 6572 6174 6564 2065 7665 6e74 7320 666f  erated events fo
-00005db0: 7220 6473 206c 6962 2074 6573 7469 6e67  r ds lib testing
-00005dc0: 0a20 2020 2020 2020 2023 20e2 949c e294  .        # .....
-00005dd0: 80e2 9480 2050 6c61 696e 2065 7665 6e74  .... Plain event
-00005de0: 2031 0a20 2020 2020 2020 2023 20e2 9494   1.        # ...
-00005df0: e294 80e2 9480 2050 6c61 696e 2065 7665  ...... Plain eve
-00005e00: 6e74 2032 0a20 2020 2020 2020 2023 203c  nt 2.        # <
-00005e10: 4272 6f6b 656e 4576 656e 743e 0a20 2020  BrokenEvent>.   
-00005e20: 2020 2020 2023 20e2 9494 e294 80e2 9480       # .........
-00005e30: 2046 616b 6520 6576 656e 740a 2020 2020   Fake event.    
-00005e40: 2020 2020 2320 3c42 726f 6b65 6e45 7665      # <BrokenEve
-00005e50: 6e74 3e0a 2020 2020 2020 2020 2320 e294  nt>.        # ..
-00005e60: 94e2 9480 e294 8020 5374 7562 4576 656e  ....... StubEven
-00005e70: 7420 2020 203c 2d2d 2d20 7468 6520 6576  t    <--- the ev
-00005e80: 656e 7420 7468 6174 2077 6173 2061 6464  ent that was add
-00005e90: 6564 2061 626f 7665 0a20 2020 2020 2020  ed above.       
-00005ea0: 200a 2020 2020 2020 2020 2320 5b33 2e36   .        # [3.6
-00005eb0: 5d20 576f 726b 696e 6720 7769 7468 2050  ] Working with P
-00005ec0: 6172 656e 7445 7665 6e74 5472 6565 436f  arentEventTreeCo
-00005ed0: 6c6c 6563 7469 6f6e 2e0a 2020 2020 2020  llection..      
-00005ee0: 2020 2320 5061 7265 6e74 4576 656e 7454    # ParentEventT
-00005ef0: 7265 6543 6f6c 6c65 6374 696f 6e20 6973  reeCollection is
-00005f00: 2061 2074 7265 6520 636f 6c6c 6563 7469   a tree collecti
-00005f10: 6f6e 206c 696b 6520 4576 656e 7454 7265  on like EventTre
-00005f20: 6543 6f6c 6c65 6374 696f 6e2c 0a20 2020  eCollection,.   
-00005f30: 2020 2020 2023 2062 7574 2069 7420 6861       # but it ha
-00005f40: 7320 6f6e 6c79 2065 7665 6e74 7320 7468  s only events th
-00005f50: 6174 2068 6176 6520 7265 6665 7265 6e63  at have referenc
-00005f60: 6573 2e0a 2020 2020 2020 2020 6461 7461  es..        data
-00005f70: 5f73 6f75 7263 653a 2049 4461 7461 536f  _source: IDataSo
-00005f80: 7572 6365 2020 2320 596f 7520 7368 6f75  urce  # You shou
-00005f90: 6c64 2069 6e69 7420 4461 7461 536f 7572  ld init DataSour
-00005fa0: 6365 206f 626a 6563 742e 2045 2e67 2e20  ce object. E.g. 
-00005fb0: 6672 6f6d 204c 7744 5020 6d6f 6475 6c65  from LwDP module
-00005fc0: 2e0a 2020 2020 2020 2020 6461 7461 5f73  ..        data_s
-00005fd0: 6f75 7263 6520 3d20 4475 6d6d 7944 6174  ource = DummyDat
-00005fe0: 6153 6f75 7263 6528 2920 2023 204e 6f74  aSource()  # Not
-00005ff0: 6521 2057 6520 7573 6520 6661 6b65 2044  e! We use fake D
-00006000: 5320 6865 7265 2e0a 2020 2020 2020 2020  S here..        
-00006010: 2320 4554 4344 7269 7665 7220 6865 7265  # ETCDriver here
-00006020: 2069 7320 6120 7374 7562 2c20 6163 7475   is a stub, actu
-00006030: 616c 6c79 2074 6865 206c 6962 2064 6f65  ally the lib doe
-00006040: 736e 2774 2068 6176 6520 7375 6368 2061  sn't have such a
-00006050: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
-00006060: 2320 596f 7520 6361 6e20 7461 6b65 2069  # You can take i
-00006070: 7420 696e 204c 7744 5020 6d6f 6475 6c65  t in LwDP module
-00006080: 206f 7220 6372 6561 7465 2079 6f75 7273   or create yours
-00006090: 656c 6620 636c 6173 7320 6966 2079 6f75  elf class if you
-000060a0: 2068 6176 6520 736f 6d65 2073 7065 6369   have some speci
-000060b0: 616c 2065 7665 6e74 7320 7374 7275 6374  al events struct
-000060c0: 7572 652e 0a20 2020 2020 2020 2066 726f  ure..        fro
-000060d0: 6d20 7468 325f 6461 7461 5f73 6572 7669  m th2_data_servi
-000060e0: 6365 732e 6461 7461 5f73 6f75 7263 652e  ces.data_source.
-000060f0: 6c77 6470 2e65 7665 6e74 5f74 7265 6520  lwdp.event_tree 
-00006100: 696d 706f 7274 2048 7474 7045 5443 4472  import HttpETCDr
-00006110: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
-00006120: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
-00006130: 2020 2064 7269 7665 7220 3d20 4554 4344     driver = ETCD
-00006140: 7269 7665 7228 6461 7461 5f73 6f75 7263  river(data_sourc
-00006150: 653d 6461 7461 5f73 6f75 7263 6529 0a20  e=data_source). 
-00006160: 2020 2020 2020 2070 6574 6320 3d20 5061         petc = Pa
-00006170: 7265 6e74 4576 656e 7454 7265 6543 6f6c  rentEventTreeCol
-00006180: 6c65 6374 696f 6e28 6472 6976 6572 290a  lection(driver).
-00006190: 2020 2020 2020 2020 7065 7463 2e62 7569          petc.bui
-000061a0: 6c64 2865 7665 6e74 7329 0a20 2020 2020  ld(events).     
-000061b0: 2020 200a 2020 2020 2020 2020 7065 7463     .        petc
-000061c0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-000061d0: 7065 7463 2e73 756d 6d61 7279 2829 0a20  petc.summary(). 
-000061e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000061f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006210: 2323 2323 2323 0a20 2020 2020 2020 2023  ######.        #
-00006220: 205b 345d 2046 6965 6c64 2052 6573 6f6c   [4] Field Resol
-00006230: 7665 7273 0a20 2020 2020 2020 2023 2323  vers.        ###
-00006240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006260: 2323 230a 2020 2020 2020 2020 2320 506c  ###.        # Pl
-00006270: 6561 7365 2072 6561 6420 6046 6965 6c64  ease read `Field
-00006280: 2052 6573 6f6c 7665 7273 6020 626c 6f63   Resolvers` bloc
-00006290: 6b20 696e 2072 6561 646d 6520 6669 7273  k in readme firs
-000062a0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-000062b0: 2020 2020 2320 5b34 2e31 5d20 5573 6167      # [4.1] Usag
-000062c0: 6520 6578 616d 706c 6520 6672 6f6d 2063  e example from c
-000062d0: 6c69 656e 7420 636f 6465 0a20 2020 2020  lient code.     
-000062e0: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
-000062f0: 5f73 6572 7669 6365 732e 6461 7461 5f73  _services.data_s
-00006300: 6f75 7263 6520 696d 706f 7274 2028 0a20  ource import (. 
-00006310: 2020 2020 2020 2020 2020 206c 7764 702c             lwdp,
-00006320: 0a20 2020 2020 2020 2029 2020 2320 6c77  .        )  # lw
-00006330: 6470 2064 6174 615f 736f 7572 6365 2069  dp data_source i
-00006340: 6e69 7469 616c 697a 6520 7468 325f 6461  nitialize th2_da
-00006350: 7461 5f73 6572 7669 6365 732e 636f 6e66  ta_services.conf
-00006360: 6967 2064 7572 696e 6720 696d 706f 7274  ig during import
-00006370: 2e0a 2020 2020 2020 2020 6672 6f6d 2074  ..        from t
-00006380: 6832 5f64 6174 615f 7365 7276 6963 6573  h2_data_services
-00006390: 2e63 6f6e 6669 6720 696d 706f 7274 206f  .config import o
-000063a0: 7074 696f 6e73 2061 7320 6f5f 0a20 2020  ptions as o_.   
-000063b0: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
-000063c0: 7461 5f73 6572 7669 6365 732e 6461 7461  ta_services.data
-000063d0: 5f73 6f75 7263 652e 6c77 6470 2e73 7475  _source.lwdp.stu
-000063e0: 625f 6275 696c 6465 7220 696d 706f 7274  b_builder import
-000063f0: 2068 7474 705f 6d65 7373 6167 655f 7374   http_message_st
-00006400: 7562 5f62 7569 6c64 6572 0a20 2020 2020  ub_builder.     
-00006410: 2020 200a 2020 2020 2020 2020 6661 6b65     .        fake
-00006420: 5f64 6174 6120 3d20 5b0a 2020 2020 2020  _data = [.      
-00006430: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
-00006440: 6765 5f73 7475 625f 6275 696c 6465 722e  ge_stub_builder.
-00006450: 6275 696c 6428 7b22 6d65 7373 6167 6549  build({"messageI
-00006460: 6422 3a20 2261 222c 2022 6d65 7373 6167  d": "a", "messag
-00006470: 6554 7970 6522 3a20 2252 6f6f 7422 7d29  eType": "Root"})
-00006480: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
-00006490: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
-000064a0: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
-000064b0: 6d65 7373 6167 6549 6422 3a20 2262 222c  messageId": "b",
-000064c0: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
-000064d0: 224e 6577 227d 292c 0a20 2020 2020 2020  "New"}),.       
-000064e0: 2020 2020 2068 7474 705f 6d65 7373 6167       http_messag
-000064f0: 655f 7374 7562 5f62 7569 6c64 6572 2e62  e_stub_builder.b
-00006500: 7569 6c64 287b 226d 6573 7361 6765 4964  uild({"messageId
-00006510: 223a 2022 6322 2c20 226d 6573 7361 6765  ": "c", "message
-00006520: 5479 7065 223a 2022 416d 656e 6422 7d29  Type": "Amend"})
-00006530: 2c0a 2020 2020 2020 2020 2020 2020 6874  ,.            ht
-00006540: 7470 5f6d 6573 7361 6765 5f73 7475 625f  tp_message_stub_
-00006550: 6275 696c 6465 722e 6275 696c 6428 7b22  builder.build({"
-00006560: 6d65 7373 6167 6549 6422 3a20 2264 222c  messageId": "d",
-00006570: 2022 6d65 7373 6167 6554 7970 6522 3a20   "messageType": 
-00006580: 2243 616e 6365 6c22 7d29 2c0a 2020 2020  "Cancel"}),.    
-00006590: 2020 2020 5d0a 2020 2020 2020 2020 6661      ].        fa
-000065a0: 6b65 5f64 6174 615f 6f62 6a20 3d20 4461  ke_data_obj = Da
-000065b0: 7461 2866 616b 655f 6461 7461 290a 2020  ta(fake_data).  
-000065c0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
-000065d0: 6f72 206d 2069 6e20 6661 6b65 5f64 6174  or m in fake_dat
-000065e0: 615f 6f62 6a3a 0a20 2020 2020 2020 2020  a_obj:.         
-000065f0: 2020 206f 5f2e 6d66 722e 6578 7061 6e64     o_.mfr.expand
-00006600: 5f6d 6573 7361 6765 286d 2920 2023 206d  _message(m)  # m
-00006610: 6672 202d 2073 7461 6e64 7320 666f 7220  fr - stands for 
-00006620: 4d65 7373 6167 6546 6965 6c64 5265 736f  MessageFieldReso
-00006630: 6c76 6572 0a20 2020 2020 2020 2023 206f  lver.        # o
-00006640: 720a 2020 2020 2020 2020 666f 7220 6d20  r.        for m 
-00006650: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
-00006660: 2e6d 6170 286f 5f2e 6d66 722e 6578 7061  .map(o_.mfr.expa
-00006670: 6e64 5f6d 6573 7361 6765 293a 0a20 2020  nd_message):.   
-00006680: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
-00006690: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000066a0: 205b 342e 325d 204c 6962 7261 7269 6573   [4.2] Libraries
-000066b0: 2075 7361 6765 2e0a 2020 2020 2020 2020   usage..        
-000066c0: 2320 446f 6e27 7420 696d 706f 7274 2065  # Don't import e
-000066d0: 7861 6374 2072 6573 6f6c 7665 7273 2069  xact resolvers i
-000066e0: 6d70 6c65 6d65 6e74 6174 696f 6e20 696e  mplementation in
-000066f0: 2079 6f75 7220 636f 6465 2c20 706c 6561   your code, plea
-00006700: 7365 2e0a 2020 2020 2020 2020 2320 416c  se..        # Al
-00006710: 6c6f 7720 796f 7572 2063 6c69 656e 7420  low your client 
-00006720: 746f 2064 6f20 6974 2069 6e73 7465 6164  to do it instead
-00006730: 2e0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
-00006740: 2069 6d70 6f72 7420 606f 7074 696f 6e73   import `options
-00006750: 6020 6672 6f6d 2060 7468 325f 6461 7461  ` from `th2_data
-00006760: 5f73 6572 7669 6365 732e 636f 6e66 6967  _services.config
-00006770: 6020 616e 6420 7573 6520 6974 2e0a 2020  ` and use it..  
-00006780: 2020 2020 2020 6672 6f6d 2074 6832 5f64        from th2_d
-00006790: 6174 615f 7365 7276 6963 6573 2e63 6f6e  ata_services.con
-000067a0: 6669 6720 696d 706f 7274 206f 7074 696f  fig import optio
-000067b0: 6e73 2061 7320 6f5f 0a20 2020 2020 2020  ns as o_.       
-000067c0: 200a 2020 2020 2020 2020 666f 7220 6d20   .        for m 
-000067d0: 696e 2066 616b 655f 6461 7461 5f6f 626a  in fake_data_obj
-000067e0: 3a0a 2020 2020 2020 2020 2020 2020 6f5f  :.            o_
-000067f0: 2e6d 6672 2e65 7870 616e 645f 6d65 7373  .mfr.expand_mess
-00006800: 6167 6528 6d29 0a20 2020 2020 2020 2023  age(m).        #
-00006810: 206f 720a 2020 2020 2020 2020 666f 7220   or.        for 
-00006820: 6d20 696e 2066 616b 655f 6461 7461 5f6f  m in fake_data_o
-00006830: 626a 2e6d 6170 286f 5f2e 6d66 722e 6578  bj.map(o_.mfr.ex
-00006840: 7061 6e64 5f6d 6573 7361 6765 293a 0a20  pand_message):. 
-00006850: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00006860: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00006870: 2023 204d 6f72 6520 7465 6368 2064 6574   # More tech det
-00006880: 6169 6c73 3a0a 2020 2020 2020 2020 2320  ails:.        # 
-00006890: 2020 496e 2074 6869 7320 6361 7365 2c20    In this case, 
-000068a0: 7468 6572 6520 6973 206e 6f20 6c69 6e65  there is no line
-000068b0: 2060 6672 6f6d 2074 6832 5f64 6174 615f   `from th2_data_
-000068c0: 7365 7276 6963 6573 2e64 6174 615f 736f  services.data_so
-000068d0: 7572 6365 2069 6d70 6f72 7420 6c77 6470  urce import lwdp
-000068e0: 2060 0a20 2020 2020 2020 2023 2020 2062   `.        #   b
-000068f0: 6563 6175 7365 2077 6520 7368 6f75 6c64  ecause we should
-00006900: 206e 6f74 2063 686f 6f73 6520 666f 7220   not choose for 
-00006910: 7468 6520 7573 6572 2077 6869 6368 2061  the user which a
-00006920: 2064 6174 6120 736f 7572 6365 2074 6f20   data source to 
-00006930: 7573 652e 0a20 2020 2020 2020 2023 2020  use..        #  
-00006940: 2057 6520 646f 206e 6f74 206b 6e6f 7720   We do not know 
-00006950: 7768 6174 2068 6520 7769 6c6c 2063 686f  what he will cho
-00006960: 6f73 652c 2074 6865 7265 666f 7265 2c20  ose, therefore, 
-00006970: 7765 206d 7573 7420 7369 6d70 6c79 2061  we must simply a
-00006980: 6363 6573 730a 2020 2020 2020 2020 2320  ccess.        # 
-00006990: 2020 7468 6520 696e 7465 7266 6163 652c    the interface,
-000069a0: 2077 6869 6368 2077 696c 6c20 6265 2069   which will be i
-000069b0: 6e69 7469 616c 697a 6564 2062 7920 7468  nitialized by th
-000069c0: 6520 7573 6572 2e0a 2020 2020 2020 2020  e user..        
-000069d0: 0a20 2020 2020 2020 2023 2323 2323 2323  .        #######
-000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000069f0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00006a00: 2020 2020 2020 2020 2320 5b35 5d20 5573          # [5] Us
-00006a10: 696e 6720 7574 696c 6974 7920 6675 6e63  ing utility func
-00006a20: 7469 6f6e 732e 0a20 2020 2020 2020 2023  tions..        #
-00006a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a50: 2323 2323 230a 2020 2020 2020 2020 6672  #####.        fr
-00006a60: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00006a70: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
-00006a80: 5f75 7469 6c73 2e66 7265 7175 656e 6369  _utils.frequenci
-00006a90: 6573 2069 6d70 6f72 7420 6765 745f 6361  es import get_ca
-00006aa0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
-00006ab0: 6573 320a 2020 2020 2020 2020 6672 6f6d  es2.        from
-00006ac0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
-00006ad0: 6573 2e75 7469 6c73 2e65 7665 6e74 5f75  es.utils.event_u
-00006ae0: 7469 6c73 2e74 6f74 616c 7320 696d 706f  tils.totals impo
-00006af0: 7274 2067 6574 5f63 6174 6567 6f72 795f  rt get_category_
-00006b00: 746f 7461 6c73 320a 2020 2020 2020 2020  totals2.        
-00006b10: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
-00006b20: 7276 6963 6573 2e75 7469 6c73 2e63 6174  rvices.utils.cat
-00006b30: 6567 6f72 7920 696d 706f 7274 2043 6174  egory import Cat
-00006b40: 6567 6f72 790a 2020 2020 2020 2020 6672  egory.        fr
-00006b50: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
-00006b60: 6963 6573 2e75 7469 6c73 2e65 7665 6e74  ices.utils.event
-00006b70: 5f75 7469 6c73 2e65 7665 6e74 5f75 7469  _utils.event_uti
-00006b80: 6c73 2069 6d70 6f72 7420 6973 5f73 6f72  ls import is_sor
-00006b90: 7465 640a 2020 2020 2020 2020 0a20 2020  ted.        .   
-00006ba0: 2020 2020 2023 205b 352e 315d 2047 6574       # [5.1] Get
-00006bb0: 2074 6865 2071 7561 6e74 6974 6965 7320   the quantities 
-00006bc0: 6f66 2065 7665 6e74 7320 666f 7220 6469  of events for di
-00006bd0: 6666 6572 656e 7420 6361 7465 676f 7269  fferent categori
-00006be0: 6573 2e0a 2020 2020 2020 2020 6d65 7472  es..        metr
-00006bf0: 6963 7320 3d20 5b0a 2020 2020 2020 2020  ics = [.        
-00006c00: 2020 2020 4361 7465 676f 7279 2822 6461      Category("da
-00006c10: 7465 222c 206c 616d 6264 6120 6d3a 2054  te", lambda m: T
-00006c20: 6832 5469 6d65 7374 616d 7043 6f6e 7665  h2TimestampConve
-00006c30: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
-00006c40: 286d 5b22 7374 6172 7454 696d 6573 7461  (m["startTimesta
-00006c50: 6d70 225d 292e 6461 7465 2829 292c 0a20  mp"]).date()),. 
-00006c60: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
-00006c70: 6f72 7928 2273 7461 7475 7322 2c20 6c61  ory("status", la
-00006c80: 6d62 6461 206d 3a20 6d5b 2273 7563 6365  mbda m: m["succe
-00006c90: 7373 6675 6c22 5d29 2c0a 2020 2020 2020  ssful"]),.      
-00006ca0: 2020 5d0a 2020 2020 2020 2020 6361 7465    ].        cate
-00006cb0: 676f 7279 5f74 6f74 616c 7320 3d20 6765  gory_totals = ge
-00006cc0: 745f 6361 7465 676f 7279 5f74 6f74 616c  t_category_total
-00006cd0: 7332 2865 7665 6e74 732c 206d 6574 7269  s2(events, metri
-00006ce0: 6373 290a 2020 2020 2020 2020 7072 696e  cs).        prin
-00006cf0: 7428 6361 7465 676f 7279 5f74 6f74 616c  t(category_total
-00006d00: 7329 0a20 2020 2020 2020 2022 2222 0a20  s).        """. 
-00006d10: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
-00006d20: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
-00006d30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006d40: 2d2d 2b0a 2020 2020 2020 2020 7c20 2020  --+.        |   
-00006d50: 2020 2020 207c 2064 6174 6520 2020 2020       | date     
-00006d60: 2020 7c20 7374 6174 7573 2020 207c 2020    | status   |  
-00006d70: 2063 6f75 6e74 207c 0a20 2020 2020 2020   count |.       
-00006d80: 202b 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d   +========+=====
-00006d90: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00006da0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ==+=========+.  
-00006db0: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-00006dc0: 2032 3032 332d 3031 2d30 3520 7c20 5472   2023-01-05 | Tr
-00006dd0: 7565 2020 2020 207c 2020 2020 2020 2033  ue     |       3
-00006de0: 207c 0a20 2020 2020 2020 202b 2d2d 2d2d   |.        +----
-00006df0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00006e00: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  -+----------+---
-00006e10: 2d2d 2d2d 2d2d 2b0a 2020 2020 2020 2020  ------+.        
-00006e20: 7c20 2020 2020 2020 207c 2032 3032 332d  |        | 2023-
-00006e30: 3031 2d30 3520 7c20 4661 6c73 6520 2020  01-05 | False   
-00006e40: 207c 2020 2020 2020 2031 207c 0a20 2020   |       1 |.   
-00006e50: 2020 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d       +--------+-
-00006e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00006e70: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00006e80: 2b0a 2020 2020 2020 2020 7c20 636f 756e  +.        | coun
-00006e90: 7420 207c 2020 2020 2020 2020 2020 2020  t  |            
-00006ea0: 7c20 2020 2020 2020 2020 207c 2020 2020  |          |    
-00006eb0: 2020 2032 207c 0a20 2020 2020 2020 202b     2 |.        +
-00006ec0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006ed0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00006ee0: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
-00006ef0: 2020 2020 7c20 746f 7461 6c73 207c 2020      | totals |  
-00006f00: 2020 2020 2020 2020 2020 7c20 312f 3120            | 1/1 
-00006f10: 2020 2020 207c 2020 2020 2020 2034 207c       |       4 |
-00006f20: 0a20 2020 2020 2020 202b 2d2d 2d2d 2d2d  .        +------
-00006f30: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  --+------------+
-00006f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00006f50: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
-00006f60: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
-00006f70: 2020 2023 205b 352e 325d 2047 6574 2074     # [5.2] Get t
-00006f80: 6865 206e 756d 6265 7220 6f66 2065 7665  he number of eve
-00006f90: 6e74 7320 7769 7468 2073 7461 7475 7320  nts with status 
-00006fa0: 7375 6363 6573 7366 756c 2e0a 2020 2020  successful..    
-00006fb0: 2020 2020 6361 7465 676f 7279 203d 2043      category = C
-00006fc0: 6174 6567 6f72 7928 2273 7461 7475 7322  ategory("status"
-00006fd0: 2c20 6c61 6d62 6461 206d 3a20 6d5b 2273  , lambda m: m["s
-00006fe0: 7563 6365 7373 6675 6c22 5d29 0a20 2020  uccessful"]).   
-00006ff0: 2020 2020 2063 6174 6567 6f72 795f 6672       category_fr
-00007000: 6571 7565 6e63 6965 7320 3d20 6765 745f  equencies = get_
-00007010: 6361 7465 676f 7279 5f66 7265 7175 656e  category_frequen
-00007020: 6369 6573 3228 6576 656e 7473 2c20 6361  cies2(events, ca
-00007030: 7465 676f 7279 290a 2020 2020 2020 2020  tegory).        
-00007040: 7072 696e 7428 6361 7465 676f 7279 5f66  print(category_f
-00007050: 7265 7175 656e 6369 6573 290a 2020 2020  requencies).    
-00007060: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007070: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
-00007080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000070a0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-000070b0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
-000070c0: 2020 7c20 2020 2020 2020 207c 2074 696d    |        | tim
-000070d0: 6573 7461 6d70 5f73 7461 7274 2020 2020  estamp_start    
-000070e0: 207c 2074 696d 6573 7461 6d70 5f65 6e64   | timestamp_end
-000070f0: 2020 2020 2020 207c 2046 616c 7365 2020         | False  
-00007100: 207c 2020 2054 7275 6520 7c0a 2020 2020   |   True |.    
-00007110: 2020 2020 2b3d 3d3d 3d3d 3d3d 3d2b 3d3d      +========+==
-00007120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007130: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
-00007140: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
-00007150: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 2b0a 2020  ===+========+.  
-00007160: 2020 2020 2020 7c20 2020 2020 2020 207c        |        |
-00007170: 2032 3032 332d 3031 2d30 3554 3133 3a35   2023-01-05T13:5
-00007180: 373a 3035 207c 2032 3032 332d 3031 2d30  7:05 | 2023-01-0
-00007190: 3554 3133 3a35 373a 3036 207c 2030 2020  5T13:57:06 | 0  
-000071a0: 2020 2020 207c 2020 2020 2020 3320 7c0a       |      3 |.
-000071b0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
-000071c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-000071d0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000071e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000071f0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00007200: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
-00007210: 2020 207c 2032 3032 332d 3031 2d30 3554     | 2023-01-05T
-00007220: 3134 3a30 323a 3035 207c 2032 3032 332d  14:02:05 | 2023-
-00007230: 3031 2d30 3554 3134 3a30 323a 3036 207c  01-05T14:02:06 |
-00007240: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
-00007250: 3020 7c0a 2020 2020 2020 2020 2b2d 2d2d  0 |.        +---
-00007260: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00007270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007290: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
-000072a0: 2d2d 2d2d 2b0a 2020 2020 2020 2020 7c20  ----+.        | 
-000072b0: 636f 756e 7420 207c 2020 2020 2020 2020  count  |        
-000072c0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 207c 2020 2020 2020 2020 207c 2020     |         |  
-000072f0: 2020 2020 3220 7c0a 2020 2020 2020 2020      2 |.        
-00007300: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
-00007310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007330: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
-00007340: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
-00007350: 2020 7c20 746f 7461 6c73 207c 2020 2020    | totals |    
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007370: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00007380: 2020 2020 2020 207c 2031 2020 2020 2020         | 1      
-00007390: 207c 2020 2020 2020 3320 7c0a 2020 2020   |      3 |.    
-000073a0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
-000073b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000073c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-000073d0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-000073e0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
-000073f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007400: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
-00007410: 335d 2043 6865 636b 2069 6620 6576 656e  3] Check if even
-00007420: 7473 2061 7265 2073 6f72 7465 642e 0a20  ts are sorted.. 
-00007430: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00007440: 6973 5f73 6f72 7465 6428 6576 656e 7473  is_sorted(events
-00007450: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00007460: 7265 7375 6c74 290a 2020 2020 2020 2020  result).        
-00007470: 6060 600a 2020 2020 2020 2020 3c21 2d2d  ```.        <!--
-00007480: 2065 6e64 2067 6574 5f73 7461 7274 6564   end get_started
-00007490: 5f65 7861 6d70 6c65 2e70 7920 2d2d 3e0a  _example.py -->.
-000074a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000074b0: 2023 2320 322e 332e 2053 686f 7274 2074   ## 2.3. Short t
-000074c0: 6865 6f72 790a 2020 2020 2020 2020 0a20  heory.        . 
-000074d0: 2020 2020 2020 2054 6865 206c 6962 7261         The libra
-000074e0: 7279 2070 726f 7669 6465 7320 746f 6f6c  ry provides tool
-000074f0: 7320 666f 7220 6861 6e64 6c69 6e67 2073  s for handling s
-00007500: 7472 6561 6d20 6461 7461 2e20 5768 6174  tream data. What
-00007510: 2773 2061 2073 7472 6561 6d3f 2049 7427  's a stream? It'
-00007520: 7320 6120 7365 7175 656e 6365 206f 6620  s a sequence of 
-00007530: 656c 656d 656e 7473 2066 726f 6d20 6120  elements from a 
-00007540: 736f 7572 6365 2074 6861 740a 2020 2020  source that.    
-00007550: 2020 2020 7375 7070 6f72 7473 2061 6767      supports agg
-00007560: 7265 6761 7465 206f 7065 7261 7469 6f6e  regate operation
-00007570: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
-00007580: 2020 2020 2323 2320 5465 726d 730a 2020      ### Terms.  
-00007590: 2020 2020 2020 0a20 2020 2020 2020 202d        .        -
-000075a0: 202a 2a44 6174 6120 6f62 6a65 6374 2a2a   **Data object**
-000075b0: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
-000075c0: 2060 4461 7461 6020 636c 6173 7320 7768   `Data` class wh
-000075d0: 6963 6820 6973 2077 7261 7070 6572 2075  ich is wrapper u
-000075e0: 6e64 6572 2073 7472 6561 6d2e 0a20 2020  nder stream..   
-000075f0: 2020 2020 202d 202a 2a53 6571 7565 6e63       - **Sequenc
-00007600: 6520 6f66 2065 6c65 6d65 6e74 732a 2a3a  e of elements**:
-00007610: 0a20 2020 2020 2020 2020 2041 205f 4461  .          A _Da
-00007620: 7461 206f 626a 6563 745f 2070 726f 7669  ta object_ provi
-00007630: 6465 7320 616e 2069 6e74 6572 6661 6365  des an interface
-00007640: 2074 6f20 6120 7365 7175 656e 6365 6420   to a sequenced 
-00007650: 7365 7420 6f66 2076 616c 7565 7320 6f66  set of values of
-00007660: 2061 2073 7065 6369 6669 6320 656c 656d   a specific elem
-00007670: 656e 7420 7479 7065 2e20 5374 7265 616d  ent type. Stream
-00007680: 2069 6e73 6964 6520 7468 6520 5f44 6174   inside the _Dat
-00007690: 610a 2020 2020 2020 2020 2020 6f62 6a65  a.          obje
-000076a0: 6374 5f20 2a2a 646f 6e19 7420 6163 7475  ct_ **don.t actu
-000076b0: 616c 6c79 2073 746f 7265 2a2a 2065 6c65  ally store** ele
-000076c0: 6d65 6e74 733b 2074 6865 7920 6172 6520  ments; they are 
-000076d0: 636f 6d70 7574 6564 206f 6e20 6465 6d61  computed on dema
-000076e0: 6e64 2e0a 2020 2020 2020 2020 2d20 2a2a  nd..        - **
-000076f0: 6461 7461 2073 6f75 7263 652a 2a20 2865  data source** (e
-00007700: 7861 6374 6c79 2069 6e20 736d 616c 6c20  xactly in small 
-00007710: 6c65 7474 6572 7329 3a0a 2020 2020 2020  letters):.      
-00007720: 2020 2020 416e 7920 736f 7572 6365 206f      Any source o
-00007730: 6620 6461 7461 2e20 452e 672e 205b 4c69  f data. E.g. [Li
-00007740: 6768 7477 6569 6768 7420 4461 7461 2050  ghtweight Data P
-00007750: 726f 7669 6465 725d 2868 7474 7073 3a2f  rovider](https:/
-00007760: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
-00007770: 6e65 742f 7468 322d 6c77 2d64 6174 612d  net/th2-lw-data-
-00007780: 7072 6f76 6964 6572 292c 2063 6f6c 6c65  provider), colle
-00007790: 6374 696f 6e73 2c0a 2020 2020 2020 2020  ctions,.        
-000077a0: 2020 6172 7261 7973 2c20 6f72 2049 2f4f    arrays, or I/O
-000077b0: 2072 6573 6f75 7263 6573 2e0a 2020 2020   resources..    
-000077c0: 2020 2020 2d20 2a2a 4461 7461 536f 7572      - **DataSour
-000077d0: 6365 2a2a 3a0a 2020 2020 2020 2020 2020  ce**:.          
-000077e0: 4120 636c 6173 7320 7468 6174 2069 7320  A class that is 
-000077f0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
-00007800: 6c69 6e6b 2062 6574 7765 656e 2074 6865  link between the
-00007810: 2053 6f75 7263 6541 5049 2061 6e64 2043   SourceAPI and C
-00007820: 6f6d 6d61 6e64 732e 0a20 2020 2020 2020  ommands..       
-00007830: 202d 202a 2a53 6f75 7263 6541 5049 2a2a   - **SourceAPI**
-00007840: 3a0a 2020 2020 2020 2020 2020 4561 6368  :.          Each
-00007850: 2073 6f75 7263 6520 6861 7320 6974 7320   source has its 
-00007860: 6f77 6e20 4150 4920 746f 2072 6574 7269  own API to retri
-00007870: 6576 6520 6461 7461 2e20 536f 7572 6365  eve data. Source
-00007880: 4150 4920 6973 2061 2063 6c61 7373 2074  API is a class t
-00007890: 6861 7420 7072 6f76 6964 6520 4150 4920  hat provide API 
-000078a0: 666f 7220 736f 6d65 2064 6174 6120 736f  for some data so
-000078b0: 7572 6365 2e0a 2020 2020 2020 2020 2d20  urce..        - 
-000078c0: 2a2a 436f 6d6d 616e 6473 2a2a 3a0a 2020  **Commands**:.  
-000078d0: 2020 2020 2020 2020 436c 6173 7365 7320          Classes 
-000078e0: 7468 6174 2070 726f 7669 6465 2075 7365  that provide use
-000078f0: 722d 6672 6965 6e64 6c79 2069 6e74 6572  r-friendly inter
-00007900: 6661 6365 7320 666f 7220 6765 7474 696e  faces for gettin
-00007910: 6720 736f 6d65 2064 6174 6120 6672 6f6d  g some data from
-00007920: 2044 6174 6153 6f75 7263 652e 2043 6f6d   DataSource. Com
-00007930: 6d61 6e64 7320 7573 6520 5f53 6f75 7263  mands use _Sourc
-00007940: 6541 5049 5f20 746f 0a20 2020 2020 2020  eAPI_ to.       
-00007950: 2020 2061 6368 6965 7665 2069 742e 0a20     achieve it.. 
-00007960: 2020 2020 2020 202d 202a 2a41 6461 7074         - **Adapt
-00007970: 6572 732a 2a3a 0a20 2020 2020 2020 2020  ers**:.         
-00007980: 2049 7427 7320 7369 6d69 6c61 7220 746f   It's similar to
-00007990: 2066 756e 6374 696f 6e20 666f 7220 6044   function for `D
-000079a0: 6174 612e 6d61 7060 206d 6574 686f 642e  ata.map` method.
-000079b0: 2041 646f 7074 6162 6c65 2063 6f6d 6d61   Adoptable comma
-000079c0: 6e64 7320 7573 6564 2069 7420 746f 2075  nds used it to u
-000079d0: 7064 6174 6520 7468 6520 6461 7461 2073  pdate the data s
-000079e0: 7472 6561 6d2e 0a20 2020 2020 2020 202d  tream..        -
-000079f0: 202a 2a41 6767 7265 6761 7465 206f 7065   **Aggregate ope
-00007a00: 7261 7469 6f6e 732a 2a3a 0a20 2020 2020  rations**:.     
-00007a10: 2020 2020 2043 6f6d 6d6f 6e20 6f70 6572       Common oper
-00007a20: 6174 696f 6e73 2073 7563 6820 6173 2066  ations such as f
-00007a30: 696c 7465 722c 206d 6170 2c20 6c69 6d69  ilter, map, limi
-00007a40: 7420 616e 6420 736f 206f 6e2e 0a20 2020  t and so on..   
-00007a50: 2020 2020 202d 202a 2a57 6f72 6b66 6c6f       - **Workflo
-00007a60: 772a 2a3a 2041 6e20 6f72 6465 7265 6420  w**: An ordered 
-00007a70: 7365 7420 6f66 205f 4167 6772 6567 6174  set of _Aggregat
-00007a80: 6520 6f70 6572 6174 696f 6e73 5f2e 0a20  e operations_.. 
-00007a90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007aa0: 2323 2320 436f 6e63 6570 740a 2020 2020  ### Concept.    
-00007ab0: 2020 2020 0a20 2020 2020 2020 2054 6865      .        The
-00007ac0: 206c 6962 7261 7279 2064 6573 6372 6962   library describ
-00007ad0: 6573 2074 6865 2068 6967 682d 6c65 7665  es the high-leve
-00007ae0: 6c20 696e 7465 7266 6163 6573 2060 4953  l interfaces `IS
-00007af0: 6f75 7263 6541 5049 602c 2060 4944 6174  ourceAPI`, `IDat
-00007b00: 6153 6f75 7263 6560 2c20 6049 436f 6d6d  aSource`, `IComm
-00007b10: 616e 6460 2c20 6049 4164 6170 7465 7260  and`, `IAdapter`
-00007b20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00007b30: 2020 2041 6e79 2064 6174 6120 736f 7572     Any data sour
-00007b40: 6365 206d 7573 7420 6265 2064 6573 6372  ce must be descr
-00007b50: 6962 6564 2062 7920 7468 6520 6049 4461  ibed by the `IDa
-00007b60: 7461 536f 7572 6365 6020 6162 7374 7261  taSource` abstra
-00007b70: 6374 2063 6c61 7373 2e20 5468 6573 6520  ct class. These 
-00007b80: 6361 6e20 6265 205f 4669 6c65 4461 7461  can be _FileData
-00007b90: 536f 7572 6365 5f2c 0a20 2020 2020 2020  Source_,.       
-00007ba0: 205f 4353 5644 6174 6153 6f75 7263 655f   _CSVDataSource_
-00007bb0: 2c20 5f44 4244 6174 6153 6f75 7263 655f  , _DBDataSource_
-00007bc0: 2061 6e64 206f 7468 6572 2e0a 2020 2020   and other..    
-00007bd0: 2020 2020 0a20 2020 2020 2020 2055 7375      .        Usu
-00007be0: 616c 6c79 2c20 6461 7461 2073 6f75 7263  ally, data sourc
-00007bf0: 6573 2068 6176 6520 736f 6d65 206b 696e  es have some kin
-00007c00: 6420 6f66 2041 5049 2e20 4461 7461 6261  d of API. Databa
-00007c10: 7365 7320 2d20 7072 6f76 6964 6520 5351  ses - provide SQ
-00007c20: 4c20 6c61 6e67 7561 6765 2c20 7768 656e  L language, when
-00007c30: 2077 6f72 6b69 6e67 2077 6974 6820 6120   working with a 
-00007c40: 6669 6c65 2c20 796f 7520 6361 6e20 7265  file, you can re
-00007c50: 6164 0a20 2020 2020 2020 206c 696e 6520  ad.        line 
-00007c60: 6279 206c 696e 652c 2065 7463 2e20 5468  by line, etc. Th
-00007c70: 6973 2041 5049 2069 7320 6465 7363 7269  is API is descri
-00007c80: 6265 6420 6279 2074 6865 2060 4953 6f75  bed by the `ISou
-00007c90: 7263 6541 5049 6020 636c 6173 732e 2042  rceAPI` class. B
-00007ca0: 6563 6175 7365 2064 6966 6665 7265 6e74  ecause different
-00007cb0: 2076 6572 7369 6f6e 7320 6f66 2074 6865   versions of the
-00007cc0: 2073 616d 6520 6461 7461 2073 6f75 7263   same data sourc
-00007cd0: 650a 2020 2020 2020 2020 6d61 7920 6861  e.        may ha
-00007ce0: 7665 2064 6966 6665 7265 6e74 2041 5049  ve different API
-00007cf0: 2c20 6974 2069 7320 6265 7474 6572 2074  , it is better t
-00007d00: 6f20 6372 6561 7465 2061 2063 6c61 7373  o create a class
-00007d10: 2066 6f72 2065 6163 6820 7665 7273 696f   for each versio
-00007d20: 6e2e 0a20 2020 2020 2020 200a 2020 2020  n..        .    
-00007d30: 2020 2020 4765 6e65 7261 6c6c 792c 2064      Generally, d
-00007d40: 6174 6120 736f 7572 6365 2041 5049 7320  ata source APIs 
-00007d50: 6172 6520 6869 6464 656e 2062 6568 696e  are hidden behin
-00007d60: 6420 636f 6e76 656e 6965 6e74 2069 6e74  d convenient int
-00007d70: 6572 6661 6365 732e 2054 6865 2072 6f6c  erfaces. The rol
-00007d80: 6520 6f66 2074 6865 7365 2069 6e74 6572  e of these inter
-00007d90: 6661 6365 7320 6973 2070 6c61 7965 640a  faces is played.
-00007da0: 2020 2020 2020 2020 6279 2060 4943 6f6d          by `ICom
-00007db0: 6d61 6e64 6020 636c 6173 7365 732e 0a20  mand` classes.. 
-00007dc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007dd0: 6049 4164 6170 7465 7260 2063 6c61 7373  `IAdapter` class
-00007de0: 6573 2074 7261 6e73 666f 726d 2064 6174  es transform dat
-00007df0: 6120 7374 7265 616d 206c 696b 6520 6675  a stream like fu
-00007e00: 6e63 7469 6f6e 7320 666f 7220 6044 6174  nctions for `Dat
-00007e10: 612e 6d61 7060 206d 6574 686f 642e 2045  a.map` method. E
-00007e20: 7373 656e 7469 616c 6c79 2069 7427 7320  ssentially it's 
-00007e30: 7468 6520 7361 6d65 2074 6869 6e67 2062  the same thing b
-00007e40: 7574 206d 6f72 650a 2020 2020 2020 2020  ut more.        
-00007e50: 666c 6578 6962 6c65 2e0a 2020 2020 2020  flexible..      
-00007e60: 2020 0a20 2020 2020 2020 2046 6f72 2065    .        For e
-00007e70: 7861 6d70 6c65 2c20 4c77 4450 2044 6174  xample, LwDP Dat
-00007e80: 6153 6f75 7263 6528 6874 7470 733a 2f2f  aSource(https://
-00007e90: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00007ea0: 6574 2f74 6832 2d64 732d 736f 7572 6365  et/th2-ds-source
-00007eb0: 2d6c 7764 7029 2075 7365 7320 7468 6573  -lwdp) uses thes
-00007ec0: 6520 6162 7374 7261 6374 2063 6c61 7373  e abstract class
-00007ed0: 6573 2074 6f20 6275 696c 6420 6974 7320  es to build its 
-00007ee0: 696d 706c 656d 656e 7461 7469 6f6e 2e59  implementation.Y
-00007ef0: 6f75 2063 616e 2065 6173 696c 7920 6372  ou can easily cr
-00007f00: 6561 7465 2079 6f75 7220 6f77 6e20 756e  eate your own un
-00007f10: 6971 7565 2063 6f6d 6d61 6e64 7320 666f  ique commands fo
-00007f20: 7220 5f4c 7744 5020 4461 7461 536f 7572  r _LwDP DataSour
-00007f30: 6365 5f2c 2061 7320 7765 6c6c 2061 7320  ce_, as well as 
-00007f40: 656e 7469 7265 0a20 2020 2020 2020 205f  entire.        _
-00007f50: 4461 7461 536f 7572 6365 5f20 636c 6173  DataSource_ clas
-00007f60: 7365 732e 205b 4865 7265 2069 7320 6120  ses. [Here is a 
-00007f70: 646f 6375 6d65 6e74 6174 696f 6e5d 2864  documentation](d
-00007f80: 6f63 756d 656e 7461 7469 6f6e 2f64 6174  ocumentation/dat
-00007f90: 6173 6f75 7263 652e 6d64 2920 6f6e 2068  asource.md) on h
-00007fa0: 6f77 2074 6f20 696d 706c 656d 656e 7420  ow to implement 
-00007fb0: 7468 6573 6520 696e 7465 7266 6163 6573  these interfaces
-00007fc0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00007fd0: 2020 2021 5b44 6174 6120 7374 7265 616d     ![Data stream
-00007fe0: 2070 6970 656c 696e 655d 2864 6f63 756d   pipeline](docum
-00007ff0: 656e 7461 7469 6f6e 2f69 6d67 2f63 6f6e  entation/img/con
-00008000: 6365 7074 2e70 6e67 290a 2020 2020 2020  cept.png).      
-00008010: 2020 0a20 2020 2020 2020 2023 2323 2053    .        ### S
-00008020: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
-00008030: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00008040: 2020 4675 7274 6865 726d 6f72 652c 2073    Furthermore, s
-00008050: 7472 6561 6d20 6f70 6572 6174 696f 6e73  tream operations
-00008060: 2068 6176 6520 7477 6f20 6675 6e64 616d   have two fundam
-00008070: 656e 7461 6c20 6368 6172 6163 7465 7269  ental characteri
-00008080: 7374 6963 7320 7468 6174 206d 616b 6520  stics that make 
-00008090: 7468 656d 2076 6572 7920 6469 6666 6572  them very differ
-000080a0: 656e 7420 6672 6f6d 2063 6f6c 6c65 6374  ent from collect
-000080b0: 696f 6e0a 2020 2020 2020 2020 6f70 6572  ion.        oper
-000080c0: 6174 696f 6e73 3a20 5f50 6970 656c 696e  ations: _Pipelin
-000080d0: 696e 675f 2061 6e64 205f 496e 7465 726e  ing_ and _Intern
-000080e0: 616c 2069 7465 7261 7469 6f6e 5f2e 0a20  al iteration_.. 
-000080f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008100: 2323 2323 2050 6970 656c 696e 696e 670a  #### Pipelining.
-00008110: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008120: 204d 616e 7920 7374 7265 616d 206f 7065   Many stream ope
-00008130: 7261 7469 6f6e 7320 7265 7475 726e 2061  rations return a
-00008140: 2073 7472 6561 6d20 7468 656d 7365 6c76   stream themselv
-00008150: 6573 2e20 5468 6973 2061 6c6c 6f77 7320  es. This allows 
-00008160: 6f70 6572 6174 696f 6e73 2074 6f20 6265  operations to be
-00008170: 2063 6861 696e 6564 2074 6f20 666f 726d   chained to form
-00008180: 2061 206c 6172 6765 7220 7069 7065 6c69   a larger pipeli
-00008190: 6e65 2e0a 2020 2020 2020 2020 0a20 2020  ne..        .   
-000081a0: 2020 2020 2021 5b44 6174 6120 7374 7265       ![Data stre
-000081b0: 616d 2070 6970 656c 696e 655d 2864 6f63  am pipeline](doc
-000081c0: 756d 656e 7461 7469 6f6e 2f69 6d67 2f64  umentation/img/d
-000081d0: 6174 615f 7374 7265 616d 5f70 6970 656c  ata_stream_pipel
-000081e0: 696e 652e 706e 6729 0a20 2020 2020 2020  ine.png).       
-000081f0: 200a 2020 2020 2020 2020 2323 2323 2049   .        #### I
-00008200: 6e74 6572 6e61 6c20 6974 6572 6174 696f  nternal iteratio
-00008210: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00008220: 2020 2049 6e20 636f 6e74 7261 7374 2074     In contrast t
-00008230: 6f20 636f 6c6c 6563 7469 6f6e 732c 2077  o collections, w
-00008240: 6869 6368 2061 7265 2069 7465 7261 7465  hich are iterate
-00008250: 6420 6578 706c 6963 6974 6c79 2028 6578  d explicitly (ex
-00008260: 7465 726e 616c 2069 7465 7261 7469 6f6e  ternal iteration
-00008270: 292c 2073 7472 6561 6d20 6f70 6572 6174  ), stream operat
-00008280: 696f 6e73 2064 6f20 7468 6520 6974 6572  ions do the iter
-00008290: 6174 696f 6e0a 2020 2020 2020 2020 6265  ation.        be
-000082a0: 6869 6e64 2074 6865 2073 6365 6e65 7320  hind the scenes 
-000082b0: 666f 7220 796f 752e 204e 6f74 652c 2069  for you. Note, i
-000082c0: 7420 646f 6573 6e27 7420 6d65 616e 2079  t doesn't mean y
-000082d0: 6f75 2063 616e 6e6f 7420 6974 6572 6174  ou cannot iterat
-000082e0: 6520 7468 6520 5f44 6174 6120 6f62 6a65  e the _Data obje
-000082f0: 6374 5f2e 0a20 2020 2020 2020 200a 2020  ct_..        .  
-00008300: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00008310: 2323 2044 6174 6120 6974 6572 6174 696f  ## Data iteratio
-00008320: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00008330: 2020 2054 6865 2044 6174 6120 6f62 6a65     The Data obje
-00008340: 6374 2063 6f6e 7374 7275 6374 6f72 206d  ct constructor m
-00008350: 6574 686f 6420 7461 6b65 7320 696e 2061  ethod takes in a
-00008360: 7320 6172 6775 6d65 6e74 2065 6974 6865  s argument eithe
-00008370: 7220 616e 2069 7465 7261 746f 7220 6f76  r an iterator ov
-00008380: 6572 206f 626a 6563 7473 206f 7220 6120  er objects or a 
-00008390: 6765 6e65 7261 746f 7220 6675 6e63 7469  generator functi
-000083a0: 6f6e 2e0a 2020 2020 2020 2020 5468 6520  on..        The 
-000083b0: 4461 7461 206f 626a 6563 7420 6974 6572  Data object iter
-000083c0: 6174 6f72 2068 616e 646c 6573 2065 6163  ator handles eac
-000083d0: 6820 6974 656d 2069 6e20 7468 6973 2069  h item in this i
-000083e0: 7465 7261 746f 7220 6f72 2067 656e 6572  terator or gener
-000083f0: 6174 6f72 2061 7320 7468 6579 2061 7265  ator as they are
-00008400: 2c20 6d65 616e 696e 6720 6974 2064 6f65  , meaning it doe
-00008410: 736e 2774 2074 7279 2074 6f20 7265 6164  sn't try to read
-00008420: 2074 6865 2063 6f6e 7465 6e74 206f 6620   the content of 
-00008430: 6974 656d 206f 7220 7265 7475 726e 2074  item or return t
-00008440: 6865 6d20 6d6f 6469 6669 6564 2069 6e20  hem modified in 
-00008450: 616e 7920 7761 792c 2069 6e73 7465 6164  any way, instead
-00008460: 2072 6574 7572 6e73 2074 6865 2069 7465   returns the ite
-00008470: 6d20 6974 7365 6c66 2e0a 2020 2020 2020  m itself..      
-00008480: 2020 5468 6520 6f6e 6c79 2065 7863 6570    The only excep
-00008490: 7469 6f6e 2074 6f20 7468 6973 2069 7320  tion to this is 
-000084a0: 7768 656e 2044 6174 6120 6f62 6a65 6374  when Data object
-000084b0: 2069 7320 6275 696c 7420 7573 696e 6720   is built using 
-000084c0: 6974 6572 6174 6f72 206f 7220 6765 6e65  iterator or gene
-000084d0: 7261 746f 7220 6f76 6572 206f 7468 6572  rator over other
-000084e0: 2044 6174 6120 6f62 6a65 6374 732e 204e   Data objects. N
-000084f0: 6f74 6520 7468 6174 2074 6869 7320 6974  ote that this it
-00008500: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
-00008510: 746f 7220 6d75 7374 206f 6e6c 7920 6265  tor must only be
-00008520: 2079 6965 6c64 696e 6720 4461 7461 206f   yielding Data o
-00008530: 626a 6563 7473 2061 6e64 206e 6f74 6869  bjects and nothi
-00008540: 6e67 2065 6c73 652e 2049 6620 7765 2062  ng else. If we b
-00008550: 7569 6c64 2066 726f 6d20 6120 6d69 7820  uild from a mix 
-00008560: 6f66 2044 6174 6120 6f62 6a65 6374 7320  of Data objects 
-00008570: 616e 6420 736f 6d65 206f 7468 6572 2074  and some other t
-00008580: 7970 6573 2c20 4461 7461 206f 626a 6563  ypes, Data objec
-00008590: 7473 2720 636f 6e74 656e 7420 776f 6e27  ts' content won'
-000085a0: 7420 6265 2072 6561 6420 616e 6420 696e  t be read and in
-000085b0: 7374 6561 6420 6974 2077 696c 6c20 6265  stead it will be
-000085c0: 2072 6574 7572 6e65 6420 6173 2044 6174   returned as Dat
-000085d0: 6120 6f62 6a65 6374 2069 7473 656c 662e  a object itself.
-000085e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000085f0: 2020 536d 616c 6c20 6578 616d 706c 6520    Small example 
-00008600: 746f 2064 656d 6f6e 7374 7261 7465 3a0a  to demonstrate:.
-00008610: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008620: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00008630: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
-00008640: 5f73 6572 7669 6365 732e 6461 7461 2069  _services.data i
-00008650: 6d70 6f72 7420 4461 7461 0a20 2020 2020  mport Data.     
-00008660: 2020 200a 2020 2020 2020 2020 6431 203d     .        d1 =
-00008670: 2044 6174 6128 5b31 2c32 2c33 5d29 0a20   Data([1,2,3]). 
-00008680: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
-00008690: 285b 342c 352c 365d 290a 2020 2020 2020  ([4,5,6]).      
-000086a0: 2020 0a20 2020 2020 2020 206f 6e6c 795f    .        only_
-000086b0: 6461 7461 5f6f 626a 6563 7473 203d 2044  data_objects = D
-000086c0: 6174 6128 5b64 312c 6432 5d29 2023 2057  ata([d1,d2]) # W
-000086d0: 696c 6c20 6974 6572 6174 6520 6173 2031  ill iterate as 1
-000086e0: 2c32 2c33 2c34 2c35 2c36 0a20 2020 2020  ,2,3,4,5,6.     
-000086f0: 2020 2064 6174 615f 616e 645f 6c69 7374     data_and_list
-00008700: 203d 2044 6174 6128 5b64 312c 5b34 2c35   = Data([d1,[4,5
-00008710: 2c36 5d5d 2920 2320 5769 6c6c 2069 7465  ,6]]) # Will ite
-00008720: 7261 7465 2061 7320 6431 2c20 5b34 2c35  rate as d1, [4,5
-00008730: 2c36 5d0a 2020 2020 2020 2020 6461 7461  ,6].        data
-00008740: 5f61 6e64 5f6e 756d 6265 7273 203d 2044  _and_numbers = D
-00008750: 6174 6128 5b64 312c 342c 352c 365d 2920  ata([d1,4,5,6]) 
-00008760: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
-00008770: 7320 6431 2c34 2c35 2c36 0a20 2020 2020  s d1,4,5,6.     
-00008780: 2020 206c 6973 7473 5f6f 6e6c 7920 3d20     lists_only = 
-00008790: 4461 7461 285b 312c 322c 335d 2c5b 342c  Data([1,2,3],[4,
-000087a0: 352c 365d 2920 2320 5769 6c6c 2069 7465  5,6]) # Will ite
-000087b0: 7261 7465 2061 7320 5b31 2c32 2c33 5d2c  rate as [1,2,3],
-000087c0: 5b34 2c35 2c36 5d0a 2020 2020 2020 2020  [4,5,6].        
-000087d0: 0a20 2020 2020 2020 2023 2049 6620 7765  .        # If we
-000087e0: 2077 616e 7420 746f 2069 7465 7261 7465   want to iterate
-000087f0: 206f 7665 7220 636f 6e74 656e 7420 6f66   over content of
-00008800: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
-00008810: 7765 2073 686f 756c 6420 6669 7273 7420  we should first 
-00008820: 6372 6561 7465 2044 6174 6120 6f62 6a65  create Data obje
-00008830: 6374 7320 6672 6f6d 2074 6865 6d2c 0a20  cts from them,. 
-00008840: 2020 2020 2020 2023 2074 6865 6e20 7573         # then us
-00008850: 6520 7468 656d 2074 6f20 636f 6e73 7472  e them to constr
-00008860: 7563 7420 6e65 7720 4461 7461 206f 626a  uct new Data obj
-00008870: 6563 7420 6173 2069 6e20 6361 7365 206f  ect as in case o
-00008880: 6620 6431 2061 6e64 2064 322c 2063 7265  f d1 and d2, cre
-00008890: 6174 696e 6720 276f 6e6c 795f 6461 7461  ating 'only_data
-000088a0: 5f6f 626a 6563 7473 2720 696e 2074 6869  _objects' in thi
-000088b0: 7320 6578 616d 706c 652e 0a20 2020 2020  s example..     
-000088c0: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
-000088d0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000088e0: 2020 2323 2320 4461 7461 2063 6163 6869    ### Data cachi
-000088f0: 6e67 0a20 2020 2020 2020 200a 2020 2020  ng.        .    
-00008900: 2020 2020 5468 6520 5f44 6174 6120 6f62      The _Data ob
-00008910: 6a65 6374 5f20 7072 6f76 6964 6573 2074  ject_ provides t
-00008920: 6865 2061 6269 6c69 7479 2074 6f20 7573  he ability to us
-00008930: 6520 7468 6520 6361 6368 652e 2054 6865  e the cache. The
-00008940: 2063 6163 6865 2077 6f72 6b73 2066 6f72   cache works for
-00008950: 2065 6163 6820 5f44 6174 6120 6f62 6a65   each _Data obje
-00008960: 6374 5f2c 2074 6861 7420 6973 2c20 796f  ct_, that is, yo
-00008970: 7520 6368 6f6f 7365 0a20 2020 2020 2020  u choose.       
-00008980: 2077 6869 6368 205f 4461 7461 206f 626a   which _Data obj
-00008990: 6563 745f 2079 6f75 2077 616e 7420 746f  ect_ you want to
-000089a0: 2073 6176 652e 2054 6865 205f 4461 7461   save. The _Data
-000089b0: 206f 626a 6563 745f 2063 6163 6865 2069   object_ cache i
-000089c0: 7320 7361 7665 6420 6166 7465 7220 7468  s saved after th
-000089d0: 6520 6669 7273 7420 6974 6572 6174 696f  e first iteratio
-000089e0: 6e2c 2062 7574 2074 6865 2069 7465 7261  n, but the itera
-000089f0: 7469 6f6e 0a20 2020 2020 2020 2073 6f75  tion.        sou
-00008a00: 7263 6520 6d61 7920 6265 2064 6966 6665  rce may be diffe
-00008a10: 7265 6e74 2e0a 2020 2020 2020 2020 0a20  rent..        . 
-00008a20: 2020 2020 2020 2049 6620 796f 7520 646f         If you do
-00008a30: 6e27 7420 7573 6520 7468 6520 6361 6368  n't use the cach
-00008a40: 652c 2079 6f75 7220 736f 7572 6365 2077  e, your source w
-00008a50: 696c 6c20 6265 2074 6865 2064 6174 6120  ill be the data 
-00008a60: 736f 7572 6365 2079 6f75 2068 6176 6520  source you have 
-00008a70: 696e 2074 6865 205f 4461 7461 204f 626a  in the _Data Obj
-00008a80: 6563 745f 2e20 4275 7420 6966 2079 6f75  ect_. But if you
-00008a90: 2075 7365 2074 6865 2063 6163 6865 2c0a   use the cache,.
-00008aa0: 2020 2020 2020 2020 796f 7572 2073 6f75          your sou
-00008ab0: 7263 6520 6361 6e20 6265 2074 6865 2064  rce can be the d
-00008ac0: 6174 6120 736f 7572 6365 2c20 7468 6520  ata source, the 
-00008ad0: 7061 7265 6e74 2063 6163 6865 2c20 6f72  parent cache, or
-00008ae0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
-00008af0: 2020 2020 0a20 2020 2020 2020 202a 2054      .        * T
-00008b00: 6865 2064 6174 6120 736f 7572 6365 3a0a  he data source:.
-00008b10: 2020 2020 2020 2020 2020 4966 2074 6865            If the
-00008b20: 205f 4461 7461 204f 626a 6563 745f 2064   _Data Object_ d
-00008b30: 6f65 736e 2774 2068 6176 6520 6120 7061  oesn't have a pa
-00008b40: 7265 6e74 2063 6163 6865 2061 6e64 2069  rent cache and i
-00008b50: 7473 2063 6163 6865 2e0a 2020 2020 2020  ts cache..      
-00008b60: 2020 2a20 5468 6520 7061 7265 6e74 2063    * The parent c
-00008b70: 6163 6865 3a0a 2020 2020 2020 2020 2020  ache:.          
-00008b80: 4966 2074 6865 205f 4461 7461 204f 626a  If the _Data Obj
-00008b90: 6563 745f 2068 6173 2061 2070 6172 656e  ect_ has a paren
-00008ba0: 7420 6361 6368 652e 2049 7420 646f 6573  t cache. It does
-00008bb0: 6e27 7420 6d61 7474 6572 2077 6861 7420  n't matter what 
-00008bc0: 706f 7369 7469 6f6e 2074 6865 2070 6172  position the par
-00008bd0: 656e 7420 6361 6368 6520 6861 7320 696e  ent cache has in
-00008be0: 2069 6e68 6572 6974 616e 6365 2e0a 2020   inheritance..  
-00008bf0: 2020 2020 2020 2020 5f44 6174 6120 4f62          _Data Ob
-00008c00: 6a65 6374 5f20 756e 6465 7273 7461 6e64  ject_ understand
-00008c10: 7320 7768 6f73 6520 6361 6368 6520 6974  s whose cache it
-00008c20: 2069 7320 616e 6420 6578 6563 7574 6573   is and executes
-00008c30: 2074 6865 2070 6172 7420 6f66 2074 6865   the part of the
-00008c40: 2077 6f72 6b66 6c6f 7720 7468 6174 2077   workflow that w
-00008c50: 6173 206e 6f74 2065 7865 6375 7465 642e  as not executed.
-00008c60: 0a20 2020 2020 2020 202a 2054 6865 206f  .        * The o
-00008c70: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
-00008c80: 2020 2020 4966 2069 7420 6973 206e 6f74      If it is not
-00008c90: 2074 6865 2066 6972 7374 2069 7465 7261   the first itera
-00008ca0: 7469 6f6e 206f 6620 7468 6973 2044 6174  tion of this Dat
-00008cb0: 6120 6f62 6a65 6374 2e0a 2020 2020 2020  a object..      
-00008cc0: 2020 0a20 2020 2020 2020 204e 6f74 6520    .        Note 
-00008cd0: 7468 6174 2074 6865 2063 6163 6865 2073  that the cache s
-00008ce0: 7461 7465 206f 6620 7468 6520 4461 7461  tate of the Data
-00008cf0: 206f 626a 6563 7420 6973 206e 6f74 2069   object is not i
-00008d00: 6e68 6572 6974 6564 2e0a 2020 2020 2020  nherited..      
-00008d10: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
-00008d20: 466f 7263 6564 2063 6163 6869 6e67 0a20  Forced caching. 
-00008d30: 2020 2020 2020 2059 6f75 2063 616e 2074         You can t
-00008d40: 656c 6c20 4453 2074 6f20 6361 6368 6520  ell DS to cache 
-00008d50: 6461 7461 2074 6f20 7370 6563 6966 6963  data to specific
-00008d60: 2063 6163 6865 2066 696c 652c 2077 6869   cache file, whi
-00008d70: 6368 2077 6f6e 2774 2062 6520 6465 6c65  ch won't be dele
-00008d80: 7465 6420 6166 7465 7220 7363 7269 7074  ted after script
-00008d90: 2065 6e64 2e0a 2020 2020 2020 2020 596f   end..        Yo
-00008da0: 7520 6361 6e20 7365 6520 6578 616d 706c  u can see exampl
-00008db0: 6520 696e 2031 2e31 3220 7365 6374 696f  e in 1.12 sectio
-00008dc0: 6e20 6f66 205b 6765 745f 7374 6172 7465  n of [get_starte
-00008dd0: 645f 6578 616d 706c 655d 2865 7861 6d70  d_example](examp
-00008de0: 6c65 732f 6765 745f 7374 6172 7465 645f  les/get_started_
-00008df0: 6578 616d 706c 652e 7079 292e 0a20 2020  example.py)..   
-00008e00: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
-00008e10: 2020 2020 2020 2023 2323 2045 7665 6e74         ### Event
-00008e20: 5472 6565 2061 6e64 2063 6f6c 6c65 6374  Tree and collect
-00008e30: 696f 6e73 0a20 2020 2020 2020 200a 2020  ions.        .  
-00008e40: 2020 2020 2020 2323 2323 2045 7665 6e74        #### Event
-00008e50: 5472 6565 0a20 2020 2020 2020 200a 2020  Tree.        .  
-00008e60: 2020 2020 2020 6045 7665 6e74 5472 6565        `EventTree
-00008e70: 6020 6973 2061 2074 7265 652d 6261 7365  ` is a tree-base
-00008e80: 6420 6461 7461 2073 7472 7563 7475 7265  d data structure
-00008e90: 206f 6620 6576 656e 7473 2e20 4974 2061   of events. It a
-00008ea0: 6c6c 6f77 7320 796f 7520 6765 7420 6368  llows you get ch
-00008eb0: 696c 6472 656e 2061 6e64 2070 6172 656e  ildren and paren
-00008ec0: 7473 206f 6620 6576 656e 742c 0a20 2020  ts of event,.   
-00008ed0: 2020 2020 2064 6973 706c 6179 2074 7265       display tre
-00008ee0: 652c 2067 6574 2066 756c 6c20 7061 7468  e, get full path
-00008ef0: 2074 6f20 6576 656e 7420 6574 632e 0a20   to event etc.. 
-00008f00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008f10: 4465 7461 696c 733a 0a20 2020 2020 2020  Details:.       
-00008f20: 200a 2020 2020 2020 2020 2a20 6045 7665   .        * `Eve
-00008f30: 6e74 5472 6565 6020 636f 6e74 6169 6e73  ntTree` contains
-00008f40: 2061 6c6c 2065 7665 6e74 7320 696e 206d   all events in m
-00008f50: 656d 6f72 792e 0a20 2020 2020 2020 202a  emory..        *
-00008f60: 2054 7265 6520 6861 7320 736f 6d65 2069   Tree has some i
-00008f70: 6d70 6f72 7461 6e74 2074 6572 6d73 3a0a  mportant terms:.
-00008f80: 2020 2020 2020 2020 2020 2020 312e 205f              1. _
-00008f90: 416e 6365 7374 6f72 5f20 6973 2061 6e79  Ancestor_ is any
-00008fa0: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
-00008fb0: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
-00008fc0: 6565 2028 6772 616e 6470 6172 656e 742c  ee (grandparent,
-00008fd0: 2070 6172 656e 7420 6574 632e 292e 0a20   parent etc.).. 
-00008fe0: 2020 2020 2020 2020 2020 2032 2e20 5f50             2. _P
-00008ff0: 6172 656e 745f 2069 7320 6f6e 6c79 2074  arent_ is only t
-00009000: 6865 2066 6972 7374 2072 656c 6174 6976  he first relativ
-00009010: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
-00009020: 7020 7468 6520 7472 6565 2e0a 2020 2020  p the tree..    
-00009030: 2020 2020 2020 2020 332e 205f 4368 696c          3. _Chil
-00009040: 645f 2069 7320 7468 6520 6669 7273 7420  d_ is the first 
-00009050: 7265 6c61 7469 7665 206f 6620 7468 6520  relative of the 
-00009060: 6576 656e 7420 646f 776e 2074 6865 2074  event down the t
-00009070: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
-00009080: 2020 2020 2020 5461 6b65 2061 206c 6f6f        Take a loo
-00009090: 6b20 6174 2074 6865 2066 6f6c 6c6f 7769  k at the followi
-000090a0: 6e67 2048 544d 4c20 7472 6565 2074 6f20  ng HTML tree to 
-000090b0: 756e 6465 7273 7461 6e64 2074 6865 6d2e  understand them.
-000090c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000090d0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-000090e0: 2020 2020 203c 626f 6479 3e20 3c21 2d2d       <body> <!--
-000090f0: 2061 6e63 6573 746f 7220 2867 7261 6e64   ancestor (grand
-00009100: 7061 7265 6e74 292c 2062 7574 206e 6f74  parent), but not
-00009110: 2070 6172 656e 7420 2d2d 3e0a 2020 2020   parent -->.    
-00009120: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00009130: 3e20 3c21 2d2d 2070 6172 656e 7420 2620  > <!-- parent & 
-00009140: 616e 6365 7374 6f72 202d 2d3e 0a20 2020  ancestor -->.   
-00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009160: 203c 703e 4865 6c6c 6f2c 2077 6f72 6c64   <p>Hello, world
-00009170: 213c 2f70 3e20 3c21 2d2d 2063 6869 6c64  !</p> <!-- child
-00009180: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
-00009190: 2020 2020 2020 2020 203c 703e 476f 6f64           <p>Good
-000091a0: 6279 6521 3c2f 703e 203c 212d 2d20 7369  bye!</p> <!-- si
-000091b0: 626c 696e 6720 2d2d 3e0a 2020 2020 2020  bling -->.      
-000091c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000091d0: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
-000091e0: 6f64 793e 0a20 2020 2020 2020 2020 2020  ody>.           
-000091f0: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00009200: 2020 2020 2023 2323 2320 436f 6c6c 6563       #### Collec
-00009210: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
-00009220: 2020 2020 2020 202a 2a45 7665 6e74 5472         **EventTr
-00009230: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
-00009240: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
-00009250: 6620 4576 656e 7454 7265 6573 2e20 5468  f EventTrees. Th
-00009260: 6520 636f 6c6c 6563 7469 6f6e 2062 7569  e collection bui
-00009270: 6c64 7320 6120 6665 7720 5f45 7665 6e74  lds a few _Event
-00009280: 5472 6565 5f20 6279 2070 6173 7365 6420  Tree_ by passed 
-00009290: 5f44 6174 610a 2020 2020 2020 2020 6f62  _Data.        ob
-000092a0: 6a65 6374 5f2e 2041 6c74 686f 7567 6820  ject_. Although 
-000092b0: 796f 7520 6361 6e20 6368 616e 6765 2074  you can change t
-000092c0: 6865 2074 7265 6520 6469 7265 6374 6c79  he tree directly
-000092d0: 2c20 6974 2773 2062 6574 7465 7220 746f  , it's better to
-000092e0: 2064 6f20 6974 2074 6872 6f75 6768 2063   do it through c
-000092f0: 6f6c 6c65 6374 696f 6e73 2062 6563 6175  ollections becau
-00009300: 7365 2074 6865 7920 6172 6520 6177 6172  se they are awar
-00009310: 6520 6f66 0a20 2020 2020 2020 2060 6465  e of.        `de
-00009320: 7461 6368 6564 5f65 7665 6e74 7360 2061  tached_events` a
-00009330: 6e64 2063 616e 2073 6f6c 7665 2073 6f6d  nd can solve som
-00009340: 6520 6576 656e 7473 2064 6570 656e 6465  e events depende
-00009350: 6e63 6965 732e 2054 6865 2063 6f6c 6c65  ncies. The colle
-00009360: 6374 696f 6e20 6861 7320 7369 6d69 6c61  ction has simila
-00009370: 7220 6665 6174 7572 6573 206c 696b 6520  r features like 
-00009380: 6120 7369 6e67 6c65 205f 4576 656e 7454  a single _EventT
-00009390: 7265 655f 0a20 2020 2020 2020 2062 7574  ree_.        but
-000093a0: 2061 7070 6c79 696e 6720 7468 656d 2066   applying them f
-000093b0: 6f72 2061 6c6c 205f 4576 656e 7454 7265  or all _EventTre
-000093c0: 6573 5f2e 0a20 2020 2020 2020 200a 2020  es_..        .  
-000093d0: 2020 2020 2020 2a2a 5061 7265 6e74 4576        **ParentEv
-000093e0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-000093f0: 6e2a 2a20 6973 2061 2063 6f6c 6c65 6374  n** is a collect
-00009400: 696f 6e20 7369 6d69 6c61 7220 746f 205f  ion similar to _
-00009410: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00009420: 696f 6e5f 2062 7574 2063 6f6e 7461 696e  ion_ but contain
-00009430: 696e 6720 6f6e 6c79 2070 6172 656e 7420  ing only parent 
-00009440: 6576 656e 7473 2074 6861 740a 2020 2020  events that.    
-00009450: 2020 2020 6172 6520 7265 6665 7265 6e63      are referenc
-00009460: 6564 2069 6e20 7468 6520 6461 7461 2073  ed in the data s
-00009470: 7472 6561 6d2e 2054 6865 2063 6f6c 6c65  tream. The colle
-00009480: 6374 696f 6e20 6861 7320 6665 6174 7572  ction has featur
-00009490: 6573 2073 696d 696c 6172 2074 6f20 5f45  es similar to _E
-000094a0: 7665 6e74 5472 6565 436f 6c6c 6563 7469  ventTreeCollecti
-000094b0: 6f6e 5f2e 0a20 2020 2020 2020 200a 2020  on_..        .  
-000094c0: 2020 2020 2020 4465 7461 696c 733a 0a20        Details:. 
-000094d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000094e0: 2a20 546f 2075 7365 2045 5420 636f 6c6c  * To use ET coll
-000094f0: 6563 7469 6f6e 7320 796f 7520 6e65 6564  ections you need
-00009500: 2074 6f20 696e 6974 6961 6c69 7a65 2074   to initialize t
-00009510: 6865 6d20 6279 205f 4554 4344 7269 7665  hem by _ETCDrive
-00009520: 725f 2e20 4461 7461 2073 6f75 7263 6573  r_. Data sources
-00009530: 2075 7375 616c 6c79 2070 726f 7669 6465   usually provide
-00009540: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
-00009550: 2059 6f75 2063 616e 2063 7265 6174 6520   You can create 
-00009560: 6974 2062 7920 796f 7572 7365 6c66 2064  it by yourself d
-00009570: 6570 656e 6469 6e67 206f 6e20 796f 7572  epending on your
-00009580: 2064 6174 6120 7374 7275 6374 7572 652e   data structure.
-00009590: 0a20 2020 2020 2020 202a 2054 6865 2063  .        * The c
-000095a0: 6f6c 6c65 6374 696f 6e20 6861 7320 6120  ollection has a 
-000095b0: 6665 6174 7572 6520 746f 2072 6563 6f76  feature to recov
-000095c0: 6572 2065 7665 6e74 732e 2041 6c6c 2065  er events. All e
-000095d0: 7665 6e74 7320 7468 6174 2061 7265 206e  vents that are n
-000095e0: 6f74 2069 6e20 7468 6520 7265 6365 6976  ot in the receiv
-000095f0: 6564 2064 6174 6120 7374 7265 616d 2c20  ed data stream, 
-00009600: 6275 7420 7768 6963 6820 6172 650a 2020  but which are.  
-00009610: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
-00009620: 6564 2077 696c 6c20 6265 206c 6f61 6465  ed will be loade
-00009630: 6420 6672 6f6d 2074 6865 2064 6174 6120  d from the data 
-00009640: 736f 7572 6365 2e0a 2020 2020 2020 2020  source..        
-00009650: 2a20 596f 7520 6361 6e20 7461 6b65 2060  * You can take `
-00009660: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
-00009670: 2074 6f20 7365 6520 7768 6963 6820 6576   to see which ev
-00009680: 656e 7473 2061 7265 206d 6973 7369 6e67  ents are missing
-00009690: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
-000096a0: 6f75 2077 616e 742c 2079 6f75 2063 616e  ou want, you can
-000096b0: 2062 7569 6c64 2070 6172 656e 746c 6573   build parentles
-000096c0: 7320 7472 6565 7320 7768 6572 6520 7468  s trees where th
-000096d0: 6520 6d69 7373 696e 6720 6576 656e 7473  e missing events
-000096e0: 2061 7265 2073 7475 6262 6564 2069 6e73   are stubbed ins
-000096f0: 7465 6164 2e20 4a75 7374 0a20 2020 2020  tead. Just.     
-00009700: 2020 2020 2075 7365 2060 6765 745f 7061       use `get_pa
-00009710: 7265 6e74 6c65 7373 5f74 7265 6573 2829  rentless_trees()
-00009720: 602e 0a20 2020 2020 2020 200a 2020 2020  `..        .    
-00009730: 2020 2020 5265 7175 6972 656d 656e 7473      Requirements
-00009740: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00009750: 2020 2031 2e20 4576 656e 7473 2070 726f     1. Events pro
-00009760: 7669 6465 6420 746f 2045 5443 2068 6176  vided to ETC hav
-00009770: 6520 746f 2068 6176 6520 6065 7665 6e74  e to have `event
-00009780: 5f6e 616d 6560 2c20 6065 7665 6e74 5f69  _name`, `event_i
-00009790: 6460 2c20 6070 6172 656e 745f 6576 656e  d`, `parent_even
-000097a0: 745f 6964 6020 6669 656c 6473 2e20 5468  t_id` fields. Th
-000097b0: 6579 0a20 2020 2020 2020 2063 616e 2068  ey.        can h
-000097c0: 6176 6520 616e 6f74 6865 7220 6e61 6d65  ave another name
-000097d0: 7320 2869 7420 7265 736f 6c76 6573 2069  s (it resolves i
-000097e0: 6e20 7468 6520 6472 6976 6572 292e 0a20  n the driver).. 
-000097f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009800: 2323 2323 2048 696e 7473 0a20 2020 2020  #### Hints.     
-00009810: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
-00009820: 6d6f 7665 2061 6c6c 2075 6e6e 6563 6573  move all unneces
-00009830: 7361 7279 2066 6965 6c64 7320 6672 6f6d  sary fields from
-00009840: 2065 7665 6e74 7320 6265 666f 7265 2070   events before p
-00009850: 6173 7369 6e67 2074 6f20 6120 5f63 6f6c  assing to a _col
-00009860: 6c65 6374 696f 6e5f 2074 6f20 7265 6475  lection_ to redu
-00009870: 6365 206d 656d 6f72 7920 7573 6167 652e  ce memory usage.
-00009880: 0a20 2020 2020 2020 202a 2055 7365 2060  .        * Use `
-00009890: 7368 6f77 2829 6020 6d65 7468 6f64 2074  show()` method t
-000098a0: 6f20 7072 696e 7420 7468 6520 7472 6565  o print the tree
-000098b0: 2069 6e20 7472 6565 2d6c 696b 6520 7669   in tree-like vi
-000098c0: 6577 2e0a 2020 2020 2020 2020 2a20 4e6f  ew..        * No
-000098d0: 7465 2074 6861 7420 7468 6520 6067 6574  te that the `get
-000098e0: 5f78 6020 6d65 7468 6f64 7320 7769 6c6c  _x` methods will
-000098f0: 2072 6169 7365 2061 6e20 6578 6365 7074   raise an except
-00009900: 696f 6e20 6966 2079 6f75 2070 6173 7320  ion if you pass 
-00009910: 616e 2075 6e6b 6e6f 776e 2065 7665 6e74  an unknown event
-00009920: 2069 642c 2075 6e6c 696b 6520 7468 6520   id, unlike the 
-00009930: 6066 696e 645f 7860 206d 6574 686f 6473  `find_x` methods
-00009940: 2028 0a20 2020 2020 2020 2020 2074 6865   (.          the
-00009950: 7920 7265 7475 726e 204e 6f6e 6529 2e0a  y return None)..
-00009960: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
-00009970: 2077 616e 7420 746f 206b 6e6f 7720 7468   want to know th
-00009980: 6174 2073 7065 6369 6669 6564 2065 7665  at specified eve
-00009990: 6e74 2065 7869 7374 732c 2075 7365 2074  nt exists, use t
-000099a0: 6865 2070 7974 686f 6e20 6069 6e60 206b  he python `in` k
-000099b0: 6579 776f 7264 2028 652e 672e 2060 2765  eyword (e.g. `'e
-000099c0: 7665 6e74 2d69 6427 2069 6e20 6576 656e  vent-id' in even
-000099d0: 7473 5f74 7265 6560 292e 0a20 2020 2020  ts_tree`)..     
-000099e0: 2020 202a 2055 7365 2074 6865 2070 7974     * Use the pyt
-000099f0: 686f 6e20 606c 656e 6020 6b65 7977 6f72  hon `len` keywor
-00009a00: 6420 746f 2067 6574 2065 7665 6e74 7320  d to get events 
-00009a10: 6e75 6d62 6572 2069 6e20 7468 6520 7472  number in the tr
-00009a20: 6565 2e0a 2020 2020 2020 2020 0a20 2020  ee..        .   
-00009a30: 2020 2020 2023 2323 2046 6965 6c64 2052       ### Field R
-00009a40: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
-00009a50: 2049 6e74 6572 6661 6365 2063 616e 2062   Interface can b
-00009a60: 6520 666f 756e 6420 696e 2060 7468 325f  e found in `th2_
-00009a70: 6461 7461 5f73 6572 7669 6365 732f 696e  data_services/in
-00009a80: 7465 7266 6163 6573 2f75 7469 6c73 2f72  terfaces/utils/r
-00009a90: 6573 6f6c 7665 722e 7079 602e 2020 0a20  esolver.py`.  . 
-00009aa0: 2020 2020 2020 2041 6c6c 2064 6174 612d         All data-
-00009ab0: 736f 7572 6365 7320 7368 6f75 6c64 2069  sources should i
-00009ac0: 6d70 6c65 6d65 6e74 2074 6865 6d2e 0a20  mplement them.. 
-00009ad0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00009ae0: 5468 6520 6964 6561 206f 6620 7573 696e  The idea of usin
-00009af0: 6720 7265 736f 6c76 6572 733a 0a20 2020  g resolvers:.   
-00009b00: 2020 2020 2049 7420 736f 6c76 6573 2074       It solves t
-00009b10: 6865 2070 726f 626c 656d 206f 6620 6861  he problem of ha
-00009b20: 7669 6e67 2061 2066 6577 2044 6174 6153  ving a few DataS
-00009b30: 6f75 7263 6573 2077 6974 6820 7369 6d69  ources with simi
-00009b40: 6c61 7220 6461 7461 2c0a 2020 2020 2020  lar data,.      
-00009b50: 2020 6275 7420 7769 7468 2064 6966 6665    but with diffe
-00009b60: 7265 6e74 2077 6179 7320 746f 2067 6574  rent ways to get
-00009b70: 2069 742e 0a20 2020 2020 2020 200a 2020   it..        .  
-00009b80: 2020 2020 2020 5468 6573 6520 636c 6173        These clas
-00009b90: 7365 7320 7072 6f76 6964 6520 796f 7520  ses provide you 
-00009ba0: 6765 7474 6572 206d 6574 686f 6473 2e0a  getter methods..
-00009bb0: 2020 2020 2020 2020 5573 696e 6720 7468          Using th
-00009bc0: 6573 6520 636c 6173 7365 7320 616c 6c6f  ese classes allo
-00009bd0: 7773 2079 6f75 2074 6f20 6672 6565 6c79  ws you to freely
-00009be0: 2073 7769 7463 6820 6265 7477 6565 6e20   switch between 
-00009bf0: 6469 6666 6572 656e 7420 6461 7461 0a20  different data. 
-00009c00: 2020 2020 2020 2066 6f72 6d61 7473 2061         formats a
-00009c10: 6e64 2064 6f6e 2774 2063 6861 6e67 6520  nd don't change 
-00009c20: 796f 7572 2063 6f64 652e 0a20 2020 2020  your code..     
-00009c30: 2020 200a 2020 2020 2020 2020 5265 736f     .        Reso
-00009c40: 6c76 6572 7320 736f 6c76 6520 7468 6520  lvers solve the 
-00009c50: 7072 6f62 6c65 6d20 6f66 2064 6174 612d  problem of data-
-00009c60: 666f 726d 6174 206d 6967 7261 7469 6f6e  format migration
-00009c70: 2e0a 2020 2020 2020 2020 2d20 6669 656c  ..        - fiel
-00009c80: 6473 2070 6c61 6365 2063 616e 2062 6520  ds place can be 
-00009c90: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
-00009ca0: 2d20 6669 656c 6473 206e 616d 6573 2063  - fields names c
-00009cb0: 616e 2062 6520 6368 616e 6765 640a 2020  an be changed.  
-00009cc0: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00009cd0: 6573 6f6c 7665 7273 2063 616e 2077 6f72  esolvers can wor
-00009ce0: 6b20 6f6e 6c79 2077 6974 6820 6f6e 6520  k only with one 
-00009cf0: 6576 656e 742f 6d65 7373 6167 652e 0a20  event/message.. 
-00009d00: 2020 2020 2020 2049 7420 6d65 616e 732c         It means,
-00009d10: 2069 6620 796f 7572 206d 6573 7361 6765   if your message
-00009d20: 2068 6173 2073 7562 2d6d 6573 7361 6765   has sub-message
-00009d30: 7320 286c 696b 6520 7468 322d 6d65 7373  s (like th2-mess
-00009d40: 6167 6573 2069 6e20 6c77 6470 2920 6974  ages in lwdp) it
-00009d50: 200a 2020 2020 2020 2020 776f 6e27 7420   .        won't 
-00009d60: 776f 726b 2c20 6265 6361 7573 6520 7265  work, because re
-00009d70: 736f 6c76 6572 2077 696c 6c20 6e6f 7420  solver will not 
-00009d80: 6b6e 6f77 2077 6974 6820 7768 6963 6820  know with which 
-00009d90: 7375 622d 6d65 7373 6167 6520 7368 6f75  sub-message shou
-00009da0: 6c64 2069 7420 776f 726b 2e20 0a20 2020  ld it work. .   
-00009db0: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
-00009dc0: 576f 726b 6172 6f75 6e64 2a2a 2020 0a20  Workaround**  . 
-00009dd0: 2020 2020 2020 2031 2e20 4578 7061 6e64         1. Expand
-00009de0: 2061 6c6c 2079 6f75 7220 6d65 7373 6167   all your messag
-00009df0: 6573 202d 3e20 606e 6577 5f64 203d 2079  es -> `new_d = y
-00009e00: 6f75 725f 6461 7461 2e6d 6170 284d 6573  our_data.map(Mes
-00009e10: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
-00009e20: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
-00009e30: 2960 0a20 2020 2020 2020 2032 2e20 5573  )`.        2. Us
-00009e40: 6520 6045 7870 616e 6465 644d 6573 7361  e `ExpandedMessa
-00009e50: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
-00009e60: 2069 6e73 7465 6164 206f 6620 7573 7561   instead of usua
-00009e70: 6c20 604d 6573 7361 6765 4669 656c 6452  l `MessageFieldR
-00009e80: 6573 6f6c 7665 7260 2077 6865 6e20 0a20  esolver` when . 
-00009e90: 2020 2020 2020 2020 2020 2079 6f75 2074             you t
-00009ea0: 616b 6520 6669 656c 6473 2066 6f72 2065  ake fields for e
-00009eb0: 7870 616e 6465 6420 6d65 7373 6167 6573  xpanded messages
-00009ec0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00009ed0: 2020 202a 2a49 6d70 6c65 6d65 6e74 6174     **Implementat
-00009ee0: 696f 6e20 6164 7669 6365 3a2a 2a0a 2020  ion advice:**.  
-00009ef0: 2020 2020 2020 312e 2072 6169 7365 204e        1. raise N
-00009f00: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00009f10: 6f72 202d 2d20 6966 2079 6f75 7220 496d  or -- if your Im
-00009f20: 706c 656d 656e 7461 7469 6f6e 2064 6f65  plementation doe
-00009f30: 736e 2774 2073 7570 706f 7274 2074 6869  sn't support thi
-00009f40: 7320 6765 7474 6572 2e0a 2020 2020 2020  s getter..      
-00009f50: 2020 0a20 2020 2020 2020 202a 2a50 6572    .        **Per
-00009f60: 666f 726d 616e 6365 2069 6d70 6163 743a  formance impact:
-00009f70: 2a2a 0a20 2020 2020 2020 202d 2049 7420  **.        - It 
-00009f80: 6120 6269 7420 736c 6f77 6572 2074 6861  a bit slower tha
-00009f90: 6e20 7573 696e 6720 6e61 6b65 6420 6669  n using naked fi
-00009fa0: 656c 6420 6163 6365 7373 2060 6469 6374  eld access `dict
-00009fb0: 5b27 6b65 7927 5d60 2e0a 2020 2020 2020  ['key']`..      
-00009fc0: 2020 0a20 2020 2020 2020 2023 2320 322e    .        ## 2.
-00009fd0: 342e 204c 696e 6b73 0a20 2020 2020 2020  4. Links.       
-00009fe0: 200a 2020 2020 2020 2020 2d20 5b52 6570   .        - [Rep
-00009ff0: 6f72 7420 4461 7461 2050 726f 7669 6465  ort Data Provide
-0000a000: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-0000a010: 622e 636f 6d2f 7468 322d 6e65 742f 7468  b.com/th2-net/th
-0000a020: 322d 7270 742d 6461 7461 2d70 726f 7669  2-rpt-data-provi
-0000a030: 6465 7229 0a20 2020 2020 2020 202d 205b  der).        - [
-0000a040: 5468 3220 4461 7461 2053 6572 7669 6365  Th2 Data Service
-0000a050: 7320 5574 696c 735d 2868 7474 7073 3a2f  s Utils](https:/
-0000a060: 2f67 6974 6875 622e 636f 6d2f 7468 322d  /github.com/th2-
-0000a070: 6e65 742f 7468 322d 6461 7461 2d73 6572  net/th2-data-ser
-0000a080: 7669 6365 732d 7574 696c 7329 0a20 2020  vices-utils).   
-0000a090: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-0000a0a0: 332e 2042 6573 7420 7072 6163 7469 6365  3. Best practice
-0000a0b0: 730a 2020 2020 2020 2020 4465 7065 6e64  s.        Depend
-0000a0c0: 696e 6720 6f6e 2068 6f77 2079 6f75 2077  ing on how you w
-0000a0d0: 6f72 6b20 7769 7468 2060 4461 7461 206f  ork with `Data o
-0000a0e0: 626a 6563 7460 2c20 6974 2063 616e 2062  bject`, it can b
-0000a0f0: 6520 736c 6f77 206f 6620 6661 7374 2e0a  e slow of fast..
-0000a100: 2020 2020 2020 2020 4173 2077 6974 6820          As with 
-0000a110: 6120 7265 6c61 7469 6f6e 616c 2064 6174  a relational dat
-0000a120: 6162 6173 652c 2079 6f75 2063 616e 2077  abase, you can w
-0000a130: 7269 7465 2061 2071 7565 7279 2074 6861  rite a query tha
-0000a140: 7420 7769 6c6c 2072 6574 7572 6e20 6461  t will return da
-0000a150: 7461 2073 6c6f 776c 7920 6f72 2071 7569  ta slowly or qui
-0000a160: 636b 6c79 2c0a 2020 2020 2020 2020 7468  ckly,.        th
-0000a170: 6520 7361 6d65 2077 6865 6e20 776f 726b  e same when work
-0000a180: 696e 6720 7769 7468 2061 2060 4461 7461  ing with a `Data
-0000a190: 206f 626a 6563 7460 2e0a 2020 2020 2020   object`..      
-0000a1a0: 2020 0a20 2020 2020 2020 2046 6f6c 6c6f    .        Follo
-0000a1b0: 7720 7468 6520 7275 6c65 7320 746f 206d  w the rules to m
-0000a1c0: 616b 6520 796f 7572 2077 6f72 6b20 7769  ake your work wi
-0000a1d0: 7468 2044 6174 6120 6f62 6a65 6374 2066  th Data object f
-0000a1e0: 6173 743a 0a20 2020 2020 2020 2031 2e20  ast:.        1. 
-0000a1f0: 5573 6520 6044 6174 612e 7573 655f 6361  Use `Data.use_ca
-0000a200: 6368 6528 2960 2069 6620 796f 7520 6974  che()` if you it
-0000a210: 6572 6174 6520 6461 7461 206d 6f72 6520  erate data more 
-0000a220: 7468 616e 206f 6e65 2074 696d 652e 0a20  than one time.. 
-0000a230: 2020 2020 2020 2032 2e20 5472 7920 746f         2. Try to
-0000a240: 2064 6f6e 2774 2069 7465 7261 7465 206f   don't iterate o
-0000a250: 6e65 2060 4461 7461 206f 626a 6563 7460  ne `Data object`
-0000a260: 2069 6e73 6964 6520 7468 6520 6f74 6865   inside the othe
-0000a270: 7220 6f6e 652e 0a20 2020 2020 2020 2020  r one..         
-0000a280: 2020 4966 2079 6f75 2073 686f 756c 6420    If you should 
-0000a290: 746f 2064 6f20 6974 2c20 7573 6520 7368  to do it, use sh
-0000a2a0: 6f72 7420 6044 6174 6120 6f62 6a65 6374  ort `Data object
-0000a2b0: 6020 6669 7273 7420 616e 6420 6c6f 6e67  ` first and long
-0000a2c0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
-0000a2d0: 6e73 6964 6520 7468 6520 6c6f 6f70 2e0a  nside the loop..
-0000a2e0: 2020 2020 2020 2020 2020 2049 7427 6c6c             It'll
-0000a2f0: 2061 6c6c 6f77 2079 6f75 206f 7065 6e20   allow you open 
-0000a300: 7468 6520 6361 6368 6520 6669 6c65 206f  the cache file o
-0000a310: 7220 6372 6561 7465 2061 2072 6571 7565  r create a reque
-0000a320: 7374 2074 6f20 6044 6174 6120 736f 7572  st to `Data sour
-0000a330: 6365 6020 6c65 7373 206e 756d 6265 7220  ce` less number 
-0000a340: 6f66 2074 696d 6573 2e0a 2020 2020 2020  of times..      
-0000a350: 2020 0a20 2020 2020 2020 2023 2034 2e20    .        # 4. 
-0000a360: 4f66 6669 6369 616c 2044 6174 6153 6f75  Official DataSou
-0000a370: 7263 6520 696d 706c 656d 656e 7461 7469  rce implementati
-0000a380: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
-0000a390: 2020 2020 202d 205b 4c69 6768 7477 6569       - [Lightwei
-0000a3a0: 6768 7420 4461 7461 2050 726f 7669 6465  ght Data Provide
-0000a3b0: 7220 4461 7461 2053 6f75 7263 655d 2868  r Data Source](h
-0000a3c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000a3d0: 6d2f 7468 322d 6e65 742f 7468 322d 6473  m/th2-net/th2-ds
-0000a3e0: 2d73 6f75 7263 652d 6c77 6470 290a 2020  -source-lwdp).  
-0000a3f0: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
-0000a400: 2020 2020 2020 2020 2320 352e 2041 5049          # 5. API
-0000a410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-0000a420: 2020 4966 2079 6f75 2061 7265 206c 6f6f    If you are loo
-0000a430: 6b69 6e67 2066 6f72 2063 6c61 7373 6573  king for classes
-0000a440: 2064 6573 6372 6970 7469 6f6e 2073 6565   description see
-0000a450: 2074 6865 205b 4150 4920 446f 6375 6d65   the [API Docume
-0000a460: 6e74 6174 696f 6e5d 2864 6f63 756d 656e  ntation](documen
-0000a470: 7461 7469 6f6e 2f61 7069 2f69 6e64 6578  tation/api/index
-0000a480: 2e6d 6429 2e0a 2020 2020 2020 2020 0a20  .md)..        . 
-0000a490: 2020 2020 2020 2023 2036 2e20 4578 616d         # 6. Exam
-0000a4a0: 706c 6573 0a20 2020 2020 2020 200a 2020  ples.        .  
-0000a4b0: 2020 2020 2020 2d20 5b67 6574 5f73 7461        - [get_sta
-0000a4c0: 7274 6564 5f65 7861 6d70 6c65 2e70 795d  rted_example.py]
-0000a4d0: 2865 7861 6d70 6c65 732f 6765 745f 7374  (examples/get_st
-0000a4e0: 6172 7465 645f 6578 616d 706c 652e 7079  arted_example.py
-0000a4f0: 290a 2020 2020 2020 2020 0a50 6c61 7466  ).        .Platf
-0000a500: 6f72 6d3a 2055 4e4b 4e4f 574e 0a52 6571  orm: UNKNOWN.Req
-0000a510: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-0000a520: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
-0000a530: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-0000a540: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
-0000a550: 6964 6573 2d45 7874 7261 3a20 7264 700a  ides-Extra: rdp.
-0000a560: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-0000a570: 7264 7035 0a50 726f 7669 6465 732d 4578  rdp5.Provides-Ex
-0000a580: 7472 613a 2072 6470 360a 5072 6f76 6964  tra: rdp6.Provid
-0000a590: 6573 2d45 7874 7261 3a20 6c77 6470 0a50  es-Extra: lwdp.P
-0000a5a0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-0000a5b0: 7764 7031 0a50 726f 7669 6465 732d 4578  wdp1.Provides-Ex
-0000a5c0: 7472 613a 206c 7764 7032 0a50 726f 7669  tra: lwdp2.Provi
-0000a5d0: 6465 732d 4578 7472 613a 206c 7764 7033  des-Extra: lwdp3
-0000a5e0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-0000a5f0: 206c 7764 702d 6465 760a 5072 6f76 6964   lwdp-dev.Provid
-0000a600: 6573 2d45 7874 7261 3a20 7574 696c 732d  es-Extra: utils-
-0000a610: 7270 742d 7669 6577 6572 0a50 726f 7669  rpt-viewer.Provi
-0000a620: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
-0000a630: 2d72 7074 2d76 6965 7765 7235 0a50 726f  -rpt-viewer5.Pro
-0000a640: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-0000a650: 6c73 2d61 6476 616e 6365 640a            ls-advanced.
+00002700: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002710: 230a 2020 2020 2020 2020 0a20 2020 2020  #.        .     
+00002720: 2020 2023 205b 312e 315d 2046 696c 7465     # [1.1] Filte
+00002730: 722e 0a20 2020 2020 2020 2066 696c 7465  r..        filte
+00002740: 7265 645f 6576 656e 7473 3a20 4461 7461  red_events: Data
+00002750: 203d 2065 7665 6e74 732e 6669 6c74 6572   = events.filter
+00002760: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
+00002770: 6d62 6461 2065 3a20 655b 2262 6f64 7922  mbda e: e["body"
+00002780: 5d20 213d 205b 5d29 2020 2320 4669 6c74  ] != [])  # Filt
+00002790: 6572 2065 7665 6e74 7320 7769 7468 2065  er events with e
+000027a0: 6d70 7479 2062 6f64 792e 0a20 2020 2020  mpty body..     
+000027b0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+000027c0: 2020 2020 2023 205b 312e 325d 204d 6170       # [1.2] Map
+000027d0: 2e0a 2020 2020 2020 2020 6465 6620 7472  ..        def tr
+000027e0: 616e 7366 6f72 6d5f 6675 6e63 7469 6f6e  ansform_function
+000027f0: 2872 6563 6f72 6429 3a0a 2020 2020 2020  (record):.      
+00002800: 2020 2020 2020 7265 7475 726e 207b 2265        return {"e
+00002810: 7665 6e74 4e61 6d65 223a 2072 6563 6f72  ventName": recor
+00002820: 645b 2265 7665 6e74 4e61 6d65 225d 2c0a  d["eventName"],.
+00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002840: 2020 2020 2273 7563 6365 7373 6675 6c22      "successful"
+00002850: 3a20 7265 636f 7264 5b22 7375 6363 6573  : record["succes
+00002860: 7366 756c 225d 7d0a 2020 2020 2020 2020  sful"]}.        
+00002870: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002880: 2020 6669 6c74 6572 6564 5f61 6e64 5f6d    filtered_and_m
+00002890: 6170 7065 645f 6576 656e 7473 203d 2066  apped_events = f
+000028a0: 696c 7465 7265 645f 6576 656e 7473 2e6d  iltered_events.m
+000028b0: 6170 2874 7261 6e73 666f 726d 5f66 756e  ap(transform_fun
+000028c0: 6374 696f 6e29 0a20 2020 2020 2020 200a  ction).        .
+000028d0: 2020 2020 2020 2020 2320 5b31 2e33 5d20          # [1.3] 
+000028e0: 4461 7461 2070 6970 656c 696e 652e 0a20  Data pipeline.. 
+000028f0: 2020 2020 2020 2023 2020 2020 2020 2049         #       I
+00002900: 6e73 7465 6164 206f 6620 646f 696e 6720  nstead of doing 
+00002910: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
+00002920: 696f 6e73 2073 7465 7020 6279 2073 7465  ions step by ste
+00002930: 7020 796f 7520 6361 6e20 646f 2069 7420  p you can do it 
+00002940: 696e 206f 6e65 206c 696e 652e 0a20 2020  in one line..   
+00002950: 2020 2020 2066 696c 7465 7265 645f 616e       filtered_an
+00002960: 645f 6d61 7070 6564 5f65 7665 6e74 735f  d_mapped_events_
+00002970: 6279 5f70 6970 656c 696e 6520 3d20 6576  by_pipeline = ev
+00002980: 656e 7473 2e66 696c 7465 7228 0a20 2020  ents.filter(.   
+00002990: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
+000029a0: 653a 2065 5b22 626f 6479 225d 2021 3d20  e: e["body"] != 
+000029b0: 5b5d 292e 6d61 7028 0a20 2020 2020 2020  []).map(.       
+000029c0: 2020 2020 2074 7261 6e73 666f 726d 5f66       transform_f
+000029d0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+000029e0: 290a 2020 2020 2020 2020 2320 436f 6e74  ).        # Cont
+000029f0: 656e 7420 6f66 2074 6865 7365 2074 776f  ent of these two
+00002a00: 2044 6174 6120 6f62 6a65 6374 7320 7368   Data objects sh
+00002a10: 6f75 6c64 2062 6520 6571 7561 6c2e 0a20  ould be equal.. 
+00002a20: 2020 2020 2020 2061 7373 6572 7420 6c69         assert li
+00002a30: 7374 2866 696c 7465 7265 645f 616e 645f  st(filtered_and_
+00002a40: 6d61 7070 6564 5f65 7665 6e74 7329 203d  mapped_events) =
+00002a50: 3d20 6c69 7374 280a 2020 2020 2020 2020  = list(.        
+00002a60: 2020 2020 6669 6c74 6572 6564 5f61 6e64      filtered_and
+00002a70: 5f6d 6170 7065 645f 6576 656e 7473 5f62  _mapped_events_b
+00002a80: 795f 7069 7065 6c69 6e65 290a 2020 2020  y_pipeline).    
+00002a90: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00002aa0: 312e 345d 2053 6966 742e 2053 6b69 7020  1.4] Sift. Skip 
+00002ab0: 7468 6520 6669 7273 7420 6665 7720 6974  the first few it
+00002ac0: 656d 7320 6f72 206c 696d 6974 2074 6865  ems or limit the
+00002ad0: 6d2e 0a20 2020 2020 2020 2064 6174 6120  m..        data 
+00002ae0: 3d20 4461 7461 285b 312c 2032 2c20 332c  = Data([1, 2, 3,
+00002af0: 2034 2c20 352c 2036 2c20 372c 2038 2c20   4, 5, 6, 7, 8, 
+00002b00: 392c 2031 302c 2031 312c 2031 322c 2031  9, 10, 11, 12, 1
+00002b10: 332c 2031 342c 2031 355d 290a 2020 2020  3, 14, 15]).    
+00002b20: 2020 2020 6974 656d 735f 6672 6f6d 5f31      items_from_1
+00002b30: 315f 746f 5f65 6e64 3a20 4765 6e65 7261  1_to_end: Genera
+00002b40: 746f 7220 3d20 6461 7461 2e73 6966 7428  tor = data.sift(
+00002b50: 736b 6970 3d31 3029 0a20 2020 2020 2020  skip=10).       
+00002b60: 206f 6e6c 795f 6669 7273 745f 3130 5f69   only_first_10_i
+00002b70: 7465 6d73 3a20 4765 6e65 7261 746f 7220  tems: Generator 
+00002b80: 3d20 6461 7461 2e73 6966 7428 6c69 6d69  = data.sift(limi
+00002b90: 743d 3130 290a 2020 2020 2020 2020 0a20  t=10).        . 
+00002ba0: 2020 2020 2020 2023 205b 312e 355d 2043         # [1.5] C
+00002bb0: 6861 6e67 696e 6720 6361 6368 6520 7374  hanging cache st
+00002bc0: 6174 7573 2e0a 2020 2020 2020 2020 6576  atus..        ev
+00002bd0: 656e 7473 2e75 7365 5f63 6163 6865 2854  ents.use_cache(T
+00002be0: 7275 6529 0a20 2020 2020 2020 2023 206f  rue).        # o
+00002bf0: 7220 6a75 7374 0a20 2020 2020 2020 2065  r just.        e
+00002c00: 7665 6e74 732e 7573 655f 6361 6368 6528  vents.use_cache(
+00002c10: 2920 2023 2049 6620 796f 7520 7761 6e74  )  # If you want
+00002c20: 2074 6f20 6163 7469 7661 7465 2063 6163   to activate cac
+00002c30: 6865 2e0a 2020 2020 2020 2020 2320 5b31  he..        # [1
+00002c40: 2e36 5d20 5761 6c6b 2074 6872 6f75 6768  .6] Walk through
+00002c50: 2064 6174 612e 0a20 2020 2020 2020 2066   data..        f
+00002c60: 6f72 2065 7665 6e74 2069 6e20 6576 656e  or event in even
+00002c70: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00002c80: 2320 446f 2073 6f6d 6574 6869 6e67 2077  # Do something w
+00002c90: 6974 6820 6576 656e 7420 2865 7665 6e74  ith event (event
+00002ca0: 2069 7320 6120 6469 6374 292e 0a20 2020   is a dict)..   
+00002cb0: 2020 2020 2020 2020 2070 7269 6e74 2865           print(e
+00002cc0: 7665 6e74 290a 2020 2020 2020 2020 2320  vent).        # 
+00002cd0: 4166 7465 7220 6669 7273 7420 6974 6572  After first iter
+00002ce0: 6174 696f 6e20 7468 6520 6576 656e 7473  ation the events
+00002cf0: 2068 6173 2061 2063 6163 6865 2066 696c   has a cache fil
+00002d00: 652e 0a20 2020 2020 2020 2023 204e 6f77  e..        # Now
+00002d10: 2074 6865 7920 7769 6c6c 2062 6520 7573   they will be us
+00002d20: 6564 2069 6e20 7468 6520 6361 6368 6520  ed in the cache 
+00002d30: 696e 2074 6865 206e 6578 7420 6974 6572  in the next iter
+00002d40: 6174 696f 6e2e 0a20 2020 2020 2020 200a  ation..        .
+00002d50: 2020 2020 2020 2020 2320 5b31 2e37 5d20          # [1.7] 
+00002d60: 4765 7420 6e75 6d62 6572 206f 6620 7468  Get number of th
+00002d70: 6520 656c 656d 656e 7473 2069 6e20 7468  e elements in th
+00002d80: 6520 4461 7461 206f 626a 6563 742e 0a20  e Data object.. 
+00002d90: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+00002da0: 5f65 7665 6e74 7320 3d20 6576 656e 7473  _events = events
+00002db0: 2e6c 656e 0a20 2020 2020 2020 200a 2020  .len.        .  
+00002dc0: 2020 2020 2020 2320 5b31 2e38 5d20 4368        # [1.8] Ch
+00002dd0: 6563 6b20 7468 6174 2044 6174 6120 6f62  eck that Data ob
+00002de0: 6a65 6374 2069 736e 2774 2065 6d70 7479  ject isn't empty
+00002df0: 2e0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+00002e00: 6461 7461 2073 6f75 7263 6520 7368 6f75  data source shou
+00002e10: 6c64 2062 6520 6e6f 7420 656d 7074 792e  ld be not empty.
+00002e20: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002e30: 6576 656e 7473 2e69 735f 656d 7074 7920  events.is_empty 
+00002e40: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
+00002e50: 200a 2020 2020 2020 2020 2320 5b31 2e39   .        # [1.9
+00002e60: 5d20 436f 6e76 6572 7420 4461 7461 206f  ] Convert Data o
+00002e70: 626a 6563 7420 746f 2074 6865 206c 6973  bject to the lis
+00002e80: 7420 6f66 2065 6c65 6d65 6e74 7328 6576  t of elements(ev
+00002e90: 656e 7473 206f 7220 6d65 7373 6167 6573  ents or messages
+00002ea0: 292e 0a20 2020 2020 2020 2023 2042 6520  )..        # Be 
+00002eb0: 6361 7265 6675 6c2c 2074 6869 7320 6361  careful, this ca
+00002ec0: 6e20 7461 6b65 2074 6f6f 206d 7563 6820  n take too much 
+00002ed0: 6d65 6d6f 7279 2e0a 2020 2020 2020 2020  memory..        
+00002ee0: 6576 656e 7473 5f6c 6973 7420 3d20 6c69  events_list = li
+00002ef0: 7374 2865 7665 6e74 7329 0a20 2020 2020  st(events).     
+00002f00: 2020 200a 2020 2020 2020 2020 2320 5b31     .        # [1
+00002f10: 2e31 305d 2054 6865 2063 6163 6865 2069  .10] The cache i
+00002f20: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
+00002f30: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
+00002f40: 6e65 7720 4461 7461 206f 626a 6563 7420  new Data object 
+00002f50: 7468 6174 2077 696c 6c20 7573 6520 6361  that will use ca
+00002f60: 6368 6520 6672 6f6d 2074 6865 2065 7665  che from the eve
+00002f70: 6e74 7320 4461 7461 206f 626a 6563 742e  nts Data object.
+00002f80: 0a20 2020 2020 2020 2065 7665 6e74 735f  .        events_
+00002f90: 6669 6c74 6572 6564 3a20 4461 7461 203d  filtered: Data =
+00002fa0: 2065 7665 6e74 732e 6669 6c74 6572 286c   events.filter(l
+00002fb0: 616d 6264 6120 7265 636f 7264 3a20 7265  ambda record: re
+00002fc0: 636f 7264 2e67 6574 2822 6261 7463 6849  cord.get("batchI
+00002fd0: 6422 2929 0a20 2020 2020 2020 200a 2020  d")).        .  
+00002fe0: 2020 2020 2020 2320 4e65 7720 4461 7461        # New Data
+00002ff0: 206f 626a 6563 7473 2064 6f6e 2774 2075   objects don't u
+00003000: 7365 2074 6865 6972 206f 776e 2063 6163  se their own cac
+00003010: 6865 2062 7920 6465 6661 756c 7420 6275  he by default bu
+00003020: 7420 7573 6520 7468 6520 6361 6368 6520  t use the cache 
+00003030: 6f66 2074 6865 2070 6172 656e 7420 4461  of the parent Da
+00003040: 7461 206f 626a 6563 742e 0a20 2020 2020  ta object..     
+00003050: 2020 2023 2055 7365 2075 7365 5f63 6163     # Use use_cac
+00003060: 6865 206d 6574 686f 6420 746f 2061 6374  he method to act
+00003070: 6976 6174 6520 6361 6368 696e 672e 0a20  ivate caching.. 
+00003080: 2020 2020 2020 2023 2041 6674 6572 2074         # After t
+00003090: 6861 742c 2074 6865 2044 6174 6120 6f62  hat, the Data ob
+000030a0: 6a65 6374 2077 696c 6c20 6372 6561 7465  ject will create
+000030b0: 2069 7473 206f 776e 2063 6163 6865 2066   its own cache f
+000030c0: 696c 652e 0a20 2020 2020 2020 2065 7665  ile..        eve
+000030d0: 6e74 735f 6669 6c74 6572 6564 2e75 7365  nts_filtered.use
+000030e0: 5f63 6163 6865 2829 0a20 2020 2020 2020  _cache().       
+000030f0: 200a 2020 2020 2020 2020 6c69 7374 280a   .        list(.
+00003100: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00003110: 7473 5f66 696c 7465 7265 6429 2020 2320  ts_filtered)  # 
+00003120: 4a75 7374 2074 6f20 6974 6572 6174 6520  Just to iterate 
+00003130: 4461 7461 206f 626a 6563 7420 2863 6163  Data object (cac
+00003140: 6865 2066 696c 6520 7769 6c6c 2062 6520  he file will be 
+00003150: 6372 6561 7465 6429 2e0a 2020 2020 2020  created)..      
+00003160: 2020 0a20 2020 2020 2020 2066 696c 7465    .        filte
+00003170: 7265 645f 6576 656e 7473 5f74 7970 6573  red_events_types
+00003180: 203d 2065 7665 6e74 735f 6669 6c74 6572   = events_filter
+00003190: 6564 2e6d 6170 280a 2020 2020 2020 2020  ed.map(.        
+000031a0: 2020 2020 6c61 6d62 6461 2072 6563 6f72      lambda recor
+000031b0: 643a 207b 2265 7665 6e74 5479 7065 223a  d: {"eventType":
+000031c0: 2072 6563 6f72 642e 6765 7428 2265 7665   record.get("eve
+000031d0: 6e74 5479 7065 2229 7d29 0a20 2020 2020  ntType")}).     
+000031e0: 2020 200a 2020 2020 2020 2020 6576 656e     .        even
+000031f0: 7473 5f77 6974 686f 7574 5f74 7970 6573  ts_without_types
+00003200: 5f77 6974 685f 6261 7463 6820 3d20 6669  _with_batch = fi
+00003210: 6c74 6572 6564 5f65 7665 6e74 735f 7479  ltered_events_ty
+00003220: 7065 732e 6669 6c74 6572 280a 2020 2020  pes.filter(.    
+00003230: 2020 2020 2020 2020 6c61 6d62 6461 2072          lambda r
+00003240: 6563 6f72 643a 206e 6f74 2072 6563 6f72  ecord: not recor
+00003250: 642e 6765 7428 2265 7665 6e74 5479 7065  d.get("eventType
+00003260: 2229 0a20 2020 2020 2020 2029 0a20 2020  ").        ).   
+00003270: 2020 2020 2065 7665 6e74 735f 7769 7468       events_with
+00003280: 6f75 745f 7479 7065 735f 7769 7468 5f62  out_types_with_b
+00003290: 6174 6368 2e75 7365 5f63 6163 6865 2829  atch.use_cache()
+000032a0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000032b0: 2020 2320 5b31 2e31 315d 2044 6174 6120    # [1.11] Data 
+000032c0: 6f62 6a65 6374 7320 6a6f 696e 696e 672e  objects joining.
+000032d0: 0a20 2020 2020 2020 2023 2059 6f75 2068  .        # You h
+000032e0: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
+000032f0: 6720 3320 4461 7461 206f 626a 6563 7473  g 3 Data objects
+00003300: 2e0a 2020 2020 2020 2020 6431 203d 2044  ..        d1 = D
+00003310: 6174 6128 5b31 2c20 322c 2033 5d29 0a20  ata([1, 2, 3]). 
+00003320: 2020 2020 2020 2064 3220 3d20 4461 7461         d2 = Data
+00003330: 285b 2261 222c 207b 2269 6422 3a20 3132  (["a", {"id": 12
+00003340: 337d 2c20 2263 225d 290a 2020 2020 2020  3}, "c"]).      
+00003350: 2020 6433 203d 2044 6174 6128 5b37 2c20    d3 = Data([7, 
+00003360: 382c 2039 5d29 0a20 2020 2020 2020 2023  8, 9]).        #
+00003370: 2059 6f75 2063 616e 206a 6f69 6e20 4461   You can join Da
+00003380: 7461 206f 626a 6563 7473 2069 6e20 666f  ta objects in fo
+00003390: 6c6c 6f77 696e 6720 7761 7973 2e0a 2020  llowing ways..  
+000033a0: 2020 2020 2020 2320 506c 6561 7365 206e        # Please n
+000033b0: 6f74 652c 206e 6577 2044 6174 6120 6f62  ote, new Data ob
+000033c0: 6a65 6374 2077 696c 6c20 6861 7665 2063  ject will have c
+000033d0: 6163 6865 2073 7461 7475 7320 3d3d 2046  ache status == F
+000033e0: 616c 7365 2e0a 2020 2020 2020 2020 6461  alse..        da
+000033f0: 7461 5f76 6961 5f69 6e69 7420 3d20 4461  ta_via_init = Da
+00003400: 7461 285b 6431 2c20 6432 2c20 6433 5d29  ta([d1, d2, d3])
+00003410: 0a20 2020 2020 2020 2064 6174 615f 7669  .        data_vi
+00003420: 615f 6164 6420 3d20 6431 202b 2064 3220  a_add = d1 + d2 
+00003430: 2b20 6433 0a20 2020 2020 2020 2064 6174  + d3.        dat
+00003440: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00003450: 6f62 6a5f 7669 615f 696e 6974 203d 2044  obj_via_init = D
+00003460: 6174 6128 5b64 312c 205b 2261 222c 207b  ata([d1, ["a", {
+00003470: 2269 6422 3a20 3132 337d 2c20 2263 225d  "id": 123}, "c"]
+00003480: 2c20 6433 5d29 0a20 2020 2020 2020 2064  , d3]).        d
+00003490: 6174 615f 7769 7468 5f6e 6f6e 5f64 6174  ata_with_non_dat
+000034a0: 615f 6f62 6a5f 7669 615f 6164 6420 3d20  a_obj_via_add = 
+000034b0: 6431 202b 205b 2261 222c 207b 2269 6422  d1 + ["a", {"id"
+000034c0: 3a20 3132 337d 2c20 2263 225d 202b 2064  : 123}, "c"] + d
+000034d0: 330a 2020 2020 2020 2020 2320 596f 7520  3.        # You 
+000034e0: 6361 6e20 6a6f 696e 2063 7572 7265 6e74  can join current
+000034f0: 2044 6174 6120 6f62 6a65 6374 206f 6e20   Data object on 
+00003500: 706c 6163 6520 7573 696e 6720 2b3d 2e0a  place using +=..
+00003510: 2020 2020 2020 2020 2320 4974 2077 696c          # It wil
+00003520: 6c20 6b65 6570 2063 6163 6865 2073 7461  l keep cache sta
+00003530: 7475 732e 0a20 2020 2020 2020 2064 3120  tus..        d1 
+00003540: 2b3d 2064 3320 2023 2064 3120 7769 6c6c  += d3  # d1 will
+00003550: 2062 6563 6f6d 6520 4461 7461 285b 312c   become Data([1,
+00003560: 322c 332c 372c 382c 395d 290a 2020 2020  2,3,7,8,9]).    
+00003570: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00003580: 312e 3132 5d20 4275 696c 6420 616e 6420  1.12] Build and 
+00003590: 7265 6164 2044 6174 6120 6f62 6a65 6374  read Data object
+000035a0: 2063 6163 6865 2066 696c 6573 2e0a 2020   cache files..  
+000035b0: 2020 2020 2020 6576 656e 7473 2e62 7569        events.bui
+000035c0: 6c64 5f63 6163 6865 2822 6361 6368 655f  ld_cache("cache_
+000035d0: 6669 6c65 6e61 6d65 5f6f 725f 7061 7468  filename_or_path
+000035e0: 2229 0a20 2020 2020 2020 2064 6174 615f  ").        data_
+000035f0: 6f62 6a5f 6672 6f6d 5f63 6163 6865 203d  obj_from_cache =
+00003600: 2044 6174 612e 6672 6f6d 5f63 6163 6865   Data.from_cache
+00003610: 5f66 696c 6528 2263 6163 6865 5f66 696c  _file("cache_fil
+00003620: 656e 616d 655f 6f72 5f70 6174 6822 290a  ename_or_path").
+00003630: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003640: 2023 205b 312e 3133 5d20 4368 6563 6b20   # [1.13] Check 
+00003650: 6966 2044 6174 6120 6973 2073 6f72 7465  if Data is sorte
+00003660: 642e 0a20 2020 2020 2020 2023 2054 6861  d..        # Tha
+00003670: 7420 7769 6c6c 2072 6574 7572 6e20 616e  t will return an
+00003680: 206f 626a 6563 7420 6069 735f 736f 7274   object `is_sort
+00003690: 6564 6020 7468 6174 2063 6f6e 7461 696e  ed` that contain
+000036a0: 7320 696e 666f 726d 6174 696f 6e0a 2020  s information.  
+000036b0: 2020 2020 2020 2320 2020 312e 2073 7461        #   1. sta
+000036c0: 7475 7320 2d2d 2073 6f72 7465 6420 6f72  tus -- sorted or
+000036d0: 206e 6f74 0a20 2020 2020 2020 2023 2020   not.        #  
+000036e0: 2032 2e20 6669 7273 745f 756e 736f 7274   2. first_unsort
+000036f0: 6564 202d 2d20 7468 6520 696e 6465 7820  ed -- the index 
+00003700: 6f66 2074 6865 2066 6972 7374 2075 6e73  of the first uns
+00003710: 6f72 7465 6420 656c 656d 656e 740a 2020  orted element.  
+00003720: 2020 2020 2020 6973 5f73 6f72 7465 6420        is_sorted 
+00003730: 3d20 6576 656e 7473 2e69 735f 736f 7274  = events.is_sort
+00003740: 6564 286c 616d 6264 6120 653a 2065 5b22  ed(lambda e: e["
+00003750: 7374 6172 7454 696d 6573 7461 6d70 225d  startTimestamp"]
+00003760: 5b22 6570 6f63 6853 6563 6f6e 6422 5d29  ["epochSecond"])
+00003770: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003780: 2020 2320 596f 7520 6361 6e20 7573 6520    # You can use 
+00003790: 7468 6973 206f 626a 6563 7420 6173 2075  this object as u
+000037a0: 7375 616c 2062 6f6f 6c20 7661 7269 6162  sual bool variab
+000037b0: 6c65 2e0a 2020 2020 2020 2020 6966 2069  le..        if i
+000037c0: 735f 736f 7274 6564 3a0a 2020 2020 2020  s_sorted:.      
+000037d0: 2020 2020 2020 7072 696e 7428 2265 7665        print("eve
+000037e0: 6e74 7320 4461 7461 206f 626a 2069 7320  nts Data obj is 
+000037f0: 736f 7274 6564 2122 290a 2020 2020 2020  sorted!").      
+00003800: 2020 0a20 2020 2020 2020 2023 205b 312e    .        # [1.
+00003810: 3134 5d20 5573 6520 6044 6174 612e 7368  14] Use `Data.sh
+00003820: 6f77 2829 6020 746f 206c 6f6f 6b20 6174  ow()` to look at
+00003830: 2074 6865 2066 6972 7374 204e 206d 6573   the first N mes
+00003840: 7361 6765 7320 696e 2074 6865 2073 7472  sages in the str
+00003850: 6561 6d2e 0a20 2020 2020 2020 2064 6174  eam..        dat
+00003860: 615f 7769 7468 5f6e 6f6e 5f64 6174 615f  a_with_non_data_
+00003870: 6f62 6a5f 7669 615f 6164 642e 7368 6f77  obj_via_add.show
+00003880: 286e 3d36 290a 2020 2020 2020 2020 2320  (n=6).        # 
+00003890: 5769 6c6c 2070 7269 6e74 0a20 2020 2020  Will print.     
+000038a0: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+000038b0: 2d2d 2050 7269 6e74 6564 2066 6972 7374  -- Printed first
+000038c0: 2036 2072 6563 6f72 6473 202d 2d2d 2d2d   6 records -----
+000038d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000038e0: 2023 205b 315d 202d 2d2d 2d2d 2d0a 2020   # [1] ------.  
+000038f0: 2020 2020 2020 2320 310a 2020 2020 2020        # 1.      
+00003900: 2020 2320 5b32 5d20 2d2d 2d2d 2d2d 0a20    # [2] ------. 
+00003910: 2020 2020 2020 2023 2032 0a20 2020 2020         # 2.     
+00003920: 2020 2023 205b 335d 202d 2d2d 2d2d 2d0a     # [3] ------.
+00003930: 2020 2020 2020 2020 2320 330a 2020 2020          # 3.    
+00003940: 2020 2020 2320 5b34 5d20 2d2d 2d2d 2d2d      # [4] ------
+00003950: 0a20 2020 2020 2020 2023 2027 6127 0a20  .        # 'a'. 
+00003960: 2020 2020 2020 2023 205b 355d 202d 2d2d         # [5] ---
+00003970: 2d2d 2d0a 2020 2020 2020 2020 2320 7b27  ---.        # {'
+00003980: 6964 273a 2031 3233 7d0a 2020 2020 2020  id': 123}.      
+00003990: 2020 2320 5b36 5d20 2d2d 2d2d 2d2d 0a20    # [6] ------. 
+000039a0: 2020 2020 2020 2023 2027 6327 0a20 2020         # 'c'.   
+000039b0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+000039c0: 5b31 2e31 355d 2059 6f75 2063 616e 2072  [1.15] You can r
+000039d0: 656d 6f76 6520 7468 6520 6361 6368 6520  emove the cache 
+000039e0: 6669 6c65 206f 6620 7468 6520 4461 7461  file of the Data
+000039f0: 206f 626a 6563 742c 2069 6620 7265 7175   object, if requ
+00003a00: 6972 6564 2e0a 2020 2020 2020 2020 6461  ired..        da
+00003a10: 7461 5f6f 626a 5f66 726f 6d5f 6361 6368  ta_obj_from_cach
+00003a20: 652e 636c 6561 725f 6361 6368 6528 290a  e.clear_cache().
+00003a30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00003a40: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00003a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003a60: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00003a70: 2320 5b32 5d20 576f 726b 696e 6720 7769  # [2] Working wi
+00003a80: 7468 2063 6f6e 7665 7274 6572 732e 0a20  th converters.. 
+00003a90: 2020 2020 2020 2023 2323 2323 2323 2323         #########
+00003aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003ab0: 2323 2323 2323 2323 2323 2323 230a 2020  #############.  
+00003ac0: 2020 2020 2020 2320 5468 6572 6520 6172        # There ar
+00003ad0: 6520 6375 7272 656e 746c 7920 7468 7265  e currently thre
+00003ae0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00003af0: 7320 6f66 2049 5469 6d65 7374 616d 7043  s of ITimestampC
+00003b00: 6f6e 7665 7274 6572 2063 6c61 7373 3a20  onverter class: 
+00003b10: 4461 7465 7469 6d65 436f 6e76 6572 7465  DatetimeConverte
+00003b20: 2c20 4461 7465 7469 6d65 5374 7269 6e67  , DatetimeString
+00003b30: 436f 6e76 6572 7465 7220 616e 6420 5072  Converter and Pr
+00003b40: 6f74 6f62 7566 5469 6d65 7374 616d 7043  otobufTimestampC
+00003b50: 6f6e 7665 7274 6572 2e0a 2020 2020 2020  onverter..      
+00003b60: 2020 2320 5468 6579 2061 6c6c 2069 6d70    # They all imp
+00003b70: 6c65 6d65 6e74 2073 616d 6520 6d65 7468  lement same meth
+00003b80: 6f64 7320 6672 6f6d 2062 6173 6520 636c  ods from base cl
+00003b90: 6173 732e 0a20 2020 2020 2020 2023 204e  ass..        # N
+00003ba0: 6f74 6520 7468 6174 2073 6f6d 6520 6163  ote that some ac
+00003bb0: 6375 7261 6379 206d 6179 2062 6520 6c6f  curacy may be lo
+00003bc0: 7374 2064 7572 696e 6720 636f 6e76 6572  st during conver
+00003bd0: 7369 6f6e 2e0a 2020 2020 2020 2020 2320  sion..        # 
+00003be0: 4966 2066 6f72 2065 7861 6d70 6c65 2079  If for example y
+00003bf0: 6f75 2075 7365 2074 6f5f 6d69 6372 6f73  ou use to_micros
+00003c00: 6563 6f6e 6473 206e 616e 6f73 6563 6f6e  econds nanosecon
+00003c10: 6473 2077 696c 6c20 6265 2063 7574 206f  ds will be cut o
+00003c20: 6666 2069 6e73 7465 6164 206f 6620 726f  ff instead of ro
+00003c30: 756e 6469 6e67 2e0a 2020 2020 2020 2020  unding..        
+00003c40: 0a20 2020 2020 2020 2023 205b 322e 315d  .        # [2.1]
+00003c50: 2044 6174 6574 696d 6543 6f6e 7665 7274   DatetimeConvert
+00003c60: 6572 2e0a 2020 2020 2020 2020 2320 4461  er..        # Da
+00003c70: 7465 7469 6d65 436f 6e76 6572 7465 7220  tetimeConverter 
+00003c80: 7461 6b65 7320 6461 7465 7469 6d65 2e64  takes datetime.d
+00003c90: 6174 6574 696d 6520 6f62 6a65 6374 2061  atetime object a
+00003ca0: 7320 696e 7075 742e 0a20 2020 2020 2020  s input..       
+00003cb0: 200a 2020 2020 2020 2020 6461 7465 7469   .        dateti
+00003cc0: 6d65 5f6f 626a 203d 2064 6174 6574 696d  me_obj = datetim
+00003cd0: 6528 7965 6172 3d32 3032 332c 206d 6f6e  e(year=2023, mon
+00003ce0: 7468 3d31 2c20 6461 793d 352c 2068 6f75  th=1, day=5, hou
+00003cf0: 723d 3134 2c20 6d69 6e75 7465 3d33 382c  r=14, minute=38,
+00003d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d20: 2073 6563 6f6e 643d 3235 2c20 6d69 6372   second=25, micr
+00003d30: 6f73 6563 6f6e 643d 3134 3630 290a 2020  osecond=1460).  
+00003d40: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00003d50: 2049 7420 6861 7320 6d65 7468 6f64 7320   It has methods 
+00003d60: 7468 6174 2072 6574 7572 6e20 7468 6520  that return the 
+00003d70: 6461 7465 7469 6d65 2069 6e20 6469 6666  datetime in diff
+00003d80: 6572 656e 7420 666f 726d 6173 3a0a 2020  erent formas:.  
+00003d90: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
+00003da0: 6174 655f 6d73 203d 2044 6174 6574 696d  ate_ms = Datetim
+00003db0: 6543 6f6e 7665 7274 6572 2e74 6f5f 6d69  eConverter.to_mi
+00003dc0: 6c6c 6973 6563 6f6e 6473 2864 6174 6574  lliseconds(datet
+00003dd0: 696d 655f 6f62 6a29 0a20 2020 2020 2020  ime_obj).       
+00003de0: 2064 6174 655f 7573 203d 2044 6174 6574   date_us = Datet
+00003df0: 696d 6543 6f6e 7665 7274 6572 2e74 6f5f  imeConverter.to_
+00003e00: 6d69 6372 6f73 6563 6f6e 6473 2864 6174  microseconds(dat
+00003e10: 6574 696d 655f 6f62 6a29 0a20 2020 2020  etime_obj).     
+00003e20: 2020 2023 2043 6f6e 7665 7274 696e 6720     # Converting 
+00003e30: 746f 206e 616e 6f73 6563 6f6e 6473 206a  to nanoseconds j
+00003e40: 7573 7473 2061 6464 7320 7468 7265 6520  usts adds three 
+00003e50: 7472 6169 6c69 6e67 207a 6572 6f73 2061  trailing zeros a
+00003e60: 7320 6461 7465 7469 6d65 206f 626a 6563  s datetime objec
+00003e70: 7420 646f 6573 6e27 7420 6861 7665 206e  t doesn't have n
+00003e80: 616e 6f73 6563 6f6e 6473 2e0a 2020 2020  anoseconds..    
+00003e90: 2020 2020 6461 7465 5f6e 7320 3d20 4461      date_ns = Da
+00003ea0: 7465 7469 6d65 436f 6e76 6572 7465 722e  tetimeConverter.
+00003eb0: 746f 5f6e 616e 6f73 6563 6f6e 6473 2864  to_nanoseconds(d
+00003ec0: 6174 6574 696d 655f 6f62 6a29 0a20 2020  atetime_obj).   
+00003ed0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00003ee0: 5b32 2e32 5d20 4461 7465 7469 6d65 5374  [2.2] DatetimeSt
+00003ef0: 7269 6e67 436f 6e76 6572 7465 720a 2020  ringConverter.  
+00003f00: 2020 2020 2020 2320 4461 7465 7469 6d65        # Datetime
+00003f10: 5374 7269 6e67 436f 6e76 6572 7465 7220  StringConverter 
+00003f20: 7461 6b65 7320 7374 7269 6e67 2069 6e20  takes string in 
+00003f30: 2279 7979 792d 4d4d 2d64 6454 4848 3a6d  "yyyy-MM-ddTHH:m
+00003f40: 6d3a 7373 5b2e 5353 5353 5353 5353 535d  m:ss[.SSSSSSSSS]
+00003f50: 5a22 2066 6f72 6d61 742e 0a20 2020 2020  Z" format..     
+00003f60: 2020 200a 2020 2020 2020 2020 6461 7465     .        date
+00003f70: 5f73 7472 696e 6720 3d20 2232 3032 332d  _string = "2023-
+00003f80: 3031 2d30 3554 3134 3a33 383a 3235 2e30  01-05T14:38:25.0
+00003f90: 3031 3436 5a22 0a20 2020 2020 2020 200a  0146Z".        .
+00003fa0: 2020 2020 2020 2020 2320 5765 2068 6176          # We hav
+00003fb0: 6520 7361 6d65 206d 6574 686f 6473 2061  e same methods a
+00003fc0: 7320 696e 2044 6174 6574 696d 6543 6f6e  s in DatetimeCon
+00003fd0: 7665 7274 6572 0a20 2020 2020 2020 2064  verter.        d
+00003fe0: 6174 655f 6d73 5f66 726f 6d5f 7374 7269  ate_ms_from_stri
+00003ff0: 6e67 203d 2044 6174 6574 696d 6553 7472  ng = DatetimeStr
+00004000: 696e 6743 6f6e 7665 7274 6572 2e74 6f5f  ingConverter.to_
+00004010: 6d69 6c6c 6973 6563 6f6e 6473 2864 6174  milliseconds(dat
+00004020: 655f 7374 7269 6e67 290a 2020 2020 2020  e_string).      
+00004030: 2020 6461 7465 5f75 735f 6672 6f6d 5f73    date_us_from_s
+00004040: 7472 696e 6720 3d20 4461 7465 7469 6d65  tring = Datetime
+00004050: 5374 7269 6e67 436f 6e76 6572 7465 722e  StringConverter.
+00004060: 746f 5f6d 6963 726f 7365 636f 6e64 7328  to_microseconds(
+00004070: 6461 7465 5f73 7472 696e 6729 0a20 2020  date_string).   
+00004080: 2020 2020 2064 6174 655f 6e73 5f66 726f       date_ns_fro
+00004090: 6d5f 7374 7269 6e67 203d 2044 6174 6574  m_string = Datet
+000040a0: 696d 6553 7472 696e 6743 6f6e 7665 7274  imeStringConvert
+000040b0: 6572 2e74 6f5f 6e61 6e6f 7365 636f 6e64  er.to_nanosecond
+000040c0: 7328 6461 7465 5f73 7472 696e 6729 0a20  s(date_string). 
+000040d0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000040e0: 2320 5765 2063 616e 2061 6c73 6f20 6765  # We can also ge
+000040f0: 7420 6461 7465 7469 6d65 206f 626a 6563  t datetime objec
+00004100: 7420 6672 6f6d 2073 7472 696e 670a 2020  t from string.  
+00004110: 2020 2020 2020 6461 7465 7469 6d65 5f66        datetime_f
+00004120: 726f 6d5f 7374 7269 6e67 203d 2044 6174  rom_string = Dat
+00004130: 6574 696d 6553 7472 696e 6743 6f6e 7665  etimeStringConve
+00004140: 7274 6572 2e74 6f5f 6461 7465 7469 6d65  rter.to_datetime
+00004150: 2864 6174 655f 7374 7269 6e67 290a 2020  (date_string).  
+00004160: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004170: 205b 322e 335d 2050 726f 746f 6275 6654   [2.3] ProtobufT
+00004180: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+00004190: 720a 2020 2020 2020 2020 2320 5072 6f74  r.        # Prot
+000041a0: 6f62 7566 2074 696d 6573 7461 6d70 7320  obuf timestamps 
+000041b0: 6d75 7374 2062 6520 696e 2066 6f72 6d20  must be in form 
+000041c0: 7b22 6570 6f63 6853 6563 6f6e 6422 3a20  {"epochSecond": 
+000041d0: 7365 636f 6e64 732c 2022 6e61 6e6f 223a  seconds, "nano":
+000041e0: 206e 616e 6f73 6563 6f6e 6473 7d0a 2020   nanoseconds}.  
+000041f0: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00004200: 726f 746f 6275 665f 7469 6d65 7374 616d  rotobuf_timestam
+00004210: 7020 3d20 7b22 6570 6f63 6853 6563 6f6e  p = {"epochSecon
+00004220: 6422 3a20 3136 3732 3932 3935 3035 2c20  d": 1672929505, 
+00004230: 226e 616e 6f22 3a20 315f 3436 305f 3030  "nano": 1_460_00
+00004240: 307d 0a20 2020 2020 2020 200a 2020 2020  0}.        .    
+00004250: 2020 2020 6461 7465 5f6d 735f 6672 6f6d      date_ms_from
+00004260: 5f74 696d 6573 7461 6d70 203d 2050 726f  _timestamp = Pro
+00004270: 746f 6275 6654 696d 6573 7461 6d70 436f  tobufTimestampCo
+00004280: 6e76 6572 7465 722e 746f 5f6d 696c 6c69  nverter.to_milli
+00004290: 7365 636f 6e64 7328 0a20 2020 2020 2020  seconds(.       
+000042a0: 2020 2020 2070 726f 746f 6275 665f 7469       protobuf_ti
+000042b0: 6d65 7374 616d 7029 0a20 2020 2020 2020  mestamp).       
+000042c0: 2064 6174 655f 7573 5f66 726f 6d5f 7469   date_us_from_ti
+000042d0: 6d65 7374 616d 7020 3d20 5072 6f74 6f62  mestamp = Protob
+000042e0: 7566 5469 6d65 7374 616d 7043 6f6e 7665  ufTimestampConve
+000042f0: 7274 6572 2e74 6f5f 6d69 6372 6f73 6563  rter.to_microsec
+00004300: 6f6e 6473 280a 2020 2020 2020 2020 2020  onds(.          
+00004310: 2020 7072 6f74 6f62 7566 5f74 696d 6573    protobuf_times
+00004320: 7461 6d70 290a 2020 2020 2020 2020 6461  tamp).        da
+00004330: 7465 5f6e 735f 6672 6f6d 5f74 696d 6573  te_ns_from_times
+00004340: 7461 6d70 203d 2050 726f 746f 6275 6654  tamp = ProtobufT
+00004350: 696d 6573 7461 6d70 436f 6e76 6572 7465  imestampConverte
+00004360: 722e 746f 5f6e 616e 6f73 6563 6f6e 6473  r.to_nanoseconds
+00004370: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
+00004380: 6f74 6f62 7566 5f74 696d 6573 7461 6d70  otobuf_timestamp
+00004390: 290a 2020 2020 2020 2020 6461 7465 7469  ).        dateti
+000043a0: 6d65 5f66 726f 6d5f 7469 6d65 7374 616d  me_from_timestam
+000043b0: 7020 3d20 5072 6f74 6f62 7566 5469 6d65  p = ProtobufTime
+000043c0: 7374 616d 7043 6f6e 7665 7274 6572 2e74  stampConverter.t
+000043d0: 6f5f 6461 7465 7469 6d65 280a 2020 2020  o_datetime(.    
+000043e0: 2020 2020 2020 2020 7072 6f74 6f62 7566          protobuf
+000043f0: 5f74 696d 6573 7461 6d70 290a 2020 2020  _timestamp).    
+00004400: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00004410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004430: 2323 230a 2020 2020 2020 2020 2320 5b33  ###.        # [3
+00004440: 5d20 576f 726b 696e 6720 7769 7468 2045  ] Working with E
+00004450: 7665 6e74 5472 6565 2061 6e64 2045 7665  ventTree and Eve
+00004460: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00004470: 2e0a 2020 2020 2020 2020 2323 2323 2323  ..        ######
+00004480: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004490: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000044a0: 0a20 2020 2020 2020 2023 2043 616e 2062  .        # Can b
+000044b0: 6520 7573 6566 756c 2069 6620 796f 7520  e useful if you 
+000044c0: 6861 7665 2064 6174 612d 7374 7265 616d  have data-stream
+000044d0: 2077 6974 6820 3c20 3130 306b 2065 6c65   with < 100k ele
+000044e0: 6d65 6e74 732c 206f 7468 6572 7769 7365  ments, otherwise
+000044f0: 2069 740a 2020 2020 2020 2020 2320 7461   it.        # ta
+00004500: 6b65 7320 746f 6f20 6d75 6368 2052 414d  kes too much RAM
+00004510: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00004520: 2020 2023 205b 332e 315d 2042 7569 6c64     # [3.1] Build
+00004530: 2061 2063 7573 746f 6d20 4576 656e 7454   a custom EventT
+00004540: 7265 650a 2020 2020 2020 2020 2320 546f  ree.        # To
+00004550: 2063 7265 6174 6520 616e 2045 7665 6e74   create an Event
+00004560: 5472 6565 206f 626a 6563 7420 796f 7520  Tree object you 
+00004570: 6e65 6564 2074 6f20 7072 6f76 6964 6520  need to provide 
+00004580: 6e61 6d65 2c20 6964 2061 6e64 2064 6174  name, id and dat
+00004590: 6120 6f66 2074 6865 2072 6f6f 7420 6576  a of the root ev
+000045a0: 656e 742e 0a20 2020 2020 2020 2074 7265  ent..        tre
+000045b0: 6520 3d20 4576 656e 7454 7265 6528 6576  e = EventTree(ev
+000045c0: 656e 745f 6e61 6d65 3d22 726f 6f74 2065  ent_name="root e
+000045d0: 7665 6e74 222c 2065 7665 6e74 5f69 643d  vent", event_id=
+000045e0: 2272 6f6f 745f 6964 222c 0a20 2020 2020  "root_id",.     
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 6461 7461 3d7b 2264 6174 6122      data={"data"
+00004610: 3a20 5b31 2c20 322c 2033 2c20 342c 2035  : [1, 2, 3, 4, 5
+00004620: 5d7d 290a 2020 2020 2020 2020 0a20 2020  ]}).        .   
+00004630: 2020 2020 2023 2054 6f20 6164 6420 6e65       # To add ne
+00004640: 7720 6e6f 6465 2075 7365 2061 7070 656e  w node use appen
+00004650: 645f 6576 656e 742e 2070 6172 656e 745f  d_event. parent_
+00004660: 6964 2069 7320 6e65 6365 7373 6172 792c  id is necessary,
+00004670: 2064 6174 6120 6973 206f 7074 696f 6e61   data is optiona
+00004680: 6c2e 0a20 2020 2020 2020 2074 7265 652e  l..        tree.
+00004690: 6170 7065 6e64 5f65 7665 6e74 2865 7665  append_event(eve
+000046a0: 6e74 5f6e 616d 653d 2241 222c 2065 7665  nt_name="A", eve
+000046b0: 6e74 5f69 643d 2241 5f69 6422 2c20 6461  nt_id="A_id", da
+000046c0: 7461 3d4e 6f6e 652c 0a20 2020 2020 2020  ta=None,.       
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2070 6172 656e 745f 6964 3d22 726f     parent_id="ro
+000046f0: 6f74 5f69 6422 290a 2020 2020 2020 2020  ot_id").        
+00004700: 0a20 2020 2020 2020 2023 205b 332e 335d  .        # [3.3]
+00004710: 2042 7569 6c64 696e 6720 7468 6520 4576   Building the Ev
+00004720: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00004730: 6e2e 0a20 2020 2020 2020 2064 6174 615f  n..        data_
+00004740: 736f 7572 6365 3a20 4944 6174 6153 6f75  source: IDataSou
+00004750: 7263 6520 2023 2059 6f75 2073 686f 756c  rce  # You shoul
+00004760: 6420 696e 6974 2044 6174 6153 6f75 7263  d init DataSourc
+00004770: 6520 6f62 6a65 6374 2e20 452e 672e 2066  e object. E.g. f
+00004780: 726f 6d20 4c77 4450 206d 6f64 756c 652e  rom LwDP module.
+00004790: 0a20 2020 2020 2020 2064 6174 615f 736f  .        data_so
+000047a0: 7572 6365 203d 2044 756d 6d79 4461 7461  urce = DummyData
+000047b0: 536f 7572 6365 2829 2020 2320 4e6f 7465  Source()  # Note
+000047c0: 2120 5765 2075 7365 2066 616b 6520 4453  ! We use fake DS
+000047d0: 2068 6572 652e 0a20 2020 2020 2020 2023   here..        #
+000047e0: 2045 5443 4472 6976 6572 2068 6572 6520   ETCDriver here 
+000047f0: 6973 2061 2073 7475 622c 2061 6374 7561  is a stub, actua
+00004800: 6c6c 7920 7468 6520 6c69 6220 646f 6573  lly the lib does
+00004810: 6e27 7420 6861 7665 2073 7563 6820 6120  n't have such a 
+00004820: 636c 6173 732e 0a20 2020 2020 2020 2023  class..        #
+00004830: 2059 6f75 2063 616e 2074 616b 6520 6974   You can take it
+00004840: 2069 6e20 4c77 4450 206d 6f64 756c 6520   in LwDP module 
+00004850: 6f72 2063 7265 6174 6520 796f 7572 7365  or create yourse
+00004860: 6c66 2063 6c61 7373 2069 6620 796f 7520  lf class if you 
+00004870: 6861 7665 2073 6f6d 6520 7370 6563 6961  have some specia
+00004880: 6c20 6576 656e 7473 2073 7472 7563 7475  l events structu
+00004890: 7265 2e0a 2020 2020 2020 2020 6672 6f6d  re..        from
+000048a0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+000048b0: 6573 2e64 6174 615f 736f 7572 6365 2e6c  es.data_source.l
+000048c0: 7764 702e 6576 656e 745f 7472 6565 2069  wdp.event_tree i
+000048d0: 6d70 6f72 740a 2020 2020 2020 2020 0a20  mport.        . 
+000048e0: 2020 2020 2020 2048 7474 7045 5443 4472         HttpETCDr
+000048f0: 6976 6572 2061 7320 4554 4344 7269 7665  iver as ETCDrive
+00004900: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00004910: 2020 2023 2049 6620 796f 7520 646f 6e27     # If you don'
+00004920: 7420 7370 6563 6966 7920 6461 7461 5f73  t specify data_s
+00004930: 6f75 7263 6520 666f 7220 7468 6520 6472  ource for the dr
+00004940: 6976 6572 2074 6865 6e20 6974 2077 6f6e  iver then it won
+00004950: 2774 2072 6563 6f76 6572 2064 6574 6163  't recover detac
+00004960: 6865 6420 6576 656e 7473 2e0a 2020 2020  hed events..    
+00004970: 2020 2020 6472 6976 6572 3a20 4945 5443      driver: IETC
+00004980: 4472 6976 6572 2020 2320 596f 7520 7368  Driver  # You sh
+00004990: 6f75 6c64 2069 6e69 7420 4554 4344 7269  ould init ETCDri
+000049a0: 7665 7220 6f62 6a65 6374 2e20 452e 672e  ver object. E.g.
+000049b0: 2066 726f 6d20 4c77 4450 206d 6f64 756c   from LwDP modul
+000049c0: 6520 6f72 2079 6f75 7220 6375 7374 6f6d  e or your custom
+000049d0: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
+000049e0: 6472 6976 6572 203d 2045 5443 4472 6976  driver = ETCDriv
+000049f0: 6572 2864 6174 615f 736f 7572 6365 3d64  er(data_source=d
+00004a00: 6174 615f 736f 7572 6365 2c20 7573 655f  ata_source, use_
+00004a10: 7374 7562 3d54 7275 6529 0a20 2020 2020  stub=True).     
+00004a20: 2020 200a 2020 2020 2020 2020 6574 6320     .        etc 
+00004a30: 3d20 4576 656e 7454 7265 6543 6f6c 6c65  = EventTreeColle
+00004a40: 6374 696f 6e28 6472 6976 6572 290a 2020  ction(driver).  
+00004a50: 2020 2020 2020 6574 632e 6275 696c 6428        etc.build(
+00004a60: 6576 656e 7473 290a 2020 2020 2020 2020  events).        
+00004a70: 6574 632e 7368 6f77 2829 0a20 2020 2020  etc.show().     
+00004a80: 2020 2023 2049 7427 6c6c 2070 7269 6e74     # It'll print
+00004a90: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00004aa0: 2020 2020 2020 2020 2320 5365 7420 6f66          # Set of
+00004ab0: 2061 7574 6f2d 6765 6e65 7261 7465 6420   auto-generated 
+00004ac0: 6576 656e 7473 2066 6f72 2064 7320 6c69  events for ds li
+00004ad0: 6220 7465 7374 696e 670a 2020 2020 2020  b testing.      
+00004ae0: 2020 2320 e294 9ce2 9480 e294 8020 506c    # ......... Pl
+00004af0: 6169 6e20 6576 656e 7420 310a 2020 2020  ain event 1.    
+00004b00: 2020 2020 2320 e294 94e2 9480 e294 8020      # ......... 
+00004b10: 506c 6169 6e20 6576 656e 7420 320a 2020  Plain event 2.  
+00004b20: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00004b30: 7269 6e74 2865 7463 290a 2020 2020 2020  rint(etc).      
+00004b40: 2020 2320 4576 656e 7454 7265 6543 6f6c    # EventTreeCol
+00004b50: 6c65 6374 696f 6e28 7472 6565 733d 312c  lection(trees=1,
+00004b60: 2065 7665 6e74 733d 335b 7472 6565 733d   events=3[trees=
+00004b70: 332c 2064 6574 6163 6865 643d 305d 290a  3, detached=0]).
+00004b80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004b90: 2023 2044 6574 6163 6865 6420 6576 656e   # Detached even
+00004ba0: 7473 2069 736e 2774 2065 6d70 7479 2e0a  ts isn't empty..
+00004bb0: 2020 2020 2020 2020 6173 7365 7274 2065          assert e
+00004bc0: 7463 2e67 6574 5f64 6574 6163 6865 645f  tc.get_detached_
+00004bd0: 6576 656e 7473 2829 2020 2320 7265 7475  events()  # retu
+00004be0: 726e 7320 6c69 7374 206f 6620 6465 7461  rns list of deta
+00004bf0: 6368 6564 5f65 7665 6e74 732e 0a20 2020  ched_events..   
+00004c00: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00004c10: 7265 636f 7665 725f 756e 6b6e 6f77 6e5f  recover_unknown_
+00004c20: 6576 656e 7473 202d 2d20 7573 6564 2074  events -- used t
+00004c30: 6f20 7265 636f 7665 7220 736f 6d65 2065  o recover some e
+00004c40: 7665 6e74 7320 7061 7265 6e74 732e 0a20  vents parents.. 
+00004c50: 2020 2020 2020 2023 2054 6861 7420 776f         # That wo
+00004c60: 6e27 7420 776f 726b 2077 6974 6820 4475  n't work with Du
+00004c70: 6d6d 7944 6174 6153 6f75 7263 652c 2073  mmyDataSource, s
+00004c80: 6f20 7761 7320 636f 6d6d 656e 7465 640a  o was commented.
+00004c90: 2020 2020 2020 2020 2320 6574 632e 7265          # etc.re
+00004ca0: 636f 7665 725f 756e 6b6e 6f77 6e5f 6576  cover_unknown_ev
+00004cb0: 656e 7473 2829 0a20 2020 2020 2020 200a  ents().        .
+00004cc0: 2020 2020 2020 2020 2320 4166 7465 7220          # After 
+00004cd0: 7468 6174 2074 6865 2064 6574 6163 6865  that the detache
+00004ce0: 6420 6576 656e 7473 2073 686f 756c 6420  d events should 
+00004cf0: 6265 2065 6d70 7479 2062 6563 6175 7365  be empty because
+00004d00: 2074 6865 7920 7765 7265 2072 6563 6f76   they were recov
+00004d10: 6572 6564 2e0a 2020 2020 2020 2020 2320  ered..        # 
+00004d20: 6173 7365 7274 206e 6f74 2065 7463 2e67  assert not etc.g
+00004d30: 6574 5f64 6574 6163 6865 645f 6576 656e  et_detached_even
+00004d40: 7473 2829 0a20 2020 2020 2020 200a 2020  ts().        .  
+00004d50: 2020 2020 2020 2320 2d2d 2d2d 2d0a 2020        # -----.  
+00004d60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00004d70: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
+00004d80: 6861 7320 4576 656e 7454 7265 6573 2065  has EventTrees e
+00004d90: 6163 6820 7769 7468 2061 2074 7265 6520  ach with a tree 
+00004da0: 6f66 2065 7665 6e74 732e 0a20 2020 2020  of events..     
+00004db0: 2020 2023 2055 7369 6e67 2043 6f6c 6c65     # Using Colle
+00004dc0: 6374 696f 6e20 616e 6420 4576 656e 7454  ction and EventT
+00004dd0: 7265 6573 2c20 796f 7520 6361 6e20 776f  rees, you can wo
+00004de0: 726b 2066 6c65 7869 626c 7920 7769 7468  rk flexibly with
+00004df0: 2065 7665 6e74 732e 0a20 2020 2020 2020   events..       
+00004e00: 200a 2020 2020 2020 2020 2320 5b33 2e33   .        # [3.3
+00004e10: 2e31 5d20 4765 7420 6c65 6176 6573 206f  .1] Get leaves o
+00004e20: 6620 616c 6c20 7472 6565 732e 0a20 2020  f all trees..   
+00004e30: 2020 2020 206c 6561 7665 733a 2054 7570       leaves: Tup
+00004e40: 6c65 5b64 6963 745d 203d 2065 7463 2e67  le[dict] = etc.g
+00004e50: 6574 5f6c 6561 7665 7328 2920 2023 2052  et_leaves()  # R
+00004e60: 6574 7572 6e73 2061 2074 7570 6c65 206f  eturns a tuple o
+00004e70: 6620 6c65 6176 6573 2065 7665 6e74 730a  f leaves events.
+00004e80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004e90: 2023 205b 332e 332e 325d 2047 6574 2072   # [3.3.2] Get r
+00004ea0: 6f6f 7473 2069 6473 206f 6620 616c 6c20  oots ids of all 
+00004eb0: 7472 6565 732e 0a20 2020 2020 2020 2072  trees..        r
+00004ec0: 6f6f 7473 3a20 4c69 7374 5b73 7472 5d20  oots: List[str] 
+00004ed0: 3d20 6574 632e 6765 745f 726f 6f74 735f  = etc.get_roots_
+00004ee0: 6964 7328 290a 2020 2020 2020 2020 2320  ids().        # 
+00004ef0: 5265 7475 726e 7320 7468 6520 6c69 7374  Returns the list
+00004f00: 206f 6620 726f 6f74 2049 6473 3a0a 2020   of root Ids:.  
+00004f10: 2020 2020 2020 2320 5b27 6465 6d6f 5f62        # ['demo_b
+00004f20: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00004f30: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+00004f40: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+00004f50: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+00004f60: 6433 3461 3631 3535 3135 3264 5f31 275d  d34a6155152d_1']
+00004f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00004f80: 2020 2320 5b33 2e33 2e33 5d20 4669 6e64    # [3.3.3] Find
+00004f90: 2061 6e20 6576 656e 7420 696e 2061 6c6c   an event in all
+00004fa0: 2074 7265 6573 2e0a 2020 2020 2020 2020   trees..        
+00004fb0: 6669 6e64 5f65 7665 6e74 3a20 4f70 7469  find_event: Opti
+00004fc0: 6f6e 616c 5b64 6963 745d 203d 2065 7463  onal[dict] = etc
+00004fd0: 2e66 696e 6428 0a20 2020 2020 2020 2020  .find(.         
+00004fe0: 2020 206c 616d 6264 6120 6576 656e 743a     lambda event:
+00004ff0: 2022 5365 6e64 206d 6573 7361 6765 2220   "Send message" 
+00005000: 696e 2065 7665 6e74 5b22 6576 656e 7454  in event["eventT
+00005010: 7970 6522 5d29 0a20 2020 2020 2020 200a  ype"]).        .
+00005020: 2020 2020 2020 2020 2320 5b33 2e33 2e34          # [3.3.4
+00005030: 5d20 4669 6e64 2061 6c6c 2065 7665 6e74  ] Find all event
+00005040: 7320 696e 2061 6c6c 2074 7265 6573 2e20  s in all trees. 
+00005050: 5468 6572 6520 6973 2061 6c73 6f20 6974  There is also it
+00005060: 6572 6162 6c65 2076 6572 7369 6f6e 2027  erable version '
+00005070: 6669 6e64 616c 6c5f 6974 6572 272e 0a20  findall_iter'.. 
+00005080: 2020 2020 2020 2066 696e 645f 6576 656e         find_even
+00005090: 7473 3a20 4c69 7374 5b64 6963 745d 203d  ts: List[dict] =
+000050a0: 2065 7463 2e66 696e 6461 6c6c 286c 616d   etc.findall(lam
+000050b0: 6264 6120 6576 656e 743a 2065 7665 6e74  bda event: event
+000050c0: 5b22 7375 6363 6573 7366 756c 225d 2069  ["successful"] i
+000050d0: 7320 5472 7565 290a 2020 2020 2020 2020  s True).        
+000050e0: 0a20 2020 2020 2020 2023 205b 332e 332e  .        # [3.3.
+000050f0: 355d 2046 696e 6420 616e 2061 6e63 6573  5] Find an ances
+00005100: 746f 7220 6f66 2074 6865 2065 7665 6e74  tor of the event
+00005110: 2e0a 2020 2020 2020 2020 616e 6365 7374  ..        ancest
+00005120: 6f72 3a20 4f70 7469 6f6e 616c 5b64 6963  or: Optional[dic
+00005130: 745d 203d 2065 7463 2e66 696e 645f 616e  t] = etc.find_an
+00005140: 6365 7374 6f72 280a 2020 2020 2020 2020  cestor(.        
+00005150: 2020 2020 2264 656d 6f5f 626f 6f6b 5f31      "demo_book_1
+00005160: 3a74 6832 2d73 636f 7065 3a32 3032 3330  :th2-scope:20230
+00005170: 3130 3531 3335 3730 3535 3630 3837 3330  1051357055608730
+00005180: 3030 3a64 3631 6539 3330 612d 3864 3030  00:d61e930a-8d00
+00005190: 2d31 3165 642d 6161 3161 2d64 3334 6136  -11ed-aa1a-d34a6
+000051a0: 3135 3531 3532 645f 3122 2c0a 2020 2020  155152d_1",.    
+000051b0: 2020 2020 2020 2020 6669 6c74 6572 3d6c          filter=l
+000051c0: 616d 6264 6120 6576 656e 743a 2022 526f  ambda event: "Ro
+000051d0: 6f74 4576 656e 7422 2069 6e20 6576 656e  otEvent" in even
+000051e0: 745b 2265 7665 6e74 4e61 6d65 225d 2c0a  t["eventName"],.
+000051f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00005200: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+00005210: 332e 365d 2047 6574 2063 6869 6c64 7265  3.6] Get childre
+00005220: 6e20 6f66 2074 6865 2065 7665 6e74 2e20  n of the event. 
+00005230: 5468 6572 6520 6973 2061 6c73 6f20 6974  There is also it
+00005240: 6572 6162 6c65 2076 6572 7369 6f6e 2027  erable version '
+00005250: 6765 745f 6368 696c 6472 656e 5f69 7465  get_children_ite
+00005260: 7227 2e0a 2020 2020 2020 2020 6368 696c  r'..        chil
+00005270: 6472 656e 3a20 5475 706c 655b 6469 6374  dren: Tuple[dict
+00005280: 5d20 3d20 6574 632e 6765 745f 6368 696c  ] = etc.get_chil
+00005290: 6472 656e 280a 2020 2020 2020 2020 2020  dren(.          
+000052a0: 2020 2264 656d 6f5f 626f 6f6b 5f31 3a74    "demo_book_1:t
+000052b0: 6832 2d73 636f 7065 3a32 3032 3330 3130  h2-scope:2023010
+000052c0: 3531 3335 3730 3535 3630 3837 3330 3030  5135705560873000
+000052d0: 3a64 3631 6539 3330 612d 3864 3030 2d31  :d61e930a-8d00-1
+000052e0: 3165 642d 6161 3161 2d64 3334 6136 3135  1ed-aa1a-d34a615
+000052f0: 3531 3532 645f 3122 0a20 2020 2020 2020  5152d_1".       
+00005300: 2029 0a20 2020 2020 2020 200a 2020 2020   ).        .    
+00005310: 2020 2020 2320 5b33 2e33 2e37 5d20 4765      # [3.3.7] Ge
+00005320: 7420 7375 6274 7265 6520 666f 7220 7370  t subtree for sp
+00005330: 6563 6966 6965 6420 6576 656e 742e 0a20  ecified event.. 
+00005340: 2020 2020 2020 2073 7562 7472 6565 3a20         subtree: 
+00005350: 4576 656e 7454 7265 6520 3d20 6574 632e  EventTree = etc.
+00005360: 6765 745f 7375 6274 7265 6528 0a20 2020  get_subtree(.   
+00005370: 2020 2020 2020 2020 2022 6465 6d6f 5f62           "demo_b
+00005380: 6f6f 6b5f 313a 7468 322d 7363 6f70 653a  ook_1:th2-scope:
+00005390: 3230 3233 3031 3035 3133 3537 3035 3536  2023010513570556
+000053a0: 3038 3733 3030 303a 6436 3165 3933 3061  0873000:d61e930a
+000053b0: 2d38 6430 302d 3131 6564 2d61 6131 612d  -8d00-11ed-aa1a-
+000053c0: 6433 3461 3631 3535 3135 3264 5f31 220a  d34a6155152d_1".
+000053d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000053e0: 2020 0a20 2020 2020 2020 2023 205b 332e    .        # [3.
+000053f0: 332e 385d 2047 6574 2066 756c 6c20 7061  3.8] Get full pa
+00005400: 7468 2074 6f20 7468 6520 6576 656e 742e  th to the event.
+00005410: 0a20 2020 2020 2020 2023 204c 6f6f 6b73  .        # Looks
+00005420: 206c 696b 6520 5b61 6e63 6573 746f 725f   like [ancestor_
+00005430: 726f 6f74 2c20 616e 6365 7374 6f72 5f6c  root, ancestor_l
+00005440: 6576 656c 312c 2061 6e63 6573 746f 725f  evel1, ancestor_
+00005450: 6c65 7665 6c32 2c20 6576 656e 745d 0a20  level2, event]. 
+00005460: 2020 2020 2020 2065 7665 6e74 5f70 6174         event_pat
+00005470: 683a 204c 6973 745b 6469 6374 5d20 3d20  h: List[dict] = 
+00005480: 6574 632e 6765 745f 6675 6c6c 5f70 6174  etc.get_full_pat
+00005490: 6828 0a20 2020 2020 2020 2020 2020 2022  h(.            "
+000054a0: 6465 6d6f 5f62 6f6f 6b5f 313a 7468 322d  demo_book_1:th2-
+000054b0: 7363 6f70 653a 3230 3233 3031 3035 3133  scope:2023010513
+000054c0: 3537 3035 3536 3038 3733 3030 303a 6436  5705560873000:d6
+000054d0: 3165 3933 3061 2d38 6430 302d 3131 6564  1e930a-8d00-11ed
+000054e0: 2d61 6131 612d 6433 3461 3631 3535 3135  -aa1a-d34a615515
+000054f0: 3264 5f31 220a 2020 2020 2020 2020 290a  2d_1".        ).
+00005500: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005510: 2023 205b 332e 332e 395d 2047 6574 2070   # [3.3.9] Get p
+00005520: 6172 656e 7420 6f66 2074 6865 2065 7665  arent of the eve
+00005530: 6e74 2e0a 2020 2020 2020 2020 7061 7265  nt..        pare
+00005540: 6e74 203d 2065 7463 2e67 6574 5f70 6172  nt = etc.get_par
+00005550: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
+00005560: 2022 6465 6d6f 5f62 6f6f 6b5f 313a 7468   "demo_book_1:th
+00005570: 322d 7363 6f70 653a 3230 3233 3031 3035  2-scope:20230105
+00005580: 3133 3537 3035 3536 3038 3733 3030 303a  135705560873000:
+00005590: 6436 3165 3933 3061 2d38 6430 302d 3131  d61e930a-8d00-11
+000055a0: 6564 2d61 6131 612d 6433 3461 3631 3535  ed-aa1a-d34a6155
+000055b0: 3135 3264 5f31 220a 2020 2020 2020 2020  152d_1".        
+000055c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000055d0: 2020 2023 205b 332e 332e 3130 5d20 4170     # [3.3.10] Ap
+000055e0: 7065 6e64 206e 6577 2065 7665 6e74 2074  pend new event t
+000055f0: 6f20 7468 6520 636f 6c6c 6563 7469 6f6e  o the collection
+00005600: 2e0a 2020 2020 2020 2020 6574 632e 6170  ..        etc.ap
+00005610: 7065 6e64 5f65 7665 6e74 280a 2020 2020  pend_event(.    
+00005620: 2020 2020 2020 2020 6576 656e 743d 7b0a          event={.
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2265 7665 6e74 4964 223a 2022 6132 3066  "eventId": "a20f
+00005650: 3565 6634 2d63 3366 652d 6262 3130 2d61  5ef4-c3fe-bb10-a
+00005660: 3239 632d 6464 3364 3738 3439 3039 6562  29c-dd3d784909eb
+00005670: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005680: 2020 2022 7061 7265 6e74 4576 656e 7449     "parentEventI
+00005690: 6422 3a20 2238 6532 3532 3466 612d 6366  d": "8e2524fa-cf
+000056a0: 3539 2d31 3165 622d 6133 6637 2d30 3934  59-11eb-a3f7-094
+000056b0: 6639 3034 6333 6136 3222 2c0a 2020 2020  f904c3a62",.    
+000056c0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+000056d0: 6e74 4e61 6d65 223a 2022 5374 7562 4576  ntName": "StubEv
+000056e0: 656e 7422 2c0a 2020 2020 2020 2020 2020  ent",.          
+000056f0: 2020 7d0a 2020 2020 2020 2020 290a 2020    }.        ).  
+00005700: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005710: 205b 332e 332e 3131 5d20 5368 6f77 2074   [3.3.11] Show t
+00005720: 6865 2065 6e74 6972 6520 636f 6c6c 6563  he entire collec
+00005730: 7469 6f6e 2e0a 2020 2020 2020 2020 6574  tion..        et
+00005740: 632e 7368 6f77 2829 0a20 2020 2020 2020  c.show().       
+00005750: 2023 2049 7427 6c6c 2070 7269 6e74 2074   # It'll print t
+00005760: 6865 2066 6f6c 6c6f 7769 6e67 3a0a 2020  he following:.  
+00005770: 2020 2020 2020 2320 5365 7420 6f66 2061        # Set of a
+00005780: 7574 6f2d 6765 6e65 7261 7465 6420 6576  uto-generated ev
+00005790: 656e 7473 2066 6f72 2064 7320 6c69 6220  ents for ds lib 
+000057a0: 7465 7374 696e 670a 2020 2020 2020 2020  testing.        
+000057b0: 2320 e294 9ce2 9480 e294 8020 506c 6169  # ......... Plai
+000057c0: 6e20 6576 656e 7420 310a 2020 2020 2020  n event 1.      
+000057d0: 2020 2320 e294 94e2 9480 e294 8020 506c    # ......... Pl
+000057e0: 6169 6e20 6576 656e 7420 320a 2020 2020  ain event 2.    
+000057f0: 2020 2020 0a20 2020 2020 2020 2023 2041      .        # A
+00005800: 7320 796f 7520 6361 6e20 7365 652c 206e  s you can see, n
+00005810: 6f74 6869 6e67 2077 6173 2063 6861 6e67  othing was chang
+00005820: 6564 2c20 6275 7420 7765 2061 6464 6564  ed, but we added
+00005830: 2074 6865 206e 6577 2065 7665 6e74 210a   the new event!.
+00005840: 2020 2020 2020 2020 2320 6c65 7427 7320          # let's 
+00005850: 6c6f 6f6b 2061 7420 7468 6520 7375 6d6d  look at the summ
+00005860: 6172 792e 0a20 2020 2020 2020 200a 2020  ary..        .  
+00005870: 2020 2020 2020 7072 696e 7428 6574 632e        print(etc.
+00005880: 7375 6d6d 6172 7928 2929 2020 2320 7468  summary())  # th
+00005890: 6520 7361 6d65 2061 7320 6a75 7374 2070  e same as just p
+000058a0: 7269 6e74 2865 7463 290a 2020 2020 2020  rint(etc).      
+000058b0: 2020 2320 4576 656e 7454 7265 6543 6f6c    # EventTreeCol
+000058c0: 6c65 6374 696f 6e28 7472 6565 733d 312c  lection(trees=1,
+000058d0: 2065 7665 6e74 733d 355b 7472 6565 733d   events=5[trees=
+000058e0: 332c 2064 6574 6163 6865 643d 325d 290a  3, detached=2]).
+000058f0: 2020 2020 2020 2020 2320 596f 7520 6361          # You ca
+00005900: 6e20 7365 6520 7468 6174 2069 7420 7761  n see that it wa
+00005910: 7320 6164 6465 6420 746f 2064 6574 6163  s added to detac
+00005920: 6865 642e 2054 6861 7427 7320 7768 7920  hed. That's why 
+00005930: 796f 7520 646f 6e27 7420 7365 6520 7468  you don't see th
+00005940: 6520 6576 656e 740a 2020 2020 2020 2020  e event.        
+00005950: 2320 7669 6120 6073 686f 7728 2960 2e20  # via `show()`. 
+00005960: 6073 686f 7728 2960 2070 7269 6e74 7320  `show()` prints 
+00005970: 6f6e 6c79 2054 7265 6573 210a 2020 2020  only Trees!.    
+00005980: 2020 2020 2320 5573 6520 6065 7463 2e67      # Use `etc.g
+00005990: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+000059a0: 6565 7328 2960 2074 6f20 636f 6e76 6572  ees()` to conver
+000059b0: 7420 6465 7461 6368 6564 2065 7665 6e74  t detached event
+000059c0: 7320 746f 2074 7265 6573 2e0a 2020 2020  s to trees..    
+000059d0: 2020 2020 2320 4d6f 7265 2069 6e66 6f72      # More infor
+000059e0: 6d61 7469 6f6e 2062 656c 6f77 2069 6e20  mation below in 
+000059f0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+00005a00: 6720 7365 6374 696f 6e2e 0a20 2020 2020  g section..     
+00005a10: 2020 200a 2020 2020 2020 2020 2320 2d2d     .        # --
+00005a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00005a30: 2020 2020 2023 205b 332e 345d 2057 6f72       # [3.4] Wor
+00005a40: 6b69 6e67 2077 6974 6820 7468 6520 4576  king with the Ev
+00005a50: 656e 7454 7265 652e 0a20 2020 2020 2020  entTree..       
+00005a60: 2023 2045 7665 6e74 5472 6565 2068 6173   # EventTree has
+00005a70: 2074 6865 2073 616d 6520 6d65 7468 6f64   the same method
+00005a80: 7320 6173 2045 7665 6e74 5472 6565 436f  s as EventTreeCo
+00005a90: 6c6c 6563 7469 6f6e 2c20 6275 7420 6f6e  llection, but on
+00005aa0: 6c79 2066 6f72 2069 7473 206f 776e 2074  ly for its own t
+00005ab0: 7265 652e 0a20 2020 2020 2020 200a 2020  ree..        .  
+00005ac0: 2020 2020 2020 2320 5b33 2e34 2e31 5d20        # [3.4.1] 
+00005ad0: 4765 7420 6120 636f 6c6c 6563 7469 6f6e  Get a collection
+00005ae0: 206f 6620 7472 6565 732e 0a20 2020 2020   of trees..     
+00005af0: 2020 2074 7265 6573 3a20 4c69 7374 5b45     trees: List[E
+00005b00: 7665 6e74 5472 6565 5d20 3d20 6574 632e  ventTree] = etc.
+00005b10: 6765 745f 7472 6565 7328 290a 2020 2020  get_trees().    
+00005b20: 2020 2020 7472 6565 3a20 4576 656e 7454      tree: EventT
+00005b30: 7265 6520 3d20 7472 6565 735b 305d 0a20  ree = trees[0]. 
+00005b40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005b50: 2320 4275 7420 4576 656e 7454 7265 6520  # But EventTree 
+00005b60: 7072 6f76 6964 6573 2061 2077 6f72 6b20  provides a work 
+00005b70: 7769 7468 2074 6865 2074 7265 652c 2062  with the tree, b
+00005b80: 7574 2064 6f65 7320 6e6f 7420 6d6f 6469  ut does not modi
+00005b90: 6679 2069 742e 0a20 2020 2020 2020 2023  fy it..        #
+00005ba0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
+00005bb0: 6d6f 6469 6679 2074 6865 2074 7265 652c  modify the tree,
+00005bc0: 2075 7365 2045 7665 6e74 5472 6565 436f   use EventTreeCo
+00005bd0: 6c6c 6563 7469 6f6e 732e 0a20 2020 2020  llections..     
+00005be0: 2020 200a 2020 2020 2020 2020 2320 5b33     .        # [3
+00005bf0: 2e35 5d20 576f 726b 696e 6720 7769 7468  .5] Working with
+00005c00: 2050 6172 656e 746c 6573 7354 7265 652e   ParentlessTree.
+00005c10: 0a20 2020 2020 2020 2023 2050 6172 656e  .        # Paren
+00005c20: 746c 6573 7354 7265 6520 6973 2061 6e20  tlessTree is an 
+00005c30: 4576 656e 7454 7265 6520 7468 6174 2068  EventTree that h
+00005c40: 6173 2064 6574 6163 6865 6420 6576 656e  as detached even
+00005c50: 7473 2077 6974 6820 7374 7562 732e 0a20  ts with stubs.. 
+00005c60: 2020 2020 2020 2070 6172 656e 746c 6573         parentles
+00005c70: 735f 7472 6565 733a 204c 6973 745b 4576  s_trees: List[Ev
+00005c80: 656e 7454 7265 655d 203d 2065 7463 2e67  entTree] = etc.g
+00005c90: 6574 5f70 6172 656e 746c 6573 735f 7472  et_parentless_tr
+00005ca0: 6565 7328 290a 2020 2020 2020 2020 7072  ees().        pr
+00005cb0: 696e 7428 2270 6172 656e 746c 6573 735f  int("parentless_
+00005cc0: 7472 6565 7320 636f 6e74 6169 6e73 3a22  trees contains:"
+00005cd0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00005ce0: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
+00005cf0: 290a 2020 2020 2020 2020 2320 5b45 7665  ).        # [Eve
+00005d00: 6e74 5472 6565 286e 616d 653d 273c 4272  ntTree(name='<Br
+00005d10: 6f6b 656e 4576 656e 743e 272c 2072 6f6f  okenEvent>', roo
+00005d20: 745f 6964 3d27 6e6f 745f 6578 6973 7473  t_id='not_exists
+00005d30: 5f69 6e5f 7468 655f 6576 656e 7473 5f73  _in_the_events_s
+00005d40: 7472 6561 6d27 2c20 6576 656e 7473 3d32  tream', events=2
+00005d50: 292c 0a20 2020 2020 2020 2023 2020 4576  ),.        #  Ev
+00005d60: 656e 7454 7265 6528 6e61 6d65 3d27 3c42  entTree(name='<B
+00005d70: 726f 6b65 6e45 7665 6e74 3e27 2c20 726f  rokenEvent>', ro
+00005d80: 6f74 5f69 643d 2738 6532 3532 3466 612d  ot_id='8e2524fa-
+00005d90: 6366 3539 2d31 3165 622d 6133 6637 2d30  cf59-11eb-a3f7-0
+00005da0: 3934 6639 3034 6333 6136 3227 2c20 6576  94f904c3a62', ev
+00005db0: 656e 7473 3d32 295d 0a20 2020 2020 2020  ents=2)].       
+00005dc0: 200a 2020 2020 2020 2020 7072 696e 7428   .        print(
+00005dd0: 225c 6e22 2022 6574 6320 6166 7465 7220  "\n" "etc after 
+00005de0: 6067 6574 5f70 6172 656e 746c 6573 735f  `get_parentless_
+00005df0: 7472 6565 7360 3a22 290a 2020 2020 2020  trees`:").      
+00005e00: 2020 7072 696e 7428 6574 632e 7375 6d6d    print(etc.summ
+00005e10: 6172 7928 2929 0a20 2020 2020 2020 2023  ary()).        #
+00005e20: 2045 7665 6e74 5472 6565 436f 6c6c 6563   EventTreeCollec
+00005e30: 7469 6f6e 2874 7265 6573 3d33 5b72 6567  tion(trees=3[reg
+00005e40: 756c 6172 3d31 2c20 7061 7265 6e74 6c65  ular=1, parentle
+00005e50: 7373 3d32 5d2c 2065 7665 6e74 733d 375b  ss=2], events=7[
+00005e60: 7472 6565 733d 372c 2064 6574 6163 6865  trees=7, detache
+00005e70: 643d 305d 2927 0a20 2020 2020 2020 2065  d=0])'.        e
+00005e80: 7463 2e73 686f 7728 290a 2020 2020 2020  tc.show().      
+00005e90: 2020 2320 5365 7420 6f66 2061 7574 6f2d    # Set of auto-
+00005ea0: 6765 6e65 7261 7465 6420 6576 656e 7473  generated events
+00005eb0: 2066 6f72 2064 7320 6c69 6220 7465 7374   for ds lib test
+00005ec0: 696e 670a 2020 2020 2020 2020 2320 e294  ing.        # ..
+00005ed0: 9ce2 9480 e294 8020 506c 6169 6e20 6576  ....... Plain ev
+00005ee0: 656e 7420 310a 2020 2020 2020 2020 2320  ent 1.        # 
+00005ef0: e294 94e2 9480 e294 8020 506c 6169 6e20  ......... Plain 
+00005f00: 6576 656e 7420 320a 2020 2020 2020 2020  event 2.        
+00005f10: 2320 3c42 726f 6b65 6e45 7665 6e74 3e0a  # <BrokenEvent>.
+00005f20: 2020 2020 2020 2020 2320 e294 94e2 9480          # ......
+00005f30: e294 8020 4661 6b65 2065 7665 6e74 0a20  ... Fake event. 
+00005f40: 2020 2020 2020 2023 203c 4272 6f6b 656e         # <Broken
+00005f50: 4576 656e 743e 0a20 2020 2020 2020 2023  Event>.        #
+00005f60: 20e2 9494 e294 80e2 9480 2053 7475 6245   ......... StubE
+00005f70: 7665 6e74 2020 2020 3c2d 2d2d 2074 6865  vent    <--- the
+00005f80: 2065 7665 6e74 2074 6861 7420 7761 7320   event that was 
+00005f90: 6164 6465 6420 6162 6f76 650a 2020 2020  added above.    
+00005fa0: 2020 2020 0a20 2020 2020 2020 2023 205b      .        # [
+00005fb0: 332e 365d 2057 6f72 6b69 6e67 2077 6974  3.6] Working wit
+00005fc0: 6820 5061 7265 6e74 4576 656e 7454 7265  h ParentEventTre
+00005fd0: 6543 6f6c 6c65 6374 696f 6e2e 0a20 2020  eCollection..   
+00005fe0: 2020 2020 2023 2050 6172 656e 7445 7665       # ParentEve
+00005ff0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00006000: 2069 7320 6120 7472 6565 2063 6f6c 6c65   is a tree colle
+00006010: 6374 696f 6e20 6c69 6b65 2045 7665 6e74  ction like Event
+00006020: 5472 6565 436f 6c6c 6563 7469 6f6e 2c0a  TreeCollection,.
+00006030: 2020 2020 2020 2020 2320 6275 7420 6974          # but it
+00006040: 2068 6173 206f 6e6c 7920 6576 656e 7473   has only events
+00006050: 2074 6861 7420 6861 7665 2072 6566 6572   that have refer
+00006060: 656e 6365 732e 0a20 2020 2020 2020 2064  ences..        d
+00006070: 6174 615f 736f 7572 6365 3a20 4944 6174  ata_source: IDat
+00006080: 6153 6f75 7263 6520 2023 2059 6f75 2073  aSource  # You s
+00006090: 686f 756c 6420 696e 6974 2044 6174 6153  hould init DataS
+000060a0: 6f75 7263 6520 6f62 6a65 6374 2e20 452e  ource object. E.
+000060b0: 672e 2066 726f 6d20 4c77 4450 206d 6f64  g. from LwDP mod
+000060c0: 756c 652e 0a20 2020 2020 2020 2064 6174  ule..        dat
+000060d0: 615f 736f 7572 6365 203d 2044 756d 6d79  a_source = Dummy
+000060e0: 4461 7461 536f 7572 6365 2829 2020 2320  DataSource()  # 
+000060f0: 4e6f 7465 2120 5765 2075 7365 2066 616b  Note! We use fak
+00006100: 6520 4453 2068 6572 652e 0a20 2020 2020  e DS here..     
+00006110: 2020 2023 2045 5443 4472 6976 6572 2068     # ETCDriver h
+00006120: 6572 6520 6973 2061 2073 7475 622c 2061  ere is a stub, a
+00006130: 6374 7561 6c6c 7920 7468 6520 6c69 6220  ctually the lib 
+00006140: 646f 6573 6e27 7420 6861 7665 2073 7563  doesn't have suc
+00006150: 6820 6120 636c 6173 732e 0a20 2020 2020  h a class..     
+00006160: 2020 2023 2059 6f75 2063 616e 2074 616b     # You can tak
+00006170: 6520 6974 2069 6e20 4c77 4450 206d 6f64  e it in LwDP mod
+00006180: 756c 6520 6f72 2063 7265 6174 6520 796f  ule or create yo
+00006190: 7572 7365 6c66 2063 6c61 7373 2069 6620  urself class if 
+000061a0: 796f 7520 6861 7665 2073 6f6d 6520 7370  you have some sp
+000061b0: 6563 6961 6c20 6576 656e 7473 2073 7472  ecial events str
+000061c0: 7563 7475 7265 2e0a 2020 2020 2020 2020  ucture..        
+000061d0: 6672 6f6d 2074 6832 5f64 6174 615f 7365  from th2_data_se
+000061e0: 7276 6963 6573 2e64 6174 615f 736f 7572  rvices.data_sour
+000061f0: 6365 2e6c 7764 702e 6576 656e 745f 7472  ce.lwdp.event_tr
+00006200: 6565 2069 6d70 6f72 740a 2020 2020 2020  ee import.      
+00006210: 2020 0a20 2020 2020 2020 2048 7474 7045    .        HttpE
+00006220: 5443 4472 6976 6572 2061 7320 4554 4344  TCDriver as ETCD
+00006230: 7269 7665 720a 2020 2020 2020 2020 0a20  river.        . 
+00006240: 2020 2020 2020 2064 7269 7665 7220 3d20         driver = 
+00006250: 4554 4344 7269 7665 7228 6461 7461 5f73  ETCDriver(data_s
+00006260: 6f75 7263 653d 6461 7461 5f73 6f75 7263  ource=data_sourc
+00006270: 6529 0a20 2020 2020 2020 2070 6574 6320  e).        petc 
+00006280: 3d20 5061 7265 6e74 4576 656e 7454 7265  = ParentEventTre
+00006290: 6543 6f6c 6c65 6374 696f 6e28 6472 6976  eCollection(driv
+000062a0: 6572 290a 2020 2020 2020 2020 7065 7463  er).        petc
+000062b0: 2e62 7569 6c64 2865 7665 6e74 7329 0a20  .build(events). 
+000062c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000062d0: 7065 7463 2e73 686f 7728 290a 2020 2020  petc.show().    
+000062e0: 2020 2020 7065 7463 2e73 756d 6d61 7279      petc.summary
+000062f0: 2829 0a20 2020 2020 2020 200a 2020 2020  ().        .    
+00006300: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00006310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006320: 2323 2323 2323 2323 2323 0a20 2020 2020  ##########.     
+00006330: 2020 2023 205b 345d 2046 6965 6c64 2052     # [4] Field R
+00006340: 6573 6f6c 7665 7273 0a20 2020 2020 2020  esolvers.       
+00006350: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00006360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006370: 2323 2323 2323 230a 2020 2020 2020 2020  #######.        
+00006380: 2320 506c 6561 7365 2072 6561 6420 6046  # Please read `F
+00006390: 6965 6c64 2052 6573 6f6c 7665 7273 6020  ield Resolvers` 
+000063a0: 626c 6f63 6b20 696e 2072 6561 646d 6520  block in readme 
+000063b0: 6669 7273 742e 0a20 2020 2020 2020 200a  first..        .
+000063c0: 2020 2020 2020 2020 2320 5b34 2e31 5d20          # [4.1] 
+000063d0: 5573 6167 6520 6578 616d 706c 6520 6672  Usage example fr
+000063e0: 6f6d 2063 6c69 656e 7420 636f 6465 0a20  om client code. 
+000063f0: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+00006400: 6461 7461 5f73 6572 7669 6365 732e 6461  data_services.da
+00006410: 7461 5f73 6f75 7263 6520 696d 706f 7274  ta_source import
+00006420: 2028 0a20 2020 2020 2020 2020 2020 206c   (.            l
+00006430: 7764 702c 0a20 2020 2020 2020 2029 2020  wdp,.        )  
+00006440: 2320 6c77 6470 2064 6174 615f 736f 7572  # lwdp data_sour
+00006450: 6365 2069 6e69 7469 616c 697a 6520 7468  ce initialize th
+00006460: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+00006470: 636f 6e66 6967 2064 7572 696e 6720 696d  config during im
+00006480: 706f 7274 2e0a 2020 2020 2020 2020 6672  port..        fr
+00006490: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+000064a0: 6963 6573 2e63 6f6e 6669 6720 696d 706f  ices.config impo
+000064b0: 7274 206f 7074 696f 6e73 2061 7320 6f5f  rt options as o_
+000064c0: 0a20 2020 2020 2020 2066 726f 6d20 7468  .        from th
+000064d0: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+000064e0: 6461 7461 5f73 6f75 7263 652e 6c77 6470  data_source.lwdp
+000064f0: 2e73 7475 625f 6275 696c 6465 7220 696d  .stub_builder im
+00006500: 706f 7274 0a20 2020 2020 2020 200a 2020  port.        .  
+00006510: 2020 2020 2020 6874 7470 5f6d 6573 7361        http_messa
+00006520: 6765 5f73 7475 625f 6275 696c 6465 720a  ge_stub_builder.
+00006530: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006540: 2066 616b 655f 6461 7461 203d 205b 0a20   fake_data = [. 
+00006550: 2020 2020 2020 2020 2020 2068 7474 705f             http_
+00006560: 6d65 7373 6167 655f 7374 7562 5f62 7569  message_stub_bui
+00006570: 6c64 6572 2e62 7569 6c64 287b 226d 6573  lder.build({"mes
+00006580: 7361 6765 4964 223a 2022 6122 2c20 226d  sageId": "a", "m
+00006590: 6573 7361 6765 5479 7065 223a 2022 526f  essageType": "Ro
+000065a0: 6f74 227d 292c 0a20 2020 2020 2020 2020  ot"}),.         
+000065b0: 2020 2068 7474 705f 6d65 7373 6167 655f     http_message_
+000065c0: 7374 7562 5f62 7569 6c64 6572 2e62 7569  stub_builder.bui
+000065d0: 6c64 287b 226d 6573 7361 6765 4964 223a  ld({"messageId":
+000065e0: 2022 6222 2c20 226d 6573 7361 6765 5479   "b", "messageTy
+000065f0: 7065 223a 2022 4e65 7722 7d29 2c0a 2020  pe": "New"}),.  
+00006600: 2020 2020 2020 2020 2020 6874 7470 5f6d            http_m
+00006610: 6573 7361 6765 5f73 7475 625f 6275 696c  essage_stub_buil
+00006620: 6465 722e 6275 696c 6428 7b22 6d65 7373  der.build({"mess
+00006630: 6167 6549 6422 3a20 2263 222c 2022 6d65  ageId": "c", "me
+00006640: 7373 6167 6554 7970 6522 3a20 2241 6d65  ssageType": "Ame
+00006650: 6e64 227d 292c 0a20 2020 2020 2020 2020  nd"}),.         
+00006660: 2020 2068 7474 705f 6d65 7373 6167 655f     http_message_
+00006670: 7374 7562 5f62 7569 6c64 6572 2e62 7569  stub_builder.bui
+00006680: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00006690: 2020 2020 7b22 6d65 7373 6167 6549 6422      {"messageId"
+000066a0: 3a20 2264 222c 2022 6d65 7373 6167 6554  : "d", "messageT
+000066b0: 7970 6522 3a20 2243 616e 6365 6c22 7d29  ype": "Cancel"})
+000066c0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+000066d0: 2020 2020 6661 6b65 5f64 6174 615f 6f62      fake_data_ob
+000066e0: 6a20 3d20 4461 7461 2866 616b 655f 6461  j = Data(fake_da
+000066f0: 7461 290a 2020 2020 2020 2020 0a20 2020  ta).        .   
+00006700: 2020 2020 2066 6f72 206d 2069 6e20 6661       for m in fa
+00006710: 6b65 5f64 6174 615f 6f62 6a3a 0a20 2020  ke_data_obj:.   
+00006720: 2020 2020 2020 2020 206f 5f2e 6d66 722e           o_.mfr.
+00006730: 6578 7061 6e64 5f6d 6573 7361 6765 286d  expand_message(m
+00006740: 2920 2023 206d 6672 202d 2073 7461 6e64  )  # mfr - stand
+00006750: 7320 666f 7220 4d65 7373 6167 6546 6965  s for MessageFie
+00006760: 6c64 5265 736f 6c76 6572 0a20 2020 2020  ldResolver.     
+00006770: 2020 2023 206f 720a 2020 2020 2020 2020     # or.        
+00006780: 666f 7220 6d20 696e 2066 616b 655f 6461  for m in fake_da
+00006790: 7461 5f6f 626a 2e6d 6170 286f 5f2e 6d66  ta_obj.map(o_.mf
+000067a0: 722e 6578 7061 6e64 5f6d 6573 7361 6765  r.expand_message
+000067b0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+000067c0: 6173 730a 2020 2020 2020 2020 0a20 2020  ass.        .   
+000067d0: 2020 2020 2023 205b 342e 325d 204c 6962       # [4.2] Lib
+000067e0: 7261 7269 6573 2075 7361 6765 2e0a 2020  raries usage..  
+000067f0: 2020 2020 2020 2320 446f 6e27 7420 696d        # Don't im
+00006800: 706f 7274 2065 7861 6374 2072 6573 6f6c  port exact resol
+00006810: 7665 7273 2069 6d70 6c65 6d65 6e74 6174  vers implementat
+00006820: 696f 6e20 696e 2079 6f75 7220 636f 6465  ion in your code
+00006830: 2c20 706c 6561 7365 2e0a 2020 2020 2020  , please..      
+00006840: 2020 2320 416c 6c6f 7720 796f 7572 2063    # Allow your c
+00006850: 6c69 656e 7420 746f 2064 6f20 6974 2069  lient to do it i
+00006860: 6e73 7465 6164 2e0a 2020 2020 2020 2020  nstead..        
+00006870: 2320 4a75 7374 2069 6d70 6f72 7420 606f  # Just import `o
+00006880: 7074 696f 6e73 6020 6672 6f6d 2060 7468  ptions` from `th
+00006890: 325f 6461 7461 5f73 6572 7669 6365 732e  2_data_services.
+000068a0: 636f 6e66 6967 6020 616e 6420 7573 6520  config` and use 
+000068b0: 6974 2e0a 2020 2020 2020 2020 6672 6f6d  it..        from
+000068c0: 2074 6832 5f64 6174 615f 7365 7276 6963   th2_data_servic
+000068d0: 6573 2e63 6f6e 6669 6720 696d 706f 7274  es.config import
+000068e0: 206f 7074 696f 6e73 2061 7320 6f5f 0a20   options as o_. 
+000068f0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006900: 666f 7220 6d20 696e 2066 616b 655f 6461  for m in fake_da
+00006910: 7461 5f6f 626a 3a0a 2020 2020 2020 2020  ta_obj:.        
+00006920: 2020 2020 6f5f 2e6d 6672 2e65 7870 616e      o_.mfr.expan
+00006930: 645f 6d65 7373 6167 6528 6d29 0a20 2020  d_message(m).   
+00006940: 2020 2020 2023 206f 720a 2020 2020 2020       # or.      
+00006950: 2020 666f 7220 6d20 696e 2066 616b 655f    for m in fake_
+00006960: 6461 7461 5f6f 626a 2e6d 6170 286f 5f2e  data_obj.map(o_.
+00006970: 6d66 722e 6578 7061 6e64 5f6d 6573 7361  mfr.expand_messa
+00006980: 6765 293a 0a20 2020 2020 2020 2020 2020  ge):.           
+00006990: 2070 6173 730a 2020 2020 2020 2020 0a20   pass.        . 
+000069a0: 2020 2020 2020 2023 204d 6f72 6520 7465         # More te
+000069b0: 6368 2064 6574 6169 6c73 3a0a 2020 2020  ch details:.    
+000069c0: 2020 2020 2320 2020 496e 2074 6869 7320      #   In this 
+000069d0: 6361 7365 2c20 7468 6572 6520 6973 206e  case, there is n
+000069e0: 6f20 6c69 6e65 2060 6672 6f6d 2074 6832  o line `from th2
+000069f0: 5f64 6174 615f 7365 7276 6963 6573 2e64  _data_services.d
+00006a00: 6174 615f 736f 7572 6365 2069 6d70 6f72  ata_source impor
+00006a10: 7420 6c77 6470 2060 0a20 2020 2020 2020  t lwdp `.       
+00006a20: 2023 2020 2062 6563 6175 7365 2077 6520   #   because we 
+00006a30: 7368 6f75 6c64 206e 6f74 2063 686f 6f73  should not choos
+00006a40: 6520 666f 7220 7468 6520 7573 6572 2077  e for the user w
+00006a50: 6869 6368 2061 2064 6174 6120 736f 7572  hich a data sour
+00006a60: 6365 2074 6f20 7573 652e 0a20 2020 2020  ce to use..     
+00006a70: 2020 2023 2020 2057 6520 646f 206e 6f74     #   We do not
+00006a80: 206b 6e6f 7720 7768 6174 2068 6520 7769   know what he wi
+00006a90: 6c6c 2063 686f 6f73 652c 2074 6865 7265  ll choose, there
+00006aa0: 666f 7265 2c20 7765 206d 7573 7420 7369  fore, we must si
+00006ab0: 6d70 6c79 2061 6363 6573 730a 2020 2020  mply access.    
+00006ac0: 2020 2020 2320 2020 7468 6520 696e 7465      #   the inte
+00006ad0: 7266 6163 652c 2077 6869 6368 2077 696c  rface, which wil
+00006ae0: 6c20 6265 2069 6e69 7469 616c 697a 6564  l be initialized
+00006af0: 2062 7920 7468 6520 7573 6572 2e0a 2020   by the user..  
+00006b00: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00006b10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b30: 2323 2323 230a 2020 2020 2020 2020 2320  #####.        # 
+00006b40: 5b35 5d20 5573 696e 6720 7574 696c 6974  [5] Using utilit
+00006b50: 7920 6675 6e63 7469 6f6e 732e 0a20 2020  y functions..   
+00006b60: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00006b70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006b80: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00006b90: 2020 2020 6672 6f6d 2074 6832 5f64 6174      from th2_dat
+00006ba0: 615f 7365 7276 6963 6573 2e75 7469 6c73  a_services.utils
+00006bb0: 2e65 7665 6e74 5f75 7469 6c73 2e66 7265  .event_utils.fre
+00006bc0: 7175 656e 6369 6573 2069 6d70 6f72 740a  quencies import.
+00006bd0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006be0: 2067 6574 5f63 6174 6567 6f72 795f 6672   get_category_fr
+00006bf0: 6571 7565 6e63 6965 7332 0a20 2020 2020  equencies2.     
+00006c00: 2020 2066 726f 6d20 7468 325f 6461 7461     from th2_data
+00006c10: 5f73 6572 7669 6365 732e 7574 696c 732e  _services.utils.
+00006c20: 6576 656e 745f 7574 696c 732e 746f 7461  event_utils.tota
+00006c30: 6c73 2069 6d70 6f72 7420 6765 745f 6361  ls import get_ca
+00006c40: 7465 676f 7279 5f74 6f74 616c 7332 0a20  tegory_totals2. 
+00006c50: 2020 2020 2020 2066 726f 6d20 7468 325f         from th2_
+00006c60: 6461 7461 5f73 6572 7669 6365 732e 7574  data_services.ut
+00006c70: 696c 732e 6361 7465 676f 7279 2069 6d70  ils.category imp
+00006c80: 6f72 7420 4361 7465 676f 7279 0a20 2020  ort Category.   
+00006c90: 2020 2020 2066 726f 6d20 7468 325f 6461       from th2_da
+00006ca0: 7461 5f73 6572 7669 6365 732e 7574 696c  ta_services.util
+00006cb0: 732e 6576 656e 745f 7574 696c 732e 6576  s.event_utils.ev
+00006cc0: 656e 745f 7574 696c 7320 696d 706f 7274  ent_utils import
+00006cd0: 2069 735f 736f 7274 6564 0a20 2020 2020   is_sorted.     
+00006ce0: 2020 200a 2020 2020 2020 2020 2320 5b35     .        # [5
+00006cf0: 2e31 5d20 4765 7420 7468 6520 7175 616e  .1] Get the quan
+00006d00: 7469 7469 6573 206f 6620 6576 656e 7473  tities of events
+00006d10: 2066 6f72 2064 6966 6665 7265 6e74 2063   for different c
+00006d20: 6174 6567 6f72 6965 732e 0a20 2020 2020  ategories..     
+00006d30: 2020 206d 6574 7269 6373 203d 205b 0a20     metrics = [. 
+00006d40: 2020 2020 2020 2020 2020 2043 6174 6567             Categ
+00006d50: 6f72 7928 2264 6174 6522 2c20 6c61 6d62  ory("date", lamb
+00006d60: 6461 206d 3a20 5468 3254 696d 6573 7461  da m: Th2Timesta
+00006d70: 6d70 436f 6e76 6572 7465 722e 746f 5f64  mpConverter.to_d
+00006d80: 6174 6574 696d 6528 0a20 2020 2020 2020  atetime(.       
+00006d90: 2020 2020 2020 2020 206d 5b22 7374 6172           m["star
+00006da0: 7454 696d 6573 7461 6d70 225d 292e 6461  tTimestamp"]).da
+00006db0: 7465 2829 292c 0a20 2020 2020 2020 2020  te()),.         
+00006dc0: 2020 2043 6174 6567 6f72 7928 2273 7461     Category("sta
+00006dd0: 7475 7322 2c20 6c61 6d62 6461 206d 3a20  tus", lambda m: 
+00006de0: 6d5b 2273 7563 6365 7373 6675 6c22 5d29  m["successful"])
+00006df0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00006e00: 2020 2020 6361 7465 676f 7279 5f74 6f74      category_tot
+00006e10: 616c 7320 3d20 6765 745f 6361 7465 676f  als = get_catego
+00006e20: 7279 5f74 6f74 616c 7332 2865 7665 6e74  ry_totals2(event
+00006e30: 732c 206d 6574 7269 6373 290a 2020 2020  s, metrics).    
+00006e40: 2020 2020 7072 696e 7428 6361 7465 676f      print(catego
+00006e50: 7279 5f74 6f74 616c 7329 0a20 2020 2020  ry_totals).     
+00006e60: 2020 2022 2222 0a20 2020 2020 2020 202b     """.        +
+00006e70: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00006e80: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00006e90: 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020  +---------+.    
+00006ea0: 2020 2020 7c20 2020 2020 2020 207c 2064      |        | d
+00006eb0: 6174 6520 2020 2020 2020 7c20 7374 6174  ate       | stat
+00006ec0: 7573 2020 207c 2020 2063 6f75 6e74 207c  us   |   count |
+00006ed0: 0a20 2020 2020 2020 202b 3d3d 3d3d 3d3d  .        +======
+00006ee0: 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ==+============+
+00006ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  ==========+=====
+00006f00: 3d3d 3d3d 2b0a 2020 2020 2020 2020 7c20  ====+.        | 
+00006f10: 2020 2020 2020 207c 2032 3032 332d 3031         | 2023-01
+00006f20: 2d30 3520 7c20 5472 7565 2020 2020 207c  -05 | True     |
+00006f30: 2020 2020 2020 2033 207c 0a20 2020 2020         3 |.     
+00006f40: 2020 202b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d     +--------+---
+00006f50: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00006f60: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a  ----+---------+.
+00006f70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006f80: 207c 2032 3032 332d 3031 2d30 3520 7c20   | 2023-01-05 | 
+00006f90: 4661 6c73 6520 2020 207c 2020 2020 2020  False    |      
+00006fa0: 2031 207c 0a20 2020 2020 2020 202b 2d2d   1 |.        +--
+00006fb0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00006fc0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  ---+----------+-
+00006fd0: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00006fe0: 2020 7c20 636f 756e 7420 207c 2020 2020    | count  |    
+00006ff0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00007000: 2020 207c 2020 2020 2020 2032 207c 0a20     |       2 |. 
+00007010: 2020 2020 2020 202b 2d2d 2d2d 2d2d 2d2d         +--------
+00007020: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  +------------+--
+00007030: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00007040: 2d2d 2b0a 2020 2020 2020 2020 7c20 746f  --+.        | to
+00007050: 7461 6c73 207c 2020 2020 2020 2020 2020  tals |          
+00007060: 2020 7c20 312f 3120 2020 2020 207c 2020    | 1/1      |  
+00007070: 2020 2020 2034 207c 0a20 2020 2020 2020       4 |.       
+00007080: 202b 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d   +--------+-----
+00007090: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000070a0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2b0a 2020  --+---------+.  
+000070b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000070c0: 2020 0a20 2020 2020 2020 2023 205b 352e    .        # [5.
+000070d0: 325d 2047 6574 2074 6865 206e 756d 6265  2] Get the numbe
+000070e0: 7220 6f66 2065 7665 6e74 7320 7769 7468  r of events with
+000070f0: 2073 7461 7475 7320 7375 6363 6573 7366   status successf
+00007100: 756c 2e0a 2020 2020 2020 2020 6361 7465  ul..        cate
+00007110: 676f 7279 203d 2043 6174 6567 6f72 7928  gory = Category(
+00007120: 2273 7461 7475 7322 2c20 6c61 6d62 6461  "status", lambda
+00007130: 206d 3a20 6d5b 2273 7563 6365 7373 6675   m: m["successfu
+00007140: 6c22 5d29 0a20 2020 2020 2020 2063 6174  l"]).        cat
+00007150: 6567 6f72 795f 6672 6571 7565 6e63 6965  egory_frequencie
+00007160: 7320 3d20 6765 745f 6361 7465 676f 7279  s = get_category
+00007170: 5f66 7265 7175 656e 6369 6573 3228 6576  _frequencies2(ev
+00007180: 656e 7473 2c20 6361 7465 676f 7279 290a  ents, category).
+00007190: 2020 2020 2020 2020 7072 696e 7428 6361          print(ca
+000071a0: 7465 676f 7279 5f66 7265 7175 656e 6369  tegory_frequenci
+000071b0: 6573 290a 2020 2020 2020 2020 2222 220a  es).        """.
+000071c0: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+000071d0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+000071e0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000071f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00007200: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007210: 2b0a 2020 2020 2020 2020 7c20 2020 2020  +.        |     
+00007220: 2020 207c 2074 696d 6573 7461 6d70 5f73     | timestamp_s
+00007230: 7461 7274 2020 2020 207c 2074 696d 6573  tart     | times
+00007240: 7461 6d70 5f65 6e64 2020 2020 2020 207c  tamp_end       |
+00007250: 2046 616c 7365 2020 207c 2020 2054 7275   False   |   Tru
+00007260: 6520 7c0a 2020 2020 2020 2020 2b3d 3d3d  e |.        +===
+00007270: 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d  =====+==========
+00007280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+00007290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000072a0: 3d2b 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  =+=========+====
+000072b0: 3d3d 3d3d 2b0a 2020 2020 2020 2020 7c20  ====+.        | 
+000072c0: 2020 2020 2020 207c 2032 3032 332d 3031         | 2023-01
+000072d0: 2d30 3554 3133 3a35 373a 3035 207c 2032  -05T13:57:05 | 2
+000072e0: 3032 332d 3031 2d30 3554 3133 3a35 373a  023-01-05T13:57:
+000072f0: 3036 207c 2030 2020 2020 2020 207c 2020  06 | 0       |  
+00007300: 2020 2020 3320 7c0a 2020 2020 2020 2020      3 |.        
+00007310: 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  +--------+------
+00007320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007340: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b  -----+---------+
+00007350: 2d2d 2d2d 2d2d 2d2d 2b0a 2020 2020 2020  --------+.      
+00007360: 2020 7c20 2020 2020 2020 207c 2032 3032    |        | 202
+00007370: 332d 3031 2d30 3554 3134 3a30 323a 3035  3-01-05T14:02:05
+00007380: 207c 2032 3032 332d 3031 2d30 3554 3134   | 2023-01-05T14
+00007390: 3a30 323a 3036 207c 2031 2020 2020 2020  :02:06 | 1      
+000073a0: 207c 2020 2020 2020 3020 7c0a 2020 2020   |      0 |.    
+000073b0: 2020 2020 2b2d 2d2d 2d2d 2d2d 2d2b 2d2d      +--------+--
+000073c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073d0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+000073e0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000073f0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2b0a 2020  ---+--------+.  
+00007400: 2020 2020 2020 7c20 636f 756e 7420 207c        | count  |
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00007430: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00007440: 2020 2020 207c 2020 2020 2020 3220 7c0a       |      2 |.
+00007450: 2020 2020 2020 2020 2b2d 2d2d 2d2d 2d2d          +-------
+00007460: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00007470: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00007480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00007490: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000074a0: 2b0a 2020 2020 2020 2020 7c20 746f 7461  +.        | tota
+000074b0: 6c73 207c 2020 2020 2020 2020 2020 2020  ls |            
+000074c0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+000074d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000074e0: 2031 2020 2020 2020 207c 2020 2020 2020   1       |      
+000074f0: 3320 7c0a 2020 2020 2020 2020 2b2d 2d2d  3 |.        +---
+00007500: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007530: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -+---------+----
+00007540: 2d2d 2d2d 2b0a 2020 2020 2020 2020 2222  ----+.        ""
+00007550: 220a 2020 2020 2020 2020 0a20 2020 2020  ".        .     
+00007560: 2020 2023 205b 352e 335d 2043 6865 636b     # [5.3] Check
+00007570: 2069 6620 6576 656e 7473 2061 7265 2073   if events are s
+00007580: 6f72 7465 642e 0a20 2020 2020 2020 2072  orted..        r
+00007590: 6573 756c 7420 3d20 6973 5f73 6f72 7465  esult = is_sorte
+000075a0: 6428 6576 656e 7473 290a 2020 2020 2020  d(events).      
+000075b0: 2020 7072 696e 7428 7265 7375 6c74 290a    print(result).
+000075c0: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+000075d0: 2020 2020 3c21 2d2d 2065 6e64 2067 6574      <!-- end get
+000075e0: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
+000075f0: 2e70 7920 2d2d 3e0a 2020 2020 2020 2020  .py -->.        
+00007600: 0a20 2020 2020 2020 2023 2320 322e 332e  .        ## 2.3.
+00007610: 2053 686f 7274 2074 6865 6f72 790a 2020   Short theory.  
+00007620: 2020 2020 2020 0a20 2020 2020 2020 2054        .        T
+00007630: 6865 206c 6962 7261 7279 2070 726f 7669  he library provi
+00007640: 6465 7320 746f 6f6c 7320 666f 7220 6861  des tools for ha
+00007650: 6e64 6c69 6e67 2073 7472 6561 6d20 6461  ndling stream da
+00007660: 7461 2e20 5768 6174 2773 2061 2073 7472  ta. What's a str
+00007670: 6561 6d3f 2049 7427 7320 6120 7365 7175  eam? It's a sequ
+00007680: 656e 6365 206f 6620 656c 656d 656e 7473  ence of elements
+00007690: 2066 726f 6d20 6120 736f 7572 6365 2074   from a source t
+000076a0: 6861 740a 2020 2020 2020 2020 7375 7070  hat.        supp
+000076b0: 6f72 7473 2061 6767 7265 6761 7465 206f  orts aggregate o
+000076c0: 7065 7261 7469 6f6e 732e 0a20 2020 2020  perations..     
+000076d0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+000076e0: 5465 726d 730a 2020 2020 2020 2020 0a20  Terms.        . 
+000076f0: 2020 2020 2020 202d 202a 2a44 6174 6120         - **Data 
+00007700: 6f62 6a65 6374 2a2a 3a20 416e 2069 6e73  object**: An ins
+00007710: 7461 6e63 6520 6f66 2060 4461 7461 6020  tance of `Data` 
+00007720: 636c 6173 7320 7768 6963 6820 6973 2077  class which is w
+00007730: 7261 7070 6572 2075 6e64 6572 2073 7472  rapper under str
+00007740: 6561 6d2e 0a20 2020 2020 2020 202d 202a  eam..        - *
+00007750: 2a53 6571 7565 6e63 6520 6f66 2065 6c65  *Sequence of ele
+00007760: 6d65 6e74 732a 2a3a 0a20 2020 2020 2020  ments**:.       
+00007770: 2020 2041 205f 4461 7461 206f 626a 6563     A _Data objec
+00007780: 745f 2070 726f 7669 6465 7320 616e 2069  t_ provides an i
+00007790: 6e74 6572 6661 6365 2074 6f20 6120 7365  nterface to a se
+000077a0: 7175 656e 6365 6420 7365 7420 6f66 2076  quenced set of v
+000077b0: 616c 7565 7320 6f66 2061 2073 7065 6369  alues of a speci
+000077c0: 6669 6320 656c 656d 656e 7420 7479 7065  fic element type
+000077d0: 2e20 5374 7265 616d 2069 6e73 6964 6520  . Stream inside 
+000077e0: 7468 6520 5f44 6174 610a 2020 2020 2020  the _Data.      
+000077f0: 2020 2020 6f62 6a65 6374 5f20 2a2a 646f      object_ **do
+00007800: 6e19 7420 6163 7475 616c 6c79 2073 746f  n.t actually sto
+00007810: 7265 2a2a 2065 6c65 6d65 6e74 733b 2074  re** elements; t
+00007820: 6865 7920 6172 6520 636f 6d70 7574 6564  hey are computed
+00007830: 206f 6e20 6465 6d61 6e64 2e0a 2020 2020   on demand..    
+00007840: 2020 2020 2d20 2a2a 6461 7461 2073 6f75      - **data sou
+00007850: 7263 652a 2a20 2865 7861 6374 6c79 2069  rce** (exactly i
+00007860: 6e20 736d 616c 6c20 6c65 7474 6572 7329  n small letters)
+00007870: 3a0a 2020 2020 2020 2020 2020 416e 7920  :.          Any 
+00007880: 736f 7572 6365 206f 6620 6461 7461 2e20  source of data. 
+00007890: 452e 672e 205b 4c69 6768 7477 6569 6768  E.g. [Lightweigh
+000078a0: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
+000078b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000078c0: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+000078d0: 6c77 2d64 6174 612d 7072 6f76 6964 6572  lw-data-provider
+000078e0: 292c 2063 6f6c 6c65 6374 696f 6e73 2c0a  ), collections,.
+000078f0: 2020 2020 2020 2020 2020 6172 7261 7973            arrays
+00007900: 2c20 6f72 2049 2f4f 2072 6573 6f75 7263  , or I/O resourc
+00007910: 6573 2e0a 2020 2020 2020 2020 2d20 2a2a  es..        - **
+00007920: 4461 7461 536f 7572 6365 2a2a 3a0a 2020  DataSource**:.  
+00007930: 2020 2020 2020 2020 4120 636c 6173 7320          A class 
+00007940: 7468 6174 2069 7320 616e 2069 6e74 6572  that is an inter
+00007950: 6d65 6469 6174 6520 6c69 6e6b 2062 6574  mediate link bet
+00007960: 7765 656e 2074 6865 2053 6f75 7263 6541  ween the SourceA
+00007970: 5049 2061 6e64 2043 6f6d 6d61 6e64 732e  PI and Commands.
+00007980: 0a20 2020 2020 2020 202d 202a 2a53 6f75  .        - **Sou
+00007990: 7263 6541 5049 2a2a 3a0a 2020 2020 2020  rceAPI**:.      
+000079a0: 2020 2020 4561 6368 2073 6f75 7263 6520      Each source 
+000079b0: 6861 7320 6974 7320 6f77 6e20 4150 4920  has its own API 
+000079c0: 746f 2072 6574 7269 6576 6520 6461 7461  to retrieve data
+000079d0: 2e20 536f 7572 6365 4150 4920 6973 2061  . SourceAPI is a
+000079e0: 2063 6c61 7373 2074 6861 7420 7072 6f76   class that prov
+000079f0: 6964 6520 4150 4920 666f 7220 736f 6d65  ide API for some
+00007a00: 2064 6174 6120 736f 7572 6365 2e0a 2020   data source..  
+00007a10: 2020 2020 2020 2d20 2a2a 436f 6d6d 616e        - **Comman
+00007a20: 6473 2a2a 3a0a 2020 2020 2020 2020 2020  ds**:.          
+00007a30: 436c 6173 7365 7320 7468 6174 2070 726f  Classes that pro
+00007a40: 7669 6465 2075 7365 722d 6672 6965 6e64  vide user-friend
+00007a50: 6c79 2069 6e74 6572 6661 6365 7320 666f  ly interfaces fo
+00007a60: 7220 6765 7474 696e 6720 736f 6d65 2064  r getting some d
+00007a70: 6174 6120 6672 6f6d 2044 6174 6153 6f75  ata from DataSou
+00007a80: 7263 652e 2043 6f6d 6d61 6e64 7320 7573  rce. Commands us
+00007a90: 6520 5f53 6f75 7263 6541 5049 5f20 746f  e _SourceAPI_ to
+00007aa0: 0a20 2020 2020 2020 2020 2061 6368 6965  .          achie
+00007ab0: 7665 2069 742e 0a20 2020 2020 2020 202d  ve it..        -
+00007ac0: 202a 2a41 6461 7074 6572 732a 2a3a 0a20   **Adapters**:. 
+00007ad0: 2020 2020 2020 2020 2049 7427 7320 7369           It's si
+00007ae0: 6d69 6c61 7220 746f 2066 756e 6374 696f  milar to functio
+00007af0: 6e20 666f 7220 6044 6174 612e 6d61 7060  n for `Data.map`
+00007b00: 206d 6574 686f 642e 2041 646f 7074 6162   method. Adoptab
+00007b10: 6c65 2063 6f6d 6d61 6e64 7320 7573 6564  le commands used
+00007b20: 2069 7420 746f 2075 7064 6174 6520 7468   it to update th
+00007b30: 6520 6461 7461 2073 7472 6561 6d2e 0a20  e data stream.. 
+00007b40: 2020 2020 2020 202d 202a 2a41 6767 7265         - **Aggre
+00007b50: 6761 7465 206f 7065 7261 7469 6f6e 732a  gate operations*
+00007b60: 2a3a 0a20 2020 2020 2020 2020 2043 6f6d  *:.          Com
+00007b70: 6d6f 6e20 6f70 6572 6174 696f 6e73 2073  mon operations s
+00007b80: 7563 6820 6173 2066 696c 7465 722c 206d  uch as filter, m
+00007b90: 6170 2c20 6c69 6d69 7420 616e 6420 736f  ap, limit and so
+00007ba0: 206f 6e2e 0a20 2020 2020 2020 202d 202a   on..        - *
+00007bb0: 2a57 6f72 6b66 6c6f 772a 2a3a 2041 6e20  *Workflow**: An 
+00007bc0: 6f72 6465 7265 6420 7365 7420 6f66 205f  ordered set of _
+00007bd0: 4167 6772 6567 6174 6520 6f70 6572 6174  Aggregate operat
+00007be0: 696f 6e73 5f2e 0a20 2020 2020 2020 200a  ions_..        .
+00007bf0: 2020 2020 2020 2020 2323 2320 436f 6e63          ### Conc
+00007c00: 6570 740a 2020 2020 2020 2020 0a20 2020  ept.        .   
+00007c10: 2020 2020 2054 6865 206c 6962 7261 7279       The library
+00007c20: 2064 6573 6372 6962 6573 2074 6865 2068   describes the h
+00007c30: 6967 682d 6c65 7665 6c20 696e 7465 7266  igh-level interf
+00007c40: 6163 6573 2060 4953 6f75 7263 6541 5049  aces `ISourceAPI
+00007c50: 602c 2060 4944 6174 6153 6f75 7263 6560  `, `IDataSource`
+00007c60: 2c20 6049 436f 6d6d 616e 6460 2c20 6049  , `ICommand`, `I
+00007c70: 4164 6170 7465 7260 2e0a 2020 2020 2020  Adapter`..      
+00007c80: 2020 0a20 2020 2020 2020 2041 6e79 2064    .        Any d
+00007c90: 6174 6120 736f 7572 6365 206d 7573 7420  ata source must 
+00007ca0: 6265 2064 6573 6372 6962 6564 2062 7920  be described by 
+00007cb0: 7468 6520 6049 4461 7461 536f 7572 6365  the `IDataSource
+00007cc0: 6020 6162 7374 7261 6374 2063 6c61 7373  ` abstract class
+00007cd0: 2e20 5468 6573 6520 6361 6e20 6265 205f  . These can be _
+00007ce0: 4669 6c65 4461 7461 536f 7572 6365 5f2c  FileDataSource_,
+00007cf0: 0a20 2020 2020 2020 205f 4353 5644 6174  .        _CSVDat
+00007d00: 6153 6f75 7263 655f 2c20 5f44 4244 6174  aSource_, _DBDat
+00007d10: 6153 6f75 7263 655f 2061 6e64 206f 7468  aSource_ and oth
+00007d20: 6572 2e0a 2020 2020 2020 2020 0a20 2020  er..        .   
+00007d30: 2020 2020 2055 7375 616c 6c79 2c20 6461       Usually, da
+00007d40: 7461 2073 6f75 7263 6573 2068 6176 6520  ta sources have 
+00007d50: 736f 6d65 206b 696e 6420 6f66 2041 5049  some kind of API
+00007d60: 2e20 4461 7461 6261 7365 7320 2d20 7072  . Databases - pr
+00007d70: 6f76 6964 6520 5351 4c20 6c61 6e67 7561  ovide SQL langua
+00007d80: 6765 2c20 7768 656e 2077 6f72 6b69 6e67  ge, when working
+00007d90: 2077 6974 6820 6120 6669 6c65 2c20 796f   with a file, yo
+00007da0: 7520 6361 6e20 7265 6164 0a20 2020 2020  u can read.     
+00007db0: 2020 206c 696e 6520 6279 206c 696e 652c     line by line,
+00007dc0: 2065 7463 2e20 5468 6973 2041 5049 2069   etc. This API i
+00007dd0: 7320 6465 7363 7269 6265 6420 6279 2074  s described by t
+00007de0: 6865 2060 4953 6f75 7263 6541 5049 6020  he `ISourceAPI` 
+00007df0: 636c 6173 732e 2042 6563 6175 7365 2064  class. Because d
+00007e00: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
+00007e10: 7320 6f66 2074 6865 2073 616d 6520 6461  s of the same da
+00007e20: 7461 2073 6f75 7263 650a 2020 2020 2020  ta source.      
+00007e30: 2020 6d61 7920 6861 7665 2064 6966 6665    may have diffe
+00007e40: 7265 6e74 2041 5049 2c20 6974 2069 7320  rent API, it is 
+00007e50: 6265 7474 6572 2074 6f20 6372 6561 7465  better to create
+00007e60: 2061 2063 6c61 7373 2066 6f72 2065 6163   a class for eac
+00007e70: 6820 7665 7273 696f 6e2e 0a20 2020 2020  h version..     
+00007e80: 2020 200a 2020 2020 2020 2020 4765 6e65     .        Gene
+00007e90: 7261 6c6c 792c 2064 6174 6120 736f 7572  rally, data sour
+00007ea0: 6365 2041 5049 7320 6172 6520 6869 6464  ce APIs are hidd
+00007eb0: 656e 2062 6568 696e 6420 636f 6e76 656e  en behind conven
+00007ec0: 6965 6e74 2069 6e74 6572 6661 6365 732e  ient interfaces.
+00007ed0: 2054 6865 2072 6f6c 6520 6f66 2074 6865   The role of the
+00007ee0: 7365 2069 6e74 6572 6661 6365 7320 6973  se interfaces is
+00007ef0: 2070 6c61 7965 640a 2020 2020 2020 2020   played.        
+00007f00: 6279 2060 4943 6f6d 6d61 6e64 6020 636c  by `ICommand` cl
+00007f10: 6173 7365 732e 0a20 2020 2020 2020 200a  asses..        .
+00007f20: 2020 2020 2020 2020 6049 4164 6170 7465          `IAdapte
+00007f30: 7260 2063 6c61 7373 6573 2074 7261 6e73  r` classes trans
+00007f40: 666f 726d 2064 6174 6120 7374 7265 616d  form data stream
+00007f50: 206c 696b 6520 6675 6e63 7469 6f6e 7320   like functions 
+00007f60: 666f 7220 6044 6174 612e 6d61 7060 206d  for `Data.map` m
+00007f70: 6574 686f 642e 2045 7373 656e 7469 616c  ethod. Essential
+00007f80: 6c79 2069 7427 7320 7468 6520 7361 6d65  ly it's the same
+00007f90: 2074 6869 6e67 2062 7574 206d 6f72 650a   thing but more.
+00007fa0: 2020 2020 2020 2020 666c 6578 6962 6c65          flexible
+00007fb0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00007fc0: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
+00007fd0: 4c77 4450 2044 6174 6153 6f75 7263 6528  LwDP DataSource(
+00007fe0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007ff0: 6f6d 2f74 6832 2d6e 6574 2f74 6832 2d64  om/th2-net/th2-d
+00008000: 732d 736f 7572 6365 2d6c 7764 7029 2075  s-source-lwdp) u
+00008010: 7365 7320 7468 6573 6520 6162 7374 7261  ses these abstra
+00008020: 6374 2063 6c61 7373 6573 2074 6f20 6275  ct classes to bu
+00008030: 696c 6420 6974 7320 696d 706c 656d 656e  ild its implemen
+00008040: 7461 7469 6f6e 2e59 6f75 2063 616e 2065  tation.You can e
+00008050: 6173 696c 7920 6372 6561 7465 2079 6f75  asily create you
+00008060: 7220 6f77 6e20 756e 6971 7565 2063 6f6d  r own unique com
+00008070: 6d61 6e64 7320 666f 7220 5f4c 7744 5020  mands for _LwDP 
+00008080: 4461 7461 536f 7572 6365 5f2c 2061 7320  DataSource_, as 
+00008090: 7765 6c6c 2061 7320 656e 7469 7265 0a20  well as entire. 
+000080a0: 2020 2020 2020 205f 4461 7461 536f 7572         _DataSour
+000080b0: 6365 5f20 636c 6173 7365 732e 205b 4865  ce_ classes. [He
+000080c0: 7265 2069 7320 6120 646f 6375 6d65 6e74  re is a document
+000080d0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
+000080e0: 7469 6f6e 2f64 6174 6173 6f75 7263 652e  tion/datasource.
+000080f0: 6d64 2920 6f6e 2068 6f77 2074 6f20 696d  md) on how to im
+00008100: 706c 656d 656e 7420 7468 6573 6520 696e  plement these in
+00008110: 7465 7266 6163 6573 2e0a 2020 2020 2020  terfaces..      
+00008120: 2020 0a20 2020 2020 2020 2021 5b44 6174    .        ![Dat
+00008130: 6120 7374 7265 616d 2070 6970 656c 696e  a stream pipelin
+00008140: 655d 2864 6f63 756d 656e 7461 7469 6f6e  e](documentation
+00008150: 2f69 6d67 2f63 6f6e 6365 7074 2e70 6e67  /img/concept.png
+00008160: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00008170: 2020 2023 2323 2053 7472 6561 6d20 6f70     ### Stream op
+00008180: 6572 6174 696f 6e73 0a20 2020 2020 2020  erations.       
+00008190: 200a 2020 2020 2020 2020 4675 7274 6865   .        Furthe
+000081a0: 726d 6f72 652c 2073 7472 6561 6d20 6f70  rmore, stream op
+000081b0: 6572 6174 696f 6e73 2068 6176 6520 7477  erations have tw
+000081c0: 6f20 6675 6e64 616d 656e 7461 6c20 6368  o fundamental ch
+000081d0: 6172 6163 7465 7269 7374 6963 7320 7468  aracteristics th
+000081e0: 6174 206d 616b 6520 7468 656d 2076 6572  at make them ver
+000081f0: 7920 6469 6666 6572 656e 7420 6672 6f6d  y different from
+00008200: 2063 6f6c 6c65 6374 696f 6e0a 2020 2020   collection.    
+00008210: 2020 2020 6f70 6572 6174 696f 6e73 3a20      operations: 
+00008220: 5f50 6970 656c 696e 696e 675f 2061 6e64  _Pipelining_ and
+00008230: 205f 496e 7465 726e 616c 2069 7465 7261   _Internal itera
+00008240: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
+00008250: 2020 2020 2020 2020 2323 2323 2050 6970          #### Pip
+00008260: 656c 696e 696e 670a 2020 2020 2020 2020  elining.        
+00008270: 0a20 2020 2020 2020 204d 616e 7920 7374  .        Many st
+00008280: 7265 616d 206f 7065 7261 7469 6f6e 7320  ream operations 
+00008290: 7265 7475 726e 2061 2073 7472 6561 6d20  return a stream 
+000082a0: 7468 656d 7365 6c76 6573 2e20 5468 6973  themselves. This
+000082b0: 2061 6c6c 6f77 7320 6f70 6572 6174 696f   allows operatio
+000082c0: 6e73 2074 6f20 6265 2063 6861 696e 6564  ns to be chained
+000082d0: 2074 6f20 666f 726d 2061 206c 6172 6765   to form a large
+000082e0: 7220 7069 7065 6c69 6e65 2e0a 2020 2020  r pipeline..    
+000082f0: 2020 2020 0a20 2020 2020 2020 2021 5b44      .        ![D
+00008300: 6174 6120 7374 7265 616d 2070 6970 656c  ata stream pipel
+00008310: 696e 655d 2864 6f63 756d 656e 7461 7469  ine](documentati
+00008320: 6f6e 2f69 6d67 2f64 6174 615f 7374 7265  on/img/data_stre
+00008330: 616d 5f70 6970 656c 696e 652e 706e 6729  am_pipeline.png)
+00008340: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00008350: 2020 2323 2323 2049 6e74 6572 6e61 6c20    #### Internal 
+00008360: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
+00008370: 2020 0a20 2020 2020 2020 2049 6e20 636f    .        In co
+00008380: 6e74 7261 7374 2074 6f20 636f 6c6c 6563  ntrast to collec
+00008390: 7469 6f6e 732c 2077 6869 6368 2061 7265  tions, which are
+000083a0: 2069 7465 7261 7465 6420 6578 706c 6963   iterated explic
+000083b0: 6974 6c79 2028 6578 7465 726e 616c 2069  itly (external i
+000083c0: 7465 7261 7469 6f6e 292c 2073 7472 6561  teration), strea
+000083d0: 6d20 6f70 6572 6174 696f 6e73 2064 6f20  m operations do 
+000083e0: 7468 6520 6974 6572 6174 696f 6e0a 2020  the iteration.  
+000083f0: 2020 2020 2020 6265 6869 6e64 2074 6865        behind the
+00008400: 2073 6365 6e65 7320 666f 7220 796f 752e   scenes for you.
+00008410: 204e 6f74 652c 2069 7420 646f 6573 6e27   Note, it doesn'
+00008420: 7420 6d65 616e 2079 6f75 2063 616e 6e6f  t mean you canno
+00008430: 7420 6974 6572 6174 6520 7468 6520 5f44  t iterate the _D
+00008440: 6174 6120 6f62 6a65 6374 5f2e 0a20 2020  ata object_..   
+00008450: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00008460: 2020 2020 2020 2023 2323 2044 6174 6120         ### Data 
+00008470: 6974 6572 6174 696f 6e0a 2020 2020 2020  iteration.      
+00008480: 2020 0a20 2020 2020 2020 2054 6865 2044    .        The D
+00008490: 6174 6120 6f62 6a65 6374 2063 6f6e 7374  ata object const
+000084a0: 7275 6374 6f72 206d 6574 686f 6420 7461  ructor method ta
+000084b0: 6b65 7320 696e 2061 7320 6172 6775 6d65  kes in as argume
+000084c0: 6e74 2065 6974 6865 7220 616e 2069 7465  nt either an ite
+000084d0: 7261 746f 7220 6f76 6572 206f 626a 6563  rator over objec
+000084e0: 7473 206f 7220 6120 6765 6e65 7261 746f  ts or a generato
+000084f0: 7220 6675 6e63 7469 6f6e 2e0a 2020 2020  r function..    
+00008500: 2020 2020 5468 6520 4461 7461 206f 626a      The Data obj
+00008510: 6563 7420 6974 6572 6174 6f72 2068 616e  ect iterator han
+00008520: 646c 6573 2065 6163 6820 6974 656d 2069  dles each item i
+00008530: 6e20 7468 6973 2069 7465 7261 746f 7220  n this iterator 
+00008540: 6f72 2067 656e 6572 6174 6f72 2061 7320  or generator as 
+00008550: 7468 6579 2061 7265 2c20 6d65 616e 696e  they are, meanin
+00008560: 6720 6974 2064 6f65 736e 2774 2074 7279  g it doesn't try
+00008570: 2074 6f20 7265 6164 2074 6865 2063 6f6e   to read the con
+00008580: 7465 6e74 206f 6620 6974 656d 206f 7220  tent of item or 
+00008590: 7265 7475 726e 2074 6865 6d20 6d6f 6469  return them modi
+000085a0: 6669 6564 2069 6e20 616e 7920 7761 792c  fied in any way,
+000085b0: 2069 6e73 7465 6164 2072 6574 7572 6e73   instead returns
+000085c0: 2074 6865 2069 7465 6d20 6974 7365 6c66   the item itself
+000085d0: 2e0a 2020 2020 2020 2020 5468 6520 6f6e  ..        The on
+000085e0: 6c79 2065 7863 6570 7469 6f6e 2074 6f20  ly exception to 
+000085f0: 7468 6973 2069 7320 7768 656e 2044 6174  this is when Dat
+00008600: 6120 6f62 6a65 6374 2069 7320 6275 696c  a object is buil
+00008610: 7420 7573 696e 6720 6974 6572 6174 6f72  t using iterator
+00008620: 206f 7220 6765 6e65 7261 746f 7220 6f76   or generator ov
+00008630: 6572 206f 7468 6572 2044 6174 6120 6f62  er other Data ob
+00008640: 6a65 6374 732e 204e 6f74 6520 7468 6174  jects. Note that
+00008650: 2074 6869 7320 6974 6572 6174 6f72 206f   this iterator o
+00008660: 7220 6765 6e65 7261 746f 7220 6d75 7374  r generator must
+00008670: 206f 6e6c 7920 6265 2079 6965 6c64 696e   only be yieldin
+00008680: 6720 4461 7461 206f 626a 6563 7473 2061  g Data objects a
+00008690: 6e64 206e 6f74 6869 6e67 2065 6c73 652e  nd nothing else.
+000086a0: 2049 6620 7765 2062 7569 6c64 2066 726f   If we build fro
+000086b0: 6d20 6120 6d69 7820 6f66 2044 6174 6120  m a mix of Data 
+000086c0: 6f62 6a65 6374 7320 616e 6420 736f 6d65  objects and some
+000086d0: 206f 7468 6572 2074 7970 6573 2c20 4461   other types, Da
+000086e0: 7461 206f 626a 6563 7473 2720 636f 6e74  ta objects' cont
+000086f0: 656e 7420 776f 6e27 7420 6265 2072 6561  ent won't be rea
+00008700: 6420 616e 6420 696e 7374 6561 6420 6974  d and instead it
+00008710: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00008720: 6420 6173 2044 6174 6120 6f62 6a65 6374  d as Data object
+00008730: 2069 7473 656c 662e 0a20 2020 2020 2020   itself..       
+00008740: 200a 2020 2020 2020 2020 536d 616c 6c20   .        Small 
+00008750: 6578 616d 706c 6520 746f 2064 656d 6f6e  example to demon
+00008760: 7374 7261 7465 3a0a 2020 2020 2020 2020  strate:.        
+00008770: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
+00008780: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
+00008790: 7468 325f 6461 7461 5f73 6572 7669 6365  th2_data_service
+000087a0: 732e 6461 7461 2069 6d70 6f72 7420 4461  s.data import Da
+000087b0: 7461 0a20 2020 2020 2020 200a 2020 2020  ta.        .    
+000087c0: 2020 2020 6431 203d 2044 6174 6128 5b31      d1 = Data([1
+000087d0: 2c32 2c33 5d29 0a20 2020 2020 2020 2064  ,2,3]).        d
+000087e0: 3220 3d20 4461 7461 285b 342c 352c 365d  2 = Data([4,5,6]
+000087f0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00008800: 2020 206f 6e6c 795f 6461 7461 5f6f 626a     only_data_obj
+00008810: 6563 7473 203d 2044 6174 6128 5b64 312c  ects = Data([d1,
+00008820: 6432 5d29 2023 2057 696c 6c20 6974 6572  d2]) # Will iter
+00008830: 6174 6520 6173 2031 2c32 2c33 2c34 2c35  ate as 1,2,3,4,5
+00008840: 2c36 0a20 2020 2020 2020 2064 6174 615f  ,6.        data_
+00008850: 616e 645f 6c69 7374 203d 2044 6174 6128  and_list = Data(
+00008860: 5b64 312c 5b34 2c35 2c36 5d5d 2920 2320  [d1,[4,5,6]]) # 
+00008870: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00008880: 6431 2c20 5b34 2c35 2c36 5d0a 2020 2020  d1, [4,5,6].    
+00008890: 2020 2020 6461 7461 5f61 6e64 5f6e 756d      data_and_num
+000088a0: 6265 7273 203d 2044 6174 6128 5b64 312c  bers = Data([d1,
+000088b0: 342c 352c 365d 2920 2320 5769 6c6c 2069  4,5,6]) # Will i
+000088c0: 7465 7261 7465 2061 7320 6431 2c34 2c35  terate as d1,4,5
+000088d0: 2c36 0a20 2020 2020 2020 206c 6973 7473  ,6.        lists
+000088e0: 5f6f 6e6c 7920 3d20 4461 7461 285b 312c  _only = Data([1,
+000088f0: 322c 335d 2c5b 342c 352c 365d 2920 2320  2,3],[4,5,6]) # 
+00008900: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00008910: 5b31 2c32 2c33 5d2c 5b34 2c35 2c36 5d0a  [1,2,3],[4,5,6].
+00008920: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008930: 2023 2049 6620 7765 2077 616e 7420 746f   # If we want to
+00008940: 2069 7465 7261 7465 206f 7665 7220 636f   iterate over co
+00008950: 6e74 656e 7420 6f66 206c 6973 7420 6f66  ntent of list of
+00008960: 206c 6973 7473 2c20 7765 2073 686f 756c   lists, we shoul
+00008970: 6420 6669 7273 7420 6372 6561 7465 2044  d first create D
+00008980: 6174 6120 6f62 6a65 6374 7320 6672 6f6d  ata objects from
+00008990: 2074 6865 6d2c 0a20 2020 2020 2020 2023   them,.        #
+000089a0: 2074 6865 6e20 7573 6520 7468 656d 2074   then use them t
+000089b0: 6f20 636f 6e73 7472 7563 7420 6e65 7720  o construct new 
+000089c0: 4461 7461 206f 626a 6563 7420 6173 2069  Data object as i
+000089d0: 6e20 6361 7365 206f 6620 6431 2061 6e64  n case of d1 and
+000089e0: 2064 322c 2063 7265 6174 696e 6720 276f   d2, creating 'o
+000089f0: 6e6c 795f 6461 7461 5f6f 626a 6563 7473  nly_data_objects
+00008a00: 2720 696e 2074 6869 7320 6578 616d 706c  ' in this exampl
+00008a10: 652e 0a20 2020 2020 2020 2060 6060 0a20  e..        ```. 
+00008a20: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008a30: 200a 2020 2020 2020 2020 2323 2320 4461   .        ### Da
+00008a40: 7461 2063 6163 6869 6e67 0a20 2020 2020  ta caching.     
+00008a50: 2020 200a 2020 2020 2020 2020 5468 6520     .        The 
+00008a60: 5f44 6174 6120 6f62 6a65 6374 5f20 7072  _Data object_ pr
+00008a70: 6f76 6964 6573 2074 6865 2061 6269 6c69  ovides the abili
+00008a80: 7479 2074 6f20 7573 6520 7468 6520 6361  ty to use the ca
+00008a90: 6368 652e 2054 6865 2063 6163 6865 2077  che. The cache w
+00008aa0: 6f72 6b73 2066 6f72 2065 6163 6820 5f44  orks for each _D
+00008ab0: 6174 6120 6f62 6a65 6374 5f2c 2074 6861  ata object_, tha
+00008ac0: 7420 6973 2c20 796f 7520 6368 6f6f 7365  t is, you choose
+00008ad0: 0a20 2020 2020 2020 2077 6869 6368 205f  .        which _
+00008ae0: 4461 7461 206f 626a 6563 745f 2079 6f75  Data object_ you
+00008af0: 2077 616e 7420 746f 2073 6176 652e 2054   want to save. T
+00008b00: 6865 205f 4461 7461 206f 626a 6563 745f  he _Data object_
+00008b10: 2063 6163 6865 2069 7320 7361 7665 6420   cache is saved 
+00008b20: 6166 7465 7220 7468 6520 6669 7273 7420  after the first 
+00008b30: 6974 6572 6174 696f 6e2c 2062 7574 2074  iteration, but t
+00008b40: 6865 2069 7465 7261 7469 6f6e 0a20 2020  he iteration.   
+00008b50: 2020 2020 2073 6f75 7263 6520 6d61 7920       source may 
+00008b60: 6265 2064 6966 6665 7265 6e74 2e0a 2020  be different..  
+00008b70: 2020 2020 2020 0a20 2020 2020 2020 2049        .        I
+00008b80: 6620 796f 7520 646f 6e27 7420 7573 6520  f you don't use 
+00008b90: 7468 6520 6361 6368 652c 2079 6f75 7220  the cache, your 
+00008ba0: 736f 7572 6365 2077 696c 6c20 6265 2074  source will be t
+00008bb0: 6865 2064 6174 6120 736f 7572 6365 2079  he data source y
+00008bc0: 6f75 2068 6176 6520 696e 2074 6865 205f  ou have in the _
+00008bd0: 4461 7461 204f 626a 6563 745f 2e20 4275  Data Object_. Bu
+00008be0: 7420 6966 2079 6f75 2075 7365 2074 6865  t if you use the
+00008bf0: 2063 6163 6865 2c0a 2020 2020 2020 2020   cache,.        
+00008c00: 796f 7572 2073 6f75 7263 6520 6361 6e20  your source can 
+00008c10: 6265 2074 6865 2064 6174 6120 736f 7572  be the data sour
+00008c20: 6365 2c20 7468 6520 7061 7265 6e74 2063  ce, the parent c
+00008c30: 6163 6865 2c20 6f72 206f 776e 2063 6163  ache, or own cac
+00008c40: 6865 3a0a 2020 2020 2020 2020 0a20 2020  he:.        .   
+00008c50: 2020 2020 202a 2054 6865 2064 6174 6120       * The data 
+00008c60: 736f 7572 6365 3a0a 2020 2020 2020 2020  source:.        
+00008c70: 2020 4966 2074 6865 205f 4461 7461 204f    If the _Data O
+00008c80: 626a 6563 745f 2064 6f65 736e 2774 2068  bject_ doesn't h
+00008c90: 6176 6520 6120 7061 7265 6e74 2063 6163  ave a parent cac
+00008ca0: 6865 2061 6e64 2069 7473 2063 6163 6865  he and its cache
+00008cb0: 2e0a 2020 2020 2020 2020 2a20 5468 6520  ..        * The 
+00008cc0: 7061 7265 6e74 2063 6163 6865 3a0a 2020  parent cache:.  
+00008cd0: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
+00008ce0: 4461 7461 204f 626a 6563 745f 2068 6173  Data Object_ has
+00008cf0: 2061 2070 6172 656e 7420 6361 6368 652e   a parent cache.
+00008d00: 2049 7420 646f 6573 6e27 7420 6d61 7474   It doesn't matt
+00008d10: 6572 2077 6861 7420 706f 7369 7469 6f6e  er what position
+00008d20: 2074 6865 2070 6172 656e 7420 6361 6368   the parent cach
+00008d30: 6520 6861 7320 696e 2069 6e68 6572 6974  e has in inherit
+00008d40: 616e 6365 2e0a 2020 2020 2020 2020 2020  ance..          
+00008d50: 5f44 6174 6120 4f62 6a65 6374 5f20 756e  _Data Object_ un
+00008d60: 6465 7273 7461 6e64 7320 7768 6f73 6520  derstands whose 
+00008d70: 6361 6368 6520 6974 2069 7320 616e 6420  cache it is and 
+00008d80: 6578 6563 7574 6573 2074 6865 2070 6172  executes the par
+00008d90: 7420 6f66 2074 6865 2077 6f72 6b66 6c6f  t of the workflo
+00008da0: 7720 7468 6174 2077 6173 206e 6f74 2065  w that was not e
+00008db0: 7865 6375 7465 642e 0a20 2020 2020 2020  xecuted..       
+00008dc0: 202a 2054 6865 206f 776e 2063 6163 6865   * The own cache
+00008dd0: 3a0a 2020 2020 2020 2020 2020 4966 2069  :.          If i
+00008de0: 7420 6973 206e 6f74 2074 6865 2066 6972  t is not the fir
+00008df0: 7374 2069 7465 7261 7469 6f6e 206f 6620  st iteration of 
+00008e00: 7468 6973 2044 6174 6120 6f62 6a65 6374  this Data object
+00008e10: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008e20: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
+00008e30: 2063 6163 6865 2073 7461 7465 206f 6620   cache state of 
+00008e40: 7468 6520 4461 7461 206f 626a 6563 7420  the Data object 
+00008e50: 6973 206e 6f74 2069 6e68 6572 6974 6564  is not inherited
+00008e60: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008e70: 2020 2023 2323 2320 466f 7263 6564 2063     #### Forced c
+00008e80: 6163 6869 6e67 0a20 2020 2020 2020 2059  aching.        Y
+00008e90: 6f75 2063 616e 2074 656c 6c20 4453 2074  ou can tell DS t
+00008ea0: 6f20 6361 6368 6520 6461 7461 2074 6f20  o cache data to 
+00008eb0: 7370 6563 6966 6963 2063 6163 6865 2066  specific cache f
+00008ec0: 696c 652c 2077 6869 6368 2077 6f6e 2774  ile, which won't
+00008ed0: 2062 6520 6465 6c65 7465 6420 6166 7465   be deleted afte
+00008ee0: 7220 7363 7269 7074 2065 6e64 2e0a 2020  r script end..  
+00008ef0: 2020 2020 2020 596f 7520 6361 6e20 7365        You can se
+00008f00: 6520 6578 616d 706c 6520 696e 2031 2e31  e example in 1.1
+00008f10: 3220 7365 6374 696f 6e20 6f66 205b 6765  2 section of [ge
+00008f20: 745f 7374 6172 7465 645f 6578 616d 706c  t_started_exampl
+00008f30: 655d 2865 7861 6d70 6c65 732f 6765 745f  e](examples/get_
+00008f40: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
+00008f50: 7079 292e 0a20 2020 2020 2020 200a 2020  py)..        .  
+00008f60: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00008f70: 2323 2045 7665 6e74 5472 6565 2061 6e64  ## EventTree and
+00008f80: 2063 6f6c 6c65 6374 696f 6e73 0a20 2020   collections.   
+00008f90: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00008fa0: 2323 2045 7665 6e74 5472 6565 0a20 2020  ## EventTree.   
+00008fb0: 2020 2020 200a 2020 2020 2020 2020 6045       .        `E
+00008fc0: 7665 6e74 5472 6565 6020 6973 2061 2074  ventTree` is a t
+00008fd0: 7265 652d 6261 7365 6420 6461 7461 2073  ree-based data s
+00008fe0: 7472 7563 7475 7265 206f 6620 6576 656e  tructure of even
+00008ff0: 7473 2e20 4974 2061 6c6c 6f77 7320 796f  ts. It allows yo
+00009000: 7520 6765 7420 6368 696c 6472 656e 2061  u get children a
+00009010: 6e64 2070 6172 656e 7473 206f 6620 6576  nd parents of ev
+00009020: 656e 742c 0a20 2020 2020 2020 2064 6973  ent,.        dis
+00009030: 706c 6179 2074 7265 652c 2067 6574 2066  play tree, get f
+00009040: 756c 6c20 7061 7468 2074 6f20 6576 656e  ull path to even
+00009050: 7420 6574 632e 0a20 2020 2020 2020 200a  t etc..        .
+00009060: 2020 2020 2020 2020 4465 7461 696c 733a          Details:
+00009070: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00009080: 2020 2a20 6045 7665 6e74 5472 6565 6020    * `EventTree` 
+00009090: 636f 6e74 6169 6e73 2061 6c6c 2065 7665  contains all eve
+000090a0: 6e74 7320 696e 206d 656d 6f72 792e 0a20  nts in memory.. 
+000090b0: 2020 2020 2020 202a 2054 7265 6520 6861         * Tree ha
+000090c0: 7320 736f 6d65 2069 6d70 6f72 7461 6e74  s some important
+000090d0: 2074 6572 6d73 3a0a 2020 2020 2020 2020   terms:.        
+000090e0: 2020 2020 312e 205f 416e 6365 7374 6f72      1. _Ancestor
+000090f0: 5f20 6973 2061 6e79 2072 656c 6174 6976  _ is any relativ
+00009100: 6520 6f66 2074 6865 2065 7665 6e74 2075  e of the event u
+00009110: 7020 7468 6520 7472 6565 2028 6772 616e  p the tree (gran
+00009120: 6470 6172 656e 742c 2070 6172 656e 7420  dparent, parent 
+00009130: 6574 632e 292e 0a20 2020 2020 2020 2020  etc.)..         
+00009140: 2020 2032 2e20 5f50 6172 656e 745f 2069     2. _Parent_ i
+00009150: 7320 6f6e 6c79 2074 6865 2066 6972 7374  s only the first
+00009160: 2072 656c 6174 6976 6520 6f66 2074 6865   relative of the
+00009170: 2065 7665 6e74 2075 7020 7468 6520 7472   event up the tr
+00009180: 6565 2e0a 2020 2020 2020 2020 2020 2020  ee..            
+00009190: 332e 205f 4368 696c 645f 2069 7320 7468  3. _Child_ is th
+000091a0: 6520 6669 7273 7420 7265 6c61 7469 7665  e first relative
+000091b0: 206f 6620 7468 6520 6576 656e 7420 646f   of the event do
+000091c0: 776e 2074 6865 2074 7265 652e 0a20 2020  wn the tree..   
+000091d0: 2020 2020 200a 2020 2020 2020 2020 5461       .        Ta
+000091e0: 6b65 2061 206c 6f6f 6b20 6174 2074 6865  ke a look at the
+000091f0: 2066 6f6c 6c6f 7769 6e67 2048 544d 4c20   following HTML 
+00009200: 7472 6565 2074 6f20 756e 6465 7273 7461  tree to understa
+00009210: 6e64 2074 6865 6d2e 0a20 2020 2020 2020  nd them..       
+00009220: 200a 2020 2020 2020 2020 2020 2060 6060   .           ```
+00009230: 0a20 2020 2020 2020 2020 2020 203c 626f  .            <bo
+00009240: 6479 3e20 3c21 2d2d 2061 6e63 6573 746f  dy> <!-- ancesto
+00009250: 7220 2867 7261 6e64 7061 7265 6e74 292c  r (grandparent),
+00009260: 2062 7574 206e 6f74 2070 6172 656e 7420   but not parent 
+00009270: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
+00009280: 2020 2020 3c64 6976 3e20 3c21 2d2d 2070      <div> <!-- p
+00009290: 6172 656e 7420 2620 616e 6365 7374 6f72  arent & ancestor
+000092a0: 202d 2d3e 0a20 2020 2020 2020 2020 2020   -->.           
+000092b0: 2020 2020 2020 2020 203c 703e 4865 6c6c           <p>Hell
+000092c0: 6f2c 2077 6f72 6c64 213c 2f70 3e20 3c21  o, world!</p> <!
+000092d0: 2d2d 2063 6869 6c64 202d 2d3e 0a20 2020  -- child -->.   
+000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092f0: 203c 703e 476f 6f64 6279 6521 3c2f 703e   <p>Goodbye!</p>
+00009300: 203c 212d 2d20 7369 626c 696e 6720 2d2d   <!-- sibling --
+00009310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00009320: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00009330: 2020 2020 203c 2f62 6f64 793e 0a20 2020       </body>.   
+00009340: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00009350: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00009360: 2320 436f 6c6c 6563 7469 6f6e 730a 2020  # Collections.  
+00009370: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
+00009380: 2a45 7665 6e74 5472 6565 436f 6c6c 6563  *EventTreeCollec
+00009390: 7469 6f6e 2a2a 2069 7320 6120 636f 6c6c  tion** is a coll
+000093a0: 6563 7469 6f6e 206f 6620 4576 656e 7454  ection of EventT
+000093b0: 7265 6573 2e20 5468 6520 636f 6c6c 6563  rees. The collec
+000093c0: 7469 6f6e 2062 7569 6c64 7320 6120 6665  tion builds a fe
+000093d0: 7720 5f45 7665 6e74 5472 6565 5f20 6279  w _EventTree_ by
+000093e0: 2070 6173 7365 6420 5f44 6174 610a 2020   passed _Data.  
+000093f0: 2020 2020 2020 6f62 6a65 6374 5f2e 2041        object_. A
+00009400: 6c74 686f 7567 6820 796f 7520 6361 6e20  lthough you can 
+00009410: 6368 616e 6765 2074 6865 2074 7265 6520  change the tree 
+00009420: 6469 7265 6374 6c79 2c20 6974 2773 2062  directly, it's b
+00009430: 6574 7465 7220 746f 2064 6f20 6974 2074  etter to do it t
+00009440: 6872 6f75 6768 2063 6f6c 6c65 6374 696f  hrough collectio
+00009450: 6e73 2062 6563 6175 7365 2074 6865 7920  ns because they 
+00009460: 6172 6520 6177 6172 6520 6f66 0a20 2020  are aware of.   
+00009470: 2020 2020 2060 6465 7461 6368 6564 5f65       `detached_e
+00009480: 7665 6e74 7360 2061 6e64 2063 616e 2073  vents` and can s
+00009490: 6f6c 7665 2073 6f6d 6520 6576 656e 7473  olve some events
+000094a0: 2064 6570 656e 6465 6e63 6965 732e 2054   dependencies. T
+000094b0: 6865 2063 6f6c 6c65 6374 696f 6e20 6861  he collection ha
+000094c0: 7320 7369 6d69 6c61 7220 6665 6174 7572  s similar featur
+000094d0: 6573 206c 696b 6520 6120 7369 6e67 6c65  es like a single
+000094e0: 205f 4576 656e 7454 7265 655f 0a20 2020   _EventTree_.   
+000094f0: 2020 2020 2062 7574 2061 7070 6c79 696e       but applyin
+00009500: 6720 7468 656d 2066 6f72 2061 6c6c 205f  g them for all _
+00009510: 4576 656e 7454 7265 6573 5f2e 0a20 2020  EventTrees_..   
+00009520: 2020 2020 200a 2020 2020 2020 2020 2a2a       .        **
+00009530: 5061 7265 6e74 4576 656e 7454 7265 6543  ParentEventTreeC
+00009540: 6f6c 6c65 6374 696f 6e2a 2a20 6973 2061  ollection** is a
+00009550: 2063 6f6c 6c65 6374 696f 6e20 7369 6d69   collection simi
+00009560: 6c61 7220 746f 205f 4576 656e 7454 7265  lar to _EventTre
+00009570: 6543 6f6c 6c65 6374 696f 6e5f 2062 7574  eCollection_ but
+00009580: 2063 6f6e 7461 696e 696e 6720 6f6e 6c79   containing only
+00009590: 2070 6172 656e 7420 6576 656e 7473 2074   parent events t
+000095a0: 6861 740a 2020 2020 2020 2020 6172 6520  hat.        are 
+000095b0: 7265 6665 7265 6e63 6564 2069 6e20 7468  referenced in th
+000095c0: 6520 6461 7461 2073 7472 6561 6d2e 2054  e data stream. T
+000095d0: 6865 2063 6f6c 6c65 6374 696f 6e20 6861  he collection ha
+000095e0: 7320 6665 6174 7572 6573 2073 696d 696c  s features simil
+000095f0: 6172 2074 6f20 5f45 7665 6e74 5472 6565  ar to _EventTree
+00009600: 436f 6c6c 6563 7469 6f6e 5f2e 0a20 2020  Collection_..   
+00009610: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
+00009620: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
+00009630: 2020 2020 2020 2020 2a20 546f 2075 7365          * To use
+00009640: 2045 5420 636f 6c6c 6563 7469 6f6e 7320   ET collections 
+00009650: 796f 7520 6e65 6564 2074 6f20 696e 6974  you need to init
+00009660: 6961 6c69 7a65 2074 6865 6d20 6279 205f  ialize them by _
+00009670: 4554 4344 7269 7665 725f 2e20 4461 7461  ETCDriver_. Data
+00009680: 2073 6f75 7263 6573 2075 7375 616c 6c79   sources usually
+00009690: 2070 726f 7669 6465 2074 6865 6d2e 0a20   provide them.. 
+000096a0: 2020 2020 2020 2020 2059 6f75 2063 616e           You can
+000096b0: 2063 7265 6174 6520 6974 2062 7920 796f   create it by yo
+000096c0: 7572 7365 6c66 2064 6570 656e 6469 6e67  urself depending
+000096d0: 206f 6e20 796f 7572 2064 6174 6120 7374   on your data st
+000096e0: 7275 6374 7572 652e 0a20 2020 2020 2020  ructure..       
+000096f0: 202a 2054 6865 2063 6f6c 6c65 6374 696f   * The collectio
+00009700: 6e20 6861 7320 6120 6665 6174 7572 6520  n has a feature 
+00009710: 746f 2072 6563 6f76 6572 2065 7665 6e74  to recover event
+00009720: 732e 2041 6c6c 2065 7665 6e74 7320 7468  s. All events th
+00009730: 6174 2061 7265 206e 6f74 2069 6e20 7468  at are not in th
+00009740: 6520 7265 6365 6976 6564 2064 6174 6120  e received data 
+00009750: 7374 7265 616d 2c20 6275 7420 7768 6963  stream, but whic
+00009760: 6820 6172 650a 2020 2020 2020 2020 2020  h are.          
+00009770: 7265 6665 7265 6e63 6564 2077 696c 6c20  referenced will 
+00009780: 6265 206c 6f61 6465 6420 6672 6f6d 2074  be loaded from t
+00009790: 6865 2064 6174 6120 736f 7572 6365 2e0a  he data source..
+000097a0: 2020 2020 2020 2020 2a20 596f 7520 6361          * You ca
+000097b0: 6e20 7461 6b65 2060 6465 7461 6368 6564  n take `detached
+000097c0: 5f65 7665 6e74 7360 2074 6f20 7365 6520  _events` to see 
+000097d0: 7768 6963 6820 6576 656e 7473 2061 7265  which events are
+000097e0: 206d 6973 7369 6e67 2e0a 2020 2020 2020   missing..      
+000097f0: 2020 2a20 4966 2079 6f75 2077 616e 742c    * If you want,
+00009800: 2079 6f75 2063 616e 2062 7569 6c64 2070   you can build p
+00009810: 6172 656e 746c 6573 7320 7472 6565 7320  arentless trees 
+00009820: 7768 6572 6520 7468 6520 6d69 7373 696e  where the missin
+00009830: 6720 6576 656e 7473 2061 7265 2073 7475  g events are stu
+00009840: 6262 6564 2069 6e73 7465 6164 2e20 4a75  bbed instead. Ju
+00009850: 7374 0a20 2020 2020 2020 2020 2075 7365  st.          use
+00009860: 2060 6765 745f 7061 7265 6e74 6c65 7373   `get_parentless
+00009870: 5f74 7265 6573 2829 602e 0a20 2020 2020  _trees()`..     
+00009880: 2020 200a 2020 2020 2020 2020 5265 7175     .        Requ
+00009890: 6972 656d 656e 7473 3a0a 2020 2020 2020  irements:.      
+000098a0: 2020 0a20 2020 2020 2020 2031 2e20 4576    .        1. Ev
+000098b0: 656e 7473 2070 726f 7669 6465 6420 746f  ents provided to
+000098c0: 2045 5443 2068 6176 6520 746f 2068 6176   ETC have to hav
+000098d0: 6520 6065 7665 6e74 5f6e 616d 6560 2c20  e `event_name`, 
+000098e0: 6065 7665 6e74 5f69 6460 2c20 6070 6172  `event_id`, `par
+000098f0: 656e 745f 6576 656e 745f 6964 6020 6669  ent_event_id` fi
+00009900: 656c 6473 2e20 5468 6579 0a20 2020 2020  elds. They.     
+00009910: 2020 2063 616e 2068 6176 6520 616e 6f74     can have anot
+00009920: 6865 7220 6e61 6d65 7320 2869 7420 7265  her names (it re
+00009930: 736f 6c76 6573 2069 6e20 7468 6520 6472  solves in the dr
+00009940: 6976 6572 292e 0a20 2020 2020 2020 200a  iver)..        .
+00009950: 2020 2020 2020 2020 2323 2323 2048 696e          #### Hin
+00009960: 7473 0a20 2020 2020 2020 200a 2020 2020  ts.        .    
+00009970: 2020 2020 2a20 5265 6d6f 7665 2061 6c6c      * Remove all
+00009980: 2075 6e6e 6563 6573 7361 7279 2066 6965   unnecessary fie
+00009990: 6c64 7320 6672 6f6d 2065 7665 6e74 7320  lds from events 
+000099a0: 6265 666f 7265 2070 6173 7369 6e67 2074  before passing t
+000099b0: 6f20 6120 5f63 6f6c 6c65 6374 696f 6e5f  o a _collection_
+000099c0: 2074 6f20 7265 6475 6365 206d 656d 6f72   to reduce memor
+000099d0: 7920 7573 6167 652e 0a20 2020 2020 2020  y usage..       
+000099e0: 202a 2055 7365 2060 7368 6f77 2829 6020   * Use `show()` 
+000099f0: 6d65 7468 6f64 2074 6f20 7072 696e 7420  method to print 
+00009a00: 7468 6520 7472 6565 2069 6e20 7472 6565  the tree in tree
+00009a10: 2d6c 696b 6520 7669 6577 2e0a 2020 2020  -like view..    
+00009a20: 2020 2020 2a20 4e6f 7465 2074 6861 7420      * Note that 
+00009a30: 7468 6520 6067 6574 5f78 6020 6d65 7468  the `get_x` meth
+00009a40: 6f64 7320 7769 6c6c 2072 6169 7365 2061  ods will raise a
+00009a50: 6e20 6578 6365 7074 696f 6e20 6966 2079  n exception if y
+00009a60: 6f75 2070 6173 7320 616e 2075 6e6b 6e6f  ou pass an unkno
+00009a70: 776e 2065 7665 6e74 2069 642c 2075 6e6c  wn event id, unl
+00009a80: 696b 6520 7468 6520 6066 696e 645f 7860  ike the `find_x`
+00009a90: 206d 6574 686f 6473 2028 0a20 2020 2020   methods (.     
+00009aa0: 2020 2020 2074 6865 7920 7265 7475 726e       they return
+00009ab0: 204e 6f6e 6529 2e0a 2020 2020 2020 2020   None)..        
+00009ac0: 2a20 4966 2079 6f75 2077 616e 7420 746f  * If you want to
+00009ad0: 206b 6e6f 7720 7468 6174 2073 7065 6369   know that speci
+00009ae0: 6669 6564 2065 7665 6e74 2065 7869 7374  fied event exist
+00009af0: 732c 2075 7365 2074 6865 2070 7974 686f  s, use the pytho
+00009b00: 6e20 6069 6e60 206b 6579 776f 7264 2028  n `in` keyword (
+00009b10: 652e 672e 2060 2765 7665 6e74 2d69 6427  e.g. `'event-id'
+00009b20: 2069 6e20 6576 656e 7473 5f74 7265 6560   in events_tree`
+00009b30: 292e 0a20 2020 2020 2020 202a 2055 7365  )..        * Use
+00009b40: 2074 6865 2070 7974 686f 6e20 606c 656e   the python `len
+00009b50: 6020 6b65 7977 6f72 6420 746f 2067 6574  ` keyword to get
+00009b60: 2065 7665 6e74 7320 6e75 6d62 6572 2069   events number i
+00009b70: 6e20 7468 6520 7472 6565 2e0a 2020 2020  n the tree..    
+00009b80: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00009b90: 2046 6965 6c64 2052 6573 6f6c 7665 7273   Field Resolvers
+00009ba0: 0a20 2020 2020 2020 2049 6e74 6572 6661  .        Interfa
+00009bb0: 6365 2063 616e 2062 6520 666f 756e 6420  ce can be found 
+00009bc0: 696e 2060 7468 325f 6461 7461 5f73 6572  in `th2_data_ser
+00009bd0: 7669 6365 732f 696e 7465 7266 6163 6573  vices/interfaces
+00009be0: 2f75 7469 6c73 2f72 6573 6f6c 7665 722e  /utils/resolver.
+00009bf0: 7079 602e 2020 0a20 2020 2020 2020 2041  py`.  .        A
+00009c00: 6c6c 2064 6174 612d 736f 7572 6365 7320  ll data-sources 
+00009c10: 7368 6f75 6c64 2069 6d70 6c65 6d65 6e74  should implement
+00009c20: 2074 6865 6d2e 0a20 2020 2020 2020 200a   them..        .
+00009c30: 2020 2020 2020 2020 5468 6520 6964 6561          The idea
+00009c40: 206f 6620 7573 696e 6720 7265 736f 6c76   of using resolv
+00009c50: 6572 733a 0a20 2020 2020 2020 2049 7420  ers:.        It 
+00009c60: 736f 6c76 6573 2074 6865 2070 726f 626c  solves the probl
+00009c70: 656d 206f 6620 6861 7669 6e67 2061 2066  em of having a f
+00009c80: 6577 2044 6174 6153 6f75 7263 6573 2077  ew DataSources w
+00009c90: 6974 6820 7369 6d69 6c61 7220 6461 7461  ith similar data
+00009ca0: 2c0a 2020 2020 2020 2020 6275 7420 7769  ,.        but wi
+00009cb0: 7468 2064 6966 6665 7265 6e74 2077 6179  th different way
+00009cc0: 7320 746f 2067 6574 2069 742e 0a20 2020  s to get it..   
+00009cd0: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00009ce0: 6573 6520 636c 6173 7365 7320 7072 6f76  ese classes prov
+00009cf0: 6964 6520 796f 7520 6765 7474 6572 206d  ide you getter m
+00009d00: 6574 686f 6473 2e0a 2020 2020 2020 2020  ethods..        
+00009d10: 5573 696e 6720 7468 6573 6520 636c 6173  Using these clas
+00009d20: 7365 7320 616c 6c6f 7773 2079 6f75 2074  ses allows you t
+00009d30: 6f20 6672 6565 6c79 2073 7769 7463 6820  o freely switch 
+00009d40: 6265 7477 6565 6e20 6469 6666 6572 656e  between differen
+00009d50: 7420 6461 7461 0a20 2020 2020 2020 2066  t data.        f
+00009d60: 6f72 6d61 7473 2061 6e64 2064 6f6e 2774  ormats and don't
+00009d70: 2063 6861 6e67 6520 796f 7572 2063 6f64   change your cod
+00009d80: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+00009d90: 2020 2020 5265 736f 6c76 6572 7320 736f      Resolvers so
+00009da0: 6c76 6520 7468 6520 7072 6f62 6c65 6d20  lve the problem 
+00009db0: 6f66 2064 6174 612d 666f 726d 6174 206d  of data-format m
+00009dc0: 6967 7261 7469 6f6e 2e0a 2020 2020 2020  igration..      
+00009dd0: 2020 2d20 6669 656c 6473 2070 6c61 6365    - fields place
+00009de0: 2063 616e 2062 6520 6368 616e 6765 640a   can be changed.
+00009df0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
+00009e00: 206e 616d 6573 2063 616e 2062 6520 6368   names can be ch
+00009e10: 616e 6765 640a 2020 2020 2020 2020 0a20  anged.        . 
+00009e20: 2020 2020 2020 2052 6573 6f6c 7665 7273         Resolvers
+00009e30: 2063 616e 2077 6f72 6b20 6f6e 6c79 2077   can work only w
+00009e40: 6974 6820 6f6e 6520 6576 656e 742f 6d65  ith one event/me
+00009e50: 7373 6167 652e 0a20 2020 2020 2020 2049  ssage..        I
+00009e60: 7420 6d65 616e 732c 2069 6620 796f 7572  t means, if your
+00009e70: 206d 6573 7361 6765 2068 6173 2073 7562   message has sub
+00009e80: 2d6d 6573 7361 6765 7320 286c 696b 6520  -messages (like 
+00009e90: 7468 322d 6d65 7373 6167 6573 2069 6e20  th2-messages in 
+00009ea0: 6c77 6470 2920 6974 200a 2020 2020 2020  lwdp) it .      
+00009eb0: 2020 776f 6e27 7420 776f 726b 2c20 6265    won't work, be
+00009ec0: 6361 7573 6520 7265 736f 6c76 6572 2077  cause resolver w
+00009ed0: 696c 6c20 6e6f 7420 6b6e 6f77 2077 6974  ill not know wit
+00009ee0: 6820 7768 6963 6820 7375 622d 6d65 7373  h which sub-mess
+00009ef0: 6167 6520 7368 6f75 6c64 2069 7420 776f  age should it wo
+00009f00: 726b 2e20 0a20 2020 2020 2020 200a 2020  rk. .        .  
+00009f10: 2020 2020 2020 2a2a 576f 726b 6172 6f75        **Workarou
+00009f20: 6e64 2a2a 2020 0a20 2020 2020 2020 2031  nd**  .        1
+00009f30: 2e20 4578 7061 6e64 2061 6c6c 2079 6f75  . Expand all you
+00009f40: 7220 6d65 7373 6167 6573 202d 3e20 606e  r messages -> `n
+00009f50: 6577 5f64 203d 2079 6f75 725f 6461 7461  ew_d = your_data
+00009f60: 2e6d 6170 284d 6573 7361 6765 4669 656c  .map(MessageFiel
+00009f70: 6452 6573 6f6c 7665 722e 6578 7061 6e64  dResolver.expand
+00009f80: 5f6d 6573 7361 6765 2960 0a20 2020 2020  _message)`.     
+00009f90: 2020 2032 2e20 5573 6520 6045 7870 616e     2. Use `Expan
+00009fa0: 6465 644d 6573 7361 6765 4669 656c 6452  dedMessageFieldR
+00009fb0: 6573 6f6c 7665 7260 2069 6e73 7465 6164  esolver` instead
+00009fc0: 206f 6620 7573 7561 6c20 604d 6573 7361   of usual `Messa
+00009fd0: 6765 4669 656c 6452 6573 6f6c 7665 7260  geFieldResolver`
+00009fe0: 2077 6865 6e20 0a20 2020 2020 2020 2020   when .         
+00009ff0: 2020 2079 6f75 2074 616b 6520 6669 656c     you take fiel
+0000a000: 6473 2066 6f72 2065 7870 616e 6465 6420  ds for expanded 
+0000a010: 6d65 7373 6167 6573 2e0a 2020 2020 2020  messages..      
+0000a020: 2020 0a20 2020 2020 2020 202a 2a49 6d70    .        **Imp
+0000a030: 6c65 6d65 6e74 6174 696f 6e20 6164 7669  lementation advi
+0000a040: 6365 3a2a 2a0a 2020 2020 2020 2020 312e  ce:**.        1.
+0000a050: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+0000a060: 656e 7465 6445 7272 6f72 202d 2d20 6966  entedError -- if
+0000a070: 2079 6f75 7220 496d 706c 656d 656e 7461   your Implementa
+0000a080: 7469 6f6e 2064 6f65 736e 2774 2073 7570  tion doesn't sup
+0000a090: 706f 7274 2074 6869 7320 6765 7474 6572  port this getter
+0000a0a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a0b0: 2020 202a 2a50 6572 666f 726d 616e 6365     **Performance
+0000a0c0: 2069 6d70 6163 743a 2a2a 0a20 2020 2020   impact:**.     
+0000a0d0: 2020 202d 2049 7420 6120 6269 7420 736c     - It a bit sl
+0000a0e0: 6f77 6572 2074 6861 6e20 7573 696e 6720  ower than using 
+0000a0f0: 6e61 6b65 6420 6669 656c 6420 6163 6365  naked field acce
+0000a100: 7373 2060 6469 6374 5b27 6b65 7927 5d60  ss `dict['key']`
+0000a110: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a120: 2020 2023 2320 322e 342e 204c 696e 6b73     ## 2.4. Links
+0000a130: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+0000a140: 2020 2d20 5b52 6570 6f72 7420 4461 7461    - [Report Data
+0000a150: 2050 726f 7669 6465 725d 2868 7474 7073   Provider](https
+0000a160: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+0000a170: 322d 6e65 742f 7468 322d 7270 742d 6461  2-net/th2-rpt-da
+0000a180: 7461 2d70 726f 7669 6465 7229 0a20 2020  ta-provider).   
+0000a190: 2020 2020 202d 205b 5468 3220 4461 7461       - [Th2 Data
+0000a1a0: 2053 6572 7669 6365 7320 5574 696c 735d   Services Utils]
+0000a1b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+0000a1c0: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+0000a1d0: 6461 7461 2d73 6572 7669 6365 732d 7574  data-services-ut
+0000a1e0: 696c 7329 0a20 2020 2020 2020 200a 2020  ils).        .  
+0000a1f0: 2020 2020 2020 2320 332e 2042 6573 7420        # 3. Best 
+0000a200: 7072 6163 7469 6365 730a 2020 2020 2020  practices.      
+0000a210: 2020 4465 7065 6e64 696e 6720 6f6e 2068    Depending on h
+0000a220: 6f77 2079 6f75 2077 6f72 6b20 7769 7468  ow you work with
+0000a230: 2060 4461 7461 206f 626a 6563 7460 2c20   `Data object`, 
+0000a240: 6974 2063 616e 2062 6520 736c 6f77 206f  it can be slow o
+0000a250: 6620 6661 7374 2e0a 2020 2020 2020 2020  f fast..        
+0000a260: 4173 2077 6974 6820 6120 7265 6c61 7469  As with a relati
+0000a270: 6f6e 616c 2064 6174 6162 6173 652c 2079  onal database, y
+0000a280: 6f75 2063 616e 2077 7269 7465 2061 2071  ou can write a q
+0000a290: 7565 7279 2074 6861 7420 7769 6c6c 2072  uery that will r
+0000a2a0: 6574 7572 6e20 6461 7461 2073 6c6f 776c  eturn data slowl
+0000a2b0: 7920 6f72 2071 7569 636b 6c79 2c0a 2020  y or quickly,.  
+0000a2c0: 2020 2020 2020 7468 6520 7361 6d65 2077        the same w
+0000a2d0: 6865 6e20 776f 726b 696e 6720 7769 7468  hen working with
+0000a2e0: 2061 2060 4461 7461 206f 626a 6563 7460   a `Data object`
+0000a2f0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a300: 2020 2046 6f6c 6c6f 7720 7468 6520 7275     Follow the ru
+0000a310: 6c65 7320 746f 206d 616b 6520 796f 7572  les to make your
+0000a320: 2077 6f72 6b20 7769 7468 2044 6174 6120   work with Data 
+0000a330: 6f62 6a65 6374 2066 6173 743a 0a20 2020  object fast:.   
+0000a340: 2020 2020 2031 2e20 5573 6520 6044 6174       1. Use `Dat
+0000a350: 612e 7573 655f 6361 6368 6528 2960 2069  a.use_cache()` i
+0000a360: 6620 796f 7520 6974 6572 6174 6520 6461  f you iterate da
+0000a370: 7461 206d 6f72 6520 7468 616e 206f 6e65  ta more than one
+0000a380: 2074 696d 652e 0a20 2020 2020 2020 2032   time..        2
+0000a390: 2e20 5472 7920 746f 2064 6f6e 2774 2069  . Try to don't i
+0000a3a0: 7465 7261 7465 206f 6e65 2060 4461 7461  terate one `Data
+0000a3b0: 206f 626a 6563 7460 2069 6e73 6964 6520   object` inside 
+0000a3c0: 7468 6520 6f74 6865 7220 6f6e 652e 0a20  the other one.. 
+0000a3d0: 2020 2020 2020 2020 2020 4966 2079 6f75            If you
+0000a3e0: 2073 686f 756c 6420 746f 2064 6f20 6974   should to do it
+0000a3f0: 2c20 7573 6520 7368 6f72 7420 6044 6174  , use short `Dat
+0000a400: 6120 6f62 6a65 6374 6020 6669 7273 7420  a object` first 
+0000a410: 616e 6420 6c6f 6e67 2060 4461 7461 206f  and long `Data o
+0000a420: 626a 6563 7460 2069 6e73 6964 6520 7468  bject` inside th
+0000a430: 6520 6c6f 6f70 2e0a 2020 2020 2020 2020  e loop..        
+0000a440: 2020 2049 7427 6c6c 2061 6c6c 6f77 2079     It'll allow y
+0000a450: 6f75 206f 7065 6e20 7468 6520 6361 6368  ou open the cach
+0000a460: 6520 6669 6c65 206f 7220 6372 6561 7465  e file or create
+0000a470: 2061 2072 6571 7565 7374 2074 6f20 6044   a request to `D
+0000a480: 6174 6120 736f 7572 6365 6020 6c65 7373  ata source` less
+0000a490: 206e 756d 6265 7220 6f66 2074 696d 6573   number of times
+0000a4a0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+0000a4b0: 2020 2023 2034 2e20 4f66 6669 6369 616c     # 4. Official
+0000a4c0: 2044 6174 6153 6f75 7263 6520 696d 706c   DataSource impl
+0000a4d0: 656d 656e 7461 7469 6f6e 730a 2020 2020  ementations.    
+0000a4e0: 2020 2020 0a20 2020 2020 2020 202d 205b      .        - [
+0000a4f0: 4c69 6768 7477 6569 6768 7420 4461 7461  Lightweight Data
+0000a500: 2050 726f 7669 6465 7220 4461 7461 2053   Provider Data S
+0000a510: 6f75 7263 655d 2868 7474 7073 3a2f 2f67  ource](https://g
+0000a520: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
+0000a530: 742f 7468 322d 6473 2d73 6f75 7263 652d  t/th2-ds-source-
+0000a540: 6c77 6470 290a 2020 2020 2020 2020 0a20  lwdp).        . 
+0000a550: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000a560: 2320 352e 2041 5049 0a20 2020 2020 2020  # 5. API.       
+0000a570: 200a 2020 2020 2020 2020 4966 2079 6f75   .        If you
+0000a580: 2061 7265 206c 6f6f 6b69 6e67 2066 6f72   are looking for
+0000a590: 2063 6c61 7373 6573 2064 6573 6372 6970   classes descrip
+0000a5a0: 7469 6f6e 2073 6565 2074 6865 205b 4150  tion see the [AP
+0000a5b0: 4920 446f 6375 6d65 6e74 6174 696f 6e5d  I Documentation]
+0000a5c0: 2864 6f63 756d 656e 7461 7469 6f6e 2f61  (documentation/a
+0000a5d0: 7069 2f69 6e64 6578 2e6d 6429 2e0a 2020  pi/index.md)..  
+0000a5e0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+0000a5f0: 2036 2e20 4578 616d 706c 6573 0a20 2020   6. Examples.   
+0000a600: 2020 2020 200a 2020 2020 2020 2020 2d20       .        - 
+0000a610: 5b67 6574 5f73 7461 7274 6564 5f65 7861  [get_started_exa
+0000a620: 6d70 6c65 2e70 795d 2865 7861 6d70 6c65  mple.py](example
+0000a630: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
+0000a640: 616d 706c 652e 7079 290a 2020 2020 2020  ample.py).      
+0000a650: 2020 0a50 6c61 7466 6f72 6d3a 2055 4e4b    .Platform: UNK
+0000a660: 4e4f 574e 0a52 6571 7569 7265 732d 5079  NOWN.Requires-Py
+0000a670: 7468 6f6e 3a20 3e3d 332e 380a 4465 7363  thon: >=3.8.Desc
+0000a680: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+0000a690: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+0000a6a0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
+0000a6b0: 7261 3a20 7264 700a 5072 6f76 6964 6573  ra: rdp.Provides
+0000a6c0: 2d45 7874 7261 3a20 7264 7035 0a50 726f  -Extra: rdp5.Pro
+0000a6d0: 7669 6465 732d 4578 7472 613a 2072 6470  vides-Extra: rdp
+0000a6e0: 360a 5072 6f76 6964 6573 2d45 7874 7261  6.Provides-Extra
+0000a6f0: 3a20 6c77 6470 0a50 726f 7669 6465 732d  : lwdp.Provides-
+0000a700: 4578 7472 613a 206c 7764 7031 0a50 726f  Extra: lwdp1.Pro
+0000a710: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
+0000a720: 7032 0a50 726f 7669 6465 732d 4578 7472  p2.Provides-Extr
+0000a730: 613a 206c 7764 7033 0a50 726f 7669 6465  a: lwdp3.Provide
+0000a740: 732d 4578 7472 613a 206c 7764 702d 6465  s-Extra: lwdp-de
+0000a750: 760a 5072 6f76 6964 6573 2d45 7874 7261  v.Provides-Extra
+0000a760: 3a20 7574 696c 732d 7270 742d 7669 6577  : utils-rpt-view
+0000a770: 6572 0a50 726f 7669 6465 732d 4578 7472  er.Provides-Extr
+0000a780: 613a 2075 7469 6c73 2d72 7074 2d76 6965  a: utils-rpt-vie
+0000a790: 7765 7235 0a50 726f 7669 6465 732d 4578  wer5.Provides-Ex
+0000a7a0: 7472 613a 2075 7469 6c73 2d61 6476 616e  tra: utils-advan
+0000a7b0: 6365 640a                                ced.
```

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev9018014082/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev9113174303/th2_data_services.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+ciso8601
 deprecated
 flatdict~=4.0
 orjson<4,>=3.10
 prettytable
 requests~=2.28
 sseclient-py~=1.7
 tabulate
```

