# Comparing `tmp/frequenz-api-weather-0.3.0.tar.gz` & `tmp/frequenz-api-weather-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-weather-0.3.0.tar", last modified: Fri Mar  1 15:45:10 2024, max compression
+gzip compressed data, was "frequenz-api-weather-0.4.0.tar", last modified: Thu May 16 09:03:03 2024, max compression
```

## Comparing `frequenz-api-weather-0.3.0.tar` & `frequenz-api-weather-0.4.0.tar`

### file list

```diff
@@ -1,116 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.614029 frequenz-api-weather-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-01 15:45:10.614029 frequenz-api-weather-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/proto/frequenz/api/common/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/proto/frequenz/api/common/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/proto/frequenz/api/common/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/proto/frequenz/api/common/pagination/pagination_params.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/proto/frequenz/api/weather/
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/proto/frequenz/api/weather/weather.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/frequenz/api/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/frequenz/api/common/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/api/common/pagination/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/api/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/frequenz/api/weather/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/api/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/api/weather/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/api/weather/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/py/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/frequenz/client/weather/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/client/weather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/client/weather/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/client/weather/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/py/frequenz/client/weather/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-01 15:45:10.000000 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-01 15:45:10.000000 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 15:45:10.000000 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-01 15:45:10.000000 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-01 15:45:10.000000 frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 15:45:10.614029 frequenz-api-weather-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.602029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.598029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.610029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.614029 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-01 15:45:00.000000 frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 15:45:10.614029 frequenz-api-weather-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-01 15:44:59.000000 frequenz-api-weather-0.3.0/tests/test_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/examples/iterate_hist_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/examples/stream_live_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.098987 frequenz-api-weather-0.4.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.098987 frequenz-api-weather-0.4.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.098987 frequenz-api-weather-0.4.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/proto/frequenz/api/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/proto/frequenz/api/weather/weather.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.098987 frequenz-api-weather-0.4.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/frequenz/api/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/frequenz/api/common/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/api/common/pagination/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/api/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/frequenz/api/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/api/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/api/weather/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/api/weather/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/py/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/frequenz/client/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/client/weather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/client/weather/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/client/weather/_historical_forecast_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/client/weather/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/py/frequenz/client/weather/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.106987 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-16 09:03:03.000000 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-16 09:03:03.000000 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:03:03.000000 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-16 09:03:03.000000 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 09:03:03.000000 frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.110987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.110987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.110987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.110987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.102987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.114987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 09:02:55.000000 frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:03:03.118987 frequenz-api-weather-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 09:02:54.000000 frequenz-api-weather-0.4.0/tests/test_weather.py
```

### Comparing `frequenz-api-weather-0.3.0/LICENSE` & `frequenz-api-weather-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/PKG-INFO` & `frequenz-api-weather-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-weather
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frequenz gRPC API for retrieving weather forecasts.
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-weather/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-weather/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-weather/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-weather
```

### Comparing `frequenz-api-weather-0.3.0/README.md` & `frequenz-api-weather-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/proto/frequenz/api/common/location.proto` & `frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // Copyright 2023 Frequenz Energy-as-a-Service GmbH
 //
 // Licensed under the MIT License (the "License");
 // you may not use this file except in compliance with the License.
 
 syntax = "proto3";
 
