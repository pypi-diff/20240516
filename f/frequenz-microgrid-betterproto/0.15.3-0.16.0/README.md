# Comparing `tmp/frequenz-microgrid-betterproto-0.15.3.tar.gz` & `tmp/frequenz-microgrid-betterproto-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-microgrid-betterproto-0.15.3.tar", last modified: Thu May 16 12:10:24 2024, max compression
+gzip compressed data, was "frequenz-microgrid-betterproto-0.16.0.tar", last modified: Thu May 16 12:50:41 2024, max compression
```

## Comparing `frequenz-microgrid-betterproto-0.15.3.tar` & `frequenz-microgrid-betterproto-0.16.0.tar`

### file list

```diff
@@ -1,141 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.400256 frequenz-microgrid-betterproto-0.15.3/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 12:10:24.400256 frequenz-microgrid-betterproto-0.15.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.388256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/common.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/meter.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17755 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/microgrid.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-16 12:10:02.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/sensor.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.380256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.392256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
--rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.396256 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 12:10:03.000000 frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:10:24.400256 frequenz-microgrid-betterproto-0.15.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.384256 frequenz-microgrid-betterproto-0.15.3/src/frequenz/microgrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.400256 frequenz-microgrid-betterproto-0.15.3/src/frequenz/microgrid/betterproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:01.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz/microgrid/betterproto/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:10:24.400256 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 12:10:24.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-16 12:10:24.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:10:24.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:10:24.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 12:10:24.000000 frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.157089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    23850 2024-05-16 12:50:27.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    41483 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.161089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 12:50:28.000000 frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.153089 frequenz-microgrid-betterproto-0.16.0/src/frequenz/microgrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/src/frequenz/microgrid/betterproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:26.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz/microgrid/betterproto/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:50:41.165089 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 12:50:41.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-16 12:50:41.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:50:41.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:50:41.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 12:50:41.000000 frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/top_level.txt
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/LICENSE` & `frequenz-microgrid-betterproto-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/MANIFEST.in` & `frequenz-microgrid-betterproto-0.16.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/PKG-INFO` & `frequenz-microgrid-betterproto-0.16.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-microgrid-betterproto
-Version: 0.15.3
+Version: 0.16.0
 Summary: Bindings to the microgrid API generated using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-microgrid-betterproto-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/README.md` & `frequenz-microgrid-betterproto-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/proto/frequenz/api/microgrid/microgrid.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-// Contains the definitions for Microgrid gRPC API.
+// protolint:disable MAX_LINE_LENGTH
+
+// Frequenz Microgrid API
 //
 // Copyright:
 // Copyright 2022 Frequenz Energy-as-a-Service GmbH
 //
 // License:
 // MIT
 
 syntax = "proto3";
 
-package frequenz.api.microgrid;
-
-import "frequenz/api/microgrid/battery.proto";
-import "frequenz/api/microgrid/ev_charger.proto";
-import "frequenz/api/microgrid/grid.proto";
-import "frequenz/api/microgrid/inverter.proto";
-import "frequenz/api/microgrid/meter.proto";
-import "frequenz/api/microgrid/sensor.proto";
+package frequenz.api.microgrid.v1;
 
-import "frequenz/api/common/components.proto";
-import "frequenz/api/common/metrics.proto";
+import "frequenz/api/common/v1/location.proto";
+import "frequenz/api/common/v1/metrics/bounds.proto";
+import "frequenz/api/common/v1/metrics/metric_sample.proto";
+import "frequenz/api/common/v1/microgrid/components/components.proto";
+import "frequenz/api/common/v1/microgrid/microgrid.proto";
+import "frequenz/api/common/v1/microgrid/sensors/sensors.proto";
 
 import "google/api/annotations.proto";
 import "google/protobuf/empty.proto";
 import "google/protobuf/timestamp.proto";
 import "google/protobuf/wrappers.proto";
 