-package frequenz.api.weatherforecast.v1;
+package frequenz.api.common.location;
 
 // A pair of geographical co-ordinates, representing the location of a place.
 message Location {
   // Latitude ranges from -90 (South) to 90 (North)
   float latitude = 1;
 
   // Longitude ranges from -180 (West) to 180 (East)
```

### Comparing `frequenz-api-weather-0.3.0/proto/frequenz/api/common/pagination/pagination_info.proto` & `frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // Copyright 2023 Frequenz Energy-as-a-Service GmbH
 //
 // Licensed under the MIT License (the "License");
 // you may not use this file except in compliance with the License.
 
 syntax = "proto3";
 
-package frequenz.api.weatherforecast.v1;
+package frequenz.api.common.v1.pagination;
 
 // A message providing metadata about paginated list results.
 // The PaginationInfo message delivers metadata concerning the paginated list
 // results and should be appended to the response message of a list request. The
 // total_items field must be set to the total count of items that adhere to the
 // filter criteria defined in the request. The next_page_token field should be
 // populated with the token to be used in the subsequent request to fetch the
```

### Comparing `frequenz-api-weather-0.3.0/proto/frequenz/api/common/pagination/pagination_params.proto` & `frequenz-api-weather-0.4.0/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // Copyright 2023 Frequenz Energy-as-a-Service GmbH
 //
 // Licensed under the MIT License (the "License");
 // you may not use this file except in compliance with the License.
 
 syntax = "proto3";
 
-package frequenz.api.weatherforecast.v1;
+package frequenz.api.common.v1.pagination;
 
 // A message defining parameters for paginating list requests.
 // It can be appended to a request message to specify the desired page of
 // results and the maximum number of results per page. For initial requests
 // (requesting the first page), the page_token should not be provided. For
 // subsequent requests (requesting any page after the first), the
 // next_page_token from the previous responses PaginationInfo must be supplied.
```

### Comparing `frequenz-api-weather-0.3.0/proto/frequenz/api/weather/weather.proto` & `frequenz-api-weather-0.4.0/proto/frequenz/api/weather/weather.proto`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 // License:
 // MIT
 
 syntax = "proto3";
 
 package frequenz.api.weatherforecast.v1;
 
-import "frequenz/api/common/location.proto";
-import "frequenz/api/common/pagination/pagination_info.proto";
-import "frequenz/api/common/pagination/pagination_params.proto";
 import "google/protobuf/timestamp.proto";
 
+import "frequenz/api/common/v1/location.proto";
+import "frequenz/api/common/v1/pagination/pagination_info.proto";
+import "frequenz/api/common/v1/pagination/pagination_params.proto";
 
 // Service provides operations related to retrieving weather forecasts for
 // locations.
 //
 // The forecasts are updated regularly, and the service will stream the latest
 // available data unless a specific time range is requested.
 // !!! note
@@ -98,15 +98,15 @@
 // The `GetHistoricalWeatherForecastRequest` message defines parameters for
 // retrieving historical weather forecasts, targeting a specific location
 // and time period, with designated features.
 message GetHistoricalWeatherForecastRequest {
   // The locations for which the forecast is being requested.
   // The maximum number of locations that can be requested is 50. If the
   // request exceeds this limit, the API will respond with an error.
-  repeated frequenz.api.weatherforecast.v1.Location locations = 1;
+  repeated frequenz.api.common.v1.Location locations = 1;
 
   // List of required features. If none are specified, all available features
   // will be returned.
   repeated ForecastFeature features = 2;
 
   // The UTC timestamp indicating the start of the requested historical forecast
   // period.
@@ -115,26 +115,26 @@
   // The UTC timestamp indicating the end of the requested historical forecast
   // period.
   google.protobuf.Timestamp end_ts = 4;
 
   // The parameters define the 'page_size' and the 'page_token'. An inital
   // query of a request will omit the 'page_token'. Subsequent queries of the
   // same request must include the 'page_token' from the previous response.
-  frequenz.api.weatherforecast.v1.PaginationParams
+  frequenz.api.common.v1.pagination.PaginationParams
     pagination_params = 5;
 }
 
 // The `ReceiveLiveWeatherForecastRequest` message defines parameters for
 // requesting live weather forecasts for a specified location, with designated
 // features.
 message ReceiveLiveWeatherForecastRequest {
   // The locations for which the forecast is being requested.
   // The maximum number of locations that can be requested is 50. If the
   // request exceeds this limit, the API will respond with an error.
-  repeated frequenz.api.weatherforecast.v1.Location locations = 1;
+  repeated frequenz.api.common.v1.Location locations = 1;
 
   // List of required features. If none are specified, all available features
   // will be streamed.
   repeated ForecastFeature features = 2;
 }
 
 // The `ForecastResponse` message  provides a structured format for representing
@@ -162,29 +162,29 @@
     repeated FeatureForecast features = 2;
   }
 
   // Weather forecasts.
   repeated Forecasts forecasts = 1;
 
   // The location for which the weather data is returned.
-  frequenz.api.weatherforecast.v1.Location location = 2;
+  frequenz.api.common.v1.Location location = 2;
 
   // The UTC timestamp indicating when the forecast was originally created.
   google.protobuf.Timestamp creation_ts = 3;
 }
 
 // The message encapsulates a collection of historical weather forecasts, each
 // corresponding to a requested location.
 message GetHistoricalWeatherForecastResponse {
   repeated LocationForecast location_forecasts = 1;
 
   // The pagination_info contains the number of 'total_items' in the response
   // and the 'next_page_token' for the subsequent query of the request. It is
   // omitted in the last response.
-  frequenz.api.weatherforecast.v1.PaginationInfo pagination_info = 2;
+  frequenz.api.common.v1.pagination.PaginationInfo pagination_info = 2;
 }
 
 // The message encapsulates a collection of live weather forecasts, each
 // corresponding to a requested location.
 message ReceiveLiveWeatherForecastResponse {
   repeated LocationForecast location_forecasts = 1;
 }
```

### Comparing `frequenz-api-weather-0.3.0/py/frequenz/client/weather/_client.py` & `frequenz-api-weather-0.4.0/py/frequenz/client/weather/_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """The Weather Forecast API client."""
 
+from datetime import datetime
+
 import grpc
 from frequenz.api.weather import weather_pb2, weather_pb2_grpc
 from frequenz.channels import Receiver
 from frequenz.client.base.streaming import GrpcStreamBroadcaster
 
+from ._historical_forecast_iterator import HistoricalForecastIterator
 from ._types import ForecastFeature, Forecasts, Location
 
 
 class Client:
     """Weather forecast client."""
 
     def __init__(self, grpc_channel: grpc.aio.Channel, svc_addr: str) -> None:
@@ -54,7 +57,27 @@
                         locations=(location.to_pb() for location in locations),
                         features=(feature.value for feature in features),
                     )
                 ),
                 Forecasts.from_pb,
             )
         return self._streams[stream_key].new_receiver()
+
+    def hist_forecast_iterator(
+        self,
+        locations: list[Location],
+        features: list[ForecastFeature],
+        start: datetime,
+        end: datetime,
+    ) -> HistoricalForecastIterator:
+        """Stream historical weather forecast data.
+
+        Args:
+            locations: locations to stream data for.
+            features: features to stream data for.
+            start: start of the time range to stream data for.
+            end: end of the time range to stream data for.
+
+        Returns:
+            A channel receiver for weather forecast data.
+        """
+        return HistoricalForecastIterator(self._stub, locations, features, start, end)
```

### Comparing `frequenz-api-weather-0.3.0/py/frequenz/client/weather/_types.py` & `frequenz-api-weather-0.4.0/py/frequenz/client/weather/_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 
 from __future__ import annotations  # required for constructor type hinting
 
 import datetime as dt
 import enum
 import logging
 import typing
+from collections import namedtuple
 from dataclasses import dataclass
 
 import numpy as np
-from frequenz.api.common import location_pb2
+from frequenz.api.common.v1 import location_pb2
 from frequenz.api.weather import weather_pb2
 
 # Set up logging
 _logger = logging.getLogger(__name__)
 
 
 class ForecastFeature(enum.Enum):
@@ -277,7 +278,88 @@
                 )
 
         # catch all exceptions
         except Exception as e:
             raise RuntimeError("Error processing forecast data") from e
 
         return array