+// The Frequenz Microgrid API
 service Microgrid {
-  /// Returns the microgrid metadata
-  /// The metadata consists of information that describes the overall
-  /// microgrid, as opposed to its components,
-  /// e.g., the microgrid ID, location.
-  rpc GetMicrogridMetadata(google.protobuf.Empty) returns (MicrogridMetadata) {
+  // Returns the microgrid metadata
+  // The metadata consists of information that describes the overall
+  // microgrid, as opposed to its electrical components or sensors,
+  // e.g., the microgrid ID, location.
+  rpc GetMicrogridMetadata(google.protobuf.Empty)
+    returns (GetMicrogridMetadataResponse) {
     option (google.api.http) = {
       get : "/v1/metadata"
     };
   }
 
-  // List components in the local microgrid, optionally filtered by a given list
-  // of component IDs and component categories.
+  // List electrical components in the local microgrid, optionally filtered by a
+  // given list of component IDs and component categories.
+  //
+  // Electrical components are a part of a microgrid's electrical infrastructure
+  // are can be connected to each other to form an electrical circuit, which can
+  // then be represented as a graph.
   //
   // If provided, the filters for component IDs and categories have an `AND`
   // relationship with one another, meaning that they are applied serially,
   // but the elements within a single filter list have an `OR` relationship with
   // each other.
   // E.g., if `ids` = [1, 2, 3], and `categories` = [
   //  `ComponentCategory::COMPONENT_CATEGORY_INVERTER`,
@@ -49,52 +54,85 @@
   // then the results will consist of elements that
   // have the IDs 1, OR 2, OR 3,
   // AND
   // are of the categories `ComponentCategory::COMPONENT_CATEGORY_INVERTER` OR
   // `ComponentCategory::COMPONENT_CATEGORY_BATTERY`.
   //
   // If a filter list is empty, then that filter is not applied.
-  rpc ListComponents(ComponentFilter) returns (ComponentList) {
+  rpc ListComponents(ListComponentsRequest) returns (ListComponentsResponse) {
     option (google.api.http) = {
       get : "/v1/components"
     };
   }
 
-  // Returns a list of the connections between components as `(start, end)`
-  // pairs of connection IDs, where the direction of individual connections
-  // is always away from the grid endpoint, i.e. aligned with the direction
-  // of positive current according to the passive sign convention:
+  // Returns a list of sensors in the local microgrid, optionally filtered by a
+  // given list of sensor IDs and sensor categories.
+  //
+  // Sensors measure physical metrics in the microgrid's surroundings, and are
+  // not classified as electrical components.
+  //
+  // If provided, the filters for sensor IDs and categories have an `AND`
+  // relationship with one another, meaning that they are applied serially,
+  // but the elements within a single filter list have an `OR` relationship with
+  // each other.
+  // E.g., if `ids` = [1, 2, 3], and `categories` = [
+  //  `SensorCategory::SENSOR_CATEGORY_THERMOMETER`,
+  //  `SensorCategory::SENSOR_CATEGORY_HYGROMETER`],
+  // then the results will consist of elements that
+  // have the IDs 1, OR 2, OR 3,
+  // AND
+  // are of the categories `SensorCategory::SENSOR_CATEGORY_THERMOMETER` OR
+  // `SensorCategory::SENSOR_CATEGORY_HYGROMETER`.
+  //
+  // If a filter list is empty, then that filter is not applied.
+  rpc ListSensors(ListSensorRequest) returns (ListSensorsResponse) {
+    option (google.api.http) = {
+      get : "/v1/sensors"
+    };
+  }
+
+  // Electrical components are a part of a microgrid's electrical infrastructure
+  // are can be connected to each other to form an electrical circuit, which can
+  // then be represented as a graph.
+  //
+  // This RPC return a list of the connections between two components, denoted
+  // by `(start, end)`. The direction of a connection is always away from the
+  // grid endpoint, i.e. aligned with the direction of positive current
+  // according to the passive sign convention:
   // https://en.wikipedia.org/wiki/Passive_sign_convention
   //
   // The request may be filtered by `start`/`end` component(s) of individual
   // connections.  If provided, the `start` and `end` filters have an `AND`
   // relationship between each other, meaning that they are applied serially,
   // but an `OR` relationship with other elements in the same list.
   // For example, if `start` = `[1, 2, 3]`, and `end` = `[4, 5, 6]`, then the
   // result should have all the connections where
   // * each `start` component ID is either `1`, `2`, OR `3`,
   //  AND
   // * each `end` component ID is either `4`, `5`, OR `6`.
-  rpc ListConnections(ConnectionFilter) returns (ConnectionList) {
+  rpc ListConnections(ListConnectionsRequest)
+    returns (ListConnectionsResponse) {
     option (google.api.http) = {
       get : "/v1/connections"
     };
   }
 
   // Returns a stream containing data from a component with a given ID.
-  rpc StreamComponentData(ComponentIdParam) returns (stream ComponentData) {
+  rpc ReceiveComponentDataStream(ReceiveComponentDataStreamRequest)
+    returns (stream ReceiveComponentDataStreamResponse) {
     option (google.api.http) = {
       get : "/v1/components/{id}/data"
     };
   }
 
-  // Returns whether the component with given ID can stream data.
-  rpc CanStreamData(ComponentIdParam) returns (google.protobuf.BoolValue) {
+  // Returns a stream containing data from a sensor with a given ID.
+  rpc ReceiveSensorDataStream(ReceiveSensorDataStreamRequest)
+    returns (stream ReceiveSensorDataStreamResponse) {
     option (google.api.http) = {
-      get : "/v1/components/{id}/canStream"
+      get : "/v1/sensors/{id}/data"
     };
   }
 
   // Adds exclusion bounds for a given metric of a given component, and returns
   // the UTC timestamp until which the given exclusion bounds will stay in
   // effect.
   //
@@ -134,17 +172,18 @@
   //
   // The following diagram illustrates the relationship between the bounds.
   // ```
   //   inclusion.lower                              inclusion.upper
   // <-------|============|------------------|============|--------->
   //                exclusion.lower    exclusion.upper
   // ```
-  // ---- values here are disallowed and wil be rejected
+  // ---- values here are disallowed and will be rejected
   // ==== vales here are allowed and will be accepted
-  rpc AddExclusionBounds(SetBoundsParam) returns (google.protobuf.Timestamp);
+  rpc AddComponentExclusionBounds(AddComponentExclusionBoundsRequest)
+    returns (AddComponentExclusionBoundsResponse);
 
   // Adds inclusion bounds for a given metric of a given component, and returns
   // the UTC timestamp until which the given inclusion bounds will stay in
   // effect.
   //
   // Inclusion bounds refer to the range of values that are allowed for the
   // metric. If these bounds for a metric are [`lower`, `upper`], then this
@@ -171,45 +210,65 @@
   //
   // The following diagram illustrates the relationship between the bounds.
   // ```
   //   inclusion.lower                              inclusion.upper
   // <-------|============|------------------|============|--------->
   //                exclusion.lower    exclusion.upper
   // ```
-  // ---- values here are disallowed and wil be rejected
+  // ---- values here are disallowed and will be rejected
   // ==== vales here are allowed and will be accepted
-  rpc AddInclusionBounds(SetBoundsParam) returns (google.protobuf.Timestamp);
+  rpc AddComponentInclusionBounds(AddComponentInclusionBoundsRequest)
+    returns (AddComponentInclusionBoundsResponse);
 
   // Sets the active power output of a component with a given ID, provided the
-  // component supports it.
+  // component supports it. The power output is specified in watts.
+  //
+  // The power output can be -ve or +ve, depending on whether the component is
+  // supposed to be discharging or charging, respectively.
+  //
+  // The return value is the timestamp until which the given power command will
+  // stay in effect. After this timestamp, the component's active power will be
+  // set to 0, if the API receives no further command to change it before then.
+  // By default, this timestamp will be set to the current time plus 60 seconds.
   //
   // Note that the target component may have a resolution of more than 1 W.
   // E.g., an inverter may have a resolution of 88 W.
   // In such cases, the magnitude of power will be floored to the nearest
   // multiple of the resolution.
   //
   // Performs the following sequence actions for the following component
   // categories:
   //
   // * Inverter: Sends the discharge command to the inverter, making it deliver
   //  AC power.
-  rpc SetPowerActive(SetPowerActiveParam) returns (google.protobuf.Empty) {
+  rpc SetComponentPowerActive(SetComponentPowerActiveRequest)
+    returns (SetComponentPowerActiveResponse) {
     option (google.api.http) = {
       get : "/v1/components/{component_id}/setPowerActive/{power}"
     };
   }
 
   // Sets the reactive power output of a component with a given ID, provided the
-  // component supports it.
+  // component supports it. The power output is specified in VAr.
+  //
+  // The power output can be -ve or +ve, depending on whether the component is
+  // supposed to be delivering inductive or capacitive power, respectively.
+  //
+  // The return value is the timestamp until which the given power command will
+  // stay in effect. After this timestamp, the component's reactive power will
+  // be set to 0, if the API receives no further command to change it before
+  // then.
+  // By default, this timestamp will be set to the current time plus 60 seconds.
   //
   // Note that the target component may have a resolution of more than 1 VAr.
   // E.g., an inverter may have a resolution of 88 VAr.
   // In such cases, the magnitude of power will be floored to the nearest
   // multiple of the resolution.
-  rpc SetPowerReactive(SetPowerReactiveParam) returns (google.protobuf.Empty) {
+  rpc SetComponentPowerReactive(SetComponentPowerReactiveRequest)
+    returns (SetComponentPowerReactiveResponse) {
     option (google.api.http) = {
       get : "/v1/components/{component_id}/setPowerReactive/{power}"
     };
   }
 
   // Starts the component, and brings it into a state where it is immediately
   // operational.
@@ -221,63 +280,52 @@
   //  * closes DC relays, if the feature is available
   //  * closes AC relays
   //  * sets power output to 0
   //
   // * Battery: Checks if DC relays are open, then
   //  * closes DC relays
   //
+  // * Relays:
+  //  * closes relays
+  //
+  // * Precharge Modules:
+  //  * starts the precharge process, and eventually closes the DC relays.
+  //
   // If any of the above mentioned actions for a given component has already
   // been performed, then this method call effectively skips that action.
   //
   // If a feature required to perform an action is missing, then that action is
   // skipped.
-  rpc Start(ComponentIdParam) returns (google.protobuf.Empty) {
+  rpc StartComponent(StartComponentRequest) returns (google.protobuf.Empty) {
     option (google.api.http) = {
       get : "/v1/components/{id}/start"
     };
   }
 
-  // Sets the given component into a hot-standby state, from which it can return
-  // into an operational state within at most 5 seconds.
-  //
-  // Performs the following sequence actions for the following component
-  // categories:
-  //
-  // * Inverter: Checks if AC and DC relays are closed, then
-  //  * sets power to 0
-  //
-  // If any of the checks mentioned above fails, then the method call returns an
-  // error.
-  //
-  // If any of the above mentioned actions for a given component has already
-  // been performed, then this method call effectively skips that action.
-  rpc HotStandby(ComponentIdParam) returns (google.protobuf.Empty) {
-    option (google.api.http) = {
-      get : "/v1/components/{id}/hotStandby"
-    };
-  }
-
-  // Sets the given component into a cold-standby state, from which it can
-  // return into an operational state within at most 2 minutes.
+  // Sets the given component into a standby state, from which it can take a
+  // few minutes to return to an operational state. A transition to an
+  // operational state can be triggered by calling the `StartComponent` RPC, or
+  // the `SetComponentPowerActive` RPC.
   //
   // Performs the following sequence actions for the following component
   // categories:
   //
   // * Inverter: Checks if AC and DC relays are closed, then
   //  * sets power to 0, and
   //  * opens AC relays
   //
   // If any of the checks mentioned above fails, then the method call returns an
   // error.
   //
   // If any of the above mentioned actions for a given component has already
   // been performed, then this method call efffectively skips that action.
-  rpc ColdStandby(ComponentIdParam) returns (google.protobuf.Empty) {
+  rpc PutComponentInStandby(PutComponentInStandbyRequest)
+    returns (google.protobuf.Empty) {
     option (google.api.http) = {
-      get : "/v1/components/{id}/coldStandby"
+      get : "/v1/components/{id}/standby"
     };
   }
 
   // Stops the component completely, potentially disengaging its power
   // electronics controller(s).
   //
   // Performs the following sequence actions for the following component
@@ -286,202 +334,276 @@
   // * Inverter:
   //  * Brings component to the cold-standby state
   //  * opens DC relays
   //
   // * Battery: Checks if the power output is 0, then
   //  * opens DC relays
   //
+  // * Relays:
+  //  * opens relays
+  //
+  // * Precharge Modules:
+  //  * opens the DC relays.
+  //
   // If any of the checks mentioned above fails, then the method call returns an
   // error.
   //
   // If any of the above mentioned actions for a given component has already
   // been performed, then this method call effectively skips that action.
   //
   // If a feature required to perform an action is missing, then that action is
   // skipped.
-  rpc Stop(ComponentIdParam) returns (google.protobuf.Empty) {
+  rpc StopComponent(StopComponentRequest) returns (google.protobuf.Empty) {
     option (google.api.http) = {
       get : "/v1/components/{id}/stop"
     };
   }
 
   // Acknowledges any recoverable error reported by the component, and brings it
   // back to the stopped or cold-standby state.
-  rpc ErrorAck(ComponentIdParam) returns (google.protobuf.Empty) {
+  rpc AckComponentError(AckComponentErrorRequest)
+    returns (google.protobuf.Empty) {
     option (google.api.http) = {
       get : "/v1/components/{id}/errorAck"
     };
   }
 }
 
-// A pair of geographical co-ordinates, representing the location of a place.
-message Location {
-  // The latitude of the place.
-  float latitude = 1;
-
-  // The longitude of the place.
-  float longitude = 2;
-}
-
 // Metadata that describes a microgrid.
-message MicrogridMetadata {
-  // The microgrid ID.
-  // This is a natural number that uniquely identifies a given microgrid.
-  uint64 microgrid_id = 1;
-
+message GetMicrogridMetadataResponse {
   // The location of the microgrid, in geographical co-ordinates.
-  Location location = 2;
+  frequenz.api.common.v1.microgrid.Microgrid  microgrid= 1;
 }
 
-// Parameters for filtering the components.
-message ComponentFilter {
+// Request parameters for the RPC `ListComponents`.
+// Contains filtering parameters for listing components.
+message ListComponentsRequest {
   // Return components that have the specified IDs only.
-  repeated uint64 ids = 1;
+  repeated uint64 component_ids = 1;
 
   // Return components that have the specified categories only.
-  repeated frequenz.api.common.components.ComponentCategory categories = 2;
+  repeated frequenz.api.common.v1.microgrid.components.ComponentCategory
+    categories = 2;
+}
+
+// A message containing a list of components.
+// Used as the return type in the RPC `ListComponents`.
+message ListComponentsResponse {
+  repeated frequenz.api.common.v1.microgrid.components.Component components = 1;
+}
+
+// Request parameters for the RPC `ListSensors`.
+// Contains filtering parameters for listing sensors.
+message ListSensorRequest {
+  // Return sensors that have the specified IDs only.
+  repeated uint64 sensor_ids = 1;
+
+  // Return sensors that have the specified categories only.
+  repeated frequenz.api.common.v1.microgrid.sensors.SensorCategory
+    categories = 2;
 }
 
-// Encapsulation of a component ID, intended to be used as a parameter for rpc
-// methods.
-message ComponentIdParam {
-  uint64 id = 1;
+// Response message for the RPC `ListSensors`.
+// A message containing a list of sensors.
+message ListSensorsResponse {
+  repeated frequenz.api.common.v1.microgrid.sensors.Sensor sensors = 1;
 }
 
-// Parameters for filtering the component connections
-message ConnectionFilter {
+// Request parameters for the RPC `ListConnections`.
+// Contains filtering parameters for listing connections.
+message ListConnectionsRequest {
   // Only return connections that start from the specified component ID(s):
   // if empty, connections with any `start` will be returned
   repeated uint64 starts = 1;
 
   // Only return connections that end at the specified component ID(s):
   // if empty, connections with any `end` will be returned
   repeated uint64 ends = 2;
 }
 
-// Parameters for setting the charge/discharge power of an appropriate
-// component.
-message PowerLevelParam {
-  // The ID of the component to set the output power of.
-  uint64 component_id = 1;
+// Response message for the RPC `ListConnections`.
+// Contains a list of connections.
+message ListConnectionsResponse {
+  // The list of connections.
+  repeated frequenz.api.common.v1.microgrid.components.ComponentConnection
+    connections = 1;
+};
 
-  // The output power level, in watts. This is always a +ve integer. The sign
-  // of the power level is controlled by the implementations of the `Charge`
-  // and `Discharge` RPC methods.
-  uint64 power_w = 2;
-}
+// Request parameters for the RPC `ReceiveComponentDataStream`.
+message ReceiveComponentDataStreamRequest {
+  // A message for specifying a filter to apply to the stream.
+  message ComponentDataStreamFilter {
+    // List of metrics to return. Only the specified metrics will be returned.
+    //
+    // !!! note
+    //     At least one metric must be specified. If no metric is specified,
+    //     then the stream will return an error.
+    //
+    // !!! note
+    //     Components may not support all metrics. If a component does not
+    //     support a given metric, then the returned data stream will not
+    //     contain that metric.
+    repeated frequenz.api.common.v1.metrics.Metric metrics = 1;
+  }
 
-// Parameters for setting the active power of an appropriate component using the
-// `SetPowerActive` RPC.
-message SetPowerActiveParam {
-  // The ID of the component to set the output active power of.
+  // The component ID to subscribe to.
   uint64 component_id = 1;
 
-  // The output active power level, in watts.
-  // -ve values are for discharging, and +ve values are for charging.
-  float power = 2;
+  // The filter to apply to the stream.
+  //
+  // This field is optional. If this is not provided, then the stream will
+  // return all metrics for the given component. If this is provided, then the
+  // stream will return only the metrics specified in the filter.
+  ComponentDataStreamFilter filter = 2;
+}
+
+// A data sample from a component in the microgrid.
+// Components belonging to all categories and types can be represented using
+// this message.
+message ReceiveComponentDataStreamResponse {
+  frequenz.api.common.v1.microgrid.components.ComponentData data = 1;
+}
+
+// Request parameters for the RPC `ReceiveSensorDataStream`.
+message ReceiveSensorDataStreamRequest {
+  // A message for specifying a filter to apply to the stream.
+  message SensorDataStreamFilter {
+    // List of metrics to return. Only the specified metrics will be returned.
+    //
+    // !!! note
+    //     At least one metric must be specified. If no metric is specified,
+    //     then the stream will return an error.
+    //
+    // !!! note
+    //     Sensors may not support all metrics. If a sensor does not support a
+    //     given metric, then the returned data stream will not contain that
+    //     metric.
+    repeated frequenz.api.common.v1.metrics.Metric metrics = 1;
+  }
+
+  // The sensor ID to subscribe to.
+  uint64 sensor_id = 1;
+
+  // The filter to apply to the stream.
+  //
+  // This field is optional. If this is not provided, then the stream will
+  // return all metrics for the given component. If this is provided, then the
+  // stream will return only the metrics specified in the filter.
+  SensorDataStreamFilter filter = 2;
+}
+
+// A data sample from a sensor in the microgrid.
+message ReceiveSensorDataStreamResponse {
+  // The sensor data.
+  frequenz.api.common.v1.microgrid.sensors.SensorData data = 1;
+}
+
+// An enumerated list of metrics whose bounds can be set using the RPCs
+// `AddComponentExclusionBounds` and `AddComponentInclusionBounds`.
+enum ComponentBoundsTargetMetric {
+  COMPONENT_BOUNDS_TARGET_METRIC_UNSPECIFIED = 0;
+  COMPONENT_BOUNDS_TARGET_METRIC_POWER_ACTIVE = 1;
+  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT = 2;
+  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_1 = 3;
+  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_2 = 4;
+  COMPONENT_BOUNDS_TARGET_METRIC_CURRENT_PHASE_3 = 5;
+  COMPONENT_BOUNDS_TARGET_METRIC_POWER_REACTIVE = 6;
 }
 
-// Parameters for setting the reactive power of an appropriate component using
-// the `SetPowerReactive` RPC.
-message SetPowerReactiveParam {
-  // The ID of the component to set the output reactive power of.
+// Request parameters for the RPC `AddComponentExclusionBounds`.
+message AddComponentExclusionBoundsRequest {
+  // The ID of the target component.
   uint64 component_id = 1;
 
-  // The output reactive power level, in VAr.
-  // -ve values are for inductive (lagging) power , and +ve values are for
-  //  capacitive (leading) power.
-  float power = 2;
+  // The target metric whose bounds have to be set.
+  ComponentBoundsTargetMetric target_metric = 2;
+
+  // The bounds for the target metric.
+  frequenz.api.common.v1.metrics.Bounds bounds = 3;
 }
 
-// Parameters for setting bounds of a given metric of a given component.
-message SetBoundsParam {
-  // An enumerated list of metrics whose bounds can be set.
-  enum TargetMetric {
-    TARGET_METRIC_UNSPECIFIED = 0;
-    TARGET_METRIC_POWER_ACTIVE = 1;
-    TARGET_METRIC_CURRENT = 2;
-    TARGET_METRIC_CURRENT_PHASE_1 = 3;
-    TARGET_METRIC_CURRENT_PHASE_2 = 4;
-    TARGET_METRIC_CURRENT_PHASE_3 = 5;
-    TARGET_METRIC_POWER_REACTIVE = 6;
-  }
+// Response message for the RPC `AddComponentExclusionBounds`.
+message AddComponentExclusionBoundsResponse {
+  // The timestamp until which the given exclusion bounds will stay in effect.
+  google.protobuf.Timestamp ts = 1;
+}
 
+// Request parameters for the RPC `AddComponentInclusionBounds`.
+message AddComponentInclusionBoundsRequest {
   // The ID of the target component.
   uint64 component_id = 1;
 
   // The target metric whose bounds have to be set.
-  TargetMetric target_metric = 2;
+  ComponentBoundsTargetMetric target_metric = 2;
 
   // The bounds for the target metric.
-  frequenz.api.common.metrics.Bounds bounds = 3;
+  frequenz.api.common.v1.metrics.Bounds bounds = 3;
 }
 
-// A generic message for components. It is used to represent any category of
-// component, with its static parameters.
-message Component {
-  // A unique identifier for the component.
-  uint64 id = 1;
+// Response message for the RPC `AddComponentInclusionBounds`.
+message AddComponentInclusionBoundsResponse {
+  // The timestamp until which the given inclusion bounds will stay in effect.
+  google.protobuf.Timestamp ts = 1;
+}
 
-  // An optional name for the component.
-  string name = 2;
+// Request parameters for the RPC `SetComponentPowerActive`.
+message SetComponentPowerActiveRequest {
+  // The ID of the component to set the output active power of.
+  uint64 component_id = 1;
 
-  // The category of the component.
-  frequenz.api.common.components.ComponentCategory category = 3;
+  // The output active power level, in watts.
+  // -ve values are for discharging, and +ve values are for charging.
+  float power = 2;
+}
 
-  // The component manufacturer.
-  string manufacturer = 4;
+// Response message for the RPC `SetComponentPowerActive`.
+message SetComponentPowerActiveResponse {
+  // The timestamp until which the given power command will stay in effect.
+  // After this timestamp, the component power will be set to 0, if the API
+  // receives no further power commands. By default, this timestamp will be set
+  // to the current time plus 60 seconds.
+  google.protobuf.Timestamp valid_until = 1;
+}
 
-  // The model name of the component.
-  string model_name = 5;
+// Request parameters for the RPC `SetComponentPowerReactive`.
+message SetComponentPowerReactiveRequest {
+  // The ID of the component to set the output reactive power of.
+  uint64 component_id = 1;
 
-  // The metadata specific to the component category.
-  oneof metadata {
-    grid.Metadata grid = 11;
-    battery.Metadata battery = 12;
-    inverter.Metadata inverter = 13;
-    meter.Metadata meter = 14;
-    ev_charger.Metadata ev_charger = 15;
-    sensor.Metadata sensor = 16;
-  }
+  // The output reactive power level, in VAr.
+  // -ve values are for inductive (lagging) power , and +ve values are for
+  //  capacitive (leading) power.
+  float power = 2;
 }
 
-// A message containing a list of components, used as a return typ in certain
-// RPC methods.
-message ComponentList {
-  repeated Component components = 1;
+// Response message for the RPC `SetComponentPowerReactive`.
+message SetComponentPowerReactiveResponse {
+  // The timestamp until which the given power command will stay in effect.
+  // After this timestamp, the component power will be set to 0, if the API
+  // receives no further power commands. By default, this timestamp will be set
+  // to the current time plus 60 seconds.
+  google.protobuf.Timestamp valid_until = 1;
 }
 
-// A generic container for data that can originate from any component type.
-message ComponentData {
-  // The timestamp of when the data was measured.
-  google.protobuf.Timestamp ts = 1;
+// Request parameters for the RPC `StartComponent`.
+message StartComponentRequest {
+  // The component ID to start.
+  uint64 component_id = 1;
+}
 
-  // The component ID.
-  uint64 id = 2;
+// Request parameters for the RPC `PutComponentInStandby`.
+message PutComponentInStandbyRequest {
+  // The component ID to set to standby.
+  uint64 component_id = 1;
+}
 
-  // The data object.
-  oneof data {
-    meter.Meter meter = 3;
-    inverter.Inverter inverter = 4;
-    battery.Battery battery = 5;
-    ev_charger.EvCharger ev_charger = 6;
-    sensor.Sensor sensor = 7;
-  }
+// Request parameters for the RPC `StopComponent`.
+message StopComponentRequest {
+  // The component ID to stop.
+  uint64 component_id = 1;
 }
 
-// Describes a single connection between components of the microgrid,
-// with direction away from the grid endpoint, meaning it is aligned
-// with positive current according to the passive sign convention:
-// https://en.wikipedia.org/wiki/Passive_sign_convention
-message Connection {
-  // `id` of the component the connection starts from
-  uint64 start = 1;
-
-  // `id` of the component the connection points to
-  uint64 end = 2;
-}
-
-// List of connections between components
-message ConnectionList {
-  repeated Connection connections = 1;
-};
+// Request parameters for the RPC `AckComponentError`.
+message AckComponentErrorRequest {
+  // The component ID to acknowledge the error for.
+  uint64 component_id = 1;
+}
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 // Copyright 2023 Frequenz Energy-as-a-Service GmbH
 //
 // Licensed under the MIT License (the "License");
 // you may not use this file except in compliance with the License.
 
 syntax = "proto3";
 
-package frequenz.api.common.location;
+package frequenz.api.common.v1;
 
 // A pair of geographical co-ordinates, representing the location of a place.
 message Location {
   // Latitude ranges from -90 (South) to 90 (North)
   float latitude = 1;
 
   // Longitude ranges from -180 (West) to 180 (East)
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 // License:
 // MIT
 
 syntax = "proto3";
 
 package frequenz.api.common.v1.microgrid.components;
 
-import "frequenz/api/common/v1/metrics/bounds.proto";
 import "frequenz/api/common/v1/metrics/metric_sample.proto";
 import "frequenz/api/common/v1/microgrid/components/battery.proto";
 import "frequenz/api/common/v1/microgrid/components/ev_charger.proto";
 import "frequenz/api/common/v1/microgrid/components/fuse.proto";
 import "frequenz/api/common/v1/microgrid/components/grid.proto";
 import "frequenz/api/common/v1/microgrid/components/inverter.proto";
 import "frequenz/api/common/v1/microgrid/components/transformer.proto";
@@ -138,34 +137,14 @@
   string model_name = 7;
 
   // The status of the component.
   ComponentStatus status = 8;
 
   // The operational lifetime of the component.
   frequenz.api.common.v1.microgrid.Lifetime operational_lifetime = 9;
-
-  // List of rated bounds present for the component identified by Metric.
-  repeated MetricConfigBounds metric_config_bounds = 10;
-}
-
-// MetricConfigBounds describes a set of limits for a specific metric consisting
-// of a lower and upper bound for said metric.
-//
-// This can be used for example to specify an allowed range of power output
-// for a component.
-message MetricConfigBounds {
-  // Metric type the config bounds are for
-  frequenz.api.common.v1.metrics.Metric metric = 1;
-
-  // The set of bounds for the specified metric.
-  //
-  // This contains the lower and upper bounds for said metric.
-  // Sources these may be derived from include the component configuration,
-  // manufacturers limits, and limits of other devices.
-  frequenz.api.common.v1.metrics.Bounds config_bounds = 2;
 }
 
 // ComponentConnection describes a single electrical link between two components
 // within a microgrid, effectively representing the physical wiring as viewed
 // from the grid connection point, if one exists, or from the islanding point,
 // in case of an islanded microgrids.
 //
@@ -225,21 +204,19 @@
 //        }
 //      ],
 //      states: [
 //        /* list of states for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
-//          warnings: [],
 //          errors: [],
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          states: [],
-//          warnings: [],
 //          errors: [],
 //        },
 //      ]
 //    }
 //  ```
 message ComponentData {
   // The ID of the microgrid component.
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/fuse.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/transformer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,7 @@
 
   // The current status of the microgrid.
   MicrogridStatus status = 6;
 
   // The UTC timestamp indicating when the microgrid was initially created.
   google.protobuf.Timestamp create_timestamp = 7;
 }
-
-// A message to link component IDs with their respective microgrid ID.
-message MicrogridComponentIDs {
-  // The ID of the microgrid.
-  uint64 microgrid_id = 1;
-
-  // List of component IDs belonging to this microgrid.
-  repeated uint64 component_ids = 2;
-}
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/sensors/sensors.proto`

 * *Files 6% similar despite different names*

```diff
@@ -103,43 +103,37 @@
   // Dew point.
   // The temperature at which the air becomes saturated with water vapor.
   //
   // In Celsius (°C).
   SENSOR_METRIC_DEW_POINT = 8;
 }
 
-// SensorData message aggregates multiple metrics, operational states, and
-// errors, related to a specific microgrid sensor.
+// ComponentData message aggregates multiple metrics, operational states, and
+// errors, related to a specific microgrid component.
 //
 // !!! example
 //   Example output of a component data message:
 //   ```
 //    {
-//      sensor_id: 13,
+//      component_id: 13,
 //      metric_samples: [
 //        /* list of metrics for multiple timestamps */
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_TEMPERATURE",
 //          sample: metric_sample_type: {simple_metric: {value: 23.5},
+//          bounds: {},
 //        },
 //        {
 //          sampled_at: "2023-10-01T00:00:00Z",
 //          metric: "METRIC_SENSOR_RELATIVE_HUMIDITY",
 //          sample: metric_sample_type: {simple_metric: {value: 23.5},
+//          bounds: {},
 //        }
-//      ],
-//      states: [
-//        {
-//          sampled_at: "2023-10-01T00:00:00Z",
-//          states: [],
-//          errors: [],
-//        },
 //      ]
-//
 //    }
 //  ```
 message SensorData {
   // The ID of the microgrid sensors.
   uint64 sensor_id = 1;
 
   // List of measurements for a metric of the specific microgrid sensor.
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto` & `frequenz-microgrid-betterproto-0.16.0/frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/pagination/pagination_params.proto`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/pyproject.toml` & `frequenz-microgrid-betterproto-0.16.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO` & `frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-microgrid-betterproto
-Version: 0.15.3
+Version: 0.16.0
 Summary: Bindings to the microgrid API generated using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-microgrid-betterproto-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-microgrid-betterproto-python
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt` & `frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 .gitmodules
 LICENSE
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 pyproject.toml
-frequenz-api-microgrid/proto/frequenz/api/microgrid/battery.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/common.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/ev_charger.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/grid.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/inverter.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/meter.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/microgrid.proto
-frequenz-api-microgrid/proto/frequenz/api/microgrid/sensor.proto
+frequenz-api-microgrid/proto/frequenz/api/microgrid/v1/microgrid.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/annotations.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/auth.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/backend.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/billing.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/client.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/config_change.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/api/consumer.proto
@@ -63,23 +56,16 @@
 frequenz-api-microgrid/submodules/api-common-protos/google/type/fraction.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/latlng.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/money.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/month.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/postal_address.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/quaternion.proto
 frequenz-api-microgrid/submodules/api-common-protos/google/type/timeofday.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/location.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/location.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_area.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/grid/delivery_duration.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/energy.proto
-frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/market/price.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/bounds.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/metrics/metric_sample.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/lifetime.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/microgrid.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/battery.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/components.proto
 frequenz-api-microgrid/submodules/frequenz-api-common/proto/frequenz/api/common/v1/microgrid/components/ev_charger.proto
```

### Comparing `frequenz-microgrid-betterproto-0.15.3/src/frequenz_microgrid_betterproto.egg-info/requires.txt` & `frequenz-microgrid-betterproto-0.16.0/src/frequenz_microgrid_betterproto.egg-info/requires.txt`

 * *Files identical despite different names*