+
+
+ForecastData = namedtuple(
+    "ForecastData",
+    ["creation_ts", "latitude", "longitude", "validity_ts", "feature", "value"],
+)
+
+
+@dataclass(frozen=True)
+class HistoricalForecasts:
+    """Historical weather forecast data."""
+
+    _forecasts_pb: weather_pb2.GetHistoricalWeatherForecastResponse
+
+    @classmethod
+    def from_pb(
+        cls, forecasts: weather_pb2.GetHistoricalWeatherForecastResponse
+    ) -> HistoricalForecasts:
+        """Convert a protobuf Forecast message to Forecast object.
+
+        Args:
+            forecasts: protobuf message with historical forecast data.
+
+        Returns:
+            Forecast object corresponding to the protobuf message.
+        """
+        return cls(_forecasts_pb=forecasts)
+
+    def flatten(
+        self,
+    ) -> list[ForecastData]:
+        """Flatten a Forecast object to a list of named tuples of data.
+
+        Returns:
+            List of named tuples with the flattened forecast data.
+
+        Raises:
+            ValueError: If the forecasts data is missing or invalid.
+        """
+        # check for empty forecasts data
+        if not self._forecasts_pb.location_forecasts:
+            raise ValueError("Forecast data is missing or invalid.")
+
+        return flatten(list(self._forecasts_pb.location_forecasts))
+
+
+def flatten(
+    location_forecasts: list[weather_pb2.LocationForecast],
+) -> list[ForecastData]:
+    """Flatten a Forecast object to a list of named tuples of data.
+
+    Each tuple contains the following data:
+    - creation timestamp
+    - latitude
+    - longitude
+    - validity timestamp
+    - feature
+    - forecast value
+
+    Args:
+        location_forecasts: The location forecasts to flatten.
+    Returns:
+        List of named tuples with the flattened forecast data.
+    """
+    data = []
+    for location_forecast in location_forecasts:
+        for forecasts in location_forecast.forecasts:
+            for feature_forecast in forecasts.features:
+                # Create and append an instance of the named tuple instead of a plain tuple
+                data.append(
+                    ForecastData(
+                        creation_ts=location_forecast.creation_ts.ToDatetime(),
+                        latitude=location_forecast.location.latitude,
+                        longitude=location_forecast.location.longitude,
+                        validity_ts=forecasts.valid_at_ts.ToDatetime(),
+                        feature=ForecastFeature(feature_forecast.feature),
+                        value=feature_forecast.value,
+                    )
+                )
+
+    return data
```

### Comparing `frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/PKG-INFO` & `frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-weather
-Version: 0.3.0
+Version: 0.4.0
 Summary: Frequenz gRPC API for retrieving weather forecasts.
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-api-weather/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-weather/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-weather/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-weather
```

### Comparing `frequenz-api-weather-0.3.0/py/frequenz_api_weather.egg-info/requires.txt` & `frequenz-api-weather-0.4.0/py/frequenz_api_weather.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+frequenz-api-common<0.6.0,>=0.5.4
 googleapis-common-protos<2,>=1.62.0
 grpcio<2,>=1.54.2
-frequenz-channels==1.0.0b2
-frequenz-client-base<0.3,>=0.2.0
+frequenz-channels==1.0.0
+frequenz-client-base<0.4,>=0.3.0
 numpy<2,>=1.24.2
 
 [dev]
 frequenz-api-weather[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==6.1.0
```

### Comparing `frequenz-api-weather-0.3.0/pyproject.toml` & `frequenz-api-weather-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,19 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
+  "frequenz-api-common >= 0.5.4, < 0.6.0",
   "googleapis-common-protos >= 1.62.0, < 2",
   "grpcio >= 1.54.2, < 2",
-  "frequenz-channels == 1.0.0b2",
-  "frequenz-client-base >= 0.2.0, < 0.3",
+  "frequenz-channels == 1.0.0",
+  "frequenz-client-base >= 0.3.0, < 0.4",
   "numpy >= 1.24.2, < 2",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
```

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-weather-0.4.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-weather-0.3.0/tests/test_types.py` & `frequenz-api-weather-0.4.0/tests/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # pylint doesn't understand the imports from the generated proto modules.
 # pylint: disable=no-name-in-module,no-member
 
 from datetime import datetime
 
 import numpy as np
 from _pytest.logging import LogCaptureFixture
-from frequenz.api.common.location_pb2 import Location as LocationProto
+from frequenz.api.common.v1.location_pb2 import Location as LocationProto
 from frequenz.api.weather import weather_pb2
 from frequenz.client.weather._types import ForecastFeature, Forecasts, Location
 from google.protobuf.timestamp_pb2 import Timestamp
 from pytest import CaptureFixture, fixture
 
 
 class TestForecastFeatureType:
```

### Comparing `frequenz-api-weather-0.3.0/tests/test_weather.py` & `frequenz-api-weather-0.4.0/tests/test_weather.py`

 * *Files identical despite different names*

