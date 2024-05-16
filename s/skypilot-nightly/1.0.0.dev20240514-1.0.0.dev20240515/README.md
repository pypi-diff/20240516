# Comparing `tmp/skypilot_nightly-1.0.0.dev20240514.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240514.tar", last modified: Tue May 14 10:38:36 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240515.tar", last modified: Wed May 15 15:03:07 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240514.tar` & `skypilot_nightly-1.0.0.dev20240515.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.777523 skypilot_nightly-1.0.0.dev20240514/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-14 10:38:36.777523 skypilot_nightly-1.0.0.dev20240514/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:38:36.777523 skypilot_nightly-1.0.0.dev20240514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-14 10:38:33.000000 skypilot_nightly-1.0.0.dev20240514/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.717523 skypilot_nightly-1.0.0.dev20240514/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.721523 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.721523 skypilot_nightly-1.0.0.dev20240514/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   230760 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.721523 skypilot_nightly-1.0.0.dev20240514/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.721523 skypilot_nightly-1.0.0.dev20240514/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   192150 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.725523 skypilot_nightly-1.0.0.dev20240514/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.729523 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.729523 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.729523 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/global_user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/jobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.733523 skypilot_nightly-1.0.0.dev20240514/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.737523 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.741523 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.741523 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.741523 skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.741523 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.741523 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.745523 skypilot_nightly-1.0.0.dev20240514/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.745523 skypilot_nightly-1.0.0.dev20240514/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-14 10:38:33.000000 skypilot_nightly-1.0.0.dev20240514/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.749523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.753523 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/skypilot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.757523 skypilot_nightly-1.0.0.dev20240514/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/jobs-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.757523 skypilot_nightly-1.0.0.dev20240514/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.757523 skypilot_nightly-1.0.0.dev20240514/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.757523 skypilot_nightly-1.0.0.dev20240514/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.761523 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/generate_kind_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/generate_static_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.765523 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 10:38:36.000000 skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:38:36.765523 skypilot_nightly-1.0.0.dev20240514/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_jobs_and_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   215704 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-14 10:38:29.000000 skypilot_nightly-1.0.0.dev20240514/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:03:07.920903 skypilot_nightly-1.0.0.dev20240515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 15:03:05.000000 skypilot_nightly-1.0.0.dev20240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.860903 skypilot_nightly-1.0.0.dev20240515/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230760 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.864903 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192150 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.868903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.872903 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/global_user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/jobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.876903 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.880903 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.884903 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.888903 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-15 15:03:05.000000 skypilot_nightly-1.0.0.dev20240515/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.892903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.896903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.896903 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/skypilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47130 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.900903 skypilot_nightly-1.0.0.dev20240515/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/jobs-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.900903 skypilot_nightly-1.0.0.dev20240515/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.904903 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_kind_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_static_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.908903 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 15:03:07.000000 skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:03:07.908903 skypilot_nightly-1.0.0.dev20240515/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_jobs_and_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   216332 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-15 15:03:01.000000 skypilot_nightly-1.0.0.dev20240515/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/LICENSE` & `skypilot_nightly-1.0.0.dev20240515/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240515/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240515/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240514
+Version: 1.0.0.dev20240515
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/README.md` & `skypilot_nightly-1.0.0.dev20240515/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240515/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/setup.py` & `skypilot_nightly-1.0.0.dev20240515/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '8a0a34d36bc75cd1e337e11d14e5bf8aeb4144e4'
+_SKYPILOT_COMMIT_SHA = '5a2f1b855e0a8b0a099390882209914f34ea8b98'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240514'
+__version__ = '1.0.0.dev20240515'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240515/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240515/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/check.py` & `skypilot_nightly-1.0.0.dev20240515/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240515/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240515/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240515/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/core.py` & `skypilot_nightly-1.0.0.dev20240515/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240515/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240515/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240515/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240515/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240515/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240515/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/constants.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/controller.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/core.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/state.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/jobs/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240515/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240515/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
             f'{backend_utils.BOLD}sky serve logs --controller {service_name}'
             f'{backend_utils.RESET_BOLD}'
             '\n'
             '\nTo monitor replica status:\t'
             f'{backend_utils.BOLD}watch -n10 sky serve status {service_name}'
             f'{backend_utils.RESET_BOLD}'
             '\nTo send a test request:\t\t'
-            f'{backend_utils.BOLD}curl -L {endpoint}'
+            f'{backend_utils.BOLD}curl {endpoint}'
             f'{backend_utils.RESET_BOLD}'
             '\n'
             f'\n{fore.GREEN}SkyServe is spinning up your service now.'
             f'{style.RESET_ALL}'
             f'\n{fore.GREEN}The replicas should be ready within a '
             f'short time.{style.RESET_ALL}')
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/load_balancing_policies.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,52 +7,64 @@
 
 if typing.TYPE_CHECKING:
     import fastapi
 
 logger = sky_logging.init_logger(__name__)
 
 
+def _request_repr(request: 'fastapi.Request') -> str:
+    return ('<Request '
+            f'method="{request.method}" '
+            f'url="{request.url}" '
+            f'headers={dict(request.headers)} '
+            f'query_params={dict(request.query_params)}>')
+
+
 class LoadBalancingPolicy:
     """Abstract class for load balancing policies."""
 
     def __init__(self) -> None:
         self.ready_replicas: List[str] = []
 
     def set_ready_replicas(self, ready_replicas: List[str]) -> None:
         raise NotImplementedError
 
+    def select_replica(self, request: 'fastapi.Request') -> Optional[str]:
+        replica = self._select_replica(request)
+        if replica is not None:
+            logger.info(f'Selected replica {replica} '
+                        f'for request {_request_repr(request)}')
+        else:
+            logger.warning('No replica selected for request '
+                           f'{_request_repr(request)}')
+        return replica
+
     # TODO(tian): We should have an abstract class for Request to
     # compatible with all frameworks.
-    def select_replica(self, request: 'fastapi.Request') -> Optional[str]:
+    def _select_replica(self, request: 'fastapi.Request') -> Optional[str]:
         raise NotImplementedError
 
 
 class RoundRobinPolicy(LoadBalancingPolicy):
     """Round-robin load balancing policy."""
 
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
+    def __init__(self) -> None:
+        super().__init__()
         self.index = 0
 
     def set_ready_replicas(self, ready_replicas: List[str]) -> None:
-        if set(ready_replicas) != set(self.ready_replicas):
-            # If the autoscaler keeps scaling up and down the replicas,
-            # we need this shuffle to not let the first replica have the
-            # most of the load.
-            random.shuffle(ready_replicas)
-            self.ready_replicas = ready_replicas
-            self.index = 0
+        if set(self.ready_replicas) == set(ready_replicas):
+            return
+        # If the autoscaler keeps scaling up and down the replicas,
+        # we need this shuffle to not let the first replica have the
+        # most of the load.
+        random.shuffle(ready_replicas)
+        self.ready_replicas = ready_replicas
+        self.index = 0
 
-    def select_replica(self, request: 'fastapi.Request') -> Optional[str]:
+    def _select_replica(self, request: 'fastapi.Request') -> Optional[str]:
+        del request  # Unused.
         if not self.ready_replicas:
             return None
         ready_replica_url = self.ready_replicas[self.index]
         self.index = (self.index + 1) % len(self.ready_replicas)
-        request_repr = ('<Request '
-                        f'method="{request.method}" '
-                        f'url="{request.url}" '
-                        f'headers={dict(request.headers)} '
-                        f'query_params={dict(request.query_params)}'
-                        '>')
-        logger.info(f'Selected replica {ready_replica_url} '
-                    f'for request {request_repr}')
         return ready_replica_url
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240515/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240515/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240515/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240515/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240515/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/task.py` & `skypilot_nightly-1.0.0.dev20240515/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/jobs-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/jobs-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/sky-serve-controller.yaml.j2`

 * *Files 16% similar despite different names*

```diff
@@ -7,16 +7,18 @@
   # This is for multicloud support. To allow controller launch on all clouds,
   # we need to install all cloud dependencies.
   {%- for cmd in cloud_dependencies_installation_commands %}
   {{cmd}}
   {%- endfor %}
 
   # Install serve dependencies.
+  # TODO(tian): Gather those into serve constants.
   pip list | grep uvicorn > /dev/null 2>&1 || pip install uvicorn > /dev/null 2>&1
   pip list | grep fastapi > /dev/null 2>&1 || pip install fastapi > /dev/null 2>&1
+  pip list | grep httpx > /dev/null 2>&1 || pip install httpx > /dev/null 2>&1
 
 file_mounts:
   {{remote_task_yaml_path}}: {{local_task_yaml_path}}
   {{remote_user_config_path}}: skypilot:local_skypilot_config_path
   {%- for remote_catalog_path, local_catalog_path in modified_catalogs.items() %}
   {{remote_catalog_path}}: {{local_catalog_path}}
   {%- endfor %}
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240515/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240515/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240515/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/generate_static_kubeconfig.sh` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/generate_static_kubeconfig.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240515/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240514
+Version: 1.0.0.dev20240515
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240515/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_jobs_and_serve.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_jobs_and_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_smoke.py`

 * *Files 1% similar despite different names*

```diff
@@ -8668,4815 +8668,4854 @@
 00021db0: 494c 5f52 4541 4459 2e66 6f72 6d61 7428  IL_READY.format(
 00021dc0: 6e61 6d65 3d6e 616d 652c 2072 6570 6c69  name=name, repli
 00021dd0: 6361 5f6e 756d 3d32 292c 0a20 2020 2020  ca_num=2),.     
 00021de0: 2020 2020 2020 2066 277b 5f53 4552 5645         f'{_SERVE
 00021df0: 5f45 4e44 504f 494e 545f 5741 4954 2e66  _ENDPOINT_WAIT.f
 00021e00: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
 00021e10: 7d3b 2027 0a20 2020 2020 2020 2020 2020  }; '.           
-00021e20: 2027 6375 726c 202d 4c20 6874 7470 3a2f   'curl -L http:/
-00021e30: 2f24 656e 6470 6f69 6e74 207c 2067 7265  /$endpoint | gre
-00021e40: 7020 2248 692c 2053 6b79 5069 6c6f 7420  p "Hi, SkyPilot 
-00021e50: 6865 7265 2227 2c0a 2020 2020 2020 2020  here"',.        
-00021e60: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
-00021e70: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
-00021e80: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
-00021e90: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-00021ea0: 7469 6d65 6f75 745f 6d69 6e75 7465 7320  timeout_minutes 
-00021eb0: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
-00021ec0: 7265 7475 726e 2074 6573 740a 0a0a 6465  return test...de
-00021ed0: 6620 5f63 6865 636b 5f72 6570 6c69 6361  f _check_replica
-00021ee0: 5f69 6e5f 7374 6174 7573 286e 616d 653a  _in_status(name:
-00021ef0: 2073 7472 2c20 6368 6563 6b5f 7475 706c   str, check_tupl
-00021f00: 6573 3a20 4c69 7374 5b54 7570 6c65 5b69  es: List[Tuple[i
-00021f10: 6e74 2c20 626f 6f6c 2c0a 2020 2020 2020  nt, bool,.      
+00021e20: 2027 6375 726c 2068 7474 703a 2f2f 2465   'curl http://$e
+00021e30: 6e64 706f 696e 7420 7c20 6772 6570 2022  ndpoint | grep "
+00021e40: 4869 2c20 536b 7950 696c 6f74 2068 6572  Hi, SkyPilot her
+00021e50: 6522 272c 0a20 2020 2020 2020 205d 2c0a  e"',.        ],.
+00021e60: 2020 2020 2020 2020 5f54 4541 5244 4f57          _TEARDOW
+00021e70: 4e5f 5345 5256 4943 452e 666f 726d 6174  N_SERVICE.format
+00021e80: 286e 616d 653d 6e61 6d65 292c 0a20 2020  (name=name),.   
+00021e90: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
+00021ea0: 656f 7574 5f6d 696e 7574 6573 202a 2036  eout_minutes * 6
+00021eb0: 302c 0a20 2020 2029 0a20 2020 2072 6574  0,.    ).    ret
+00021ec0: 7572 6e20 7465 7374 0a0a 0a64 6566 205f  urn test...def _
+00021ed0: 6368 6563 6b5f 7265 706c 6963 615f 696e  check_replica_in
+00021ee0: 5f73 7461 7475 7328 6e61 6d65 3a20 7374  _status(name: st
+00021ef0: 722c 2063 6865 636b 5f74 7570 6c65 733a  r, check_tuples:
+00021f00: 204c 6973 745b 5475 706c 655b 696e 742c   List[Tuple[int,
+00021f10: 2062 6f6f 6c2c 0a20 2020 2020 2020 2020   bool,.         
 00021f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f50: 2020 2020 2020 2020 2020 2073 7472 5d5d             str]]
-00021f60: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00021f70: 2243 6865 636b 2072 6570 6c69 6361 7327  "Check replicas'
-00021f80: 2073 7461 7475 7320 616e 6420 636f 756e   status and coun
-00021f90: 7420 696e 2073 6b79 2073 6572 7665 2073  t in sky serve s
-00021fa0: 7461 7475 730a 0a20 2020 2057 6520 7769  tatus..    We wi
-00021fb0: 6c6c 2063 6865 636b 2076 4350 553d 322c  ll check vCPU=2,
-00021fc0: 2061 7320 616c 6c20 6f75 7220 7465 7374   as all our test
-00021fd0: 7320 7573 6520 7643 5055 3d32 2e0a 2020  s use vCPU=2..  
-00021fe0: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
-00021ff0: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-00022000: 616d 6520 6f66 2074 6865 2073 6572 7669  ame of the servi
-00022010: 6365 0a20 2020 2020 2020 2063 6865 636b  ce.        check
-00022020: 5f74 7570 6c65 733a 2041 206c 6973 7420  _tuples: A list 
-00022030: 6f66 2072 6570 6c69 6361 2070 726f 7065  of replica prope
-00022040: 7274 7920 746f 2063 6865 636b 2e20 4561  rty to check. Ea
-00022050: 6368 2074 7570 6c65 2069 730a 2020 2020  ch tuple is.    
-00022060: 2020 2020 2020 2020 2863 6f75 6e74 2c20          (count, 
-00022070: 6973 5f73 706f 742c 2073 7461 7475 7329  is_spot, status)
-00022080: 0a20 2020 2022 2222 0a20 2020 2063 6865  .    """.    che
-00022090: 636b 5f63 6d64 203d 2027 270a 2020 2020  ck_cmd = ''.    
-000220a0: 666f 7220 6368 6563 6b5f 7475 706c 6520  for check_tuple 
-000220b0: 696e 2063 6865 636b 5f74 7570 6c65 733a  in check_tuples:
-000220c0: 0a20 2020 2020 2020 2063 6f75 6e74 2c20  .        count, 
-000220d0: 6973 5f73 706f 742c 2073 7461 7475 7320  is_spot, status 
-000220e0: 3d20 6368 6563 6b5f 7475 706c 650a 2020  = check_tuple.  
-000220f0: 2020 2020 2020 7265 736f 7572 6365 5f73        resource_s
-00022100: 7472 203d 2027 270a 2020 2020 2020 2020  tr = ''.        
-00022110: 6966 2073 7461 7475 7320 6e6f 7420 696e  if status not in
-00022120: 205b 2750 454e 4449 4e47 272c 2027 5348   ['PENDING', 'SH
-00022130: 5554 5449 4e47 5f44 4f57 4e27 0a20 2020  UTTING_DOWN'.   
+00021f50: 2020 2020 2020 2020 7374 725d 5d29 202d          str]]) -
+00021f60: 3e20 7374 723a 0a20 2020 2022 2222 4368  > str:.    """Ch
+00021f70: 6563 6b20 7265 706c 6963 6173 2720 7374  eck replicas' st
+00021f80: 6174 7573 2061 6e64 2063 6f75 6e74 2069  atus and count i
+00021f90: 6e20 736b 7920 7365 7276 6520 7374 6174  n sky serve stat
+00021fa0: 7573 0a0a 2020 2020 5765 2077 696c 6c20  us..    We will 
+00021fb0: 6368 6563 6b20 7643 5055 3d32 2c20 6173  check vCPU=2, as
+00021fc0: 2061 6c6c 206f 7572 2074 6573 7473 2075   all our tests u
+00021fd0: 7365 2076 4350 553d 322e 0a20 2020 200a  se vCPU=2..    .
+00021fe0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00021ff0: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
+00022000: 206f 6620 7468 6520 7365 7276 6963 650a   of the service.
+00022010: 2020 2020 2020 2020 6368 6563 6b5f 7475          check_tu
+00022020: 706c 6573 3a20 4120 6c69 7374 206f 6620  ples: A list of 
+00022030: 7265 706c 6963 6120 7072 6f70 6572 7479  replica property
+00022040: 2074 6f20 6368 6563 6b2e 2045 6163 6820   to check. Each 
+00022050: 7475 706c 6520 6973 0a20 2020 2020 2020  tuple is.       
+00022060: 2020 2020 2028 636f 756e 742c 2069 735f       (count, is_
+00022070: 7370 6f74 2c20 7374 6174 7573 290a 2020  spot, status).  
+00022080: 2020 2222 220a 2020 2020 6368 6563 6b5f    """.    check_
+00022090: 636d 6420 3d20 2727 0a20 2020 2066 6f72  cmd = ''.    for
+000220a0: 2063 6865 636b 5f74 7570 6c65 2069 6e20   check_tuple in 
+000220b0: 6368 6563 6b5f 7475 706c 6573 3a0a 2020  check_tuples:.  
+000220c0: 2020 2020 2020 636f 756e 742c 2069 735f        count, is_
+000220d0: 7370 6f74 2c20 7374 6174 7573 203d 2063  spot, status = c
+000220e0: 6865 636b 5f74 7570 6c65 0a20 2020 2020  heck_tuple.     
+000220f0: 2020 2072 6573 6f75 7263 655f 7374 7220     resource_str 
+00022100: 3d20 2727 0a20 2020 2020 2020 2069 6620  = ''.        if 
+00022110: 7374 6174 7573 206e 6f74 2069 6e20 5b27  status not in ['
+00022120: 5045 4e44 494e 4727 2c20 2753 4855 5454  PENDING', 'SHUTT
+00022130: 494e 475f 444f 574e 270a 2020 2020 2020  ING_DOWN'.      
 00022140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022150: 2020 2020 2020 5d20 616e 6420 6e6f 7420        ] and not 
-00022160: 7374 6174 7573 2e73 7461 7274 7377 6974  status.startswit
-00022170: 6828 2746 4149 4c45 4427 293a 0a20 2020  h('FAILED'):.   
-00022180: 2020 2020 2020 2020 2073 706f 745f 7374           spot_st
-00022190: 7220 3d20 2727 0a20 2020 2020 2020 2020  r = ''.         
-000221a0: 2020 2069 6620 6973 5f73 706f 743a 0a20     if is_spot:. 
-000221b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000221c0: 706f 745f 7374 7220 3d20 275c 5b53 706f  pot_str = '\[Spo
-000221d0: 745c 5d27 0a20 2020 2020 2020 2020 2020  t\]'.           
-000221e0: 2072 6573 6f75 7263 655f 7374 7220 3d20   resource_str = 
-000221f0: 6627 287b 7370 6f74 5f73 7472 7d76 4350  f'({spot_str}vCP
-00022200: 553d 3229 270a 2020 2020 2020 2020 6368  U=2)'.        ch
-00022210: 6563 6b5f 636d 6420 2b3d 2028 6627 2065  eck_cmd += (f' e
-00022220: 6368 6f20 2224 7322 207c 2067 7265 7020  cho "$s" | grep 
-00022230: 227b 7265 736f 7572 6365 5f73 7472 7d22  "{resource_str}"
-00022240: 207c 2027 0a20 2020 2020 2020 2020 2020   | '.           
-00022250: 2020 2020 2020 2020 2020 2066 2767 7265             f'gre
-00022260: 7020 227b 7374 6174 7573 7d22 207c 2077  p "{status}" | w
-00022270: 6320 2d6c 207c 2067 7265 7020 7b63 6f75  c -l | grep {cou
-00022280: 6e74 7d20 7c7c 2065 7869 7420 313b 2729  nt} || exit 1;')
-00022290: 0a20 2020 2072 6574 7572 6e20 2866 277b  .    return (f'{
-000222a0: 5f53 4552 5645 5f53 5441 5455 535f 5741  _SERVE_STATUS_WA
-000222b0: 4954 2e66 6f72 6d61 7428 6e61 6d65 3d6e  IT.format(name=n
-000222c0: 616d 6529 7d3b 2065 6368 6f20 2224 7322  ame)}; echo "$s"
-000222d0: 3b20 2720 2b20 6368 6563 6b5f 636d 6429  ; ' + check_cmd)
-000222e0: 0a0a 0a64 6566 205f 6368 6563 6b5f 7365  ...def _check_se
-000222f0: 7276 6963 655f 7665 7273 696f 6e28 7365  rvice_version(se
-00022300: 7276 6963 655f 6e61 6d65 3a20 7374 722c  rvice_name: str,
-00022310: 2076 6572 7369 6f6e 3a20 7374 7229 202d   version: str) -
-00022320: 3e20 7374 723a 0a20 2020 2023 2047 7265  > str:.    # Gre
-00022330: 7020 7468 6520 6c69 6e65 7320 6265 666f  p the lines befo
-00022340: 7265 2027 5365 7276 6963 6520 5265 706c  re 'Service Repl
-00022350: 6963 6173 2720 616e 6420 6368 6563 6b20  icas' and check 
-00022360: 6966 2074 6865 2073 6572 7669 6365 2076  if the service v
-00022370: 6572 7369 6f6e 0a20 2020 2023 2069 7320  ersion.    # is 
-00022380: 636f 7272 6563 742e 0a20 2020 2072 6574  correct..    ret
-00022390: 7572 6e20 2866 2765 6368 6f20 2224 7322  urn (f'echo "$s"
-000223a0: 207c 2067 7265 7020 2d42 3130 3030 2022   | grep -B1000 "
-000223b0: 5365 7276 6963 6520 5265 706c 6963 6173  Service Replicas
-000223c0: 2220 7c20 270a 2020 2020 2020 2020 2020  " | '.          
-000223d0: 2020 6627 6772 6570 202d 4520 227b 7365    f'grep -E "{se
-000223e0: 7276 6963 655f 6e61 6d65 7d5c 732b 7b76  rvice_name}\s+{v
-000223f0: 6572 7369 6f6e 7d22 207c 7c20 6578 6974  ersion}" || exit
-00022400: 2031 3b20 2729 0a0a 0a40 7079 7465 7374   1; ')...@pytest
-00022410: 2e6d 6172 6b2e 6763 700a 4070 7974 6573  .mark.gcp.@pytes
-00022420: 742e 6d61 726b 2e73 6572 7665 0a64 6566  t.mark.serve.def
-00022430: 2074 6573 745f 736b 7973 6572 7665 5f67   test_skyserve_g
-00022440: 6370 5f68 7474 7028 293a 0a20 2020 2022  cp_http():.    "
-00022450: 2222 5465 7374 2073 6b79 7365 7276 6520  ""Test skyserve 
-00022460: 6f6e 2047 4350 2222 220a 2020 2020 6e61  on GCP""".    na
-00022470: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
-00022480: 655f 6e61 6d65 2829 0a20 2020 2074 6573  e_name().    tes
-00022490: 7420 3d20 5f67 6574 5f73 6b79 7365 7276  t = _get_skyserv
-000224a0: 655f 6874 7470 5f74 6573 7428 6e61 6d65  e_http_test(name
-000224b0: 2c20 2767 6370 272c 2032 3029 0a20 2020  , 'gcp', 20).   
-000224c0: 2072 756e 5f6f 6e65 5f74 6573 7428 7465   run_one_test(te
-000224d0: 7374 290a 0a0a 4070 7974 6573 742e 6d61  st)...@pytest.ma
-000224e0: 726b 2e61 7773 0a40 7079 7465 7374 2e6d  rk.aws.@pytest.m
-000224f0: 6172 6b2e 7365 7276 650a 6465 6620 7465  ark.serve.def te
-00022500: 7374 5f73 6b79 7365 7276 655f 6177 735f  st_skyserve_aws_
-00022510: 6874 7470 2829 3a0a 2020 2020 2222 2254  http():.    """T
-00022520: 6573 7420 736b 7973 6572 7665 206f 6e20  est skyserve on 
-00022530: 4157 5322 2222 0a20 2020 206e 616d 6520  AWS""".    name 
-00022540: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
-00022550: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
-00022560: 205f 6765 745f 736b 7973 6572 7665 5f68   _get_skyserve_h
-00022570: 7474 705f 7465 7374 286e 616d 652c 2027  ttp_test(name, '
-00022580: 6177 7327 2c20 3230 290a 2020 2020 7275  aws', 20).    ru
-00022590: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
-000225a0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
-000225b0: 617a 7572 650a 4070 7974 6573 742e 6d61  azure.@pytest.ma
-000225c0: 726b 2e73 6572 7665 0a64 6566 2074 6573  rk.serve.def tes
-000225d0: 745f 736b 7973 6572 7665 5f61 7a75 7265  t_skyserve_azure
-000225e0: 5f68 7474 7028 293a 0a20 2020 2022 2222  _http():.    """
-000225f0: 5465 7374 2073 6b79 7365 7276 6520 6f6e  Test skyserve on
-00022600: 2041 7a75 7265 2222 220a 2020 2020 6e61   Azure""".    na
-00022610: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
-00022620: 655f 6e61 6d65 2829 0a20 2020 2074 6573  e_name().    tes
-00022630: 7420 3d20 5f67 6574 5f73 6b79 7365 7276  t = _get_skyserv
-00022640: 655f 6874 7470 5f74 6573 7428 6e61 6d65  e_http_test(name
-00022650: 2c20 2761 7a75 7265 272c 2033 3029 0a20  , 'azure', 30). 
-00022660: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-00022670: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-00022680: 6d61 726b 2e6b 7562 6572 6e65 7465 730a  mark.kubernetes.
-00022690: 4070 7974 6573 742e 6d61 726b 2e73 6572  @pytest.mark.ser
-000226a0: 7665 0a64 6566 2074 6573 745f 736b 7973  ve.def test_skys
-000226b0: 6572 7665 5f6b 7562 6572 6e65 7465 735f  erve_kubernetes_
-000226c0: 6874 7470 2829 3a0a 2020 2020 2222 2254  http():.    """T
-000226d0: 6573 7420 736b 7973 6572 7665 206f 6e20  est skyserve on 
-000226e0: 4b75 6265 726e 6574 6573 2222 220a 2020  Kubernetes""".  
-000226f0: 2020 6e61 6d65 203d 205f 6765 745f 7365    name = _get_se
-00022700: 7276 6963 655f 6e61 6d65 2829 0a20 2020  rvice_name().   
-00022710: 2074 6573 7420 3d20 5f67 6574 5f73 6b79   test = _get_sky
-00022720: 7365 7276 655f 6874 7470 5f74 6573 7428  serve_http_test(
-00022730: 6e61 6d65 2c20 276b 7562 6572 6e65 7465  name, 'kubernete
-00022740: 7327 2c20 3330 290a 2020 2020 7275 6e5f  s', 30).    run_
-00022750: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
-00022760: 0a40 7079 7465 7374 2e6d 6172 6b2e 7365  .@pytest.mark.se
-00022770: 7276 650a 6465 6620 7465 7374 5f73 6b79  rve.def test_sky
-00022780: 7365 7276 655f 6c6c 6d28 6765 6e65 7269  serve_llm(generi
-00022790: 635f 636c 6f75 643a 2073 7472 293a 0a20  c_cloud: str):. 
-000227a0: 2020 2022 2222 5465 7374 2073 6b79 7365     """Test skyse
-000227b0: 7276 6520 7769 7468 2072 6561 6c20 4c4c  rve with real LL
-000227c0: 4d20 7573 6563 6173 6522 2222 0a20 2020  M usecase""".   
-000227d0: 206e 616d 6520 3d20 5f67 6574 5f73 6572   name = _get_ser
-000227e0: 7669 6365 5f6e 616d 6528 290a 0a20 2020  vice_name()..   
-000227f0: 2064 6566 2067 656e 6572 6174 655f 6c6c   def generate_ll
-00022800: 6d5f 7465 7374 5f63 6f6d 6d61 6e64 2870  m_test_command(p
-00022810: 726f 6d70 743a 2073 7472 2c20 6578 7065  rompt: str, expe
-00022820: 6374 6564 5f6f 7574 7075 743a 2073 7472  cted_output: str
-00022830: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00022840: 2020 7072 6f6d 7074 203d 2073 686c 6578    prompt = shlex
-00022850: 2e71 756f 7465 2870 726f 6d70 7429 0a20  .quote(prompt). 
-00022860: 2020 2020 2020 2065 7870 6563 7465 645f         expected_
-00022870: 6f75 7470 7574 203d 2073 686c 6578 2e71  output = shlex.q
-00022880: 756f 7465 2865 7870 6563 7465 645f 6f75  uote(expected_ou
-00022890: 7470 7574 290a 2020 2020 2020 2020 7265  tput).        re
-000228a0: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
-000228b0: 2020 2066 277b 5f53 4552 5645 5f45 4e44     f'{_SERVE_END
-000228c0: 504f 494e 545f 5741 4954 2e66 6f72 6d61  POINT_WAIT.forma
-000228d0: 7428 6e61 6d65 3d6e 616d 6529 7d3b 2027  t(name=name)}; '
-000228e0: 0a20 2020 2020 2020 2020 2020 2027 7079  .            'py
-000228f0: 7468 6f6e 2074 6573 7473 2f73 6b79 7365  thon tests/skyse
-00022900: 7276 652f 6c6c 6d2f 6765 745f 7265 7370  rve/llm/get_resp
-00022910: 6f6e 7365 2e70 7920 2d2d 656e 6470 6f69  onse.py --endpoi
-00022920: 6e74 2024 656e 6470 6f69 6e74 2027 0a20  nt $endpoint '. 
-00022930: 2020 2020 2020 2020 2020 2066 272d 2d70             f'--p
-00022940: 726f 6d70 7420 7b70 726f 6d70 747d 207c  rompt {prompt} |
-00022950: 2067 7265 7020 7b65 7870 6563 7465 645f   grep {expected_
-00022960: 6f75 7470 7574 7d27 290a 0a20 2020 2077  output}')..    w
-00022970: 6974 6820 6f70 656e 2827 7465 7374 732f  ith open('tests/
-00022980: 736b 7973 6572 7665 2f6c 6c6d 2f70 726f  skyserve/llm/pro
-00022990: 6d70 745f 6f75 7470 7574 2e6a 736f 6e27  mpt_output.json'
-000229a0: 2c20 2772 272c 0a20 2020 2020 2020 2020  , 'r',.         
-000229b0: 2020 2020 2065 6e63 6f64 696e 673d 2775       encoding='u
-000229c0: 7466 2d38 2729 2061 7320 663a 0a20 2020  tf-8') as f:.   
-000229d0: 2020 2020 2070 726f 6d70 7432 6f75 7470       prompt2outp
-000229e0: 7574 203d 206a 736f 6e2e 6c6f 6164 2866  ut = json.load(f
-000229f0: 290a 0a20 2020 2074 6573 7420 3d20 5465  )..    test = Te
-00022a00: 7374 280a 2020 2020 2020 2020 6627 7465  st(.        f'te
-00022a10: 7374 2d73 6b79 7365 7276 652d 6c6c 6d27  st-skyserve-llm'
-00022a20: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-00022a30: 2020 2020 2020 2020 6627 736b 7920 7365          f'sky se
-00022a40: 7276 6520 7570 202d 6e20 7b6e 616d 657d  rve up -n {name}
-00022a50: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
-00022a60: 635f 636c 6f75 647d 202d 7920 7465 7374  c_cloud} -y test
-00022a70: 732f 736b 7973 6572 7665 2f6c 6c6d 2f73  s/skyserve/llm/s
-00022a80: 6572 7669 6365 2e79 616d 6c27 2c0a 2020  ervice.yaml',.  
-00022a90: 2020 2020 2020 2020 2020 5f53 4552 5645            _SERVE
-00022aa0: 5f57 4149 545f 554e 5449 4c5f 5245 4144  _WAIT_UNTIL_READ
-00022ab0: 592e 666f 726d 6174 286e 616d 653d 6e61  Y.format(name=na
-00022ac0: 6d65 2c20 7265 706c 6963 615f 6e75 6d3d  me, replica_num=
-00022ad0: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
-00022ae0: 2a5b 0a20 2020 2020 2020 2020 2020 2020  *[.             
-00022af0: 2020 2067 656e 6572 6174 655f 6c6c 6d5f     generate_llm_
-00022b00: 7465 7374 5f63 6f6d 6d61 6e64 2870 726f  test_command(pro
-00022b10: 6d70 742c 206f 7574 7075 7429 0a20 2020  mpt, output).   
-00022b20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00022b30: 2070 726f 6d70 742c 206f 7574 7075 7420   prompt, output 
-00022b40: 696e 2070 726f 6d70 7432 6f75 7470 7574  in prompt2output
-00022b50: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
-00022b60: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00022b70: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
-00022b80: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
-00022b90: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
-00022ba0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-00022bb0: 3430 202a 2036 302c 0a20 2020 2029 0a20  40 * 60,.    ). 
-00022bc0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-00022bd0: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-00022be0: 6d61 726b 2e67 6370 0a40 7079 7465 7374  mark.gcp.@pytest
-00022bf0: 2e6d 6172 6b2e 7365 7276 650a 6465 6620  .mark.serve.def 
-00022c00: 7465 7374 5f73 6b79 7365 7276 655f 7370  test_skyserve_sp
-00022c10: 6f74 5f72 6563 6f76 6572 7928 293a 0a20  ot_recovery():. 
-00022c20: 2020 206e 616d 6520 3d20 5f67 6574 5f73     name = _get_s
-00022c30: 6572 7669 6365 5f6e 616d 6528 290a 2020  ervice_name().  
-00022c40: 2020 7a6f 6e65 203d 2027 7573 2d63 656e    zone = 'us-cen
-00022c50: 7472 616c 312d 6127 0a0a 2020 2020 7465  tral1-a'..    te
-00022c60: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00022c70: 2020 2066 2774 6573 742d 736b 7973 6572     f'test-skyser
-00022c80: 7665 2d73 706f 742d 7265 636f 7665 7279  ve-spot-recovery
-00022c90: 2d67 6370 272c 0a20 2020 2020 2020 205b  -gcp',.        [
-00022ca0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00022cb0: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
-00022cc0: 6e61 6d65 7d20 2d79 2074 6573 7473 2f73  name} -y tests/s
-00022cd0: 6b79 7365 7276 652f 7370 6f74 2f72 6563  kyserve/spot/rec
-00022ce0: 6f76 6572 792e 7961 6d6c 272c 0a20 2020  overy.yaml',.   
-00022cf0: 2020 2020 2020 2020 205f 5345 5256 455f           _SERVE_
-00022d00: 5741 4954 5f55 4e54 494c 5f52 4541 4459  WAIT_UNTIL_READY
-00022d10: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
-00022d20: 652c 2072 6570 6c69 6361 5f6e 756d 3d31  e, replica_num=1
-00022d30: 292c 0a20 2020 2020 2020 2020 2020 2066  ),.            f
-00022d40: 277b 5f53 4552 5645 5f45 4e44 504f 494e  '{_SERVE_ENDPOIN
-00022d50: 545f 5741 4954 2e66 6f72 6d61 7428 6e61  T_WAIT.format(na
-00022d60: 6d65 3d6e 616d 6529 7d3b 2027 0a20 2020  me=name)}; '.   
-00022d70: 2020 2020 2020 2020 2027 7265 7175 6573           'reques
-00022d80: 745f 6f75 7470 7574 3d24 2863 7572 6c20  t_output=$(curl 
-00022d90: 2d4c 2068 7474 703a 2f2f 2465 6e64 706f  -L http://$endpo
-00022da0: 696e 7429 3b20 6563 686f 2022 2472 6571  int); echo "$req
-00022db0: 7565 7374 5f6f 7574 7075 7422 3b20 6563  uest_output"; ec
-00022dc0: 686f 2022 2472 6571 7565 7374 5f6f 7574  ho "$request_out
-00022dd0: 7075 7422 207c 2067 7265 7020 2248 692c  put" | grep "Hi,
-00022de0: 2053 6b79 5069 6c6f 7420 6865 7265 2227   SkyPilot here"'
-00022df0: 2c0a 2020 2020 2020 2020 2020 2020 5f74  ,.            _t
-00022e00: 6572 6d69 6e61 7465 5f67 6370 5f72 6570  erminate_gcp_rep
-00022e10: 6c69 6361 286e 616d 652c 207a 6f6e 652c  lica(name, zone,
-00022e20: 2031 292c 0a20 2020 2020 2020 2020 2020   1),.           
-00022e30: 205f 5345 5256 455f 5741 4954 5f55 4e54   _SERVE_WAIT_UNT
-00022e40: 494c 5f52 4541 4459 2e66 6f72 6d61 7428  IL_READY.format(
-00022e50: 6e61 6d65 3d6e 616d 652c 2072 6570 6c69  name=name, repli
-00022e60: 6361 5f6e 756d 3d31 292c 0a20 2020 2020  ca_num=1),.     
-00022e70: 2020 2020 2020 2066 277b 5f53 4552 5645         f'{_SERVE
-00022e80: 5f45 4e44 504f 494e 545f 5741 4954 2e66  _ENDPOINT_WAIT.f
-00022e90: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
-00022ea0: 7d3b 2027 0a20 2020 2020 2020 2020 2020  }; '.           
-00022eb0: 2027 7265 7175 6573 745f 6f75 7470 7574   'request_output
-00022ec0: 3d24 2863 7572 6c20 2d4c 2068 7474 703a  =$(curl -L http:
-00022ed0: 2f2f 2465 6e64 706f 696e 7429 3b20 6563  //$endpoint); ec
-00022ee0: 686f 2022 2472 6571 7565 7374 5f6f 7574  ho "$request_out
-00022ef0: 7075 7422 3b20 6563 686f 2022 2472 6571  put"; echo "$req
-00022f00: 7565 7374 5f6f 7574 7075 7422 207c 2067  uest_output" | g
-00022f10: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
-00022f20: 7420 6865 7265 2227 2c0a 2020 2020 2020  t here"',.      
-00022f30: 2020 5d2c 0a20 2020 2020 2020 205f 5445    ],.        _TE
-00022f40: 4152 444f 574e 5f53 4552 5649 4345 2e66  ARDOWN_SERVICE.f
-00022f50: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
-00022f60: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
-00022f70: 743d 3230 202a 2036 302c 0a20 2020 2029  t=20 * 60,.    )
-00022f80: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
-00022f90: 7428 7465 7374 290a 0a0a 4070 7974 6573  t(test)...@pytes
-00022fa0: 742e 6d61 726b 2e73 6572 7665 0a40 7079  t.mark.serve.@py
-00022fb0: 7465 7374 2e6d 6172 6b2e 6e6f 5f6b 7562  test.mark.no_kub
-00022fc0: 6572 6e65 7465 730a 6465 6620 7465 7374  ernetes.def test
-00022fd0: 5f73 6b79 7365 7276 655f 6261 7365 5f6f  _skyserve_base_o
-00022fe0: 6e64 656d 616e 645f 6661 6c6c 6261 636b  ndemand_fallback
-00022ff0: 2867 656e 6572 6963 5f63 6c6f 7564 3a20  (generic_cloud: 
-00023000: 7374 7229 3a0a 2020 2020 6e61 6d65 203d  str):.    name =
-00023010: 205f 6765 745f 7365 7276 6963 655f 6e61   _get_service_na
-00023020: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-00023030: 5465 7374 280a 2020 2020 2020 2020 6627  Test(.        f'
-00023040: 7465 7374 2d73 6b79 7365 7276 652d 6261  test-skyserve-ba
-00023050: 7365 2d6f 6e64 656d 616e 642d 6661 6c6c  se-ondemand-fall
-00023060: 6261 636b 272c 0a20 2020 2020 2020 205b  back',.        [
-00023070: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00023080: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
-00023090: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
-000230a0: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
-000230b0: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
-000230c0: 7370 6f74 2f62 6173 655f 6f6e 6465 6d61  spot/base_ondema
-000230d0: 6e64 5f66 616c 6c62 6163 6b2e 7961 6d6c  nd_fallback.yaml
-000230e0: 272c 0a20 2020 2020 2020 2020 2020 205f  ',.            _
-000230f0: 5345 5256 455f 5741 4954 5f55 4e54 494c  SERVE_WAIT_UNTIL
-00023100: 5f52 4541 4459 2e66 6f72 6d61 7428 6e61  _READY.format(na
-00023110: 6d65 3d6e 616d 652c 2072 6570 6c69 6361  me=name, replica
-00023120: 5f6e 756d 3d32 292c 0a20 2020 2020 2020  _num=2),.       
-00023130: 2020 2020 205f 6368 6563 6b5f 7265 706c       _check_repl
-00023140: 6963 615f 696e 5f73 7461 7475 7328 6e61  ica_in_status(na
-00023150: 6d65 2c20 5b28 312c 2054 7275 652c 2027  me, [(1, True, '
-00023160: 5245 4144 5927 292c 0a20 2020 2020 2020  READY'),.       
+00022150: 2020 205d 2061 6e64 206e 6f74 2073 7461     ] and not sta
+00022160: 7475 732e 7374 6172 7473 7769 7468 2827  tus.startswith('
+00022170: 4641 494c 4544 2729 3a0a 2020 2020 2020  FAILED'):.      
+00022180: 2020 2020 2020 7370 6f74 5f73 7472 203d        spot_str =
+00022190: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
+000221a0: 6966 2069 735f 7370 6f74 3a0a 2020 2020  if is_spot:.    
+000221b0: 2020 2020 2020 2020 2020 2020 7370 6f74              spot
+000221c0: 5f73 7472 203d 2027 5c5b 5370 6f74 5c5d  _str = '\[Spot\]
+000221d0: 270a 2020 2020 2020 2020 2020 2020 7265  '.            re
+000221e0: 736f 7572 6365 5f73 7472 203d 2066 2728  source_str = f'(
+000221f0: 7b73 706f 745f 7374 727d 7643 5055 3d32  {spot_str}vCPU=2
+00022200: 2927 0a20 2020 2020 2020 2063 6865 636b  )'.        check
+00022210: 5f63 6d64 202b 3d20 2866 2720 6563 686f  _cmd += (f' echo
+00022220: 2022 2473 2220 7c20 6772 6570 2022 7b72   "$s" | grep "{r
+00022230: 6573 6f75 7263 655f 7374 727d 2220 7c20  esource_str}" | 
+00022240: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00022250: 2020 2020 2020 2020 6627 6772 6570 2022          f'grep "
+00022260: 7b73 7461 7475 737d 2220 7c20 7763 202d  {status}" | wc -
+00022270: 6c20 7c20 6772 6570 207b 636f 756e 747d  l | grep {count}
+00022280: 207c 7c20 6578 6974 2031 3b27 290a 2020   || exit 1;').  
+00022290: 2020 7265 7475 726e 2028 6627 7b5f 5345    return (f'{_SE
+000222a0: 5256 455f 5354 4154 5553 5f57 4149 542e  RVE_STATUS_WAIT.
+000222b0: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
+000222c0: 297d 3b20 6563 686f 2022 2473 223b 2027  )}; echo "$s"; '
+000222d0: 202b 2063 6865 636b 5f63 6d64 290a 0a0a   + check_cmd)...
+000222e0: 6465 6620 5f63 6865 636b 5f73 6572 7669  def _check_servi
+000222f0: 6365 5f76 6572 7369 6f6e 2873 6572 7669  ce_version(servi
+00022300: 6365 5f6e 616d 653a 2073 7472 2c20 7665  ce_name: str, ve
+00022310: 7273 696f 6e3a 2073 7472 2920 2d3e 2073  rsion: str) -> s
+00022320: 7472 3a0a 2020 2020 2320 4772 6570 2074  tr:.    # Grep t
+00022330: 6865 206c 696e 6573 2062 6566 6f72 6520  he lines before 
+00022340: 2753 6572 7669 6365 2052 6570 6c69 6361  'Service Replica
+00022350: 7327 2061 6e64 2063 6865 636b 2069 6620  s' and check if 
+00022360: 7468 6520 7365 7276 6963 6520 7665 7273  the service vers
+00022370: 696f 6e0a 2020 2020 2320 6973 2063 6f72  ion.    # is cor
+00022380: 7265 6374 2e0a 2020 2020 7265 7475 726e  rect..    return
+00022390: 2028 6627 6563 686f 2022 2473 2220 7c20   (f'echo "$s" | 
+000223a0: 6772 6570 202d 4231 3030 3020 2253 6572  grep -B1000 "Ser
+000223b0: 7669 6365 2052 6570 6c69 6361 7322 207c  vice Replicas" |
+000223c0: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
+000223d0: 2767 7265 7020 2d45 2022 7b73 6572 7669  'grep -E "{servi
+000223e0: 6365 5f6e 616d 657d 5c73 2b7b 7665 7273  ce_name}\s+{vers
+000223f0: 696f 6e7d 2220 7c7c 2065 7869 7420 313b  ion}" || exit 1;
+00022400: 2027 290a 0a0a 4070 7974 6573 742e 6d61   ')...@pytest.ma
+00022410: 726b 2e67 6370 0a40 7079 7465 7374 2e6d  rk.gcp.@pytest.m
+00022420: 6172 6b2e 7365 7276 650a 6465 6620 7465  ark.serve.def te
+00022430: 7374 5f73 6b79 7365 7276 655f 6763 705f  st_skyserve_gcp_
+00022440: 6874 7470 2829 3a0a 2020 2020 2222 2254  http():.    """T
+00022450: 6573 7420 736b 7973 6572 7665 206f 6e20  est skyserve on 
+00022460: 4743 5022 2222 0a20 2020 206e 616d 6520  GCP""".    name 
+00022470: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
+00022480: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
+00022490: 205f 6765 745f 736b 7973 6572 7665 5f68   _get_skyserve_h
+000224a0: 7474 705f 7465 7374 286e 616d 652c 2027  ttp_test(name, '
+000224b0: 6763 7027 2c20 3230 290a 2020 2020 7275  gcp', 20).    ru
+000224c0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+000224d0: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+000224e0: 6177 730a 4070 7974 6573 742e 6d61 726b  aws.@pytest.mark
+000224f0: 2e73 6572 7665 0a64 6566 2074 6573 745f  .serve.def test_
+00022500: 736b 7973 6572 7665 5f61 7773 5f68 7474  skyserve_aws_htt
+00022510: 7028 293a 0a20 2020 2022 2222 5465 7374  p():.    """Test
+00022520: 2073 6b79 7365 7276 6520 6f6e 2041 5753   skyserve on AWS
+00022530: 2222 220a 2020 2020 6e61 6d65 203d 205f  """.    name = _
+00022540: 6765 745f 7365 7276 6963 655f 6e61 6d65  get_service_name
+00022550: 2829 0a20 2020 2074 6573 7420 3d20 5f67  ().    test = _g
+00022560: 6574 5f73 6b79 7365 7276 655f 6874 7470  et_skyserve_http
+00022570: 5f74 6573 7428 6e61 6d65 2c20 2761 7773  _test(name, 'aws
+00022580: 272c 2032 3029 0a20 2020 2072 756e 5f6f  ', 20).    run_o
+00022590: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+000225a0: 4070 7974 6573 742e 6d61 726b 2e61 7a75  @pytest.mark.azu
+000225b0: 7265 0a40 7079 7465 7374 2e6d 6172 6b2e  re.@pytest.mark.
+000225c0: 7365 7276 650a 6465 6620 7465 7374 5f73  serve.def test_s
+000225d0: 6b79 7365 7276 655f 617a 7572 655f 6874  kyserve_azure_ht
+000225e0: 7470 2829 3a0a 2020 2020 2222 2254 6573  tp():.    """Tes
+000225f0: 7420 736b 7973 6572 7665 206f 6e20 417a  t skyserve on Az
+00022600: 7572 6522 2222 0a20 2020 206e 616d 6520  ure""".    name 
+00022610: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
+00022620: 616d 6528 290a 2020 2020 7465 7374 203d  ame().    test =
+00022630: 205f 6765 745f 736b 7973 6572 7665 5f68   _get_skyserve_h
+00022640: 7474 705f 7465 7374 286e 616d 652c 2027  ttp_test(name, '
+00022650: 617a 7572 6527 2c20 3330 290a 2020 2020  azure', 30).    
+00022660: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00022670: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+00022680: 6b2e 6b75 6265 726e 6574 6573 0a40 7079  k.kubernetes.@py
+00022690: 7465 7374 2e6d 6172 6b2e 7365 7276 650a  test.mark.serve.
+000226a0: 6465 6620 7465 7374 5f73 6b79 7365 7276  def test_skyserv
+000226b0: 655f 6b75 6265 726e 6574 6573 5f68 7474  e_kubernetes_htt
+000226c0: 7028 293a 0a20 2020 2022 2222 5465 7374  p():.    """Test
+000226d0: 2073 6b79 7365 7276 6520 6f6e 204b 7562   skyserve on Kub
+000226e0: 6572 6e65 7465 7322 2222 0a20 2020 206e  ernetes""".    n
+000226f0: 616d 6520 3d20 5f67 6574 5f73 6572 7669  ame = _get_servi
+00022700: 6365 5f6e 616d 6528 290a 2020 2020 7465  ce_name().    te
+00022710: 7374 203d 205f 6765 745f 736b 7973 6572  st = _get_skyser
+00022720: 7665 5f68 7474 705f 7465 7374 286e 616d  ve_http_test(nam
+00022730: 652c 2027 6b75 6265 726e 6574 6573 272c  e, 'kubernetes',
+00022740: 2033 3029 0a20 2020 2072 756e 5f6f 6e65   30).    run_one
+00022750: 5f74 6573 7428 7465 7374 290a 0a0a 4070  _test(test)...@p
+00022760: 7974 6573 742e 6d61 726b 2e73 6572 7665  ytest.mark.serve
+00022770: 0a64 6566 2074 6573 745f 736b 7973 6572  .def test_skyser
+00022780: 7665 5f6c 6c6d 2867 656e 6572 6963 5f63  ve_llm(generic_c
+00022790: 6c6f 7564 3a20 7374 7229 3a0a 2020 2020  loud: str):.    
+000227a0: 2222 2254 6573 7420 736b 7973 6572 7665  """Test skyserve
+000227b0: 2077 6974 6820 7265 616c 204c 4c4d 2075   with real LLM u
+000227c0: 7365 6361 7365 2222 220a 2020 2020 6e61  secase""".    na
+000227d0: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
+000227e0: 655f 6e61 6d65 2829 0a0a 2020 2020 6465  e_name()..    de
+000227f0: 6620 6765 6e65 7261 7465 5f6c 6c6d 5f74  f generate_llm_t
+00022800: 6573 745f 636f 6d6d 616e 6428 7072 6f6d  est_command(prom
+00022810: 7074 3a20 7374 722c 2065 7870 6563 7465  pt: str, expecte
+00022820: 645f 6f75 7470 7574 3a20 7374 7229 202d  d_output: str) -
+00022830: 3e20 7374 723a 0a20 2020 2020 2020 2070  > str:.        p
+00022840: 726f 6d70 7420 3d20 7368 6c65 782e 7175  rompt = shlex.qu
+00022850: 6f74 6528 7072 6f6d 7074 290a 2020 2020  ote(prompt).    
+00022860: 2020 2020 6578 7065 6374 6564 5f6f 7574      expected_out
+00022870: 7075 7420 3d20 7368 6c65 782e 7175 6f74  put = shlex.quot
+00022880: 6528 6578 7065 6374 6564 5f6f 7574 7075  e(expected_outpu
+00022890: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
+000228a0: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
+000228b0: 6627 7b5f 5345 5256 455f 454e 4450 4f49  f'{_SERVE_ENDPOI
+000228c0: 4e54 5f57 4149 542e 666f 726d 6174 286e  NT_WAIT.format(n
+000228d0: 616d 653d 6e61 6d65 297d 3b20 270a 2020  ame=name)}; '.  
+000228e0: 2020 2020 2020 2020 2020 2770 7974 686f            'pytho
+000228f0: 6e20 7465 7374 732f 736b 7973 6572 7665  n tests/skyserve
+00022900: 2f6c 6c6d 2f67 6574 5f72 6573 706f 6e73  /llm/get_respons
+00022910: 652e 7079 202d 2d65 6e64 706f 696e 7420  e.py --endpoint 
+00022920: 2465 6e64 706f 696e 7420 270a 2020 2020  $endpoint '.    
+00022930: 2020 2020 2020 2020 6627 2d2d 7072 6f6d          f'--prom
+00022940: 7074 207b 7072 6f6d 7074 7d20 7c20 6772  pt {prompt} | gr
+00022950: 6570 207b 6578 7065 6374 6564 5f6f 7574  ep {expected_out
+00022960: 7075 747d 2729 0a0a 2020 2020 7769 7468  put}')..    with
+00022970: 206f 7065 6e28 2774 6573 7473 2f73 6b79   open('tests/sky
+00022980: 7365 7276 652f 6c6c 6d2f 7072 6f6d 7074  serve/llm/prompt
+00022990: 5f6f 7574 7075 742e 6a73 6f6e 272c 2027  _output.json', '
+000229a0: 7227 2c0a 2020 2020 2020 2020 2020 2020  r',.            
+000229b0: 2020 656e 636f 6469 6e67 3d27 7574 662d    encoding='utf-
+000229c0: 3827 2920 6173 2066 3a0a 2020 2020 2020  8') as f:.      
+000229d0: 2020 7072 6f6d 7074 326f 7574 7075 7420    prompt2output 
+000229e0: 3d20 6a73 6f6e 2e6c 6f61 6428 6629 0a0a  = json.load(f)..
+000229f0: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
+00022a00: 0a20 2020 2020 2020 2066 2774 6573 742d  .        f'test-
+00022a10: 736b 7973 6572 7665 2d6c 6c6d 272c 0a20  skyserve-llm',. 
+00022a20: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00022a30: 2020 2020 2066 2773 6b79 2073 6572 7665       f'sky serve
+00022a40: 2075 7020 2d6e 207b 6e61 6d65 7d20 2d2d   up -n {name} --
+00022a50: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+00022a60: 6c6f 7564 7d20 2d79 2074 6573 7473 2f73  loud} -y tests/s
+00022a70: 6b79 7365 7276 652f 6c6c 6d2f 7365 7276  kyserve/llm/serv
+00022a80: 6963 652e 7961 6d6c 272c 0a20 2020 2020  ice.yaml',.     
+00022a90: 2020 2020 2020 205f 5345 5256 455f 5741         _SERVE_WA
+00022aa0: 4954 5f55 4e54 494c 5f52 4541 4459 2e66  IT_UNTIL_READY.f
+00022ab0: 6f72 6d61 7428 6e61 6d65 3d6e 616d 652c  ormat(name=name,
+00022ac0: 2072 6570 6c69 6361 5f6e 756d 3d31 292c   replica_num=1),
+00022ad0: 0a20 2020 2020 2020 2020 2020 202a 5b0a  .            *[.
+00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022af0: 6765 6e65 7261 7465 5f6c 6c6d 5f74 6573  generate_llm_tes
+00022b00: 745f 636f 6d6d 616e 6428 7072 6f6d 7074  t_command(prompt
+00022b10: 2c20 6f75 7470 7574 290a 2020 2020 2020  , output).      
+00022b20: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
+00022b30: 6f6d 7074 2c20 6f75 7470 7574 2069 6e20  ompt, output in 
+00022b40: 7072 6f6d 7074 326f 7574 7075 742e 6974  prompt2output.it
+00022b50: 656d 7328 290a 2020 2020 2020 2020 2020  ems().          
+00022b60: 2020 5d2c 0a20 2020 2020 2020 205d 2c0a    ],.        ],.
+00022b70: 2020 2020 2020 2020 5f54 4541 5244 4f57          _TEARDOW
+00022b80: 4e5f 5345 5256 4943 452e 666f 726d 6174  N_SERVICE.format
+00022b90: 286e 616d 653d 6e61 6d65 292c 0a20 2020  (name=name),.   
+00022ba0: 2020 2020 2074 696d 656f 7574 3d34 3020       timeout=40 
+00022bb0: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
+00022bc0: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00022bd0: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+00022be0: 6b2e 6763 700a 4070 7974 6573 742e 6d61  k.gcp.@pytest.ma
+00022bf0: 726b 2e73 6572 7665 0a64 6566 2074 6573  rk.serve.def tes
+00022c00: 745f 736b 7973 6572 7665 5f73 706f 745f  t_skyserve_spot_
+00022c10: 7265 636f 7665 7279 2829 3a0a 2020 2020  recovery():.    
+00022c20: 6e61 6d65 203d 205f 6765 745f 7365 7276  name = _get_serv
+00022c30: 6963 655f 6e61 6d65 2829 0a20 2020 207a  ice_name().    z
+00022c40: 6f6e 6520 3d20 2775 732d 6365 6e74 7261  one = 'us-centra
+00022c50: 6c31 2d61 270a 0a20 2020 2074 6573 7420  l1-a'..    test 
+00022c60: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
+00022c70: 6627 7465 7374 2d73 6b79 7365 7276 652d  f'test-skyserve-
+00022c80: 7370 6f74 2d72 6563 6f76 6572 792d 6763  spot-recovery-gc
+00022c90: 7027 2c0a 2020 2020 2020 2020 5b0a 2020  p',.        [.  
+00022ca0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00022cb0: 7365 7276 6520 7570 202d 6e20 7b6e 616d  serve up -n {nam
+00022cc0: 657d 202d 7920 7465 7374 732f 736b 7973  e} -y tests/skys
+00022cd0: 6572 7665 2f73 706f 742f 7265 636f 7665  erve/spot/recove
+00022ce0: 7279 2e79 616d 6c27 2c0a 2020 2020 2020  ry.yaml',.      
+00022cf0: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
+00022d00: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
+00022d10: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
+00022d20: 7265 706c 6963 615f 6e75 6d3d 3129 2c0a  replica_num=1),.
+00022d30: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00022d40: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
+00022d50: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
+00022d60: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
+00022d70: 2020 2020 2020 2772 6571 7565 7374 5f6f        'request_o
+00022d80: 7574 7075 743d 2428 6375 726c 2068 7474  utput=$(curl htt
+00022d90: 703a 2f2f 2465 6e64 706f 696e 7429 3b20  p://$endpoint); 
+00022da0: 6563 686f 2022 2472 6571 7565 7374 5f6f  echo "$request_o
+00022db0: 7574 7075 7422 3b20 6563 686f 2022 2472  utput"; echo "$r
+00022dc0: 6571 7565 7374 5f6f 7574 7075 7422 207c  equest_output" |
+00022dd0: 2067 7265 7020 2248 692c 2053 6b79 5069   grep "Hi, SkyPi
+00022de0: 6c6f 7420 6865 7265 2227 2c0a 2020 2020  lot here"',.    
+00022df0: 2020 2020 2020 2020 5f74 6572 6d69 6e61          _termina
+00022e00: 7465 5f67 6370 5f72 6570 6c69 6361 286e  te_gcp_replica(n
+00022e10: 616d 652c 207a 6f6e 652c 2031 292c 0a20  ame, zone, 1),. 
+00022e20: 2020 2020 2020 2020 2020 205f 5345 5256             _SERV
+00022e30: 455f 5741 4954 5f55 4e54 494c 5f52 4541  E_WAIT_UNTIL_REA
+00022e40: 4459 2e66 6f72 6d61 7428 6e61 6d65 3d6e  DY.format(name=n
+00022e50: 616d 652c 2072 6570 6c69 6361 5f6e 756d  ame, replica_num
+00022e60: 3d31 292c 0a20 2020 2020 2020 2020 2020  =1),.           
+00022e70: 2066 277b 5f53 4552 5645 5f45 4e44 504f   f'{_SERVE_ENDPO
+00022e80: 494e 545f 5741 4954 2e66 6f72 6d61 7428  INT_WAIT.format(
+00022e90: 6e61 6d65 3d6e 616d 6529 7d3b 2027 0a20  name=name)}; '. 
+00022ea0: 2020 2020 2020 2020 2020 2027 7265 7175             'requ
+00022eb0: 6573 745f 6f75 7470 7574 3d24 2863 7572  est_output=$(cur
+00022ec0: 6c20 6874 7470 3a2f 2f24 656e 6470 6f69  l http://$endpoi
+00022ed0: 6e74 293b 2065 6368 6f20 2224 7265 7175  nt); echo "$requ
+00022ee0: 6573 745f 6f75 7470 7574 223b 2065 6368  est_output"; ech
+00022ef0: 6f20 2224 7265 7175 6573 745f 6f75 7470  o "$request_outp
+00022f00: 7574 2220 7c20 6772 6570 2022 4869 2c20  ut" | grep "Hi, 
+00022f10: 536b 7950 696c 6f74 2068 6572 6522 272c  SkyPilot here"',
+00022f20: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+00022f30: 2020 2020 5f54 4541 5244 4f57 4e5f 5345      _TEARDOWN_SE
+00022f40: 5256 4943 452e 666f 726d 6174 286e 616d  RVICE.format(nam
+00022f50: 653d 6e61 6d65 292c 0a20 2020 2020 2020  e=name),.       
+00022f60: 2074 696d 656f 7574 3d32 3020 2a20 3630   timeout=20 * 60
+00022f70: 2c0a 2020 2020 290a 2020 2020 7275 6e5f  ,.    ).    run_
+00022f80: 6f6e 655f 7465 7374 2874 6573 7429 0a0a  one_test(test)..
+00022f90: 0a40 7079 7465 7374 2e6d 6172 6b2e 7365  .@pytest.mark.se
+00022fa0: 7276 650a 4070 7974 6573 742e 6d61 726b  rve.@pytest.mark
+00022fb0: 2e6e 6f5f 6b75 6265 726e 6574 6573 0a64  .no_kubernetes.d
+00022fc0: 6566 2074 6573 745f 736b 7973 6572 7665  ef test_skyserve
+00022fd0: 5f62 6173 655f 6f6e 6465 6d61 6e64 5f66  _base_ondemand_f
+00022fe0: 616c 6c62 6163 6b28 6765 6e65 7269 635f  allback(generic_
+00022ff0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
+00023000: 206e 616d 6520 3d20 5f67 6574 5f73 6572   name = _get_ser
+00023010: 7669 6365 5f6e 616d 6528 290a 2020 2020  vice_name().    
+00023020: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+00023030: 2020 2020 2066 2774 6573 742d 736b 7973       f'test-skys
+00023040: 6572 7665 2d62 6173 652d 6f6e 6465 6d61  erve-base-ondema
+00023050: 6e64 2d66 616c 6c62 6163 6b27 2c0a 2020  nd-fallback',.  
+00023060: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00023070: 2020 2020 6627 736b 7920 7365 7276 6520      f'sky serve 
+00023080: 7570 202d 6e20 7b6e 616d 657d 202d 2d63  up -n {name} --c
+00023090: 6c6f 7564 207b 6765 6e65 7269 635f 636c  loud {generic_cl
+000230a0: 6f75 647d 202d 7920 7465 7374 732f 736b  oud} -y tests/sk
+000230b0: 7973 6572 7665 2f73 706f 742f 6261 7365  yserve/spot/base
+000230c0: 5f6f 6e64 656d 616e 645f 6661 6c6c 6261  _ondemand_fallba
+000230d0: 636b 2e79 616d 6c27 2c0a 2020 2020 2020  ck.yaml',.      
+000230e0: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
+000230f0: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
+00023100: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
+00023110: 7265 706c 6963 615f 6e75 6d3d 3229 2c0a  replica_num=2),.
+00023120: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
+00023130: 636b 5f72 6570 6c69 6361 5f69 6e5f 7374  ck_replica_in_st
+00023140: 6174 7573 286e 616d 652c 205b 2831 2c20  atus(name, [(1, 
+00023150: 5472 7565 2c20 2752 4541 4459 2729 2c0a  True, 'READY'),.
+00023160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023190: 2020 2020 2028 312c 2046 616c 7365 2c20       (1, False, 
-000231a0: 2752 4541 4459 2729 5d29 2c0a 2020 2020  'READY')]),.    
-000231b0: 2020 2020 5d2c 0a20 2020 2020 2020 205f      ],.        _
-000231c0: 5445 4152 444f 574e 5f53 4552 5649 4345  TEARDOWN_SERVICE
-000231d0: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
-000231e0: 6529 2c0a 2020 2020 2020 2020 7469 6d65  e),.        time
-000231f0: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
-00023200: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
-00023210: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
-00023220: 6573 742e 6d61 726b 2e67 6370 0a40 7079  est.mark.gcp.@py
-00023230: 7465 7374 2e6d 6172 6b2e 7365 7276 650a  test.mark.serve.
-00023240: 6465 6620 7465 7374 5f73 6b79 7365 7276  def test_skyserv
-00023250: 655f 6479 6e61 6d69 635f 6f6e 6465 6d61  e_dynamic_ondema
-00023260: 6e64 5f66 616c 6c62 6163 6b28 293a 0a20  nd_fallback():. 
-00023270: 2020 206e 616d 6520 3d20 5f67 6574 5f73     name = _get_s
-00023280: 6572 7669 6365 5f6e 616d 6528 290a 2020  ervice_name().  
-00023290: 2020 7a6f 6e65 203d 2027 7573 2d63 656e    zone = 'us-cen
-000232a0: 7472 616c 312d 6127 0a0a 2020 2020 7465  tral1-a'..    te
-000232b0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-000232c0: 2020 2066 2774 6573 742d 736b 7973 6572     f'test-skyser
-000232d0: 7665 2d64 796e 616d 6963 2d6f 6e64 656d  ve-dynamic-ondem
-000232e0: 616e 642d 6661 6c6c 6261 636b 272c 0a20  and-fallback',. 
-000232f0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00023300: 2020 2020 2066 2773 6b79 2073 6572 7665       f'sky serve
-00023310: 2075 7020 2d6e 207b 6e61 6d65 7d20 2d2d   up -n {name} --
-00023320: 636c 6f75 6420 6763 7020 2d79 2074 6573  cloud gcp -y tes
-00023330: 7473 2f73 6b79 7365 7276 652f 7370 6f74  ts/skyserve/spot
-00023340: 2f64 796e 616d 6963 5f6f 6e64 656d 616e  /dynamic_ondeman
-00023350: 645f 6661 6c6c 6261 636b 2e79 616d 6c27  d_fallback.yaml'
-00023360: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00023370: 736c 6565 7020 3430 272c 0a20 2020 2020  sleep 40',.     
-00023380: 2020 2020 2020 2023 2032 206f 6e2d 6465         # 2 on-de
-00023390: 6d61 6e64 2028 7072 6f76 6973 696f 6e69  mand (provisioni
-000233a0: 6e67 2920 2b20 3220 5370 6f74 2028 7072  ng) + 2 Spot (pr
-000233b0: 6f76 6973 696f 6e69 6e67 292e 0a20 2020  ovisioning)..   
-000233c0: 2020 2020 2020 2020 2066 277b 5f53 4552           f'{_SER
-000233d0: 5645 5f53 5441 5455 535f 5741 4954 2e66  VE_STATUS_WAIT.f
-000233e0: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
-000233f0: 7d3b 2065 6368 6f20 2224 7322 3b27 0a20  }; echo "$s";'. 
-00023400: 2020 2020 2020 2020 2020 2027 6563 686f             'echo
-00023410: 2022 2473 2220 7c20 6772 6570 202d 7120   "$s" | grep -q 
-00023420: 2230 2f34 2220 7c7c 2065 7869 7420 3127  "0/4" || exit 1'
-00023430: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00023440: 5761 6974 2066 6f72 2074 6865 2070 726f  Wait for the pro
-00023450: 7669 7369 6f6e 696e 6720 7374 6172 7473  visioning starts
-00023460: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-00023470: 6c65 6570 2034 3027 2c0a 2020 2020 2020  leep 40',.      
-00023480: 2020 2020 2020 5f63 6865 636b 5f72 6570        _check_rep
-00023490: 6c69 6361 5f69 6e5f 7374 6174 7573 286e  lica_in_status(n
-000234a0: 616d 652c 205b 0a20 2020 2020 2020 2020  ame, [.         
-000234b0: 2020 2020 2020 2028 322c 2054 7275 652c         (2, True,
-000234c0: 205f 5345 5256 4943 455f 4c41 554e 4348   _SERVICE_LAUNCH
-000234d0: 494e 475f 5354 4154 5553 5f52 4547 4558  ING_STATUS_REGEX
-000234e0: 202b 2027 5c7c 5245 4144 5927 292c 0a20   + '\|READY'),. 
-000234f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00023500: 322c 2046 616c 7365 2c20 5f53 4552 5649  2, False, _SERVI
-00023510: 4345 5f4c 4155 4e43 4849 4e47 5f53 5441  CE_LAUNCHING_STA
-00023520: 5455 535f 5245 4745 5820 2b20 275c 7c53  TUS_REGEX + '\|S
-00023530: 4855 5454 494e 475f 444f 574e 2729 0a20  HUTTING_DOWN'). 
-00023540: 2020 2020 2020 2020 2020 205d 292c 0a0a             ]),..
-00023550: 2020 2020 2020 2020 2020 2020 2320 5761              # Wa
-00023560: 6974 2075 6e74 696c 2032 2073 706f 7420  it until 2 spot 
-00023570: 696e 7374 616e 6365 7320 6172 6520 7265  instances are re
-00023580: 6164 792e 0a20 2020 2020 2020 2020 2020  ady..           
-00023590: 205f 5345 5256 455f 5741 4954 5f55 4e54   _SERVE_WAIT_UNT
-000235a0: 494c 5f52 4541 4459 2e66 6f72 6d61 7428  IL_READY.format(
-000235b0: 6e61 6d65 3d6e 616d 652c 2072 6570 6c69  name=name, repli
-000235c0: 6361 5f6e 756d 3d32 292c 0a20 2020 2020  ca_num=2),.     
-000235d0: 2020 2020 2020 205f 6368 6563 6b5f 7265         _check_re
-000235e0: 706c 6963 615f 696e 5f73 7461 7475 7328  plica_in_status(
-000235f0: 6e61 6d65 2c20 5b28 322c 2054 7275 652c  name, [(2, True,
-00023600: 2027 5245 4144 5927 292c 0a20 2020 2020   'READY'),.     
+00023180: 2020 2020 2020 2020 2020 2020 2831 2c20              (1, 
+00023190: 4661 6c73 652c 2027 5245 4144 5927 295d  False, 'READY')]
+000231a0: 292c 0a20 2020 2020 2020 205d 2c0a 2020  ),.        ],.  
+000231b0: 2020 2020 2020 5f54 4541 5244 4f57 4e5f        _TEARDOWN_
+000231c0: 5345 5256 4943 452e 666f 726d 6174 286e  SERVICE.format(n
+000231d0: 616d 653d 6e61 6d65 292c 0a20 2020 2020  ame=name),.     
+000231e0: 2020 2074 696d 656f 7574 3d32 3020 2a20     timeout=20 * 
+000231f0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00023200: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00023210: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00023220: 6763 700a 4070 7974 6573 742e 6d61 726b  gcp.@pytest.mark
+00023230: 2e73 6572 7665 0a64 6566 2074 6573 745f  .serve.def test_
+00023240: 736b 7973 6572 7665 5f64 796e 616d 6963  skyserve_dynamic
+00023250: 5f6f 6e64 656d 616e 645f 6661 6c6c 6261  _ondemand_fallba
+00023260: 636b 2829 3a0a 2020 2020 6e61 6d65 203d  ck():.    name =
+00023270: 205f 6765 745f 7365 7276 6963 655f 6e61   _get_service_na
+00023280: 6d65 2829 0a20 2020 207a 6f6e 6520 3d20  me().    zone = 
+00023290: 2775 732d 6365 6e74 7261 6c31 2d61 270a  'us-central1-a'.
+000232a0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+000232b0: 280a 2020 2020 2020 2020 6627 7465 7374  (.        f'test
+000232c0: 2d73 6b79 7365 7276 652d 6479 6e61 6d69  -skyserve-dynami
+000232d0: 632d 6f6e 6465 6d61 6e64 2d66 616c 6c62  c-ondemand-fallb
+000232e0: 6163 6b27 2c0a 2020 2020 2020 2020 5b0a  ack',.        [.
+000232f0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00023300: 7920 7365 7276 6520 7570 202d 6e20 7b6e  y serve up -n {n
+00023310: 616d 657d 202d 2d63 6c6f 7564 2067 6370  ame} --cloud gcp
+00023320: 202d 7920 7465 7374 732f 736b 7973 6572   -y tests/skyser
+00023330: 7665 2f73 706f 742f 6479 6e61 6d69 635f  ve/spot/dynamic_
+00023340: 6f6e 6465 6d61 6e64 5f66 616c 6c62 6163  ondemand_fallbac
+00023350: 6b2e 7961 6d6c 272c 0a20 2020 2020 2020  k.yaml',.       
+00023360: 2020 2020 2066 2773 6c65 6570 2034 3027       f'sleep 40'
+00023370: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00023380: 3220 6f6e 2d64 656d 616e 6420 2870 726f  2 on-demand (pro
+00023390: 7669 7369 6f6e 696e 6729 202b 2032 2053  visioning) + 2 S
+000233a0: 706f 7420 2870 726f 7669 7369 6f6e 696e  pot (provisionin
+000233b0: 6729 2e0a 2020 2020 2020 2020 2020 2020  g)..            
+000233c0: 6627 7b5f 5345 5256 455f 5354 4154 5553  f'{_SERVE_STATUS
+000233d0: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
+000233e0: 653d 6e61 6d65 297d 3b20 6563 686f 2022  e=name)}; echo "
+000233f0: 2473 223b 270a 2020 2020 2020 2020 2020  $s";'.          
+00023400: 2020 2765 6368 6f20 2224 7322 207c 2067    'echo "$s" | g
+00023410: 7265 7020 2d71 2022 302f 3422 207c 7c20  rep -q "0/4" || 
+00023420: 6578 6974 2031 272c 0a20 2020 2020 2020  exit 1',.       
+00023430: 2020 2020 2023 2057 6169 7420 666f 7220       # Wait for 
+00023440: 7468 6520 7072 6f76 6973 696f 6e69 6e67  the provisioning
+00023450: 2073 7461 7274 730a 2020 2020 2020 2020   starts.        
+00023460: 2020 2020 6627 736c 6565 7020 3430 272c      f'sleep 40',
+00023470: 0a20 2020 2020 2020 2020 2020 205f 6368  .            _ch
+00023480: 6563 6b5f 7265 706c 6963 615f 696e 5f73  eck_replica_in_s
+00023490: 7461 7475 7328 6e61 6d65 2c20 5b0a 2020  tatus(name, [.  
+000234a0: 2020 2020 2020 2020 2020 2020 2020 2832                (2
+000234b0: 2c20 5472 7565 2c20 5f53 4552 5649 4345  , True, _SERVICE
+000234c0: 5f4c 4155 4e43 4849 4e47 5f53 5441 5455  _LAUNCHING_STATU
+000234d0: 535f 5245 4745 5820 2b20 275c 7c52 4541  S_REGEX + '\|REA
+000234e0: 4459 2729 2c0a 2020 2020 2020 2020 2020  DY'),.          
+000234f0: 2020 2020 2020 2832 2c20 4661 6c73 652c        (2, False,
+00023500: 205f 5345 5256 4943 455f 4c41 554e 4348   _SERVICE_LAUNCH
+00023510: 494e 475f 5354 4154 5553 5f52 4547 4558  ING_STATUS_REGEX
+00023520: 202b 2027 5c7c 5348 5554 5449 4e47 5f44   + '\|SHUTTING_D
+00023530: 4f57 4e27 290a 2020 2020 2020 2020 2020  OWN').          
+00023540: 2020 5d29 2c0a 0a20 2020 2020 2020 2020    ]),..         
+00023550: 2020 2023 2057 6169 7420 756e 7469 6c20     # Wait until 
+00023560: 3220 7370 6f74 2069 6e73 7461 6e63 6573  2 spot instances
+00023570: 2061 7265 2072 6561 6479 2e0a 2020 2020   are ready..    
+00023580: 2020 2020 2020 2020 5f53 4552 5645 5f57          _SERVE_W
+00023590: 4149 545f 554e 5449 4c5f 5245 4144 592e  AIT_UNTIL_READY.
+000235a0: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
+000235b0: 2c20 7265 706c 6963 615f 6e75 6d3d 3229  , replica_num=2)
+000235c0: 2c0a 2020 2020 2020 2020 2020 2020 5f63  ,.            _c
+000235d0: 6865 636b 5f72 6570 6c69 6361 5f69 6e5f  heck_replica_in_
+000235e0: 7374 6174 7573 286e 616d 652c 205b 2832  status(name, [(2
+000235f0: 2c20 5472 7565 2c20 2752 4541 4459 2729  , True, 'READY')
+00023600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00023610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023630: 2020 2020 2020 2028 302c 2046 616c 7365         (0, False
-00023640: 2c20 2727 295d 292c 0a20 2020 2020 2020  , '')]),.       
-00023650: 2020 2020 205f 7465 726d 696e 6174 655f       _terminate_
-00023660: 6763 705f 7265 706c 6963 6128 6e61 6d65  gcp_replica(name
-00023670: 2c20 7a6f 6e65 2c20 3129 2c0a 2020 2020  , zone, 1),.    
-00023680: 2020 2020 2020 2020 6627 736c 6565 7020          f'sleep 
-00023690: 3430 272c 0a20 2020 2020 2020 2020 2020  40',.           
-000236a0: 2023 2031 206f 6e2d 6465 6d61 6e64 2028   # 1 on-demand (
-000236b0: 7072 6f76 6973 696f 6e69 6e67 2920 2b20  provisioning) + 
-000236c0: 3120 5370 6f74 2028 7265 6164 7929 202b  1 Spot (ready) +
-000236d0: 2031 2073 706f 7420 2870 726f 7669 7369   1 spot (provisi
-000236e0: 6f6e 696e 6729 2e0a 2020 2020 2020 2020  oning)..        
-000236f0: 2020 2020 6627 7b5f 5345 5256 455f 5354      f'{_SERVE_ST
-00023700: 4154 5553 5f57 4149 542e 666f 726d 6174  ATUS_WAIT.format
-00023710: 286e 616d 653d 6e61 6d65 297d 3b20 270a  (name=name)}; '.
-00023720: 2020 2020 2020 2020 2020 2020 2765 6368              'ech
-00023730: 6f20 2224 7322 207c 2067 7265 7020 2d71  o "$s" | grep -q
-00023740: 2022 312f 3322 272c 0a20 2020 2020 2020   "1/3"',.       
-00023750: 2020 2020 205f 6368 6563 6b5f 7265 706c       _check_repl
-00023760: 6963 615f 696e 5f73 7461 7475 7328 0a20  ica_in_status(. 
-00023770: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00023780: 616d 652c 205b 2831 2c20 5472 7565 2c20  ame, [(1, True, 
-00023790: 2752 4541 4459 2729 2c0a 2020 2020 2020  'READY'),.      
-000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237b0: 2028 312c 2054 7275 652c 205f 5345 5256   (1, True, _SERV
-000237c0: 4943 455f 4c41 554e 4348 494e 475f 5354  ICE_LAUNCHING_ST
-000237d0: 4154 5553 5f52 4547 4558 292c 0a20 2020  ATUS_REGEX),.   
-000237e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237f0: 2020 2020 2831 2c20 4661 6c73 652c 205f      (1, False, _
-00023800: 5345 5256 4943 455f 4c41 554e 4348 494e  SERVICE_LAUNCHIN
-00023810: 475f 5354 4154 5553 5f52 4547 4558 295d  G_STATUS_REGEX)]
-00023820: 292c 0a0a 2020 2020 2020 2020 2020 2020  ),..            
-00023830: 2320 5761 6974 2075 6e74 696c 2032 2073  # Wait until 2 s
-00023840: 706f 7420 696e 7374 616e 6365 7320 6172  pot instances ar
-00023850: 6520 7265 6164 792e 0a20 2020 2020 2020  e ready..       
-00023860: 2020 2020 205f 5345 5256 455f 5741 4954       _SERVE_WAIT
-00023870: 5f55 4e54 494c 5f52 4541 4459 2e66 6f72  _UNTIL_READY.for
-00023880: 6d61 7428 6e61 6d65 3d6e 616d 652c 2072  mat(name=name, r
-00023890: 6570 6c69 6361 5f6e 756d 3d32 292c 0a20  eplica_num=2),. 
-000238a0: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
-000238b0: 6b5f 7265 706c 6963 615f 696e 5f73 7461  k_replica_in_sta
-000238c0: 7475 7328 6e61 6d65 2c20 5b28 322c 2054  tus(name, [(2, T
-000238d0: 7275 652c 2027 5245 4144 5927 292c 0a20  rue, 'READY'),. 
+00023620: 2020 2020 2020 2020 2020 2020 2020 2830                (0
+00023630: 2c20 4661 6c73 652c 2027 2729 5d29 2c0a  , False, '')]),.
+00023640: 2020 2020 2020 2020 2020 2020 5f74 6572              _ter
+00023650: 6d69 6e61 7465 5f67 6370 5f72 6570 6c69  minate_gcp_repli
+00023660: 6361 286e 616d 652c 207a 6f6e 652c 2031  ca(name, zone, 1
+00023670: 292c 0a20 2020 2020 2020 2020 2020 2066  ),.            f
+00023680: 2773 6c65 6570 2034 3027 2c0a 2020 2020  'sleep 40',.    
+00023690: 2020 2020 2020 2020 2320 3120 6f6e 2d64          # 1 on-d
+000236a0: 656d 616e 6420 2870 726f 7669 7369 6f6e  emand (provision
+000236b0: 696e 6729 202b 2031 2053 706f 7420 2872  ing) + 1 Spot (r
+000236c0: 6561 6479 2920 2b20 3120 7370 6f74 2028  eady) + 1 spot (
+000236d0: 7072 6f76 6973 696f 6e69 6e67 292e 0a20  provisioning).. 
+000236e0: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+000236f0: 4552 5645 5f53 5441 5455 535f 5741 4954  ERVE_STATUS_WAIT
+00023700: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
+00023710: 6529 7d3b 2027 0a20 2020 2020 2020 2020  e)}; '.         
+00023720: 2020 2027 6563 686f 2022 2473 2220 7c20     'echo "$s" | 
+00023730: 6772 6570 202d 7120 2231 2f33 2227 2c0a  grep -q "1/3"',.
+00023740: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
+00023750: 636b 5f72 6570 6c69 6361 5f69 6e5f 7374  ck_replica_in_st
+00023760: 6174 7573 280a 2020 2020 2020 2020 2020  atus(.          
+00023770: 2020 2020 2020 6e61 6d65 2c20 5b28 312c        name, [(1,
+00023780: 2054 7275 652c 2027 5245 4144 5927 292c   True, 'READY'),
+00023790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000237a0: 2020 2020 2020 2020 2831 2c20 5472 7565          (1, True
+000237b0: 2c20 5f53 4552 5649 4345 5f4c 4155 4e43  , _SERVICE_LAUNC
+000237c0: 4849 4e47 5f53 5441 5455 535f 5245 4745  HING_STATUS_REGE
+000237d0: 5829 2c0a 2020 2020 2020 2020 2020 2020  X),.            
+000237e0: 2020 2020 2020 2020 2020 2028 312c 2046             (1, F
+000237f0: 616c 7365 2c20 5f53 4552 5649 4345 5f4c  alse, _SERVICE_L
+00023800: 4155 4e43 4849 4e47 5f53 5441 5455 535f  AUNCHING_STATUS_
+00023810: 5245 4745 5829 5d29 2c0a 0a20 2020 2020  REGEX)]),..     
+00023820: 2020 2020 2020 2023 2057 6169 7420 756e         # Wait un
+00023830: 7469 6c20 3220 7370 6f74 2069 6e73 7461  til 2 spot insta
+00023840: 6e63 6573 2061 7265 2072 6561 6479 2e0a  nces are ready..
+00023850: 2020 2020 2020 2020 2020 2020 5f53 4552              _SER
+00023860: 5645 5f57 4149 545f 554e 5449 4c5f 5245  VE_WAIT_UNTIL_RE
+00023870: 4144 592e 666f 726d 6174 286e 616d 653d  ADY.format(name=
+00023880: 6e61 6d65 2c20 7265 706c 6963 615f 6e75  name, replica_nu
+00023890: 6d3d 3229 2c0a 2020 2020 2020 2020 2020  m=2),.          
+000238a0: 2020 5f63 6865 636b 5f72 6570 6c69 6361    _check_replica
+000238b0: 5f69 6e5f 7374 6174 7573 286e 616d 652c  _in_status(name,
+000238c0: 205b 2832 2c20 5472 7565 2c20 2752 4541   [(2, True, 'REA
+000238d0: 4459 2729 2c0a 2020 2020 2020 2020 2020  DY'),.          
 000238e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000238f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023900: 2020 2020 2020 2020 2020 2028 302c 2046             (0, F
-00023910: 616c 7365 2c20 2727 295d 292c 0a20 2020  alse, '')]),.   
-00023920: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00023930: 5f54 4541 5244 4f57 4e5f 5345 5256 4943  _TEARDOWN_SERVIC
-00023940: 452e 666f 726d 6174 286e 616d 653d 6e61  E.format(name=na
-00023950: 6d65 292c 0a20 2020 2020 2020 2074 696d  me),.        tim
-00023960: 656f 7574 3d32 3020 2a20 3630 2c0a 2020  eout=20 * 60,.  
-00023970: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-00023980: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00023990: 7465 7374 2e6d 6172 6b2e 7365 7276 650a  test.mark.serve.
-000239a0: 6465 6620 7465 7374 5f73 6b79 7365 7276  def test_skyserv
-000239b0: 655f 7573 6572 5f62 7567 5f72 6573 7461  e_user_bug_resta
-000239c0: 7274 2867 656e 6572 6963 5f63 6c6f 7564  rt(generic_cloud
-000239d0: 3a20 7374 7229 3a0a 2020 2020 2222 2254  : str):.    """T
-000239e0: 6573 7473 2074 6861 7420 7765 2072 6573  ests that we res
-000239f0: 7461 7274 2074 6865 2073 6572 7669 6365  tart the service
-00023a00: 2061 6674 6572 2075 7365 7220 6275 672e   after user bug.
-00023a10: 2222 220a 2020 2020 2320 544f 444f 287a  """.    # TODO(z
-00023a20: 6877 7529 3a20 7468 6973 2062 6568 6176  hwu): this behav
-00023a30: 696f 7220 6e65 6564 7320 736f 6d65 2072  ior needs some r
-00023a40: 6574 6869 6e6b 696e 672e 0a20 2020 206e  ethinking..    n
-00023a50: 616d 6520 3d20 5f67 6574 5f73 6572 7669  ame = _get_servi
-00023a60: 6365 5f6e 616d 6528 290a 2020 2020 7465  ce_name().    te
-00023a70: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00023a80: 2020 2066 2774 6573 742d 736b 7973 6572     f'test-skyser
-00023a90: 7665 2d75 7365 722d 6275 672d 7265 7374  ve-user-bug-rest
-00023aa0: 6172 7427 2c0a 2020 2020 2020 2020 5b0a  art',.        [.
-00023ab0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00023ac0: 7920 7365 7276 6520 7570 202d 6e20 7b6e  y serve up -n {n
-00023ad0: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
-00023ae0: 6e65 7269 635f 636c 6f75 647d 202d 7920  neric_cloud} -y 
-00023af0: 7465 7374 732f 736b 7973 6572 7665 2f72  tests/skyserve/r
-00023b00: 6573 7461 7274 2f75 7365 725f 6275 672e  estart/user_bug.
-00023b10: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00023b20: 2020 2066 2773 3d24 2873 6b79 2073 6572     f's=$(sky ser
-00023b30: 7665 2073 7461 7475 7320 7b6e 616d 657d  ve status {name}
-00023b40: 293b 2065 6368 6f20 2224 7322 3b27 0a20  ); echo "$s";'. 
-00023b50: 2020 2020 2020 2020 2020 2027 756e 7469             'unti
-00023b60: 6c20 6563 686f 2022 2473 2220 7c20 6772  l echo "$s" | gr
-00023b70: 6570 202d 4120 3130 3020 2253 6572 7669  ep -A 100 "Servi
-00023b80: 6365 2052 6570 6c69 6361 7322 207c 2067  ce Replicas" | g
-00023b90: 7265 7020 2253 4855 5454 494e 475f 444f  rep "SHUTTING_DO
-00023ba0: 574e 223b 2027 0a20 2020 2020 2020 2020  WN"; '.         
-00023bb0: 2020 2027 646f 2065 6368 6f20 2257 6169     'do echo "Wai
-00023bc0: 7469 6e67 2066 6f72 2066 6972 7374 2073  ting for first s
-00023bd0: 6572 7669 6365 2074 6f20 6265 2053 4855  ervice to be SHU
-00023be0: 5454 494e 4720 444f 574e 2e2e 2e22 3b20  TTING DOWN..."; 
-00023bf0: 270a 2020 2020 2020 2020 2020 2020 6627  '.            f'
-00023c00: 736c 6565 7020 353b 2073 3d24 2873 6b79  sleep 5; s=$(sky
-00023c10: 2073 6572 7665 2073 7461 7475 7320 7b6e   serve status {n
-00023c20: 616d 657d 293b 2065 6368 6f20 2224 7322  ame}); echo "$s"
-00023c30: 3b20 646f 6e65 3b20 272c 0a20 2020 2020  ; done; ',.     
-00023c40: 2020 2020 2020 2066 2773 3d24 2873 6b79         f's=$(sky
-00023c50: 2073 6572 7665 2073 7461 7475 7320 7b6e   serve status {n
-00023c60: 616d 657d 293b 2065 6368 6f20 2224 7322  ame}); echo "$s"
-00023c70: 3b27 0a20 2020 2020 2020 2020 2020 2027  ;'.            '
-00023c80: 756e 7469 6c20 6563 686f 2022 2473 2220  until echo "$s" 
-00023c90: 7c20 6772 6570 202d 4120 3130 3020 2253  | grep -A 100 "S
-00023ca0: 6572 7669 6365 2052 6570 6c69 6361 7322  ervice Replicas"
-00023cb0: 207c 2067 7265 7020 2246 4149 4c45 4422   | grep "FAILED"
-00023cc0: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
-00023cd0: 2764 6f20 6563 686f 2022 5761 6974 696e  'do echo "Waitin
-00023ce0: 6720 666f 7220 6669 7273 7420 7365 7276  g for first serv
-00023cf0: 6963 6520 746f 2062 6520 4641 494c 4544  ice to be FAILED
-00023d00: 2e2e 2e22 3b20 270a 2020 2020 2020 2020  ..."; '.        
-00023d10: 2020 2020 6627 736c 6565 7020 353b 2073      f'sleep 5; s
-00023d20: 3d24 2873 6b79 2073 6572 7665 2073 7461  =$(sky serve sta
-00023d30: 7475 7320 7b6e 616d 657d 293b 2065 6368  tus {name}); ech
-00023d40: 6f20 2224 7322 3b20 646f 6e65 3b20 6563  o "$s"; done; ec
-00023d50: 686f 2022 2473 223b 2027 0a20 2020 2020  ho "$s"; '.     
-00023d60: 2020 2020 2020 202b 205f 6368 6563 6b5f         + _check_
-00023d70: 7265 706c 6963 615f 696e 5f73 7461 7475  replica_in_statu
-00023d80: 7328 6e61 6d65 2c20 5b28 312c 2054 7275  s(name, [(1, Tru
-00023d90: 652c 2027 4641 494c 4544 2729 5d29 202b  e, 'FAILED')]) +
-00023da0: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
-00023db0: 7365 7220 6275 6720 6661 696c 7572 6520  ser bug failure 
-00023dc0: 7769 6c6c 2063 6175 7365 206e 6f20 6675  will cause no fu
-00023dd0: 7274 6865 7220 7363 616c 696e 672e 0a20  rther scaling.. 
-00023de0: 2020 2020 2020 2020 2020 2066 2765 6368             f'ech
-00023df0: 6f20 2224 7322 207c 2067 7265 7020 2d41  o "$s" | grep -A
-00023e00: 2031 3030 2022 5365 7276 6963 6520 5265   100 "Service Re
-00023e10: 706c 6963 6173 2220 7c20 6772 6570 2022  plicas" | grep "
-00023e20: 7b6e 616d 657d 2220 7c20 7763 202d 6c20  {name}" | wc -l 
-00023e30: 7c20 6772 6570 2031 3b20 270a 2020 2020  | grep 1; '.    
-00023e40: 2020 2020 2020 2020 6627 6563 686f 2022          f'echo "
-00023e50: 2473 2220 7c20 6772 6570 202d 4220 3130  $s" | grep -B 10
-00023e60: 3020 224e 4f5f 5245 504c 4943 4122 207c  0 "NO_REPLICA" |
-00023e70: 2067 7265 7020 2230 2f30 2227 2c0a 2020   grep "0/0"',.  
-00023e80: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00023e90: 7365 7276 6520 7570 6461 7465 207b 6e61  serve update {na
-00023ea0: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
-00023eb0: 6572 6963 5f63 6c6f 7564 7d20 2d79 2074  eric_cloud} -y t
-00023ec0: 6573 7473 2f73 6b79 7365 7276 652f 6175  ests/skyserve/au
-00023ed0: 746f 5f72 6573 7461 7274 2e79 616d 6c27  to_restart.yaml'
-00023ee0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00023ef0: 7b5f 5345 5256 455f 454e 4450 4f49 4e54  {_SERVE_ENDPOINT
-00023f00: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
-00023f10: 653d 6e61 6d65 297d 3b20 270a 2020 2020  e=name)}; '.    
-00023f20: 2020 2020 2020 2020 2775 6e74 696c 2063          'until c
-00023f30: 7572 6c20 2d4c 2068 7474 703a 2f2f 2465  url -L http://$e
-00023f40: 6e64 706f 696e 7420 7c20 6772 6570 2022  ndpoint | grep "
-00023f50: 4869 2c20 536b 7950 696c 6f74 2068 6572  Hi, SkyPilot her
-00023f60: 6521 223b 2064 6f20 736c 6565 7020 323b  e!"; do sleep 2;
-00023f70: 2064 6f6e 653b 2073 6c65 6570 2032 3b20   done; sleep 2; 
-00023f80: 270a 2020 2020 2020 2020 2020 2020 2b20  '.            + 
-00023f90: 5f63 6865 636b 5f72 6570 6c69 6361 5f69  _check_replica_i
-00023fa0: 6e5f 7374 6174 7573 286e 616d 652c 205b  n_status(name, [
-00023fb0: 2831 2c20 4661 6c73 652c 2027 5245 4144  (1, False, 'READ
-00023fc0: 5927 292c 0a20 2020 2020 2020 2020 2020  Y'),.           
+00023900: 2020 2830 2c20 4661 6c73 652c 2027 2729    (0, False, '')
+00023910: 5d29 2c0a 2020 2020 2020 2020 5d2c 0a20  ]),.        ],. 
+00023920: 2020 2020 2020 205f 5445 4152 444f 574e         _TEARDOWN
+00023930: 5f53 4552 5649 4345 2e66 6f72 6d61 7428  _SERVICE.format(
+00023940: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
+00023950: 2020 2020 7469 6d65 6f75 743d 3230 202a      timeout=20 *
+00023960: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
+00023970: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
+00023980: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
+00023990: 2e73 6572 7665 0a64 6566 2074 6573 745f  .serve.def test_
+000239a0: 736b 7973 6572 7665 5f75 7365 725f 6275  skyserve_user_bu
+000239b0: 675f 7265 7374 6172 7428 6765 6e65 7269  g_restart(generi
+000239c0: 635f 636c 6f75 643a 2073 7472 293a 0a20  c_cloud: str):. 
+000239d0: 2020 2022 2222 5465 7374 7320 7468 6174     """Tests that
+000239e0: 2077 6520 7265 7374 6172 7420 7468 6520   we restart the 
+000239f0: 7365 7276 6963 6520 6166 7465 7220 7573  service after us
+00023a00: 6572 2062 7567 2e22 2222 0a20 2020 2023  er bug.""".    #
+00023a10: 2054 4f44 4f28 7a68 7775 293a 2074 6869   TODO(zhwu): thi
+00023a20: 7320 6265 6861 7669 6f72 206e 6565 6473  s behavior needs
+00023a30: 2073 6f6d 6520 7265 7468 696e 6b69 6e67   some rethinking
+00023a40: 2e0a 2020 2020 6e61 6d65 203d 205f 6765  ..    name = _ge
+00023a50: 745f 7365 7276 6963 655f 6e61 6d65 2829  t_service_name()
+00023a60: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+00023a70: 280a 2020 2020 2020 2020 6627 7465 7374  (.        f'test
+00023a80: 2d73 6b79 7365 7276 652d 7573 6572 2d62  -skyserve-user-b
+00023a90: 7567 2d72 6573 7461 7274 272c 0a20 2020  ug-restart',.   
+00023aa0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00023ab0: 2020 2066 2773 6b79 2073 6572 7665 2075     f'sky serve u
+00023ac0: 7020 2d6e 207b 6e61 6d65 7d20 2d2d 636c  p -n {name} --cl
+00023ad0: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
+00023ae0: 7564 7d20 2d79 2074 6573 7473 2f73 6b79  ud} -y tests/sky
+00023af0: 7365 7276 652f 7265 7374 6172 742f 7573  serve/restart/us
+00023b00: 6572 5f62 7567 2e79 616d 6c27 2c0a 2020  er_bug.yaml',.  
+00023b10: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
+00023b20: 736b 7920 7365 7276 6520 7374 6174 7573  sky serve status
+00023b30: 207b 6e61 6d65 7d29 3b20 6563 686f 2022   {name}); echo "
+00023b40: 2473 223b 270a 2020 2020 2020 2020 2020  $s";'.          
+00023b50: 2020 2775 6e74 696c 2065 6368 6f20 2224    'until echo "$
+00023b60: 7322 207c 2067 7265 7020 2d41 2031 3030  s" | grep -A 100
+00023b70: 2022 5365 7276 6963 6520 5265 706c 6963   "Service Replic
+00023b80: 6173 2220 7c20 6772 6570 2022 5348 5554  as" | grep "SHUT
+00023b90: 5449 4e47 5f44 4f57 4e22 3b20 270a 2020  TING_DOWN"; '.  
+00023ba0: 2020 2020 2020 2020 2020 2764 6f20 6563            'do ec
+00023bb0: 686f 2022 5761 6974 696e 6720 666f 7220  ho "Waiting for 
+00023bc0: 6669 7273 7420 7365 7276 6963 6520 746f  first service to
+00023bd0: 2062 6520 5348 5554 5449 4e47 2044 4f57   be SHUTTING DOW
+00023be0: 4e2e 2e2e 223b 2027 0a20 2020 2020 2020  N..."; '.       
+00023bf0: 2020 2020 2066 2773 6c65 6570 2035 3b20       f'sleep 5; 
+00023c00: 733d 2428 736b 7920 7365 7276 6520 7374  s=$(sky serve st
+00023c10: 6174 7573 207b 6e61 6d65 7d29 3b20 6563  atus {name}); ec
+00023c20: 686f 2022 2473 223b 2064 6f6e 653b 2027  ho "$s"; done; '
+00023c30: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
+00023c40: 733d 2428 736b 7920 7365 7276 6520 7374  s=$(sky serve st
+00023c50: 6174 7573 207b 6e61 6d65 7d29 3b20 6563  atus {name}); ec
+00023c60: 686f 2022 2473 223b 270a 2020 2020 2020  ho "$s";'.      
+00023c70: 2020 2020 2020 2775 6e74 696c 2065 6368        'until ech
+00023c80: 6f20 2224 7322 207c 2067 7265 7020 2d41  o "$s" | grep -A
+00023c90: 2031 3030 2022 5365 7276 6963 6520 5265   100 "Service Re
+00023ca0: 706c 6963 6173 2220 7c20 6772 6570 2022  plicas" | grep "
+00023cb0: 4641 494c 4544 223b 2027 0a20 2020 2020  FAILED"; '.     
+00023cc0: 2020 2020 2020 2027 646f 2065 6368 6f20         'do echo 
+00023cd0: 2257 6169 7469 6e67 2066 6f72 2066 6972  "Waiting for fir
+00023ce0: 7374 2073 6572 7669 6365 2074 6f20 6265  st service to be
+00023cf0: 2046 4149 4c45 442e 2e2e 223b 2027 0a20   FAILED..."; '. 
+00023d00: 2020 2020 2020 2020 2020 2066 2773 6c65             f'sle
+00023d10: 6570 2035 3b20 733d 2428 736b 7920 7365  ep 5; s=$(sky se
+00023d20: 7276 6520 7374 6174 7573 207b 6e61 6d65  rve status {name
+00023d30: 7d29 3b20 6563 686f 2022 2473 223b 2064  }); echo "$s"; d
+00023d40: 6f6e 653b 2065 6368 6f20 2224 7322 3b20  one; echo "$s"; 
+00023d50: 270a 2020 2020 2020 2020 2020 2020 2b20  '.            + 
+00023d60: 5f63 6865 636b 5f72 6570 6c69 6361 5f69  _check_replica_i
+00023d70: 6e5f 7374 6174 7573 286e 616d 652c 205b  n_status(name, [
+00023d80: 2831 2c20 5472 7565 2c20 2746 4149 4c45  (1, True, 'FAILE
+00023d90: 4427 295d 2920 2b0a 2020 2020 2020 2020  D')]) +.        
+00023da0: 2020 2020 2320 5573 6572 2062 7567 2066      # User bug f
+00023db0: 6169 6c75 7265 2077 696c 6c20 6361 7573  ailure will caus
+00023dc0: 6520 6e6f 2066 7572 7468 6572 2073 6361  e no further sca
+00023dd0: 6c69 6e67 2e0a 2020 2020 2020 2020 2020  ling..          
+00023de0: 2020 6627 6563 686f 2022 2473 2220 7c20    f'echo "$s" | 
+00023df0: 6772 6570 202d 4120 3130 3020 2253 6572  grep -A 100 "Ser
+00023e00: 7669 6365 2052 6570 6c69 6361 7322 207c  vice Replicas" |
+00023e10: 2067 7265 7020 227b 6e61 6d65 7d22 207c   grep "{name}" |
+00023e20: 2077 6320 2d6c 207c 2067 7265 7020 313b   wc -l | grep 1;
+00023e30: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
+00023e40: 2765 6368 6f20 2224 7322 207c 2067 7265  'echo "$s" | gre
+00023e50: 7020 2d42 2031 3030 2022 4e4f 5f52 4550  p -B 100 "NO_REP
+00023e60: 4c49 4341 2220 7c20 6772 6570 2022 302f  LICA" | grep "0/
+00023e70: 3022 272c 0a20 2020 2020 2020 2020 2020  0"',.           
+00023e80: 2066 2773 6b79 2073 6572 7665 2075 7064   f'sky serve upd
+00023e90: 6174 6520 7b6e 616d 657d 202d 2d63 6c6f  ate {name} --clo
+00023ea0: 7564 207b 6765 6e65 7269 635f 636c 6f75  ud {generic_clou
+00023eb0: 647d 202d 7920 7465 7374 732f 736b 7973  d} -y tests/skys
+00023ec0: 6572 7665 2f61 7574 6f5f 7265 7374 6172  erve/auto_restar
+00023ed0: 742e 7961 6d6c 272c 0a20 2020 2020 2020  t.yaml',.       
+00023ee0: 2020 2020 2066 277b 5f53 4552 5645 5f45       f'{_SERVE_E
+00023ef0: 4e44 504f 494e 545f 5741 4954 2e66 6f72  NDPOINT_WAIT.for
+00023f00: 6d61 7428 6e61 6d65 3d6e 616d 6529 7d3b  mat(name=name)};
+00023f10: 2027 0a20 2020 2020 2020 2020 2020 2027   '.            '
+00023f20: 756e 7469 6c20 6375 726c 2068 7474 703a  until curl http:
+00023f30: 2f2f 2465 6e64 706f 696e 7420 7c20 6772  //$endpoint | gr
+00023f40: 6570 2022 4869 2c20 536b 7950 696c 6f74  ep "Hi, SkyPilot
+00023f50: 2068 6572 6521 223b 2064 6f20 736c 6565   here!"; do slee
+00023f60: 7020 323b 2064 6f6e 653b 2073 6c65 6570  p 2; done; sleep
+00023f70: 2032 3b20 270a 2020 2020 2020 2020 2020   2; '.          
+00023f80: 2020 2b20 5f63 6865 636b 5f72 6570 6c69    + _check_repli
+00023f90: 6361 5f69 6e5f 7374 6174 7573 286e 616d  ca_in_status(nam
+00023fa0: 652c 205b 2831 2c20 4661 6c73 652c 2027  e, [(1, False, '
+00023fb0: 5245 4144 5927 292c 0a20 2020 2020 2020  READY'),.       
+00023fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ff0: 2020 2028 312c 2046 616c 7365 2c20 2746     (1, False, 'F
-00024000: 4149 4c45 4427 295d 292c 0a20 2020 2020  AILED')]),.     
-00024010: 2020 205d 2c0a 2020 2020 2020 2020 5f54     ],.        _T
-00024020: 4541 5244 4f57 4e5f 5345 5256 4943 452e  EARDOWN_SERVICE.
-00024030: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
-00024040: 292c 0a20 2020 2020 2020 2074 696d 656f  ),.        timeo
-00024050: 7574 3d32 3020 2a20 3630 2c0a 2020 2020  ut=20 * 60,.    
-00024060: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-00024070: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
-00024080: 7374 2e6d 6172 6b2e 7365 7276 650a 4070  st.mark.serve.@p
-00024090: 7974 6573 742e 6d61 726b 2e6e 6f5f 6b75  ytest.mark.no_ku
-000240a0: 6265 726e 6574 6573 2020 2320 5265 706c  bernetes  # Repl
-000240b0: 6963 6173 206f 6e20 6b38 7320 6d61 7920  icas on k8s may 
-000240c0: 6265 2072 756e 6e69 6e67 206f 6e20 7468  be running on th
-000240d0: 6520 7361 6d65 206e 6f64 6520 616e 6420  e same node and 
-000240e0: 6861 7665 2074 6865 2073 616d 6520 7075  have the same pu
-000240f0: 626c 6963 2049 500a 6465 6620 7465 7374  blic IP.def test
-00024100: 5f73 6b79 7365 7276 655f 6c6f 6164 5f62  _skyserve_load_b
-00024110: 616c 616e 6365 7228 6765 6e65 7269 635f  alancer(generic_
-00024120: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00024130: 2022 2222 5465 7374 2073 6b79 7365 7276   """Test skyserv
-00024140: 6520 6c6f 6164 2062 616c 616e 6365 7220  e load balancer 
-00024150: 726f 756e 642d 726f 6269 6e20 706f 6c69  round-robin poli
-00024160: 6379 2222 220a 2020 2020 6e61 6d65 203d  cy""".    name =
-00024170: 205f 6765 745f 7365 7276 6963 655f 6e61   _get_service_na
-00024180: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
-00024190: 5465 7374 280a 2020 2020 2020 2020 6627  Test(.        f'
-000241a0: 7465 7374 2d73 6b79 7365 7276 652d 6c6f  test-skyserve-lo
-000241b0: 6164 2d62 616c 616e 6365 7227 2c0a 2020  ad-balancer',.  
-000241c0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-000241d0: 2020 2020 6627 736b 7920 7365 7276 6520      f'sky serve 
-000241e0: 7570 202d 6e20 7b6e 616d 657d 202d 2d63  up -n {name} --c
-000241f0: 6c6f 7564 207b 6765 6e65 7269 635f 636c  loud {generic_cl
-00024200: 6f75 647d 202d 7920 7465 7374 732f 736b  oud} -y tests/sk
-00024210: 7973 6572 7665 2f6c 6f61 645f 6261 6c61  yserve/load_bala
-00024220: 6e63 6572 2f73 6572 7669 6365 2e79 616d  ncer/service.yam
-00024230: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-00024240: 5f53 4552 5645 5f57 4149 545f 554e 5449  _SERVE_WAIT_UNTI
-00024250: 4c5f 5245 4144 592e 666f 726d 6174 286e  L_READY.format(n
-00024260: 616d 653d 6e61 6d65 2c20 7265 706c 6963  ame=name, replic
-00024270: 615f 6e75 6d3d 3329 2c0a 2020 2020 2020  a_num=3),.      
-00024280: 2020 2020 2020 6627 7b5f 5345 5256 455f        f'{_SERVE_
-00024290: 454e 4450 4f49 4e54 5f57 4149 542e 666f  ENDPOINT_WAIT.fo
-000242a0: 726d 6174 286e 616d 653d 6e61 6d65 297d  rmat(name=name)}
-000242b0: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
-000242c0: 6627 7b5f 5345 5256 455f 5354 4154 5553  f'{_SERVE_STATUS
-000242d0: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
-000242e0: 653d 6e61 6d65 297d 3b20 270a 2020 2020  e=name)}; '.    
-000242f0: 2020 2020 2020 2020 6627 7b5f 6765 745f          f'{_get_
-00024300: 7265 706c 6963 615f 6970 286e 616d 652c  replica_ip(name,
-00024310: 2031 297d 3b20 270a 2020 2020 2020 2020   1)}; '.        
-00024320: 2020 2020 6627 7b5f 6765 745f 7265 706c      f'{_get_repl
-00024330: 6963 615f 6970 286e 616d 652c 2032 297d  ica_ip(name, 2)}
-00024340: 3b20 7b5f 6765 745f 7265 706c 6963 615f  ; {_get_replica_
-00024350: 6970 286e 616d 652c 2033 297d 3b20 270a  ip(name, 3)}; '.
-00024360: 2020 2020 2020 2020 2020 2020 2770 7974              'pyt
-00024370: 686f 6e20 7465 7374 732f 736b 7973 6572  hon tests/skyser
-00024380: 7665 2f6c 6f61 645f 6261 6c61 6e63 6572  ve/load_balancer
-00024390: 2f74 6573 745f 726f 756e 645f 726f 6269  /test_round_robi
-000243a0: 6e2e 7079 2027 0a20 2020 2020 2020 2020  n.py '.         
-000243b0: 2020 2027 2d2d 656e 6470 6f69 6e74 2024     '--endpoint $
-000243c0: 656e 6470 6f69 6e74 202d 2d72 6570 6c69  endpoint --repli
-000243d0: 6361 2d6e 756d 2033 202d 2d72 6570 6c69  ca-num 3 --repli
-000243e0: 6361 2d69 7073 2024 6970 3120 2469 7032  ca-ips $ip1 $ip2
-000243f0: 2024 6970 3327 2c0a 2020 2020 2020 2020   $ip3',.        
-00024400: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
-00024410: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
-00024420: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
-00024430: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-00024440: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
-00024450: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
-00024460: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
-00024470: 6d61 726b 2e67 6370 0a40 7079 7465 7374  mark.gcp.@pytest
-00024480: 2e6d 6172 6b2e 7365 7276 650a 4070 7974  .mark.serve.@pyt
-00024490: 6573 742e 6d61 726b 2e6e 6f5f 6b75 6265  est.mark.no_kube
-000244a0: 726e 6574 6573 0a64 6566 2074 6573 745f  rnetes.def test_
-000244b0: 736b 7973 6572 7665 5f61 7574 6f5f 7265  skyserve_auto_re
-000244c0: 7374 6172 7428 293a 0a20 2020 2022 2222  start():.    """
-000244d0: 5465 7374 2073 6b79 7365 7276 6520 7769  Test skyserve wi
-000244e0: 7468 2061 7574 6f20 7265 7374 6172 7422  th auto restart"
-000244f0: 2222 0a20 2020 206e 616d 6520 3d20 5f67  "".    name = _g
-00024500: 6574 5f73 6572 7669 6365 5f6e 616d 6528  et_service_name(
-00024510: 290a 2020 2020 7a6f 6e65 203d 2027 7573  ).    zone = 'us
-00024520: 2d63 656e 7472 616c 312d 6127 0a20 2020  -central1-a'.   
-00024530: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
-00024540: 2020 2020 2020 6627 7465 7374 2d73 6b79        f'test-sky
-00024550: 7365 7276 652d 6175 746f 2d72 6573 7461  serve-auto-resta
-00024560: 7274 272c 0a20 2020 2020 2020 205b 0a20  rt',.        [. 
-00024570: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00024580: 4f28 7469 616e 293a 2077 6520 6361 6e20  O(tian): we can 
-00024590: 6479 6e61 6d69 6361 6c6c 7920 6765 6e65  dynamically gene
-000245a0: 7261 7465 2059 414d 4c20 6672 6f6d 2074  rate YAML from t
-000245b0: 656d 706c 6174 6520 746f 0a20 2020 2020  emplate to.     
-000245c0: 2020 2020 2020 2023 2061 766f 6964 206d         # avoid m
-000245d0: 6169 6e74 6169 6e69 6e67 2074 6f6f 206d  aintaining too m
-000245e0: 616e 7920 5941 4d4c 2066 696c 6573 0a20  any YAML files. 
-000245f0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00024600: 2073 6572 7665 2075 7020 2d6e 207b 6e61   serve up -n {na
-00024610: 6d65 7d20 2d79 2074 6573 7473 2f73 6b79  me} -y tests/sky
-00024620: 7365 7276 652f 6175 746f 5f72 6573 7461  serve/auto_resta
-00024630: 7274 2e79 616d 6c27 2c0a 2020 2020 2020  rt.yaml',.      
-00024640: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
-00024650: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
-00024660: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
-00024670: 7265 706c 6963 615f 6e75 6d3d 3129 2c0a  replica_num=1),.
-00024680: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00024690: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
-000246a0: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
-000246b0: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
-000246c0: 2020 2020 2020 2772 6571 7565 7374 5f6f        'request_o
-000246d0: 7574 7075 743d 2428 6375 726c 202d 4c20  utput=$(curl -L 
-000246e0: 6874 7470 3a2f 2f24 656e 6470 6f69 6e74  http://$endpoint
-000246f0: 293b 2065 6368 6f20 2224 7265 7175 6573  ); echo "$reques
-00024700: 745f 6f75 7470 7574 223b 2065 6368 6f20  t_output"; echo 
-00024710: 2224 7265 7175 6573 745f 6f75 7470 7574  "$request_output
-00024720: 2220 7c20 6772 6570 2022 4869 2c20 536b  " | grep "Hi, Sk
-00024730: 7950 696c 6f74 2068 6572 6522 272c 0a20  yPilot here"',. 
-00024740: 2020 2020 2020 2020 2020 2023 2073 6c65             # sle
-00024750: 6570 2066 6f72 2032 3020 7365 636f 6e64  ep for 20 second
-00024760: 7320 2869 6e69 7469 616c 2064 656c 6179  s (initial delay
-00024770: 2920 746f 206d 616b 6520 7375 7265 2069  ) to make sure i
-00024780: 7420 7769 6c6c 0a20 2020 2020 2020 2020  t will.         
-00024790: 2020 2023 2062 6520 7265 7374 6172 7465     # be restarte
-000247a0: 640a 2020 2020 2020 2020 2020 2020 6627  d.            f'
-000247b0: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
-000247c0: 2020 2020 2020 205f 7465 726d 696e 6174         _terminat
-000247d0: 655f 6763 705f 7265 706c 6963 6128 6e61  e_gcp_replica(na
-000247e0: 6d65 2c20 7a6f 6e65 2c20 3129 2c0a 2020  me, zone, 1),.  
-000247f0: 2020 2020 2020 2020 2020 2320 5761 6974            # Wait
-00024800: 2066 6f72 2063 6f6e 7365 6375 7469 7665   for consecutive
-00024810: 2066 6169 6c75 7265 2074 696d 656f 7574   failure timeout
-00024820: 2070 6173 7365 642e 0a20 2020 2020 2020   passed..       
-00024830: 2020 2020 2023 2049 6620 7468 6520 636c       # If the cl
-00024840: 7573 7465 7220 6973 206e 6f74 2075 7369  uster is not usi
-00024850: 6e67 2073 706f 742c 2069 7420 776f 6e27  ng spot, it won'
-00024860: 7420 6368 6563 6b20 7468 6520 636c 7573  t check the clus
-00024870: 7465 7220 7374 6174 7573 0a20 2020 2020  ter status.     
-00024880: 2020 2020 2020 2023 206f 6e20 7468 6520         # on the 
-00024890: 636c 6f75 6420 2873 696e 6365 206d 616e  cloud (since man
-000248a0: 7561 6c20 7368 7574 646f 776e 2069 7320  ual shutdown is 
-000248b0: 6e6f 7420 6120 636f 6d6d 6f6e 2062 6568  not a common beh
-000248c0: 6176 696f 7220 616e 6420 7375 6368 0a20  avior and such. 
-000248d0: 2020 2020 2020 2020 2020 2023 2071 7565             # que
-000248e0: 7269 6573 2074 616b 6573 2061 206c 6f74  ries takes a lot
-000248f0: 206f 6620 7469 6d65 292e 2049 6e73 7465   of time). Inste
-00024900: 6164 2c20 7765 2074 6869 6e6b 2063 6f6e  ad, we think con
-00024910: 7469 6e75 6f75 7320 3320 6d69 6e20 7072  tinuous 3 min pr
-00024920: 6f62 650a 2020 2020 2020 2020 2020 2020  obe.            
-00024930: 2320 6661 696c 7572 6520 6973 206e 6f74  # failure is not
-00024940: 2061 2074 656d 706f 7261 7279 2070 726f   a temporary pro
-00024950: 626c 656d 2062 7574 2069 6e64 6565 6420  blem but indeed 
-00024960: 6120 6661 696c 7572 652e 0a20 2020 2020  a failure..     
-00024970: 2020 2020 2020 2027 736c 6565 7020 3138         'sleep 18
-00024980: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00024990: 2320 5765 2063 616e 6e6f 7420 7573 6520  # We cannot use 
-000249a0: 5f53 4552 5645 5f57 4149 545f 554e 5449  _SERVE_WAIT_UNTI
-000249b0: 4c5f 5245 4144 593b 2074 6865 7265 2077  L_READY; there w
-000249c0: 696c 6c20 6265 2061 2069 6e74 6572 6d65  ill be a interme
-000249d0: 6469 6174 6520 7469 6d65 0a20 2020 2020  diate time.     
-000249e0: 2020 2020 2020 2023 2074 6861 7420 7468         # that th
-000249f0: 6520 6f75 7470 7574 206f 6620 6073 6b79  e output of `sky
-00024a00: 2073 6572 7665 2073 7461 7475 7360 2073   serve status` s
-00024a10: 686f 7773 2046 4149 4c45 4420 616e 6420  hows FAILED and 
-00024a20: 7468 6973 2073 7461 7475 7320 7769 6c6c  this status will
-00024a30: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
-00024a40: 6175 7365 205f 5345 5256 455f 5741 4954  ause _SERVE_WAIT
-00024a50: 5f55 4e54 494c 5f52 4541 4459 2074 6f20  _UNTIL_READY to 
-00024a60: 6561 726c 7920 7175 6974 2e0a 2020 2020  early quit..    
-00024a70: 2020 2020 2020 2020 2728 7768 696c 6520          '(while 
-00024a80: 7472 7565 3b20 646f 270a 2020 2020 2020  true; do'.      
-00024a90: 2020 2020 2020 6627 2020 2020 6f75 7470        f'    outp
-00024aa0: 7574 3d24 2873 6b79 2073 6572 7665 2073  ut=$(sky serve s
-00024ab0: 7461 7475 7320 7b6e 616d 657d 293b 270a  tatus {name});'.
-00024ac0: 2020 2020 2020 2020 2020 2020 2720 2020              '   
-00024ad0: 2020 6563 686f 2022 246f 7574 7075 7422    echo "$output"
-00024ae0: 207c 2067 7265 7020 2d71 2022 312f 3122   | grep -q "1/1"
-00024af0: 2026 2620 6272 6561 6b3b 270a 2020 2020   && break;'.    
-00024b00: 2020 2020 2020 2020 2720 2020 2020 736c          '     sl
-00024b10: 6565 7020 3130 3b27 0a20 2020 2020 2020  eep 10;'.       
-00024b20: 2020 2020 2066 2764 6f6e 6529 3b20 736c       f'done); sl
-00024b30: 6565 7020 7b73 6572 7665 2e4c 425f 434f  eep {serve.LB_CO
-00024b40: 4e54 524f 4c4c 4552 5f53 594e 435f 494e  NTROLLER_SYNC_IN
-00024b50: 5445 5256 414c 5f53 4543 4f4e 4453 7d3b  TERVAL_SECONDS};
-00024b60: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-00024b70: 277b 5f53 4552 5645 5f45 4e44 504f 494e  '{_SERVE_ENDPOIN
-00024b80: 545f 5741 4954 2e66 6f72 6d61 7428 6e61  T_WAIT.format(na
-00024b90: 6d65 3d6e 616d 6529 7d3b 2027 0a20 2020  me=name)}; '.   
-00024ba0: 2020 2020 2020 2020 2027 7265 7175 6573           'reques
-00024bb0: 745f 6f75 7470 7574 3d24 2863 7572 6c20  t_output=$(curl 
-00024bc0: 2d4c 2068 7474 703a 2f2f 2465 6e64 706f  -L http://$endpo
-00024bd0: 696e 7429 3b20 6563 686f 2022 2472 6571  int); echo "$req
-00024be0: 7565 7374 5f6f 7574 7075 7422 3b20 6563  uest_output"; ec
-00024bf0: 686f 2022 2472 6571 7565 7374 5f6f 7574  ho "$request_out
-00024c00: 7075 7422 207c 2067 7265 7020 2248 692c  put" | grep "Hi,
-00024c10: 2053 6b79 5069 6c6f 7420 6865 7265 2227   SkyPilot here"'
-00024c20: 2c0a 2020 2020 2020 2020 5d2c 0a20 2020  ,.        ],.   
-00024c30: 2020 2020 205f 5445 4152 444f 574e 5f53       _TEARDOWN_S
-00024c40: 4552 5649 4345 2e66 6f72 6d61 7428 6e61  ERVICE.format(na
-00024c50: 6d65 3d6e 616d 6529 2c0a 2020 2020 2020  me=name),.      
-00024c60: 2020 7469 6d65 6f75 743d 3230 202a 2036    timeout=20 * 6
-00024c70: 302c 0a20 2020 2029 0a20 2020 2072 756e  0,.    ).    run
-00024c80: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
-00024c90: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
-00024ca0: 6572 7665 0a64 6566 2074 6573 745f 736b  erve.def test_sk
-00024cb0: 7973 6572 7665 5f63 616e 6365 6c28 6765  yserve_cancel(ge
-00024cc0: 6e65 7269 635f 636c 6f75 643a 2073 7472  neric_cloud: str
-00024cd0: 293a 0a20 2020 2022 2222 5465 7374 2073  ):.    """Test s
-00024ce0: 6b79 7365 7276 6520 7769 7468 2063 616e  kyserve with can
-00024cf0: 6365 6c22 2222 0a20 2020 206e 616d 6520  cel""".    name 
-00024d00: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
-00024d10: 616d 6528 290a 0a20 2020 2074 6573 7420  ame()..    test 
-00024d20: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
-00024d30: 6627 7465 7374 2d73 6b79 7365 7276 652d  f'test-skyserve-
-00024d40: 6361 6e63 656c 272c 0a20 2020 2020 2020  cancel',.       
-00024d50: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
-00024d60: 2773 6b79 2073 6572 7665 2075 7020 2d6e  'sky serve up -n
-00024d70: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
-00024d80: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
-00024d90: 2d79 2074 6573 7473 2f73 6b79 7365 7276  -y tests/skyserv
-00024da0: 652f 6361 6e63 656c 2f63 616e 6365 6c2e  e/cancel/cancel.
-00024db0: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00024dc0: 2020 205f 5345 5256 455f 5741 4954 5f55     _SERVE_WAIT_U
-00024dd0: 4e54 494c 5f52 4541 4459 2e66 6f72 6d61  NTIL_READY.forma
-00024de0: 7428 6e61 6d65 3d6e 616d 652c 2072 6570  t(name=name, rep
-00024df0: 6c69 6361 5f6e 756d 3d31 292c 0a20 2020  lica_num=1),.   
-00024e00: 2020 2020 2020 2020 2066 277b 5f53 4552           f'{_SER
-00024e10: 5645 5f45 4e44 504f 494e 545f 5741 4954  VE_ENDPOINT_WAIT
-00024e20: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
-00024e30: 6529 7d3b 2070 7974 686f 6e33 2027 0a20  e)}; python3 '. 
-00024e40: 2020 2020 2020 2020 2020 2027 7465 7374             'test
-00024e50: 732f 736b 7973 6572 7665 2f63 616e 6365  s/skyserve/cance
-00024e60: 6c2f 7365 6e64 5f63 616e 6365 6c5f 7265  l/send_cancel_re
-00024e70: 7175 6573 742e 7079 2027 0a20 2020 2020  quest.py '.     
-00024e80: 2020 2020 2020 2027 2d2d 656e 6470 6f69         '--endpoi
-00024e90: 6e74 2024 656e 6470 6f69 6e74 207c 2067  nt $endpoint | g
-00024ea0: 7265 7020 2252 6571 7565 7374 2077 6173  rep "Request was
-00024eb0: 2063 616e 6365 6c6c 6564 2227 2c0a 2020   cancelled"',.  
-00024ec0: 2020 2020 2020 2020 2020 6627 733d 2428            f's=$(
-00024ed0: 736b 7920 7365 7276 6520 6c6f 6773 207b  sky serve logs {
-00024ee0: 6e61 6d65 7d20 3120 2d2d 6e6f 2d66 6f6c  name} 1 --no-fol
-00024ef0: 6c6f 7729 3b20 270a 2020 2020 2020 2020  low); '.        
-00024f00: 2020 2020 2775 6e74 696c 2021 2065 6368      'until ! ech
-00024f10: 6f20 2224 7322 207c 2067 7265 7020 2250  o "$s" | grep "P
-00024f20: 6c65 6173 6520 7761 6974 2066 6f72 2074  lease wait for t
-00024f30: 6865 2063 6f6e 7472 6f6c 6c65 7220 746f  he controller to
-00024f40: 2062 6522 3b20 270a 2020 2020 2020 2020   be"; '.        
-00024f50: 2020 2020 2764 6f20 6563 686f 2022 5761      'do echo "Wa
-00024f60: 6974 696e 6720 666f 7220 7365 7276 6520  iting for serve 
-00024f70: 6c6f 6773 223b 2073 6c65 6570 2031 303b  logs"; sleep 10;
-00024f80: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
-00024f90: 2773 3d24 2873 6b79 2073 6572 7665 206c  's=$(sky serve l
-00024fa0: 6f67 7320 7b6e 616d 657d 2031 202d 2d6e  ogs {name} 1 --n
-00024fb0: 6f2d 666f 6c6c 6f77 293b 2064 6f6e 653b  o-follow); done;
-00024fc0: 2027 0a20 2020 2020 2020 2020 2020 2027   '.            '
-00024fd0: 6563 686f 2022 2473 223b 2065 6368 6f20  echo "$s"; echo 
-00024fe0: 2224 7322 207c 2067 7265 7020 2243 6c69  "$s" | grep "Cli
-00024ff0: 656e 7420 6469 7363 6f6e 6e65 6374 6564  ent disconnected
-00025000: 2c20 7374 6f70 7069 6e67 2063 6f6d 7075  , stopping compu
-00025010: 7461 7469 6f6e 2227 2c0a 2020 2020 2020  tation"',.      
-00025020: 2020 5d2c 0a20 2020 2020 2020 205f 5445    ],.        _TE
-00025030: 4152 444f 574e 5f53 4552 5649 4345 2e66  ARDOWN_SERVICE.f
-00025040: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
-00025050: 2c0a 2020 2020 2020 2020 7469 6d65 6f75  ,.        timeou
-00025060: 743d 3230 202a 2036 302c 0a20 2020 2029  t=20 * 60,.    )
-00025070: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
-00025080: 7428 7465 7374 290a 0a0a 4070 7974 6573  t(test)...@pytes
-00025090: 742e 6d61 726b 2e73 6572 7665 0a64 6566  t.mark.serve.def
-000250a0: 2074 6573 745f 736b 7973 6572 7665 5f75   test_skyserve_u
-000250b0: 7064 6174 6528 6765 6e65 7269 635f 636c  pdate(generic_cl
-000250c0: 6f75 643a 2073 7472 293a 0a20 2020 2022  oud: str):.    "
-000250d0: 2222 5465 7374 2073 6b79 7365 7276 6520  ""Test skyserve 
-000250e0: 7769 7468 2075 7064 6174 6522 2222 0a20  with update""". 
-000250f0: 2020 206e 616d 6520 3d20 5f67 6574 5f73     name = _get_s
-00025100: 6572 7669 6365 5f6e 616d 6528 290a 2020  ervice_name().  
-00025110: 2020 7465 7374 203d 2054 6573 7428 0a20    test = Test(. 
-00025120: 2020 2020 2020 2066 2774 6573 742d 736b         f'test-sk
-00025130: 7973 6572 7665 2d75 7064 6174 6527 2c0a  yserve-update',.
-00025140: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00025150: 2020 2020 2020 6627 736b 7920 7365 7276        f'sky serv
-00025160: 6520 7570 202d 6e20 7b6e 616d 657d 202d  e up -n {name} -
-00025170: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
-00025180: 636c 6f75 647d 202d 7920 7465 7374 732f  cloud} -y tests/
-00025190: 736b 7973 6572 7665 2f75 7064 6174 652f  skyserve/update/
-000251a0: 6f6c 642e 7961 6d6c 272c 0a20 2020 2020  old.yaml',.     
+00023fe0: 2020 2020 2020 2028 312c 2046 616c 7365         (1, False
+00023ff0: 2c20 2746 4149 4c45 4427 295d 292c 0a20  , 'FAILED')]),. 
+00024000: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00024010: 2020 5f54 4541 5244 4f57 4e5f 5345 5256    _TEARDOWN_SERV
+00024020: 4943 452e 666f 726d 6174 286e 616d 653d  ICE.format(name=
+00024030: 6e61 6d65 292c 0a20 2020 2020 2020 2074  name),.        t
+00024040: 696d 656f 7574 3d32 3020 2a20 3630 2c0a  imeout=20 * 60,.
+00024050: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+00024060: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
+00024070: 7079 7465 7374 2e6d 6172 6b2e 7365 7276  pytest.mark.serv
+00024080: 650a 4070 7974 6573 742e 6d61 726b 2e6e  e.@pytest.mark.n
+00024090: 6f5f 6b75 6265 726e 6574 6573 2020 2320  o_kubernetes  # 
+000240a0: 5265 706c 6963 6173 206f 6e20 6b38 7320  Replicas on k8s 
+000240b0: 6d61 7920 6265 2072 756e 6e69 6e67 206f  may be running o
+000240c0: 6e20 7468 6520 7361 6d65 206e 6f64 6520  n the same node 
+000240d0: 616e 6420 6861 7665 2074 6865 2073 616d  and have the sam
+000240e0: 6520 7075 626c 6963 2049 500a 6465 6620  e public IP.def 
+000240f0: 7465 7374 5f73 6b79 7365 7276 655f 6c6f  test_skyserve_lo
+00024100: 6164 5f62 616c 616e 6365 7228 6765 6e65  ad_balancer(gene
+00024110: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+00024120: 0a20 2020 2022 2222 5465 7374 2073 6b79  .    """Test sky
+00024130: 7365 7276 6520 6c6f 6164 2062 616c 616e  serve load balan
+00024140: 6365 7220 726f 756e 642d 726f 6269 6e20  cer round-robin 
+00024150: 706f 6c69 6379 2222 220a 2020 2020 6e61  policy""".    na
+00024160: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
+00024170: 655f 6e61 6d65 2829 0a20 2020 2074 6573  e_name().    tes
+00024180: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
+00024190: 2020 6627 7465 7374 2d73 6b79 7365 7276    f'test-skyserv
+000241a0: 652d 6c6f 6164 2d62 616c 616e 6365 7227  e-load-balancer'
+000241b0: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+000241c0: 2020 2020 2020 2020 6627 736b 7920 7365          f'sky se
+000241d0: 7276 6520 7570 202d 6e20 7b6e 616d 657d  rve up -n {name}
+000241e0: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
+000241f0: 635f 636c 6f75 647d 202d 7920 7465 7374  c_cloud} -y test
+00024200: 732f 736b 7973 6572 7665 2f6c 6f61 645f  s/skyserve/load_
+00024210: 6261 6c61 6e63 6572 2f73 6572 7669 6365  balancer/service
+00024220: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+00024230: 2020 2020 5f53 4552 5645 5f57 4149 545f      _SERVE_WAIT_
+00024240: 554e 5449 4c5f 5245 4144 592e 666f 726d  UNTIL_READY.form
+00024250: 6174 286e 616d 653d 6e61 6d65 2c20 7265  at(name=name, re
+00024260: 706c 6963 615f 6e75 6d3d 3329 2c0a 2020  plica_num=3),.  
+00024270: 2020 2020 2020 2020 2020 6627 7b5f 5345            f'{_SE
+00024280: 5256 455f 454e 4450 4f49 4e54 5f57 4149  RVE_ENDPOINT_WAI
+00024290: 542e 666f 726d 6174 286e 616d 653d 6e61  T.format(name=na
+000242a0: 6d65 297d 3b20 270a 2020 2020 2020 2020  me)}; '.        
+000242b0: 2020 2020 6627 7b5f 5345 5256 455f 5354      f'{_SERVE_ST
+000242c0: 4154 5553 5f57 4149 542e 666f 726d 6174  ATUS_WAIT.format
+000242d0: 286e 616d 653d 6e61 6d65 297d 3b20 270a  (name=name)}; '.
+000242e0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+000242f0: 6765 745f 7265 706c 6963 615f 6970 286e  get_replica_ip(n
+00024300: 616d 652c 2031 297d 3b20 270a 2020 2020  ame, 1)}; '.    
+00024310: 2020 2020 2020 2020 6627 7b5f 6765 745f          f'{_get_
+00024320: 7265 706c 6963 615f 6970 286e 616d 652c  replica_ip(name,
+00024330: 2032 297d 3b20 7b5f 6765 745f 7265 706c   2)}; {_get_repl
+00024340: 6963 615f 6970 286e 616d 652c 2033 297d  ica_ip(name, 3)}
+00024350: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
+00024360: 2770 7974 686f 6e20 7465 7374 732f 736b  'python tests/sk
+00024370: 7973 6572 7665 2f6c 6f61 645f 6261 6c61  yserve/load_bala
+00024380: 6e63 6572 2f74 6573 745f 726f 756e 645f  ncer/test_round_
+00024390: 726f 6269 6e2e 7079 2027 0a20 2020 2020  robin.py '.     
+000243a0: 2020 2020 2020 2027 2d2d 656e 6470 6f69         '--endpoi
+000243b0: 6e74 2024 656e 6470 6f69 6e74 202d 2d72  nt $endpoint --r
+000243c0: 6570 6c69 6361 2d6e 756d 2033 202d 2d72  eplica-num 3 --r
+000243d0: 6570 6c69 6361 2d69 7073 2024 6970 3120  eplica-ips $ip1 
+000243e0: 2469 7032 2024 6970 3327 2c0a 2020 2020  $ip2 $ip3',.    
+000243f0: 2020 2020 5d2c 0a20 2020 2020 2020 205f      ],.        _
+00024400: 5445 4152 444f 574e 5f53 4552 5649 4345  TEARDOWN_SERVICE
+00024410: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
+00024420: 6529 2c0a 2020 2020 2020 2020 7469 6d65  e),.        time
+00024430: 6f75 743d 3230 202a 2036 302c 0a20 2020  out=20 * 60,.   
+00024440: 2029 0a20 2020 2072 756e 5f6f 6e65 5f74   ).    run_one_t
+00024450: 6573 7428 7465 7374 290a 0a0a 4070 7974  est(test)...@pyt
+00024460: 6573 742e 6d61 726b 2e67 6370 0a40 7079  est.mark.gcp.@py
+00024470: 7465 7374 2e6d 6172 6b2e 7365 7276 650a  test.mark.serve.
+00024480: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+00024490: 6b75 6265 726e 6574 6573 0a64 6566 2074  kubernetes.def t
+000244a0: 6573 745f 736b 7973 6572 7665 5f61 7574  est_skyserve_aut
+000244b0: 6f5f 7265 7374 6172 7428 293a 0a20 2020  o_restart():.   
+000244c0: 2022 2222 5465 7374 2073 6b79 7365 7276   """Test skyserv
+000244d0: 6520 7769 7468 2061 7574 6f20 7265 7374  e with auto rest
+000244e0: 6172 7422 2222 0a20 2020 206e 616d 6520  art""".    name 
+000244f0: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
+00024500: 616d 6528 290a 2020 2020 7a6f 6e65 203d  ame().    zone =
+00024510: 2027 7573 2d63 656e 7472 616c 312d 6127   'us-central1-a'
+00024520: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+00024530: 280a 2020 2020 2020 2020 6627 7465 7374  (.        f'test
+00024540: 2d73 6b79 7365 7276 652d 6175 746f 2d72  -skyserve-auto-r
+00024550: 6573 7461 7274 272c 0a20 2020 2020 2020  estart',.       
+00024560: 205b 0a20 2020 2020 2020 2020 2020 2023   [.            #
+00024570: 2054 4f44 4f28 7469 616e 293a 2077 6520   TODO(tian): we 
+00024580: 6361 6e20 6479 6e61 6d69 6361 6c6c 7920  can dynamically 
+00024590: 6765 6e65 7261 7465 2059 414d 4c20 6672  generate YAML fr
+000245a0: 6f6d 2074 656d 706c 6174 6520 746f 0a20  om template to. 
+000245b0: 2020 2020 2020 2020 2020 2023 2061 766f             # avo
+000245c0: 6964 206d 6169 6e74 6169 6e69 6e67 2074  id maintaining t
+000245d0: 6f6f 206d 616e 7920 5941 4d4c 2066 696c  oo many YAML fil
+000245e0: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
+000245f0: 2773 6b79 2073 6572 7665 2075 7020 2d6e  'sky serve up -n
+00024600: 207b 6e61 6d65 7d20 2d79 2074 6573 7473   {name} -y tests
+00024610: 2f73 6b79 7365 7276 652f 6175 746f 5f72  /skyserve/auto_r
+00024620: 6573 7461 7274 2e79 616d 6c27 2c0a 2020  estart.yaml',.  
+00024630: 2020 2020 2020 2020 2020 5f53 4552 5645            _SERVE
+00024640: 5f57 4149 545f 554e 5449 4c5f 5245 4144  _WAIT_UNTIL_READ
+00024650: 592e 666f 726d 6174 286e 616d 653d 6e61  Y.format(name=na
+00024660: 6d65 2c20 7265 706c 6963 615f 6e75 6d3d  me, replica_num=
+00024670: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
+00024680: 6627 7b5f 5345 5256 455f 454e 4450 4f49  f'{_SERVE_ENDPOI
+00024690: 4e54 5f57 4149 542e 666f 726d 6174 286e  NT_WAIT.format(n
+000246a0: 616d 653d 6e61 6d65 297d 3b20 270a 2020  ame=name)}; '.  
+000246b0: 2020 2020 2020 2020 2020 2772 6571 7565            'reque
+000246c0: 7374 5f6f 7574 7075 743d 2428 6375 726c  st_output=$(curl
+000246d0: 2068 7474 703a 2f2f 2465 6e64 706f 696e   http://$endpoin
+000246e0: 7429 3b20 6563 686f 2022 2472 6571 7565  t); echo "$reque
+000246f0: 7374 5f6f 7574 7075 7422 3b20 6563 686f  st_output"; echo
+00024700: 2022 2472 6571 7565 7374 5f6f 7574 7075   "$request_outpu
+00024710: 7422 207c 2067 7265 7020 2248 692c 2053  t" | grep "Hi, S
+00024720: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
+00024730: 2020 2020 2020 2020 2020 2020 2320 736c              # sl
+00024740: 6565 7020 666f 7220 3230 2073 6563 6f6e  eep for 20 secon
+00024750: 6473 2028 696e 6974 6961 6c20 6465 6c61  ds (initial dela
+00024760: 7929 2074 6f20 6d61 6b65 2073 7572 6520  y) to make sure 
+00024770: 6974 2077 696c 6c0a 2020 2020 2020 2020  it will.        
+00024780: 2020 2020 2320 6265 2072 6573 7461 7274      # be restart
+00024790: 6564 0a20 2020 2020 2020 2020 2020 2066  ed.            f
+000247a0: 2773 6c65 6570 2032 3027 2c0a 2020 2020  'sleep 20',.    
+000247b0: 2020 2020 2020 2020 5f74 6572 6d69 6e61          _termina
+000247c0: 7465 5f67 6370 5f72 6570 6c69 6361 286e  te_gcp_replica(n
+000247d0: 616d 652c 207a 6f6e 652c 2031 292c 0a20  ame, zone, 1),. 
+000247e0: 2020 2020 2020 2020 2020 2023 2057 6169             # Wai
+000247f0: 7420 666f 7220 636f 6e73 6563 7574 6976  t for consecutiv
+00024800: 6520 6661 696c 7572 6520 7469 6d65 6f75  e failure timeou
+00024810: 7420 7061 7373 6564 2e0a 2020 2020 2020  t passed..      
+00024820: 2020 2020 2020 2320 4966 2074 6865 2063        # If the c
+00024830: 6c75 7374 6572 2069 7320 6e6f 7420 7573  luster is not us
+00024840: 696e 6720 7370 6f74 2c20 6974 2077 6f6e  ing spot, it won
+00024850: 2774 2063 6865 636b 2074 6865 2063 6c75  't check the clu
+00024860: 7374 6572 2073 7461 7475 730a 2020 2020  ster status.    
+00024870: 2020 2020 2020 2020 2320 6f6e 2074 6865          # on the
+00024880: 2063 6c6f 7564 2028 7369 6e63 6520 6d61   cloud (since ma
+00024890: 6e75 616c 2073 6875 7464 6f77 6e20 6973  nual shutdown is
+000248a0: 206e 6f74 2061 2063 6f6d 6d6f 6e20 6265   not a common be
+000248b0: 6861 7669 6f72 2061 6e64 2073 7563 680a  havior and such.
+000248c0: 2020 2020 2020 2020 2020 2020 2320 7175              # qu
+000248d0: 6572 6965 7320 7461 6b65 7320 6120 6c6f  eries takes a lo
+000248e0: 7420 6f66 2074 696d 6529 2e20 496e 7374  t of time). Inst
+000248f0: 6561 642c 2077 6520 7468 696e 6b20 636f  ead, we think co
+00024900: 6e74 696e 756f 7573 2033 206d 696e 2070  ntinuous 3 min p
+00024910: 726f 6265 0a20 2020 2020 2020 2020 2020  robe.           
+00024920: 2023 2066 6169 6c75 7265 2069 7320 6e6f   # failure is no
+00024930: 7420 6120 7465 6d70 6f72 6172 7920 7072  t a temporary pr
+00024940: 6f62 6c65 6d20 6275 7420 696e 6465 6564  oblem but indeed
+00024950: 2061 2066 6169 6c75 7265 2e0a 2020 2020   a failure..    
+00024960: 2020 2020 2020 2020 2773 6c65 6570 2031          'sleep 1
+00024970: 3830 272c 0a20 2020 2020 2020 2020 2020  80',.           
+00024980: 2023 2057 6520 6361 6e6e 6f74 2075 7365   # We cannot use
+00024990: 205f 5345 5256 455f 5741 4954 5f55 4e54   _SERVE_WAIT_UNT
+000249a0: 494c 5f52 4541 4459 3b20 7468 6572 6520  IL_READY; there 
+000249b0: 7769 6c6c 2062 6520 6120 696e 7465 726d  will be a interm
+000249c0: 6564 6961 7465 2074 696d 650a 2020 2020  ediate time.    
+000249d0: 2020 2020 2020 2020 2320 7468 6174 2074          # that t
+000249e0: 6865 206f 7574 7075 7420 6f66 2060 736b  he output of `sk
+000249f0: 7920 7365 7276 6520 7374 6174 7573 6020  y serve status` 
+00024a00: 7368 6f77 7320 4641 494c 4544 2061 6e64  shows FAILED and
+00024a10: 2074 6869 7320 7374 6174 7573 2077 696c   this status wil
+00024a20: 6c0a 2020 2020 2020 2020 2020 2020 2320  l.            # 
+00024a30: 6361 7573 6520 5f53 4552 5645 5f57 4149  cause _SERVE_WAI
+00024a40: 545f 554e 5449 4c5f 5245 4144 5920 746f  T_UNTIL_READY to
+00024a50: 2065 6172 6c79 2071 7569 742e 0a20 2020   early quit..   
+00024a60: 2020 2020 2020 2020 2027 2877 6869 6c65           '(while
+00024a70: 2074 7275 653b 2064 6f27 0a20 2020 2020   true; do'.     
+00024a80: 2020 2020 2020 2066 2720 2020 206f 7574         f'    out
+00024a90: 7075 743d 2428 736b 7920 7365 7276 6520  put=$(sky serve 
+00024aa0: 7374 6174 7573 207b 6e61 6d65 7d29 3b27  status {name});'
+00024ab0: 0a20 2020 2020 2020 2020 2020 2027 2020  .            '  
+00024ac0: 2020 2065 6368 6f20 2224 6f75 7470 7574     echo "$output
+00024ad0: 2220 7c20 6772 6570 202d 7120 2231 2f31  " | grep -q "1/1
+00024ae0: 2220 2626 2062 7265 616b 3b27 0a20 2020  " && break;'.   
+00024af0: 2020 2020 2020 2020 2027 2020 2020 2073           '     s
+00024b00: 6c65 6570 2031 303b 270a 2020 2020 2020  leep 10;'.      
+00024b10: 2020 2020 2020 6627 646f 6e65 293b 2073        f'done); s
+00024b20: 6c65 6570 207b 7365 7276 652e 4c42 5f43  leep {serve.LB_C
+00024b30: 4f4e 5452 4f4c 4c45 525f 5359 4e43 5f49  ONTROLLER_SYNC_I
+00024b40: 4e54 4552 5641 4c5f 5345 434f 4e44 537d  NTERVAL_SECONDS}
+00024b50: 3b27 2c0a 2020 2020 2020 2020 2020 2020  ;',.            
+00024b60: 6627 7b5f 5345 5256 455f 454e 4450 4f49  f'{_SERVE_ENDPOI
+00024b70: 4e54 5f57 4149 542e 666f 726d 6174 286e  NT_WAIT.format(n
+00024b80: 616d 653d 6e61 6d65 297d 3b20 270a 2020  ame=name)}; '.  
+00024b90: 2020 2020 2020 2020 2020 2772 6571 7565            'reque
+00024ba0: 7374 5f6f 7574 7075 743d 2428 6375 726c  st_output=$(curl
+00024bb0: 2068 7474 703a 2f2f 2465 6e64 706f 696e   http://$endpoin
+00024bc0: 7429 3b20 6563 686f 2022 2472 6571 7565  t); echo "$reque
+00024bd0: 7374 5f6f 7574 7075 7422 3b20 6563 686f  st_output"; echo
+00024be0: 2022 2472 6571 7565 7374 5f6f 7574 7075   "$request_outpu
+00024bf0: 7422 207c 2067 7265 7020 2248 692c 2053  t" | grep "Hi, S
+00024c00: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
+00024c10: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00024c20: 2020 205f 5445 4152 444f 574e 5f53 4552     _TEARDOWN_SER
+00024c30: 5649 4345 2e66 6f72 6d61 7428 6e61 6d65  VICE.format(name
+00024c40: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
+00024c50: 7469 6d65 6f75 743d 3230 202a 2036 302c  timeout=20 * 60,
+00024c60: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
+00024c70: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
+00024c80: 4070 7974 6573 742e 6d61 726b 2e73 6572  @pytest.mark.ser
+00024c90: 7665 0a64 6566 2074 6573 745f 736b 7973  ve.def test_skys
+00024ca0: 6572 7665 5f63 616e 6365 6c28 6765 6e65  erve_cancel(gene
+00024cb0: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
+00024cc0: 0a20 2020 2022 2222 5465 7374 2073 6b79  .    """Test sky
+00024cd0: 7365 7276 6520 7769 7468 2063 616e 6365  serve with cance
+00024ce0: 6c22 2222 0a20 2020 206e 616d 6520 3d20  l""".    name = 
+00024cf0: 5f67 6574 5f73 6572 7669 6365 5f6e 616d  _get_service_nam
+00024d00: 6528 290a 0a20 2020 2074 6573 7420 3d20  e()..    test = 
+00024d10: 5465 7374 280a 2020 2020 2020 2020 6627  Test(.        f'
+00024d20: 7465 7374 2d73 6b79 7365 7276 652d 6361  test-skyserve-ca
+00024d30: 6e63 656c 272c 0a20 2020 2020 2020 205b  ncel',.        [
+00024d40: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00024d50: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
+00024d60: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
+00024d70: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
+00024d80: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
+00024d90: 6361 6e63 656c 2f63 616e 6365 6c2e 7961  cancel/cancel.ya
+00024da0: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
+00024db0: 205f 5345 5256 455f 5741 4954 5f55 4e54   _SERVE_WAIT_UNT
+00024dc0: 494c 5f52 4541 4459 2e66 6f72 6d61 7428  IL_READY.format(
+00024dd0: 6e61 6d65 3d6e 616d 652c 2072 6570 6c69  name=name, repli
+00024de0: 6361 5f6e 756d 3d31 292c 0a20 2020 2020  ca_num=1),.     
+00024df0: 2020 2020 2020 2066 277b 5f53 4552 5645         f'{_SERVE
+00024e00: 5f45 4e44 504f 494e 545f 5741 4954 2e66  _ENDPOINT_WAIT.f
+00024e10: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
+00024e20: 7d3b 2070 7974 686f 6e33 2027 0a20 2020  }; python3 '.   
+00024e30: 2020 2020 2020 2020 2027 7465 7374 732f           'tests/
+00024e40: 736b 7973 6572 7665 2f63 616e 6365 6c2f  skyserve/cancel/
+00024e50: 7365 6e64 5f63 616e 6365 6c5f 7265 7175  send_cancel_requ
+00024e60: 6573 742e 7079 2027 0a20 2020 2020 2020  est.py '.       
+00024e70: 2020 2020 2027 2d2d 656e 6470 6f69 6e74       '--endpoint
+00024e80: 2024 656e 6470 6f69 6e74 207c 2067 7265   $endpoint | gre
+00024e90: 7020 2252 6571 7565 7374 2077 6173 2063  p "Request was c
+00024ea0: 616e 6365 6c6c 6564 2227 2c0a 2020 2020  ancelled"',.    
+00024eb0: 2020 2020 2020 2020 6627 733d 2428 736b          f's=$(sk
+00024ec0: 7920 7365 7276 6520 6c6f 6773 207b 6e61  y serve logs {na
+00024ed0: 6d65 7d20 3120 2d2d 6e6f 2d66 6f6c 6c6f  me} 1 --no-follo
+00024ee0: 7729 3b20 270a 2020 2020 2020 2020 2020  w); '.          
+00024ef0: 2020 2775 6e74 696c 2021 2065 6368 6f20    'until ! echo 
+00024f00: 2224 7322 207c 2067 7265 7020 2250 6c65  "$s" | grep "Ple
+00024f10: 6173 6520 7761 6974 2066 6f72 2074 6865  ase wait for the
+00024f20: 2063 6f6e 7472 6f6c 6c65 7220 746f 2062   controller to b
+00024f30: 6522 3b20 270a 2020 2020 2020 2020 2020  e"; '.          
+00024f40: 2020 2764 6f20 6563 686f 2022 5761 6974    'do echo "Wait
+00024f50: 696e 6720 666f 7220 7365 7276 6520 6c6f  ing for serve lo
+00024f60: 6773 223b 2073 6c65 6570 2031 303b 2027  gs"; sleep 10; '
+00024f70: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00024f80: 3d24 2873 6b79 2073 6572 7665 206c 6f67  =$(sky serve log
+00024f90: 7320 7b6e 616d 657d 2031 202d 2d6e 6f2d  s {name} 1 --no-
+00024fa0: 666f 6c6c 6f77 293b 2064 6f6e 653b 2027  follow); done; '
+00024fb0: 0a20 2020 2020 2020 2020 2020 2027 6563  .            'ec
+00024fc0: 686f 2022 2473 223b 2065 6368 6f20 2224  ho "$s"; echo "$
+00024fd0: 7322 207c 2067 7265 7020 2243 6c69 656e  s" | grep "Clien
+00024fe0: 7420 6469 7363 6f6e 6e65 6374 6564 2c20  t disconnected, 
+00024ff0: 7374 6f70 7069 6e67 2063 6f6d 7075 7461  stopping computa
+00025000: 7469 6f6e 2227 2c0a 2020 2020 2020 2020  tion"',.        
+00025010: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
+00025020: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
+00025030: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
+00025040: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00025050: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
+00025060: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00025070: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00025080: 6d61 726b 2e73 6572 7665 0a64 6566 2074  mark.serve.def t
+00025090: 6573 745f 736b 7973 6572 7665 5f73 7472  est_skyserve_str
+000250a0: 6561 6d69 6e67 2867 656e 6572 6963 5f63  eaming(generic_c
+000250b0: 6c6f 7564 3a20 7374 7229 3a0a 2020 2020  loud: str):.    
+000250c0: 2222 2254 6573 7420 736b 7973 6572 7665  """Test skyserve
+000250d0: 2077 6974 6820 7374 7265 616d 696e 6722   with streaming"
+000250e0: 2222 0a20 2020 206e 616d 6520 3d20 5f67  "".    name = _g
+000250f0: 6574 5f73 6572 7669 6365 5f6e 616d 6528  et_service_name(
+00025100: 290a 2020 2020 7465 7374 203d 2054 6573  ).    test = Tes
+00025110: 7428 0a20 2020 2020 2020 2066 2774 6573  t(.        f'tes
+00025120: 742d 736b 7973 6572 7665 2d73 7472 6561  t-skyserve-strea
+00025130: 6d69 6e67 272c 0a20 2020 2020 2020 205b  ming',.        [
+00025140: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00025150: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
+00025160: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
+00025170: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
+00025180: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
+00025190: 7374 7265 616d 696e 672f 7374 7265 616d  streaming/stream
+000251a0: 696e 672e 7961 6d6c 272c 0a20 2020 2020  ing.yaml',.     
 000251b0: 2020 2020 2020 205f 5345 5256 455f 5741         _SERVE_WA
 000251c0: 4954 5f55 4e54 494c 5f52 4541 4459 2e66  IT_UNTIL_READY.f
 000251d0: 6f72 6d61 7428 6e61 6d65 3d6e 616d 652c  ormat(name=name,
-000251e0: 2072 6570 6c69 6361 5f6e 756d 3d32 292c   replica_num=2),
+000251e0: 2072 6570 6c69 6361 5f6e 756d 3d31 292c   replica_num=1),
 000251f0: 0a20 2020 2020 2020 2020 2020 2066 277b  .            f'{
 00025200: 5f53 4552 5645 5f45 4e44 504f 494e 545f  _SERVE_ENDPOINT_
 00025210: 5741 4954 2e66 6f72 6d61 7428 6e61 6d65  WAIT.format(name
-00025220: 3d6e 616d 6529 7d3b 2063 7572 6c20 2d4c  =name)}; curl -L
-00025230: 2068 7474 703a 2f2f 2465 6e64 706f 696e   http://$endpoin
-00025240: 7420 7c20 6772 6570 2022 4869 2c20 536b  t | grep "Hi, Sk
-00025250: 7950 696c 6f74 2068 6572 6522 272c 0a20  yPilot here"',. 
-00025260: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00025270: 2073 6572 7665 2075 7064 6174 6520 7b6e   serve update {n
-00025280: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
-00025290: 6e65 7269 635f 636c 6f75 647d 202d 2d6d  neric_cloud} --m
-000252a0: 6f64 6520 626c 7565 5f67 7265 656e 202d  ode blue_green -
-000252b0: 7920 7465 7374 732f 736b 7973 6572 7665  y tests/skyserve
-000252c0: 2f75 7064 6174 652f 6e65 772e 7961 6d6c  /update/new.yaml
-000252d0: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
-000252e0: 2073 6c65 6570 2062 6566 6f72 6520 7570   sleep before up
-000252f0: 6461 7465 2069 7320 7265 6769 7374 6572  date is register
-00025300: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
-00025310: 2773 6c65 6570 2032 3027 2c0a 2020 2020  'sleep 20',.    
-00025320: 2020 2020 2020 2020 6627 7b5f 5345 5256          f'{_SERV
-00025330: 455f 454e 4450 4f49 4e54 5f57 4149 542e  E_ENDPOINT_WAIT.
-00025340: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
-00025350: 297d 3b20 270a 2020 2020 2020 2020 2020  )}; '.          
-00025360: 2020 2775 6e74 696c 2063 7572 6c20 2d4c    'until curl -L
-00025370: 2068 7474 703a 2f2f 2465 6e64 706f 696e   http://$endpoin
-00025380: 7420 7c20 6772 6570 2022 4869 2c20 6e65  t | grep "Hi, ne
-00025390: 7720 536b 7950 696c 6f74 2068 6572 6521  w SkyPilot here!
-000253a0: 223b 2064 6f20 736c 6565 7020 323b 2064  "; do sleep 2; d
-000253b0: 6f6e 653b 270a 2020 2020 2020 2020 2020  one;'.          
-000253c0: 2020 2320 4d61 6b65 2073 7572 6520 7468    # Make sure th
-000253d0: 6520 7472 6166 6669 6320 6973 206e 6f74  e traffic is not
-000253e0: 206d 6978 6564 0a20 2020 2020 2020 2020   mixed.         
-000253f0: 2020 2027 6375 726c 202d 4c20 6874 7470     'curl -L http
-00025400: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
-00025410: 7265 7020 2248 692c 206e 6577 2053 6b79  rep "Hi, new Sky
-00025420: 5069 6c6f 7420 6865 7265 2227 2c0a 2020  Pilot here"',.  
-00025430: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
-00025440: 6c61 7465 7374 2032 2076 6572 7369 6f6e  latest 2 version
-00025450: 2073 686f 756c 6420 6265 2052 4541 4459   should be READY
-00025460: 2061 6e64 2074 6865 206f 6c64 6572 2076   and the older v
-00025470: 6572 7369 6f6e 7320 7368 6f75 6c64 2062  ersions should b
-00025480: 6520 7368 7574 7469 6e67 2064 6f77 6e0a  e shutting down.
-00025490: 2020 2020 2020 2020 2020 2020 285f 6368              (_ch
-000254a0: 6563 6b5f 7265 706c 6963 615f 696e 5f73  eck_replica_in_s
-000254b0: 7461 7475 7328 6e61 6d65 2c20 5b28 322c  tatus(name, [(2,
-000254c0: 2046 616c 7365 2c20 2752 4541 4459 2729   False, 'READY')
-000254d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000254e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000254f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00025500: 322c 2046 616c 7365 2c20 2753 4855 5454  2, False, 'SHUTT
-00025510: 494e 475f 444f 574e 2729 5d29 202b 0a20  ING_DOWN')]) +. 
-00025520: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
-00025530: 636b 5f73 6572 7669 6365 5f76 6572 7369  ck_service_versi
-00025540: 6f6e 286e 616d 652c 2022 3222 2929 2c0a  on(name, "2")),.
-00025550: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00025560: 2020 205f 5445 4152 444f 574e 5f53 4552     _TEARDOWN_SER
-00025570: 5649 4345 2e66 6f72 6d61 7428 6e61 6d65  VICE.format(name
-00025580: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
-00025590: 7469 6d65 6f75 743d 3230 202a 2036 302c  timeout=20 * 60,
-000255a0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-000255b0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-000255c0: 4070 7974 6573 742e 6d61 726b 2e73 6572  @pytest.mark.ser
-000255d0: 7665 0a64 6566 2074 6573 745f 736b 7973  ve.def test_skys
-000255e0: 6572 7665 5f72 6f6c 6c69 6e67 5f75 7064  erve_rolling_upd
-000255f0: 6174 6528 6765 6e65 7269 635f 636c 6f75  ate(generic_clou
-00025600: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
-00025610: 5465 7374 2073 6b79 7365 7276 6520 7769  Test skyserve wi
-00025620: 7468 2072 6f6c 6c69 6e67 2075 7064 6174  th rolling updat
-00025630: 6522 2222 0a20 2020 206e 616d 6520 3d20  e""".    name = 
-00025640: 5f67 6574 5f73 6572 7669 6365 5f6e 616d  _get_service_nam
-00025650: 6528 290a 2020 2020 7369 6e67 6c65 5f6e  e().    single_n
-00025660: 6577 5f72 6570 6c69 6361 203d 205f 6368  ew_replica = _ch
-00025670: 6563 6b5f 7265 706c 6963 615f 696e 5f73  eck_replica_in_s
-00025680: 7461 7475 7328 0a20 2020 2020 2020 206e  tatus(.        n
-00025690: 616d 652c 205b 2832 2c20 4661 6c73 652c  ame, [(2, False,
-000256a0: 2027 5245 4144 5927 292c 2028 312c 2046   'READY'), (1, F
-000256b0: 616c 7365 2c20 5f53 4552 5649 4345 5f4c  alse, _SERVICE_L
-000256c0: 4155 4e43 4849 4e47 5f53 5441 5455 535f  AUNCHING_STATUS_
-000256d0: 5245 4745 5829 2c0a 2020 2020 2020 2020  REGEX),.        
-000256e0: 2020 2020 2020 2028 312c 2046 616c 7365         (1, False
-000256f0: 2c20 2753 4855 5454 494e 475f 444f 574e  , 'SHUTTING_DOWN
-00025700: 2729 5d29 0a20 2020 2074 6573 7420 3d20  ')]).    test = 
-00025710: 5465 7374 280a 2020 2020 2020 2020 6627  Test(.        f'
-00025720: 7465 7374 2d73 6b79 7365 7276 652d 726f  test-skyserve-ro
-00025730: 6c6c 696e 672d 7570 6461 7465 272c 0a20  lling-update',. 
-00025740: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00025750: 2020 2020 2066 2773 6b79 2073 6572 7665       f'sky serve
-00025760: 2075 7020 2d6e 207b 6e61 6d65 7d20 2d2d   up -n {name} --
-00025770: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
-00025780: 6c6f 7564 7d20 2d79 2074 6573 7473 2f73  loud} -y tests/s
-00025790: 6b79 7365 7276 652f 7570 6461 7465 2f6f  kyserve/update/o
-000257a0: 6c64 2e79 616d 6c27 2c0a 2020 2020 2020  ld.yaml',.      
-000257b0: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
-000257c0: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
-000257d0: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
-000257e0: 7265 706c 6963 615f 6e75 6d3d 3229 2c0a  replica_num=2),.
-000257f0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00025800: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
-00025810: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
-00025820: 6e61 6d65 297d 3b20 6375 726c 202d 4c20  name)}; curl -L 
-00025830: 6874 7470 3a2f 2f24 656e 6470 6f69 6e74  http://$endpoint
-00025840: 207c 2067 7265 7020 2248 692c 2053 6b79   | grep "Hi, Sky
-00025850: 5069 6c6f 7420 6865 7265 2227 2c0a 2020  Pilot here"',.  
-00025860: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-00025870: 7365 7276 6520 7570 6461 7465 207b 6e61  serve update {na
-00025880: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
-00025890: 6572 6963 5f63 6c6f 7564 7d20 2d79 2074  eric_cloud} -y t
-000258a0: 6573 7473 2f73 6b79 7365 7276 652f 7570  ests/skyserve/up
-000258b0: 6461 7465 2f6e 6577 2e79 616d 6c27 2c0a  date/new.yaml',.
-000258c0: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
-000258d0: 6b65 2073 7572 6520 7468 6520 7472 6166  ke sure the traf
-000258e0: 6669 6320 6973 206d 6978 6564 2061 6372  fic is mixed acr
-000258f0: 6f73 7320 7477 6f20 7665 7273 696f 6e73  oss two versions
-00025900: 2c20 7468 6520 7265 706c 6963 6173 0a20  , the replicas. 
-00025910: 2020 2020 2020 2020 2020 2023 2077 6974             # wit
-00025920: 6820 6576 656e 2069 6420 7769 6c6c 2073  h even id will s
-00025930: 6c65 6570 2036 3020 7365 636f 6e64 7320  leep 60 seconds 
-00025940: 6265 666f 7265 2062 6569 6e67 2072 6561  before being rea
-00025950: 6479 2c20 736f 2077 650a 2020 2020 2020  dy, so we.      
-00025960: 2020 2020 2020 2320 7368 6f75 6c64 2062        # should b
-00025970: 6520 6162 6c65 2074 6f20 6765 7420 6f62  e able to get ob
-00025980: 7365 7276 6520 7468 6520 7065 7269 6f64  serve the period
-00025990: 2074 6861 7420 7468 6520 7472 6166 6669   that the traffi
-000259a0: 6320 6973 206d 6978 6564 0a20 2020 2020  c is mixed.     
-000259b0: 2020 2020 2020 2023 2061 6372 6f73 7320         # across 
-000259c0: 7477 6f20 7665 7273 696f 6e73 2e0a 2020  two versions..  
-000259d0: 2020 2020 2020 2020 2020 6627 7b5f 5345            f'{_SE
-000259e0: 5256 455f 454e 4450 4f49 4e54 5f57 4149  RVE_ENDPOINT_WAI
-000259f0: 542e 666f 726d 6174 286e 616d 653d 6e61  T.format(name=na
-00025a00: 6d65 297d 3b20 270a 2020 2020 2020 2020  me)}; '.        
-00025a10: 2020 2020 2775 6e74 696c 2063 7572 6c20      'until curl 
-00025a20: 2d4c 2068 7474 703a 2f2f 2465 6e64 706f  -L http://$endpo
-00025a30: 696e 7420 7c20 6772 6570 2022 4869 2c20  int | grep "Hi, 
-00025a40: 6e65 7720 536b 7950 696c 6f74 2068 6572  new SkyPilot her
-00025a50: 6521 223b 2064 6f20 736c 6565 7020 323b  e!"; do sleep 2;
-00025a60: 2064 6f6e 653b 2073 6c65 6570 2032 3b20   done; sleep 2; 
-00025a70: 270a 2020 2020 2020 2020 2020 2020 2320  '.            # 
-00025a80: 5468 6520 6c61 7465 7374 2076 6572 7369  The latest versi
-00025a90: 6f6e 2073 686f 756c 6420 6861 7665 206f  on should have o
-00025aa0: 6e65 2052 4541 4459 2061 6e64 2074 6865  ne READY and the
-00025ab0: 206f 6e65 206f 6620 7468 6520 6f6c 6465   one of the olde
-00025ac0: 7220 7665 7273 696f 6e73 2073 686f 756c  r versions shoul
-00025ad0: 6420 6265 2073 6875 7474 696e 6720 646f  d be shutting do
-00025ae0: 776e 0a20 2020 2020 2020 2020 2020 2066  wn.            f
-00025af0: 277b 7369 6e67 6c65 5f6e 6577 5f72 6570  '{single_new_rep
-00025b00: 6c69 6361 7d20 7b5f 6368 6563 6b5f 7365  lica} {_check_se
-00025b10: 7276 6963 655f 7665 7273 696f 6e28 6e61  rvice_version(na
-00025b20: 6d65 2c20 2231 2c32 2229 7d20 270a 2020  me, "1,2")} '.  
-00025b30: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
-00025b40: 6b20 7468 6520 6f75 7470 7574 2066 726f  k the output fro
-00025b50: 6d20 7468 6520 6f6c 6420 7665 7273 696f  m the old versio
-00025b60: 6e2c 2069 6d6d 6564 6961 7465 6c79 2061  n, immediately a
-00025b70: 6674 6572 2074 6865 0a20 2020 2020 2020  fter the.       
-00025b80: 2020 2020 2023 206f 7574 7075 7420 6672       # output fr
-00025b90: 6f6d 2074 6865 206e 6577 2076 6572 7369  om the new versi
-00025ba0: 6f6e 2061 7070 6561 7273 2e20 5468 6973  on appears. This
-00025bb0: 2069 7320 6775 6172 616e 7465 6564 2062   is guaranteed b
-00025bc0: 7920 7468 650a 2020 2020 2020 2020 2020  y the.          
-00025bd0: 2020 2320 726f 756e 6420 726f 6269 6e20    # round robin 
-00025be0: 6c6f 6164 2062 616c 616e 6369 6e67 2070  load balancing p
-00025bf0: 6f6c 6963 792e 0a20 2020 2020 2020 2020  olicy..         
-00025c00: 2020 2023 2054 4f44 4f28 7a68 7775 293a     # TODO(zhwu):
-00025c10: 2077 6520 7368 6f75 6c64 2068 6176 6520   we should have 
-00025c20: 6120 6d6f 7265 2067 656e 6572 616c 697a  a more generaliz
-00025c30: 6564 2077 6179 2066 6f72 2063 6865 636b  ed way for check
-00025c40: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
-00025c50: 2020 2020 2320 6d69 7865 6420 7665 7273      # mixed vers
-00025c60: 696f 6e20 6f66 2072 6570 6c69 6361 7320  ion of replicas 
-00025c70: 746f 2061 766f 6964 2064 6570 656e 6469  to avoid dependi
-00025c80: 6e67 206f 6e20 7468 6520 7370 6563 6966  ng on the specif
-00025c90: 6963 0a20 2020 2020 2020 2020 2020 2023  ic.            #
-00025ca0: 2072 6f75 6e64 2072 6f62 696e 206c 6f61   round robin loa
-00025cb0: 6420 6261 6c61 6e63 696e 6720 706f 6c69  d balancing poli
-00025cc0: 6379 2e0a 2020 2020 2020 2020 2020 2020  cy..            
-00025cd0: 2763 7572 6c20 2d4c 2068 7474 703a 2f2f  'curl -L http://
-00025ce0: 2465 6e64 706f 696e 7420 7c20 6772 6570  $endpoint | grep
-00025cf0: 2022 4869 2c20 536b 7950 696c 6f74 2068   "Hi, SkyPilot h
-00025d00: 6572 6522 272c 0a20 2020 2020 2020 205d  ere"',.        ]
-00025d10: 2c0a 2020 2020 2020 2020 5f54 4541 5244  ,.        _TEARD
-00025d20: 4f57 4e5f 5345 5256 4943 452e 666f 726d  OWN_SERVICE.form
-00025d30: 6174 286e 616d 653d 6e61 6d65 292c 0a20  at(name=name),. 
-00025d40: 2020 2020 2020 2074 696d 656f 7574 3d32         timeout=2
-00025d50: 3020 2a20 3630 2c0a 2020 2020 290a 2020  0 * 60,.    ).  
-00025d60: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-00025d70: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
-00025d80: 6172 6b2e 7365 7276 650a 6465 6620 7465  ark.serve.def te
-00025d90: 7374 5f73 6b79 7365 7276 655f 6661 7374  st_skyserve_fast
-00025da0: 5f75 7064 6174 6528 6765 6e65 7269 635f  _update(generic_
-00025db0: 636c 6f75 643a 2073 7472 293a 0a20 2020  cloud: str):.   
-00025dc0: 2022 2222 5465 7374 2073 6b79 7365 7276   """Test skyserv
-00025dd0: 6520 7769 7468 2066 6173 7420 7570 6461  e with fast upda
-00025de0: 7465 2028 496e 6372 656d 656e 7420 7665  te (Increment ve
-00025df0: 7273 696f 6e20 6f66 206f 6c64 2072 6570  rsion of old rep
-00025e00: 6c69 6361 7329 2222 220a 2020 2020 6e61  licas)""".    na
-00025e10: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
-00025e20: 655f 6e61 6d65 2829 0a0a 2020 2020 7465  e_name()..    te
-00025e30: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
-00025e40: 2020 2066 2774 6573 742d 736b 7973 6572     f'test-skyser
-00025e50: 7665 2d66 6173 742d 7570 6461 7465 272c  ve-fast-update',
-00025e60: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
-00025e70: 2020 2020 2020 2066 2773 6b79 2073 6572         f'sky ser
-00025e80: 7665 2075 7020 2d6e 207b 6e61 6d65 7d20  ve up -n {name} 
-00025e90: 2d79 202d 2d63 6c6f 7564 207b 6765 6e65  -y --cloud {gene
-00025ea0: 7269 635f 636c 6f75 647d 2074 6573 7473  ric_cloud} tests
-00025eb0: 2f73 6b79 7365 7276 652f 7570 6461 7465  /skyserve/update
-00025ec0: 2f62 756d 705f 7665 7273 696f 6e5f 6265  /bump_version_be
-00025ed0: 666f 7265 2e79 616d 6c27 2c0a 2020 2020  fore.yaml',.    
-00025ee0: 2020 2020 2020 2020 5f53 4552 5645 5f57          _SERVE_W
-00025ef0: 4149 545f 554e 5449 4c5f 5245 4144 592e  AIT_UNTIL_READY.
-00025f00: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
-00025f10: 2c20 7265 706c 6963 615f 6e75 6d3d 3229  , replica_num=2)
-00025f20: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00025f30: 7b5f 5345 5256 455f 454e 4450 4f49 4e54  {_SERVE_ENDPOINT
-00025f40: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
-00025f50: 653d 6e61 6d65 297d 3b20 6375 726c 202d  e=name)}; curl -
-00025f60: 4c20 6874 7470 3a2f 2f24 656e 6470 6f69  L http://$endpoi
-00025f70: 6e74 207c 2067 7265 7020 2248 692c 2053  nt | grep "Hi, S
-00025f80: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
-00025f90: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00025fa0: 7920 7365 7276 6520 7570 6461 7465 207b  y serve update {
-00025fb0: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
-00025fc0: 656e 6572 6963 5f63 6c6f 7564 7d20 2d2d  eneric_cloud} --
-00025fd0: 6d6f 6465 2062 6c75 655f 6772 6565 6e20  mode blue_green 
-00025fe0: 2d79 2074 6573 7473 2f73 6b79 7365 7276  -y tests/skyserv
-00025ff0: 652f 7570 6461 7465 2f62 756d 705f 7665  e/update/bump_ve
-00026000: 7273 696f 6e5f 6166 7465 722e 7961 6d6c  rsion_after.yaml
-00026010: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
-00026020: 2073 6c65 6570 2074 6f20 7761 6974 2066   sleep to wait f
-00026030: 6f72 2075 7064 6174 6520 746f 2062 6520  or update to be 
-00026040: 7265 6769 7374 6572 6564 2e0a 2020 2020  registered..    
-00026050: 2020 2020 2020 2020 2773 6c65 6570 2033          'sleep 3
-00026060: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00026070: 2320 3220 6f6e 2d64 6561 6d6e 6420 2872  # 2 on-deamnd (r
-00026080: 6561 6479 2920 2b20 3120 6f6e 2d64 656d  eady) + 1 on-dem
-00026090: 616e 6420 2870 726f 7669 7369 6f6e 696e  and (provisionin
-000260a0: 6729 2e0a 2020 2020 2020 2020 2020 2020  g)..            
-000260b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000260c0: 2020 5f63 6865 636b 5f72 6570 6c69 6361    _check_replica
-000260d0: 5f69 6e5f 7374 6174 7573 280a 2020 2020  _in_status(.    
-000260e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000260f0: 6e61 6d65 2c20 5b28 322c 2046 616c 7365  name, [(2, False
-00026100: 2c20 2752 4541 4459 2729 2c0a 2020 2020  , 'READY'),.    
-00026110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026120: 2020 2020 2020 2028 312c 2046 616c 7365         (1, False
-00026130: 2c20 5f53 4552 5649 4345 5f4c 4155 4e43  , _SERVICE_LAUNC
-00026140: 4849 4e47 5f53 5441 5455 535f 5245 4745  HING_STATUS_REGE
-00026150: 5829 5d29 202b 0a20 2020 2020 2020 2020  X)]) +.         
-00026160: 2020 2020 2020 2023 2046 6173 7420 7570         # Fast up
-00026170: 6461 7465 2077 696c 6c20 6469 7265 6374  date will direct
-00026180: 6c79 2068 6176 6520 7468 6520 6c61 7465  ly have the late
-00026190: 7374 2076 6572 7369 6f6e 2072 6561 6479  st version ready
-000261a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000261b0: 2020 5f63 6865 636b 5f73 6572 7669 6365    _check_service
-000261c0: 5f76 6572 7369 6f6e 286e 616d 652c 2022  _version(name, "
-000261d0: 3222 2929 2c0a 2020 2020 2020 2020 2020  2")),.          
-000261e0: 2020 5f53 4552 5645 5f57 4149 545f 554e    _SERVE_WAIT_UN
-000261f0: 5449 4c5f 5245 4144 592e 666f 726d 6174  TIL_READY.format
-00026200: 286e 616d 653d 6e61 6d65 2c20 7265 706c  (name=name, repl
-00026210: 6963 615f 6e75 6d3d 3329 202b 0a20 2020  ica_num=3) +.   
-00026220: 2020 2020 2020 2020 205f 6368 6563 6b5f           _check_
-00026230: 7365 7276 6963 655f 7665 7273 696f 6e28  service_version(
-00026240: 6e61 6d65 2c20 2232 2229 2c0a 2020 2020  name, "2"),.    
-00026250: 2020 2020 2020 2020 6627 7b5f 5345 5256          f'{_SERV
-00026260: 455f 454e 4450 4f49 4e54 5f57 4149 542e  E_ENDPOINT_WAIT.
-00026270: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
-00026280: 297d 3b20 6375 726c 202d 4c20 6874 7470  )}; curl -L http
-00026290: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
-000262a0: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
-000262b0: 7420 6865 7265 2227 2c0a 2020 2020 2020  t here"',.      
-000262c0: 2020 2020 2020 2320 5465 7374 2072 6f6c        # Test rol
-000262d0: 6c69 6e67 2075 7064 6174 650a 2020 2020  ling update.    
-000262e0: 2020 2020 2020 2020 6627 736b 7920 7365          f'sky se
-000262f0: 7276 6520 7570 6461 7465 207b 6e61 6d65  rve update {name
-00026300: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
-00026310: 6963 5f63 6c6f 7564 7d20 2d79 2074 6573  ic_cloud} -y tes
-00026320: 7473 2f73 6b79 7365 7276 652f 7570 6461  ts/skyserve/upda
-00026330: 7465 2f62 756d 705f 7665 7273 696f 6e5f  te/bump_version_
-00026340: 6265 666f 7265 2e79 616d 6c27 2c0a 2020  before.yaml',.  
-00026350: 2020 2020 2020 2020 2020 2320 736c 6565            # slee
-00026360: 7020 746f 2077 6169 7420 666f 7220 7570  p to wait for up
-00026370: 6461 7465 2074 6f20 6265 2072 6567 6973  date to be regis
-00026380: 7465 7265 642e 0a20 2020 2020 2020 2020  tered..         
-00026390: 2020 2027 736c 6565 7020 3135 272c 0a20     'sleep 15',. 
-000263a0: 2020 2020 2020 2020 2020 2023 2032 206f             # 2 o
-000263b0: 6e2d 6465 616d 6e64 2028 7265 6164 7929  n-deamnd (ready)
-000263c0: 202b 2031 206f 6e2d 6465 6d61 6e64 2028   + 1 on-demand (
-000263d0: 7368 7574 7469 6e67 2064 6f77 6e29 2e0a  shutting down)..
-000263e0: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
-000263f0: 636b 5f72 6570 6c69 6361 5f69 6e5f 7374  ck_replica_in_st
-00026400: 6174 7573 286e 616d 652c 205b 2832 2c20  atus(name, [(2, 
-00026410: 4661 6c73 652c 2027 5245 4144 5927 292c  False, 'READY'),
-00026420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026440: 2020 2020 2020 2020 2020 2020 2028 312c               (1,
-00026450: 2046 616c 7365 2c20 2753 4855 5454 494e   False, 'SHUTTIN
-00026460: 475f 444f 574e 2729 5d29 2c0a 2020 2020  G_DOWN')]),.    
-00026470: 2020 2020 2020 2020 5f53 4552 5645 5f57          _SERVE_W
-00026480: 4149 545f 554e 5449 4c5f 5245 4144 592e  AIT_UNTIL_READY.
-00026490: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
-000264a0: 2c20 7265 706c 6963 615f 6e75 6d3d 3229  , replica_num=2)
-000264b0: 202b 0a20 2020 2020 2020 2020 2020 205f   +.            _
-000264c0: 6368 6563 6b5f 7365 7276 6963 655f 7665  check_service_ve
-000264d0: 7273 696f 6e28 6e61 6d65 2c20 2233 2229  rsion(name, "3")
-000264e0: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-000264f0: 7b5f 5345 5256 455f 454e 4450 4f49 4e54  {_SERVE_ENDPOINT
-00026500: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
-00026510: 653d 6e61 6d65 297d 3b20 6375 726c 202d  e=name)}; curl -
-00026520: 4c20 6874 7470 3a2f 2f24 656e 6470 6f69  L http://$endpoi
-00026530: 6e74 207c 2067 7265 7020 2248 692c 2053  nt | grep "Hi, S
-00026540: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
-00026550: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00026560: 2020 205f 5445 4152 444f 574e 5f53 4552     _TEARDOWN_SER
-00026570: 5649 4345 2e66 6f72 6d61 7428 6e61 6d65  VICE.format(name
-00026580: 3d6e 616d 6529 2c0a 2020 2020 2020 2020  =name),.        
-00026590: 7469 6d65 6f75 743d 3330 202a 2036 302c  timeout=30 * 60,
-000265a0: 0a20 2020 2029 0a20 2020 2072 756e 5f6f  .    ).    run_o
-000265b0: 6e65 5f74 6573 7428 7465 7374 290a 0a0a  ne_test(test)...
-000265c0: 4070 7974 6573 742e 6d61 726b 2e73 6572  @pytest.mark.ser
-000265d0: 7665 0a64 6566 2074 6573 745f 736b 7973  ve.def test_skys
-000265e0: 6572 7665 5f75 7064 6174 655f 6175 746f  erve_update_auto
-000265f0: 7363 616c 6528 6765 6e65 7269 635f 636c  scale(generic_cl
-00026600: 6f75 643a 2073 7472 293a 0a20 2020 2022  oud: str):.    "
-00026610: 2222 5465 7374 2073 6b79 7365 7276 6520  ""Test skyserve 
-00026620: 7570 6461 7465 2077 6974 6820 6175 746f  update with auto
-00026630: 7363 616c 6522 2222 0a20 2020 206e 616d  scale""".    nam
-00026640: 6520 3d20 5f67 6574 5f73 6572 7669 6365  e = _get_service
-00026650: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-00026660: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-00026670: 2066 2774 6573 742d 736b 7973 6572 7665   f'test-skyserve
-00026680: 2d75 7064 6174 652d 6175 746f 7363 616c  -update-autoscal
-00026690: 6527 2c0a 2020 2020 2020 2020 5b0a 2020  e',.        [.  
-000266a0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
-000266b0: 7365 7276 6520 7570 202d 6e20 7b6e 616d  serve up -n {nam
-000266c0: 657d 202d 2d63 6c6f 7564 207b 6765 6e65  e} --cloud {gene
-000266d0: 7269 635f 636c 6f75 647d 202d 7920 7465  ric_cloud} -y te
-000266e0: 7374 732f 736b 7973 6572 7665 2f75 7064  sts/skyserve/upd
-000266f0: 6174 652f 6e75 6d5f 6d69 6e5f 7477 6f2e  ate/num_min_two.
-00026700: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
-00026710: 2020 205f 5345 5256 455f 5741 4954 5f55     _SERVE_WAIT_U
-00026720: 4e54 494c 5f52 4541 4459 2e66 6f72 6d61  NTIL_READY.forma
-00026730: 7428 6e61 6d65 3d6e 616d 652c 2072 6570  t(name=name, rep
-00026740: 6c69 6361 5f6e 756d 3d32 2920 2b0a 2020  lica_num=2) +.  
-00026750: 2020 2020 2020 2020 2020 5f63 6865 636b            _check
-00026760: 5f73 6572 7669 6365 5f76 6572 7369 6f6e  _service_version
-00026770: 286e 616d 652c 2022 3122 292c 0a20 2020  (name, "1"),.   
-00026780: 2020 2020 2020 2020 2066 277b 5f53 4552           f'{_SER
-00026790: 5645 5f45 4e44 504f 494e 545f 5741 4954  VE_ENDPOINT_WAIT
-000267a0: 2e66 6f72 6d61 7428 6e61 6d65 3d6e 616d  .format(name=nam
-000267b0: 6529 7d3b 2027 0a20 2020 2020 2020 2020  e)}; '.         
-000267c0: 2020 2027 6375 726c 202d 4c20 6874 7470     'curl -L http
-000267d0: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
-000267e0: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
-000267f0: 7420 6865 7265 2227 2c0a 2020 2020 2020  t here"',.      
-00026800: 2020 2020 2020 6627 736b 7920 7365 7276        f'sky serv
-00026810: 6520 7570 6461 7465 207b 6e61 6d65 7d20  e update {name} 
-00026820: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
-00026830: 5f63 6c6f 7564 7d20 2d2d 6d6f 6465 2062  _cloud} --mode b
-00026840: 6c75 655f 6772 6565 6e20 2d79 2074 6573  lue_green -y tes
-00026850: 7473 2f73 6b79 7365 7276 652f 7570 6461  ts/skyserve/upda
-00026860: 7465 2f6e 756d 5f6d 696e 5f6f 6e65 2e79  te/num_min_one.y
-00026870: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
-00026880: 2020 2320 736c 6565 7020 6265 666f 7265    # sleep before
-00026890: 2075 7064 6174 6520 6973 2072 6567 6973   update is regis
-000268a0: 7465 7265 642e 0a20 2020 2020 2020 2020  tered..         
-000268b0: 2020 2027 736c 6565 7020 3230 272c 0a20     'sleep 20',. 
-000268c0: 2020 2020 2020 2020 2020 2023 2054 696d             # Tim
-000268d0: 656f 7574 2077 696c 6c20 6265 2074 7269  eout will be tri
-000268e0: 6767 6572 6564 2077 6865 6e20 7570 6461  ggered when upda
-000268f0: 7465 2066 6169 6c73 2e0a 2020 2020 2020  te fails..      
-00026900: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
-00026910: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
-00026920: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
-00026930: 7265 706c 6963 615f 6e75 6d3d 3129 202b  replica_num=1) +
-00026940: 0a20 2020 2020 2020 2020 2020 205f 6368  .            _ch
-00026950: 6563 6b5f 7365 7276 6963 655f 7665 7273  eck_service_vers
-00026960: 696f 6e28 6e61 6d65 2c20 2232 2229 2c0a  ion(name, "2"),.
-00026970: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
-00026980: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
-00026990: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
-000269a0: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
-000269b0: 2020 2020 2020 2763 7572 6c20 2d4c 2068        'curl -L h
-000269c0: 7474 703a 2f2f 2465 6e64 706f 696e 7420  ttp://$endpoint 
-000269d0: 7c20 6772 6570 2022 4869 2c20 536b 7950  | grep "Hi, SkyP
-000269e0: 696c 6f74 2068 6572 6521 2227 2c0a 2020  ilot here!"',.  
-000269f0: 2020 2020 2020 2020 2020 2320 526f 6c6c            # Roll
-00026a00: 696e 6720 5570 6461 7465 0a20 2020 2020  ing Update.     
-00026a10: 2020 2020 2020 2066 2773 6b79 2073 6572         f'sky ser
-00026a20: 7665 2075 7064 6174 6520 7b6e 616d 657d  ve update {name}
-00026a30: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
-00026a40: 635f 636c 6f75 647d 202d 7920 7465 7374  c_cloud} -y test
-00026a50: 732f 736b 7973 6572 7665 2f75 7064 6174  s/skyserve/updat
-00026a60: 652f 6e75 6d5f 6d69 6e5f 7477 6f2e 7961  e/num_min_two.ya
-00026a70: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
-00026a80: 2023 2073 6c65 6570 2062 6566 6f72 6520   # sleep before 
-00026a90: 7570 6461 7465 2069 7320 7265 6769 7374  update is regist
-00026aa0: 6572 6564 2e0a 2020 2020 2020 2020 2020  ered..          
-00026ab0: 2020 2773 6c65 6570 2032 3027 2c0a 2020    'sleep 20',.  
-00026ac0: 2020 2020 2020 2020 2020 2320 5469 6d65            # Time
-00026ad0: 6f75 7420 7769 6c6c 2062 6520 7472 6967  out will be trig
-00026ae0: 6765 7265 6420 7768 656e 2075 7064 6174  gered when updat
-00026af0: 6520 6661 696c 732e 0a20 2020 2020 2020  e fails..       
-00026b00: 2020 2020 205f 5345 5256 455f 5741 4954       _SERVE_WAIT
-00026b10: 5f55 4e54 494c 5f52 4541 4459 2e66 6f72  _UNTIL_READY.for
-00026b20: 6d61 7428 6e61 6d65 3d6e 616d 652c 2072  mat(name=name, r
-00026b30: 6570 6c69 6361 5f6e 756d 3d32 2920 2b0a  eplica_num=2) +.
-00026b40: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
-00026b50: 636b 5f73 6572 7669 6365 5f76 6572 7369  ck_service_versi
-00026b60: 6f6e 286e 616d 652c 2022 3322 292c 0a20  on(name, "3"),. 
-00026b70: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
-00026b80: 4552 5645 5f45 4e44 504f 494e 545f 5741  ERVE_ENDPOINT_WA
-00026b90: 4954 2e66 6f72 6d61 7428 6e61 6d65 3d6e  IT.format(name=n
-00026ba0: 616d 6529 7d3b 2027 0a20 2020 2020 2020  ame)}; '.       
-00026bb0: 2020 2020 2027 6375 726c 202d 4c20 6874       'curl -L ht
-00026bc0: 7470 3a2f 2f24 656e 6470 6f69 6e74 207c  tp://$endpoint |
-00026bd0: 2067 7265 7020 2248 692c 2053 6b79 5069   grep "Hi, SkyPi
-00026be0: 6c6f 7420 6865 7265 2122 272c 0a20 2020  lot here!"',.   
-00026bf0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00026c00: 5f54 4541 5244 4f57 4e5f 5345 5256 4943  _TEARDOWN_SERVIC
-00026c10: 452e 666f 726d 6174 286e 616d 653d 6e61  E.format(name=na
-00026c20: 6d65 292c 0a20 2020 2020 2020 2074 696d  me),.        tim
-00026c30: 656f 7574 3d33 3020 2a20 3630 2c0a 2020  eout=30 * 60,.  
-00026c40: 2020 290a 2020 2020 7275 6e5f 6f6e 655f    ).    run_one_
-00026c50: 7465 7374 2874 6573 7429 0a0a 0a40 7079  test(test)...@py
-00026c60: 7465 7374 2e6d 6172 6b2e 7365 7276 650a  test.mark.serve.
-00026c70: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-00026c80: 6b75 6265 726e 6574 6573 2020 2320 5370  kubernetes  # Sp
-00026c90: 6f74 2069 6e73 7461 6e63 6573 2061 7265  ot instances are
-00026ca0: 206e 6f74 2073 7570 706f 7274 6564 2069   not supported i
-00026cb0: 6e20 4b75 6265 726e 6574 6573 0a40 7079  n Kubernetes.@py
-00026cc0: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-00026cd0: 7472 697a 6528 276d 6f64 6527 2c20 5b27  trize('mode', ['
-00026ce0: 726f 6c6c 696e 6727 2c20 2762 6c75 655f  rolling', 'blue_
-00026cf0: 6772 6565 6e27 5d29 0a64 6566 2074 6573  green']).def tes
-00026d00: 745f 736b 7973 6572 7665 5f6e 6577 5f61  t_skyserve_new_a
-00026d10: 7574 6f73 6361 6c65 725f 7570 6461 7465  utoscaler_update
-00026d20: 286d 6f64 653a 2073 7472 2c20 6765 6e65  (mode: str, gene
-00026d30: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
-00026d40: 0a20 2020 2022 2222 5465 7374 2073 6b79  .    """Test sky
-00026d50: 7365 7276 6520 7769 7468 2075 7064 6174  serve with updat
-00026d60: 6520 7468 6174 2063 6861 6e67 6573 2061  e that changes a
-00026d70: 7574 6f73 6361 6c65 7222 2222 0a20 2020  utoscaler""".   
-00026d80: 206e 616d 6520 3d20 5f67 6574 5f73 6572   name = _get_ser
-00026d90: 7669 6365 5f6e 616d 6528 2920 2b20 6d6f  vice_name() + mo
-00026da0: 6465 0a0a 2020 2020 666f 7572 5f73 706f  de..    four_spo
-00026db0: 745f 7570 5f63 6d64 203d 205f 6368 6563  t_up_cmd = _chec
-00026dc0: 6b5f 7265 706c 6963 615f 696e 5f73 7461  k_replica_in_sta
-00026dd0: 7475 7328 6e61 6d65 2c20 5b28 342c 2054  tus(name, [(4, T
-00026de0: 7275 652c 2027 5245 4144 5927 295d 290a  rue, 'READY')]).
-00026df0: 2020 2020 7570 6461 7465 5f63 6865 636b      update_check
-00026e00: 203d 205b 6627 756e 7469 6c20 287b 666f   = [f'until ({fo
-00026e10: 7572 5f73 706f 745f 7570 5f63 6d64 7d29  ur_spot_up_cmd})
-00026e20: 3b20 646f 2073 6c65 6570 2035 3b20 646f  ; do sleep 5; do
-00026e30: 6e65 3b20 736c 6565 7020 3130 3b27 5d0a  ne; sleep 10;'].
-00026e40: 2020 2020 6966 206d 6f64 6520 3d3d 2027      if mode == '
-00026e50: 726f 6c6c 696e 6727 3a0a 2020 2020 2020  rolling':.      
-00026e60: 2020 2320 4368 6563 6b20 726f 6c6c 696e    # Check rollin
-00026e70: 6720 7570 6461 7465 2c20 6974 2077 696c  g update, it wil
-00026e80: 6c20 7465 726d 696e 6174 6520 6f6e 6520  l terminate one 
-00026e90: 6f66 2074 6865 206f 6c64 206f 6e2d 6465  of the old on-de
-00026ea0: 6d61 6e64 0a20 2020 2020 2020 2023 2069  mand.        # i
-00026eb0: 6e73 7461 6e63 6573 2c20 6f6e 6365 2074  nstances, once t
-00026ec0: 6865 7265 2061 7265 2034 2073 706f 7420  here are 4 spot 
-00026ed0: 696e 7374 616e 6365 2072 6561 6479 2e0a  instance ready..
-00026ee0: 2020 2020 2020 2020 7570 6461 7465 5f63          update_c
-00026ef0: 6865 636b 202b 3d20 5b0a 2020 2020 2020  heck += [.      
-00026f00: 2020 2020 2020 5f63 6865 636b 5f72 6570        _check_rep
-00026f10: 6c69 6361 5f69 6e5f 7374 6174 7573 280a  lica_in_status(.
-00026f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f30: 6e61 6d65 2c20 5b28 312c 2046 616c 7365  name, [(1, False
-00026f40: 2c20 5f53 4552 5649 4345 5f4c 4155 4e43  , _SERVICE_LAUNC
-00026f50: 4849 4e47 5f53 5441 5455 535f 5245 4745  HING_STATUS_REGE
-00026f60: 5829 2c0a 2020 2020 2020 2020 2020 2020  X),.            
-00026f70: 2020 2020 2020 2020 2020 2028 312c 2046             (1, F
-00026f80: 616c 7365 2c20 2753 4855 5454 494e 475f  alse, 'SHUTTING_
-00026f90: 444f 574e 2729 2c20 2831 2c20 4661 6c73  DOWN'), (1, Fals
-00026fa0: 652c 2027 5245 4144 5927 295d 2920 2b0a  e, 'READY')]) +.
-00026fb0: 2020 2020 2020 2020 2020 2020 5f63 6865              _che
-00026fc0: 636b 5f73 6572 7669 6365 5f76 6572 7369  ck_service_versi
-00026fd0: 6f6e 286e 616d 652c 2022 312c 3222 292c  on(name, "1,2"),
-00026fe0: 0a20 2020 2020 2020 205d 0a20 2020 2065  .        ].    e
-00026ff0: 6c73 653a 0a20 2020 2020 2020 2023 2043  lse:.        # C
-00027000: 6865 636b 2062 6c75 6520 6772 6565 6e20  heck blue green 
-00027010: 7570 6461 7465 2c20 6974 2077 696c 6c20  update, it will 
-00027020: 6b65 6570 2062 6f74 6820 6f6c 6420 6f6e  keep both old on
-00027030: 2d64 656d 616e 6420 696e 7374 616e 6365  -demand instance
-00027040: 730a 2020 2020 2020 2020 2320 7275 6e6e  s.        # runn
-00027050: 696e 672c 206f 6e63 6520 7468 6572 6520  ing, once there 
-00027060: 6172 6520 3420 7370 6f74 2069 6e73 7461  are 4 spot insta
-00027070: 6e63 6520 7265 6164 792e 0a20 2020 2020  nce ready..     
-00027080: 2020 2075 7064 6174 655f 6368 6563 6b20     update_check 
-00027090: 2b3d 205b 0a20 2020 2020 2020 2020 2020  += [.           
-000270a0: 205f 6368 6563 6b5f 7265 706c 6963 615f   _check_replica_
-000270b0: 696e 5f73 7461 7475 7328 0a20 2020 2020  in_status(.     
-000270c0: 2020 2020 2020 2020 2020 206e 616d 652c             name,
-000270d0: 205b 2831 2c20 4661 6c73 652c 205f 5345   [(1, False, _SE
-000270e0: 5256 4943 455f 4c41 554e 4348 494e 475f  RVICE_LAUNCHING_
-000270f0: 5354 4154 5553 5f52 4547 4558 292c 0a20  STATUS_REGEX),. 
-00027100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027110: 2020 2020 2020 2832 2c20 4661 6c73 652c        (2, False,
-00027120: 2027 5245 4144 5927 295d 2920 2b0a 2020   'READY')]) +.  
-00027130: 2020 2020 2020 2020 2020 5f63 6865 636b            _check
-00027140: 5f73 6572 7669 6365 5f76 6572 7369 6f6e  _service_version
-00027150: 286e 616d 652c 2022 3122 292c 0a20 2020  (name, "1"),.   
-00027160: 2020 2020 205d 0a20 2020 2074 6573 7420       ].    test 
-00027170: 3d20 5465 7374 280a 2020 2020 2020 2020  = Test(.        
-00027180: 2774 6573 742d 736b 7973 6572 7665 2d6e  'test-skyserve-n
-00027190: 6577 2d61 7574 6f73 6361 6c65 722d 7570  ew-autoscaler-up
-000271a0: 6461 7465 272c 0a20 2020 2020 2020 205b  date',.        [
-000271b0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-000271c0: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
-000271d0: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
-000271e0: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
-000271f0: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
-00027200: 7570 6461 7465 2f6e 6577 5f61 7574 6f73  update/new_autos
-00027210: 6361 6c65 725f 6265 666f 7265 2e79 616d  caler_before.yam
-00027220: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-00027230: 5f53 4552 5645 5f57 4149 545f 554e 5449  _SERVE_WAIT_UNTI
-00027240: 4c5f 5245 4144 592e 666f 726d 6174 286e  L_READY.format(n
-00027250: 616d 653d 6e61 6d65 2c20 7265 706c 6963  ame=name, replic
-00027260: 615f 6e75 6d3d 3229 202b 0a20 2020 2020  a_num=2) +.     
-00027270: 2020 2020 2020 205f 6368 6563 6b5f 7365         _check_se
-00027280: 7276 6963 655f 7665 7273 696f 6e28 6e61  rvice_version(na
-00027290: 6d65 2c20 2231 2229 2c0a 2020 2020 2020  me, "1"),.      
-000272a0: 2020 2020 2020 6627 7b5f 5345 5256 455f        f'{_SERVE_
-000272b0: 454e 4450 4f49 4e54 5f57 4149 542e 666f  ENDPOINT_WAIT.fo
-000272c0: 726d 6174 286e 616d 653d 6e61 6d65 297d  rmat(name=name)}
-000272d0: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
-000272e0: 2773 3d24 2863 7572 6c20 2d4c 2068 7474  's=$(curl -L htt
-000272f0: 703a 2f2f 2465 6e64 706f 696e 7429 3b20  p://$endpoint); 
-00027300: 6563 686f 2022 2473 223b 2065 6368 6f20  echo "$s"; echo 
-00027310: 2224 7322 207c 2067 7265 7020 2248 692c  "$s" | grep "Hi,
-00027320: 2053 6b79 5069 6c6f 7420 6865 7265 2227   SkyPilot here"'
-00027330: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00027340: 736b 7920 7365 7276 6520 7570 6461 7465  sky serve update
-00027350: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
-00027360: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
-00027370: 2d2d 6d6f 6465 207b 6d6f 6465 7d20 2d79  --mode {mode} -y
-00027380: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
-00027390: 7570 6461 7465 2f6e 6577 5f61 7574 6f73  update/new_autos
-000273a0: 6361 6c65 725f 6166 7465 722e 7961 6d6c  caler_after.yaml
-000273b0: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
-000273c0: 2057 6169 7420 666f 7220 7570 6461 7465   Wait for update
-000273d0: 2074 6f20 6265 2072 6567 6973 7465 7265   to be registere
-000273e0: 640a 2020 2020 2020 2020 2020 2020 6627  d.            f'
-000273f0: 736c 6565 7020 3132 3027 2c0a 2020 2020  sleep 120',.    
-00027400: 2020 2020 2020 2020 5f63 6865 636b 5f72          _check_r
-00027410: 6570 6c69 6361 5f69 6e5f 7374 6174 7573  eplica_in_status
-00027420: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00027430: 2020 6e61 6d65 2c20 5b28 342c 2054 7275    name, [(4, Tru
-00027440: 652c 205f 5345 5256 4943 455f 4c41 554e  e, _SERVICE_LAUN
-00027450: 4348 494e 475f 5354 4154 5553 5f52 4547  CHING_STATUS_REG
-00027460: 4558 202b 2027 5c7c 5245 4144 5927 292c  EX + '\|READY'),
-00027470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027480: 2020 2020 2020 2020 2831 2c20 4661 6c73          (1, Fals
-00027490: 652c 205f 5345 5256 4943 455f 4c41 554e  e, _SERVICE_LAUN
-000274a0: 4348 494e 475f 5354 4154 5553 5f52 4547  CHING_STATUS_REG
-000274b0: 4558 292c 0a20 2020 2020 2020 2020 2020  EX),.           
-000274c0: 2020 2020 2020 2020 2020 2020 2832 2c20              (2, 
-000274d0: 4661 6c73 652c 2027 5245 4144 5927 295d  False, 'READY')]
-000274e0: 292c 0a20 2020 2020 2020 2020 2020 202a  ),.            *
-000274f0: 7570 6461 7465 5f63 6865 636b 2c0a 2020  update_check,.  
-00027500: 2020 2020 2020 2020 2020 5f53 4552 5645            _SERVE
-00027510: 5f57 4149 545f 554e 5449 4c5f 5245 4144  _WAIT_UNTIL_READ
-00027520: 592e 666f 726d 6174 286e 616d 653d 6e61  Y.format(name=na
-00027530: 6d65 2c20 7265 706c 6963 615f 6e75 6d3d  me, replica_num=
-00027540: 3529 2c0a 2020 2020 2020 2020 2020 2020  5),.            
-00027550: 6627 7b5f 5345 5256 455f 454e 4450 4f49  f'{_SERVE_ENDPOI
-00027560: 4e54 5f57 4149 542e 666f 726d 6174 286e  NT_WAIT.format(n
-00027570: 616d 653d 6e61 6d65 297d 3b20 270a 2020  ame=name)}; '.  
-00027580: 2020 2020 2020 2020 2020 2763 7572 6c20            'curl 
-00027590: 2d4c 2068 7474 703a 2f2f 2465 6e64 706f  -L http://$endpo
-000275a0: 696e 7420 7c20 6772 6570 2022 4869 2c20  int | grep "Hi, 
-000275b0: 536b 7950 696c 6f74 2068 6572 6522 272c  SkyPilot here"',
-000275c0: 0a20 2020 2020 2020 2020 2020 205f 6368  .            _ch
-000275d0: 6563 6b5f 7265 706c 6963 615f 696e 5f73  eck_replica_in_s
-000275e0: 7461 7475 7328 6e61 6d65 2c20 5b28 342c  tatus(name, [(4,
-000275f0: 2054 7275 652c 2027 5245 4144 5927 292c   True, 'READY'),
-00027600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027620: 2020 2020 2020 2020 2020 2020 2028 312c               (1,
-00027630: 2046 616c 7365 2c20 2752 4541 4459 2729   False, 'READY')
-00027640: 5d29 2c0a 2020 2020 2020 2020 5d2c 0a20  ]),.        ],. 
-00027650: 2020 2020 2020 205f 5445 4152 444f 574e         _TEARDOWN
-00027660: 5f53 4552 5649 4345 2e66 6f72 6d61 7428  _SERVICE.format(
-00027670: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00027680: 2020 2020 7469 6d65 6f75 743d 3230 202a      timeout=20 *
-00027690: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-000276a0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-000276b0: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-000276c0: 2e73 6572 7665 0a64 6566 2074 6573 745f  .serve.def test_
-000276d0: 736b 7973 6572 7665 5f66 6169 6c75 7265  skyserve_failure
-000276e0: 7328 6765 6e65 7269 635f 636c 6f75 643a  s(generic_cloud:
-000276f0: 2073 7472 293a 0a20 2020 2022 2222 5465   str):.    """Te
-00027700: 7374 2072 6570 6c69 6361 2066 6169 6c75  st replica failu
-00027710: 7265 2073 7461 7475 7365 7322 2222 0a20  re statuses""". 
-00027720: 2020 206e 616d 6520 3d20 5f67 6574 5f73     name = _get_s
-00027730: 6572 7669 6365 5f6e 616d 6528 290a 0a20  ervice_name().. 
-00027740: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
-00027750: 2020 2020 2020 2020 2774 6573 742d 736b          'test-sk
-00027760: 7973 6572 7665 2d66 6169 6c75 7265 7327  yserve-failures'
-00027770: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-00027780: 2020 2020 2020 2020 6627 736b 7920 7365          f'sky se
-00027790: 7276 6520 7570 202d 6e20 7b6e 616d 657d  rve up -n {name}
-000277a0: 202d 2d63 6c6f 7564 207b 6765 6e65 7269   --cloud {generi
-000277b0: 635f 636c 6f75 647d 202d 7920 7465 7374  c_cloud} -y test
-000277c0: 732f 736b 7973 6572 7665 2f66 6169 6c75  s/skyserve/failu
-000277d0: 7265 732f 696e 6974 6961 6c5f 6465 6c61  res/initial_dela
-000277e0: 792e 7961 6d6c 272c 0a20 2020 2020 2020  y.yaml',.       
-000277f0: 2020 2020 2066 2773 3d24 2873 6b79 2073       f's=$(sky s
-00027800: 6572 7665 2073 7461 7475 7320 7b6e 616d  erve status {nam
-00027810: 657d 293b 2027 0a20 2020 2020 2020 2020  e}); '.         
-00027820: 2020 2066 2775 6e74 696c 2065 6368 6f20     f'until echo 
-00027830: 2224 7322 207c 2067 7265 7020 2246 4149  "$s" | grep "FAI
-00027840: 4c45 445f 494e 4954 4941 4c5f 4445 4c41  LED_INITIAL_DELA
-00027850: 5922 3b20 646f 2027 0a20 2020 2020 2020  Y"; do '.       
-00027860: 2020 2020 2027 6563 686f 2022 5761 6974       'echo "Wait
-00027870: 696e 6720 666f 7220 7265 706c 6963 6120  ing for replica 
-00027880: 746f 2062 6520 6661 696c 6564 2e2e 2e22  to be failed..."
-00027890: 3b20 736c 6565 7020 353b 2027 0a20 2020  ; sleep 5; '.   
-000278a0: 2020 2020 2020 2020 2066 2773 3d24 2873           f's=$(s
-000278b0: 6b79 2073 6572 7665 2073 7461 7475 7320  ky serve status 
-000278c0: 7b6e 616d 657d 293b 2065 6368 6f20 2224  {name}); echo "$
-000278d0: 7322 3b20 646f 6e65 3b27 2c0a 2020 2020  s"; done;',.    
-000278e0: 2020 2020 2020 2020 2773 6c65 6570 2036          'sleep 6
-000278f0: 3027 2c0a 2020 2020 2020 2020 2020 2020  0',.            
-00027900: 6627 7b5f 5345 5256 455f 5354 4154 5553  f'{_SERVE_STATUS
-00027910: 5f57 4149 542e 666f 726d 6174 286e 616d  _WAIT.format(nam
-00027920: 653d 6e61 6d65 297d 3b20 6563 686f 2022  e=name)}; echo "
-00027930: 2473 2220 7c20 6772 6570 2022 7b6e 616d  $s" | grep "{nam
-00027940: 657d 2220 7c20 6772 6570 2022 4641 494c  e}" | grep "FAIL
-00027950: 4544 5f49 4e49 5449 414c 5f44 454c 4159  ED_INITIAL_DELAY
-00027960: 2220 7c20 7763 202d 6c20 7c20 6772 6570  " | wc -l | grep
-00027970: 2032 3b20 270a 2020 2020 2020 2020 2020   2; '.          
-00027980: 2020 2320 4d61 6b65 2073 7572 6520 6e6f    # Make sure no
-00027990: 206e 6577 2072 6570 6c69 6361 7320 6172   new replicas ar
-000279a0: 6520 7374 6172 7465 6420 666f 7220 6561  e started for ea
-000279b0: 726c 7920 6661 696c 7572 652e 0a20 2020  rly failure..   
-000279c0: 2020 2020 2020 2020 2066 2765 6368 6f20           f'echo 
-000279d0: 2224 7322 207c 2067 7265 7020 2d41 2031  "$s" | grep -A 1
-000279e0: 3030 2022 5365 7276 6963 6520 5265 706c  00 "Service Repl
-000279f0: 6963 6173 2220 7c20 6772 6570 2022 7b6e  icas" | grep "{n
-00027a00: 616d 657d 2220 7c20 7763 202d 6c20 7c20  ame}" | wc -l | 
-00027a10: 6772 6570 2032 3b27 2c0a 2020 2020 2020  grep 2;',.      
-00027a20: 2020 2020 2020 6627 736b 7920 7365 7276        f'sky serv
-00027a30: 6520 7570 6461 7465 207b 6e61 6d65 7d20  e update {name} 
-00027a40: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
-00027a50: 5f63 6c6f 7564 7d20 2d79 2074 6573 7473  _cloud} -y tests
-00027a60: 2f73 6b79 7365 7276 652f 6661 696c 7572  /skyserve/failur
-00027a70: 6573 2f70 726f 6269 6e67 2e79 616d 6c27  es/probing.yaml'
-00027a80: 2c0a 2020 2020 2020 2020 2020 2020 6627  ,.            f'
-00027a90: 733d 2428 736b 7920 7365 7276 6520 7374  s=$(sky serve st
-00027aa0: 6174 7573 207b 6e61 6d65 7d29 3b20 270a  atus {name}); '.
-00027ab0: 2020 2020 2020 2020 2020 2020 2320 5761              # Wa
-00027ac0: 6974 2066 6f72 2072 6570 6c69 6361 2074  it for replica t
-00027ad0: 6f20 6265 2072 6561 6479 2e0a 2020 2020  o be ready..    
-00027ae0: 2020 2020 2020 2020 6627 756e 7469 6c20          f'until 
-00027af0: 6563 686f 2022 2473 2220 7c20 6772 6570  echo "$s" | grep
-00027b00: 2022 5245 4144 5922 3b20 646f 2027 0a20   "READY"; do '. 
-00027b10: 2020 2020 2020 2020 2020 2027 6563 686f             'echo
-00027b20: 2022 5761 6974 696e 6720 666f 7220 7265   "Waiting for re
-00027b30: 706c 6963 6120 746f 2062 6520 6661 696c  plica to be fail
-00027b40: 6564 2e2e 2e22 3b20 736c 6565 7020 353b  ed..."; sleep 5;
-00027b50: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
-00027b60: 2773 3d24 2873 6b79 2073 6572 7665 2073  's=$(sky serve s
-00027b70: 7461 7475 7320 7b6e 616d 657d 293b 2065  tatus {name}); e
-00027b80: 6368 6f20 2224 7322 3b20 646f 6e65 3b27  cho "$s"; done;'
-00027b90: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-00027ba0: 5761 6974 2066 6f72 2072 6570 6c69 6361  Wait for replica
-00027bb0: 2074 6f20 6368 616e 6765 2074 6f20 4641   to change to FA
-00027bc0: 494c 4544 5f50 524f 4249 4e47 0a20 2020  ILED_PROBING.   
-00027bd0: 2020 2020 2020 2020 2066 2773 3d24 2873           f's=$(s
-00027be0: 6b79 2073 6572 7665 2073 7461 7475 7320  ky serve status 
-00027bf0: 7b6e 616d 657d 293b 2027 0a20 2020 2020  {name}); '.     
-00027c00: 2020 2020 2020 2066 2775 6e74 696c 2065         f'until e
-00027c10: 6368 6f20 2224 7322 207c 2067 7265 7020  cho "$s" | grep 
-00027c20: 2246 4149 4c45 445f 5052 4f42 494e 4722  "FAILED_PROBING"
-00027c30: 3b20 646f 2027 0a20 2020 2020 2020 2020  ; do '.         
-00027c40: 2020 2027 6563 686f 2022 5761 6974 696e     'echo "Waitin
-00027c50: 6720 666f 7220 7265 706c 6963 6120 746f  g for replica to
-00027c60: 2062 6520 6661 696c 6564 2e2e 2e22 3b20   be failed..."; 
-00027c70: 736c 6565 7020 353b 2027 0a20 2020 2020  sleep 5; '.     
-00027c80: 2020 2020 2020 2066 2773 3d24 2873 6b79         f's=$(sky
-00027c90: 2073 6572 7665 2073 7461 7475 7320 7b6e   serve status {n
-00027ca0: 616d 657d 293b 2065 6368 6f20 2224 7322  ame}); echo "$s"
-00027cb0: 3b20 646f 6e65 3b27 202b 0a20 2020 2020  ; done;' +.     
-00027cc0: 2020 2020 2020 205f 6368 6563 6b5f 7265         _check_re
-00027cd0: 706c 6963 615f 696e 5f73 7461 7475 7328  plica_in_status(
-00027ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027cf0: 206e 616d 652c 205b 2831 2c20 4661 6c73   name, [(1, Fals
-00027d00: 652c 2027 4641 494c 4544 5f50 524f 4249  e, 'FAILED_PROBI
-00027d10: 4e47 2729 2c0a 2020 2020 2020 2020 2020  NG'),.          
-00027d20: 2020 2020 2020 2020 2020 2020 2028 312c               (1,
-00027d30: 2046 616c 7365 2c20 5f53 4552 5649 4345   False, _SERVICE
-00027d40: 5f4c 4155 4e43 4849 4e47 5f53 5441 5455  _LAUNCHING_STATU
-00027d50: 535f 5245 4745 5829 5d29 2c0a 2020 2020  S_REGEX)]),.    
-00027d60: 2020 2020 2020 2020 2320 544f 444f 287a          # TODO(z
-00027d70: 6877 7529 3a20 6164 6420 7465 7374 2066  hwu): add test f
-00027d80: 6f72 2046 4149 4c45 445f 5052 4f56 4953  or FAILED_PROVIS
-00027d90: 494f 4e0a 2020 2020 2020 2020 5d2c 0a20  ION.        ],. 
-00027da0: 2020 2020 2020 205f 5445 4152 444f 574e         _TEARDOWN
-00027db0: 5f53 4552 5649 4345 2e66 6f72 6d61 7428  _SERVICE.format(
-00027dc0: 6e61 6d65 3d6e 616d 6529 2c0a 2020 2020  name=name),.    
-00027dd0: 2020 2020 7469 6d65 6f75 743d 3230 202a      timeout=20 *
-00027de0: 2036 302c 0a20 2020 2029 0a20 2020 2072   60,.    ).    r
-00027df0: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00027e00: 290a 0a0a 2320 544f 444f 285a 696d 696e  )...# TODO(Zimin
-00027e10: 672c 2054 6961 6e29 3a20 4164 6420 7465  g, Tian): Add te
-00027e20: 7374 7320 666f 7220 6175 746f 7363 616c  sts for autoscal
-00027e30: 696e 672e 0a0a 0a23 202d 2d2d 2d2d 2d2d  ing....# -------
-00027e40: 2054 6573 7469 6e67 2075 7365 7220 7261   Testing user ra
-00027e50: 7920 636c 7573 7465 7220 2d2d 2d2d 2d2d  y cluster ------
-00027e60: 2d2d 0a64 6566 2074 6573 745f 7573 6572  --.def test_user
-00027e70: 5f72 6179 5f63 6c75 7374 6572 2867 656e  _ray_cluster(gen
-00027e80: 6572 6963 5f63 6c6f 7564 3a20 7374 7229  eric_cloud: str)
-00027e90: 3a0a 2020 2020 6e61 6d65 203d 205f 6765  :.    name = _ge
-00027ea0: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-00027eb0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-00027ec0: 280a 2020 2020 2020 2020 2775 7365 722d  (.        'user-
-00027ed0: 7261 792d 636c 7573 7465 7227 2c0a 2020  ray-cluster',.  
-00027ee0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00027ef0: 2020 2020 6627 736b 7920 6c61 756e 6368      f'sky launch
-00027f00: 202d 7920 2d63 207b 6e61 6d65 7d20 2d2d   -y -c {name} --
-00027f10: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
-00027f20: 6c6f 7564 7d20 2272 6179 2073 7461 7274  loud} "ray start
-00027f30: 202d 2d68 6561 6422 272c 0a20 2020 2020   --head"',.     
-00027f40: 2020 2020 2020 2066 2773 6b79 2065 7865         f'sky exe
-00027f50: 6320 7b6e 616d 657d 2022 6563 686f 2068  c {name} "echo h
-00027f60: 6922 272c 0a20 2020 2020 2020 2020 2020  i"',.           
-00027f70: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
-00027f80: 657d 2031 202d 2d73 7461 7475 7327 2c0a  e} 1 --status',.
-00027f90: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00027fa0: 7920 7374 6174 7573 202d 7220 7b6e 616d  y status -r {nam
-00027fb0: 657d 207c 2067 7265 7020 5550 272c 0a20  e} | grep UP',. 
-00027fc0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
-00027fd0: 2065 7865 6320 7b6e 616d 657d 2022 6563   exec {name} "ec
-00027fe0: 686f 2062 7965 2227 2c0a 2020 2020 2020  ho bye"',.      
-00027ff0: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
-00028000: 207b 6e61 6d65 7d20 3220 2d2d 7374 6174   {name} 2 --stat
-00028010: 7573 272c 0a20 2020 2020 2020 205d 2c0a  us',.        ],.
-00028020: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
-00028030: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
-00028040: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
-00028050: 5f74 6573 7428 7465 7374 290a 0a0a 2320  _test(test)...# 
-00028060: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-00028070: 7468 6520 636f 7265 2041 5049 202d 2d2d  the core API ---
-00028080: 2d2d 2d2d 2d0a 2320 4d6f 7374 206f 6620  -----.# Most of 
-00028090: 7468 6520 636f 7265 2041 5049 7320 6861  the core APIs ha
-000280a0: 7665 2062 6565 6e20 7465 7374 6564 2069  ve been tested i
-000280b0: 6e20 7468 6520 434c 4920 7465 7374 732e  n the CLI tests.
-000280c0: 0a23 2054 6865 7365 2074 6573 7473 2061  .# These tests a
-000280d0: 7265 2066 6f72 2074 6573 7469 6e67 2074  re for testing t
-000280e0: 6865 2072 6574 7572 6e20 7661 6c75 6520  he return value 
-000280f0: 6f66 2074 6865 2041 5049 7320 6e6f 7420  of the APIs not 
-00028100: 6675 6c6c 7920 7573 6564 2069 6e20 434c  fully used in CL
-00028110: 492e 0a0a 0a40 7079 7465 7374 2e6d 6172  I....@pytest.mar
-00028120: 6b2e 6763 700a 6465 6620 7465 7374 5f63  k.gcp.def test_c
-00028130: 6f72 655f 6170 695f 736b 795f 6c61 756e  ore_api_sky_laun
-00028140: 6368 5f65 7865 6328 293a 0a20 2020 206e  ch_exec():.    n
-00028150: 616d 6520 3d20 5f67 6574 5f63 6c75 7374  ame = _get_clust
-00028160: 6572 5f6e 616d 6528 290a 2020 2020 7461  er_name().    ta
-00028170: 736b 203d 2073 6b79 2e54 6173 6b28 7275  sk = sky.Task(ru
-00028180: 6e3d 2277 686f 616d 6922 290a 2020 2020  n="whoami").    
-00028190: 7461 736b 2e73 6574 5f72 6573 6f75 7263  task.set_resourc
-000281a0: 6573 2873 6b79 2e52 6573 6f75 7263 6573  es(sky.Resources
-000281b0: 2863 6c6f 7564 3d73 6b79 2e47 4350 2829  (cloud=sky.GCP()
-000281c0: 2929 0a20 2020 206a 6f62 5f69 642c 2068  )).    job_id, h
-000281d0: 616e 646c 6520 3d20 736b 792e 6c61 756e  andle = sky.laun
-000281e0: 6368 2874 6173 6b2c 2063 6c75 7374 6572  ch(task, cluster
-000281f0: 5f6e 616d 653d 6e61 6d65 290a 2020 2020  _name=name).    
-00028200: 6173 7365 7274 206a 6f62 5f69 6420 3d3d  assert job_id ==
-00028210: 2031 0a20 2020 2061 7373 6572 7420 6861   1.    assert ha
-00028220: 6e64 6c65 2069 7320 6e6f 7420 4e6f 6e65  ndle is not None
-00028230: 0a20 2020 2061 7373 6572 7420 6861 6e64  .    assert hand
-00028240: 6c65 2e63 6c75 7374 6572 5f6e 616d 6520  le.cluster_name 
-00028250: 3d3d 206e 616d 650a 2020 2020 6173 7365  == name.    asse
-00028260: 7274 2068 616e 646c 652e 6c61 756e 6368  rt handle.launch
-00028270: 6564 5f72 6573 6f75 7263 6573 2e63 6c6f  ed_resources.clo
-00028280: 7564 2e69 735f 7361 6d65 5f63 6c6f 7564  ud.is_same_cloud
-00028290: 2873 6b79 2e47 4350 2829 290a 2020 2020  (sky.GCP()).    
-000282a0: 6a6f 625f 6964 5f65 7865 632c 2068 616e  job_id_exec, han
-000282b0: 646c 655f 6578 6563 203d 2073 6b79 2e65  dle_exec = sky.e
-000282c0: 7865 6328 7461 736b 2c20 636c 7573 7465  xec(task, cluste
-000282d0: 725f 6e61 6d65 3d6e 616d 6529 0a20 2020  r_name=name).   
-000282e0: 2061 7373 6572 7420 6a6f 625f 6964 5f65   assert job_id_e
-000282f0: 7865 6320 3d3d 2032 0a20 2020 2061 7373  xec == 2.    ass
-00028300: 6572 7420 6861 6e64 6c65 5f65 7865 6320  ert handle_exec 
-00028310: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-00028320: 6173 7365 7274 2068 616e 646c 655f 6578  assert handle_ex
-00028330: 6563 2e63 6c75 7374 6572 5f6e 616d 6520  ec.cluster_name 
-00028340: 3d3d 206e 616d 650a 2020 2020 6173 7365  == name.    asse
-00028350: 7274 2068 616e 646c 655f 6578 6563 2e6c  rt handle_exec.l
-00028360: 6175 6e63 6865 645f 7265 736f 7572 6365  aunched_resource
-00028370: 732e 636c 6f75 642e 6973 5f73 616d 655f  s.cloud.is_same_
-00028380: 636c 6f75 6428 736b 792e 4743 5028 2929  cloud(sky.GCP())
-00028390: 0a20 2020 2023 2046 6f72 2064 756d 6d79  .    # For dummy
-000283a0: 2074 6173 6b20 2869 2e65 2e20 7461 736b   task (i.e. task
-000283b0: 2e72 756e 2069 7320 4e6f 6e65 292c 2074  .run is None), t
-000283c0: 6865 206a 6f62 2077 6f6e 2774 2062 6520  he job won't be 
-000283d0: 7375 626d 6974 7465 642e 0a20 2020 2064  submitted..    d
-000283e0: 756d 6d79 5f74 6173 6b20 3d20 736b 792e  ummy_task = sky.
-000283f0: 5461 736b 2829 0a20 2020 206a 6f62 5f69  Task().    job_i
-00028400: 645f 6475 6d6d 792c 205f 203d 2073 6b79  d_dummy, _ = sky
-00028410: 2e65 7865 6328 6475 6d6d 795f 7461 736b  .exec(dummy_task
-00028420: 2c20 636c 7573 7465 725f 6e61 6d65 3d6e  , cluster_name=n
-00028430: 616d 6529 0a20 2020 2061 7373 6572 7420  ame).    assert 
-00028440: 6a6f 625f 6964 5f64 756d 6d79 2069 7320  job_id_dummy is 
-00028450: 4e6f 6e65 0a20 2020 2073 6b79 2e64 6f77  None.    sky.dow
-00028460: 6e28 6e61 6d65 290a 0a0a 2320 2d2d 2d2d  n(name)...# ----
-00028470: 2d2d 2d2d 2d2d 2054 6573 7469 6e67 2053  ------ Testing S
-00028480: 746f 7261 6765 202d 2d2d 2d2d 2d2d 2d2d  torage ---------
-00028490: 2d0a 636c 6173 7320 5465 7374 5374 6f72  -.class TestStor
-000284a0: 6167 6557 6974 6843 7265 6465 6e74 6961  ageWithCredentia
-000284b0: 6c73 3a0a 2020 2020 2222 2253 746f 7261  ls:.    """Stora
-000284c0: 6765 2074 6573 7473 2077 6869 6368 2072  ge tests which r
-000284d0: 6571 7569 7265 2063 7265 6465 6e74 6961  equire credentia
-000284e0: 6c73 2061 6e64 206e 6574 776f 726b 2063  ls and network c
-000284f0: 6f6e 6e65 6374 696f 6e22 2222 0a0a 2020  onnection"""..  
-00028500: 2020 4157 535f 494e 5641 4c49 445f 4e41    AWS_INVALID_NA
-00028510: 4d45 5320 3d20 5b0a 2020 2020 2020 2020  MES = [.        
-00028520: 2761 6227 2c20 2023 206c 6573 7320 7468  'ab',  # less th
-00028530: 616e 2033 2063 6861 7261 6374 6572 730a  an 3 characters.
-00028540: 2020 2020 2020 2020 2761 6263 6465 6667          'abcdefg
-00028550: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
-00028560: 7879 7a61 6263 6465 6667 6869 6a6b 6c6d  xyzabcdefghijklm
-00028570: 6e6f 7071 7273 7475 7677 7879 7a61 6263  nopqrstuvwxyzabc
-00028580: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00028590: 7475 7677 7879 7a31 272c 0a20 2020 2020  tuvwxyz1',.     
-000285a0: 2020 2023 206d 6f72 6520 7468 616e 2036     # more than 6
-000285b0: 3320 6368 6172 6163 7465 7273 0a20 2020  3 characters.   
-000285c0: 2020 2020 2027 4162 6364 6566 272c 2020       'Abcdef',  
-000285d0: 2320 636f 6e74 6169 6e73 2061 6e20 7570  # contains an up
-000285e0: 7065 7263 6173 6520 6c65 7474 6572 0a20  percase letter. 
-000285f0: 2020 2020 2020 2027 6162 6320 6465 6627         'abc def'
-00028600: 2c20 2023 2063 6f6e 7461 696e 7320 6120  ,  # contains a 
-00028610: 7370 6163 650a 2020 2020 2020 2020 2761  space.        'a
-00028620: 6263 2e2e 6465 6627 2c20 2023 2074 776f  bc..def',  # two
-00028630: 2061 646a 6163 656e 7420 7065 7269 6f64   adjacent period
-00028640: 730a 2020 2020 2020 2020 2731 3932 2e31  s.        '192.1
-00028650: 3638 2e35 2e34 272c 2020 2320 666f 726d  68.5.4',  # form
-00028660: 6174 7465 6420 6173 2061 6e20 4950 2061  atted as an IP a
-00028670: 6464 7265 7373 0a20 2020 2020 2020 2027  ddress.        '
-00028680: 786e 2d2d 6275 636b 6574 272c 2020 2320  xn--bucket',  # 
-00028690: 7374 6172 7473 2077 6974 6820 2778 6e2d  starts with 'xn-
-000286a0: 2d27 2070 7265 6669 780a 2020 2020 2020  -' prefix.      
-000286b0: 2020 2762 7563 6b65 742d 7333 616c 6961    'bucket-s3alia
-000286c0: 7327 2c20 2023 2065 6e64 7320 7769 7468  s',  # ends with
-000286d0: 2027 2d73 3361 6c69 6173 2720 7375 6666   '-s3alias' suff
-000286e0: 6978 0a20 2020 2020 2020 2027 6275 636b  ix.        'buck
-000286f0: 6574 2d2d 6f6c 2d73 3327 2c20 2023 2065  et--ol-s3',  # e
-00028700: 6e64 7320 7769 7468 2027 2d2d 6f6c 2d73  nds with '--ol-s
-00028710: 3327 2073 7566 6669 780a 2020 2020 2020  3' suffix.      
-00028720: 2020 272e 6162 6327 2c20 2023 2073 7461    '.abc',  # sta
-00028730: 7274 7320 7769 7468 2061 2064 6f74 0a20  rts with a dot. 
-00028740: 2020 2020 2020 2027 6162 632e 272c 2020         'abc.',  
-00028750: 2320 656e 6473 2077 6974 6820 6120 646f  # ends with a do
-00028760: 740a 2020 2020 2020 2020 272d 6162 6327  t.        '-abc'
-00028770: 2c20 2023 2073 7461 7274 7320 7769 7468  ,  # starts with
-00028780: 2061 2068 7970 6865 6e0a 2020 2020 2020   a hyphen.      
-00028790: 2020 2761 6263 2d27 2c20 2023 2065 6e64    'abc-',  # end
-000287a0: 7320 7769 7468 2061 2068 7970 6865 6e0a  s with a hyphen.
-000287b0: 2020 2020 5d0a 0a20 2020 2047 4353 5f49      ]..    GCS_I
-000287c0: 4e56 414c 4944 5f4e 414d 4553 203d 205b  NVALID_NAMES = [
-000287d0: 0a20 2020 2020 2020 2027 6162 272c 2020  .        'ab',  
-000287e0: 2320 6c65 7373 2074 6861 6e20 3320 6368  # less than 3 ch
-000287f0: 6172 6163 7465 7273 0a20 2020 2020 2020  aracters.       
-00028800: 2027 6162 6364 6566 6768 696a 6b6c 6d6e   'abcdefghijklmn
-00028810: 6f70 7172 7374 7576 7778 797a 6162 6364  opqrstuvwxyzabcd
-00028820: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
-00028830: 7576 7778 797a 6162 6364 6566 6768 696a  uvwxyzabcdefghij
-00028840: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
-00028850: 3127 2c0a 2020 2020 2020 2020 2320 6d6f  1',.        # mo
-00028860: 7265 2074 6861 6e20 3633 2063 6861 7261  re than 63 chara
-00028870: 6374 6572 7320 2877 6974 686f 7574 2064  cters (without d
-00028880: 6f74 7329 0a20 2020 2020 2020 2027 4162  ots).        'Ab
-00028890: 6364 6566 272c 2020 2320 636f 6e74 6169  cdef',  # contai
-000288a0: 6e73 2061 6e20 7570 7065 7263 6173 6520  ns an uppercase 
-000288b0: 6c65 7474 6572 0a20 2020 2020 2020 2027  letter.        '
-000288c0: 6162 6320 6465 6627 2c20 2023 2063 6f6e  abc def',  # con
-000288d0: 7461 696e 7320 6120 7370 6163 650a 2020  tains a space.  
-000288e0: 2020 2020 2020 2761 6263 2e2e 6465 6627        'abc..def'
-000288f0: 2c20 2023 2074 776f 2061 646a 6163 656e  ,  # two adjacen
-00028900: 7420 7065 7269 6f64 730a 2020 2020 2020  t periods.      
-00028910: 2020 2761 6263 5f2e 6465 662e 6768 692e    'abc_.def.ghi.
-00028920: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
-00028930: 7a61 6263 6465 6667 6869 6a6b 6c6d 6e6f  zabcdefghijklmno
-00028940: 7071 7273 7475 7677 7879 7a61 6263 6465  pqrstuvwxyzabcde
-00028950: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00028960: 7677 7879 7a31 270a 2020 2020 2020 2020  vwxyz1'.        
-00028970: 2320 4d6f 7265 2074 6861 6e20 3633 2063  # More than 63 c
-00028980: 6861 7261 6374 6572 7320 6265 7477 6565  haracters betwee
-00028990: 6e20 646f 7473 0a20 2020 2020 2020 2027  n dots.        '
-000289a0: 6162 635f 2e64 6566 2e67 6869 2e6a 6b6c  abc_.def.ghi.jkl
-000289b0: 6d6e 6f70 7172 7374 7576 7778 797a 6162  mnopqrstuvwxyzab
-000289c0: 6364 6566 6768 696a 6b6c 6d6e 6f70 7166  cdefghijklmnopqf
-000289d0: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
-000289e0: 7727 202a 2035 2c0a 2020 2020 2020 2020  w' * 5,.        
-000289f0: 2320 6d6f 7265 2074 6861 6e20 3232 3220  # more than 222 
-00028a00: 6368 6172 6163 7465 7273 2028 7769 7468  characters (with
-00028a10: 2064 6f74 7329 0a20 2020 2020 2020 2027   dots).        '
-00028a20: 3139 322e 3136 382e 352e 3427 2c20 2023  192.168.5.4',  #
-00028a30: 2066 6f72 6d61 7474 6564 2061 7320 616e   formatted as an
-00028a40: 2049 5020 6164 6472 6573 730a 2020 2020   IP address.    
-00028a50: 2020 2020 2767 6f6f 6762 7563 6b65 7427      'googbucket'
-00028a60: 2c20 2023 2073 7461 7274 7320 7769 7468  ,  # starts with
-00028a70: 2027 676f 6f67 2720 7072 6566 6978 0a20   'goog' prefix. 
-00028a80: 2020 2020 2020 2027 676f 6f67 6c65 6275         'googlebu
-00028a90: 636b 6574 272c 2020 2320 636f 6e74 6169  cket',  # contai
-00028aa0: 6e73 2027 676f 6f67 6c65 270a 2020 2020  ns 'google'.    
-00028ab0: 2020 2020 2767 3030 676c 6562 7563 6b65      'g00glebucke
-00028ac0: 7427 2c20 2023 2076 6172 6961 6e74 206f  t',  # variant o
-00028ad0: 6620 2767 6f6f 676c 6527 0a20 2020 2020  f 'google'.     
-00028ae0: 2020 2027 676f 3067 6c65 6275 636b 6574     'go0glebucket
-00028af0: 272c 2020 2320 7661 7269 616e 7420 6f66  ',  # variant of
-00028b00: 2027 676f 6f67 6c65 270a 2020 2020 2020   'google'.      
-00028b10: 2020 2767 306f 676c 6562 7563 6b65 7427    'g0oglebucket'
-00028b20: 2c20 2023 2076 6172 6961 6e74 206f 6620  ,  # variant of 
-00028b30: 2767 6f6f 676c 6527 0a20 2020 2020 2020  'google'.       
-00028b40: 2027 2e61 6263 272c 2020 2320 7374 6172   '.abc',  # star
-00028b50: 7473 2077 6974 6820 6120 646f 740a 2020  ts with a dot.  
-00028b60: 2020 2020 2020 2761 6263 2e27 2c20 2023        'abc.',  #
-00028b70: 2065 6e64 7320 7769 7468 2061 2064 6f74   ends with a dot
-00028b80: 0a20 2020 2020 2020 2027 5f61 6263 272c  .        '_abc',
-00028b90: 2020 2320 7374 6172 7473 2077 6974 6820    # starts with 
-00028ba0: 616e 2075 6e64 6572 7363 6f72 650a 2020  an underscore.  
-00028bb0: 2020 2020 2020 2761 6263 5f27 2c20 2023        'abc_',  #
-00028bc0: 2065 6e64 7320 7769 7468 2061 6e20 756e   ends with an un
-00028bd0: 6465 7273 636f 7265 0a20 2020 205d 0a0a  derscore.    ]..
-00028be0: 2020 2020 4942 4d5f 494e 5641 4c49 445f      IBM_INVALID_
-00028bf0: 4e41 4d45 5320 3d20 5b0a 2020 2020 2020  NAMES = [.      
-00028c00: 2020 2761 6227 2c20 2023 206c 6573 7320    'ab',  # less 
-00028c10: 7468 616e 2033 2063 6861 7261 6374 6572  than 3 character
-00028c20: 730a 2020 2020 2020 2020 2761 6263 6465  s.        'abcde
-00028c30: 6667 6869 6a6b 6c6d 6e6f 7071 7273 7475  fghijklmnopqrstu
-00028c40: 7677 7879 7a61 6263 6465 6667 6869 6a6b  vwxyzabcdefghijk
-00028c50: 6c6d 6e6f 7071 7273 7475 7677 7879 7a61  lmnopqrstuvwxyza
-00028c60: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
-00028c70: 7273 7475 7677 7879 7a31 272c 0a20 2020  rstuvwxyz1',.   
-00028c80: 2020 2020 2023 206d 6f72 6520 7468 616e       # more than
-00028c90: 2036 3320 6368 6172 6163 7465 7273 0a20   63 characters. 
-00028ca0: 2020 2020 2020 2027 4162 6364 6566 272c         'Abcdef',
-00028cb0: 2020 2320 636f 6e74 6169 6e73 2061 6e20    # contains an 
-00028cc0: 7570 7065 7263 6173 6520 6c65 7474 6572  uppercase letter
-00028cd0: 0a20 2020 2020 2020 2027 6162 6320 6465  .        'abc de
-00028ce0: 6627 2c20 2023 2063 6f6e 7461 696e 7320  f',  # contains 
-00028cf0: 6120 7370 6163 650a 2020 2020 2020 2020  a space.        
-00028d00: 2761 6263 2e2e 6465 6627 2c20 2023 2074  'abc..def',  # t
-00028d10: 776f 2061 646a 6163 656e 7420 7065 7269  wo adjacent peri
-00028d20: 6f64 730a 2020 2020 2020 2020 2731 3932  ods.        '192
-00028d30: 2e31 3638 2e35 2e34 272c 2020 2320 666f  .168.5.4',  # fo
-00028d40: 726d 6174 7465 6420 6173 2061 6e20 4950  rmatted as an IP
-00028d50: 2061 6464 7265 7373 0a20 2020 2020 2020   address.       
-00028d60: 2027 786e 2d2d 6275 636b 6574 272c 2020   'xn--bucket',  
-00028d70: 2320 7374 6172 7473 2077 6974 6820 2778  # starts with 'x
-00028d80: 6e2d 2d27 2070 7265 6669 780a 2020 2020  n--' prefix.    
-00028d90: 2020 2020 272e 6162 6327 2c20 2023 2073      '.abc',  # s
-00028da0: 7461 7274 7320 7769 7468 2061 2064 6f74  tarts with a dot
-00028db0: 0a20 2020 2020 2020 2027 6162 632e 272c  .        'abc.',
-00028dc0: 2020 2320 656e 6473 2077 6974 6820 6120    # ends with a 
-00028dd0: 646f 740a 2020 2020 2020 2020 272d 6162  dot.        '-ab
-00028de0: 6327 2c20 2023 2073 7461 7274 7320 7769  c',  # starts wi
-00028df0: 7468 2061 2068 7970 6865 6e0a 2020 2020  th a hyphen.    
-00028e00: 2020 2020 2761 6263 2d27 2c20 2023 2065      'abc-',  # e
-00028e10: 6e64 7320 7769 7468 2061 2068 7970 6865  nds with a hyphe
-00028e20: 6e0a 2020 2020 2020 2020 2761 2e2d 6263  n.        'a.-bc
-00028e30: 272c 2020 2320 636f 6e74 6169 6e73 2074  ',  # contains t
-00028e40: 6865 2073 6571 7565 6e63 6520 272e 2d27  he sequence '.-'
-00028e50: 0a20 2020 2020 2020 2027 612d 2e62 6327  .        'a-.bc'
-00028e60: 2c20 2023 2063 6f6e 7461 696e 7320 7468  ,  # contains th
-00028e70: 6520 7365 7175 656e 6365 2027 2d2e 270a  e sequence '-.'.
-00028e80: 2020 2020 2020 2020 2761 2662 6327 2020          'a&bc'  
-00028e90: 2320 636f 6e74 6169 6e73 2073 7065 6369  # contains speci
-00028ea0: 616c 2063 6861 7261 6374 6572 730a 2020  al characters.  
-00028eb0: 2020 2020 2020 2761 625e 6327 2020 2320        'ab^c'  # 
-00028ec0: 636f 6e74 6169 6e73 2073 7065 6369 616c  contains special
-00028ed0: 2063 6861 7261 6374 6572 730a 2020 2020   characters.    
-00028ee0: 5d0a 2020 2020 4749 5449 474e 4f52 455f  ].    GITIGNORE_
-00028ef0: 5359 4e43 5f54 4553 545f 4449 525f 5354  SYNC_TEST_DIR_ST
-00028f00: 5255 4354 5552 4520 3d20 7b0a 2020 2020  RUCTURE = {.    
-00028f10: 2020 2020 2764 6f75 626c 655f 6173 7465      'double_aste
-00028f20: 7269 736b 273a 207b 0a20 2020 2020 2020  risk': {.       
-00028f30: 2020 2020 2027 646f 7562 6c65 5f61 7374       'double_ast
-00028f40: 6572 6973 6b5f 6578 636c 7564 6564 273a  erisk_excluded':
-00028f50: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00028f60: 2020 2027 646f 7562 6c65 5f61 7374 6572     'double_aster
-00028f70: 6973 6b5f 6578 636c 7564 6564 5f64 6972  isk_excluded_dir
-00028f80: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
-00028f90: 2020 2020 2027 6469 725f 6578 636c 7564       'dir_exclud
-00028fa0: 6564 273a 204e 6f6e 652c 0a20 2020 2020  ed': None,.     
-00028fb0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00028fc0: 2020 7d2c 0a20 2020 2020 2020 2027 646f    },.        'do
-00028fd0: 7562 6c65 5f61 7374 6572 6973 6b5f 7061  uble_asterisk_pa
-00028fe0: 7265 6e74 273a 207b 0a20 2020 2020 2020  rent': {.       
-00028ff0: 2020 2020 2027 7061 7265 6e74 273a 207b       'parent': {
-00029000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029010: 2027 616c 736f 5f65 7863 6c75 6465 642e   'also_excluded.
-00029020: 7478 7427 3a20 4e6f 6e65 2c0a 2020 2020  txt': None,.    
-00029030: 2020 2020 2020 2020 2020 2020 2763 6869              'chi
-00029040: 6c64 273a 207b 0a20 2020 2020 2020 2020  ld': {.         
-00029050: 2020 2020 2020 2020 2020 2027 646f 7562             'doub
-00029060: 6c65 5f61 7374 6572 6973 6b5f 7061 7265  le_asterisk_pare
-00029070: 6e74 5f63 6869 6c64 5f65 7863 6c75 6465  nt_child_exclude
-00029080: 642e 7478 7427 3a20 4e6f 6e65 2c0a 2020  d.txt': None,.  
-00029090: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000290a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000290b0: 2027 646f 7562 6c65 5f61 7374 6572 6973   'double_asteris
-000290c0: 6b5f 7061 7265 6e74 5f65 7863 6c75 6465  k_parent_exclude
-000290d0: 642e 7478 7427 3a20 4e6f 6e65 2c0a 2020  d.txt': None,.  
-000290e0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000290f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00029100: 2765 7863 6c75 6465 642e 6c6f 6727 3a20  'excluded.log': 
-00029110: 4e6f 6e65 2c0a 2020 2020 2020 2020 2765  None,.        'e
-00029120: 7863 6c75 6465 645f 6469 7227 3a20 7b0a  xcluded_dir': {.
-00029130: 2020 2020 2020 2020 2020 2020 2765 7863              'exc
-00029140: 6c75 6465 642e 7478 7427 3a20 4e6f 6e65  luded.txt': None
-00029150: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-00029160: 6573 7465 645f 6578 636c 7564 6564 273a  ested_excluded':
-00029170: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00029180: 2020 2027 6578 636c 7564 6564 273a 204e     'excluded': N
-00029190: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000291a0: 207d 2c0a 2020 2020 2020 2020 7d2c 0a20   },.        },. 
-000291b0: 2020 2020 2020 2027 6578 702d 3127 3a20         'exp-1': 
-000291c0: 7b0a 2020 2020 2020 2020 2020 2020 2762  {.            'b
-000291d0: 655f 6578 636c 7564 6564 273a 204e 6f6e  e_excluded': Non
-000291e0: 652c 0a20 2020 2020 2020 207d 2c0a 2020  e,.        },.  
-000291f0: 2020 2020 2020 2765 7870 2d32 273a 207b        'exp-2': {
-00029200: 0a20 2020 2020 2020 2020 2020 2027 6265  .            'be
-00029210: 5f65 7863 6c75 6465 6427 3a20 4e6f 6e65  _excluded': None
-00029220: 2c0a 2020 2020 2020 2020 7d2c 0a20 2020  ,.        },.   
-00029230: 2020 2020 2027 6672 6f6e 745f 736c 6173       'front_slas
-00029240: 685f 6578 636c 7564 6564 273a 204e 6f6e  h_excluded': Non
-00029250: 652c 0a20 2020 2020 2020 2027 696e 636c  e,.        'incl
-00029260: 7564 6564 2e6c 6f67 273a 204e 6f6e 652c  uded.log': None,
-00029270: 0a20 2020 2020 2020 2027 696e 636c 7564  .        'includ
-00029280: 6564 2e74 7874 273a 204e 6f6e 652c 0a20  ed.txt': None,. 
-00029290: 2020 2020 2020 2027 696e 636c 7564 655f         'include_
-000292a0: 6469 7227 3a20 7b0a 2020 2020 2020 2020  dir': {.        
-000292b0: 2020 2020 2765 7863 6c75 6465 642e 6c6f      'excluded.lo
-000292c0: 6727 3a20 4e6f 6e65 2c0a 2020 2020 2020  g': None,.      
-000292d0: 2020 2020 2020 2769 6e63 6c75 6465 642e        'included.
-000292e0: 6c6f 6727 3a20 4e6f 6e65 2c0a 2020 2020  log': None,.    
-000292f0: 2020 2020 7d2c 0a20 2020 2020 2020 2027      },.        '
-00029300: 6e65 7374 6564 5f64 6f75 626c 655f 6173  nested_double_as
-00029310: 7465 7269 736b 273a 207b 0a20 2020 2020  terisk': {.     
-00029320: 2020 2020 2020 2027 6f6e 6527 3a20 7b0a         'one': {.
-00029330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029340: 2761 6c73 6f5f 6578 636c 7564 652e 7478  'also_exclude.tx
-00029350: 7427 3a20 4e6f 6e65 2c0a 2020 2020 2020  t': None,.      
-00029360: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00029370: 2020 2020 2027 7477 6f27 3a20 7b0a 2020       'two': {.  
-00029380: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00029390: 6c73 6f5f 6578 636c 7564 652e 7478 7427  lso_exclude.txt'
-000293a0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
-000293b0: 2020 2020 7d2c 0a20 2020 2020 2020 207d      },.        }
-000293c0: 2c0a 2020 2020 2020 2020 276e 6573 7465  ,.        'neste
-000293d0: 645f 7769 6c64 6361 7264 5f64 6972 273a  d_wildcard_dir':
-000293e0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-000293f0: 6d6f 6e64 6179 273a 207b 0a20 2020 2020  monday': {.     
-00029400: 2020 2020 2020 2020 2020 2027 616c 736f             'also
-00029410: 5f65 7863 6c75 6465 2e74 7874 273a 204e  _exclude.txt': N
-00029420: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00029430: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00029440: 2774 7565 7364 6179 273a 207b 0a20 2020  'tuesday': {.   
-00029450: 2020 2020 2020 2020 2020 2020 2027 616c               'al
-00029460: 736f 5f65 7863 6c75 6465 2e74 7874 273a  so_exclude.txt':
-00029470: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00029480: 2020 207d 2c0a 2020 2020 2020 2020 7d2c     },.        },
-00029490: 0a20 2020 2020 2020 2027 6e6f 5f73 6c61  .        'no_sla
-000294a0: 7368 5f65 7863 6c75 6465 6427 3a20 4e6f  sh_excluded': No
-000294b0: 6e65 2c0a 2020 2020 2020 2020 276e 6f5f  ne,.        'no_
-000294c0: 736c 6173 685f 7465 7374 7327 3a20 7b0a  slash_tests': {.
-000294d0: 2020 2020 2020 2020 2020 2020 276e 6f5f              'no_
-000294e0: 736c 6173 685f 6578 636c 7564 6564 273a  slash_excluded':
-000294f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00029500: 2020 2027 616c 736f 5f65 7863 6c75 6465     'also_exclude
-00029510: 642e 7478 7427 3a20 4e6f 6e65 2c0a 2020  d.txt': None,.  
-00029520: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00029530: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00029540: 2771 7565 7374 696f 6e5f 6d61 726b 273a  'question_mark':
-00029550: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00029560: 6578 636c 7564 6564 312e 7478 7427 3a20  excluded1.txt': 
-00029570: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00029580: 2020 2765 7863 6c75 6465 6440 2e74 7874    'excluded@.txt
-00029590: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
-000295a0: 207d 2c0a 2020 2020 2020 2020 2773 7175   },.        'squ
-000295b0: 6172 655f 6272 6163 6b65 7427 3a20 7b0a  are_bracket': {.
-000295c0: 2020 2020 2020 2020 2020 2020 2765 7863              'exc
-000295d0: 6c75 6465 6431 2e74 7874 273a 204e 6f6e  luded1.txt': Non
-000295e0: 652c 0a20 2020 2020 2020 207d 2c0a 2020  e,.        },.  
-000295f0: 2020 2020 2020 2773 7175 6172 655f 6272        'square_br
-00029600: 6163 6b65 745f 616c 7068 6127 3a20 7b0a  acket_alpha': {.
-00029610: 2020 2020 2020 2020 2020 2020 2765 7863              'exc
-00029620: 6c75 6465 647a 2e74 7874 273a 204e 6f6e  ludedz.txt': Non
-00029630: 652c 0a20 2020 2020 2020 207d 2c0a 2020  e,.        },.  
-00029640: 2020 2020 2020 2773 7175 6172 655f 6272        'square_br
-00029650: 6163 6b65 745f 6578 636c 6127 3a20 7b0a  acket_excla': {.
-00029660: 2020 2020 2020 2020 2020 2020 2765 7863              'exc
-00029670: 6c75 6465 6432 2e74 7874 273a 204e 6f6e  luded2.txt': Non
-00029680: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-00029690: 6578 636c 7564 6564 402e 7478 7427 3a20  excluded@.txt': 
-000296a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7d2c  None,.        },
-000296b0: 0a20 2020 2020 2020 2027 7371 7561 7265  .        'square
-000296c0: 5f62 7261 636b 6574 5f73 696e 676c 6527  _bracket_single'
-000296d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000296e0: 2765 7863 6c75 6465 6430 2e74 7874 273a  'excluded0.txt':
-000296f0: 204e 6f6e 652c 0a20 2020 2020 2020 207d   None,.        }
-00029700: 2c0a 2020 2020 7d0a 0a20 2020 2040 7374  ,.    }..    @st
-00029710: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00029720: 6566 2063 7265 6174 655f 6469 725f 7374  ef create_dir_st
-00029730: 7275 6374 7572 6528 6261 7365 5f70 6174  ructure(base_pat
-00029740: 682c 2073 7472 7563 7475 7265 293a 0a20  h, structure):. 
-00029750: 2020 2020 2020 2023 2063 7265 6174 6573         # creates
-00029760: 2061 2067 6976 656e 2066 696c 6520 5354   a given file ST
-00029770: 5255 4354 5552 4520 696e 2042 4153 455f  RUCTURE in BASE_
-00029780: 5041 5448 0a20 2020 2020 2020 2066 6f72  PATH.        for
-00029790: 206e 616d 652c 2073 7562 7374 7275 6374   name, substruct
-000297a0: 7572 6520 696e 2073 7472 7563 7475 7265  ure in structure
-000297b0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-000297c0: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
-000297d0: 7061 7468 2e6a 6f69 6e28 6261 7365 5f70  path.join(base_p
-000297e0: 6174 682c 206e 616d 6529 0a20 2020 2020  ath, name).     
-000297f0: 2020 2020 2020 2069 6620 7375 6273 7472         if substr
-00029800: 7563 7475 7265 2069 7320 4e6f 6e65 3a0a  ucture is None:.
-00029810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029820: 2320 4372 6561 7465 2061 2066 696c 650a  # Create a file.
-00029830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029840: 6f70 656e 2870 6174 682c 2027 6127 2c20  open(path, 'a', 
-00029850: 656e 636f 6469 6e67 3d27 7574 662d 3827  encoding='utf-8'
-00029860: 292e 636c 6f73 6528 290a 2020 2020 2020  ).close().      
-00029870: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00029880: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
-00029890: 6561 7465 2061 2073 7562 6469 7265 6374  eate a subdirect
-000298a0: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
-000298b0: 2020 2020 6f73 2e6d 6b64 6972 2870 6174      os.mkdir(pat
-000298c0: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
-000298d0: 2020 2054 6573 7453 746f 7261 6765 5769     TestStorageWi
-000298e0: 7468 4372 6564 656e 7469 616c 732e 6372  thCredentials.cr
-000298f0: 6561 7465 5f64 6972 5f73 7472 7563 7475  eate_dir_structu
-00029900: 7265 280a 2020 2020 2020 2020 2020 2020  re(.            
-00029910: 2020 2020 2020 2020 7061 7468 2c20 7375          path, su
-00029920: 6273 7472 7563 7475 7265 290a 0a20 2020  bstructure)..   
-00029930: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00029940: 2020 2064 6566 2063 6c69 5f64 656c 6574     def cli_delet
-00029950: 655f 636d 6428 7374 6f72 655f 7479 7065  e_cmd(store_type
-00029960: 2c20 6275 636b 6574 5f6e 616d 6529 3a0a  , bucket_name):.
-00029970: 2020 2020 2020 2020 6966 2073 746f 7265          if store
-00029980: 5f74 7970 6520 3d3d 2073 746f 7261 6765  _type == storage
-00029990: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
-000299a0: 333a 0a20 2020 2020 2020 2020 2020 2075  3:.            u
-000299b0: 726c 203d 2066 2773 333a 2f2f 7b62 7563  rl = f's3://{buc
-000299c0: 6b65 745f 6e61 6d65 7d27 0a20 2020 2020  ket_name}'.     
-000299d0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-000299e0: 6177 7320 7333 2072 6220 7b75 726c 7d20  aws s3 rb {url} 
-000299f0: 2d2d 666f 7263 6527 0a20 2020 2020 2020  --force'.       
-00029a00: 2069 6620 7374 6f72 655f 7479 7065 203d   if store_type =
-00029a10: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
-00029a20: 6f72 6554 7970 652e 4743 533a 0a20 2020  oreType.GCS:.   
-00029a30: 2020 2020 2020 2020 2075 726c 203d 2066           url = f
-00029a40: 2767 733a 2f2f 7b62 7563 6b65 745f 6e61  'gs://{bucket_na
-00029a50: 6d65 7d27 0a20 2020 2020 2020 2020 2020  me}'.           
-00029a60: 2067 7375 7469 6c5f 616c 6961 732c 2061   gsutil_alias, a
-00029a70: 6c69 6173 5f67 656e 203d 2064 6174 615f  lias_gen = data_
-00029a80: 7574 696c 732e 6765 745f 6773 7574 696c  utils.get_gsutil
-00029a90: 5f63 6f6d 6d61 6e64 2829 0a20 2020 2020  _command().     
-00029aa0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
-00029ab0: 7b61 6c69 6173 5f67 656e 7d3b 207b 6773  {alias_gen}; {gs
-00029ac0: 7574 696c 5f61 6c69 6173 7d20 726d 202d  util_alias} rm -
-00029ad0: 7220 7b75 726c 7d27 0a20 2020 2020 2020  r {url}'.       
-00029ae0: 2069 6620 7374 6f72 655f 7479 7065 203d   if store_type =
-00029af0: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
-00029b00: 6f72 6554 7970 652e 5232 3a0a 2020 2020  oreType.R2:.    
-00029b10: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-00029b20: 5f75 726c 203d 2063 6c6f 7564 666c 6172  _url = cloudflar
-00029b30: 652e 6372 6561 7465 5f65 6e64 706f 696e  e.create_endpoin
-00029b40: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00029b50: 7572 6c20 3d20 6627 7333 3a2f 2f7b 6275  url = f's3://{bu
-00029b60: 636b 6574 5f6e 616d 657d 270a 2020 2020  cket_name}'.    
-00029b70: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00029b80: 2741 5753 5f53 4841 5245 445f 4352 4544  'AWS_SHARED_CRED
-00029b90: 454e 5449 414c 535f 4649 4c45 3d7b 636c  ENTIALS_FILE={cl
-00029ba0: 6f75 6466 6c61 7265 2e52 325f 4352 4544  oudflare.R2_CRED
-00029bb0: 454e 5449 414c 535f 5041 5448 7d20 6177  ENTIALS_PATH} aw
-00029bc0: 7320 7333 2072 6220 7b75 726c 7d20 2d2d  s s3 rb {url} --
-00029bd0: 666f 7263 6520 2d2d 656e 6470 6f69 6e74  force --endpoint
-00029be0: 207b 656e 6470 6f69 6e74 5f75 726c 7d20   {endpoint_url} 
-00029bf0: 2d2d 7072 6f66 696c 653d 7232 270a 2020  --profile=r2'.  
-00029c00: 2020 2020 2020 6966 2073 746f 7265 5f74        if store_t
-00029c10: 7970 6520 3d3d 2073 746f 7261 6765 5f6c  ype == storage_l
-00029c20: 6962 2e53 746f 7265 5479 7065 2e49 424d  ib.StoreType.IBM
-00029c30: 3a0a 2020 2020 2020 2020 2020 2020 6275  :.            bu
-00029c40: 636b 6574 5f72 636c 6f6e 655f 7072 6f66  cket_rclone_prof
-00029c50: 696c 6520 3d20 5263 6c6f 6e65 2e67 656e  ile = Rclone.gen
-00029c60: 6572 6174 655f 7263 6c6f 6e65 5f62 7563  erate_rclone_buc
-00029c70: 6b65 745f 7072 6f66 696c 655f 6e61 6d65  ket_profile_name
-00029c80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00029c90: 2020 6275 636b 6574 5f6e 616d 652c 2052    bucket_name, R
-00029ca0: 636c 6f6e 652e 5263 6c6f 6e65 436c 6f75  clone.RcloneClou
-00029cb0: 6473 2e49 424d 290a 2020 2020 2020 2020  ds.IBM).        
-00029cc0: 2020 2020 7265 7475 726e 2066 2772 636c      return f'rcl
-00029cd0: 6f6e 6520 7075 7267 6520 7b62 7563 6b65  one purge {bucke
-00029ce0: 745f 7263 6c6f 6e65 5f70 726f 6669 6c65  t_rclone_profile
-00029cf0: 7d3a 7b62 7563 6b65 745f 6e61 6d65 7d20  }:{bucket_name} 
-00029d00: 2626 2072 636c 6f6e 6520 636f 6e66 6967  && rclone config
-00029d10: 2064 656c 6574 6520 7b62 7563 6b65 745f   delete {bucket_
-00029d20: 7263 6c6f 6e65 5f70 726f 6669 6c65 7d27  rclone_profile}'
-00029d30: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00029d40: 686f 640a 2020 2020 6465 6620 636c 695f  hod.    def cli_
-00029d50: 6c73 5f63 6d64 2873 746f 7265 5f74 7970  ls_cmd(store_typ
-00029d60: 652c 2062 7563 6b65 745f 6e61 6d65 2c20  e, bucket_name, 
-00029d70: 7375 6666 6978 3d27 2729 3a0a 2020 2020  suffix=''):.    
-00029d80: 2020 2020 6966 2073 746f 7265 5f74 7970      if store_typ
-00029d90: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
-00029da0: 2e53 746f 7265 5479 7065 2e53 333a 0a20  .StoreType.S3:. 
-00029db0: 2020 2020 2020 2020 2020 2069 6620 7375             if su
-00029dc0: 6666 6978 3a0a 2020 2020 2020 2020 2020  ffix:.          
-00029dd0: 2020 2020 2020 7572 6c20 3d20 6627 7333        url = f's3
-00029de0: 3a2f 2f7b 6275 636b 6574 5f6e 616d 657d  ://{bucket_name}
-00029df0: 2f7b 7375 6666 6978 7d27 0a20 2020 2020  /{suffix}'.     
-00029e00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00029e10: 2020 2020 2020 2020 2020 2020 2075 726c               url
-00029e20: 203d 2066 2773 333a 2f2f 7b62 7563 6b65   = f's3://{bucke
-00029e30: 745f 6e61 6d65 7d27 0a20 2020 2020 2020  t_name}'.       
-00029e40: 2020 2020 2072 6574 7572 6e20 6627 6177       return f'aw
-00029e50: 7320 7333 206c 7320 7b75 726c 7d27 0a20  s s3 ls {url}'. 
-00029e60: 2020 2020 2020 2069 6620 7374 6f72 655f         if store_
-00029e70: 7479 7065 203d 3d20 7374 6f72 6167 655f  type == storage_
-00029e80: 6c69 622e 5374 6f72 6554 7970 652e 4743  lib.StoreType.GC
-00029e90: 533a 0a20 2020 2020 2020 2020 2020 2069  S:.            i
-00029ea0: 6620 7375 6666 6978 3a0a 2020 2020 2020  f suffix:.      
-00029eb0: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-00029ec0: 6627 6773 3a2f 2f7b 6275 636b 6574 5f6e  f'gs://{bucket_n
-00029ed0: 616d 657d 2f7b 7375 6666 6978 7d27 0a20  ame}/{suffix}'. 
-00029ee0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00029ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00029f00: 2075 726c 203d 2066 2767 733a 2f2f 7b62   url = f'gs://{b
-00029f10: 7563 6b65 745f 6e61 6d65 7d27 0a20 2020  ucket_name}'.   
-00029f20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00029f30: 6627 6773 7574 696c 206c 7320 7b75 726c  f'gsutil ls {url
-00029f40: 7d27 0a20 2020 2020 2020 2069 6620 7374  }'.        if st
-00029f50: 6f72 655f 7479 7065 203d 3d20 7374 6f72  ore_type == stor
-00029f60: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-00029f70: 652e 5232 3a0a 2020 2020 2020 2020 2020  e.R2:.          
-00029f80: 2020 656e 6470 6f69 6e74 5f75 726c 203d    endpoint_url =
-00029f90: 2063 6c6f 7564 666c 6172 652e 6372 6561   cloudflare.crea
-00029fa0: 7465 5f65 6e64 706f 696e 7428 290a 2020  te_endpoint().  
-00029fb0: 2020 2020 2020 2020 2020 6966 2073 7566            if suf
-00029fc0: 6669 783a 0a20 2020 2020 2020 2020 2020  fix:.           
-00029fd0: 2020 2020 2075 726c 203d 2066 2773 333a       url = f's3:
-00029fe0: 2f2f 7b62 7563 6b65 745f 6e61 6d65 7d2f  //{bucket_name}/
-00029ff0: 7b73 7566 6669 787d 270a 2020 2020 2020  {suffix}'.      
-0002a000: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0002a010: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
-0002a020: 3d20 6627 7333 3a2f 2f7b 6275 636b 6574  = f's3://{bucket
-0002a030: 5f6e 616d 657d 270a 2020 2020 2020 2020  _name}'.        
-0002a040: 2020 2020 7265 7475 726e 2066 2741 5753      return f'AWS
-0002a050: 5f53 4841 5245 445f 4352 4544 454e 5449  _SHARED_CREDENTI
-0002a060: 414c 535f 4649 4c45 3d7b 636c 6f75 6466  ALS_FILE={cloudf
-0002a070: 6c61 7265 2e52 325f 4352 4544 454e 5449  lare.R2_CREDENTI
-0002a080: 414c 535f 5041 5448 7d20 6177 7320 7333  ALS_PATH} aws s3
-0002a090: 206c 7320 7b75 726c 7d20 2d2d 656e 6470   ls {url} --endp
-0002a0a0: 6f69 6e74 207b 656e 6470 6f69 6e74 5f75  oint {endpoint_u
-0002a0b0: 726c 7d20 2d2d 7072 6f66 696c 653d 7232  rl} --profile=r2
-0002a0c0: 270a 2020 2020 2020 2020 6966 2073 746f  '.        if sto
-0002a0d0: 7265 5f74 7970 6520 3d3d 2073 746f 7261  re_type == stora
-0002a0e0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
-0002a0f0: 2e49 424d 3a0a 2020 2020 2020 2020 2020  .IBM:.          
-0002a100: 2020 6275 636b 6574 5f72 636c 6f6e 655f    bucket_rclone_
-0002a110: 7072 6f66 696c 6520 3d20 5263 6c6f 6e65  profile = Rclone
-0002a120: 2e67 656e 6572 6174 655f 7263 6c6f 6e65  .generate_rclone
-0002a130: 5f62 7563 6b65 745f 7072 6f66 696c 655f  _bucket_profile_
-0002a140: 6e61 6d65 280a 2020 2020 2020 2020 2020  name(.          
-0002a150: 2020 2020 2020 6275 636b 6574 5f6e 616d        bucket_nam
-0002a160: 652c 2052 636c 6f6e 652e 5263 6c6f 6e65  e, Rclone.Rclone
-0002a170: 436c 6f75 6473 2e49 424d 290a 2020 2020  Clouds.IBM).    
-0002a180: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0002a190: 2772 636c 6f6e 6520 6c73 207b 6275 636b  'rclone ls {buck
-0002a1a0: 6574 5f72 636c 6f6e 655f 7072 6f66 696c  et_rclone_profil
-0002a1b0: 657d 3a7b 6275 636b 6574 5f6e 616d 657d  e}:{bucket_name}
-0002a1c0: 2f7b 7375 6666 6978 7d27 0a0a 2020 2020  /{suffix}'..    
-0002a1d0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-0002a1e0: 2020 6465 6620 636c 695f 7265 6769 6f6e    def cli_region
-0002a1f0: 5f63 6d64 2873 746f 7265 5f74 7970 652c  _cmd(store_type,
-0002a200: 2062 7563 6b65 745f 6e61 6d65 293a 0a20   bucket_name):. 
-0002a210: 2020 2020 2020 2069 6620 7374 6f72 655f         if store_
-0002a220: 7479 7065 203d 3d20 7374 6f72 6167 655f  type == storage_
-0002a230: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
-0002a240: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002a250: 7475 726e 2028 2761 7773 2073 3361 7069  turn ('aws s3api
-0002a260: 2067 6574 2d62 7563 6b65 742d 6c6f 6361   get-bucket-loca
-0002a270: 7469 6f6e 2027 0a20 2020 2020 2020 2020  tion '.         
-0002a280: 2020 2020 2020 2020 2020 2066 272d 2d62             f'--b
-0002a290: 7563 6b65 7420 7b62 7563 6b65 745f 6e61  ucket {bucket_na
-0002a2a0: 6d65 7d20 2d2d 6f75 7470 7574 2074 6578  me} --output tex
-0002a2b0: 7427 290a 2020 2020 2020 2020 656c 6966  t').        elif
-0002a2c0: 2073 746f 7265 5f74 7970 6520 3d3d 2073   store_type == s
-0002a2d0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0002a2e0: 5479 7065 2e47 4353 3a0a 2020 2020 2020  Type.GCS:.      
-0002a2f0: 2020 2020 2020 7265 7475 726e 2028 6627        return (f'
-0002a300: 6773 7574 696c 206c 7320 2d4c 202d 6220  gsutil ls -L -b 
-0002a310: 6773 3a2f 2f7b 6275 636b 6574 5f6e 616d  gs://{bucket_nam
-0002a320: 657d 2f20 7c20 270a 2020 2020 2020 2020  e}/ | '.        
-0002a330: 2020 2020 2020 2020 2020 2020 2767 7265              'gre
-0002a340: 7020 224c 6f63 6174 696f 6e20 636f 6e73  p "Location cons
-0002a350: 7472 6169 6e74 2220 7c20 270a 2020 2020  traint" | '.    
-0002a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a370: 2761 776b 205c 277b 7072 696e 7420 746f  'awk \'{print to
-0002a380: 6c6f 7765 7228 244e 4629 7d5c 2727 290a  lower($NF)}\'').
-0002a390: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0002a3a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0002a3b0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-0002a3c0: 726f 7228 6627 5265 6769 6f6e 2063 6f6d  ror(f'Region com
-0002a3d0: 6d61 6e64 206e 6f74 2069 6d70 6c65 6d65  mand not impleme
-0002a3e0: 6e74 6564 2066 6f72 2027 0a20 2020 2020  nted for '.     
-0002a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a410: 2066 277b 7374 6f72 655f 7479 7065 7d27   f'{store_type}'
-0002a420: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
-0002a430: 7468 6f64 0a20 2020 2064 6566 2063 6c69  thod.    def cli
-0002a440: 5f63 6f75 6e74 5f6e 616d 655f 696e 5f62  _count_name_in_b
-0002a450: 7563 6b65 7428 7374 6f72 655f 7479 7065  ucket(store_type
-0002a460: 2c20 6275 636b 6574 5f6e 616d 652c 2066  , bucket_name, f
-0002a470: 696c 655f 6e61 6d65 2c20 7375 6666 6978  ile_name, suffix
-0002a480: 3d27 2729 3a0a 2020 2020 2020 2020 6966  =''):.        if
-0002a490: 2073 746f 7265 5f74 7970 6520 3d3d 2073   store_type == s
-0002a4a0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-0002a4b0: 5479 7065 2e53 333a 0a20 2020 2020 2020  Type.S3:.       
-0002a4c0: 2020 2020 2069 6620 7375 6666 6978 3a0a       if suffix:.
-0002a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a4e0: 7265 7475 726e 2066 2761 7773 2073 3361  return f'aws s3a
-0002a4f0: 7069 206c 6973 742d 6f62 6a65 6374 7320  pi list-objects 
-0002a500: 2d2d 6275 636b 6574 2022 7b62 7563 6b65  --bucket "{bucke
-0002a510: 745f 6e61 6d65 7d22 202d 2d70 7265 6669  t_name}" --prefi
-0002a520: 7820 7b73 7566 6669 787d 202d 2d71 7565  x {suffix} --que
-0002a530: 7279 2022 6c65 6e67 7468 2843 6f6e 7465  ry "length(Conte
-0002a540: 6e74 735b 3f63 6f6e 7461 696e 7328 4b65  nts[?contains(Ke
-0002a550: 792c 5c27 7b66 696c 655f 6e61 6d65 7d5c  y,\'{file_name}\
-0002a560: 2729 5d2e 4b65 7929 2227 0a20 2020 2020  ')].Key)"'.     
-0002a570: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0002a580: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0002a590: 7572 6e20 6627 6177 7320 7333 6170 6920  urn f'aws s3api 
-0002a5a0: 6c69 7374 2d6f 626a 6563 7473 202d 2d62  list-objects --b
-0002a5b0: 7563 6b65 7420 227b 6275 636b 6574 5f6e  ucket "{bucket_n
-0002a5c0: 616d 657d 2220 2d2d 7175 6572 7920 226c  ame}" --query "l
-0002a5d0: 656e 6774 6828 436f 6e74 656e 7473 5b3f  ength(Contents[?
-0002a5e0: 636f 6e74 6169 6e73 284b 6579 2c5c 277b  contains(Key,\'{
-0002a5f0: 6669 6c65 5f6e 616d 657d 5c27 295d 2e4b  file_name}\')].K
-0002a600: 6579 2922 270a 2020 2020 2020 2020 656c  ey)"'.        el
-0002a610: 6966 2073 746f 7265 5f74 7970 6520 3d3d  if store_type ==
-0002a620: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-0002a630: 7265 5479 7065 2e47 4353 3a0a 2020 2020  reType.GCS:.    
-0002a640: 2020 2020 2020 2020 6966 2073 7566 6669          if suffi
-0002a650: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-0002a660: 2020 2072 6574 7572 6e20 6627 6773 7574     return f'gsut
-0002a670: 696c 206c 7320 2d72 2067 733a 2f2f 7b62  il ls -r gs://{b
-0002a680: 7563 6b65 745f 6e61 6d65 7d2f 7b73 7566  ucket_name}/{suf
-0002a690: 6669 787d 207c 2067 7265 7020 227b 6669  fix} | grep "{fi
-0002a6a0: 6c65 5f6e 616d 657d 2220 7c20 7763 202d  le_name}" | wc -
-0002a6b0: 6c27 0a20 2020 2020 2020 2020 2020 2065  l'.            e
-0002a6c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0002a6d0: 2020 2020 2072 6574 7572 6e20 6627 6773       return f'gs
-0002a6e0: 7574 696c 206c 7320 2d72 2067 733a 2f2f  util ls -r gs://
-0002a6f0: 7b62 7563 6b65 745f 6e61 6d65 7d20 7c20  {bucket_name} | 
-0002a700: 6772 6570 2022 7b66 696c 655f 6e61 6d65  grep "{file_name
-0002a710: 7d22 207c 2077 6320 2d6c 270a 2020 2020  }" | wc -l'.    
-0002a720: 2020 2020 656c 6966 2073 746f 7265 5f74      elif store_t
-0002a730: 7970 6520 3d3d 2073 746f 7261 6765 5f6c  ype == storage_l
-0002a740: 6962 2e53 746f 7265 5479 7065 2e52 323a  ib.StoreType.R2:
-0002a750: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-0002a760: 706f 696e 745f 7572 6c20 3d20 636c 6f75  point_url = clou
-0002a770: 6466 6c61 7265 2e63 7265 6174 655f 656e  dflare.create_en
-0002a780: 6470 6f69 6e74 2829 0a20 2020 2020 2020  dpoint().       
-0002a790: 2020 2020 2069 6620 7375 6666 6978 3a0a       if suffix:.
-0002a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a7b0: 7265 7475 726e 2066 2741 5753 5f53 4841  return f'AWS_SHA
-0002a7c0: 5245 445f 4352 4544 454e 5449 414c 535f  RED_CREDENTIALS_
-0002a7d0: 4649 4c45 3d7b 636c 6f75 6466 6c61 7265  FILE={cloudflare
-0002a7e0: 2e52 325f 4352 4544 454e 5449 414c 535f  .R2_CREDENTIALS_
-0002a7f0: 5041 5448 7d20 6177 7320 7333 6170 6920  PATH} aws s3api 
-0002a800: 6c69 7374 2d6f 626a 6563 7473 202d 2d62  list-objects --b
-0002a810: 7563 6b65 7420 227b 6275 636b 6574 5f6e  ucket "{bucket_n
-0002a820: 616d 657d 2220 2d2d 7072 6566 6978 207b  ame}" --prefix {
-0002a830: 7375 6666 6978 7d20 2d2d 7175 6572 7920  suffix} --query 
-0002a840: 226c 656e 6774 6828 436f 6e74 656e 7473  "length(Contents
-0002a850: 5b3f 636f 6e74 6169 6e73 284b 6579 2c5c  [?contains(Key,\
-0002a860: 277b 6669 6c65 5f6e 616d 657d 5c27 295d  '{file_name}\')]
-0002a870: 2e4b 6579 2922 202d 2d65 6e64 706f 696e  .Key)" --endpoin
-0002a880: 7420 7b65 6e64 706f 696e 745f 7572 6c7d  t {endpoint_url}
-0002a890: 202d 2d70 726f 6669 6c65 3d72 3227 0a20   --profile=r2'. 
-0002a8a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0002a8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a8c0: 2072 6574 7572 6e20 6627 4157 535f 5348   return f'AWS_SH
-0002a8d0: 4152 4544 5f43 5245 4445 4e54 4941 4c53  ARED_CREDENTIALS
-0002a8e0: 5f46 494c 453d 7b63 6c6f 7564 666c 6172  _FILE={cloudflar
-0002a8f0: 652e 5232 5f43 5245 4445 4e54 4941 4c53  e.R2_CREDENTIALS
-0002a900: 5f50 4154 487d 2061 7773 2073 3361 7069  _PATH} aws s3api
-0002a910: 206c 6973 742d 6f62 6a65 6374 7320 2d2d   list-objects --
-0002a920: 6275 636b 6574 2022 7b62 7563 6b65 745f  bucket "{bucket_
-0002a930: 6e61 6d65 7d22 202d 2d71 7565 7279 2022  name}" --query "
-0002a940: 6c65 6e67 7468 2843 6f6e 7465 6e74 735b  length(Contents[
-0002a950: 3f63 6f6e 7461 696e 7328 4b65 792c 5c27  ?contains(Key,\'
-0002a960: 7b66 696c 655f 6e61 6d65 7d5c 2729 5d2e  {file_name}\')].
-0002a970: 4b65 7929 2220 2d2d 656e 6470 6f69 6e74  Key)" --endpoint
-0002a980: 207b 656e 6470 6f69 6e74 5f75 726c 7d20   {endpoint_url} 
-0002a990: 2d2d 7072 6f66 696c 653d 7232 270a 0a20  --profile=r2'.. 
-0002a9a0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-0002a9b0: 0a20 2020 2064 6566 2063 6c69 5f63 6f75  .    def cli_cou
-0002a9c0: 6e74 5f66 696c 655f 696e 5f62 7563 6b65  nt_file_in_bucke
-0002a9d0: 7428 7374 6f72 655f 7479 7065 2c20 6275  t(store_type, bu
-0002a9e0: 636b 6574 5f6e 616d 6529 3a0a 2020 2020  cket_name):.    
-0002a9f0: 2020 2020 6966 2073 746f 7265 5f74 7970      if store_typ
-0002aa00: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
-0002aa10: 2e53 746f 7265 5479 7065 2e53 333a 0a20  .StoreType.S3:. 
-0002aa20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0002aa30: 6e20 6627 6177 7320 7333 206c 7320 7333  n f'aws s3 ls s3
-0002aa40: 3a2f 2f7b 6275 636b 6574 5f6e 616d 657d  ://{bucket_name}
-0002aa50: 202d 2d72 6563 7572 7369 7665 207c 2077   --recursive | w
-0002aa60: 6320 2d6c 270a 2020 2020 2020 2020 656c  c -l'.        el
-0002aa70: 6966 2073 746f 7265 5f74 7970 6520 3d3d  if store_type ==
-0002aa80: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-0002aa90: 7265 5479 7065 2e47 4353 3a0a 2020 2020  reType.GCS:.    
-0002aaa0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0002aab0: 2767 7375 7469 6c20 6c73 202d 7220 6773  'gsutil ls -r gs
-0002aac0: 3a2f 2f7b 6275 636b 6574 5f6e 616d 657d  ://{bucket_name}
-0002aad0: 2f2a 2a20 7c20 7763 202d 6c27 0a20 2020  /** | wc -l'.   
-0002aae0: 2020 2020 2065 6c69 6620 7374 6f72 655f       elif store_
-0002aaf0: 7479 7065 203d 3d20 7374 6f72 6167 655f  type == storage_
-0002ab00: 6c69 622e 5374 6f72 6554 7970 652e 5232  lib.StoreType.R2
-0002ab10: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
-0002ab20: 6470 6f69 6e74 5f75 726c 203d 2063 6c6f  dpoint_url = clo
-0002ab30: 7564 666c 6172 652e 6372 6561 7465 5f65  udflare.create_e
-0002ab40: 6e64 706f 696e 7428 290a 2020 2020 2020  ndpoint().      
-0002ab50: 2020 2020 2020 7265 7475 726e 2066 2741        return f'A
-0002ab60: 5753 5f53 4841 5245 445f 4352 4544 454e  WS_SHARED_CREDEN
-0002ab70: 5449 414c 535f 4649 4c45 3d7b 636c 6f75  TIALS_FILE={clou
-0002ab80: 6466 6c61 7265 2e52 325f 4352 4544 454e  dflare.R2_CREDEN
-0002ab90: 5449 414c 535f 5041 5448 7d20 6177 7320  TIALS_PATH} aws 
-0002aba0: 7333 206c 7320 7333 3a2f 2f7b 6275 636b  s3 ls s3://{buck
-0002abb0: 6574 5f6e 616d 657d 202d 2d72 6563 7572  et_name} --recur
-0002abc0: 7369 7665 202d 2d65 6e64 706f 696e 7420  sive --endpoint 
-0002abd0: 7b65 6e64 706f 696e 745f 7572 6c7d 202d  {endpoint_url} -
-0002abe0: 2d70 726f 6669 6c65 3d72 3220 7c20 7763  -profile=r2 | wc
-0002abf0: 202d 6c27 0a0a 2020 2020 4070 7974 6573   -l'..    @pytes
-0002ac00: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
-0002ac10: 6620 746d 705f 736f 7572 6365 2873 656c  f tmp_source(sel
-0002ac20: 662c 2074 6d70 5f70 6174 6829 3a0a 2020  f, tmp_path):.  
-0002ac30: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
-0002ac40: 6120 7465 6d70 6f72 6172 7920 6469 7265  a temporary dire
-0002ac50: 6374 6f72 7920 7769 7468 2061 2066 696c  ctory with a fil
-0002ac60: 6520 696e 2069 740a 2020 2020 2020 2020  e in it.        
-0002ac70: 746d 705f 6469 7220 3d20 746d 705f 7061  tmp_dir = tmp_pa
-0002ac80: 7468 202f 2027 746d 702d 736f 7572 6365  th / 'tmp-source
-0002ac90: 270a 2020 2020 2020 2020 746d 705f 6469  '.        tmp_di
-0002aca0: 722e 6d6b 6469 7228 290a 2020 2020 2020  r.mkdir().      
-0002acb0: 2020 746d 705f 6669 6c65 203d 2074 6d70    tmp_file = tmp
-0002acc0: 5f64 6972 202f 2027 746d 702d 6669 6c65  _dir / 'tmp-file
-0002acd0: 270a 2020 2020 2020 2020 746d 705f 6669  '.        tmp_fi
-0002ace0: 6c65 2e77 7269 7465 5f74 6578 7428 2774  le.write_text('t
-0002acf0: 6573 7427 290a 2020 2020 2020 2020 6369  est').        ci
-0002ad00: 7263 6c65 5f6c 696e 6b20 3d20 746d 705f  rcle_link = tmp_
-0002ad10: 6469 7220 2f20 2763 6972 636c 652d 6c69  dir / 'circle-li
-0002ad20: 6e6b 270a 2020 2020 2020 2020 6369 7263  nk'.        circ
-0002ad30: 6c65 5f6c 696e 6b2e 7379 6d6c 696e 6b5f  le_link.symlink_
-0002ad40: 746f 2874 6d70 5f64 6972 2c20 7461 7267  to(tmp_dir, targ
-0002ad50: 6574 5f69 735f 6469 7265 6374 6f72 793d  et_is_directory=
-0002ad60: 5472 7565 290a 2020 2020 2020 2020 7969  True).        yi
-0002ad70: 656c 6420 7374 7228 746d 705f 6469 7229  eld str(tmp_dir)
-0002ad80: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0002ad90: 686f 640a 2020 2020 6465 6620 6765 6e65  hod.    def gene
-0002ada0: 7261 7465 5f62 7563 6b65 745f 6e61 6d65  rate_bucket_name
-0002adb0: 2829 3a0a 2020 2020 2020 2020 2320 4372  ():.        # Cr
-0002adc0: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-0002add0: 7920 6275 636b 6574 206e 616d 650a 2020  y bucket name.  
-0002ade0: 2020 2020 2020 2320 7469 6d65 2e74 696d        # time.tim
-0002adf0: 6528 2920 7265 7475 726e 7320 7661 7279  e() returns vary
-0002ae00: 696e 6720 7072 6563 6973 696f 6e20 6f6e  ing precision on
-0002ae10: 2064 6966 6665 7265 6e74 2073 7973 7465   different syste
-0002ae20: 6d73 2c20 736f 2077 650a 2020 2020 2020  ms, so we.      
-0002ae30: 2020 2320 7265 706c 6163 6520 7468 6520    # replace the 
-0002ae40: 6465 6369 6d61 6c20 706f 696e 7420 616e  decimal point an
-0002ae50: 6420 7573 6520 7768 6174 6576 6572 2070  d use whatever p
-0002ae60: 7265 6369 7369 6f6e 2077 6520 6361 6e20  recision we can 
-0002ae70: 6765 742e 0a20 2020 2020 2020 2074 696d  get..        tim
-0002ae80: 6573 7461 6d70 203d 2073 7472 2874 696d  estamp = str(tim
-0002ae90: 652e 7469 6d65 2829 292e 7265 706c 6163  e.time()).replac
-0002aea0: 6528 272e 272c 2027 2729 0a20 2020 2020  e('.', '').     
-0002aeb0: 2020 2072 6574 7572 6e20 6627 736b 792d     return f'sky-
-0002aec0: 7465 7374 2d7b 7469 6d65 7374 616d 707d  test-{timestamp}
-0002aed0: 270a 0a20 2020 2040 7079 7465 7374 2e66  '..    @pytest.f
-0002aee0: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
-0002aef0: 6d70 5f62 7563 6b65 745f 6e61 6d65 2873  mp_bucket_name(s
-0002af00: 656c 6629 3a0a 2020 2020 2020 2020 7969  elf):.        yi
-0002af10: 656c 6420 7365 6c66 2e67 656e 6572 6174  eld self.generat
-0002af20: 655f 6275 636b 6574 5f6e 616d 6528 290a  e_bucket_name().
-0002af30: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-0002af40: 6f64 0a20 2020 2064 6566 2079 6965 6c64  od.    def yield
-0002af50: 5f73 746f 7261 6765 5f6f 626a 6563 7428  _storage_object(
-0002af60: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0002af70: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-0002af80: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002af90: 2020 2020 2073 6f75 7263 653a 204f 7074       source: Opt
-0002afa0: 696f 6e61 6c5b 7374 6f72 6167 655f 6c69  ional[storage_li
-0002afb0: 622e 5061 7468 5d20 3d20 4e6f 6e65 2c0a  b.Path] = None,.
-0002afc0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-0002afd0: 6573 3a20 4f70 7469 6f6e 616c 5b44 6963  es: Optional[Dic
-0002afe0: 745b 7374 6f72 6167 655f 6c69 622e 5374  t[storage_lib.St
-0002aff0: 6f72 6554 7970 652c 0a20 2020 2020 2020  oreType,.       
-0002b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b010: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-0002b020: 6765 5f6c 6962 2e41 6273 7472 6163 7453  ge_lib.AbstractS
-0002b030: 746f 7265 5d5d 203d 204e 6f6e 652c 0a20  tore]] = None,. 
-0002b040: 2020 2020 2020 2020 2020 2070 6572 7369             persi
-0002b050: 7374 656e 743a 204f 7074 696f 6e61 6c5b  stent: Optional[
-0002b060: 626f 6f6c 5d20 3d20 5472 7565 2c0a 2020  bool] = True,.  
-0002b070: 2020 2020 2020 2020 2020 6d6f 6465 3a20            mode: 
-0002b080: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0002b090: 6167 654d 6f64 6520 3d20 7374 6f72 6167  ageMode = storag
-0002b0a0: 655f 6c69 622e 5374 6f72 6167 654d 6f64  e_lib.StorageMod
-0002b0b0: 652e 4d4f 554e 5429 3a0a 2020 2020 2020  e.MOUNT):.      
-0002b0c0: 2020 2320 4372 6561 7465 7320 6120 7465    # Creates a te
-0002b0d0: 6d70 6f72 6172 7920 7374 6f72 6167 6520  mporary storage 
-0002b0e0: 6f62 6a65 6374 2e20 5374 6f72 6573 206d  object. Stores m
-0002b0f0: 7573 7420 6265 2061 6464 6564 2069 6e20  ust be added in 
-0002b100: 7468 6520 7465 7374 2e0a 2020 2020 2020  the test..      
-0002b110: 2020 7374 6f72 6167 655f 6f62 6a20 3d20    storage_obj = 
-0002b120: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0002b130: 6167 6528 6e61 6d65 3d6e 616d 652c 0a20  age(name=name,. 
-0002b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b160: 2020 2020 2020 2020 2073 6f75 7263 653d           source=
-0002b170: 736f 7572 6365 2c0a 2020 2020 2020 2020  source,.        
-0002b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1a0: 2020 7374 6f72 6573 3d73 746f 7265 732c    stores=stores,
-0002b1b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b1d0: 2020 2020 2020 2020 2020 2070 6572 7369             persi
-0002b1e0: 7374 656e 743d 7065 7273 6973 7465 6e74  stent=persistent
-0002b1f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0002b200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b210: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-0002b220: 3d6d 6f64 6529 0a20 2020 2020 2020 2079  =mode).        y
-0002b230: 6965 6c64 2073 746f 7261 6765 5f6f 626a  ield storage_obj
-0002b240: 0a20 2020 2020 2020 2068 616e 646c 6520  .        handle 
-0002b250: 3d20 676c 6f62 616c 5f75 7365 725f 7374  = global_user_st
-0002b260: 6174 652e 6765 745f 6861 6e64 6c65 5f66  ate.get_handle_f
-0002b270: 726f 6d5f 7374 6f72 6167 655f 6e61 6d65  rom_storage_name
-0002b280: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-0002b290: 6f72 6167 655f 6f62 6a2e 6e61 6d65 290a  orage_obj.name).
-0002b2a0: 2020 2020 2020 2020 6966 2068 616e 646c          if handl
-0002b2b0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0002b2c0: 2049 6620 6861 6e64 6c65 2065 7869 7374   If handle exist
-0002b2d0: 732c 2064 656c 6574 6520 6d61 6e75 616c  s, delete manual
-0002b2e0: 6c79 0a20 2020 2020 2020 2020 2020 2023  ly.            #
-0002b2f0: 2054 4f44 4f28 726f 6d69 6c62 293a 2054   TODO(romilb): T
-0002b300: 6869 7320 6973 2070 6f74 656e 7469 616c  his is potential
-0002b310: 6c79 2072 6973 6b79 202d 2069 6620 7468  ly risky - if th
-0002b320: 6520 6465 6c65 7465 206d 6574 686f 6420  e delete method 
-0002b330: 6861 730a 2020 2020 2020 2020 2020 2020  has.            
-0002b340: 2320 2020 6275 6773 2c20 7468 6973 2063  #   bugs, this c
-0002b350: 616e 2063 6175 7365 2072 6573 6f75 7263  an cause resourc
-0002b360: 6520 6c65 616b 732e 2049 6465 616c 6c79  e leaks. Ideally
-0002b370: 2077 6520 7368 6f75 6c64 206d 616e 7561   we should manua
-0002b380: 6c6c 790a 2020 2020 2020 2020 2020 2020  lly.            
-0002b390: 2320 2020 656a 6563 7420 7374 6f72 6167  #   eject storag
-0002b3a0: 6520 6672 6f6d 2067 6c6f 6261 6c5f 7573  e from global_us
-0002b3b0: 6572 5f73 7461 7465 2061 6e64 2064 656c  er_state and del
-0002b3c0: 6574 6520 7468 6520 6275 636b 6574 2075  ete the bucket u
-0002b3d0: 7369 6e67 0a20 2020 2020 2020 2020 2020  sing.           
-0002b3e0: 2023 2020 2062 6f74 6f33 2064 6972 6563   #   boto3 direc
-0002b3f0: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
-0002b400: 2073 746f 7261 6765 5f6f 626a 2e64 656c   storage_obj.del
-0002b410: 6574 6528 290a 0a20 2020 2040 7079 7465  ete()..    @pyte
-0002b420: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
-0002b430: 6566 2074 6d70 5f73 6372 6174 6368 5f73  ef tmp_scratch_s
-0002b440: 746f 7261 6765 5f6f 626a 2873 656c 662c  torage_obj(self,
-0002b450: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
-0002b460: 293a 0a20 2020 2020 2020 2023 2043 7265  ):.        # Cre
-0002b470: 6174 6573 2061 2073 746f 7261 6765 206f  ates a storage o
-0002b480: 626a 6563 7420 7769 7468 206e 6f20 736f  bject with no so
-0002b490: 7572 6365 2074 6f20 6372 6561 7465 2061  urce to create a
-0002b4a0: 2073 6372 6174 6368 2073 746f 7261 6765   scratch storage
-0002b4b0: 2e0a 2020 2020 2020 2020 2320 5374 6f72  ..        # Stor
-0002b4c0: 6573 206d 7573 7420 6265 2061 6464 6564  es must be added
-0002b4d0: 2069 6e20 7468 6520 7465 7374 2e0a 2020   in the test..  
-0002b4e0: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
-0002b4f0: 2073 656c 662e 7969 656c 645f 7374 6f72   self.yield_stor
-0002b500: 6167 655f 6f62 6a65 6374 286e 616d 653d  age_object(name=
-0002b510: 746d 705f 6275 636b 6574 5f6e 616d 6529  tmp_bucket_name)
-0002b520: 0a0a 2020 2020 4070 7974 6573 742e 6669  ..    @pytest.fi
-0002b530: 7874 7572 650a 2020 2020 6465 6620 746d  xture.    def tm
-0002b540: 705f 6d75 6c74 6970 6c65 5f73 6372 6174  p_multiple_scrat
-0002b550: 6368 5f73 746f 7261 6765 5f6f 626a 2873  ch_storage_obj(s
-0002b560: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-0002b570: 4372 6561 7465 7320 6120 6c69 7374 206f  Creates a list o
-0002b580: 6620 3520 7374 6f72 6167 6520 6f62 6a65  f 5 storage obje
-0002b590: 6374 7320 7769 7468 206e 6f20 736f 7572  cts with no sour
-0002b5a0: 6365 2074 6f20 6372 6561 7465 0a20 2020  ce to create.   
-0002b5b0: 2020 2020 2023 206d 756c 7469 706c 6520       # multiple 
-0002b5c0: 7363 7261 7463 6820 7374 6f72 6167 6573  scratch storages
-0002b5d0: 2e0a 2020 2020 2020 2020 2320 5374 6f72  ..        # Stor
-0002b5e0: 6573 2066 6f72 2065 6163 6820 6f62 6a65  es for each obje
-0002b5f0: 6374 2069 6e20 7468 6520 6c69 7374 206d  ct in the list m
-0002b600: 7573 7420 6265 2061 6464 6564 2069 6e20  ust be added in 
-0002b610: 7468 6520 7465 7374 2e0a 2020 2020 2020  the test..      
-0002b620: 2020 7374 6f72 6167 655f 6d75 6c74 5f6f    storage_mult_o
-0002b630: 626a 203d 205b 5d0a 2020 2020 2020 2020  bj = [].        
-0002b640: 666f 7220 5f20 696e 2072 616e 6765 2835  for _ in range(5
-0002b650: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
-0002b660: 696d 6573 7461 6d70 203d 2073 7472 2874  imestamp = str(t
-0002b670: 696d 652e 7469 6d65 2829 292e 7265 706c  ime.time()).repl
-0002b680: 6163 6528 272e 272c 2027 2729 0a20 2020  ace('.', '').   
-0002b690: 2020 2020 2020 2020 2073 746f 7265 5f6f           store_o
-0002b6a0: 626a 203d 2073 746f 7261 6765 5f6c 6962  bj = storage_lib
-0002b6b0: 2e53 746f 7261 6765 286e 616d 653d 6627  .Storage(name=f'
-0002b6c0: 736b 792d 7465 7374 2d7b 7469 6d65 7374  sky-test-{timest
-0002b6d0: 616d 707d 2729 0a20 2020 2020 2020 2020  amp}').         
-0002b6e0: 2020 2073 746f 7261 6765 5f6d 756c 745f     storage_mult_
-0002b6f0: 6f62 6a2e 6170 7065 6e64 2873 746f 7265  obj.append(store
-0002b700: 5f6f 626a 290a 2020 2020 2020 2020 7969  _obj).        yi
-0002b710: 656c 6420 7374 6f72 6167 655f 6d75 6c74  eld storage_mult
-0002b720: 5f6f 626a 0a20 2020 2020 2020 2066 6f72  _obj.        for
-0002b730: 2073 746f 7261 6765 5f6f 626a 2069 6e20   storage_obj in 
-0002b740: 7374 6f72 6167 655f 6d75 6c74 5f6f 626a  storage_mult_obj
-0002b750: 3a0a 2020 2020 2020 2020 2020 2020 6861  :.            ha
-0002b760: 6e64 6c65 203d 2067 6c6f 6261 6c5f 7573  ndle = global_us
-0002b770: 6572 5f73 7461 7465 2e67 6574 5f68 616e  er_state.get_han
-0002b780: 646c 655f 6672 6f6d 5f73 746f 7261 6765  dle_from_storage
-0002b790: 5f6e 616d 6528 0a20 2020 2020 2020 2020  _name(.         
-0002b7a0: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0002b7b0: 626a 2e6e 616d 6529 0a20 2020 2020 2020  bj.name).       
-0002b7c0: 2020 2020 2069 6620 6861 6e64 6c65 3a0a       if handle:.
-0002b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b7e0: 2320 4966 2068 616e 646c 6520 6578 6973  # If handle exis
-0002b7f0: 7473 2c20 6465 6c65 7465 206d 616e 7561  ts, delete manua
-0002b800: 6c6c 790a 2020 2020 2020 2020 2020 2020  lly.            
-0002b810: 2020 2020 2320 544f 444f 2872 6f6d 696c      # TODO(romil
-0002b820: 6229 3a20 5468 6973 2069 7320 706f 7465  b): This is pote
-0002b830: 6e74 6961 6c6c 7920 7269 736b 7920 2d20  ntially risky - 
-0002b840: 6966 2074 6865 2064 656c 6574 6520 6d65  if the delete me
-0002b850: 7468 6f64 2068 6173 0a20 2020 2020 2020  thod has.       
-0002b860: 2020 2020 2020 2020 2023 2062 7567 732c           # bugs,
-0002b870: 2074 6869 7320 6361 6e20 6361 7573 6520   this can cause 
-0002b880: 7265 736f 7572 6365 206c 6561 6b73 2e20  resource leaks. 
-0002b890: 4964 6561 6c6c 7920 7765 2073 686f 756c  Ideally we shoul
-0002b8a0: 6420 6d61 6e75 616c 6c79 0a20 2020 2020  d manually.     
-0002b8b0: 2020 2020 2020 2020 2020 2023 2065 6a65             # eje
-0002b8c0: 6374 2073 746f 7261 6765 2066 726f 6d20  ct storage from 
-0002b8d0: 676c 6f62 616c 5f75 7365 725f 7374 6174  global_user_stat
-0002b8e0: 6520 616e 6420 6465 6c65 7465 2074 6865  e and delete the
-0002b8f0: 2062 7563 6b65 7420 7573 696e 670a 2020   bucket using.  
-0002b900: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0002b910: 626f 746f 3320 6469 7265 6374 6c79 2e0a  boto3 directly..
-0002b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b930: 7374 6f72 6167 655f 6f62 6a2e 6465 6c65  storage_obj.dele
-0002b940: 7465 2829 0a0a 2020 2020 4070 7974 6573  te()..    @pytes
-0002b950: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
-0002b960: 6620 746d 705f 6d75 6c74 6970 6c65 5f63  f tmp_multiple_c
-0002b970: 7573 746f 6d5f 736f 7572 6365 5f73 746f  ustom_source_sto
-0002b980: 7261 6765 5f6f 626a 2873 656c 6629 3a0a  rage_obj(self):.
-0002b990: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0002b9a0: 7320 6120 6c69 7374 206f 6620 7374 6f72  s a list of stor
-0002b9b0: 6167 6520 6f62 6a65 6374 7320 7769 7468  age objects with
-0002b9c0: 2063 7573 746f 6d20 736f 7572 6365 206e   custom source n
-0002b9d0: 616d 6573 2074 6f0a 2020 2020 2020 2020  ames to.        
-0002b9e0: 2320 6372 6561 7465 206d 756c 7469 706c  # create multipl
-0002b9f0: 6520 7363 7261 7463 6820 7374 6f72 6167  e scratch storag
-0002ba00: 6573 2e0a 2020 2020 2020 2020 2320 5374  es..        # St
-0002ba10: 6f72 6573 2066 6f72 2065 6163 6820 6f62  ores for each ob
-0002ba20: 6a65 6374 2069 6e20 7468 6520 6c69 7374  ject in the list
-0002ba30: 206d 7573 7420 6265 2061 6464 6564 2069   must be added i
-0002ba40: 6e20 7468 6520 7465 7374 2e0a 2020 2020  n the test..    
-0002ba50: 2020 2020 6375 7374 6f6d 5f73 6f75 7263      custom_sourc
-0002ba60: 655f 6e61 6d65 7320 3d20 5b27 2270 6174  e_names = ['"pat
-0002ba70: 6820 5769 7468 2053 7061 6365 7322 272c  h With Spaces"',
-0002ba80: 2027 7061 7468 2057 6974 6820 5370 6163   'path With Spac
-0002ba90: 6573 275d 0a20 2020 2020 2020 2073 746f  es'].        sto
-0002baa0: 7261 6765 5f6d 756c 745f 6f62 6a20 3d20  rage_mult_obj = 
-0002bab0: 5b5d 0a20 2020 2020 2020 2066 6f72 206e  [].        for n
-0002bac0: 616d 6520 696e 2063 7573 746f 6d5f 736f  ame in custom_so
-0002bad0: 7572 6365 5f6e 616d 6573 3a0a 2020 2020  urce_names:.    
-0002bae0: 2020 2020 2020 2020 7372 635f 7061 7468          src_path
-0002baf0: 203d 206f 732e 7061 7468 2e65 7870 616e   = os.path.expan
-0002bb00: 6475 7365 7228 6627 7e2f 7b6e 616d 657d  duser(f'~/{name}
-0002bb10: 2729 0a20 2020 2020 2020 2020 2020 2070  ').            p
-0002bb20: 6174 686c 6962 2e50 6174 6828 7372 635f  athlib.Path(src_
-0002bb30: 7061 7468 292e 6578 7061 6e64 7573 6572  path).expanduser
-0002bb40: 2829 2e6d 6b64 6972 2865 7869 7374 5f6f  ().mkdir(exist_o
-0002bb50: 6b3d 5472 7565 290a 2020 2020 2020 2020  k=True).        
-0002bb60: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
-0002bb70: 7374 7228 7469 6d65 2e74 696d 6528 2929  str(time.time())
-0002bb80: 2e72 6570 6c61 6365 2827 2e27 2c20 2727  .replace('.', ''
-0002bb90: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-0002bba0: 6f72 655f 6f62 6a20 3d20 7374 6f72 6167  ore_obj = storag
-0002bbb0: 655f 6c69 622e 5374 6f72 6167 6528 6e61  e_lib.Storage(na
-0002bbc0: 6d65 3d66 2773 6b79 2d74 6573 742d 7b74  me=f'sky-test-{t
-0002bbd0: 696d 6573 7461 6d70 7d27 2c0a 2020 2020  imestamp}',.    
-0002bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002bc00: 2020 2020 2020 2020 736f 7572 6365 3d73          source=s
-0002bc10: 7263 5f70 6174 6829 0a20 2020 2020 2020  rc_path).       
-0002bc20: 2020 2020 2073 746f 7261 6765 5f6d 756c       storage_mul
-0002bc30: 745f 6f62 6a2e 6170 7065 6e64 2873 746f  t_obj.append(sto
-0002bc40: 7265 5f6f 626a 290a 2020 2020 2020 2020  re_obj).        
-0002bc50: 7969 656c 6420 7374 6f72 6167 655f 6d75  yield storage_mu
-0002bc60: 6c74 5f6f 626a 0a20 2020 2020 2020 2066  lt_obj.        f
-0002bc70: 6f72 2073 746f 7261 6765 5f6f 626a 2069  or storage_obj i
-0002bc80: 6e20 7374 6f72 6167 655f 6d75 6c74 5f6f  n storage_mult_o
-0002bc90: 626a 3a0a 2020 2020 2020 2020 2020 2020  bj:.            
-0002bca0: 6861 6e64 6c65 203d 2067 6c6f 6261 6c5f  handle = global_
-0002bcb0: 7573 6572 5f73 7461 7465 2e67 6574 5f68  user_state.get_h
-0002bcc0: 616e 646c 655f 6672 6f6d 5f73 746f 7261  andle_from_stora
-0002bcd0: 6765 5f6e 616d 6528 0a20 2020 2020 2020  ge_name(.       
-0002bce0: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-0002bcf0: 5f6f 626a 2e6e 616d 6529 0a20 2020 2020  _obj.name).     
-0002bd00: 2020 2020 2020 2069 6620 6861 6e64 6c65         if handle
-0002bd10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002bd20: 2020 7374 6f72 6167 655f 6f62 6a2e 6465    storage_obj.de
-0002bd30: 6c65 7465 2829 0a0a 2020 2020 4070 7974  lete()..    @pyt
-0002bd40: 6573 742e 6669 7874 7572 650a 2020 2020  est.fixture.    
-0002bd50: 6465 6620 746d 705f 6c6f 6361 6c5f 7374  def tmp_local_st
-0002bd60: 6f72 6167 655f 6f62 6a28 7365 6c66 2c20  orage_obj(self, 
-0002bd70: 746d 705f 6275 636b 6574 5f6e 616d 652c  tmp_bucket_name,
-0002bd80: 2074 6d70 5f73 6f75 7263 6529 3a0a 2020   tmp_source):.  
-0002bd90: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
-0002bda0: 6120 7465 6d70 6f72 6172 7920 7374 6f72  a temporary stor
-0002bdb0: 6167 6520 6f62 6a65 6374 2e20 5374 6f72  age object. Stor
-0002bdc0: 6573 206d 7573 7420 6265 2061 6464 6564  es must be added
-0002bdd0: 2069 6e20 7468 6520 7465 7374 2e0a 2020   in the test..  
-0002bde0: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
-0002bdf0: 2073 656c 662e 7969 656c 645f 7374 6f72   self.yield_stor
-0002be00: 6167 655f 6f62 6a65 6374 286e 616d 653d  age_object(name=
-0002be10: 746d 705f 6275 636b 6574 5f6e 616d 652c  tmp_bucket_name,
-0002be20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002be40: 2020 2020 2020 2020 2020 2020 2020 736f                so
-0002be50: 7572 6365 3d74 6d70 5f73 6f75 7263 6529  urce=tmp_source)
-0002be60: 0a0a 2020 2020 4070 7974 6573 742e 6669  ..    @pytest.fi
-0002be70: 7874 7572 650a 2020 2020 6465 6620 746d  xture.    def tm
-0002be80: 705f 6c6f 6361 6c5f 6c69 7374 5f73 746f  p_local_list_sto
-0002be90: 7261 6765 5f6f 626a 2873 656c 662c 2074  rage_obj(self, t
-0002bea0: 6d70 5f62 7563 6b65 745f 6e61 6d65 2c20  mp_bucket_name, 
-0002beb0: 746d 705f 736f 7572 6365 293a 0a20 2020  tmp_source):.   
-0002bec0: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
-0002bed0: 2074 656d 7020 7374 6f72 6167 6520 6f62   temp storage ob
-0002bee0: 6a65 6374 2077 6869 6368 2075 7365 7320  ject which uses 
-0002bef0: 6120 6c69 7374 206f 6620 7061 7468 7320  a list of paths 
-0002bf00: 6173 2073 6f75 7263 652e 0a20 2020 2020  as source..     
-0002bf10: 2020 2023 2053 746f 7265 7320 6d75 7374     # Stores must
-0002bf20: 2062 6520 6164 6465 6420 696e 2074 6865   be added in the
-0002bf30: 2074 6573 742e 2041 6674 6572 2075 706c   test. After upl
-0002bf40: 6f61 642c 2074 6865 2062 7563 6b65 7420  oad, the bucket 
-0002bf50: 7368 6f75 6c64 0a20 2020 2020 2020 2023  should.        #
-0002bf60: 2068 6176 6520 7477 6f20 6669 6c65 7320   have two files 
-0002bf70: 2d20 2f74 6d70 2d66 696c 6520 616e 6420  - /tmp-file and 
-0002bf80: 2f74 6d70 2d73 6f75 7263 652f 746d 702d  /tmp-source/tmp-
-0002bf90: 6669 6c65 0a20 2020 2020 2020 206c 6973  file.        lis
-0002bfa0: 745f 736f 7572 6365 203d 205b 746d 705f  t_source = [tmp_
-0002bfb0: 736f 7572 6365 2c20 746d 705f 736f 7572  source, tmp_sour
-0002bfc0: 6365 202b 2027 2f74 6d70 2d66 696c 6527  ce + '/tmp-file'
-0002bfd0: 5d0a 2020 2020 2020 2020 7969 656c 6420  ].        yield 
-0002bfe0: 6672 6f6d 2073 656c 662e 7969 656c 645f  from self.yield_
-0002bff0: 7374 6f72 6167 655f 6f62 6a65 6374 286e  storage_object(n
-0002c000: 616d 653d 746d 705f 6275 636b 6574 5f6e  ame=tmp_bucket_n
-0002c010: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0002c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c040: 2020 736f 7572 6365 3d6c 6973 745f 736f    source=list_so
-0002c050: 7572 6365 290a 0a20 2020 2040 7079 7465  urce)..    @pyte
-0002c060: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
-0002c070: 6566 2074 6d70 5f62 756c 6b5f 6465 6c5f  ef tmp_bulk_del_
-0002c080: 7374 6f72 6167 655f 6f62 6a28 7365 6c66  storage_obj(self
-0002c090: 2c20 746d 705f 6275 636b 6574 5f6e 616d  , tmp_bucket_nam
-0002c0a0: 6529 3a0a 2020 2020 2020 2020 2320 4372  e):.        # Cr
-0002c0b0: 6561 7465 7320 6120 7465 6d70 6f72 6172  eates a temporar
-0002c0c0: 7920 7374 6f72 6167 6520 6f62 6a65 6374  y storage object
-0002c0d0: 2066 6f72 2074 6573 7469 6e67 2062 756c   for testing bul
-0002c0e0: 6b20 6465 6c65 7469 6f6e 2e0a 2020 2020  k deletion..    
-0002c0f0: 2020 2020 2320 5374 6f72 6573 206d 7573      # Stores mus
-0002c100: 7420 6265 2061 6464 6564 2069 6e20 7468  t be added in th
-0002c110: 6520 7465 7374 2e0a 2020 2020 2020 2020  e test..        
-0002c120: 7769 7468 2074 656d 7066 696c 652e 5465  with tempfile.Te
-0002c130: 6d70 6f72 6172 7944 6972 6563 746f 7279  mporaryDirectory
-0002c140: 2829 2061 7320 746d 7064 6972 3a0a 2020  () as tmpdir:.  
-0002c150: 2020 2020 2020 2020 2020 7375 6270 726f            subpro
-0002c160: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-0002c170: 7428 6627 6d6b 6469 7220 2d70 207b 746d  t(f'mkdir -p {tm
-0002c180: 7064 6972 7d2f 666f 6c64 6572 7b7b 3030  pdir}/folder{{00
-0002c190: 302e 2e32 3535 7d7d 272c 0a20 2020 2020  0..255}}',.     
-0002c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c1b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002c1c0: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
-0002c1d0: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-0002c1e0: 732e 6368 6563 6b5f 6f75 7470 7574 2866  s.check_output(f
-0002c1f0: 2774 6f75 6368 207b 746d 7064 6972 7d2f  'touch {tmpdir}/
-0002c200: 7465 7374 7b7b 3030 302e 2e32 3535 7d7d  test{{000..255}}
-0002c210: 2e74 7874 272c 0a20 2020 2020 2020 2020  .txt',.         
-0002c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c230: 2020 2020 2020 2020 2020 2073 6865 6c6c             shell
-0002c240: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0002c250: 2020 2073 7562 7072 6f63 6573 732e 6368     subprocess.ch
-0002c260: 6563 6b5f 6f75 7470 7574 280a 2020 2020  eck_output(.    
-0002c270: 2020 2020 2020 2020 2020 2020 6627 746f              f'to
-0002c280: 7563 6820 7b74 6d70 6469 727d 2f66 6f6c  uch {tmpdir}/fol
-0002c290: 6465 727b 7b30 3030 2e2e 3235 357d 7d2f  der{{000..255}}/
-0002c2a0: 7465 7374 2e74 7874 272c 2073 6865 6c6c  test.txt', shell
-0002c2b0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0002c2c0: 2020 2079 6965 6c64 2066 726f 6d20 7365     yield from se
-0002c2d0: 6c66 2e79 6965 6c64 5f73 746f 7261 6765  lf.yield_storage
-0002c2e0: 5f6f 626a 6563 7428 6e61 6d65 3d74 6d70  _object(name=tmp
-0002c2f0: 5f62 7563 6b65 745f 6e61 6d65 2c0a 2020  _bucket_name,.  
-0002c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002c330: 6f75 7263 653d 746d 7064 6972 290a 0a20  ource=tmpdir).. 
-0002c340: 2020 2040 7079 7465 7374 2e66 6978 7475     @pytest.fixtu
-0002c350: 7265 0a20 2020 2064 6566 2074 6d70 5f63  re.    def tmp_c
-0002c360: 6f70 795f 6d6e 745f 6578 6973 7469 6e67  opy_mnt_existing
-0002c370: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
-0002c380: 662c 2074 6d70 5f73 6372 6174 6368 5f73  f, tmp_scratch_s
-0002c390: 746f 7261 6765 5f6f 626a 293a 0a20 2020  torage_obj):.   
-0002c3a0: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
-0002c3b0: 2063 6f70 7920 6d6f 756e 7420 7374 6f72   copy mount stor
-0002c3c0: 6167 6520 7768 6963 6820 7265 7573 6573  age which reuses
-0002c3d0: 2061 6e20 6578 6973 7469 6e67 2073 746f   an existing sto
-0002c3e0: 7261 6765 206f 626a 6563 742e 0a20 2020  rage object..   
-0002c3f0: 2020 2020 2074 6d70 5f73 6372 6174 6368       tmp_scratch
-0002c400: 5f73 746f 7261 6765 5f6f 626a 2e61 6464  _storage_obj.add
-0002c410: 5f73 746f 7265 2873 746f 7261 6765 5f6c  _store(storage_l
-0002c420: 6962 2e53 746f 7265 5479 7065 2e53 3329  ib.StoreType.S3)
-0002c430: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
-0002c440: 5f6e 616d 6520 3d20 746d 705f 7363 7261  _name = tmp_scra
-0002c450: 7463 685f 7374 6f72 6167 655f 6f62 6a2e  tch_storage_obj.
-0002c460: 6e61 6d65 0a0a 2020 2020 2020 2020 2320  name..        # 
-0002c470: 5472 7920 746f 2069 6e69 7469 616c 697a  Try to initializ
-0002c480: 6520 616e 6f74 6865 7220 7374 6f72 6167  e another storag
-0002c490: 6520 7769 7468 2074 6865 2073 746f 7261  e with the stora
-0002c4a0: 6765 206f 626a 6563 7420 6372 6561 7465  ge object create
-0002c4b0: 640a 2020 2020 2020 2020 2320 6162 6f76  d.        # abov
-0002c4c0: 652c 2062 7574 206e 6f77 2069 6e20 434f  e, but now in CO
-0002c4d0: 5059 206d 6f64 652e 2054 6869 7320 7368  PY mode. This sh
-0002c4e0: 6f75 6c64 2073 7563 6365 6564 2e0a 2020  ould succeed..  
-0002c4f0: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
-0002c500: 2073 656c 662e 7969 656c 645f 7374 6f72   self.yield_stor
-0002c510: 6167 655f 6f62 6a65 6374 286e 616d 653d  age_object(name=
-0002c520: 7374 6f72 6167 655f 6e61 6d65 2c0a 2020  storage_name,.  
-0002c530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002c550: 2020 2020 2020 2020 2020 206d 6f64 653d             mode=
-0002c560: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0002c570: 6167 654d 6f64 652e 434f 5059 290a 0a20  ageMode.COPY).. 
-0002c580: 2020 2040 7079 7465 7374 2e66 6978 7475     @pytest.fixtu
-0002c590: 7265 0a20 2020 2064 6566 2074 6d70 5f67  re.    def tmp_g
-0002c5a0: 6974 6967 6e6f 7265 5f73 746f 7261 6765  itignore_storage
-0002c5b0: 5f6f 626a 2873 656c 662c 2074 6d70 5f62  _obj(self, tmp_b
-0002c5c0: 7563 6b65 745f 6e61 6d65 2c20 6769 7469  ucket_name, giti
-0002c5d0: 676e 6f72 655f 7374 7275 6374 7572 6529  gnore_structure)
-0002c5e0: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
-0002c5f0: 7465 7320 6120 7465 6d70 6f72 6172 7920  tes a temporary 
-0002c600: 7374 6f72 6167 6520 6f62 6a65 6374 2066  storage object f
-0002c610: 6f72 2074 6573 7469 6e67 202e 6769 7469  or testing .giti
-0002c620: 676e 6f72 6520 6669 6c74 6572 2e0a 2020  gnore filter..  
-0002c630: 2020 2020 2020 2320 4749 5449 4749 4e4f        # GITIGINO
-0002c640: 5245 5f53 5452 5543 5455 5245 2069 7320  RE_STRUCTURE is 
-0002c650: 7265 7072 6573 656e 7469 6e67 2061 2066  representing a f
-0002c660: 696c 6520 7374 7275 6374 7572 6520 696e  ile structure in
-0002c670: 2061 2064 6963 7469 6f6e 6172 790a 2020   a dictionary.  
-0002c680: 2020 2020 2020 2320 666f 726d 6174 2e20        # format. 
-0002c690: 4372 6561 7465 6420 7374 6f72 6167 6520  Created storage 
-0002c6a0: 6f62 6a65 6374 2077 696c 6c20 636f 6e74  object will cont
-0002c6b0: 6169 6e20 7468 6520 6669 6c65 2073 7472  ain the file str
-0002c6c0: 7563 7475 7265 2061 6c6f 6e67 0a20 2020  ucture along.   
-0002c6d0: 2020 2020 2023 2077 6974 6820 2e67 6974       # with .git
-0002c6e0: 6967 6e6f 7265 2061 6e64 202e 6769 742f  ignore and .git/
-0002c6f0: 696e 666f 2f65 7863 6c75 6465 2066 696c  info/exclude fil
-0002c700: 6573 2074 6f20 7465 7374 2065 7863 6c75  es to test exclu
-0002c710: 6465 2066 696c 7465 722e 0a20 2020 2020  de filter..     
-0002c720: 2020 2023 2053 746f 7265 7320 6d75 7374     # Stores must
-0002c730: 2062 6520 6164 6465 6420 696e 2074 6865   be added in the
-0002c740: 2074 6573 742e 0a20 2020 2020 2020 2077   test..        w
-0002c750: 6974 6820 7465 6d70 6669 6c65 2e54 656d  ith tempfile.Tem
-0002c760: 706f 7261 7279 4469 7265 6374 6f72 7928  poraryDirectory(
-0002c770: 2920 6173 2074 6d70 6469 723a 0a20 2020  ) as tmpdir:.   
-0002c780: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
-0002c790: 6573 2066 696c 6520 7374 7275 6374 7572  es file structur
-0002c7a0: 6520 746f 2062 6520 7570 6c6f 6164 6564  e to be uploaded
-0002c7b0: 2069 6e20 7468 6520 5374 6f72 6167 650a   in the Storage.
-0002c7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c7d0: 2e63 7265 6174 655f 6469 725f 7374 7275  .create_dir_stru
-0002c7e0: 6374 7572 6528 746d 7064 6972 2c20 6769  cture(tmpdir, gi
-0002c7f0: 7469 676e 6f72 655f 7374 7275 6374 7572  tignore_structur
-0002c800: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-0002c810: 2320 4372 6561 7465 202e 6769 7469 676e  # Create .gitign
-0002c820: 6f72 6520 616e 6420 6c69 7374 2066 696c  ore and list fil
-0002c830: 6573 2f64 6972 7320 746f 2062 6520 6578  es/dirs to be ex
-0002c840: 636c 7564 6564 2069 6e20 6974 0a20 2020  cluded in it.   
-0002c850: 2020 2020 2020 2020 2073 6b79 7069 6c6f           skypilo
-0002c860: 745f 7061 7468 203d 206f 732e 7061 7468  t_path = os.path
-0002c870: 2e64 6972 6e61 6d65 286f 732e 7061 7468  .dirname(os.path
-0002c880: 2e64 6972 6e61 6d65 2873 6b79 2e5f 5f66  .dirname(sky.__f
-0002c890: 696c 655f 5f29 290a 2020 2020 2020 2020  ile__)).        
-0002c8a0: 2020 2020 7465 6d70 5f70 6174 6820 3d20      temp_path = 
-0002c8b0: 6627 7b74 6d70 6469 727d 2f2e 6769 7469  f'{tmpdir}/.giti
-0002c8c0: 676e 6f72 6527 0a20 2020 2020 2020 2020  gnore'.         
-0002c8d0: 2020 2066 696c 655f 7061 7468 203d 206f     file_path = o
-0002c8e0: 732e 7061 7468 2e6a 6f69 6e28 736b 7970  s.path.join(skyp
-0002c8f0: 696c 6f74 5f70 6174 682c 2027 7465 7374  ilot_path, 'test
-0002c900: 732f 6769 7469 676e 6f72 655f 7465 7374  s/gitignore_test
-0002c910: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-0002c920: 6875 7469 6c2e 636f 7079 6669 6c65 2866  hutil.copyfile(f
-0002c930: 696c 655f 7061 7468 2c20 7465 6d70 5f70  ile_path, temp_p
-0002c940: 6174 6829 0a0a 2020 2020 2020 2020 2020  ath)..          
-0002c950: 2020 2320 4372 6561 7465 202e 6769 742f    # Create .git/
-0002c960: 696e 666f 2f65 7863 6c75 6465 2061 6e64  info/exclude and
-0002c970: 206c 6973 7420 6669 6c65 732f 6469 7273   list files/dirs
-0002c980: 2074 6f20 6265 2065 7863 6c75 6465 6420   to be excluded 
-0002c990: 696e 2069 740a 2020 2020 2020 2020 2020  in it.          
-0002c9a0: 2020 7465 6d70 5f70 6174 6820 3d20 6627    temp_path = f'
-0002c9b0: 7b74 6d70 6469 727d 2f2e 6769 742f 696e  {tmpdir}/.git/in
-0002c9c0: 666f 2f27 0a20 2020 2020 2020 2020 2020  fo/'.           
-0002c9d0: 206f 732e 6d61 6b65 6469 7273 2874 656d   os.makedirs(tem
-0002c9e0: 705f 7061 7468 290a 2020 2020 2020 2020  p_path).        
-0002c9f0: 2020 2020 7465 6d70 5f65 7863 6c75 6465      temp_exclude
-0002ca00: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0002ca10: 6a6f 696e 2874 656d 705f 7061 7468 2c20  join(temp_path, 
-0002ca20: 2765 7863 6c75 6465 2729 0a20 2020 2020  'exclude').     
-0002ca30: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
-0002ca40: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0002ca50: 736b 7970 696c 6f74 5f70 6174 682c 0a20  skypilot_path,. 
-0002ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ca80: 2020 2020 2774 6573 7473 2f67 6974 5f69      'tests/git_i
-0002ca90: 6e66 6f5f 6578 636c 7564 655f 7465 7374  nfo_exclude_test
-0002caa0: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-0002cab0: 6875 7469 6c2e 636f 7079 6669 6c65 2866  hutil.copyfile(f
-0002cac0: 696c 655f 7061 7468 2c20 7465 6d70 5f65  ile_path, temp_e
-0002cad0: 7863 6c75 6465 5f70 6174 6829 0a0a 2020  xclude_path)..  
-0002cae0: 2020 2020 2020 2020 2020 2320 4372 6561            # Crea
-0002caf0: 7465 2073 6b79 2053 746f 7261 6765 2077  te sky Storage w
-0002cb00: 6974 6820 7468 6520 6669 6c65 7320 6372  ith the files cr
-0002cb10: 6561 7465 640a 2020 2020 2020 2020 2020  eated.          
-0002cb20: 2020 7969 656c 6420 6672 6f6d 2073 656c    yield from sel
-0002cb30: 662e 7969 656c 645f 7374 6f72 6167 655f  f.yield_storage_
-0002cb40: 6f62 6a65 6374 280a 2020 2020 2020 2020  object(.        
-0002cb50: 2020 2020 2020 2020 6e61 6d65 3d74 6d70          name=tmp
-0002cb60: 5f62 7563 6b65 745f 6e61 6d65 2c0a 2020  _bucket_name,.  
-0002cb70: 2020 2020 2020 2020 2020 2020 2020 736f                so
-0002cb80: 7572 6365 3d74 6d70 6469 722c 0a20 2020  urce=tmpdir,.   
-0002cb90: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0002cba0: 653d 7374 6f72 6167 655f 6c69 622e 5374  e=storage_lib.St
-0002cbb0: 6f72 6167 654d 6f64 652e 434f 5059 290a  orageMode.COPY).
-0002cbc0: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-0002cbd0: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
-0002cbe0: 5f61 7773 636c 695f 6275 636b 6574 2873  _awscli_bucket(s
-0002cbf0: 656c 662c 2074 6d70 5f62 7563 6b65 745f  elf, tmp_bucket_
-0002cc00: 6e61 6d65 293a 0a20 2020 2020 2020 2023  name):.        #
-0002cc10: 2043 7265 6174 6573 2061 2074 656d 706f   Creates a tempo
-0002cc20: 7261 7279 2062 7563 6b65 7420 7573 696e  rary bucket usin
-0002cc30: 6720 6177 7363 6c69 0a20 2020 2020 2020  g awscli.       
-0002cc40: 2062 7563 6b65 745f 7572 6920 3d20 6627   bucket_uri = f'
-0002cc50: 7333 3a2f 2f7b 746d 705f 6275 636b 6574  s3://{tmp_bucket
-0002cc60: 5f6e 616d 657d 270a 2020 2020 2020 2020  _name}'.        
-0002cc70: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0002cc80: 5f63 616c 6c28 5b27 6177 7327 2c20 2773  _call(['aws', 's
-0002cc90: 3327 2c20 276d 6227 2c20 6275 636b 6574  3', 'mb', bucket
-0002cca0: 5f75 7269 5d29 0a20 2020 2020 2020 2079  _uri]).        y
-0002ccb0: 6965 6c64 2074 6d70 5f62 7563 6b65 745f  ield tmp_bucket_
-0002ccc0: 6e61 6d65 2c20 6275 636b 6574 5f75 7269  name, bucket_uri
-0002ccd0: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
-0002cce0: 6573 732e 6368 6563 6b5f 6361 6c6c 285b  ess.check_call([
-0002ccf0: 2761 7773 272c 2027 7333 272c 2027 7262  'aws', 's3', 'rb
-0002cd00: 272c 2062 7563 6b65 745f 7572 692c 2027  ', bucket_uri, '
-0002cd10: 2d2d 666f 7263 6527 5d29 0a0a 2020 2020  --force'])..    
-0002cd20: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-0002cd30: 2020 2020 6465 6620 746d 705f 6773 7574      def tmp_gsut
-0002cd40: 696c 5f62 7563 6b65 7428 7365 6c66 2c20  il_bucket(self, 
-0002cd50: 746d 705f 6275 636b 6574 5f6e 616d 6529  tmp_bucket_name)
-0002cd60: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
-0002cd70: 7465 7320 6120 7465 6d70 6f72 6172 7920  tes a temporary 
-0002cd80: 6275 636b 6574 2075 7369 6e67 2067 7375  bucket using gsu
-0002cd90: 7469 6c0a 2020 2020 2020 2020 6275 636b  til.        buck
-0002cda0: 6574 5f75 7269 203d 2066 2767 733a 2f2f  et_uri = f'gs://
-0002cdb0: 7b74 6d70 5f62 7563 6b65 745f 6e61 6d65  {tmp_bucket_name
-0002cdc0: 7d27 0a20 2020 2020 2020 2073 7562 7072  }'.        subpr
-0002cdd0: 6f63 6573 732e 6368 6563 6b5f 6361 6c6c  ocess.check_call
-0002cde0: 285b 2767 7375 7469 6c27 2c20 276d 6227  (['gsutil', 'mb'
-0002cdf0: 2c20 6275 636b 6574 5f75 7269 5d29 0a20  , bucket_uri]). 
-0002ce00: 2020 2020 2020 2079 6965 6c64 2074 6d70         yield tmp
-0002ce10: 5f62 7563 6b65 745f 6e61 6d65 2c20 6275  _bucket_name, bu
-0002ce20: 636b 6574 5f75 7269 0a20 2020 2020 2020  cket_uri.       
-0002ce30: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-0002ce40: 6b5f 6361 6c6c 285b 2767 7375 7469 6c27  k_call(['gsutil'
-0002ce50: 2c20 2772 6d27 2c20 272d 7227 2c20 6275  , 'rm', '-r', bu
-0002ce60: 636b 6574 5f75 7269 5d29 0a0a 2020 2020  cket_uri])..    
-0002ce70: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
-0002ce80: 2020 2020 6465 6620 746d 705f 6177 7363      def tmp_awsc
-0002ce90: 6c69 5f62 7563 6b65 745f 7232 2873 656c  li_bucket_r2(sel
-0002cea0: 662c 2074 6d70 5f62 7563 6b65 745f 6e61  f, tmp_bucket_na
-0002ceb0: 6d65 293a 0a20 2020 2020 2020 2023 2043  me):.        # C
-0002cec0: 7265 6174 6573 2061 2074 656d 706f 7261  reates a tempora
-0002ced0: 7279 2062 7563 6b65 7420 7573 696e 6720  ry bucket using 
-0002cee0: 6177 7363 6c69 0a20 2020 2020 2020 2065  awscli.        e
-0002cef0: 6e64 706f 696e 745f 7572 6c20 3d20 636c  ndpoint_url = cl
-0002cf00: 6f75 6466 6c61 7265 2e63 7265 6174 655f  oudflare.create_
-0002cf10: 656e 6470 6f69 6e74 2829 0a20 2020 2020  endpoint().     
-0002cf20: 2020 2062 7563 6b65 745f 7572 6920 3d20     bucket_uri = 
-0002cf30: 6627 7333 3a2f 2f7b 746d 705f 6275 636b  f's3://{tmp_buck
-0002cf40: 6574 5f6e 616d 657d 270a 2020 2020 2020  et_name}'.      
-0002cf50: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
-0002cf60: 636b 5f63 616c 6c28 0a20 2020 2020 2020  ck_call(.       
-0002cf70: 2020 2020 2066 2741 5753 5f53 4841 5245       f'AWS_SHARE
-0002cf80: 445f 4352 4544 454e 5449 414c 535f 4649  D_CREDENTIALS_FI
-0002cf90: 4c45 3d7b 636c 6f75 6466 6c61 7265 2e52  LE={cloudflare.R
-0002cfa0: 325f 4352 4544 454e 5449 414c 535f 5041  2_CREDENTIALS_PA
-0002cfb0: 5448 7d20 6177 7320 7333 206d 6220 7b62  TH} aws s3 mb {b
-0002cfc0: 7563 6b65 745f 7572 697d 202d 2d65 6e64  ucket_uri} --end
-0002cfd0: 706f 696e 7420 7b65 6e64 706f 696e 745f  point {endpoint_
-0002cfe0: 7572 6c7d 202d 2d70 726f 6669 6c65 3d72  url} --profile=r
-0002cff0: 3227 2c0a 2020 2020 2020 2020 2020 2020  2',.            
-0002d000: 7368 656c 6c3d 5472 7565 290a 2020 2020  shell=True).    
-0002d010: 2020 2020 7969 656c 6420 746d 705f 6275      yield tmp_bu
-0002d020: 636b 6574 5f6e 616d 652c 2062 7563 6b65  cket_name, bucke
-0002d030: 745f 7572 690a 2020 2020 2020 2020 7375  t_uri.        su
-0002d040: 6270 726f 6365 7373 2e63 6865 636b 5f63  bprocess.check_c
-0002d050: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
-0002d060: 2066 2741 5753 5f53 4841 5245 445f 4352   f'AWS_SHARED_CR
-0002d070: 4544 454e 5449 414c 535f 4649 4c45 3d7b  EDENTIALS_FILE={
-0002d080: 636c 6f75 6466 6c61 7265 2e52 325f 4352  cloudflare.R2_CR
-0002d090: 4544 454e 5449 414c 535f 5041 5448 7d20  EDENTIALS_PATH} 
-0002d0a0: 6177 7320 7333 2072 6220 7b62 7563 6b65  aws s3 rb {bucke
-0002d0b0: 745f 7572 697d 202d 2d66 6f72 6365 202d  t_uri} --force -
-0002d0c0: 2d65 6e64 706f 696e 7420 7b65 6e64 706f  -endpoint {endpo
-0002d0d0: 696e 745f 7572 6c7d 202d 2d70 726f 6669  int_url} --profi
-0002d0e0: 6c65 3d72 3227 2c0a 2020 2020 2020 2020  le=r2',.        
-0002d0f0: 2020 2020 7368 656c 6c3d 5472 7565 290a      shell=True).
-0002d100: 0a20 2020 2040 7079 7465 7374 2e66 6978  .    @pytest.fix
-0002d110: 7475 7265 0a20 2020 2064 6566 2074 6d70  ture.    def tmp
-0002d120: 5f69 626d 5f63 6f73 5f62 7563 6b65 7428  _ibm_cos_bucket(
-0002d130: 7365 6c66 2c20 746d 705f 6275 636b 6574  self, tmp_bucket
-0002d140: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
-0002d150: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
-0002d160: 6f72 6172 7920 6275 636b 6574 2075 7369  orary bucket usi
-0002d170: 6e67 2049 424d 2043 4f53 2041 5049 0a20  ng IBM COS API. 
-0002d180: 2020 2020 2020 2073 746f 7261 6765 5f6f         storage_o
-0002d190: 626a 203d 2073 746f 7261 6765 5f6c 6962  bj = storage_lib
-0002d1a0: 2e49 424d 436f 7353 746f 7265 2873 6f75  .IBMCosStore(sou
-0002d1b0: 7263 653d 2222 2c20 6e61 6d65 3d74 6d70  rce="", name=tmp
-0002d1c0: 5f62 7563 6b65 745f 6e61 6d65 290a 2020  _bucket_name).  
-0002d1d0: 2020 2020 2020 7969 656c 6420 746d 705f        yield tmp_
-0002d1e0: 6275 636b 6574 5f6e 616d 650a 2020 2020  bucket_name.    
-0002d1f0: 2020 2020 7374 6f72 6167 655f 6f62 6a2e      storage_obj.
-0002d200: 6465 6c65 7465 2829 0a0a 2020 2020 4070  delete()..    @p
-0002d210: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
-0002d220: 2020 6465 6620 746d 705f 7075 626c 6963    def tmp_public
-0002d230: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
-0002d240: 662c 2072 6571 7565 7374 293a 0a20 2020  f, request):.   
-0002d250: 2020 2020 2023 2049 6e69 7469 616c 697a       # Initializ
-0002d260: 6573 2061 2073 746f 7261 6765 206f 626a  es a storage obj
-0002d270: 6563 7420 7769 7468 2061 2070 7562 6c69  ect with a publi
-0002d280: 6320 6275 636b 6574 0a20 2020 2020 2020  c bucket.       
-0002d290: 2073 746f 7261 6765 5f6f 626a 203d 2073   storage_obj = s
-0002d2a0: 746f 7261 6765 5f6c 6962 2e53 746f 7261  torage_lib.Stora
-0002d2b0: 6765 2873 6f75 7263 653d 7265 7175 6573  ge(source=reques
-0002d2c0: 742e 7061 7261 6d29 0a20 2020 2020 2020  t.param).       
-0002d2d0: 2079 6965 6c64 2073 746f 7261 6765 5f6f   yield storage_o
-0002d2e0: 626a 0a20 2020 2020 2020 2023 2054 6869  bj.        # Thi
-0002d2f0: 7320 646f 6573 206e 6f74 2072 6571 7569  s does not requi
-0002d300: 7265 2061 6e79 2064 656c 6574 696f 6e20  re any deletion 
-0002d310: 6c6f 6769 6320 6265 6361 7573 6520 6974  logic because it
-0002d320: 2069 7320 6120 7075 626c 6963 2062 7563   is a public buc
-0002d330: 6b65 740a 2020 2020 2020 2020 2320 616e  ket.        # an
-0002d340: 6420 7368 6f75 6c64 206e 6f74 2067 6574  d should not get
-0002d350: 2061 6464 6564 2074 6f20 676c 6f62 616c   added to global
-0002d360: 5f75 7365 725f 7374 6174 652e 0a0a 2020  _user_state...  
-0002d370: 2020 4070 7974 6573 742e 6d61 726b 2e6e    @pytest.mark.n
-0002d380: 6f5f 666c 7569 6473 7461 636b 0a20 2020  o_fluidstack.   
-0002d390: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
-0002d3a0: 7261 6d65 7472 697a 6528 2773 746f 7265  rametrize('store
-0002d3b0: 5f74 7970 6527 2c20 5b0a 2020 2020 2020  _type', [.      
-0002d3c0: 2020 7374 6f72 6167 655f 6c69 622e 5374    storage_lib.St
-0002d3d0: 6f72 6554 7970 652e 5333 2c20 7374 6f72  oreType.S3, stor
-0002d3e0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002d3f0: 652e 4743 532c 0a20 2020 2020 2020 2070  e.GCS,.        p
-0002d400: 7974 6573 742e 7061 7261 6d28 7374 6f72  ytest.param(stor
-0002d410: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002d420: 652e 4942 4d2c 206d 6172 6b73 3d70 7974  e.IBM, marks=pyt
-0002d430: 6573 742e 6d61 726b 2e69 626d 292c 0a20  est.mark.ibm),. 
-0002d440: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
-0002d450: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
-0002d460: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
-0002d470: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
-0002d480: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
-0002d490: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
-0002d4a0: 6e65 775f 6275 636b 6574 5f63 7265 6174  new_bucket_creat
-0002d4b0: 696f 6e5f 616e 645f 6465 6c65 7469 6f6e  ion_and_deletion
-0002d4c0: 2873 656c 662c 2074 6d70 5f6c 6f63 616c  (self, tmp_local
-0002d4d0: 5f73 746f 7261 6765 5f6f 626a 2c0a 2020  _storage_obj,.  
-0002d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002d500: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
-0002d510: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
-0002d520: 2023 2043 7265 6174 6573 2061 206e 6577   # Creates a new
-0002d530: 2062 7563 6b65 7420 7769 7468 2061 206c   bucket with a l
-0002d540: 6f63 616c 2073 6f75 7263 652c 2075 706c  ocal source, upl
-0002d550: 6f61 6473 2066 696c 6573 2074 6f20 6974  oads files to it
-0002d560: 0a20 2020 2020 2020 2023 2061 6e64 2064  .        # and d
-0002d570: 656c 6574 6573 2069 742e 0a20 2020 2020  eletes it..     
-0002d580: 2020 2074 6d70 5f6c 6f63 616c 5f73 746f     tmp_local_sto
-0002d590: 7261 6765 5f6f 626a 2e61 6464 5f73 746f  rage_obj.add_sto
-0002d5a0: 7265 2873 746f 7265 5f74 7970 6529 0a0a  re(store_type)..
-0002d5b0: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
-0002d5c0: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
-0002d5d0: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
-0002d5e0: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
-0002d5f0: 6e20 7468 6520 6f75 7470 7574 0a20 2020  n the output.   
-0002d600: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0002d610: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0002d620: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
-0002d630: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
-0002d640: 2020 2020 2061 7373 6572 7420 746d 705f       assert tmp_
-0002d650: 6c6f 6361 6c5f 7374 6f72 6167 655f 6f62  local_storage_ob
-0002d660: 6a2e 6e61 6d65 2069 6e20 6f75 742e 6465  j.name in out.de
-0002d670: 636f 6465 2827 7574 662d 3827 290a 0a20  code('utf-8').. 
-0002d680: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
-0002d690: 2073 746f 7261 6765 2064 656c 6574 6520   storage delete 
-0002d6a0: 746f 2064 656c 6574 6520 7468 6520 7374  to delete the st
-0002d6b0: 6f72 6167 6520 6f62 6a65 6374 0a20 2020  orage object.   
-0002d6c0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-0002d6d0: 6368 6563 6b5f 6f75 7470 7574 280a 2020  check_output(.  
-0002d6e0: 2020 2020 2020 2020 2020 5b27 736b 7927            ['sky'
-0002d6f0: 2c20 2773 746f 7261 6765 272c 2027 6465  , 'storage', 'de
-0002d700: 6c65 7465 272c 2074 6d70 5f6c 6f63 616c  lete', tmp_local
-0002d710: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-0002d720: 652c 2027 2d2d 7965 7327 5d29 0a0a 2020  e, '--yes'])..  
-0002d730: 2020 2020 2020 2320 5275 6e20 736b 7920        # Run sky 
-0002d740: 7374 6f72 6167 6520 6c73 2074 6f20 6368  storage ls to ch
-0002d750: 6563 6b20 6966 2073 746f 7261 6765 206f  eck if storage o
-0002d760: 626a 6563 7420 6973 2064 656c 6574 6564  bject is deleted
-0002d770: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0002d780: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0002d790: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
-0002d7a0: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
-0002d7b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0002d7c0: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
-0002d7d0: 655f 6f62 6a2e 6e61 6d65 206e 6f74 2069  e_obj.name not i
-0002d7e0: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0002d7f0: 662d 3827 290a 0a20 2020 2040 7079 7465  f-8')..    @pyte
-0002d800: 7374 2e6d 6172 6b2e 6e6f 5f66 6c75 6964  st.mark.no_fluid
-0002d810: 7374 6163 6b0a 2020 2020 4070 7974 6573  stack.    @pytes
-0002d820: 742e 6d61 726b 2e78 6469 7374 5f67 726f  t.mark.xdist_gro
-0002d830: 7570 2827 6d75 6c74 6970 6c65 5f62 7563  up('multiple_buc
-0002d840: 6b65 745f 6465 6c65 7469 6f6e 2729 0a20  ket_deletion'). 
-0002d850: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-0002d860: 7061 7261 6d65 7472 697a 6528 2773 746f  parametrize('sto
-0002d870: 7265 5f74 7970 6527 2c20 5b0a 2020 2020  re_type', [.    
-0002d880: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
-0002d890: 5374 6f72 6554 7970 652e 5333 2c20 7374  StoreType.S3, st
-0002d8a0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-0002d8b0: 7970 652e 4743 532c 0a20 2020 2020 2020  ype.GCS,.       
-0002d8c0: 2070 7974 6573 742e 7061 7261 6d28 7374   pytest.param(st
-0002d8d0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-0002d8e0: 7970 652e 5232 2c20 6d61 726b 733d 7079  ype.R2, marks=py
-0002d8f0: 7465 7374 2e6d 6172 6b2e 636c 6f75 6466  test.mark.cloudf
-0002d900: 6c61 7265 292c 0a20 2020 2020 2020 2070  lare),.        p
-0002d910: 7974 6573 742e 7061 7261 6d28 7374 6f72  ytest.param(stor
-0002d920: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002d930: 652e 4942 4d2c 206d 6172 6b73 3d70 7974  e.IBM, marks=pyt
-0002d940: 6573 742e 6d61 726b 2e69 626d 290a 2020  est.mark.ibm).  
-0002d950: 2020 5d29 0a20 2020 2064 6566 2074 6573    ]).    def tes
-0002d960: 745f 6d75 6c74 6970 6c65 5f62 7563 6b65  t_multiple_bucke
-0002d970: 7473 5f63 7265 6174 696f 6e5f 616e 645f  ts_creation_and_
-0002d980: 6465 6c65 7469 6f6e 280a 2020 2020 2020  deletion(.      
-0002d990: 2020 2020 2020 7365 6c66 2c20 746d 705f        self, tmp_
-0002d9a0: 6d75 6c74 6970 6c65 5f73 6372 6174 6368  multiple_scratch
-0002d9b0: 5f73 746f 7261 6765 5f6f 626a 2c20 7374  _storage_obj, st
-0002d9c0: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
-0002d9d0: 2020 2023 2043 7265 6174 6573 206d 756c     # Creates mul
-0002d9e0: 7469 706c 6520 6e65 7720 6275 636b 6574  tiple new bucket
-0002d9f0: 7328 3520 6275 636b 6574 7329 2077 6974  s(5 buckets) wit
-0002da00: 6820 6120 6c6f 6361 6c20 736f 7572 6365  h a local source
-0002da10: 0a20 2020 2020 2020 2023 2061 6e64 2064  .        # and d
-0002da20: 656c 6574 6573 2074 6865 6d2e 0a20 2020  eletes them..   
-0002da30: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
-0002da40: 5f6e 616d 6520 3d20 5b5d 0a20 2020 2020  _name = [].     
-0002da50: 2020 2066 6f72 2073 746f 7265 5f6f 626a     for store_obj
-0002da60: 2069 6e20 746d 705f 6d75 6c74 6970 6c65   in tmp_multiple
-0002da70: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
-0002da80: 5f6f 626a 3a0a 2020 2020 2020 2020 2020  _obj:.          
-0002da90: 2020 7374 6f72 655f 6f62 6a2e 6164 645f    store_obj.add_
-0002daa0: 7374 6f72 6528 7374 6f72 655f 7479 7065  store(store_type
-0002dab0: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-0002dac0: 6f72 6167 655f 6f62 6a5f 6e61 6d65 2e61  orage_obj_name.a
-0002dad0: 7070 656e 6428 7374 6f72 655f 6f62 6a2e  ppend(store_obj.
-0002dae0: 6e61 6d65 290a 0a20 2020 2020 2020 2023  name)..        #
-0002daf0: 2052 756e 2073 6b79 2073 746f 7261 6765   Run sky storage
-0002db00: 206c 7320 746f 2063 6865 636b 2069 6620   ls to check if 
-0002db10: 616c 6c20 7374 6f72 6167 6520 6f62 6a65  all storage obje
-0002db20: 6374 7320 6578 6973 7473 2069 6e20 7468  cts exists in th
-0002db30: 650a 2020 2020 2020 2020 2320 6f75 7470  e.        # outp
-0002db40: 7574 2066 696c 7465 7265 6420 6279 2073  ut filtered by s
-0002db50: 746f 7265 2074 7970 650a 2020 2020 2020  tore type.      
-0002db60: 2020 6f75 745f 616c 6c20 3d20 7375 6270    out_all = subp
-0002db70: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
-0002db80: 7075 7428 5b27 736b 7927 2c20 2773 746f  put(['sky', 'sto
-0002db90: 7261 6765 272c 2027 6c73 275d 290a 2020  rage', 'ls']).  
-0002dba0: 2020 2020 2020 6f75 7420 3d20 5b0a 2020        out = [.  
-0002dbb0: 2020 2020 2020 2020 2020 6974 656d 2e73            item.s
-0002dbc0: 706c 6974 2829 5b30 5d0a 2020 2020 2020  plit()[0].      
-0002dbd0: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-0002dbe0: 6e20 6f75 745f 616c 6c2e 6465 636f 6465  n out_all.decode
-0002dbf0: 2827 7574 662d 3827 292e 7370 6c69 746c  ('utf-8').splitl
-0002dc00: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
-0002dc10: 2020 2069 6620 7374 6f72 655f 7479 7065     if store_type
-0002dc20: 2e76 616c 7565 2069 6e20 6974 656d 0a20  .value in item. 
-0002dc30: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0002dc40: 2061 7373 6572 7420 616c 6c28 5b69 7465   assert all([ite
-0002dc50: 6d20 696e 206f 7574 2066 6f72 2069 7465  m in out for ite
-0002dc60: 6d20 696e 2073 746f 7261 6765 5f6f 626a  m in storage_obj
-0002dc70: 5f6e 616d 655d 290a 0a20 2020 2020 2020  _name])..       
-0002dc80: 2023 2052 756e 2073 6b79 2073 746f 7261   # Run sky stora
-0002dc90: 6765 2064 656c 6574 6520 616c 6c20 746f  ge delete all to
-0002dca0: 2064 656c 6574 6520 616c 6c20 7374 6f72   delete all stor
-0002dcb0: 6167 6520 6f62 6a65 6374 730a 2020 2020  age objects.    
-0002dcc0: 2020 2020 6465 6c65 7465 5f63 6d64 203d      delete_cmd =
-0002dcd0: 205b 2773 6b79 272c 2027 7374 6f72 6167   ['sky', 'storag
-0002dce0: 6527 2c20 2764 656c 6574 6527 2c20 272d  e', 'delete', '-
-0002dcf0: 2d79 6573 275d 0a20 2020 2020 2020 2064  -yes'].        d
-0002dd00: 656c 6574 655f 636d 6420 2b3d 2073 746f  elete_cmd += sto
-0002dd10: 7261 6765 5f6f 626a 5f6e 616d 650a 2020  rage_obj_name.  
-0002dd20: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
-0002dd30: 2e63 6865 636b 5f6f 7574 7075 7428 6465  .check_output(de
-0002dd40: 6c65 7465 5f63 6d64 290a 0a20 2020 2020  lete_cmd)..     
-0002dd50: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
-0002dd60: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
-0002dd70: 2069 6620 616c 6c20 7374 6f72 6167 6520   if all storage 
-0002dd80: 6f62 6a65 6374 7320 6669 6c74 6572 6564  objects filtered
-0002dd90: 2062 7920 7374 6f72 650a 2020 2020 2020   by store.      
-0002dda0: 2020 2320 7479 7065 2061 7265 2064 656c    # type are del
-0002ddb0: 6574 6564 0a20 2020 2020 2020 206f 7574  eted.        out
-0002ddc0: 5f61 6c6c 203d 2073 7562 7072 6f63 6573  _all = subproces
-0002ddd0: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
-0002dde0: 2773 6b79 272c 2027 7374 6f72 6167 6527  'sky', 'storage'
-0002ddf0: 2c20 276c 7327 5d29 0a20 2020 2020 2020  , 'ls']).       
-0002de00: 206f 7574 203d 205b 0a20 2020 2020 2020   out = [.       
-0002de10: 2020 2020 2069 7465 6d2e 7370 6c69 7428       item.split(
-0002de20: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-0002de30: 2066 6f72 2069 7465 6d20 696e 206f 7574   for item in out
-0002de40: 5f61 6c6c 2e64 6563 6f64 6528 2775 7466  _all.decode('utf
-0002de50: 2d38 2729 2e73 706c 6974 6c69 6e65 7328  -8').splitlines(
-0002de60: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0002de70: 2073 746f 7265 5f74 7970 652e 7661 6c75   store_type.valu
-0002de80: 6520 696e 2069 7465 6d0a 2020 2020 2020  e in item.      
-0002de90: 2020 5d0a 2020 2020 2020 2020 6173 7365    ].        asse
-0002dea0: 7274 2061 6c6c 285b 6974 656d 206e 6f74  rt all([item not
-0002deb0: 2069 6e20 6f75 7420 666f 7220 6974 656d   in out for item
-0002dec0: 2069 6e20 7374 6f72 6167 655f 6f62 6a5f   in storage_obj_
-0002ded0: 6e61 6d65 5d29 0a0a 2020 2020 4070 7974  name])..    @pyt
-0002dee0: 6573 742e 6d61 726b 2e6e 6f5f 666c 7569  est.mark.no_flui
-0002def0: 6473 7461 636b 0a20 2020 2040 7079 7465  dstack.    @pyte
-0002df00: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-0002df10: 697a 6528 2773 746f 7265 5f74 7970 6527  ize('store_type'
-0002df20: 2c20 5b0a 2020 2020 2020 2020 7374 6f72  , [.        stor
-0002df30: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002df40: 652e 5333 2c20 7374 6f72 6167 655f 6c69  e.S3, storage_li
-0002df50: 622e 5374 6f72 6554 7970 652e 4743 532c  b.StoreType.GCS,
-0002df60: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
-0002df70: 7061 7261 6d28 7374 6f72 6167 655f 6c69  param(storage_li
-0002df80: 622e 5374 6f72 6554 7970 652e 4942 4d2c  b.StoreType.IBM,
-0002df90: 206d 6172 6b73 3d70 7974 6573 742e 6d61   marks=pytest.ma
-0002dfa0: 726b 2e69 626d 292c 0a20 2020 2020 2020  rk.ibm),.       
-0002dfb0: 2070 7974 6573 742e 7061 7261 6d28 7374   pytest.param(st
-0002dfc0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-0002dfd0: 7970 652e 5232 2c20 6d61 726b 733d 7079  ype.R2, marks=py
-0002dfe0: 7465 7374 2e6d 6172 6b2e 636c 6f75 6466  test.mark.cloudf
-0002dff0: 6c61 7265 290a 2020 2020 5d29 0a20 2020  lare).    ]).   
-0002e000: 2064 6566 2074 6573 745f 7570 6c6f 6164   def test_upload
-0002e010: 5f73 6f75 7263 655f 7769 7468 5f73 7061  _source_with_spa
-0002e020: 6365 7328 7365 6c66 2c20 7374 6f72 655f  ces(self, store_
-0002e030: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
-0002e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e050: 2020 2020 2020 2020 2020 2020 2074 6d70               tmp
-0002e060: 5f6d 756c 7469 706c 655f 6375 7374 6f6d  _multiple_custom
-0002e070: 5f73 6f75 7263 655f 7374 6f72 6167 655f  _source_storage_
-0002e080: 6f62 6a29 3a0a 2020 2020 2020 2020 2320  obj):.        # 
-0002e090: 4372 6561 7465 7320 7477 6f20 6275 636b  Creates two buck
-0002e0a0: 6574 7320 7769 7468 2073 7065 6369 6669  ets with specifi
-0002e0b0: 6564 206c 6f63 616c 2073 6f75 7263 6573  ed local sources
-0002e0c0: 0a20 2020 2020 2020 2023 2077 6974 6820  .        # with 
-0002e0d0: 7370 6163 6573 2069 6e20 7468 6520 6e61  spaces in the na
-0002e0e0: 6d65 0a20 2020 2020 2020 2073 746f 7261  me.        stora
-0002e0f0: 6765 5f6f 626a 5f6e 616d 6573 203d 205b  ge_obj_names = [
-0002e100: 5d0a 2020 2020 2020 2020 666f 7220 7374  ].        for st
-0002e110: 6f72 6167 655f 6f62 6a20 696e 2074 6d70  orage_obj in tmp
-0002e120: 5f6d 756c 7469 706c 655f 6375 7374 6f6d  _multiple_custom
-0002e130: 5f73 6f75 7263 655f 7374 6f72 6167 655f  _source_storage_
-0002e140: 6f62 6a3a 0a20 2020 2020 2020 2020 2020  obj:.           
-0002e150: 2073 746f 7261 6765 5f6f 626a 2e61 6464   storage_obj.add
-0002e160: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
-0002e170: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-0002e180: 746f 7261 6765 5f6f 626a 5f6e 616d 6573  torage_obj_names
-0002e190: 2e61 7070 656e 6428 7374 6f72 6167 655f  .append(storage_
-0002e1a0: 6f62 6a2e 6e61 6d65 290a 0a20 2020 2020  obj.name)..     
-0002e1b0: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
-0002e1c0: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
-0002e1d0: 2069 6620 616c 6c20 7374 6f72 6167 6520   if all storage 
-0002e1e0: 6f62 6a65 6374 7320 6578 6973 7473 2069  objects exists i
-0002e1f0: 6e20 7468 650a 2020 2020 2020 2020 2320  n the.        # 
-0002e200: 6f75 7470 7574 2066 696c 7465 7265 6420  output filtered 
-0002e210: 6279 2073 746f 7265 2074 7970 650a 2020  by store type.  
-0002e220: 2020 2020 2020 6f75 745f 616c 6c20 3d20        out_all = 
-0002e230: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0002e240: 5f6f 7574 7075 7428 5b27 736b 7927 2c20  _output(['sky', 
-0002e250: 2773 746f 7261 6765 272c 2027 6c73 275d  'storage', 'ls']
-0002e260: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
-0002e270: 5b0a 2020 2020 2020 2020 2020 2020 6974  [.            it
-0002e280: 656d 2e73 706c 6974 2829 5b30 5d0a 2020  em.split()[0].  
-0002e290: 2020 2020 2020 2020 2020 666f 7220 6974            for it
-0002e2a0: 656d 2069 6e20 6f75 745f 616c 6c2e 6465  em in out_all.de
-0002e2b0: 636f 6465 2827 7574 662d 3827 292e 7370  code('utf-8').sp
-0002e2c0: 6c69 746c 696e 6573 2829 0a20 2020 2020  litlines().     
-0002e2d0: 2020 2020 2020 2069 6620 7374 6f72 655f         if store_
-0002e2e0: 7479 7065 2e76 616c 7565 2069 6e20 6974  type.value in it
-0002e2f0: 656d 0a20 2020 2020 2020 205d 0a20 2020  em.        ].   
-0002e300: 2020 2020 2061 7373 6572 7420 616c 6c28       assert all(
-0002e310: 5b69 7465 6d20 696e 206f 7574 2066 6f72  [item in out for
-0002e320: 2069 7465 6d20 696e 2073 746f 7261 6765   item in storage
-0002e330: 5f6f 626a 5f6e 616d 6573 5d29 0a0a 2020  _obj_names])..  
-0002e340: 2020 4070 7974 6573 742e 6d61 726b 2e6e    @pytest.mark.n
-0002e350: 6f5f 666c 7569 6473 7461 636b 0a20 2020  o_fluidstack.   
-0002e360: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
-0002e370: 7261 6d65 7472 697a 6528 2773 746f 7265  rametrize('store
-0002e380: 5f74 7970 6527 2c20 5b0a 2020 2020 2020  _type', [.      
-0002e390: 2020 7374 6f72 6167 655f 6c69 622e 5374    storage_lib.St
-0002e3a0: 6f72 6554 7970 652e 5333 2c20 7374 6f72  oreType.S3, stor
-0002e3b0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002e3c0: 652e 4743 532c 0a20 2020 2020 2020 2070  e.GCS,.        p
-0002e3d0: 7974 6573 742e 7061 7261 6d28 7374 6f72  ytest.param(stor
-0002e3e0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-0002e3f0: 652e 4942 4d2c 206d 6172 6b73 3d70 7974  e.IBM, marks=pyt
-0002e400: 6573 742e 6d61 726b 2e69 626d 292c 0a20  est.mark.ibm),. 
-0002e410: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
-0002e420: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
-0002e430: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
-0002e440: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
-0002e450: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
-0002e460: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
-0002e470: 6275 636b 6574 5f65 7874 6572 6e61 6c5f  bucket_external_
-0002e480: 6465 6c65 7469 6f6e 2873 656c 662c 2074  deletion(self, t
-0002e490: 6d70 5f73 6372 6174 6368 5f73 746f 7261  mp_scratch_stora
-0002e4a0: 6765 5f6f 626a 2c0a 2020 2020 2020 2020  ge_obj,.        
-0002e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e4c0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0002e4d0: 6f72 655f 7479 7065 293a 0a20 2020 2020  ore_type):.     
-0002e4e0: 2020 2023 2043 7265 6174 6573 2061 2062     # Creates a b
-0002e4f0: 7563 6b65 742c 2064 656c 6574 6573 2069  ucket, deletes i
-0002e500: 7420 6578 7465 726e 616c 6c79 2075 7369  t externally usi
-0002e510: 6e67 2063 6c6f 7564 2063 6c69 2063 6f6d  ng cloud cli com
-0002e520: 6d61 6e64 730a 2020 2020 2020 2020 2320  mands.        # 
-0002e530: 616e 6420 7468 656e 2074 7269 6573 2074  and then tries t
-0002e540: 6f20 6465 6c65 7465 2069 7420 7573 696e  o delete it usin
-0002e550: 6720 736b 7920 7374 6f72 6167 6520 6465  g sky storage de
-0002e560: 6c65 7465 2e0a 2020 2020 2020 2020 746d  lete..        tm
-0002e570: 705f 7363 7261 7463 685f 7374 6f72 6167  p_scratch_storag
-0002e580: 655f 6f62 6a2e 6164 645f 7374 6f72 6528  e_obj.add_store(
-0002e590: 7374 6f72 655f 7479 7065 290a 0a20 2020  store_type)..   
-0002e5a0: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
-0002e5b0: 746f 7261 6765 206c 7320 746f 2063 6865  torage ls to che
-0002e5c0: 636b 2069 6620 7374 6f72 6167 6520 6f62  ck if storage ob
-0002e5d0: 6a65 6374 2065 7869 7374 7320 696e 2074  ject exists in t
-0002e5e0: 6865 206f 7574 7075 740a 2020 2020 2020  he output.      
-0002e5f0: 2020 6f75 7420 3d20 7375 6270 726f 6365    out = subproce
-0002e600: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-0002e610: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
-0002e620: 272c 2027 6c73 275d 290a 2020 2020 2020  ', 'ls']).      
-0002e630: 2020 6173 7365 7274 2074 6d70 5f73 6372    assert tmp_scr
-0002e640: 6174 6368 5f73 746f 7261 6765 5f6f 626a  atch_storage_obj
-0002e650: 2e6e 616d 6520 696e 206f 7574 2e64 6563  .name in out.dec
-0002e660: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
-0002e670: 2020 2020 2020 2320 4465 6c65 7465 2062        # Delete b
-0002e680: 7563 6b65 7420 6578 7465 726e 616c 6c79  ucket externally
-0002e690: 0a20 2020 2020 2020 2063 6d64 203d 2073  .        cmd = s
-0002e6a0: 656c 662e 636c 695f 6465 6c65 7465 5f63  elf.cli_delete_c
-0002e6b0: 6d64 2873 746f 7265 5f74 7970 652c 2074  md(store_type, t
-0002e6c0: 6d70 5f73 6372 6174 6368 5f73 746f 7261  mp_scratch_stora
-0002e6d0: 6765 5f6f 626a 2e6e 616d 6529 0a20 2020  ge_obj.name).   
-0002e6e0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-0002e6f0: 6368 6563 6b5f 6f75 7470 7574 2863 6d64  check_output(cmd
-0002e700: 2c20 7368 656c 6c3d 5472 7565 290a 0a20  , shell=True).. 
-0002e710: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
-0002e720: 2073 746f 7261 6765 2064 656c 6574 6520   storage delete 
-0002e730: 746f 2064 656c 6574 6520 7468 6520 7374  to delete the st
-0002e740: 6f72 6167 6520 6f62 6a65 6374 0a20 2020  orage object.   
-0002e750: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-0002e760: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-0002e770: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
-0002e780: 5b27 736b 7927 2c20 2773 746f 7261 6765  ['sky', 'storage
-0002e790: 272c 2027 6465 6c65 7465 272c 2074 6d70  ', 'delete', tmp
-0002e7a0: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
-0002e7b0: 5f6f 626a 2e6e 616d 652c 2027 2d2d 7965  _obj.name, '--ye
-0002e7c0: 7327 5d29 0a20 2020 2020 2020 2023 204d  s']).        # M
-0002e7d0: 616b 6520 7375 7265 2062 7563 6b65 7420  ake sure bucket 
-0002e7e0: 7761 7320 6e6f 7420 6372 6561 7465 6420  was not created 
-0002e7f0: 6475 7269 6e67 2064 656c 6574 696f 6e20  during deletion 
-0002e800: 2873 6565 2069 7373 7565 2023 3133 3232  (see issue #1322
-0002e810: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0002e820: 2027 6372 6561 7465 6427 206e 6f74 2069   'created' not i
-0002e830: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-0002e840: 662d 3827 292e 6c6f 7765 7228 290a 0a20  f-8').lower().. 
-0002e850: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
-0002e860: 2073 746f 7261 6765 206c 7320 746f 2063   storage ls to c
-0002e870: 6865 636b 2069 6620 7374 6f72 6167 6520  heck if storage 
-0002e880: 6f62 6a65 6374 2069 7320 6465 6c65 7465  object is delete
-0002e890: 640a 2020 2020 2020 2020 6f75 7420 3d20  d.        out = 
-0002e8a0: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-0002e8b0: 5f6f 7574 7075 7428 5b27 736b 7927 2c20  _output(['sky', 
-0002e8c0: 2773 746f 7261 6765 272c 2027 6c73 275d  'storage', 'ls']
-0002e8d0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0002e8e0: 2074 6d70 5f73 6372 6174 6368 5f73 746f   tmp_scratch_sto
-0002e8f0: 7261 6765 5f6f 626a 2e6e 616d 6520 6e6f  rage_obj.name no
-0002e900: 7420 696e 206f 7574 2e64 6563 6f64 6528  t in out.decode(
-0002e910: 2775 7466 2d38 2729 0a0a 2020 2020 4070  'utf-8')..    @p
-0002e920: 7974 6573 742e 6d61 726b 2e6e 6f5f 666c  ytest.mark.no_fl
-0002e930: 7569 6473 7461 636b 0a20 2020 2040 7079  uidstack.    @py
-0002e940: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-0002e950: 7472 697a 6528 2773 746f 7265 5f74 7970  trize('store_typ
-0002e960: 6527 2c20 5b0a 2020 2020 2020 2020 7374  e', [.        st
-0002e970: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
-0002e980: 7970 652e 5333 2c20 7374 6f72 6167 655f  ype.S3, storage_
-0002e990: 6c69 622e 5374 6f72 6554 7970 652e 4743  lib.StoreType.GC
-0002e9a0: 532c 0a20 2020 2020 2020 2070 7974 6573  S,.        pytes
-0002e9b0: 742e 7061 7261 6d28 7374 6f72 6167 655f  t.param(storage_
-0002e9c0: 6c69 622e 5374 6f72 6554 7970 652e 4942  lib.StoreType.IB
-0002e9d0: 4d2c 206d 6172 6b73 3d70 7974 6573 742e  M, marks=pytest.
-0002e9e0: 6d61 726b 2e69 626d 292c 0a20 2020 2020  mark.ibm),.     
-0002e9f0: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
-0002ea00: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0002ea10: 6554 7970 652e 5232 2c20 6d61 726b 733d  eType.R2, marks=
-0002ea20: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
-0002ea30: 6466 6c61 7265 290a 2020 2020 5d29 0a20  dflare).    ]). 
-0002ea40: 2020 2064 6566 2074 6573 745f 6275 636b     def test_buck
-0002ea50: 6574 5f62 756c 6b5f 6465 6c65 7469 6f6e  et_bulk_deletion
-0002ea60: 2873 656c 662c 2073 746f 7265 5f74 7970  (self, store_typ
-0002ea70: 652c 2074 6d70 5f62 756c 6b5f 6465 6c5f  e, tmp_bulk_del_
-0002ea80: 7374 6f72 6167 655f 6f62 6a29 3a0a 2020  storage_obj):.  
-0002ea90: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
-0002eaa0: 6120 7465 6d70 2066 6f6c 6465 7220 7769  a temp folder wi
-0002eab0: 7468 206f 7665 7220 3235 3620 6669 6c65  th over 256 file
-0002eac0: 7320 616e 6420 666f 6c64 6572 732c 2075  s and folders, u
-0002ead0: 706c 6f61 640a 2020 2020 2020 2020 2320  pload.        # 
-0002eae0: 6669 6c65 7320 616e 6420 666f 6c64 6572  files and folder
-0002eaf0: 7320 746f 2061 206e 6577 2062 7563 6b65  s to a new bucke
-0002eb00: 742c 2074 6865 6e20 6465 6c65 7465 2062  t, then delete b
-0002eb10: 7563 6b65 742e 0a20 2020 2020 2020 2074  ucket..        t
-0002eb20: 6d70 5f62 756c 6b5f 6465 6c5f 7374 6f72  mp_bulk_del_stor
-0002eb30: 6167 655f 6f62 6a2e 6164 645f 7374 6f72  age_obj.add_stor
-0002eb40: 6528 7374 6f72 655f 7479 7065 290a 0a20  e(store_type).. 
-0002eb50: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-0002eb60: 732e 6368 6563 6b5f 6f75 7470 7574 285b  s.check_output([
-0002eb70: 0a20 2020 2020 2020 2020 2020 2027 736b  .            'sk
-0002eb80: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
-0002eb90: 6465 6c65 7465 272c 2074 6d70 5f62 756c  delete', tmp_bul
-0002eba0: 6b5f 6465 6c5f 7374 6f72 6167 655f 6f62  k_del_storage_ob
-0002ebb0: 6a2e 6e61 6d65 2c20 272d 2d79 6573 270a  j.name, '--yes'.
-0002ebc0: 2020 2020 2020 2020 5d29 0a0a 2020 2020          ])..    
-0002ebd0: 2020 2020 6f75 7470 7574 203d 2073 7562      output = sub
-0002ebe0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-0002ebf0: 7470 7574 285b 2773 6b79 272c 2027 7374  tput(['sky', 'st
-0002ec00: 6f72 6167 6527 2c20 276c 7327 5d29 0a20  orage', 'ls']). 
-0002ec10: 2020 2020 2020 2061 7373 6572 7420 746d         assert tm
-0002ec20: 705f 6275 6c6b 5f64 656c 5f73 746f 7261  p_bulk_del_stora
-0002ec30: 6765 5f6f 626a 2e6e 616d 6520 6e6f 7420  ge_obj.name not 
-0002ec40: 696e 206f 7574 7075 742e 6465 636f 6465  in output.decode
-0002ec50: 2827 7574 662d 3827 290a 0a20 2020 2040  ('utf-8')..    @
-0002ec60: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f66  pytest.mark.no_f
-0002ec70: 6c75 6964 7374 6163 6b0a 2020 2020 4070  luidstack.    @p
-0002ec80: 7974 6573 742e 6d61 726b 2e70 6172 616d  ytest.mark.param
-0002ec90: 6574 7269 7a65 280a 2020 2020 2020 2020  etrize(.        
-0002eca0: 2774 6d70 5f70 7562 6c69 635f 7374 6f72  'tmp_public_stor
-0002ecb0: 6167 655f 6f62 6a2c 2073 746f 7265 5f74  age_obj, store_t
-0002ecc0: 7970 6527 2c0a 2020 2020 2020 2020 5b28  ype',.        [(
-0002ecd0: 2773 333a 2f2f 7463 6761 2d32 2d6f 7065  's3://tcga-2-ope
-0002ece0: 6e27 2c20 7374 6f72 6167 655f 6c69 622e  n', storage_lib.
-0002ecf0: 5374 6f72 6554 7970 652e 5333 292c 0a20  StoreType.S3),. 
-0002ed00: 2020 2020 2020 2020 2827 7333 3a2f 2f64          ('s3://d
-0002ed10: 6967 6974 616c 636f 7270 6f72 6127 2c20  igitalcorpora', 
-0002ed20: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-0002ed30: 6554 7970 652e 5333 292c 0a20 2020 2020  eType.S3),.     
-0002ed40: 2020 2020 2827 6773 3a2f 2f67 6370 2d70      ('gs://gcp-p
-0002ed50: 7562 6c69 632d 6461 7461 2d73 656e 7469  ublic-data-senti
-0002ed60: 6e65 6c2d 3227 2c20 7374 6f72 6167 655f  nel-2', storage_
-0002ed70: 6c69 622e 5374 6f72 6554 7970 652e 4743  lib.StoreType.GC
-0002ed80: 5329 5d2c 0a20 2020 2020 2020 2069 6e64  S)],.        ind
-0002ed90: 6972 6563 743d 5b27 746d 705f 7075 626c  irect=['tmp_publ
-0002eda0: 6963 5f73 746f 7261 6765 5f6f 626a 275d  ic_storage_obj']
-0002edb0: 290a 2020 2020 6465 6620 7465 7374 5f70  ).    def test_p
-0002edc0: 7562 6c69 635f 6275 636b 6574 2873 656c  ublic_bucket(sel
-0002edd0: 662c 2074 6d70 5f70 7562 6c69 635f 7374  f, tmp_public_st
-0002ede0: 6f72 6167 655f 6f62 6a2c 2073 746f 7265  orage_obj, store
-0002edf0: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
-0002ee00: 2320 4372 6561 7465 7320 6120 6e65 7720  # Creates a new 
-0002ee10: 6275 636b 6574 2077 6974 6820 6120 7075  bucket with a pu
-0002ee20: 626c 6963 2073 6f75 7263 6520 616e 6420  blic source and 
-0002ee30: 7665 7269 6669 6573 2074 6861 7420 6974  verifies that it
-0002ee40: 2069 7320 6e6f 740a 2020 2020 2020 2020   is not.        
-0002ee50: 2320 6164 6465 6420 746f 2067 6c6f 6261  # added to globa
-0002ee60: 6c5f 7573 6572 5f73 7461 7465 2e0a 2020  l_user_state..  
-0002ee70: 2020 2020 2020 746d 705f 7075 626c 6963        tmp_public
-0002ee80: 5f73 746f 7261 6765 5f6f 626a 2e61 6464  _storage_obj.add
-0002ee90: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
-0002eea0: 6529 0a0a 2020 2020 2020 2020 2320 5275  e)..        # Ru
-0002eeb0: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
-0002eec0: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
-0002eed0: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
-0002eee0: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
-0002eef0: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
-0002ef00: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
-0002ef10: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
-0002ef20: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
-0002ef30: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0002ef40: 746d 705f 7075 626c 6963 5f73 746f 7261  tmp_public_stora
-0002ef50: 6765 5f6f 626a 2e6e 616d 6520 6e6f 7420  ge_obj.name not 
-0002ef60: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
-0002ef70: 7466 2d38 2729 0a0a 2020 2020 4070 7974  tf-8')..    @pyt
-0002ef80: 6573 742e 6d61 726b 2e6e 6f5f 666c 7569  est.mark.no_flui
-0002ef90: 6473 7461 636b 0a20 2020 2040 7079 7465  dstack.    @pyte
-0002efa0: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-0002efb0: 697a 6528 276e 6f6e 6578 6973 745f 6275  ize('nonexist_bu
-0002efc0: 636b 6574 5f75 726c 272c 205b 0a20 2020  cket_url', [.   
-0002efd0: 2020 2020 2027 7333 3a2f 2f7b 7261 6e64       's3://{rand
-0002efe0: 6f6d 5f6e 616d 657d 272c 2027 6773 3a2f  om_name}', 'gs:/
-0002eff0: 2f7b 7261 6e64 6f6d 5f6e 616d 657d 272c  /{random_name}',
-0002f000: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
-0002f010: 7061 7261 6d28 2763 6f73 3a2f 2f75 732d  param('cos://us-
-0002f020: 6561 7374 2f7b 7261 6e64 6f6d 5f6e 616d  east/{random_nam
-0002f030: 657d 272c 206d 6172 6b73 3d70 7974 6573  e}', marks=pytes
-0002f040: 742e 6d61 726b 2e69 626d 292c 0a20 2020  t.mark.ibm),.   
-0002f050: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
-0002f060: 6d28 2772 323a 2f2f 7b72 616e 646f 6d5f  m('r2://{random_
-0002f070: 6e61 6d65 7d27 2c20 6d61 726b 733d 7079  name}', marks=py
-0002f080: 7465 7374 2e6d 6172 6b2e 636c 6f75 6466  test.mark.cloudf
-0002f090: 6c61 7265 290a 2020 2020 5d29 0a20 2020  lare).    ]).   
-0002f0a0: 2064 6566 2074 6573 745f 6e6f 6e65 7869   def test_nonexi
-0002f0b0: 7374 656e 745f 6275 636b 6574 2873 656c  stent_bucket(sel
-0002f0c0: 662c 206e 6f6e 6578 6973 745f 6275 636b  f, nonexist_buck
-0002f0d0: 6574 5f75 726c 293a 0a20 2020 2020 2020  et_url):.       
-0002f0e0: 2023 2041 7474 656d 7074 7320 746f 2063   # Attempts to c
-0002f0f0: 7265 6174 6520 6665 7463 6820 6120 7374  reate fetch a st
-0002f100: 726f 6167 6520 7769 7468 2061 206e 6f6e  roage with a non
-0002f110: 2d65 7869 7374 656e 7420 736f 7572 6365  -existent source
-0002f120: 2e0a 2020 2020 2020 2020 2320 4765 6e65  ..        # Gene
-0002f130: 7261 7465 2061 2072 616e 646f 6d20 6275  rate a random bu
-0002f140: 636b 6574 206e 616d 6520 616e 6420 7665  cket name and ve
-0002f150: 7269 6679 2069 7420 646f 6573 6e27 7420  rify it doesn't 
-0002f160: 6578 6973 743a 0a20 2020 2020 2020 2072  exist:.        r
-0002f170: 6574 7279 5f63 6f75 6e74 203d 2030 0a20  etry_count = 0. 
-0002f180: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-0002f190: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-0002f1a0: 6f6e 6578 6973 745f 6275 636b 6574 5f6e  onexist_bucket_n
-0002f1b0: 616d 6520 3d20 7374 7228 7575 6964 2e75  ame = str(uuid.u
-0002f1c0: 7569 6434 2829 290a 2020 2020 2020 2020  uid4()).        
-0002f1d0: 2020 2020 6966 206e 6f6e 6578 6973 745f      if nonexist_
-0002f1e0: 6275 636b 6574 5f75 726c 2e73 7461 7274  bucket_url.start
-0002f1f0: 7377 6974 6828 2773 3327 293a 0a20 2020  swith('s3'):.   
-0002f200: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-0002f210: 6d61 6e64 203d 2066 2761 7773 2073 3361  mand = f'aws s3a
-0002f220: 7069 2068 6561 642d 6275 636b 6574 202d  pi head-bucket -
-0002f230: 2d62 7563 6b65 7420 7b6e 6f6e 6578 6973  -bucket {nonexis
-0002f240: 745f 6275 636b 6574 5f6e 616d 657d 270a  t_bucket_name}'.
-0002f250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f260: 6578 7065 6374 6564 5f6f 7574 7075 7420  expected_output 
-0002f270: 3d20 2734 3034 270a 2020 2020 2020 2020  = '404'.        
-0002f280: 2020 2020 656c 6966 206e 6f6e 6578 6973      elif nonexis
-0002f290: 745f 6275 636b 6574 5f75 726c 2e73 7461  t_bucket_url.sta
-0002f2a0: 7274 7377 6974 6828 2767 7327 293a 0a20  rtswith('gs'):. 
-0002f2b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0002f2c0: 6f6d 6d61 6e64 203d 2066 2767 7375 7469  ommand = f'gsuti
-0002f2d0: 6c20 6c73 207b 6e6f 6e65 7869 7374 5f62  l ls {nonexist_b
-0002f2e0: 7563 6b65 745f 7572 6c2e 666f 726d 6174  ucket_url.format
-0002f2f0: 2872 616e 646f 6d5f 6e61 6d65 3d6e 6f6e  (random_name=non
-0002f300: 6578 6973 745f 6275 636b 6574 5f6e 616d  exist_bucket_nam
-0002f310: 6529 7d27 0a20 2020 2020 2020 2020 2020  e)}'.           
-0002f320: 2020 2020 2065 7870 6563 7465 645f 6f75       expected_ou
-0002f330: 7470 7574 203d 2027 4275 636b 6574 4e6f  tput = 'BucketNo
-0002f340: 7446 6f75 6e64 4578 6365 7074 696f 6e27  tFoundException'
-0002f350: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0002f360: 6620 6e6f 6e65 7869 7374 5f62 7563 6b65  f nonexist_bucke
-0002f370: 745f 7572 6c2e 7374 6172 7473 7769 7468  t_url.startswith
-0002f380: 2827 7232 2729 3a0a 2020 2020 2020 2020  ('r2'):.        
-0002f390: 2020 2020 2020 2020 656e 6470 6f69 6e74          endpoint
-0002f3a0: 5f75 726c 203d 2063 6c6f 7564 666c 6172  _url = cloudflar
-0002f3b0: 652e 6372 6561 7465 5f65 6e64 706f 696e  e.create_endpoin
-0002f3c0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0002f3d0: 2020 2020 636f 6d6d 616e 6420 3d20 6627      command = f'
-0002f3e0: 4157 535f 5348 4152 4544 5f43 5245 4445  AWS_SHARED_CREDE
-0002f3f0: 4e54 4941 4c53 5f46 494c 453d 7b63 6c6f  NTIALS_FILE={clo
-0002f400: 7564 666c 6172 652e 5232 5f43 5245 4445  udflare.R2_CREDE
-0002f410: 4e54 4941 4c53 5f50 4154 487d 2061 7773  NTIALS_PATH} aws
-0002f420: 2073 3361 7069 2068 6561 642d 6275 636b   s3api head-buck
-0002f430: 6574 202d 2d62 7563 6b65 7420 7b6e 6f6e  et --bucket {non
-0002f440: 6578 6973 745f 6275 636b 6574 5f6e 616d  exist_bucket_nam
-0002f450: 657d 202d 2d65 6e64 706f 696e 7420 7b65  e} --endpoint {e
-0002f460: 6e64 706f 696e 745f 7572 6c7d 202d 2d70  ndpoint_url} --p
-0002f470: 726f 6669 6c65 3d72 3227 0a20 2020 2020  rofile=r2'.     
-0002f480: 2020 2020 2020 2020 2020 2065 7870 6563             expec
-0002f490: 7465 645f 6f75 7470 7574 203d 2027 3430  ted_output = '40
-0002f4a0: 3427 0a20 2020 2020 2020 2020 2020 2065  4'.            e
-0002f4b0: 6c69 6620 6e6f 6e65 7869 7374 5f62 7563  lif nonexist_buc
-0002f4c0: 6b65 745f 7572 6c2e 7374 6172 7473 7769  ket_url.startswi
-0002f4d0: 7468 2827 636f 7327 293a 0a20 2020 2020  th('cos'):.     
-0002f4e0: 2020 2020 2020 2020 2020 2023 2055 7369             # Usi
-0002f4f0: 6e67 2041 5049 2063 616c 6c73 2c20 7369  ng API calls, si
-0002f500: 6e63 6520 7573 696e 6720 7263 6c6f 6e65  nce using rclone
-0002f510: 2072 6571 7569 7265 7320 6120 7072 6f66   requires a prof
-0002f520: 696c 6527 7320 6e61 6d65 0a20 2020 2020  ile's name.     
-0002f530: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0002f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f550: 2020 2020 6578 7065 6374 6564 5f6f 7574      expected_out
-0002f560: 7075 7420 3d20 636f 6d6d 616e 6420 3d20  put = command = 
-0002f570: 2265 6368 6f22 2020 2320 6176 6f69 6420  "echo"  # avoid 
-0002f580: 756e 7265 6c61 7465 6420 6578 6365 7074  unrelated except
-0002f590: 696f 6e20 696e 2063 6173 6520 6f66 2066  ion in case of f
-0002f5a0: 6169 6c75 7265 2e0a 2020 2020 2020 2020  ailure..        
-0002f5b0: 2020 2020 2020 2020 2020 2020 6275 636b              buck
-0002f5c0: 6574 5f6e 616d 6520 3d20 7572 6c6c 6962  et_name = urllib
-0002f5d0: 2e70 6172 7365 2e75 726c 7370 6c69 7428  .parse.urlsplit(
-0002f5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f5f0: 2020 2020 2020 2020 206e 6f6e 6578 6973           nonexis
-0002f600: 745f 6275 636b 6574 5f75 726c 2e66 6f72  t_bucket_url.for
-0002f610: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-0002f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f630: 2072 616e 646f 6d5f 6e61 6d65 3d6e 6f6e   random_name=non
-0002f640: 6578 6973 745f 6275 636b 6574 5f6e 616d  exist_bucket_nam
-0002f650: 6529 292e 7061 7468 2e73 7472 6970 2827  e)).path.strip('
-0002f660: 2f27 290a 2020 2020 2020 2020 2020 2020  /').            
-0002f670: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
-0002f680: 2069 626d 2e67 6574 5f63 6f73 5f63 6c69   ibm.get_cos_cli
-0002f690: 656e 7428 2775 732d 6561 7374 2729 0a20  ent('us-east'). 
-0002f6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f6b0: 2020 2063 6c69 656e 742e 6865 6164 5f62     client.head_b
-0002f6c0: 7563 6b65 7428 4275 636b 6574 3d62 7563  ucket(Bucket=buc
-0002f6d0: 6b65 745f 6e61 6d65 290a 2020 2020 2020  ket_name).      
-0002f6e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0002f6f0: 2069 626d 2e69 626d 5f62 6f74 6f63 6f72   ibm.ibm_botocor
-0002f700: 652e 6578 6365 7074 696f 6e73 2e43 6c69  e.exceptions.Cli
-0002f710: 656e 7445 7272 6f72 2061 7320 653a 0a20  entError as e:. 
-0002f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f730: 2020 2069 6620 652e 7265 7370 6f6e 7365     if e.response
-0002f740: 5b27 4572 726f 7227 5d5b 2743 6f64 6527  ['Error']['Code'
-0002f750: 5d20 3d3d 2027 3430 3427 3a0a 2020 2020  ] == '404':.    
-0002f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f770: 2020 2020 2320 7375 6363 6573 730a 2020      # success.  
-0002f780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f790: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0002f7a0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0002f7b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0002f7c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0002f7d0: 2755 6e73 7570 706f 7274 6564 2062 7563  'Unsupported buc
-0002f7e0: 6b65 7420 7479 7065 2027 0a20 2020 2020  ket type '.     
-0002f7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f800: 2020 2020 2020 2020 2020 2020 6627 7b6e              f'{n
-0002f810: 6f6e 6578 6973 745f 6275 636b 6574 5f75  onexist_bucket_u
-0002f820: 726c 7d27 290a 0a20 2020 2020 2020 2020  rl}')..         
-0002f830: 2020 2023 2043 6865 636b 2069 6620 6275     # Check if bu
-0002f840: 636b 6574 2065 7869 7374 7320 7573 696e  cket exists usin
-0002f850: 6720 7468 6520 636c 693a 0a20 2020 2020  g the cli:.     
-0002f860: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0002f870: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-0002f880: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
-0002f890: 636b 5f6f 7574 7075 7428 636f 6d6d 616e  ck_output(comman
-0002f8a0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0002f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f8d0: 2073 7464 6572 723d 7375 6270 726f 6365   stderr=subproce
-0002f8e0: 7373 2e53 5444 4f55 542c 0a20 2020 2020  ss.STDOUT,.     
-0002f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f910: 2020 2020 2020 2020 2073 6865 6c6c 3d54           shell=T
-0002f920: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0002f930: 2065 7863 6570 7420 7375 6270 726f 6365   except subproce
-0002f940: 7373 2e43 616c 6c65 6450 726f 6365 7373  ss.CalledProcess
-0002f950: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-0002f960: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-0002f970: 3d20 652e 6f75 7470 7574 0a20 2020 2020  = e.output.     
-0002f980: 2020 2020 2020 206f 7574 203d 206f 7574         out = out
-0002f990: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-0002f9a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0002f9b0: 6578 7065 6374 6564 5f6f 7574 7075 7420  expected_output 
-0002f9c0: 696e 206f 7574 3a0a 2020 2020 2020 2020  in out:.        
-0002f9d0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-0002f9e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0002f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002fa00: 7265 7472 795f 636f 756e 7420 2b3d 2031  retry_count += 1
-0002fa10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002fa20: 2069 6620 7265 7472 795f 636f 756e 7420   if retry_count 
-0002fa30: 3e20 333a 0a20 2020 2020 2020 2020 2020  > 3:.           
-0002fa40: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
-0002fa50: 756e 7469 6d65 4572 726f 7228 2755 6e61  untimeError('Una
-0002fa60: 626c 6520 746f 2066 696e 6420 6120 6e6f  ble to find a no
-0002fa70: 6e65 7869 7374 656e 7420 6275 636b 6574  nexistent bucket
-0002fa80: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-0002fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002faa0: 2020 2020 2020 2020 2020 2774 6f20 7573            'to us
-0002fab0: 652e 2054 6869 7320 6973 2068 6967 6c79  e. This is higly
-0002fac0: 2075 6e6c 696b 656c 7920 2d20 270a 2020   unlikely - '.  
-0002fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025220: 3d6e 616d 6529 7d3b 2027 0a20 2020 2020  =name)}; '.     
+00025230: 2020 2020 2020 2027 7079 7468 6f6e 3320         'python3 
+00025240: 7465 7374 732f 736b 7973 6572 7665 2f73  tests/skyserve/s
+00025250: 7472 6561 6d69 6e67 2f73 656e 645f 7374  treaming/send_st
+00025260: 7265 616d 696e 675f 7265 7175 6573 742e  reaming_request.
+00025270: 7079 2027 0a20 2020 2020 2020 2020 2020  py '.           
+00025280: 2027 2d2d 656e 6470 6f69 6e74 2024 656e   '--endpoint $en
+00025290: 6470 6f69 6e74 207c 2067 7265 7020 2253  dpoint | grep "S
+000252a0: 7472 6561 6d69 6e67 2074 6573 7420 7061  treaming test pa
+000252b0: 7373 6564 2227 2c0a 2020 2020 2020 2020  ssed"',.        
+000252c0: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
+000252d0: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
+000252e0: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
+000252f0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00025300: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
+00025310: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00025320: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00025330: 6d61 726b 2e73 6572 7665 0a64 6566 2074  mark.serve.def t
+00025340: 6573 745f 736b 7973 6572 7665 5f75 7064  est_skyserve_upd
+00025350: 6174 6528 6765 6e65 7269 635f 636c 6f75  ate(generic_clou
+00025360: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
+00025370: 5465 7374 2073 6b79 7365 7276 6520 7769  Test skyserve wi
+00025380: 7468 2075 7064 6174 6522 2222 0a20 2020  th update""".   
+00025390: 206e 616d 6520 3d20 5f67 6574 5f73 6572   name = _get_ser
+000253a0: 7669 6365 5f6e 616d 6528 290a 2020 2020  vice_name().    
+000253b0: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+000253c0: 2020 2020 2066 2774 6573 742d 736b 7973       f'test-skys
+000253d0: 6572 7665 2d75 7064 6174 6527 2c0a 2020  erve-update',.  
+000253e0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+000253f0: 2020 2020 6627 736b 7920 7365 7276 6520      f'sky serve 
+00025400: 7570 202d 6e20 7b6e 616d 657d 202d 2d63  up -n {name} --c
+00025410: 6c6f 7564 207b 6765 6e65 7269 635f 636c  loud {generic_cl
+00025420: 6f75 647d 202d 7920 7465 7374 732f 736b  oud} -y tests/sk
+00025430: 7973 6572 7665 2f75 7064 6174 652f 6f6c  yserve/update/ol
+00025440: 642e 7961 6d6c 272c 0a20 2020 2020 2020  d.yaml',.       
+00025450: 2020 2020 205f 5345 5256 455f 5741 4954       _SERVE_WAIT
+00025460: 5f55 4e54 494c 5f52 4541 4459 2e66 6f72  _UNTIL_READY.for
+00025470: 6d61 7428 6e61 6d65 3d6e 616d 652c 2072  mat(name=name, r
+00025480: 6570 6c69 6361 5f6e 756d 3d32 292c 0a20  eplica_num=2),. 
+00025490: 2020 2020 2020 2020 2020 2066 277b 5f53             f'{_S
+000254a0: 4552 5645 5f45 4e44 504f 494e 545f 5741  ERVE_ENDPOINT_WA
+000254b0: 4954 2e66 6f72 6d61 7428 6e61 6d65 3d6e  IT.format(name=n
+000254c0: 616d 6529 7d3b 2063 7572 6c20 6874 7470  ame)}; curl http
+000254d0: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
+000254e0: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
+000254f0: 7420 6865 7265 2227 2c0a 2020 2020 2020  t here"',.      
+00025500: 2020 2020 2020 6627 736b 7920 7365 7276        f'sky serv
+00025510: 6520 7570 6461 7465 207b 6e61 6d65 7d20  e update {name} 
+00025520: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+00025530: 5f63 6c6f 7564 7d20 2d2d 6d6f 6465 2062  _cloud} --mode b
+00025540: 6c75 655f 6772 6565 6e20 2d79 2074 6573  lue_green -y tes
+00025550: 7473 2f73 6b79 7365 7276 652f 7570 6461  ts/skyserve/upda
+00025560: 7465 2f6e 6577 2e79 616d 6c27 2c0a 2020  te/new.yaml',.  
+00025570: 2020 2020 2020 2020 2020 2320 736c 6565            # slee
+00025580: 7020 6265 666f 7265 2075 7064 6174 6520  p before update 
+00025590: 6973 2072 6567 6973 7465 7265 642e 0a20  is registered.. 
+000255a0: 2020 2020 2020 2020 2020 2027 736c 6565             'slee
+000255b0: 7020 3230 272c 0a20 2020 2020 2020 2020  p 20',.         
+000255c0: 2020 2066 277b 5f53 4552 5645 5f45 4e44     f'{_SERVE_END
+000255d0: 504f 494e 545f 5741 4954 2e66 6f72 6d61  POINT_WAIT.forma
+000255e0: 7428 6e61 6d65 3d6e 616d 6529 7d3b 2027  t(name=name)}; '
+000255f0: 0a20 2020 2020 2020 2020 2020 2027 756e  .            'un
+00025600: 7469 6c20 6375 726c 2068 7474 703a 2f2f  til curl http://
+00025610: 2465 6e64 706f 696e 7420 7c20 6772 6570  $endpoint | grep
+00025620: 2022 4869 2c20 6e65 7720 536b 7950 696c   "Hi, new SkyPil
+00025630: 6f74 2068 6572 6521 223b 2064 6f20 736c  ot here!"; do sl
+00025640: 6565 7020 323b 2064 6f6e 653b 270a 2020  eep 2; done;'.  
+00025650: 2020 2020 2020 2020 2020 2320 4d61 6b65            # Make
+00025660: 2073 7572 6520 7468 6520 7472 6166 6669   sure the traffi
+00025670: 6320 6973 206e 6f74 206d 6978 6564 0a20  c is not mixed. 
+00025680: 2020 2020 2020 2020 2020 2027 6375 726c             'curl
+00025690: 2068 7474 703a 2f2f 2465 6e64 706f 696e   http://$endpoin
+000256a0: 7420 7c20 6772 6570 2022 4869 2c20 6e65  t | grep "Hi, ne
+000256b0: 7720 536b 7950 696c 6f74 2068 6572 6522  w SkyPilot here"
+000256c0: 272c 0a20 2020 2020 2020 2020 2020 2023  ',.            #
+000256d0: 2054 6865 206c 6174 6573 7420 3220 7665   The latest 2 ve
+000256e0: 7273 696f 6e20 7368 6f75 6c64 2062 6520  rsion should be 
+000256f0: 5245 4144 5920 616e 6420 7468 6520 6f6c  READY and the ol
+00025700: 6465 7220 7665 7273 696f 6e73 2073 686f  der versions sho
+00025710: 756c 6420 6265 2073 6875 7474 696e 6720  uld be shutting 
+00025720: 646f 776e 0a20 2020 2020 2020 2020 2020  down.           
+00025730: 2028 5f63 6865 636b 5f72 6570 6c69 6361   (_check_replica
+00025740: 5f69 6e5f 7374 6174 7573 286e 616d 652c  _in_status(name,
+00025750: 205b 2832 2c20 4661 6c73 652c 2027 5245   [(2, False, 'RE
+00025760: 4144 5927 292c 0a20 2020 2020 2020 2020  ADY'),.         
+00025770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025790: 2020 2020 2832 2c20 4661 6c73 652c 2027      (2, False, '
+000257a0: 5348 5554 5449 4e47 5f44 4f57 4e27 295d  SHUTTING_DOWN')]
+000257b0: 2920 2b0a 2020 2020 2020 2020 2020 2020  ) +.            
+000257c0: 205f 6368 6563 6b5f 7365 7276 6963 655f   _check_service_
+000257d0: 7665 7273 696f 6e28 6e61 6d65 2c20 2232  version(name, "2
+000257e0: 2229 292c 0a20 2020 2020 2020 205d 2c0a  ")),.        ],.
+000257f0: 2020 2020 2020 2020 5f54 4541 5244 4f57          _TEARDOW
+00025800: 4e5f 5345 5256 4943 452e 666f 726d 6174  N_SERVICE.format
+00025810: 286e 616d 653d 6e61 6d65 292c 0a20 2020  (name=name),.   
+00025820: 2020 2020 2074 696d 656f 7574 3d32 3020       timeout=20 
+00025830: 2a20 3630 2c0a 2020 2020 290a 2020 2020  * 60,.    ).    
+00025840: 7275 6e5f 6f6e 655f 7465 7374 2874 6573  run_one_test(tes
+00025850: 7429 0a0a 0a40 7079 7465 7374 2e6d 6172  t)...@pytest.mar
+00025860: 6b2e 7365 7276 650a 6465 6620 7465 7374  k.serve.def test
+00025870: 5f73 6b79 7365 7276 655f 726f 6c6c 696e  _skyserve_rollin
+00025880: 675f 7570 6461 7465 2867 656e 6572 6963  g_update(generic
+00025890: 5f63 6c6f 7564 3a20 7374 7229 3a0a 2020  _cloud: str):.  
+000258a0: 2020 2222 2254 6573 7420 736b 7973 6572    """Test skyser
+000258b0: 7665 2077 6974 6820 726f 6c6c 696e 6720  ve with rolling 
+000258c0: 7570 6461 7465 2222 220a 2020 2020 6e61  update""".    na
+000258d0: 6d65 203d 205f 6765 745f 7365 7276 6963  me = _get_servic
+000258e0: 655f 6e61 6d65 2829 0a20 2020 2073 696e  e_name().    sin
+000258f0: 676c 655f 6e65 775f 7265 706c 6963 6120  gle_new_replica 
+00025900: 3d20 5f63 6865 636b 5f72 6570 6c69 6361  = _check_replica
+00025910: 5f69 6e5f 7374 6174 7573 280a 2020 2020  _in_status(.    
+00025920: 2020 2020 6e61 6d65 2c20 5b28 322c 2046      name, [(2, F
+00025930: 616c 7365 2c20 2752 4541 4459 2729 2c20  alse, 'READY'), 
+00025940: 2831 2c20 4661 6c73 652c 205f 5345 5256  (1, False, _SERV
+00025950: 4943 455f 4c41 554e 4348 494e 475f 5354  ICE_LAUNCHING_ST
+00025960: 4154 5553 5f52 4547 4558 292c 0a20 2020  ATUS_REGEX),.   
+00025970: 2020 2020 2020 2020 2020 2020 2831 2c20              (1, 
+00025980: 4661 6c73 652c 2027 5348 5554 5449 4e47  False, 'SHUTTING
+00025990: 5f44 4f57 4e27 295d 290a 2020 2020 7465  _DOWN')]).    te
+000259a0: 7374 203d 2054 6573 7428 0a20 2020 2020  st = Test(.     
+000259b0: 2020 2066 2774 6573 742d 736b 7973 6572     f'test-skyser
+000259c0: 7665 2d72 6f6c 6c69 6e67 2d75 7064 6174  ve-rolling-updat
+000259d0: 6527 2c0a 2020 2020 2020 2020 5b0a 2020  e',.        [.  
+000259e0: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+000259f0: 7365 7276 6520 7570 202d 6e20 7b6e 616d  serve up -n {nam
+00025a00: 657d 202d 2d63 6c6f 7564 207b 6765 6e65  e} --cloud {gene
+00025a10: 7269 635f 636c 6f75 647d 202d 7920 7465  ric_cloud} -y te
+00025a20: 7374 732f 736b 7973 6572 7665 2f75 7064  sts/skyserve/upd
+00025a30: 6174 652f 6f6c 642e 7961 6d6c 272c 0a20  ate/old.yaml',. 
+00025a40: 2020 2020 2020 2020 2020 205f 5345 5256             _SERV
+00025a50: 455f 5741 4954 5f55 4e54 494c 5f52 4541  E_WAIT_UNTIL_REA
+00025a60: 4459 2e66 6f72 6d61 7428 6e61 6d65 3d6e  DY.format(name=n
+00025a70: 616d 652c 2072 6570 6c69 6361 5f6e 756d  ame, replica_num
+00025a80: 3d32 292c 0a20 2020 2020 2020 2020 2020  =2),.           
+00025a90: 2066 277b 5f53 4552 5645 5f45 4e44 504f   f'{_SERVE_ENDPO
+00025aa0: 494e 545f 5741 4954 2e66 6f72 6d61 7428  INT_WAIT.format(
+00025ab0: 6e61 6d65 3d6e 616d 6529 7d3b 2063 7572  name=name)}; cur
+00025ac0: 6c20 6874 7470 3a2f 2f24 656e 6470 6f69  l http://$endpoi
+00025ad0: 6e74 207c 2067 7265 7020 2248 692c 2053  nt | grep "Hi, S
+00025ae0: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
+00025af0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00025b00: 7920 7365 7276 6520 7570 6461 7465 207b  y serve update {
+00025b10: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
+00025b20: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
+00025b30: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
+00025b40: 7570 6461 7465 2f6e 6577 2e79 616d 6c27  update/new.yaml'
+00025b50: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00025b60: 4d61 6b65 2073 7572 6520 7468 6520 7472  Make sure the tr
+00025b70: 6166 6669 6320 6973 206d 6978 6564 2061  affic is mixed a
+00025b80: 6372 6f73 7320 7477 6f20 7665 7273 696f  cross two versio
+00025b90: 6e73 2c20 7468 6520 7265 706c 6963 6173  ns, the replicas
+00025ba0: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+00025bb0: 6974 6820 6576 656e 2069 6420 7769 6c6c  ith even id will
+00025bc0: 2073 6c65 6570 2036 3020 7365 636f 6e64   sleep 60 second
+00025bd0: 7320 6265 666f 7265 2062 6569 6e67 2072  s before being r
+00025be0: 6561 6479 2c20 736f 2077 650a 2020 2020  eady, so we.    
+00025bf0: 2020 2020 2020 2020 2320 7368 6f75 6c64          # should
+00025c00: 2062 6520 6162 6c65 2074 6f20 6765 7420   be able to get 
+00025c10: 6f62 7365 7276 6520 7468 6520 7065 7269  observe the peri
+00025c20: 6f64 2074 6861 7420 7468 6520 7472 6166  od that the traf
+00025c30: 6669 6320 6973 206d 6978 6564 0a20 2020  fic is mixed.   
+00025c40: 2020 2020 2020 2020 2023 2061 6372 6f73           # acros
+00025c50: 7320 7477 6f20 7665 7273 696f 6e73 2e0a  s two versions..
+00025c60: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00025c70: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
+00025c80: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
+00025c90: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
+00025ca0: 2020 2020 2020 2775 6e74 696c 2063 7572        'until cur
+00025cb0: 6c20 6874 7470 3a2f 2f24 656e 6470 6f69  l http://$endpoi
+00025cc0: 6e74 207c 2067 7265 7020 2248 692c 206e  nt | grep "Hi, n
+00025cd0: 6577 2053 6b79 5069 6c6f 7420 6865 7265  ew SkyPilot here
+00025ce0: 2122 3b20 646f 2073 6c65 6570 2032 3b20  !"; do sleep 2; 
+00025cf0: 646f 6e65 3b20 736c 6565 7020 323b 2027  done; sleep 2; '
+00025d00: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00025d10: 6865 206c 6174 6573 7420 7665 7273 696f  he latest versio
+00025d20: 6e20 7368 6f75 6c64 2068 6176 6520 6f6e  n should have on
+00025d30: 6520 5245 4144 5920 616e 6420 7468 6520  e READY and the 
+00025d40: 6f6e 6520 6f66 2074 6865 206f 6c64 6572  one of the older
+00025d50: 2076 6572 7369 6f6e 7320 7368 6f75 6c64   versions should
+00025d60: 2062 6520 7368 7574 7469 6e67 2064 6f77   be shutting dow
+00025d70: 6e0a 2020 2020 2020 2020 2020 2020 6627  n.            f'
+00025d80: 7b73 696e 676c 655f 6e65 775f 7265 706c  {single_new_repl
+00025d90: 6963 617d 207b 5f63 6865 636b 5f73 6572  ica} {_check_ser
+00025da0: 7669 6365 5f76 6572 7369 6f6e 286e 616d  vice_version(nam
+00025db0: 652c 2022 312c 3222 297d 2027 0a20 2020  e, "1,2")} '.   
+00025dc0: 2020 2020 2020 2020 2023 2043 6865 636b           # Check
+00025dd0: 2074 6865 206f 7574 7075 7420 6672 6f6d   the output from
+00025de0: 2074 6865 206f 6c64 2076 6572 7369 6f6e   the old version
+00025df0: 2c20 696d 6d65 6469 6174 656c 7920 6166  , immediately af
+00025e00: 7465 7220 7468 650a 2020 2020 2020 2020  ter the.        
+00025e10: 2020 2020 2320 6f75 7470 7574 2066 726f      # output fro
+00025e20: 6d20 7468 6520 6e65 7720 7665 7273 696f  m the new versio
+00025e30: 6e20 6170 7065 6172 732e 2054 6869 7320  n appears. This 
+00025e40: 6973 2067 7561 7261 6e74 6565 6420 6279  is guaranteed by
+00025e50: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00025e60: 2023 2072 6f75 6e64 2072 6f62 696e 206c   # round robin l
+00025e70: 6f61 6420 6261 6c61 6e63 696e 6720 706f  oad balancing po
+00025e80: 6c69 6379 2e0a 2020 2020 2020 2020 2020  licy..          
+00025e90: 2020 2320 544f 444f 287a 6877 7529 3a20    # TODO(zhwu): 
+00025ea0: 7765 2073 686f 756c 6420 6861 7665 2061  we should have a
+00025eb0: 206d 6f72 6520 6765 6e65 7261 6c69 7a65   more generalize
+00025ec0: 6420 7761 7920 666f 7220 6368 6563 6b69  d way for checki
+00025ed0: 6e67 2074 6865 0a20 2020 2020 2020 2020  ng the.         
+00025ee0: 2020 2023 206d 6978 6564 2076 6572 7369     # mixed versi
+00025ef0: 6f6e 206f 6620 7265 706c 6963 6173 2074  on of replicas t
+00025f00: 6f20 6176 6f69 6420 6465 7065 6e64 696e  o avoid dependin
+00025f10: 6720 6f6e 2074 6865 2073 7065 6369 6669  g on the specifi
+00025f20: 630a 2020 2020 2020 2020 2020 2020 2320  c.            # 
+00025f30: 726f 756e 6420 726f 6269 6e20 6c6f 6164  round robin load
+00025f40: 2062 616c 616e 6369 6e67 2070 6f6c 6963   balancing polic
+00025f50: 792e 0a20 2020 2020 2020 2020 2020 2027  y..            '
+00025f60: 6375 726c 2068 7474 703a 2f2f 2465 6e64  curl http://$end
+00025f70: 706f 696e 7420 7c20 6772 6570 2022 4869  point | grep "Hi
+00025f80: 2c20 536b 7950 696c 6f74 2068 6572 6522  , SkyPilot here"
+00025f90: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
+00025fa0: 2020 2020 2020 5f54 4541 5244 4f57 4e5f        _TEARDOWN_
+00025fb0: 5345 5256 4943 452e 666f 726d 6174 286e  SERVICE.format(n
+00025fc0: 616d 653d 6e61 6d65 292c 0a20 2020 2020  ame=name),.     
+00025fd0: 2020 2074 696d 656f 7574 3d32 3020 2a20     timeout=20 * 
+00025fe0: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00025ff0: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00026000: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00026010: 7365 7276 650a 6465 6620 7465 7374 5f73  serve.def test_s
+00026020: 6b79 7365 7276 655f 6661 7374 5f75 7064  kyserve_fast_upd
+00026030: 6174 6528 6765 6e65 7269 635f 636c 6f75  ate(generic_clou
+00026040: 643a 2073 7472 293a 0a20 2020 2022 2222  d: str):.    """
+00026050: 5465 7374 2073 6b79 7365 7276 6520 7769  Test skyserve wi
+00026060: 7468 2066 6173 7420 7570 6461 7465 2028  th fast update (
+00026070: 496e 6372 656d 656e 7420 7665 7273 696f  Increment versio
+00026080: 6e20 6f66 206f 6c64 2072 6570 6c69 6361  n of old replica
+00026090: 7329 2222 220a 2020 2020 6e61 6d65 203d  s)""".    name =
+000260a0: 205f 6765 745f 7365 7276 6963 655f 6e61   _get_service_na
+000260b0: 6d65 2829 0a0a 2020 2020 7465 7374 203d  me()..    test =
+000260c0: 2054 6573 7428 0a20 2020 2020 2020 2066   Test(.        f
+000260d0: 2774 6573 742d 736b 7973 6572 7665 2d66  'test-skyserve-f
+000260e0: 6173 742d 7570 6461 7465 272c 0a20 2020  ast-update',.   
+000260f0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00026100: 2020 2066 2773 6b79 2073 6572 7665 2075     f'sky serve u
+00026110: 7020 2d6e 207b 6e61 6d65 7d20 2d79 202d  p -n {name} -y -
+00026120: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
+00026130: 636c 6f75 647d 2074 6573 7473 2f73 6b79  cloud} tests/sky
+00026140: 7365 7276 652f 7570 6461 7465 2f62 756d  serve/update/bum
+00026150: 705f 7665 7273 696f 6e5f 6265 666f 7265  p_version_before
+00026160: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
+00026170: 2020 2020 5f53 4552 5645 5f57 4149 545f      _SERVE_WAIT_
+00026180: 554e 5449 4c5f 5245 4144 592e 666f 726d  UNTIL_READY.form
+00026190: 6174 286e 616d 653d 6e61 6d65 2c20 7265  at(name=name, re
+000261a0: 706c 6963 615f 6e75 6d3d 3229 2c0a 2020  plica_num=2),.  
+000261b0: 2020 2020 2020 2020 2020 6627 7b5f 5345            f'{_SE
+000261c0: 5256 455f 454e 4450 4f49 4e54 5f57 4149  RVE_ENDPOINT_WAI
+000261d0: 542e 666f 726d 6174 286e 616d 653d 6e61  T.format(name=na
+000261e0: 6d65 297d 3b20 6375 726c 2068 7474 703a  me)}; curl http:
+000261f0: 2f2f 2465 6e64 706f 696e 7420 7c20 6772  //$endpoint | gr
+00026200: 6570 2022 4869 2c20 536b 7950 696c 6f74  ep "Hi, SkyPilot
+00026210: 2068 6572 6522 272c 0a20 2020 2020 2020   here"',.       
+00026220: 2020 2020 2066 2773 6b79 2073 6572 7665       f'sky serve
+00026230: 2075 7064 6174 6520 7b6e 616d 657d 202d   update {name} -
+00026240: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
+00026250: 636c 6f75 647d 202d 2d6d 6f64 6520 626c  cloud} --mode bl
+00026260: 7565 5f67 7265 656e 202d 7920 7465 7374  ue_green -y test
+00026270: 732f 736b 7973 6572 7665 2f75 7064 6174  s/skyserve/updat
+00026280: 652f 6275 6d70 5f76 6572 7369 6f6e 5f61  e/bump_version_a
+00026290: 6674 6572 2e79 616d 6c27 2c0a 2020 2020  fter.yaml',.    
+000262a0: 2020 2020 2020 2020 2320 736c 6565 7020          # sleep 
+000262b0: 746f 2077 6169 7420 666f 7220 7570 6461  to wait for upda
+000262c0: 7465 2074 6f20 6265 2072 6567 6973 7465  te to be registe
+000262d0: 7265 642e 0a20 2020 2020 2020 2020 2020  red..           
+000262e0: 2027 736c 6565 7020 3330 272c 0a20 2020   'sleep 30',.   
+000262f0: 2020 2020 2020 2020 2023 2032 206f 6e2d           # 2 on-
+00026300: 6465 616d 6e64 2028 7265 6164 7929 202b  deamnd (ready) +
+00026310: 2031 206f 6e2d 6465 6d61 6e64 2028 7072   1 on-demand (pr
+00026320: 6f76 6973 696f 6e69 6e67 292e 0a20 2020  ovisioning)..   
+00026330: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+00026340: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
+00026350: 6b5f 7265 706c 6963 615f 696e 5f73 7461  k_replica_in_sta
+00026360: 7475 7328 0a20 2020 2020 2020 2020 2020  tus(.           
+00026370: 2020 2020 2020 2020 206e 616d 652c 205b           name, [
+00026380: 2832 2c20 4661 6c73 652c 2027 5245 4144  (2, False, 'READ
+00026390: 5927 292c 0a20 2020 2020 2020 2020 2020  Y'),.           
+000263a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263b0: 2831 2c20 4661 6c73 652c 205f 5345 5256  (1, False, _SERV
+000263c0: 4943 455f 4c41 554e 4348 494e 475f 5354  ICE_LAUNCHING_ST
+000263d0: 4154 5553 5f52 4547 4558 295d 2920 2b0a  ATUS_REGEX)]) +.
+000263e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263f0: 2320 4661 7374 2075 7064 6174 6520 7769  # Fast update wi
+00026400: 6c6c 2064 6972 6563 746c 7920 6861 7665  ll directly have
+00026410: 2074 6865 206c 6174 6573 7420 7665 7273   the latest vers
+00026420: 696f 6e20 7265 6164 792e 0a20 2020 2020  ion ready..     
+00026430: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
+00026440: 6b5f 7365 7276 6963 655f 7665 7273 696f  k_service_versio
+00026450: 6e28 6e61 6d65 2c20 2232 2229 292c 0a20  n(name, "2")),. 
+00026460: 2020 2020 2020 2020 2020 205f 5345 5256             _SERV
+00026470: 455f 5741 4954 5f55 4e54 494c 5f52 4541  E_WAIT_UNTIL_REA
+00026480: 4459 2e66 6f72 6d61 7428 6e61 6d65 3d6e  DY.format(name=n
+00026490: 616d 652c 2072 6570 6c69 6361 5f6e 756d  ame, replica_num
+000264a0: 3d33 2920 2b0a 2020 2020 2020 2020 2020  =3) +.          
+000264b0: 2020 5f63 6865 636b 5f73 6572 7669 6365    _check_service
+000264c0: 5f76 6572 7369 6f6e 286e 616d 652c 2022  _version(name, "
+000264d0: 3222 292c 0a20 2020 2020 2020 2020 2020  2"),.           
+000264e0: 2066 277b 5f53 4552 5645 5f45 4e44 504f   f'{_SERVE_ENDPO
+000264f0: 494e 545f 5741 4954 2e66 6f72 6d61 7428  INT_WAIT.format(
+00026500: 6e61 6d65 3d6e 616d 6529 7d3b 2063 7572  name=name)}; cur
+00026510: 6c20 6874 7470 3a2f 2f24 656e 6470 6f69  l http://$endpoi
+00026520: 6e74 207c 2067 7265 7020 2248 692c 2053  nt | grep "Hi, S
+00026530: 6b79 5069 6c6f 7420 6865 7265 2227 2c0a  kyPilot here"',.
+00026540: 2020 2020 2020 2020 2020 2020 2320 5465              # Te
+00026550: 7374 2072 6f6c 6c69 6e67 2075 7064 6174  st rolling updat
+00026560: 650a 2020 2020 2020 2020 2020 2020 6627  e.            f'
+00026570: 736b 7920 7365 7276 6520 7570 6461 7465  sky serve update
+00026580: 207b 6e61 6d65 7d20 2d2d 636c 6f75 6420   {name} --cloud 
+00026590: 7b67 656e 6572 6963 5f63 6c6f 7564 7d20  {generic_cloud} 
+000265a0: 2d79 2074 6573 7473 2f73 6b79 7365 7276  -y tests/skyserv
+000265b0: 652f 7570 6461 7465 2f62 756d 705f 7665  e/update/bump_ve
+000265c0: 7273 696f 6e5f 6265 666f 7265 2e79 616d  rsion_before.yam
+000265d0: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
+000265e0: 2320 736c 6565 7020 746f 2077 6169 7420  # sleep to wait 
+000265f0: 666f 7220 7570 6461 7465 2074 6f20 6265  for update to be
+00026600: 2072 6567 6973 7465 7265 642e 0a20 2020   registered..   
+00026610: 2020 2020 2020 2020 2027 736c 6565 7020           'sleep 
+00026620: 3135 272c 0a20 2020 2020 2020 2020 2020  15',.           
+00026630: 2023 2032 206f 6e2d 6465 616d 6e64 2028   # 2 on-deamnd (
+00026640: 7265 6164 7929 202b 2031 206f 6e2d 6465  ready) + 1 on-de
+00026650: 6d61 6e64 2028 7368 7574 7469 6e67 2064  mand (shutting d
+00026660: 6f77 6e29 2e0a 2020 2020 2020 2020 2020  own)..          
+00026670: 2020 5f63 6865 636b 5f72 6570 6c69 6361    _check_replica
+00026680: 5f69 6e5f 7374 6174 7573 286e 616d 652c  _in_status(name,
+00026690: 205b 2832 2c20 4661 6c73 652c 2027 5245   [(2, False, 'RE
+000266a0: 4144 5927 292c 0a20 2020 2020 2020 2020  ADY'),.         
+000266b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000266c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000266d0: 2020 2028 312c 2046 616c 7365 2c20 2753     (1, False, 'S
+000266e0: 4855 5454 494e 475f 444f 574e 2729 5d29  HUTTING_DOWN')])
+000266f0: 2c0a 2020 2020 2020 2020 2020 2020 5f53  ,.            _S
+00026700: 4552 5645 5f57 4149 545f 554e 5449 4c5f  ERVE_WAIT_UNTIL_
+00026710: 5245 4144 592e 666f 726d 6174 286e 616d  READY.format(nam
+00026720: 653d 6e61 6d65 2c20 7265 706c 6963 615f  e=name, replica_
+00026730: 6e75 6d3d 3229 202b 0a20 2020 2020 2020  num=2) +.       
+00026740: 2020 2020 205f 6368 6563 6b5f 7365 7276       _check_serv
+00026750: 6963 655f 7665 7273 696f 6e28 6e61 6d65  ice_version(name
+00026760: 2c20 2233 2229 2c0a 2020 2020 2020 2020  , "3"),.        
+00026770: 2020 2020 6627 7b5f 5345 5256 455f 454e      f'{_SERVE_EN
+00026780: 4450 4f49 4e54 5f57 4149 542e 666f 726d  DPOINT_WAIT.form
+00026790: 6174 286e 616d 653d 6e61 6d65 297d 3b20  at(name=name)}; 
+000267a0: 6375 726c 2068 7474 703a 2f2f 2465 6e64  curl http://$end
+000267b0: 706f 696e 7420 7c20 6772 6570 2022 4869  point | grep "Hi
+000267c0: 2c20 536b 7950 696c 6f74 2068 6572 6522  , SkyPilot here"
+000267d0: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
+000267e0: 2020 2020 2020 5f54 4541 5244 4f57 4e5f        _TEARDOWN_
+000267f0: 5345 5256 4943 452e 666f 726d 6174 286e  SERVICE.format(n
+00026800: 616d 653d 6e61 6d65 292c 0a20 2020 2020  ame=name),.     
+00026810: 2020 2074 696d 656f 7574 3d33 3020 2a20     timeout=30 * 
+00026820: 3630 2c0a 2020 2020 290a 2020 2020 7275  60,.    ).    ru
+00026830: 6e5f 6f6e 655f 7465 7374 2874 6573 7429  n_one_test(test)
+00026840: 0a0a 0a40 7079 7465 7374 2e6d 6172 6b2e  ...@pytest.mark.
+00026850: 7365 7276 650a 6465 6620 7465 7374 5f73  serve.def test_s
+00026860: 6b79 7365 7276 655f 7570 6461 7465 5f61  kyserve_update_a
+00026870: 7574 6f73 6361 6c65 2867 656e 6572 6963  utoscale(generic
+00026880: 5f63 6c6f 7564 3a20 7374 7229 3a0a 2020  _cloud: str):.  
+00026890: 2020 2222 2254 6573 7420 736b 7973 6572    """Test skyser
+000268a0: 7665 2075 7064 6174 6520 7769 7468 2061  ve update with a
+000268b0: 7574 6f73 6361 6c65 2222 220a 2020 2020  utoscale""".    
+000268c0: 6e61 6d65 203d 205f 6765 745f 7365 7276  name = _get_serv
+000268d0: 6963 655f 6e61 6d65 2829 0a20 2020 2074  ice_name().    t
+000268e0: 6573 7420 3d20 5465 7374 280a 2020 2020  est = Test(.    
+000268f0: 2020 2020 6627 7465 7374 2d73 6b79 7365      f'test-skyse
+00026900: 7276 652d 7570 6461 7465 2d61 7574 6f73  rve-update-autos
+00026910: 6361 6c65 272c 0a20 2020 2020 2020 205b  cale',.        [
+00026920: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00026930: 6b79 2073 6572 7665 2075 7020 2d6e 207b  ky serve up -n {
+00026940: 6e61 6d65 7d20 2d2d 636c 6f75 6420 7b67  name} --cloud {g
+00026950: 656e 6572 6963 5f63 6c6f 7564 7d20 2d79  eneric_cloud} -y
+00026960: 2074 6573 7473 2f73 6b79 7365 7276 652f   tests/skyserve/
+00026970: 7570 6461 7465 2f6e 756d 5f6d 696e 5f74  update/num_min_t
+00026980: 776f 2e79 616d 6c27 2c0a 2020 2020 2020  wo.yaml',.      
+00026990: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
+000269a0: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
+000269b0: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
+000269c0: 7265 706c 6963 615f 6e75 6d3d 3229 202b  replica_num=2) +
+000269d0: 0a20 2020 2020 2020 2020 2020 205f 6368  .            _ch
+000269e0: 6563 6b5f 7365 7276 6963 655f 7665 7273  eck_service_vers
+000269f0: 696f 6e28 6e61 6d65 2c20 2231 2229 2c0a  ion(name, "1"),.
+00026a00: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00026a10: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
+00026a20: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
+00026a30: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
+00026a40: 2020 2020 2020 2763 7572 6c20 6874 7470        'curl http
+00026a50: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
+00026a60: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
+00026a70: 7420 6865 7265 2227 2c0a 2020 2020 2020  t here"',.      
+00026a80: 2020 2020 2020 6627 736b 7920 7365 7276        f'sky serv
+00026a90: 6520 7570 6461 7465 207b 6e61 6d65 7d20  e update {name} 
+00026aa0: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+00026ab0: 5f63 6c6f 7564 7d20 2d2d 6d6f 6465 2062  _cloud} --mode b
+00026ac0: 6c75 655f 6772 6565 6e20 2d79 2074 6573  lue_green -y tes
+00026ad0: 7473 2f73 6b79 7365 7276 652f 7570 6461  ts/skyserve/upda
+00026ae0: 7465 2f6e 756d 5f6d 696e 5f6f 6e65 2e79  te/num_min_one.y
+00026af0: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+00026b00: 2020 2320 736c 6565 7020 6265 666f 7265    # sleep before
+00026b10: 2075 7064 6174 6520 6973 2072 6567 6973   update is regis
+00026b20: 7465 7265 642e 0a20 2020 2020 2020 2020  tered..         
+00026b30: 2020 2027 736c 6565 7020 3230 272c 0a20     'sleep 20',. 
+00026b40: 2020 2020 2020 2020 2020 2023 2054 696d             # Tim
+00026b50: 656f 7574 2077 696c 6c20 6265 2074 7269  eout will be tri
+00026b60: 6767 6572 6564 2077 6865 6e20 7570 6461  ggered when upda
+00026b70: 7465 2066 6169 6c73 2e0a 2020 2020 2020  te fails..      
+00026b80: 2020 2020 2020 5f53 4552 5645 5f57 4149        _SERVE_WAI
+00026b90: 545f 554e 5449 4c5f 5245 4144 592e 666f  T_UNTIL_READY.fo
+00026ba0: 726d 6174 286e 616d 653d 6e61 6d65 2c20  rmat(name=name, 
+00026bb0: 7265 706c 6963 615f 6e75 6d3d 3129 202b  replica_num=1) +
+00026bc0: 0a20 2020 2020 2020 2020 2020 205f 6368  .            _ch
+00026bd0: 6563 6b5f 7365 7276 6963 655f 7665 7273  eck_service_vers
+00026be0: 696f 6e28 6e61 6d65 2c20 2232 2229 2c0a  ion(name, "2"),.
+00026bf0: 2020 2020 2020 2020 2020 2020 6627 7b5f              f'{_
+00026c00: 5345 5256 455f 454e 4450 4f49 4e54 5f57  SERVE_ENDPOINT_W
+00026c10: 4149 542e 666f 726d 6174 286e 616d 653d  AIT.format(name=
+00026c20: 6e61 6d65 297d 3b20 270a 2020 2020 2020  name)}; '.      
+00026c30: 2020 2020 2020 2763 7572 6c20 6874 7470        'curl http
+00026c40: 3a2f 2f24 656e 6470 6f69 6e74 207c 2067  ://$endpoint | g
+00026c50: 7265 7020 2248 692c 2053 6b79 5069 6c6f  rep "Hi, SkyPilo
+00026c60: 7420 6865 7265 2122 272c 0a20 2020 2020  t here!"',.     
+00026c70: 2020 2020 2020 2023 2052 6f6c 6c69 6e67         # Rolling
+00026c80: 2055 7064 6174 650a 2020 2020 2020 2020   Update.        
+00026c90: 2020 2020 6627 736b 7920 7365 7276 6520      f'sky serve 
+00026ca0: 7570 6461 7465 207b 6e61 6d65 7d20 2d2d  update {name} --
+00026cb0: 636c 6f75 6420 7b67 656e 6572 6963 5f63  cloud {generic_c
+00026cc0: 6c6f 7564 7d20 2d79 2074 6573 7473 2f73  loud} -y tests/s
+00026cd0: 6b79 7365 7276 652f 7570 6461 7465 2f6e  kyserve/update/n
+00026ce0: 756d 5f6d 696e 5f74 776f 2e79 616d 6c27  um_min_two.yaml'
+00026cf0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00026d00: 736c 6565 7020 6265 666f 7265 2075 7064  sleep before upd
+00026d10: 6174 6520 6973 2072 6567 6973 7465 7265  ate is registere
+00026d20: 642e 0a20 2020 2020 2020 2020 2020 2027  d..            '
+00026d30: 736c 6565 7020 3230 272c 0a20 2020 2020  sleep 20',.     
+00026d40: 2020 2020 2020 2023 2054 696d 656f 7574         # Timeout
+00026d50: 2077 696c 6c20 6265 2074 7269 6767 6572   will be trigger
+00026d60: 6564 2077 6865 6e20 7570 6461 7465 2066  ed when update f
+00026d70: 6169 6c73 2e0a 2020 2020 2020 2020 2020  ails..          
+00026d80: 2020 5f53 4552 5645 5f57 4149 545f 554e    _SERVE_WAIT_UN
+00026d90: 5449 4c5f 5245 4144 592e 666f 726d 6174  TIL_READY.format
+00026da0: 286e 616d 653d 6e61 6d65 2c20 7265 706c  (name=name, repl
+00026db0: 6963 615f 6e75 6d3d 3229 202b 0a20 2020  ica_num=2) +.   
+00026dc0: 2020 2020 2020 2020 205f 6368 6563 6b5f           _check_
+00026dd0: 7365 7276 6963 655f 7665 7273 696f 6e28  service_version(
+00026de0: 6e61 6d65 2c20 2233 2229 2c0a 2020 2020  name, "3"),.    
+00026df0: 2020 2020 2020 2020 6627 7b5f 5345 5256          f'{_SERV
+00026e00: 455f 454e 4450 4f49 4e54 5f57 4149 542e  E_ENDPOINT_WAIT.
+00026e10: 666f 726d 6174 286e 616d 653d 6e61 6d65  format(name=name
+00026e20: 297d 3b20 270a 2020 2020 2020 2020 2020  )}; '.          
+00026e30: 2020 2763 7572 6c20 6874 7470 3a2f 2f24    'curl http://$
+00026e40: 656e 6470 6f69 6e74 207c 2067 7265 7020  endpoint | grep 
+00026e50: 2248 692c 2053 6b79 5069 6c6f 7420 6865  "Hi, SkyPilot he
+00026e60: 7265 2122 272c 0a20 2020 2020 2020 205d  re!"',.        ]
+00026e70: 2c0a 2020 2020 2020 2020 5f54 4541 5244  ,.        _TEARD
+00026e80: 4f57 4e5f 5345 5256 4943 452e 666f 726d  OWN_SERVICE.form
+00026e90: 6174 286e 616d 653d 6e61 6d65 292c 0a20  at(name=name),. 
+00026ea0: 2020 2020 2020 2074 696d 656f 7574 3d33         timeout=3
+00026eb0: 3020 2a20 3630 2c0a 2020 2020 290a 2020  0 * 60,.    ).  
+00026ec0: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
+00026ed0: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
+00026ee0: 6172 6b2e 7365 7276 650a 4070 7974 6573  ark.serve.@pytes
+00026ef0: 742e 6d61 726b 2e6e 6f5f 6b75 6265 726e  t.mark.no_kubern
+00026f00: 6574 6573 2020 2320 5370 6f74 2069 6e73  etes  # Spot ins
+00026f10: 7461 6e63 6573 2061 7265 206e 6f74 2073  tances are not s
+00026f20: 7570 706f 7274 6564 2069 6e20 4b75 6265  upported in Kube
+00026f30: 726e 6574 6573 0a40 7079 7465 7374 2e6d  rnetes.@pytest.m
+00026f40: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00026f50: 276d 6f64 6527 2c20 5b27 726f 6c6c 696e  'mode', ['rollin
+00026f60: 6727 2c20 2762 6c75 655f 6772 6565 6e27  g', 'blue_green'
+00026f70: 5d29 0a64 6566 2074 6573 745f 736b 7973  ]).def test_skys
+00026f80: 6572 7665 5f6e 6577 5f61 7574 6f73 6361  erve_new_autosca
+00026f90: 6c65 725f 7570 6461 7465 286d 6f64 653a  ler_update(mode:
+00026fa0: 2073 7472 2c20 6765 6e65 7269 635f 636c   str, generic_cl
+00026fb0: 6f75 643a 2073 7472 293a 0a20 2020 2022  oud: str):.    "
+00026fc0: 2222 5465 7374 2073 6b79 7365 7276 6520  ""Test skyserve 
+00026fd0: 7769 7468 2075 7064 6174 6520 7468 6174  with update that
+00026fe0: 2063 6861 6e67 6573 2061 7574 6f73 6361   changes autosca
+00026ff0: 6c65 7222 2222 0a20 2020 206e 616d 6520  ler""".    name 
+00027000: 3d20 5f67 6574 5f73 6572 7669 6365 5f6e  = _get_service_n
+00027010: 616d 6528 2920 2b20 6d6f 6465 0a0a 2020  ame() + mode..  
+00027020: 2020 666f 7572 5f73 706f 745f 7570 5f63    four_spot_up_c
+00027030: 6d64 203d 205f 6368 6563 6b5f 7265 706c  md = _check_repl
+00027040: 6963 615f 696e 5f73 7461 7475 7328 6e61  ica_in_status(na
+00027050: 6d65 2c20 5b28 342c 2054 7275 652c 2027  me, [(4, True, '
+00027060: 5245 4144 5927 295d 290a 2020 2020 7570  READY')]).    up
+00027070: 6461 7465 5f63 6865 636b 203d 205b 6627  date_check = [f'
+00027080: 756e 7469 6c20 287b 666f 7572 5f73 706f  until ({four_spo
+00027090: 745f 7570 5f63 6d64 7d29 3b20 646f 2073  t_up_cmd}); do s
+000270a0: 6c65 6570 2035 3b20 646f 6e65 3b20 736c  leep 5; done; sl
+000270b0: 6565 7020 3130 3b27 5d0a 2020 2020 6966  eep 10;'].    if
+000270c0: 206d 6f64 6520 3d3d 2027 726f 6c6c 696e   mode == 'rollin
+000270d0: 6727 3a0a 2020 2020 2020 2020 2320 4368  g':.        # Ch
+000270e0: 6563 6b20 726f 6c6c 696e 6720 7570 6461  eck rolling upda
+000270f0: 7465 2c20 6974 2077 696c 6c20 7465 726d  te, it will term
+00027100: 696e 6174 6520 6f6e 6520 6f66 2074 6865  inate one of the
+00027110: 206f 6c64 206f 6e2d 6465 6d61 6e64 0a20   old on-demand. 
+00027120: 2020 2020 2020 2023 2069 6e73 7461 6e63         # instanc
+00027130: 6573 2c20 6f6e 6365 2074 6865 7265 2061  es, once there a
+00027140: 7265 2034 2073 706f 7420 696e 7374 616e  re 4 spot instan
+00027150: 6365 2072 6561 6479 2e0a 2020 2020 2020  ce ready..      
+00027160: 2020 7570 6461 7465 5f63 6865 636b 202b    update_check +
+00027170: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00027180: 5f63 6865 636b 5f72 6570 6c69 6361 5f69  _check_replica_i
+00027190: 6e5f 7374 6174 7573 280a 2020 2020 2020  n_status(.      
+000271a0: 2020 2020 2020 2020 2020 6e61 6d65 2c20            name, 
+000271b0: 5b28 312c 2046 616c 7365 2c20 5f53 4552  [(1, False, _SER
+000271c0: 5649 4345 5f4c 4155 4e43 4849 4e47 5f53  VICE_LAUNCHING_S
+000271d0: 5441 5455 535f 5245 4745 5829 2c0a 2020  TATUS_REGEX),.  
+000271e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000271f0: 2020 2020 2028 312c 2046 616c 7365 2c20       (1, False, 
+00027200: 2753 4855 5454 494e 475f 444f 574e 2729  'SHUTTING_DOWN')
+00027210: 2c20 2831 2c20 4661 6c73 652c 2027 5245  , (1, False, 'RE
+00027220: 4144 5927 295d 2920 2b0a 2020 2020 2020  ADY')]) +.      
+00027230: 2020 2020 2020 5f63 6865 636b 5f73 6572        _check_ser
+00027240: 7669 6365 5f76 6572 7369 6f6e 286e 616d  vice_version(nam
+00027250: 652c 2022 312c 3222 292c 0a20 2020 2020  e, "1,2"),.     
+00027260: 2020 205d 0a20 2020 2065 6c73 653a 0a20     ].    else:. 
+00027270: 2020 2020 2020 2023 2043 6865 636b 2062         # Check b
+00027280: 6c75 6520 6772 6565 6e20 7570 6461 7465  lue green update
+00027290: 2c20 6974 2077 696c 6c20 6b65 6570 2062  , it will keep b
+000272a0: 6f74 6820 6f6c 6420 6f6e 2d64 656d 616e  oth old on-deman
+000272b0: 6420 696e 7374 616e 6365 730a 2020 2020  d instances.    
+000272c0: 2020 2020 2320 7275 6e6e 696e 672c 206f      # running, o
+000272d0: 6e63 6520 7468 6572 6520 6172 6520 3420  nce there are 4 
+000272e0: 7370 6f74 2069 6e73 7461 6e63 6520 7265  spot instance re
+000272f0: 6164 792e 0a20 2020 2020 2020 2075 7064  ady..        upd
+00027300: 6174 655f 6368 6563 6b20 2b3d 205b 0a20  ate_check += [. 
+00027310: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
+00027320: 6b5f 7265 706c 6963 615f 696e 5f73 7461  k_replica_in_sta
+00027330: 7475 7328 0a20 2020 2020 2020 2020 2020  tus(.           
+00027340: 2020 2020 206e 616d 652c 205b 2831 2c20       name, [(1, 
+00027350: 4661 6c73 652c 205f 5345 5256 4943 455f  False, _SERVICE_
+00027360: 4c41 554e 4348 494e 475f 5354 4154 5553  LAUNCHING_STATUS
+00027370: 5f52 4547 4558 292c 0a20 2020 2020 2020  _REGEX),.       
+00027380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027390: 2832 2c20 4661 6c73 652c 2027 5245 4144  (2, False, 'READ
+000273a0: 5927 295d 2920 2b0a 2020 2020 2020 2020  Y')]) +.        
+000273b0: 2020 2020 5f63 6865 636b 5f73 6572 7669      _check_servi
+000273c0: 6365 5f76 6572 7369 6f6e 286e 616d 652c  ce_version(name,
+000273d0: 2022 3122 292c 0a20 2020 2020 2020 205d   "1"),.        ]
+000273e0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
+000273f0: 280a 2020 2020 2020 2020 2774 6573 742d  (.        'test-
+00027400: 736b 7973 6572 7665 2d6e 6577 2d61 7574  skyserve-new-aut
+00027410: 6f73 6361 6c65 722d 7570 6461 7465 272c  oscaler-update',
+00027420: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00027430: 2020 2020 2020 2066 2773 6b79 2073 6572         f'sky ser
+00027440: 7665 2075 7020 2d6e 207b 6e61 6d65 7d20  ve up -n {name} 
+00027450: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+00027460: 5f63 6c6f 7564 7d20 2d79 2074 6573 7473  _cloud} -y tests
+00027470: 2f73 6b79 7365 7276 652f 7570 6461 7465  /skyserve/update
+00027480: 2f6e 6577 5f61 7574 6f73 6361 6c65 725f  /new_autoscaler_
+00027490: 6265 666f 7265 2e79 616d 6c27 2c0a 2020  before.yaml',.  
+000274a0: 2020 2020 2020 2020 2020 5f53 4552 5645            _SERVE
+000274b0: 5f57 4149 545f 554e 5449 4c5f 5245 4144  _WAIT_UNTIL_READ
+000274c0: 592e 666f 726d 6174 286e 616d 653d 6e61  Y.format(name=na
+000274d0: 6d65 2c20 7265 706c 6963 615f 6e75 6d3d  me, replica_num=
+000274e0: 3229 202b 0a20 2020 2020 2020 2020 2020  2) +.           
+000274f0: 205f 6368 6563 6b5f 7365 7276 6963 655f   _check_service_
+00027500: 7665 7273 696f 6e28 6e61 6d65 2c20 2231  version(name, "1
+00027510: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00027520: 6627 7b5f 5345 5256 455f 454e 4450 4f49  f'{_SERVE_ENDPOI
+00027530: 4e54 5f57 4149 542e 666f 726d 6174 286e  NT_WAIT.format(n
+00027540: 616d 653d 6e61 6d65 297d 3b20 270a 2020  ame=name)}; '.  
+00027550: 2020 2020 2020 2020 2020 2773 3d24 2863            's=$(c
+00027560: 7572 6c20 6874 7470 3a2f 2f24 656e 6470  url http://$endp
+00027570: 6f69 6e74 293b 2065 6368 6f20 2224 7322  oint); echo "$s"
+00027580: 3b20 6563 686f 2022 2473 2220 7c20 6772  ; echo "$s" | gr
+00027590: 6570 2022 4869 2c20 536b 7950 696c 6f74  ep "Hi, SkyPilot
+000275a0: 2068 6572 6522 272c 0a20 2020 2020 2020   here"',.       
+000275b0: 2020 2020 2066 2773 6b79 2073 6572 7665       f'sky serve
+000275c0: 2075 7064 6174 6520 7b6e 616d 657d 202d   update {name} -
+000275d0: 2d63 6c6f 7564 207b 6765 6e65 7269 635f  -cloud {generic_
+000275e0: 636c 6f75 647d 202d 2d6d 6f64 6520 7b6d  cloud} --mode {m
+000275f0: 6f64 657d 202d 7920 7465 7374 732f 736b  ode} -y tests/sk
+00027600: 7973 6572 7665 2f75 7064 6174 652f 6e65  yserve/update/ne
+00027610: 775f 6175 746f 7363 616c 6572 5f61 6674  w_autoscaler_aft
+00027620: 6572 2e79 616d 6c27 2c0a 2020 2020 2020  er.yaml',.      
+00027630: 2020 2020 2020 2320 5761 6974 2066 6f72        # Wait for
+00027640: 2075 7064 6174 6520 746f 2062 6520 7265   update to be re
+00027650: 6769 7374 6572 6564 0a20 2020 2020 2020  gistered.       
+00027660: 2020 2020 2066 2773 6c65 6570 2031 3230       f'sleep 120
+00027670: 272c 0a20 2020 2020 2020 2020 2020 205f  ',.            _
+00027680: 6368 6563 6b5f 7265 706c 6963 615f 696e  check_replica_in
+00027690: 5f73 7461 7475 7328 0a20 2020 2020 2020  _status(.       
+000276a0: 2020 2020 2020 2020 206e 616d 652c 205b           name, [
+000276b0: 2834 2c20 5472 7565 2c20 5f53 4552 5649  (4, True, _SERVI
+000276c0: 4345 5f4c 4155 4e43 4849 4e47 5f53 5441  CE_LAUNCHING_STA
+000276d0: 5455 535f 5245 4745 5820 2b20 275c 7c52  TUS_REGEX + '\|R
+000276e0: 4541 4459 2729 2c0a 2020 2020 2020 2020  EADY'),.        
+000276f0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00027700: 312c 2046 616c 7365 2c20 5f53 4552 5649  1, False, _SERVI
+00027710: 4345 5f4c 4155 4e43 4849 4e47 5f53 5441  CE_LAUNCHING_STA
+00027720: 5455 535f 5245 4745 5829 2c0a 2020 2020  TUS_REGEX),.    
+00027730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027740: 2020 2028 322c 2046 616c 7365 2c20 2752     (2, False, 'R
+00027750: 4541 4459 2729 5d29 2c0a 2020 2020 2020  EADY')]),.      
+00027760: 2020 2020 2020 2a75 7064 6174 655f 6368        *update_ch
+00027770: 6563 6b2c 0a20 2020 2020 2020 2020 2020  eck,.           
+00027780: 205f 5345 5256 455f 5741 4954 5f55 4e54   _SERVE_WAIT_UNT
+00027790: 494c 5f52 4541 4459 2e66 6f72 6d61 7428  IL_READY.format(
+000277a0: 6e61 6d65 3d6e 616d 652c 2072 6570 6c69  name=name, repli
+000277b0: 6361 5f6e 756d 3d35 292c 0a20 2020 2020  ca_num=5),.     
+000277c0: 2020 2020 2020 2066 277b 5f53 4552 5645         f'{_SERVE
+000277d0: 5f45 4e44 504f 494e 545f 5741 4954 2e66  _ENDPOINT_WAIT.f
+000277e0: 6f72 6d61 7428 6e61 6d65 3d6e 616d 6529  ormat(name=name)
+000277f0: 7d3b 2027 0a20 2020 2020 2020 2020 2020  }; '.           
+00027800: 2027 6375 726c 2068 7474 703a 2f2f 2465   'curl http://$e
+00027810: 6e64 706f 696e 7420 7c20 6772 6570 2022  ndpoint | grep "
+00027820: 4869 2c20 536b 7950 696c 6f74 2068 6572  Hi, SkyPilot her
+00027830: 6522 272c 0a20 2020 2020 2020 2020 2020  e"',.           
+00027840: 205f 6368 6563 6b5f 7265 706c 6963 615f   _check_replica_
+00027850: 696e 5f73 7461 7475 7328 6e61 6d65 2c20  in_status(name, 
+00027860: 5b28 342c 2054 7275 652c 2027 5245 4144  [(4, True, 'READ
+00027870: 5927 292c 0a20 2020 2020 2020 2020 2020  Y'),.           
+00027880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000278a0: 2028 312c 2046 616c 7365 2c20 2752 4541   (1, False, 'REA
+000278b0: 4459 2729 5d29 2c0a 2020 2020 2020 2020  DY')]),.        
+000278c0: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
+000278d0: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
+000278e0: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
+000278f0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00027900: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
+00027910: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00027920: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00027930: 6d61 726b 2e73 6572 7665 0a64 6566 2074  mark.serve.def t
+00027940: 6573 745f 736b 7973 6572 7665 5f66 6169  est_skyserve_fai
+00027950: 6c75 7265 7328 6765 6e65 7269 635f 636c  lures(generic_cl
+00027960: 6f75 643a 2073 7472 293a 0a20 2020 2022  oud: str):.    "
+00027970: 2222 5465 7374 2072 6570 6c69 6361 2066  ""Test replica f
+00027980: 6169 6c75 7265 2073 7461 7475 7365 7322  ailure statuses"
+00027990: 2222 0a20 2020 206e 616d 6520 3d20 5f67  "".    name = _g
+000279a0: 6574 5f73 6572 7669 6365 5f6e 616d 6528  et_service_name(
+000279b0: 290a 0a20 2020 2074 6573 7420 3d20 5465  )..    test = Te
+000279c0: 7374 280a 2020 2020 2020 2020 2774 6573  st(.        'tes
+000279d0: 742d 736b 7973 6572 7665 2d66 6169 6c75  t-skyserve-failu
+000279e0: 7265 7327 2c0a 2020 2020 2020 2020 5b0a  res',.        [.
+000279f0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+00027a00: 7920 7365 7276 6520 7570 202d 6e20 7b6e  y serve up -n {n
+00027a10: 616d 657d 202d 2d63 6c6f 7564 207b 6765  ame} --cloud {ge
+00027a20: 6e65 7269 635f 636c 6f75 647d 202d 7920  neric_cloud} -y 
+00027a30: 7465 7374 732f 736b 7973 6572 7665 2f66  tests/skyserve/f
+00027a40: 6169 6c75 7265 732f 696e 6974 6961 6c5f  ailures/initial_
+00027a50: 6465 6c61 792e 7961 6d6c 272c 0a20 2020  delay.yaml',.   
+00027a60: 2020 2020 2020 2020 2066 2773 3d24 2873           f's=$(s
+00027a70: 6b79 2073 6572 7665 2073 7461 7475 7320  ky serve status 
+00027a80: 7b6e 616d 657d 293b 2027 0a20 2020 2020  {name}); '.     
+00027a90: 2020 2020 2020 2066 2775 6e74 696c 2065         f'until e
+00027aa0: 6368 6f20 2224 7322 207c 2067 7265 7020  cho "$s" | grep 
+00027ab0: 2246 4149 4c45 445f 494e 4954 4941 4c5f  "FAILED_INITIAL_
+00027ac0: 4445 4c41 5922 3b20 646f 2027 0a20 2020  DELAY"; do '.   
+00027ad0: 2020 2020 2020 2020 2027 6563 686f 2022           'echo "
+00027ae0: 5761 6974 696e 6720 666f 7220 7265 706c  Waiting for repl
+00027af0: 6963 6120 746f 2062 6520 6661 696c 6564  ica to be failed
+00027b00: 2e2e 2e22 3b20 736c 6565 7020 353b 2027  ..."; sleep 5; '
+00027b10: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00027b20: 3d24 2873 6b79 2073 6572 7665 2073 7461  =$(sky serve sta
+00027b30: 7475 7320 7b6e 616d 657d 293b 2065 6368  tus {name}); ech
+00027b40: 6f20 2224 7322 3b20 646f 6e65 3b27 2c0a  o "$s"; done;',.
+00027b50: 2020 2020 2020 2020 2020 2020 2773 6c65              'sle
+00027b60: 6570 2036 3027 2c0a 2020 2020 2020 2020  ep 60',.        
+00027b70: 2020 2020 6627 7b5f 5345 5256 455f 5354      f'{_SERVE_ST
+00027b80: 4154 5553 5f57 4149 542e 666f 726d 6174  ATUS_WAIT.format
+00027b90: 286e 616d 653d 6e61 6d65 297d 3b20 6563  (name=name)}; ec
+00027ba0: 686f 2022 2473 2220 7c20 6772 6570 2022  ho "$s" | grep "
+00027bb0: 7b6e 616d 657d 2220 7c20 6772 6570 2022  {name}" | grep "
+00027bc0: 4641 494c 4544 5f49 4e49 5449 414c 5f44  FAILED_INITIAL_D
+00027bd0: 454c 4159 2220 7c20 7763 202d 6c20 7c20  ELAY" | wc -l | 
+00027be0: 6772 6570 2032 3b20 270a 2020 2020 2020  grep 2; '.      
+00027bf0: 2020 2020 2020 2320 4d61 6b65 2073 7572        # Make sur
+00027c00: 6520 6e6f 206e 6577 2072 6570 6c69 6361  e no new replica
+00027c10: 7320 6172 6520 7374 6172 7465 6420 666f  s are started fo
+00027c20: 7220 6561 726c 7920 6661 696c 7572 652e  r early failure.
+00027c30: 0a20 2020 2020 2020 2020 2020 2066 2765  .            f'e
+00027c40: 6368 6f20 2224 7322 207c 2067 7265 7020  cho "$s" | grep 
+00027c50: 2d41 2031 3030 2022 5365 7276 6963 6520  -A 100 "Service 
+00027c60: 5265 706c 6963 6173 2220 7c20 6772 6570  Replicas" | grep
+00027c70: 2022 7b6e 616d 657d 2220 7c20 7763 202d   "{name}" | wc -
+00027c80: 6c20 7c20 6772 6570 2032 3b27 2c0a 2020  l | grep 2;',.  
+00027c90: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00027ca0: 7365 7276 6520 7570 6461 7465 207b 6e61  serve update {na
+00027cb0: 6d65 7d20 2d2d 636c 6f75 6420 7b67 656e  me} --cloud {gen
+00027cc0: 6572 6963 5f63 6c6f 7564 7d20 2d79 2074  eric_cloud} -y t
+00027cd0: 6573 7473 2f73 6b79 7365 7276 652f 6661  ests/skyserve/fa
+00027ce0: 696c 7572 6573 2f70 726f 6269 6e67 2e79  ilures/probing.y
+00027cf0: 616d 6c27 2c0a 2020 2020 2020 2020 2020  aml',.          
+00027d00: 2020 6627 733d 2428 736b 7920 7365 7276    f's=$(sky serv
+00027d10: 6520 7374 6174 7573 207b 6e61 6d65 7d29  e status {name})
+00027d20: 3b20 270a 2020 2020 2020 2020 2020 2020  ; '.            
+00027d30: 2320 5761 6974 2066 6f72 2072 6570 6c69  # Wait for repli
+00027d40: 6361 2074 6f20 6265 2072 6561 6479 2e0a  ca to be ready..
+00027d50: 2020 2020 2020 2020 2020 2020 6627 756e              f'un
+00027d60: 7469 6c20 6563 686f 2022 2473 2220 7c20  til echo "$s" | 
+00027d70: 6772 6570 2022 5245 4144 5922 3b20 646f  grep "READY"; do
+00027d80: 2027 0a20 2020 2020 2020 2020 2020 2027   '.            '
+00027d90: 6563 686f 2022 5761 6974 696e 6720 666f  echo "Waiting fo
+00027da0: 7220 7265 706c 6963 6120 746f 2062 6520  r replica to be 
+00027db0: 6661 696c 6564 2e2e 2e22 3b20 736c 6565  failed..."; slee
+00027dc0: 7020 353b 2027 0a20 2020 2020 2020 2020  p 5; '.         
+00027dd0: 2020 2066 2773 3d24 2873 6b79 2073 6572     f's=$(sky ser
+00027de0: 7665 2073 7461 7475 7320 7b6e 616d 657d  ve status {name}
+00027df0: 293b 2065 6368 6f20 2224 7322 3b20 646f  ); echo "$s"; do
+00027e00: 6e65 3b27 2c0a 2020 2020 2020 2020 2020  ne;',.          
+00027e10: 2020 2320 5761 6974 2066 6f72 2072 6570    # Wait for rep
+00027e20: 6c69 6361 2074 6f20 6368 616e 6765 2074  lica to change t
+00027e30: 6f20 4641 494c 4544 5f50 524f 4249 4e47  o FAILED_PROBING
+00027e40: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00027e50: 3d24 2873 6b79 2073 6572 7665 2073 7461  =$(sky serve sta
+00027e60: 7475 7320 7b6e 616d 657d 293b 2027 0a20  tus {name}); '. 
+00027e70: 2020 2020 2020 2020 2020 2066 2775 6e74             f'unt
+00027e80: 696c 2065 6368 6f20 2224 7322 207c 2067  il echo "$s" | g
+00027e90: 7265 7020 2246 4149 4c45 445f 5052 4f42  rep "FAILED_PROB
+00027ea0: 494e 4722 3b20 646f 2027 0a20 2020 2020  ING"; do '.     
+00027eb0: 2020 2020 2020 2027 6563 686f 2022 5761         'echo "Wa
+00027ec0: 6974 696e 6720 666f 7220 7265 706c 6963  iting for replic
+00027ed0: 6120 746f 2062 6520 6661 696c 6564 2e2e  a to be failed..
+00027ee0: 2e22 3b20 736c 6565 7020 353b 2027 0a20  ."; sleep 5; '. 
+00027ef0: 2020 2020 2020 2020 2020 2066 2773 3d24             f's=$
+00027f00: 2873 6b79 2073 6572 7665 2073 7461 7475  (sky serve statu
+00027f10: 7320 7b6e 616d 657d 293b 2065 6368 6f20  s {name}); echo 
+00027f20: 2224 7322 3b20 646f 6e65 3b27 202b 0a20  "$s"; done;' +. 
+00027f30: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
+00027f40: 6b5f 7265 706c 6963 615f 696e 5f73 7461  k_replica_in_sta
+00027f50: 7475 7328 0a20 2020 2020 2020 2020 2020  tus(.           
+00027f60: 2020 2020 206e 616d 652c 205b 2831 2c20       name, [(1, 
+00027f70: 4661 6c73 652c 2027 4641 494c 4544 5f50  False, 'FAILED_P
+00027f80: 524f 4249 4e47 2729 2c0a 2020 2020 2020  ROBING'),.      
+00027f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fa0: 2028 312c 2046 616c 7365 2c20 5f53 4552   (1, False, _SER
+00027fb0: 5649 4345 5f4c 4155 4e43 4849 4e47 5f53  VICE_LAUNCHING_S
+00027fc0: 5441 5455 535f 5245 4745 5829 5d29 2c0a  TATUS_REGEX)]),.
+00027fd0: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
+00027fe0: 444f 287a 6877 7529 3a20 6164 6420 7465  DO(zhwu): add te
+00027ff0: 7374 2066 6f72 2046 4149 4c45 445f 5052  st for FAILED_PR
+00028000: 4f56 4953 494f 4e0a 2020 2020 2020 2020  OVISION.        
+00028010: 5d2c 0a20 2020 2020 2020 205f 5445 4152  ],.        _TEAR
+00028020: 444f 574e 5f53 4552 5649 4345 2e66 6f72  DOWN_SERVICE.for
+00028030: 6d61 7428 6e61 6d65 3d6e 616d 6529 2c0a  mat(name=name),.
+00028040: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
+00028050: 3230 202a 2036 302c 0a20 2020 2029 0a20  20 * 60,.    ). 
+00028060: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00028070: 7465 7374 290a 0a0a 2320 544f 444f 285a  test)...# TODO(Z
+00028080: 696d 696e 672c 2054 6961 6e29 3a20 4164  iming, Tian): Ad
+00028090: 6420 7465 7374 7320 666f 7220 6175 746f  d tests for auto
+000280a0: 7363 616c 696e 672e 0a0a 0a23 202d 2d2d  scaling....# ---
+000280b0: 2d2d 2d2d 2054 6573 7469 6e67 2075 7365  ---- Testing use
+000280c0: 7220 7261 7920 636c 7573 7465 7220 2d2d  r ray cluster --
+000280d0: 2d2d 2d2d 2d2d 0a64 6566 2074 6573 745f  ------.def test_
+000280e0: 7573 6572 5f72 6179 5f63 6c75 7374 6572  user_ray_cluster
+000280f0: 2867 656e 6572 6963 5f63 6c6f 7564 3a20  (generic_cloud: 
+00028100: 7374 7229 3a0a 2020 2020 6e61 6d65 203d  str):.    name =
+00028110: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00028120: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+00028130: 5465 7374 280a 2020 2020 2020 2020 2775  Test(.        'u
+00028140: 7365 722d 7261 792d 636c 7573 7465 7227  ser-ray-cluster'
+00028150: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
+00028160: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
+00028170: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
+00028180: 7d20 2d2d 636c 6f75 6420 7b67 656e 6572  } --cloud {gener
+00028190: 6963 5f63 6c6f 7564 7d20 2272 6179 2073  ic_cloud} "ray s
+000281a0: 7461 7274 202d 2d68 6561 6422 272c 0a20  tart --head"',. 
+000281b0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+000281c0: 2065 7865 6320 7b6e 616d 657d 2022 6563   exec {name} "ec
+000281d0: 686f 2068 6922 272c 0a20 2020 2020 2020  ho hi"',.       
+000281e0: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
+000281f0: 7b6e 616d 657d 2031 202d 2d73 7461 7475  {name} 1 --statu
+00028200: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+00028210: 6627 736b 7920 7374 6174 7573 202d 7220  f'sky status -r 
+00028220: 7b6e 616d 657d 207c 2067 7265 7020 5550  {name} | grep UP
+00028230: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
+00028240: 2773 6b79 2065 7865 6320 7b6e 616d 657d  'sky exec {name}
+00028250: 2022 6563 686f 2062 7965 2227 2c0a 2020   "echo bye"',.  
+00028260: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00028270: 6c6f 6773 207b 6e61 6d65 7d20 3220 2d2d  logs {name} 2 --
+00028280: 7374 6174 7573 272c 0a20 2020 2020 2020  status',.       
+00028290: 205d 2c0a 2020 2020 2020 2020 6627 736b   ],.        f'sk
+000282a0: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
+000282b0: 272c 0a20 2020 2029 0a20 2020 2072 756e  ',.    ).    run
+000282c0: 5f6f 6e65 5f74 6573 7428 7465 7374 290a  _one_test(test).
+000282d0: 0a0a 2320 2d2d 2d2d 2d2d 2d20 5465 7374  ..# ------- Test
+000282e0: 696e 6720 7468 6520 636f 7265 2041 5049  ing the core API
+000282f0: 202d 2d2d 2d2d 2d2d 2d0a 2320 4d6f 7374   --------.# Most
+00028300: 206f 6620 7468 6520 636f 7265 2041 5049   of the core API
+00028310: 7320 6861 7665 2062 6565 6e20 7465 7374  s have been test
+00028320: 6564 2069 6e20 7468 6520 434c 4920 7465  ed in the CLI te
+00028330: 7374 732e 0a23 2054 6865 7365 2074 6573  sts..# These tes
+00028340: 7473 2061 7265 2066 6f72 2074 6573 7469  ts are for testi
+00028350: 6e67 2074 6865 2072 6574 7572 6e20 7661  ng the return va
+00028360: 6c75 6520 6f66 2074 6865 2041 5049 7320  lue of the APIs 
+00028370: 6e6f 7420 6675 6c6c 7920 7573 6564 2069  not fully used i
+00028380: 6e20 434c 492e 0a0a 0a40 7079 7465 7374  n CLI....@pytest
+00028390: 2e6d 6172 6b2e 6763 700a 6465 6620 7465  .mark.gcp.def te
+000283a0: 7374 5f63 6f72 655f 6170 695f 736b 795f  st_core_api_sky_
+000283b0: 6c61 756e 6368 5f65 7865 6328 293a 0a20  launch_exec():. 
+000283c0: 2020 206e 616d 6520 3d20 5f67 6574 5f63     name = _get_c
+000283d0: 6c75 7374 6572 5f6e 616d 6528 290a 2020  luster_name().  
+000283e0: 2020 7461 736b 203d 2073 6b79 2e54 6173    task = sky.Tas
+000283f0: 6b28 7275 6e3d 2277 686f 616d 6922 290a  k(run="whoami").
+00028400: 2020 2020 7461 736b 2e73 6574 5f72 6573      task.set_res
+00028410: 6f75 7263 6573 2873 6b79 2e52 6573 6f75  ources(sky.Resou
+00028420: 7263 6573 2863 6c6f 7564 3d73 6b79 2e47  rces(cloud=sky.G
+00028430: 4350 2829 2929 0a20 2020 206a 6f62 5f69  CP())).    job_i
+00028440: 642c 2068 616e 646c 6520 3d20 736b 792e  d, handle = sky.
+00028450: 6c61 756e 6368 2874 6173 6b2c 2063 6c75  launch(task, clu
+00028460: 7374 6572 5f6e 616d 653d 6e61 6d65 290a  ster_name=name).
+00028470: 2020 2020 6173 7365 7274 206a 6f62 5f69      assert job_i
+00028480: 6420 3d3d 2031 0a20 2020 2061 7373 6572  d == 1.    asser
+00028490: 7420 6861 6e64 6c65 2069 7320 6e6f 7420  t handle is not 
+000284a0: 4e6f 6e65 0a20 2020 2061 7373 6572 7420  None.    assert 
+000284b0: 6861 6e64 6c65 2e63 6c75 7374 6572 5f6e  handle.cluster_n
+000284c0: 616d 6520 3d3d 206e 616d 650a 2020 2020  ame == name.    
+000284d0: 6173 7365 7274 2068 616e 646c 652e 6c61  assert handle.la
+000284e0: 756e 6368 6564 5f72 6573 6f75 7263 6573  unched_resources
+000284f0: 2e63 6c6f 7564 2e69 735f 7361 6d65 5f63  .cloud.is_same_c
+00028500: 6c6f 7564 2873 6b79 2e47 4350 2829 290a  loud(sky.GCP()).
+00028510: 2020 2020 6a6f 625f 6964 5f65 7865 632c      job_id_exec,
+00028520: 2068 616e 646c 655f 6578 6563 203d 2073   handle_exec = s
+00028530: 6b79 2e65 7865 6328 7461 736b 2c20 636c  ky.exec(task, cl
+00028540: 7573 7465 725f 6e61 6d65 3d6e 616d 6529  uster_name=name)
+00028550: 0a20 2020 2061 7373 6572 7420 6a6f 625f  .    assert job_
+00028560: 6964 5f65 7865 6320 3d3d 2032 0a20 2020  id_exec == 2.   
+00028570: 2061 7373 6572 7420 6861 6e64 6c65 5f65   assert handle_e
+00028580: 7865 6320 6973 206e 6f74 204e 6f6e 650a  xec is not None.
+00028590: 2020 2020 6173 7365 7274 2068 616e 646c      assert handl
+000285a0: 655f 6578 6563 2e63 6c75 7374 6572 5f6e  e_exec.cluster_n
+000285b0: 616d 6520 3d3d 206e 616d 650a 2020 2020  ame == name.    
+000285c0: 6173 7365 7274 2068 616e 646c 655f 6578  assert handle_ex
+000285d0: 6563 2e6c 6175 6e63 6865 645f 7265 736f  ec.launched_reso
+000285e0: 7572 6365 732e 636c 6f75 642e 6973 5f73  urces.cloud.is_s
+000285f0: 616d 655f 636c 6f75 6428 736b 792e 4743  ame_cloud(sky.GC
+00028600: 5028 2929 0a20 2020 2023 2046 6f72 2064  P()).    # For d
+00028610: 756d 6d79 2074 6173 6b20 2869 2e65 2e20  ummy task (i.e. 
+00028620: 7461 736b 2e72 756e 2069 7320 4e6f 6e65  task.run is None
+00028630: 292c 2074 6865 206a 6f62 2077 6f6e 2774  ), the job won't
+00028640: 2062 6520 7375 626d 6974 7465 642e 0a20   be submitted.. 
+00028650: 2020 2064 756d 6d79 5f74 6173 6b20 3d20     dummy_task = 
+00028660: 736b 792e 5461 736b 2829 0a20 2020 206a  sky.Task().    j
+00028670: 6f62 5f69 645f 6475 6d6d 792c 205f 203d  ob_id_dummy, _ =
+00028680: 2073 6b79 2e65 7865 6328 6475 6d6d 795f   sky.exec(dummy_
+00028690: 7461 736b 2c20 636c 7573 7465 725f 6e61  task, cluster_na
+000286a0: 6d65 3d6e 616d 6529 0a20 2020 2061 7373  me=name).    ass
+000286b0: 6572 7420 6a6f 625f 6964 5f64 756d 6d79  ert job_id_dummy
+000286c0: 2069 7320 4e6f 6e65 0a20 2020 2073 6b79   is None.    sky
+000286d0: 2e64 6f77 6e28 6e61 6d65 290a 0a0a 2320  .down(name)...# 
+000286e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2054 6573 7469  ---------- Testi
+000286f0: 6e67 2053 746f 7261 6765 202d 2d2d 2d2d  ng Storage -----
+00028700: 2d2d 2d2d 2d0a 636c 6173 7320 5465 7374  -----.class Test
+00028710: 5374 6f72 6167 6557 6974 6843 7265 6465  StorageWithCrede
+00028720: 6e74 6961 6c73 3a0a 2020 2020 2222 2253  ntials:.    """S
+00028730: 746f 7261 6765 2074 6573 7473 2077 6869  torage tests whi
+00028740: 6368 2072 6571 7569 7265 2063 7265 6465  ch require crede
+00028750: 6e74 6961 6c73 2061 6e64 206e 6574 776f  ntials and netwo
+00028760: 726b 2063 6f6e 6e65 6374 696f 6e22 2222  rk connection"""
+00028770: 0a0a 2020 2020 4157 535f 494e 5641 4c49  ..    AWS_INVALI
+00028780: 445f 4e41 4d45 5320 3d20 5b0a 2020 2020  D_NAMES = [.    
+00028790: 2020 2020 2761 6227 2c20 2023 206c 6573      'ab',  # les
+000287a0: 7320 7468 616e 2033 2063 6861 7261 6374  s than 3 charact
+000287b0: 6572 730a 2020 2020 2020 2020 2761 6263  ers.        'abc
+000287c0: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
+000287d0: 7475 7677 7879 7a61 6263 6465 6667 6869  tuvwxyzabcdefghi
+000287e0: 6a6b 6c6d 6e6f 7071 7273 7475 7677 7879  jklmnopqrstuvwxy
+000287f0: 7a61 6263 6465 6667 6869 6a6b 6c6d 6e6f  zabcdefghijklmno
+00028800: 7071 7273 7475 7677 7879 7a31 272c 0a20  pqrstuvwxyz1',. 
+00028810: 2020 2020 2020 2023 206d 6f72 6520 7468         # more th
+00028820: 616e 2036 3320 6368 6172 6163 7465 7273  an 63 characters
+00028830: 0a20 2020 2020 2020 2027 4162 6364 6566  .        'Abcdef
+00028840: 272c 2020 2320 636f 6e74 6169 6e73 2061  ',  # contains a
+00028850: 6e20 7570 7065 7263 6173 6520 6c65 7474  n uppercase lett
+00028860: 6572 0a20 2020 2020 2020 2027 6162 6320  er.        'abc 
+00028870: 6465 6627 2c20 2023 2063 6f6e 7461 696e  def',  # contain
+00028880: 7320 6120 7370 6163 650a 2020 2020 2020  s a space.      
+00028890: 2020 2761 6263 2e2e 6465 6627 2c20 2023    'abc..def',  #
+000288a0: 2074 776f 2061 646a 6163 656e 7420 7065   two adjacent pe
+000288b0: 7269 6f64 730a 2020 2020 2020 2020 2731  riods.        '1
+000288c0: 3932 2e31 3638 2e35 2e34 272c 2020 2320  92.168.5.4',  # 
+000288d0: 666f 726d 6174 7465 6420 6173 2061 6e20  formatted as an 
+000288e0: 4950 2061 6464 7265 7373 0a20 2020 2020  IP address.     
+000288f0: 2020 2027 786e 2d2d 6275 636b 6574 272c     'xn--bucket',
+00028900: 2020 2320 7374 6172 7473 2077 6974 6820    # starts with 
+00028910: 2778 6e2d 2d27 2070 7265 6669 780a 2020  'xn--' prefix.  
+00028920: 2020 2020 2020 2762 7563 6b65 742d 7333        'bucket-s3
+00028930: 616c 6961 7327 2c20 2023 2065 6e64 7320  alias',  # ends 
+00028940: 7769 7468 2027 2d73 3361 6c69 6173 2720  with '-s3alias' 
+00028950: 7375 6666 6978 0a20 2020 2020 2020 2027  suffix.        '
+00028960: 6275 636b 6574 2d2d 6f6c 2d73 3327 2c20  bucket--ol-s3', 
+00028970: 2023 2065 6e64 7320 7769 7468 2027 2d2d   # ends with '--
+00028980: 6f6c 2d73 3327 2073 7566 6669 780a 2020  ol-s3' suffix.  
+00028990: 2020 2020 2020 272e 6162 6327 2c20 2023        '.abc',  #
+000289a0: 2073 7461 7274 7320 7769 7468 2061 2064   starts with a d
+000289b0: 6f74 0a20 2020 2020 2020 2027 6162 632e  ot.        'abc.
+000289c0: 272c 2020 2320 656e 6473 2077 6974 6820  ',  # ends with 
+000289d0: 6120 646f 740a 2020 2020 2020 2020 272d  a dot.        '-
+000289e0: 6162 6327 2c20 2023 2073 7461 7274 7320  abc',  # starts 
+000289f0: 7769 7468 2061 2068 7970 6865 6e0a 2020  with a hyphen.  
+00028a00: 2020 2020 2020 2761 6263 2d27 2c20 2023        'abc-',  #
+00028a10: 2065 6e64 7320 7769 7468 2061 2068 7970   ends with a hyp
+00028a20: 6865 6e0a 2020 2020 5d0a 0a20 2020 2047  hen.    ]..    G
+00028a30: 4353 5f49 4e56 414c 4944 5f4e 414d 4553  CS_INVALID_NAMES
+00028a40: 203d 205b 0a20 2020 2020 2020 2027 6162   = [.        'ab
+00028a50: 272c 2020 2320 6c65 7373 2074 6861 6e20  ',  # less than 
+00028a60: 3320 6368 6172 6163 7465 7273 0a20 2020  3 characters.   
+00028a70: 2020 2020 2027 6162 6364 6566 6768 696a       'abcdefghij
+00028a80: 6b6c 6d6e 6f70 7172 7374 7576 7778 797a  klmnopqrstuvwxyz
+00028a90: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
+00028aa0: 7172 7374 7576 7778 797a 6162 6364 6566  qrstuvwxyzabcdef
+00028ab0: 6768 696a 6b6c 6d6e 6f70 7172 7374 7576  ghijklmnopqrstuv
+00028ac0: 7778 797a 3127 2c0a 2020 2020 2020 2020  wxyz1',.        
+00028ad0: 2320 6d6f 7265 2074 6861 6e20 3633 2063  # more than 63 c
+00028ae0: 6861 7261 6374 6572 7320 2877 6974 686f  haracters (witho
+00028af0: 7574 2064 6f74 7329 0a20 2020 2020 2020  ut dots).       
+00028b00: 2027 4162 6364 6566 272c 2020 2320 636f   'Abcdef',  # co
+00028b10: 6e74 6169 6e73 2061 6e20 7570 7065 7263  ntains an upperc
+00028b20: 6173 6520 6c65 7474 6572 0a20 2020 2020  ase letter.     
+00028b30: 2020 2027 6162 6320 6465 6627 2c20 2023     'abc def',  #
+00028b40: 2063 6f6e 7461 696e 7320 6120 7370 6163   contains a spac
+00028b50: 650a 2020 2020 2020 2020 2761 6263 2e2e  e.        'abc..
+00028b60: 6465 6627 2c20 2023 2074 776f 2061 646a  def',  # two adj
+00028b70: 6163 656e 7420 7065 7269 6f64 730a 2020  acent periods.  
+00028b80: 2020 2020 2020 2761 6263 5f2e 6465 662e        'abc_.def.
+00028b90: 6768 692e 6a6b 6c6d 6e6f 7071 7273 7475  ghi.jklmnopqrstu
+00028ba0: 7677 7879 7a61 6263 6465 6667 6869 6a6b  vwxyzabcdefghijk
+00028bb0: 6c6d 6e6f 7071 7273 7475 7677 7879 7a61  lmnopqrstuvwxyza
+00028bc0: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+00028bd0: 7273 7475 7677 7879 7a31 270a 2020 2020  rstuvwxyz1'.    
+00028be0: 2020 2020 2320 4d6f 7265 2074 6861 6e20      # More than 
+00028bf0: 3633 2063 6861 7261 6374 6572 7320 6265  63 characters be
+00028c00: 7477 6565 6e20 646f 7473 0a20 2020 2020  tween dots.     
+00028c10: 2020 2027 6162 635f 2e64 6566 2e67 6869     'abc_.def.ghi
+00028c20: 2e6a 6b6c 6d6e 6f70 7172 7374 7576 7778  .jklmnopqrstuvwx
+00028c30: 797a 6162 6364 6566 6768 696a 6b6c 6d6e  yzabcdefghijklmn
+00028c40: 6f70 7166 6768 696a 6b6c 6d6e 6f70 7172  opqfghijklmnopqr
+00028c50: 7374 7576 7727 202a 2035 2c0a 2020 2020  stuvw' * 5,.    
+00028c60: 2020 2020 2320 6d6f 7265 2074 6861 6e20      # more than 
+00028c70: 3232 3220 6368 6172 6163 7465 7273 2028  222 characters (
+00028c80: 7769 7468 2064 6f74 7329 0a20 2020 2020  with dots).     
+00028c90: 2020 2027 3139 322e 3136 382e 352e 3427     '192.168.5.4'
+00028ca0: 2c20 2023 2066 6f72 6d61 7474 6564 2061  ,  # formatted a
+00028cb0: 7320 616e 2049 5020 6164 6472 6573 730a  s an IP address.
+00028cc0: 2020 2020 2020 2020 2767 6f6f 6762 7563          'googbuc
+00028cd0: 6b65 7427 2c20 2023 2073 7461 7274 7320  ket',  # starts 
+00028ce0: 7769 7468 2027 676f 6f67 2720 7072 6566  with 'goog' pref
+00028cf0: 6978 0a20 2020 2020 2020 2027 676f 6f67  ix.        'goog
+00028d00: 6c65 6275 636b 6574 272c 2020 2320 636f  lebucket',  # co
+00028d10: 6e74 6169 6e73 2027 676f 6f67 6c65 270a  ntains 'google'.
+00028d20: 2020 2020 2020 2020 2767 3030 676c 6562          'g00gleb
+00028d30: 7563 6b65 7427 2c20 2023 2076 6172 6961  ucket',  # varia
+00028d40: 6e74 206f 6620 2767 6f6f 676c 6527 0a20  nt of 'google'. 
+00028d50: 2020 2020 2020 2027 676f 3067 6c65 6275         'go0glebu
+00028d60: 636b 6574 272c 2020 2320 7661 7269 616e  cket',  # varian
+00028d70: 7420 6f66 2027 676f 6f67 6c65 270a 2020  t of 'google'.  
+00028d80: 2020 2020 2020 2767 306f 676c 6562 7563        'g0oglebuc
+00028d90: 6b65 7427 2c20 2023 2076 6172 6961 6e74  ket',  # variant
+00028da0: 206f 6620 2767 6f6f 676c 6527 0a20 2020   of 'google'.   
+00028db0: 2020 2020 2027 2e61 6263 272c 2020 2320       '.abc',  # 
+00028dc0: 7374 6172 7473 2077 6974 6820 6120 646f  starts with a do
+00028dd0: 740a 2020 2020 2020 2020 2761 6263 2e27  t.        'abc.'
+00028de0: 2c20 2023 2065 6e64 7320 7769 7468 2061  ,  # ends with a
+00028df0: 2064 6f74 0a20 2020 2020 2020 2027 5f61   dot.        '_a
+00028e00: 6263 272c 2020 2320 7374 6172 7473 2077  bc',  # starts w
+00028e10: 6974 6820 616e 2075 6e64 6572 7363 6f72  ith an underscor
+00028e20: 650a 2020 2020 2020 2020 2761 6263 5f27  e.        'abc_'
+00028e30: 2c20 2023 2065 6e64 7320 7769 7468 2061  ,  # ends with a
+00028e40: 6e20 756e 6465 7273 636f 7265 0a20 2020  n underscore.   
+00028e50: 205d 0a0a 2020 2020 4942 4d5f 494e 5641   ]..    IBM_INVA
+00028e60: 4c49 445f 4e41 4d45 5320 3d20 5b0a 2020  LID_NAMES = [.  
+00028e70: 2020 2020 2020 2761 6227 2c20 2023 206c        'ab',  # l
+00028e80: 6573 7320 7468 616e 2033 2063 6861 7261  ess than 3 chara
+00028e90: 6374 6572 730a 2020 2020 2020 2020 2761  cters.        'a
+00028ea0: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+00028eb0: 7273 7475 7677 7879 7a61 6263 6465 6667  rstuvwxyzabcdefg
+00028ec0: 6869 6a6b 6c6d 6e6f 7071 7273 7475 7677  hijklmnopqrstuvw
+00028ed0: 7879 7a61 6263 6465 6667 6869 6a6b 6c6d  xyzabcdefghijklm
+00028ee0: 6e6f 7071 7273 7475 7677 7879 7a31 272c  nopqrstuvwxyz1',
+00028ef0: 0a20 2020 2020 2020 2023 206d 6f72 6520  .        # more 
+00028f00: 7468 616e 2036 3320 6368 6172 6163 7465  than 63 characte
+00028f10: 7273 0a20 2020 2020 2020 2027 4162 6364  rs.        'Abcd
+00028f20: 6566 272c 2020 2320 636f 6e74 6169 6e73  ef',  # contains
+00028f30: 2061 6e20 7570 7065 7263 6173 6520 6c65   an uppercase le
+00028f40: 7474 6572 0a20 2020 2020 2020 2027 6162  tter.        'ab
+00028f50: 6320 6465 6627 2c20 2023 2063 6f6e 7461  c def',  # conta
+00028f60: 696e 7320 6120 7370 6163 650a 2020 2020  ins a space.    
+00028f70: 2020 2020 2761 6263 2e2e 6465 6627 2c20      'abc..def', 
+00028f80: 2023 2074 776f 2061 646a 6163 656e 7420   # two adjacent 
+00028f90: 7065 7269 6f64 730a 2020 2020 2020 2020  periods.        
+00028fa0: 2731 3932 2e31 3638 2e35 2e34 272c 2020  '192.168.5.4',  
+00028fb0: 2320 666f 726d 6174 7465 6420 6173 2061  # formatted as a
+00028fc0: 6e20 4950 2061 6464 7265 7373 0a20 2020  n IP address.   
+00028fd0: 2020 2020 2027 786e 2d2d 6275 636b 6574       'xn--bucket
+00028fe0: 272c 2020 2320 7374 6172 7473 2077 6974  ',  # starts wit
+00028ff0: 6820 2778 6e2d 2d27 2070 7265 6669 780a  h 'xn--' prefix.
+00029000: 2020 2020 2020 2020 272e 6162 6327 2c20          '.abc', 
+00029010: 2023 2073 7461 7274 7320 7769 7468 2061   # starts with a
+00029020: 2064 6f74 0a20 2020 2020 2020 2027 6162   dot.        'ab
+00029030: 632e 272c 2020 2320 656e 6473 2077 6974  c.',  # ends wit
+00029040: 6820 6120 646f 740a 2020 2020 2020 2020  h a dot.        
+00029050: 272d 6162 6327 2c20 2023 2073 7461 7274  '-abc',  # start
+00029060: 7320 7769 7468 2061 2068 7970 6865 6e0a  s with a hyphen.
+00029070: 2020 2020 2020 2020 2761 6263 2d27 2c20          'abc-', 
+00029080: 2023 2065 6e64 7320 7769 7468 2061 2068   # ends with a h
+00029090: 7970 6865 6e0a 2020 2020 2020 2020 2761  yphen.        'a
+000290a0: 2e2d 6263 272c 2020 2320 636f 6e74 6169  .-bc',  # contai
+000290b0: 6e73 2074 6865 2073 6571 7565 6e63 6520  ns the sequence 
+000290c0: 272e 2d27 0a20 2020 2020 2020 2027 612d  '.-'.        'a-
+000290d0: 2e62 6327 2c20 2023 2063 6f6e 7461 696e  .bc',  # contain
+000290e0: 7320 7468 6520 7365 7175 656e 6365 2027  s the sequence '
+000290f0: 2d2e 270a 2020 2020 2020 2020 2761 2662  -.'.        'a&b
+00029100: 6327 2020 2320 636f 6e74 6169 6e73 2073  c'  # contains s
+00029110: 7065 6369 616c 2063 6861 7261 6374 6572  pecial character
+00029120: 730a 2020 2020 2020 2020 2761 625e 6327  s.        'ab^c'
+00029130: 2020 2320 636f 6e74 6169 6e73 2073 7065    # contains spe
+00029140: 6369 616c 2063 6861 7261 6374 6572 730a  cial characters.
+00029150: 2020 2020 5d0a 2020 2020 4749 5449 474e      ].    GITIGN
+00029160: 4f52 455f 5359 4e43 5f54 4553 545f 4449  ORE_SYNC_TEST_DI
+00029170: 525f 5354 5255 4354 5552 4520 3d20 7b0a  R_STRUCTURE = {.
+00029180: 2020 2020 2020 2020 2764 6f75 626c 655f          'double_
+00029190: 6173 7465 7269 736b 273a 207b 0a20 2020  asterisk': {.   
+000291a0: 2020 2020 2020 2020 2027 646f 7562 6c65           'double
+000291b0: 5f61 7374 6572 6973 6b5f 6578 636c 7564  _asterisk_exclud
+000291c0: 6564 273a 204e 6f6e 652c 0a20 2020 2020  ed': None,.     
+000291d0: 2020 2020 2020 2027 646f 7562 6c65 5f61         'double_a
+000291e0: 7374 6572 6973 6b5f 6578 636c 7564 6564  sterisk_excluded
+000291f0: 5f64 6972 273a 207b 0a20 2020 2020 2020  _dir': {.       
+00029200: 2020 2020 2020 2020 2027 6469 725f 6578           'dir_ex
+00029210: 636c 7564 6564 273a 204e 6f6e 652c 0a20  cluded': None,. 
+00029220: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00029230: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00029240: 2027 646f 7562 6c65 5f61 7374 6572 6973   'double_asteris
+00029250: 6b5f 7061 7265 6e74 273a 207b 0a20 2020  k_parent': {.   
+00029260: 2020 2020 2020 2020 2027 7061 7265 6e74           'parent
+00029270: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
+00029280: 2020 2020 2027 616c 736f 5f65 7863 6c75       'also_exclu
+00029290: 6465 642e 7478 7427 3a20 4e6f 6e65 2c0a  ded.txt': None,.
+000292a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000292b0: 2763 6869 6c64 273a 207b 0a20 2020 2020  'child': {.     
+000292c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000292d0: 646f 7562 6c65 5f61 7374 6572 6973 6b5f  double_asterisk_
+000292e0: 7061 7265 6e74 5f63 6869 6c64 5f65 7863  parent_child_exc
+000292f0: 6c75 6465 642e 7478 7427 3a20 4e6f 6e65  luded.txt': None
+00029300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00029310: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00029320: 2020 2020 2027 646f 7562 6c65 5f61 7374       'double_ast
+00029330: 6572 6973 6b5f 7061 7265 6e74 5f65 7863  erisk_parent_exc
+00029340: 6c75 6465 642e 7478 7427 3a20 4e6f 6e65  luded.txt': None
+00029350: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
+00029360: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00029370: 2020 2020 2765 7863 6c75 6465 642e 6c6f      'excluded.lo
+00029380: 6727 3a20 4e6f 6e65 2c0a 2020 2020 2020  g': None,.      
+00029390: 2020 2765 7863 6c75 6465 645f 6469 7227    'excluded_dir'
+000293a0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000293b0: 2765 7863 6c75 6465 642e 7478 7427 3a20  'excluded.txt': 
+000293c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+000293d0: 2020 276e 6573 7465 645f 6578 636c 7564    'nested_exclud
+000293e0: 6564 273a 207b 0a20 2020 2020 2020 2020  ed': {.         
+000293f0: 2020 2020 2020 2027 6578 636c 7564 6564         'excluded
+00029400: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+00029410: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00029420: 7d2c 0a20 2020 2020 2020 2027 6578 702d  },.        'exp-
+00029430: 3127 3a20 7b0a 2020 2020 2020 2020 2020  1': {.          
+00029440: 2020 2762 655f 6578 636c 7564 6564 273a    'be_excluded':
+00029450: 204e 6f6e 652c 0a20 2020 2020 2020 207d   None,.        }
+00029460: 2c0a 2020 2020 2020 2020 2765 7870 2d32  ,.        'exp-2
+00029470: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
+00029480: 2027 6265 5f65 7863 6c75 6465 6427 3a20   'be_excluded': 
+00029490: 4e6f 6e65 2c0a 2020 2020 2020 2020 7d2c  None,.        },
+000294a0: 0a20 2020 2020 2020 2027 6672 6f6e 745f  .        'front_
+000294b0: 736c 6173 685f 6578 636c 7564 6564 273a  slash_excluded':
+000294c0: 204e 6f6e 652c 0a20 2020 2020 2020 2027   None,.        '
+000294d0: 696e 636c 7564 6564 2e6c 6f67 273a 204e  included.log': N
+000294e0: 6f6e 652c 0a20 2020 2020 2020 2027 696e  one,.        'in
+000294f0: 636c 7564 6564 2e74 7874 273a 204e 6f6e  cluded.txt': Non
+00029500: 652c 0a20 2020 2020 2020 2027 696e 636c  e,.        'incl
+00029510: 7564 655f 6469 7227 3a20 7b0a 2020 2020  ude_dir': {.    
+00029520: 2020 2020 2020 2020 2765 7863 6c75 6465          'exclude
+00029530: 642e 6c6f 6727 3a20 4e6f 6e65 2c0a 2020  d.log': None,.  
+00029540: 2020 2020 2020 2020 2020 2769 6e63 6c75            'inclu
+00029550: 6465 642e 6c6f 6727 3a20 4e6f 6e65 2c0a  ded.log': None,.
+00029560: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00029570: 2020 2027 6e65 7374 6564 5f64 6f75 626c     'nested_doubl
+00029580: 655f 6173 7465 7269 736b 273a 207b 0a20  e_asterisk': {. 
+00029590: 2020 2020 2020 2020 2020 2027 6f6e 6527             'one'
+000295a0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000295b0: 2020 2020 2761 6c73 6f5f 6578 636c 7564      'also_exclud
+000295c0: 652e 7478 7427 3a20 4e6f 6e65 2c0a 2020  e.txt': None,.  
+000295d0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000295e0: 2020 2020 2020 2020 2027 7477 6f27 3a20           'two': 
+000295f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00029600: 2020 2761 6c73 6f5f 6578 636c 7564 652e    'also_exclude.
+00029610: 7478 7427 3a20 4e6f 6e65 2c0a 2020 2020  txt': None,.    
+00029620: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00029630: 2020 207d 2c0a 2020 2020 2020 2020 276e     },.        'n
+00029640: 6573 7465 645f 7769 6c64 6361 7264 5f64  ested_wildcard_d
+00029650: 6972 273a 207b 0a20 2020 2020 2020 2020  ir': {.         
+00029660: 2020 2027 6d6f 6e64 6179 273a 207b 0a20     'monday': {. 
+00029670: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00029680: 616c 736f 5f65 7863 6c75 6465 2e74 7874  also_exclude.txt
+00029690: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+000296a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000296b0: 2020 2020 2774 7565 7364 6179 273a 207b      'tuesday': {
+000296c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000296d0: 2027 616c 736f 5f65 7863 6c75 6465 2e74   'also_exclude.t
+000296e0: 7874 273a 204e 6f6e 652c 0a20 2020 2020  xt': None,.     
+000296f0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00029700: 2020 7d2c 0a20 2020 2020 2020 2027 6e6f    },.        'no
+00029710: 5f73 6c61 7368 5f65 7863 6c75 6465 6427  _slash_excluded'
+00029720: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+00029730: 276e 6f5f 736c 6173 685f 7465 7374 7327  'no_slash_tests'
+00029740: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00029750: 276e 6f5f 736c 6173 685f 6578 636c 7564  'no_slash_exclud
+00029760: 6564 273a 207b 0a20 2020 2020 2020 2020  ed': {.         
+00029770: 2020 2020 2020 2027 616c 736f 5f65 7863         'also_exc
+00029780: 6c75 6465 642e 7478 7427 3a20 4e6f 6e65  luded.txt': None
+00029790: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
+000297a0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000297b0: 2020 2020 2771 7565 7374 696f 6e5f 6d61      'question_ma
+000297c0: 726b 273a 207b 0a20 2020 2020 2020 2020  rk': {.         
+000297d0: 2020 2027 6578 636c 7564 6564 312e 7478     'excluded1.tx
+000297e0: 7427 3a20 4e6f 6e65 2c0a 2020 2020 2020  t': None,.      
+000297f0: 2020 2020 2020 2765 7863 6c75 6465 6440        'excluded@
+00029800: 2e74 7874 273a 204e 6f6e 652c 0a20 2020  .txt': None,.   
+00029810: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00029820: 2773 7175 6172 655f 6272 6163 6b65 7427  'square_bracket'
+00029830: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00029840: 2765 7863 6c75 6465 6431 2e74 7874 273a  'excluded1.txt':
+00029850: 204e 6f6e 652c 0a20 2020 2020 2020 207d   None,.        }
+00029860: 2c0a 2020 2020 2020 2020 2773 7175 6172  ,.        'squar
+00029870: 655f 6272 6163 6b65 745f 616c 7068 6127  e_bracket_alpha'
+00029880: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00029890: 2765 7863 6c75 6465 647a 2e74 7874 273a  'excludedz.txt':
+000298a0: 204e 6f6e 652c 0a20 2020 2020 2020 207d   None,.        }
+000298b0: 2c0a 2020 2020 2020 2020 2773 7175 6172  ,.        'squar
+000298c0: 655f 6272 6163 6b65 745f 6578 636c 6127  e_bracket_excla'
+000298d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000298e0: 2765 7863 6c75 6465 6432 2e74 7874 273a  'excluded2.txt':
+000298f0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00029900: 2020 2027 6578 636c 7564 6564 402e 7478     'excluded@.tx
+00029910: 7427 3a20 4e6f 6e65 2c0a 2020 2020 2020  t': None,.      
+00029920: 2020 7d2c 0a20 2020 2020 2020 2027 7371    },.        'sq
+00029930: 7561 7265 5f62 7261 636b 6574 5f73 696e  uare_bracket_sin
+00029940: 676c 6527 3a20 7b0a 2020 2020 2020 2020  gle': {.        
+00029950: 2020 2020 2765 7863 6c75 6465 6430 2e74      'excluded0.t
+00029960: 7874 273a 204e 6f6e 652c 0a20 2020 2020  xt': None,.     
+00029970: 2020 207d 2c0a 2020 2020 7d0a 0a20 2020     },.    }..   
+00029980: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00029990: 2020 2064 6566 2063 7265 6174 655f 6469     def create_di
+000299a0: 725f 7374 7275 6374 7572 6528 6261 7365  r_structure(base
+000299b0: 5f70 6174 682c 2073 7472 7563 7475 7265  _path, structure
+000299c0: 293a 0a20 2020 2020 2020 2023 2063 7265  ):.        # cre
+000299d0: 6174 6573 2061 2067 6976 656e 2066 696c  ates a given fil
+000299e0: 6520 5354 5255 4354 5552 4520 696e 2042  e STRUCTURE in B
+000299f0: 4153 455f 5041 5448 0a20 2020 2020 2020  ASE_PATH.       
+00029a00: 2066 6f72 206e 616d 652c 2073 7562 7374   for name, subst
+00029a10: 7275 6374 7572 6520 696e 2073 7472 7563  ructure in struc
+00029a20: 7475 7265 2e69 7465 6d73 2829 3a0a 2020  ture.items():.  
+00029a30: 2020 2020 2020 2020 2020 7061 7468 203d            path =
+00029a40: 206f 732e 7061 7468 2e6a 6f69 6e28 6261   os.path.join(ba
+00029a50: 7365 5f70 6174 682c 206e 616d 6529 0a20  se_path, name). 
+00029a60: 2020 2020 2020 2020 2020 2069 6620 7375             if su
+00029a70: 6273 7472 7563 7475 7265 2069 7320 4e6f  bstructure is No
+00029a80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00029a90: 2020 2020 2320 4372 6561 7465 2061 2066      # Create a f
+00029aa0: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+00029ab0: 2020 2020 6f70 656e 2870 6174 682c 2027      open(path, '
+00029ac0: 6127 2c20 656e 636f 6469 6e67 3d27 7574  a', encoding='ut
+00029ad0: 662d 3827 292e 636c 6f73 6528 290a 2020  f-8').close().  
+00029ae0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00029af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029b00: 2320 4372 6561 7465 2061 2073 7562 6469  # Create a subdi
+00029b10: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+00029b20: 2020 2020 2020 2020 6f73 2e6d 6b64 6972          os.mkdir
+00029b30: 2870 6174 6829 0a20 2020 2020 2020 2020  (path).         
+00029b40: 2020 2020 2020 2054 6573 7453 746f 7261         TestStora
+00029b50: 6765 5769 7468 4372 6564 656e 7469 616c  geWithCredential
+00029b60: 732e 6372 6561 7465 5f64 6972 5f73 7472  s.create_dir_str
+00029b70: 7563 7475 7265 280a 2020 2020 2020 2020  ucture(.        
+00029b80: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00029b90: 2c20 7375 6273 7472 7563 7475 7265 290a  , substructure).
+00029ba0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00029bb0: 6f64 0a20 2020 2064 6566 2063 6c69 5f64  od.    def cli_d
+00029bc0: 656c 6574 655f 636d 6428 7374 6f72 655f  elete_cmd(store_
+00029bd0: 7479 7065 2c20 6275 636b 6574 5f6e 616d  type, bucket_nam
+00029be0: 6529 3a0a 2020 2020 2020 2020 6966 2073  e):.        if s
+00029bf0: 746f 7265 5f74 7970 6520 3d3d 2073 746f  tore_type == sto
+00029c00: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+00029c10: 7065 2e53 333a 0a20 2020 2020 2020 2020  pe.S3:.         
+00029c20: 2020 2075 726c 203d 2066 2773 333a 2f2f     url = f's3://
+00029c30: 7b62 7563 6b65 745f 6e61 6d65 7d27 0a20  {bucket_name}'. 
+00029c40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00029c50: 6e20 6627 6177 7320 7333 2072 6220 7b75  n f'aws s3 rb {u
+00029c60: 726c 7d20 2d2d 666f 7263 6527 0a20 2020  rl} --force'.   
+00029c70: 2020 2020 2069 6620 7374 6f72 655f 7479       if store_ty
+00029c80: 7065 203d 3d20 7374 6f72 6167 655f 6c69  pe == storage_li
+00029c90: 622e 5374 6f72 6554 7970 652e 4743 533a  b.StoreType.GCS:
+00029ca0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+00029cb0: 203d 2066 2767 733a 2f2f 7b62 7563 6b65   = f'gs://{bucke
+00029cc0: 745f 6e61 6d65 7d27 0a20 2020 2020 2020  t_name}'.       
+00029cd0: 2020 2020 2067 7375 7469 6c5f 616c 6961       gsutil_alia
+00029ce0: 732c 2061 6c69 6173 5f67 656e 203d 2064  s, alias_gen = d
+00029cf0: 6174 615f 7574 696c 732e 6765 745f 6773  ata_utils.get_gs
+00029d00: 7574 696c 5f63 6f6d 6d61 6e64 2829 0a20  util_command(). 
+00029d10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00029d20: 6e20 6627 7b61 6c69 6173 5f67 656e 7d3b  n f'{alias_gen};
+00029d30: 207b 6773 7574 696c 5f61 6c69 6173 7d20   {gsutil_alias} 
+00029d40: 726d 202d 7220 7b75 726c 7d27 0a20 2020  rm -r {url}'.   
+00029d50: 2020 2020 2069 6620 7374 6f72 655f 7479       if store_ty
+00029d60: 7065 203d 3d20 7374 6f72 6167 655f 6c69  pe == storage_li
+00029d70: 622e 5374 6f72 6554 7970 652e 5232 3a0a  b.StoreType.R2:.
+00029d80: 2020 2020 2020 2020 2020 2020 656e 6470              endp
+00029d90: 6f69 6e74 5f75 726c 203d 2063 6c6f 7564  oint_url = cloud
+00029da0: 666c 6172 652e 6372 6561 7465 5f65 6e64  flare.create_end
+00029db0: 706f 696e 7428 290a 2020 2020 2020 2020  point().        
+00029dc0: 2020 2020 7572 6c20 3d20 6627 7333 3a2f      url = f's3:/
+00029dd0: 2f7b 6275 636b 6574 5f6e 616d 657d 270a  /{bucket_name}'.
+00029de0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00029df0: 726e 2066 2741 5753 5f53 4841 5245 445f  rn f'AWS_SHARED_
+00029e00: 4352 4544 454e 5449 414c 535f 4649 4c45  CREDENTIALS_FILE
+00029e10: 3d7b 636c 6f75 6466 6c61 7265 2e52 325f  ={cloudflare.R2_
+00029e20: 4352 4544 454e 5449 414c 535f 5041 5448  CREDENTIALS_PATH
+00029e30: 7d20 6177 7320 7333 2072 6220 7b75 726c  } aws s3 rb {url
+00029e40: 7d20 2d2d 666f 7263 6520 2d2d 656e 6470  } --force --endp
+00029e50: 6f69 6e74 207b 656e 6470 6f69 6e74 5f75  oint {endpoint_u
+00029e60: 726c 7d20 2d2d 7072 6f66 696c 653d 7232  rl} --profile=r2
+00029e70: 270a 2020 2020 2020 2020 6966 2073 746f  '.        if sto
+00029e80: 7265 5f74 7970 6520 3d3d 2073 746f 7261  re_type == stora
+00029e90: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+00029ea0: 2e49 424d 3a0a 2020 2020 2020 2020 2020  .IBM:.          
+00029eb0: 2020 6275 636b 6574 5f72 636c 6f6e 655f    bucket_rclone_
+00029ec0: 7072 6f66 696c 6520 3d20 5263 6c6f 6e65  profile = Rclone
+00029ed0: 2e67 656e 6572 6174 655f 7263 6c6f 6e65  .generate_rclone
+00029ee0: 5f62 7563 6b65 745f 7072 6f66 696c 655f  _bucket_profile_
+00029ef0: 6e61 6d65 280a 2020 2020 2020 2020 2020  name(.          
+00029f00: 2020 2020 2020 6275 636b 6574 5f6e 616d        bucket_nam
+00029f10: 652c 2052 636c 6f6e 652e 5263 6c6f 6e65  e, Rclone.Rclone
+00029f20: 436c 6f75 6473 2e49 424d 290a 2020 2020  Clouds.IBM).    
+00029f30: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00029f40: 2772 636c 6f6e 6520 7075 7267 6520 7b62  'rclone purge {b
+00029f50: 7563 6b65 745f 7263 6c6f 6e65 5f70 726f  ucket_rclone_pro
+00029f60: 6669 6c65 7d3a 7b62 7563 6b65 745f 6e61  file}:{bucket_na
+00029f70: 6d65 7d20 2626 2072 636c 6f6e 6520 636f  me} && rclone co
+00029f80: 6e66 6967 2064 656c 6574 6520 7b62 7563  nfig delete {buc
+00029f90: 6b65 745f 7263 6c6f 6e65 5f70 726f 6669  ket_rclone_profi
+00029fa0: 6c65 7d27 0a0a 2020 2020 4073 7461 7469  le}'..    @stati
+00029fb0: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00029fc0: 636c 695f 6c73 5f63 6d64 2873 746f 7265  cli_ls_cmd(store
+00029fd0: 5f74 7970 652c 2062 7563 6b65 745f 6e61  _type, bucket_na
+00029fe0: 6d65 2c20 7375 6666 6978 3d27 2729 3a0a  me, suffix=''):.
+00029ff0: 2020 2020 2020 2020 6966 2073 746f 7265          if store
+0002a000: 5f74 7970 6520 3d3d 2073 746f 7261 6765  _type == storage
+0002a010: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
+0002a020: 333a 0a20 2020 2020 2020 2020 2020 2069  3:.            i
+0002a030: 6620 7375 6666 6978 3a0a 2020 2020 2020  f suffix:.      
+0002a040: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
+0002a050: 6627 7333 3a2f 2f7b 6275 636b 6574 5f6e  f's3://{bucket_n
+0002a060: 616d 657d 2f7b 7375 6666 6978 7d27 0a20  ame}/{suffix}'. 
+0002a070: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0002a080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a090: 2075 726c 203d 2066 2773 333a 2f2f 7b62   url = f's3://{b
+0002a0a0: 7563 6b65 745f 6e61 6d65 7d27 0a20 2020  ucket_name}'.   
+0002a0b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002a0c0: 6627 6177 7320 7333 206c 7320 7b75 726c  f'aws s3 ls {url
+0002a0d0: 7d27 0a20 2020 2020 2020 2069 6620 7374  }'.        if st
+0002a0e0: 6f72 655f 7479 7065 203d 3d20 7374 6f72  ore_type == stor
+0002a0f0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002a100: 652e 4743 533a 0a20 2020 2020 2020 2020  e.GCS:.         
+0002a110: 2020 2069 6620 7375 6666 6978 3a0a 2020     if suffix:.  
+0002a120: 2020 2020 2020 2020 2020 2020 2020 7572                ur
+0002a130: 6c20 3d20 6627 6773 3a2f 2f7b 6275 636b  l = f'gs://{buck
+0002a140: 6574 5f6e 616d 657d 2f7b 7375 6666 6978  et_name}/{suffix
+0002a150: 7d27 0a20 2020 2020 2020 2020 2020 2065  }'.            e
+0002a160: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002a170: 2020 2020 2075 726c 203d 2066 2767 733a       url = f'gs:
+0002a180: 2f2f 7b62 7563 6b65 745f 6e61 6d65 7d27  //{bucket_name}'
+0002a190: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0002a1a0: 7572 6e20 6627 6773 7574 696c 206c 7320  urn f'gsutil ls 
+0002a1b0: 7b75 726c 7d27 0a20 2020 2020 2020 2069  {url}'.        i
+0002a1c0: 6620 7374 6f72 655f 7479 7065 203d 3d20  f store_type == 
+0002a1d0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002a1e0: 6554 7970 652e 5232 3a0a 2020 2020 2020  eType.R2:.      
+0002a1f0: 2020 2020 2020 656e 6470 6f69 6e74 5f75        endpoint_u
+0002a200: 726c 203d 2063 6c6f 7564 666c 6172 652e  rl = cloudflare.
+0002a210: 6372 6561 7465 5f65 6e64 706f 696e 7428  create_endpoint(
+0002a220: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0002a230: 2073 7566 6669 783a 0a20 2020 2020 2020   suffix:.       
+0002a240: 2020 2020 2020 2020 2075 726c 203d 2066           url = f
+0002a250: 2773 333a 2f2f 7b62 7563 6b65 745f 6e61  's3://{bucket_na
+0002a260: 6d65 7d2f 7b73 7566 6669 787d 270a 2020  me}/{suffix}'.  
+0002a270: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0002a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a290: 7572 6c20 3d20 6627 7333 3a2f 2f7b 6275  url = f's3://{bu
+0002a2a0: 636b 6574 5f6e 616d 657d 270a 2020 2020  cket_name}'.    
+0002a2b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0002a2c0: 2741 5753 5f53 4841 5245 445f 4352 4544  'AWS_SHARED_CRED
+0002a2d0: 454e 5449 414c 535f 4649 4c45 3d7b 636c  ENTIALS_FILE={cl
+0002a2e0: 6f75 6466 6c61 7265 2e52 325f 4352 4544  oudflare.R2_CRED
+0002a2f0: 454e 5449 414c 535f 5041 5448 7d20 6177  ENTIALS_PATH} aw
+0002a300: 7320 7333 206c 7320 7b75 726c 7d20 2d2d  s s3 ls {url} --
+0002a310: 656e 6470 6f69 6e74 207b 656e 6470 6f69  endpoint {endpoi
+0002a320: 6e74 5f75 726c 7d20 2d2d 7072 6f66 696c  nt_url} --profil
+0002a330: 653d 7232 270a 2020 2020 2020 2020 6966  e=r2'.        if
+0002a340: 2073 746f 7265 5f74 7970 6520 3d3d 2073   store_type == s
+0002a350: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
+0002a360: 5479 7065 2e49 424d 3a0a 2020 2020 2020  Type.IBM:.      
+0002a370: 2020 2020 2020 6275 636b 6574 5f72 636c        bucket_rcl
+0002a380: 6f6e 655f 7072 6f66 696c 6520 3d20 5263  one_profile = Rc
+0002a390: 6c6f 6e65 2e67 656e 6572 6174 655f 7263  lone.generate_rc
+0002a3a0: 6c6f 6e65 5f62 7563 6b65 745f 7072 6f66  lone_bucket_prof
+0002a3b0: 696c 655f 6e61 6d65 280a 2020 2020 2020  ile_name(.      
+0002a3c0: 2020 2020 2020 2020 2020 6275 636b 6574            bucket
+0002a3d0: 5f6e 616d 652c 2052 636c 6f6e 652e 5263  _name, Rclone.Rc
+0002a3e0: 6c6f 6e65 436c 6f75 6473 2e49 424d 290a  loneClouds.IBM).
+0002a3f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002a400: 726e 2066 2772 636c 6f6e 6520 6c73 207b  rn f'rclone ls {
+0002a410: 6275 636b 6574 5f72 636c 6f6e 655f 7072  bucket_rclone_pr
+0002a420: 6f66 696c 657d 3a7b 6275 636b 6574 5f6e  ofile}:{bucket_n
+0002a430: 616d 657d 2f7b 7375 6666 6978 7d27 0a0a  ame}/{suffix}'..
+0002a440: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+0002a450: 640a 2020 2020 6465 6620 636c 695f 7265  d.    def cli_re
+0002a460: 6769 6f6e 5f63 6d64 2873 746f 7265 5f74  gion_cmd(store_t
+0002a470: 7970 652c 2062 7563 6b65 745f 6e61 6d65  ype, bucket_name
+0002a480: 293a 0a20 2020 2020 2020 2069 6620 7374  ):.        if st
+0002a490: 6f72 655f 7479 7065 203d 3d20 7374 6f72  ore_type == stor
+0002a4a0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002a4b0: 652e 5333 3a0a 2020 2020 2020 2020 2020  e.S3:.          
+0002a4c0: 2020 7265 7475 726e 2028 2761 7773 2073    return ('aws s
+0002a4d0: 3361 7069 2067 6574 2d62 7563 6b65 742d  3api get-bucket-
+0002a4e0: 6c6f 6361 7469 6f6e 2027 0a20 2020 2020  location '.     
+0002a4f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0002a500: 272d 2d62 7563 6b65 7420 7b62 7563 6b65  '--bucket {bucke
+0002a510: 745f 6e61 6d65 7d20 2d2d 6f75 7470 7574  t_name} --output
+0002a520: 2074 6578 7427 290a 2020 2020 2020 2020   text').        
+0002a530: 656c 6966 2073 746f 7265 5f74 7970 6520  elif store_type 
+0002a540: 3d3d 2073 746f 7261 6765 5f6c 6962 2e53  == storage_lib.S
+0002a550: 746f 7265 5479 7065 2e47 4353 3a0a 2020  toreType.GCS:.  
+0002a560: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002a570: 2028 6627 6773 7574 696c 206c 7320 2d4c   (f'gsutil ls -L
+0002a580: 202d 6220 6773 3a2f 2f7b 6275 636b 6574   -b gs://{bucket
+0002a590: 5f6e 616d 657d 2f20 7c20 270a 2020 2020  _name}/ | '.    
+0002a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a5b0: 2767 7265 7020 224c 6f63 6174 696f 6e20  'grep "Location 
+0002a5c0: 636f 6e73 7472 6169 6e74 2220 7c20 270a  constraint" | '.
+0002a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a5e0: 2020 2020 2761 776b 205c 277b 7072 696e      'awk \'{prin
+0002a5f0: 7420 746f 6c6f 7765 7228 244e 4629 7d5c  t tolower($NF)}\
+0002a600: 2727 290a 2020 2020 2020 2020 656c 7365  '').        else
+0002a610: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0002a620: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+0002a630: 6564 4572 726f 7228 6627 5265 6769 6f6e  edError(f'Region
+0002a640: 2063 6f6d 6d61 6e64 206e 6f74 2069 6d70   command not imp
+0002a650: 6c65 6d65 6e74 6564 2066 6f72 2027 0a20  lemented for '. 
+0002a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a680: 2020 2020 2066 277b 7374 6f72 655f 7479       f'{store_ty
+0002a690: 7065 7d27 290a 0a20 2020 2040 7374 6174  pe}')..    @stat
+0002a6a0: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+0002a6b0: 2063 6c69 5f63 6f75 6e74 5f6e 616d 655f   cli_count_name_
+0002a6c0: 696e 5f62 7563 6b65 7428 7374 6f72 655f  in_bucket(store_
+0002a6d0: 7479 7065 2c20 6275 636b 6574 5f6e 616d  type, bucket_nam
+0002a6e0: 652c 2066 696c 655f 6e61 6d65 2c20 7375  e, file_name, su
+0002a6f0: 6666 6978 3d27 2729 3a0a 2020 2020 2020  ffix=''):.      
+0002a700: 2020 6966 2073 746f 7265 5f74 7970 6520    if store_type 
+0002a710: 3d3d 2073 746f 7261 6765 5f6c 6962 2e53  == storage_lib.S
+0002a720: 746f 7265 5479 7065 2e53 333a 0a20 2020  toreType.S3:.   
+0002a730: 2020 2020 2020 2020 2069 6620 7375 6666           if suff
+0002a740: 6978 3a0a 2020 2020 2020 2020 2020 2020  ix:.            
+0002a750: 2020 2020 7265 7475 726e 2066 2761 7773      return f'aws
+0002a760: 2073 3361 7069 206c 6973 742d 6f62 6a65   s3api list-obje
+0002a770: 6374 7320 2d2d 6275 636b 6574 2022 7b62  cts --bucket "{b
+0002a780: 7563 6b65 745f 6e61 6d65 7d22 202d 2d70  ucket_name}" --p
+0002a790: 7265 6669 7820 7b73 7566 6669 787d 202d  refix {suffix} -
+0002a7a0: 2d71 7565 7279 2022 6c65 6e67 7468 2843  -query "length(C
+0002a7b0: 6f6e 7465 6e74 735b 3f63 6f6e 7461 696e  ontents[?contain
+0002a7c0: 7328 4b65 792c 5c27 7b66 696c 655f 6e61  s(Key,\'{file_na
+0002a7d0: 6d65 7d5c 2729 5d2e 4b65 7929 2227 0a20  me}\')].Key)"'. 
+0002a7e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0002a7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002a800: 2072 6574 7572 6e20 6627 6177 7320 7333   return f'aws s3
+0002a810: 6170 6920 6c69 7374 2d6f 626a 6563 7473  api list-objects
+0002a820: 202d 2d62 7563 6b65 7420 227b 6275 636b   --bucket "{buck
+0002a830: 6574 5f6e 616d 657d 2220 2d2d 7175 6572  et_name}" --quer
+0002a840: 7920 226c 656e 6774 6828 436f 6e74 656e  y "length(Conten
+0002a850: 7473 5b3f 636f 6e74 6169 6e73 284b 6579  ts[?contains(Key
+0002a860: 2c5c 277b 6669 6c65 5f6e 616d 657d 5c27  ,\'{file_name}\'
+0002a870: 295d 2e4b 6579 2922 270a 2020 2020 2020  )].Key)"'.      
+0002a880: 2020 656c 6966 2073 746f 7265 5f74 7970    elif store_typ
+0002a890: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
+0002a8a0: 2e53 746f 7265 5479 7065 2e47 4353 3a0a  .StoreType.GCS:.
+0002a8b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0002a8c0: 7566 6669 783a 0a20 2020 2020 2020 2020  uffix:.         
+0002a8d0: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
+0002a8e0: 6773 7574 696c 206c 7320 2d72 2067 733a  gsutil ls -r gs:
+0002a8f0: 2f2f 7b62 7563 6b65 745f 6e61 6d65 7d2f  //{bucket_name}/
+0002a900: 7b73 7566 6669 787d 207c 2067 7265 7020  {suffix} | grep 
+0002a910: 227b 6669 6c65 5f6e 616d 657d 2220 7c20  "{file_name}" | 
+0002a920: 7763 202d 6c27 0a20 2020 2020 2020 2020  wc -l'.         
+0002a930: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0002a940: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002a950: 6627 6773 7574 696c 206c 7320 2d72 2067  f'gsutil ls -r g
+0002a960: 733a 2f2f 7b62 7563 6b65 745f 6e61 6d65  s://{bucket_name
+0002a970: 7d20 7c20 6772 6570 2022 7b66 696c 655f  } | grep "{file_
+0002a980: 6e61 6d65 7d22 207c 2077 6320 2d6c 270a  name}" | wc -l'.
+0002a990: 2020 2020 2020 2020 656c 6966 2073 746f          elif sto
+0002a9a0: 7265 5f74 7970 6520 3d3d 2073 746f 7261  re_type == stora
+0002a9b0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+0002a9c0: 2e52 323a 0a20 2020 2020 2020 2020 2020  .R2:.           
+0002a9d0: 2065 6e64 706f 696e 745f 7572 6c20 3d20   endpoint_url = 
+0002a9e0: 636c 6f75 6466 6c61 7265 2e63 7265 6174  cloudflare.creat
+0002a9f0: 655f 656e 6470 6f69 6e74 2829 0a20 2020  e_endpoint().   
+0002aa00: 2020 2020 2020 2020 2069 6620 7375 6666           if suff
+0002aa10: 6978 3a0a 2020 2020 2020 2020 2020 2020  ix:.            
+0002aa20: 2020 2020 7265 7475 726e 2066 2741 5753      return f'AWS
+0002aa30: 5f53 4841 5245 445f 4352 4544 454e 5449  _SHARED_CREDENTI
+0002aa40: 414c 535f 4649 4c45 3d7b 636c 6f75 6466  ALS_FILE={cloudf
+0002aa50: 6c61 7265 2e52 325f 4352 4544 454e 5449  lare.R2_CREDENTI
+0002aa60: 414c 535f 5041 5448 7d20 6177 7320 7333  ALS_PATH} aws s3
+0002aa70: 6170 6920 6c69 7374 2d6f 626a 6563 7473  api list-objects
+0002aa80: 202d 2d62 7563 6b65 7420 227b 6275 636b   --bucket "{buck
+0002aa90: 6574 5f6e 616d 657d 2220 2d2d 7072 6566  et_name}" --pref
+0002aaa0: 6978 207b 7375 6666 6978 7d20 2d2d 7175  ix {suffix} --qu
+0002aab0: 6572 7920 226c 656e 6774 6828 436f 6e74  ery "length(Cont
+0002aac0: 656e 7473 5b3f 636f 6e74 6169 6e73 284b  ents[?contains(K
+0002aad0: 6579 2c5c 277b 6669 6c65 5f6e 616d 657d  ey,\'{file_name}
+0002aae0: 5c27 295d 2e4b 6579 2922 202d 2d65 6e64  \')].Key)" --end
+0002aaf0: 706f 696e 7420 7b65 6e64 706f 696e 745f  point {endpoint_
+0002ab00: 7572 6c7d 202d 2d70 726f 6669 6c65 3d72  url} --profile=r
+0002ab10: 3227 0a20 2020 2020 2020 2020 2020 2065  2'.            e
+0002ab20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0002ab30: 2020 2020 2072 6574 7572 6e20 6627 4157       return f'AW
+0002ab40: 535f 5348 4152 4544 5f43 5245 4445 4e54  S_SHARED_CREDENT
+0002ab50: 4941 4c53 5f46 494c 453d 7b63 6c6f 7564  IALS_FILE={cloud
+0002ab60: 666c 6172 652e 5232 5f43 5245 4445 4e54  flare.R2_CREDENT
+0002ab70: 4941 4c53 5f50 4154 487d 2061 7773 2073  IALS_PATH} aws s
+0002ab80: 3361 7069 206c 6973 742d 6f62 6a65 6374  3api list-object
+0002ab90: 7320 2d2d 6275 636b 6574 2022 7b62 7563  s --bucket "{buc
+0002aba0: 6b65 745f 6e61 6d65 7d22 202d 2d71 7565  ket_name}" --que
+0002abb0: 7279 2022 6c65 6e67 7468 2843 6f6e 7465  ry "length(Conte
+0002abc0: 6e74 735b 3f63 6f6e 7461 696e 7328 4b65  nts[?contains(Ke
+0002abd0: 792c 5c27 7b66 696c 655f 6e61 6d65 7d5c  y,\'{file_name}\
+0002abe0: 2729 5d2e 4b65 7929 2220 2d2d 656e 6470  ')].Key)" --endp
+0002abf0: 6f69 6e74 207b 656e 6470 6f69 6e74 5f75  oint {endpoint_u
+0002ac00: 726c 7d20 2d2d 7072 6f66 696c 653d 7232  rl} --profile=r2
+0002ac10: 270a 0a20 2020 2040 7374 6174 6963 6d65  '..    @staticme
+0002ac20: 7468 6f64 0a20 2020 2064 6566 2063 6c69  thod.    def cli
+0002ac30: 5f63 6f75 6e74 5f66 696c 655f 696e 5f62  _count_file_in_b
+0002ac40: 7563 6b65 7428 7374 6f72 655f 7479 7065  ucket(store_type
+0002ac50: 2c20 6275 636b 6574 5f6e 616d 6529 3a0a  , bucket_name):.
+0002ac60: 2020 2020 2020 2020 6966 2073 746f 7265          if store
+0002ac70: 5f74 7970 6520 3d3d 2073 746f 7261 6765  _type == storage
+0002ac80: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
+0002ac90: 333a 0a20 2020 2020 2020 2020 2020 2072  3:.            r
+0002aca0: 6574 7572 6e20 6627 6177 7320 7333 206c  eturn f'aws s3 l
+0002acb0: 7320 7333 3a2f 2f7b 6275 636b 6574 5f6e  s s3://{bucket_n
+0002acc0: 616d 657d 202d 2d72 6563 7572 7369 7665  ame} --recursive
+0002acd0: 207c 2077 6320 2d6c 270a 2020 2020 2020   | wc -l'.      
+0002ace0: 2020 656c 6966 2073 746f 7265 5f74 7970    elif store_typ
+0002acf0: 6520 3d3d 2073 746f 7261 6765 5f6c 6962  e == storage_lib
+0002ad00: 2e53 746f 7265 5479 7065 2e47 4353 3a0a  .StoreType.GCS:.
+0002ad10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002ad20: 726e 2066 2767 7375 7469 6c20 6c73 202d  rn f'gsutil ls -
+0002ad30: 7220 6773 3a2f 2f7b 6275 636b 6574 5f6e  r gs://{bucket_n
+0002ad40: 616d 657d 2f2a 2a20 7c20 7763 202d 6c27  ame}/** | wc -l'
+0002ad50: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
+0002ad60: 6f72 655f 7479 7065 203d 3d20 7374 6f72  ore_type == stor
+0002ad70: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002ad80: 652e 5232 3a0a 2020 2020 2020 2020 2020  e.R2:.          
+0002ad90: 2020 656e 6470 6f69 6e74 5f75 726c 203d    endpoint_url =
+0002ada0: 2063 6c6f 7564 666c 6172 652e 6372 6561   cloudflare.crea
+0002adb0: 7465 5f65 6e64 706f 696e 7428 290a 2020  te_endpoint().  
+0002adc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002add0: 2066 2741 5753 5f53 4841 5245 445f 4352   f'AWS_SHARED_CR
+0002ade0: 4544 454e 5449 414c 535f 4649 4c45 3d7b  EDENTIALS_FILE={
+0002adf0: 636c 6f75 6466 6c61 7265 2e52 325f 4352  cloudflare.R2_CR
+0002ae00: 4544 454e 5449 414c 535f 5041 5448 7d20  EDENTIALS_PATH} 
+0002ae10: 6177 7320 7333 206c 7320 7333 3a2f 2f7b  aws s3 ls s3://{
+0002ae20: 6275 636b 6574 5f6e 616d 657d 202d 2d72  bucket_name} --r
+0002ae30: 6563 7572 7369 7665 202d 2d65 6e64 706f  ecursive --endpo
+0002ae40: 696e 7420 7b65 6e64 706f 696e 745f 7572  int {endpoint_ur
+0002ae50: 6c7d 202d 2d70 726f 6669 6c65 3d72 3220  l} --profile=r2 
+0002ae60: 7c20 7763 202d 6c27 0a0a 2020 2020 4070  | wc -l'..    @p
+0002ae70: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
+0002ae80: 2020 6465 6620 746d 705f 736f 7572 6365    def tmp_source
+0002ae90: 2873 656c 662c 2074 6d70 5f70 6174 6829  (self, tmp_path)
+0002aea0: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
+0002aeb0: 7465 7320 6120 7465 6d70 6f72 6172 7920  tes a temporary 
+0002aec0: 6469 7265 6374 6f72 7920 7769 7468 2061  directory with a
+0002aed0: 2066 696c 6520 696e 2069 740a 2020 2020   file in it.    
+0002aee0: 2020 2020 746d 705f 6469 7220 3d20 746d      tmp_dir = tm
+0002aef0: 705f 7061 7468 202f 2027 746d 702d 736f  p_path / 'tmp-so
+0002af00: 7572 6365 270a 2020 2020 2020 2020 746d  urce'.        tm
+0002af10: 705f 6469 722e 6d6b 6469 7228 290a 2020  p_dir.mkdir().  
+0002af20: 2020 2020 2020 746d 705f 6669 6c65 203d        tmp_file =
+0002af30: 2074 6d70 5f64 6972 202f 2027 746d 702d   tmp_dir / 'tmp-
+0002af40: 6669 6c65 270a 2020 2020 2020 2020 746d  file'.        tm
+0002af50: 705f 6669 6c65 2e77 7269 7465 5f74 6578  p_file.write_tex
+0002af60: 7428 2774 6573 7427 290a 2020 2020 2020  t('test').      
+0002af70: 2020 6369 7263 6c65 5f6c 696e 6b20 3d20    circle_link = 
+0002af80: 746d 705f 6469 7220 2f20 2763 6972 636c  tmp_dir / 'circl
+0002af90: 652d 6c69 6e6b 270a 2020 2020 2020 2020  e-link'.        
+0002afa0: 6369 7263 6c65 5f6c 696e 6b2e 7379 6d6c  circle_link.syml
+0002afb0: 696e 6b5f 746f 2874 6d70 5f64 6972 2c20  ink_to(tmp_dir, 
+0002afc0: 7461 7267 6574 5f69 735f 6469 7265 6374  target_is_direct
+0002afd0: 6f72 793d 5472 7565 290a 2020 2020 2020  ory=True).      
+0002afe0: 2020 7969 656c 6420 7374 7228 746d 705f    yield str(tmp_
+0002aff0: 6469 7229 0a0a 2020 2020 4073 7461 7469  dir)..    @stati
+0002b000: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+0002b010: 6765 6e65 7261 7465 5f62 7563 6b65 745f  generate_bucket_
+0002b020: 6e61 6d65 2829 3a0a 2020 2020 2020 2020  name():.        
+0002b030: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+0002b040: 6f72 6172 7920 6275 636b 6574 206e 616d  orary bucket nam
+0002b050: 650a 2020 2020 2020 2020 2320 7469 6d65  e.        # time
+0002b060: 2e74 696d 6528 2920 7265 7475 726e 7320  .time() returns 
+0002b070: 7661 7279 696e 6720 7072 6563 6973 696f  varying precisio
+0002b080: 6e20 6f6e 2064 6966 6665 7265 6e74 2073  n on different s
+0002b090: 7973 7465 6d73 2c20 736f 2077 650a 2020  ystems, so we.  
+0002b0a0: 2020 2020 2020 2320 7265 706c 6163 6520        # replace 
+0002b0b0: 7468 6520 6465 6369 6d61 6c20 706f 696e  the decimal poin
+0002b0c0: 7420 616e 6420 7573 6520 7768 6174 6576  t and use whatev
+0002b0d0: 6572 2070 7265 6369 7369 6f6e 2077 6520  er precision we 
+0002b0e0: 6361 6e20 6765 742e 0a20 2020 2020 2020  can get..       
+0002b0f0: 2074 696d 6573 7461 6d70 203d 2073 7472   timestamp = str
+0002b100: 2874 696d 652e 7469 6d65 2829 292e 7265  (time.time()).re
+0002b110: 706c 6163 6528 272e 272c 2027 2729 0a20  place('.', ''). 
+0002b120: 2020 2020 2020 2072 6574 7572 6e20 6627         return f'
+0002b130: 736b 792d 7465 7374 2d7b 7469 6d65 7374  sky-test-{timest
+0002b140: 616d 707d 270a 0a20 2020 2040 7079 7465  amp}'..    @pyte
+0002b150: 7374 2e66 6978 7475 7265 0a20 2020 2064  st.fixture.    d
+0002b160: 6566 2074 6d70 5f62 7563 6b65 745f 6e61  ef tmp_bucket_na
+0002b170: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+0002b180: 2020 7969 656c 6420 7365 6c66 2e67 656e    yield self.gen
+0002b190: 6572 6174 655f 6275 636b 6574 5f6e 616d  erate_bucket_nam
+0002b1a0: 6528 290a 0a20 2020 2040 7374 6174 6963  e()..    @static
+0002b1b0: 6d65 7468 6f64 0a20 2020 2064 6566 2079  method.    def y
+0002b1c0: 6965 6c64 5f73 746f 7261 6765 5f6f 626a  ield_storage_obj
+0002b1d0: 6563 7428 0a20 2020 2020 2020 2020 2020  ect(.           
+0002b1e0: 206e 616d 653a 204f 7074 696f 6e61 6c5b   name: Optional[
+0002b1f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0002b200: 2020 2020 2020 2020 2073 6f75 7263 653a           source:
+0002b210: 204f 7074 696f 6e61 6c5b 7374 6f72 6167   Optional[storag
+0002b220: 655f 6c69 622e 5061 7468 5d20 3d20 4e6f  e_lib.Path] = No
+0002b230: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0002b240: 7374 6f72 6573 3a20 4f70 7469 6f6e 616c  stores: Optional
+0002b250: 5b44 6963 745b 7374 6f72 6167 655f 6c69  [Dict[storage_li
+0002b260: 622e 5374 6f72 6554 7970 652c 0a20 2020  b.StoreType,.   
+0002b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0002b290: 746f 7261 6765 5f6c 6962 2e41 6273 7472  torage_lib.Abstr
+0002b2a0: 6163 7453 746f 7265 5d5d 203d 204e 6f6e  actStore]] = Non
+0002b2b0: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+0002b2c0: 6572 7369 7374 656e 743a 204f 7074 696f  ersistent: Optio
+0002b2d0: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
+0002b2e0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+0002b2f0: 6465 3a20 7374 6f72 6167 655f 6c69 622e  de: storage_lib.
+0002b300: 5374 6f72 6167 654d 6f64 6520 3d20 7374  StorageMode = st
+0002b310: 6f72 6167 655f 6c69 622e 5374 6f72 6167  orage_lib.Storag
+0002b320: 654d 6f64 652e 4d4f 554e 5429 3a0a 2020  eMode.MOUNT):.  
+0002b330: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
+0002b340: 6120 7465 6d70 6f72 6172 7920 7374 6f72  a temporary stor
+0002b350: 6167 6520 6f62 6a65 6374 2e20 5374 6f72  age object. Stor
+0002b360: 6573 206d 7573 7420 6265 2061 6464 6564  es must be added
+0002b370: 2069 6e20 7468 6520 7465 7374 2e0a 2020   in the test..  
+0002b380: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+0002b390: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
+0002b3a0: 5374 6f72 6167 6528 6e61 6d65 3d6e 616d  Storage(name=nam
+0002b3b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0002b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b3d0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+0002b3e0: 7263 653d 736f 7572 6365 2c0a 2020 2020  rce=source,.    
+0002b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b410: 2020 2020 2020 7374 6f72 6573 3d73 746f        stores=sto
+0002b420: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+0002b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b440: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002b450: 6572 7369 7374 656e 743d 7065 7273 6973  ersistent=persis
+0002b460: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
+0002b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b490: 6d6f 6465 3d6d 6f64 6529 0a20 2020 2020  mode=mode).     
+0002b4a0: 2020 2079 6965 6c64 2073 746f 7261 6765     yield storage
+0002b4b0: 5f6f 626a 0a20 2020 2020 2020 2068 616e  _obj.        han
+0002b4c0: 646c 6520 3d20 676c 6f62 616c 5f75 7365  dle = global_use
+0002b4d0: 725f 7374 6174 652e 6765 745f 6861 6e64  r_state.get_hand
+0002b4e0: 6c65 5f66 726f 6d5f 7374 6f72 6167 655f  le_from_storage_
+0002b4f0: 6e61 6d65 280a 2020 2020 2020 2020 2020  name(.          
+0002b500: 2020 7374 6f72 6167 655f 6f62 6a2e 6e61    storage_obj.na
+0002b510: 6d65 290a 2020 2020 2020 2020 6966 2068  me).        if h
+0002b520: 616e 646c 653a 0a20 2020 2020 2020 2020  andle:.         
+0002b530: 2020 2023 2049 6620 6861 6e64 6c65 2065     # If handle e
+0002b540: 7869 7374 732c 2064 656c 6574 6520 6d61  xists, delete ma
+0002b550: 6e75 616c 6c79 0a20 2020 2020 2020 2020  nually.         
+0002b560: 2020 2023 2054 4f44 4f28 726f 6d69 6c62     # TODO(romilb
+0002b570: 293a 2054 6869 7320 6973 2070 6f74 656e  ): This is poten
+0002b580: 7469 616c 6c79 2072 6973 6b79 202d 2069  tially risky - i
+0002b590: 6620 7468 6520 6465 6c65 7465 206d 6574  f the delete met
+0002b5a0: 686f 6420 6861 730a 2020 2020 2020 2020  hod has.        
+0002b5b0: 2020 2020 2320 2020 6275 6773 2c20 7468      #   bugs, th
+0002b5c0: 6973 2063 616e 2063 6175 7365 2072 6573  is can cause res
+0002b5d0: 6f75 7263 6520 6c65 616b 732e 2049 6465  ource leaks. Ide
+0002b5e0: 616c 6c79 2077 6520 7368 6f75 6c64 206d  ally we should m
+0002b5f0: 616e 7561 6c6c 790a 2020 2020 2020 2020  anually.        
+0002b600: 2020 2020 2320 2020 656a 6563 7420 7374      #   eject st
+0002b610: 6f72 6167 6520 6672 6f6d 2067 6c6f 6261  orage from globa
+0002b620: 6c5f 7573 6572 5f73 7461 7465 2061 6e64  l_user_state and
+0002b630: 2064 656c 6574 6520 7468 6520 6275 636b   delete the buck
+0002b640: 6574 2075 7369 6e67 0a20 2020 2020 2020  et using.       
+0002b650: 2020 2020 2023 2020 2062 6f74 6f33 2064       #   boto3 d
+0002b660: 6972 6563 746c 792e 0a20 2020 2020 2020  irectly..       
+0002b670: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+0002b680: 2e64 656c 6574 6528 290a 0a20 2020 2040  .delete()..    @
+0002b690: 7079 7465 7374 2e66 6978 7475 7265 0a20  pytest.fixture. 
+0002b6a0: 2020 2064 6566 2074 6d70 5f73 6372 6174     def tmp_scrat
+0002b6b0: 6368 5f73 746f 7261 6765 5f6f 626a 2873  ch_storage_obj(s
+0002b6c0: 656c 662c 2074 6d70 5f62 7563 6b65 745f  elf, tmp_bucket_
+0002b6d0: 6e61 6d65 293a 0a20 2020 2020 2020 2023  name):.        #
+0002b6e0: 2043 7265 6174 6573 2061 2073 746f 7261   Creates a stora
+0002b6f0: 6765 206f 626a 6563 7420 7769 7468 206e  ge object with n
+0002b700: 6f20 736f 7572 6365 2074 6f20 6372 6561  o source to crea
+0002b710: 7465 2061 2073 6372 6174 6368 2073 746f  te a scratch sto
+0002b720: 7261 6765 2e0a 2020 2020 2020 2020 2320  rage..        # 
+0002b730: 5374 6f72 6573 206d 7573 7420 6265 2061  Stores must be a
+0002b740: 6464 6564 2069 6e20 7468 6520 7465 7374  dded in the test
+0002b750: 2e0a 2020 2020 2020 2020 7969 656c 6420  ..        yield 
+0002b760: 6672 6f6d 2073 656c 662e 7969 656c 645f  from self.yield_
+0002b770: 7374 6f72 6167 655f 6f62 6a65 6374 286e  storage_object(n
+0002b780: 616d 653d 746d 705f 6275 636b 6574 5f6e  ame=tmp_bucket_n
+0002b790: 616d 6529 0a0a 2020 2020 4070 7974 6573  ame)..    @pytes
+0002b7a0: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
+0002b7b0: 6620 746d 705f 6d75 6c74 6970 6c65 5f73  f tmp_multiple_s
+0002b7c0: 6372 6174 6368 5f73 746f 7261 6765 5f6f  cratch_storage_o
+0002b7d0: 626a 2873 656c 6629 3a0a 2020 2020 2020  bj(self):.      
+0002b7e0: 2020 2320 4372 6561 7465 7320 6120 6c69    # Creates a li
+0002b7f0: 7374 206f 6620 3520 7374 6f72 6167 6520  st of 5 storage 
+0002b800: 6f62 6a65 6374 7320 7769 7468 206e 6f20  objects with no 
+0002b810: 736f 7572 6365 2074 6f20 6372 6561 7465  source to create
+0002b820: 0a20 2020 2020 2020 2023 206d 756c 7469  .        # multi
+0002b830: 706c 6520 7363 7261 7463 6820 7374 6f72  ple scratch stor
+0002b840: 6167 6573 2e0a 2020 2020 2020 2020 2320  ages..        # 
+0002b850: 5374 6f72 6573 2066 6f72 2065 6163 6820  Stores for each 
+0002b860: 6f62 6a65 6374 2069 6e20 7468 6520 6c69  object in the li
+0002b870: 7374 206d 7573 7420 6265 2061 6464 6564  st must be added
+0002b880: 2069 6e20 7468 6520 7465 7374 2e0a 2020   in the test..  
+0002b890: 2020 2020 2020 7374 6f72 6167 655f 6d75        storage_mu
+0002b8a0: 6c74 5f6f 626a 203d 205b 5d0a 2020 2020  lt_obj = [].    
+0002b8b0: 2020 2020 666f 7220 5f20 696e 2072 616e      for _ in ran
+0002b8c0: 6765 2835 293a 0a20 2020 2020 2020 2020  ge(5):.         
+0002b8d0: 2020 2074 696d 6573 7461 6d70 203d 2073     timestamp = s
+0002b8e0: 7472 2874 696d 652e 7469 6d65 2829 292e  tr(time.time()).
+0002b8f0: 7265 706c 6163 6528 272e 272c 2027 2729  replace('.', '')
+0002b900: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
+0002b910: 7265 5f6f 626a 203d 2073 746f 7261 6765  re_obj = storage
+0002b920: 5f6c 6962 2e53 746f 7261 6765 286e 616d  _lib.Storage(nam
+0002b930: 653d 6627 736b 792d 7465 7374 2d7b 7469  e=f'sky-test-{ti
+0002b940: 6d65 7374 616d 707d 2729 0a20 2020 2020  mestamp}').     
+0002b950: 2020 2020 2020 2073 746f 7261 6765 5f6d         storage_m
+0002b960: 756c 745f 6f62 6a2e 6170 7065 6e64 2873  ult_obj.append(s
+0002b970: 746f 7265 5f6f 626a 290a 2020 2020 2020  tore_obj).      
+0002b980: 2020 7969 656c 6420 7374 6f72 6167 655f    yield storage_
+0002b990: 6d75 6c74 5f6f 626a 0a20 2020 2020 2020  mult_obj.       
+0002b9a0: 2066 6f72 2073 746f 7261 6765 5f6f 626a   for storage_obj
+0002b9b0: 2069 6e20 7374 6f72 6167 655f 6d75 6c74   in storage_mult
+0002b9c0: 5f6f 626a 3a0a 2020 2020 2020 2020 2020  _obj:.          
+0002b9d0: 2020 6861 6e64 6c65 203d 2067 6c6f 6261    handle = globa
+0002b9e0: 6c5f 7573 6572 5f73 7461 7465 2e67 6574  l_user_state.get
+0002b9f0: 5f68 616e 646c 655f 6672 6f6d 5f73 746f  _handle_from_sto
+0002ba00: 7261 6765 5f6e 616d 6528 0a20 2020 2020  rage_name(.     
+0002ba10: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+0002ba20: 6765 5f6f 626a 2e6e 616d 6529 0a20 2020  ge_obj.name).   
+0002ba30: 2020 2020 2020 2020 2069 6620 6861 6e64           if hand
+0002ba40: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+0002ba50: 2020 2020 2320 4966 2068 616e 646c 6520      # If handle 
+0002ba60: 6578 6973 7473 2c20 6465 6c65 7465 206d  exists, delete m
+0002ba70: 616e 7561 6c6c 790a 2020 2020 2020 2020  anually.        
+0002ba80: 2020 2020 2020 2020 2320 544f 444f 2872          # TODO(r
+0002ba90: 6f6d 696c 6229 3a20 5468 6973 2069 7320  omilb): This is 
+0002baa0: 706f 7465 6e74 6961 6c6c 7920 7269 736b  potentially risk
+0002bab0: 7920 2d20 6966 2074 6865 2064 656c 6574  y - if the delet
+0002bac0: 6520 6d65 7468 6f64 2068 6173 0a20 2020  e method has.   
+0002bad0: 2020 2020 2020 2020 2020 2020 2023 2062               # b
+0002bae0: 7567 732c 2074 6869 7320 6361 6e20 6361  ugs, this can ca
+0002baf0: 7573 6520 7265 736f 7572 6365 206c 6561  use resource lea
+0002bb00: 6b73 2e20 4964 6561 6c6c 7920 7765 2073  ks. Ideally we s
+0002bb10: 686f 756c 6420 6d61 6e75 616c 6c79 0a20  hould manually. 
+0002bb20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0002bb30: 2065 6a65 6374 2073 746f 7261 6765 2066   eject storage f
+0002bb40: 726f 6d20 676c 6f62 616c 5f75 7365 725f  rom global_user_
+0002bb50: 7374 6174 6520 616e 6420 6465 6c65 7465  state and delete
+0002bb60: 2074 6865 2062 7563 6b65 7420 7573 696e   the bucket usin
+0002bb70: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+0002bb80: 2020 2320 626f 746f 3320 6469 7265 6374    # boto3 direct
+0002bb90: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+0002bba0: 2020 2020 7374 6f72 6167 655f 6f62 6a2e      storage_obj.
+0002bbb0: 6465 6c65 7465 2829 0a0a 2020 2020 4070  delete()..    @p
+0002bbc0: 7974 6573 742e 6669 7874 7572 650a 2020  ytest.fixture.  
+0002bbd0: 2020 6465 6620 746d 705f 6d75 6c74 6970    def tmp_multip
+0002bbe0: 6c65 5f63 7573 746f 6d5f 736f 7572 6365  le_custom_source
+0002bbf0: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
+0002bc00: 6629 3a0a 2020 2020 2020 2020 2320 4372  f):.        # Cr
+0002bc10: 6561 7465 7320 6120 6c69 7374 206f 6620  eates a list of 
+0002bc20: 7374 6f72 6167 6520 6f62 6a65 6374 7320  storage objects 
+0002bc30: 7769 7468 2063 7573 746f 6d20 736f 7572  with custom sour
+0002bc40: 6365 206e 616d 6573 2074 6f0a 2020 2020  ce names to.    
+0002bc50: 2020 2020 2320 6372 6561 7465 206d 756c      # create mul
+0002bc60: 7469 706c 6520 7363 7261 7463 6820 7374  tiple scratch st
+0002bc70: 6f72 6167 6573 2e0a 2020 2020 2020 2020  orages..        
+0002bc80: 2320 5374 6f72 6573 2066 6f72 2065 6163  # Stores for eac
+0002bc90: 6820 6f62 6a65 6374 2069 6e20 7468 6520  h object in the 
+0002bca0: 6c69 7374 206d 7573 7420 6265 2061 6464  list must be add
+0002bcb0: 6564 2069 6e20 7468 6520 7465 7374 2e0a  ed in the test..
+0002bcc0: 2020 2020 2020 2020 6375 7374 6f6d 5f73          custom_s
+0002bcd0: 6f75 7263 655f 6e61 6d65 7320 3d20 5b27  ource_names = ['
+0002bce0: 2270 6174 6820 5769 7468 2053 7061 6365  "path With Space
+0002bcf0: 7322 272c 2027 7061 7468 2057 6974 6820  s"', 'path With 
+0002bd00: 5370 6163 6573 275d 0a20 2020 2020 2020  Spaces'].       
+0002bd10: 2073 746f 7261 6765 5f6d 756c 745f 6f62   storage_mult_ob
+0002bd20: 6a20 3d20 5b5d 0a20 2020 2020 2020 2066  j = [].        f
+0002bd30: 6f72 206e 616d 6520 696e 2063 7573 746f  or name in custo
+0002bd40: 6d5f 736f 7572 6365 5f6e 616d 6573 3a0a  m_source_names:.
+0002bd50: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+0002bd60: 7061 7468 203d 206f 732e 7061 7468 2e65  path = os.path.e
+0002bd70: 7870 616e 6475 7365 7228 6627 7e2f 7b6e  xpanduser(f'~/{n
+0002bd80: 616d 657d 2729 0a20 2020 2020 2020 2020  ame}').         
+0002bd90: 2020 2070 6174 686c 6962 2e50 6174 6828     pathlib.Path(
+0002bda0: 7372 635f 7061 7468 292e 6578 7061 6e64  src_path).expand
+0002bdb0: 7573 6572 2829 2e6d 6b64 6972 2865 7869  user().mkdir(exi
+0002bdc0: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
+0002bdd0: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+0002bde0: 7020 3d20 7374 7228 7469 6d65 2e74 696d  p = str(time.tim
+0002bdf0: 6528 2929 2e72 6570 6c61 6365 2827 2e27  e()).replace('.'
+0002be00: 2c20 2727 290a 2020 2020 2020 2020 2020  , '').          
+0002be10: 2020 7374 6f72 655f 6f62 6a20 3d20 7374    store_obj = st
+0002be20: 6f72 6167 655f 6c69 622e 5374 6f72 6167  orage_lib.Storag
+0002be30: 6528 6e61 6d65 3d66 2773 6b79 2d74 6573  e(name=f'sky-tes
+0002be40: 742d 7b74 696d 6573 7461 6d70 7d27 2c0a  t-{timestamp}',.
+0002be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002be70: 2020 2020 2020 2020 2020 2020 736f 7572              sour
+0002be80: 6365 3d73 7263 5f70 6174 6829 0a20 2020  ce=src_path).   
+0002be90: 2020 2020 2020 2020 2073 746f 7261 6765           storage
+0002bea0: 5f6d 756c 745f 6f62 6a2e 6170 7065 6e64  _mult_obj.append
+0002beb0: 2873 746f 7265 5f6f 626a 290a 2020 2020  (store_obj).    
+0002bec0: 2020 2020 7969 656c 6420 7374 6f72 6167      yield storag
+0002bed0: 655f 6d75 6c74 5f6f 626a 0a20 2020 2020  e_mult_obj.     
+0002bee0: 2020 2066 6f72 2073 746f 7261 6765 5f6f     for storage_o
+0002bef0: 626a 2069 6e20 7374 6f72 6167 655f 6d75  bj in storage_mu
+0002bf00: 6c74 5f6f 626a 3a0a 2020 2020 2020 2020  lt_obj:.        
+0002bf10: 2020 2020 6861 6e64 6c65 203d 2067 6c6f      handle = glo
+0002bf20: 6261 6c5f 7573 6572 5f73 7461 7465 2e67  bal_user_state.g
+0002bf30: 6574 5f68 616e 646c 655f 6672 6f6d 5f73  et_handle_from_s
+0002bf40: 746f 7261 6765 5f6e 616d 6528 0a20 2020  torage_name(.   
+0002bf50: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+0002bf60: 7261 6765 5f6f 626a 2e6e 616d 6529 0a20  rage_obj.name). 
+0002bf70: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+0002bf80: 6e64 6c65 3a0a 2020 2020 2020 2020 2020  ndle:.          
+0002bf90: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+0002bfa0: 6a2e 6465 6c65 7465 2829 0a0a 2020 2020  j.delete()..    
+0002bfb0: 4070 7974 6573 742e 6669 7874 7572 650a  @pytest.fixture.
+0002bfc0: 2020 2020 6465 6620 746d 705f 6c6f 6361      def tmp_loca
+0002bfd0: 6c5f 7374 6f72 6167 655f 6f62 6a28 7365  l_storage_obj(se
+0002bfe0: 6c66 2c20 746d 705f 6275 636b 6574 5f6e  lf, tmp_bucket_n
+0002bff0: 616d 652c 2074 6d70 5f73 6f75 7263 6529  ame, tmp_source)
+0002c000: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
+0002c010: 7465 7320 6120 7465 6d70 6f72 6172 7920  tes a temporary 
+0002c020: 7374 6f72 6167 6520 6f62 6a65 6374 2e20  storage object. 
+0002c030: 5374 6f72 6573 206d 7573 7420 6265 2061  Stores must be a
+0002c040: 6464 6564 2069 6e20 7468 6520 7465 7374  dded in the test
+0002c050: 2e0a 2020 2020 2020 2020 7969 656c 6420  ..        yield 
+0002c060: 6672 6f6d 2073 656c 662e 7969 656c 645f  from self.yield_
+0002c070: 7374 6f72 6167 655f 6f62 6a65 6374 286e  storage_object(n
+0002c080: 616d 653d 746d 705f 6275 636b 6574 5f6e  ame=tmp_bucket_n
+0002c090: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0002c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c0c0: 2020 736f 7572 6365 3d74 6d70 5f73 6f75    source=tmp_sou
+0002c0d0: 7263 6529 0a0a 2020 2020 4070 7974 6573  rce)..    @pytes
+0002c0e0: 742e 6669 7874 7572 650a 2020 2020 6465  t.fixture.    de
+0002c0f0: 6620 746d 705f 6c6f 6361 6c5f 6c69 7374  f tmp_local_list
+0002c100: 5f73 746f 7261 6765 5f6f 626a 2873 656c  _storage_obj(sel
+0002c110: 662c 2074 6d70 5f62 7563 6b65 745f 6e61  f, tmp_bucket_na
+0002c120: 6d65 2c20 746d 705f 736f 7572 6365 293a  me, tmp_source):
+0002c130: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+0002c140: 6573 2061 2074 656d 7020 7374 6f72 6167  es a temp storag
+0002c150: 6520 6f62 6a65 6374 2077 6869 6368 2075  e object which u
+0002c160: 7365 7320 6120 6c69 7374 206f 6620 7061  ses a list of pa
+0002c170: 7468 7320 6173 2073 6f75 7263 652e 0a20  ths as source.. 
+0002c180: 2020 2020 2020 2023 2053 746f 7265 7320         # Stores 
+0002c190: 6d75 7374 2062 6520 6164 6465 6420 696e  must be added in
+0002c1a0: 2074 6865 2074 6573 742e 2041 6674 6572   the test. After
+0002c1b0: 2075 706c 6f61 642c 2074 6865 2062 7563   upload, the buc
+0002c1c0: 6b65 7420 7368 6f75 6c64 0a20 2020 2020  ket should.     
+0002c1d0: 2020 2023 2068 6176 6520 7477 6f20 6669     # have two fi
+0002c1e0: 6c65 7320 2d20 2f74 6d70 2d66 696c 6520  les - /tmp-file 
+0002c1f0: 616e 6420 2f74 6d70 2d73 6f75 7263 652f  and /tmp-source/
+0002c200: 746d 702d 6669 6c65 0a20 2020 2020 2020  tmp-file.       
+0002c210: 206c 6973 745f 736f 7572 6365 203d 205b   list_source = [
+0002c220: 746d 705f 736f 7572 6365 2c20 746d 705f  tmp_source, tmp_
+0002c230: 736f 7572 6365 202b 2027 2f74 6d70 2d66  source + '/tmp-f
+0002c240: 696c 6527 5d0a 2020 2020 2020 2020 7969  ile'].        yi
+0002c250: 656c 6420 6672 6f6d 2073 656c 662e 7969  eld from self.yi
+0002c260: 656c 645f 7374 6f72 6167 655f 6f62 6a65  eld_storage_obje
+0002c270: 6374 286e 616d 653d 746d 705f 6275 636b  ct(name=tmp_buck
+0002c280: 6574 5f6e 616d 652c 0a20 2020 2020 2020  et_name,.       
+0002c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c2b0: 2020 2020 2020 736f 7572 6365 3d6c 6973        source=lis
+0002c2c0: 745f 736f 7572 6365 290a 0a20 2020 2040  t_source)..    @
+0002c2d0: 7079 7465 7374 2e66 6978 7475 7265 0a20  pytest.fixture. 
+0002c2e0: 2020 2064 6566 2074 6d70 5f62 756c 6b5f     def tmp_bulk_
+0002c2f0: 6465 6c5f 7374 6f72 6167 655f 6f62 6a28  del_storage_obj(
+0002c300: 7365 6c66 2c20 746d 705f 6275 636b 6574  self, tmp_bucket
+0002c310: 5f6e 616d 6529 3a0a 2020 2020 2020 2020  _name):.        
+0002c320: 2320 4372 6561 7465 7320 6120 7465 6d70  # Creates a temp
+0002c330: 6f72 6172 7920 7374 6f72 6167 6520 6f62  orary storage ob
+0002c340: 6a65 6374 2066 6f72 2074 6573 7469 6e67  ject for testing
+0002c350: 2062 756c 6b20 6465 6c65 7469 6f6e 2e0a   bulk deletion..
+0002c360: 2020 2020 2020 2020 2320 5374 6f72 6573          # Stores
+0002c370: 206d 7573 7420 6265 2061 6464 6564 2069   must be added i
+0002c380: 6e20 7468 6520 7465 7374 2e0a 2020 2020  n the test..    
+0002c390: 2020 2020 7769 7468 2074 656d 7066 696c      with tempfil
+0002c3a0: 652e 5465 6d70 6f72 6172 7944 6972 6563  e.TemporaryDirec
+0002c3b0: 746f 7279 2829 2061 7320 746d 7064 6972  tory() as tmpdir
+0002c3c0: 3a0a 2020 2020 2020 2020 2020 2020 7375  :.            su
+0002c3d0: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+0002c3e0: 7574 7075 7428 6627 6d6b 6469 7220 2d70  utput(f'mkdir -p
+0002c3f0: 207b 746d 7064 6972 7d2f 666f 6c64 6572   {tmpdir}/folder
+0002c400: 7b7b 3030 302e 2e32 3535 7d7d 272c 0a20  {{000..255}}',. 
+0002c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c430: 2020 2073 6865 6c6c 3d54 7275 6529 0a20     shell=True). 
+0002c440: 2020 2020 2020 2020 2020 2073 7562 7072             subpr
+0002c450: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+0002c460: 7574 2866 2774 6f75 6368 207b 746d 7064  ut(f'touch {tmpd
+0002c470: 6972 7d2f 7465 7374 7b7b 3030 302e 2e32  ir}/test{{000..2
+0002c480: 3535 7d7d 2e74 7874 272c 0a20 2020 2020  55}}.txt',.     
+0002c490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0002c4b0: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
+0002c4c0: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
+0002c4d0: 732e 6368 6563 6b5f 6f75 7470 7574 280a  s.check_output(.
+0002c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c4f0: 6627 746f 7563 6820 7b74 6d70 6469 727d  f'touch {tmpdir}
+0002c500: 2f66 6f6c 6465 727b 7b30 3030 2e2e 3235  /folder{{000..25
+0002c510: 357d 7d2f 7465 7374 2e74 7874 272c 2073  5}}/test.txt', s
+0002c520: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
+0002c530: 2020 2020 2020 2079 6965 6c64 2066 726f         yield fro
+0002c540: 6d20 7365 6c66 2e79 6965 6c64 5f73 746f  m self.yield_sto
+0002c550: 7261 6765 5f6f 626a 6563 7428 6e61 6d65  rage_object(name
+0002c560: 3d74 6d70 5f62 7563 6b65 745f 6e61 6d65  =tmp_bucket_name
+0002c570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c5a0: 2020 2073 6f75 7263 653d 746d 7064 6972     source=tmpdir
+0002c5b0: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
+0002c5c0: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
+0002c5d0: 6d70 5f63 6f70 795f 6d6e 745f 6578 6973  mp_copy_mnt_exis
+0002c5e0: 7469 6e67 5f73 746f 7261 6765 5f6f 626a  ting_storage_obj
+0002c5f0: 2873 656c 662c 2074 6d70 5f73 6372 6174  (self, tmp_scrat
+0002c600: 6368 5f73 746f 7261 6765 5f6f 626a 293a  ch_storage_obj):
+0002c610: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+0002c620: 6573 2061 2063 6f70 7920 6d6f 756e 7420  es a copy mount 
+0002c630: 7374 6f72 6167 6520 7768 6963 6820 7265  storage which re
+0002c640: 7573 6573 2061 6e20 6578 6973 7469 6e67  uses an existing
+0002c650: 2073 746f 7261 6765 206f 626a 6563 742e   storage object.
+0002c660: 0a20 2020 2020 2020 2074 6d70 5f73 6372  .        tmp_scr
+0002c670: 6174 6368 5f73 746f 7261 6765 5f6f 626a  atch_storage_obj
+0002c680: 2e61 6464 5f73 746f 7265 2873 746f 7261  .add_store(stora
+0002c690: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+0002c6a0: 2e53 3329 0a20 2020 2020 2020 2073 746f  .S3).        sto
+0002c6b0: 7261 6765 5f6e 616d 6520 3d20 746d 705f  rage_name = tmp_
+0002c6c0: 7363 7261 7463 685f 7374 6f72 6167 655f  scratch_storage_
+0002c6d0: 6f62 6a2e 6e61 6d65 0a0a 2020 2020 2020  obj.name..      
+0002c6e0: 2020 2320 5472 7920 746f 2069 6e69 7469    # Try to initi
+0002c6f0: 616c 697a 6520 616e 6f74 6865 7220 7374  alize another st
+0002c700: 6f72 6167 6520 7769 7468 2074 6865 2073  orage with the s
+0002c710: 746f 7261 6765 206f 626a 6563 7420 6372  torage object cr
+0002c720: 6561 7465 640a 2020 2020 2020 2020 2320  eated.        # 
+0002c730: 6162 6f76 652c 2062 7574 206e 6f77 2069  above, but now i
+0002c740: 6e20 434f 5059 206d 6f64 652e 2054 6869  n COPY mode. Thi
+0002c750: 7320 7368 6f75 6c64 2073 7563 6365 6564  s should succeed
+0002c760: 2e0a 2020 2020 2020 2020 7969 656c 6420  ..        yield 
+0002c770: 6672 6f6d 2073 656c 662e 7969 656c 645f  from self.yield_
+0002c780: 7374 6f72 6167 655f 6f62 6a65 6374 286e  storage_object(n
+0002c790: 616d 653d 7374 6f72 6167 655f 6e61 6d65  ame=storage_name
+0002c7a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002c7c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002c7d0: 6f64 653d 7374 6f72 6167 655f 6c69 622e  ode=storage_lib.
+0002c7e0: 5374 6f72 6167 654d 6f64 652e 434f 5059  StorageMode.COPY
+0002c7f0: 290a 0a20 2020 2040 7079 7465 7374 2e66  )..    @pytest.f
+0002c800: 6978 7475 7265 0a20 2020 2064 6566 2074  ixture.    def t
+0002c810: 6d70 5f67 6974 6967 6e6f 7265 5f73 746f  mp_gitignore_sto
+0002c820: 7261 6765 5f6f 626a 2873 656c 662c 2074  rage_obj(self, t
+0002c830: 6d70 5f62 7563 6b65 745f 6e61 6d65 2c20  mp_bucket_name, 
+0002c840: 6769 7469 676e 6f72 655f 7374 7275 6374  gitignore_struct
+0002c850: 7572 6529 3a0a 2020 2020 2020 2020 2320  ure):.        # 
+0002c860: 4372 6561 7465 7320 6120 7465 6d70 6f72  Creates a tempor
+0002c870: 6172 7920 7374 6f72 6167 6520 6f62 6a65  ary storage obje
+0002c880: 6374 2066 6f72 2074 6573 7469 6e67 202e  ct for testing .
+0002c890: 6769 7469 676e 6f72 6520 6669 6c74 6572  gitignore filter
+0002c8a0: 2e0a 2020 2020 2020 2020 2320 4749 5449  ..        # GITI
+0002c8b0: 4749 4e4f 5245 5f53 5452 5543 5455 5245  GINORE_STRUCTURE
+0002c8c0: 2069 7320 7265 7072 6573 656e 7469 6e67   is representing
+0002c8d0: 2061 2066 696c 6520 7374 7275 6374 7572   a file structur
+0002c8e0: 6520 696e 2061 2064 6963 7469 6f6e 6172  e in a dictionar
+0002c8f0: 790a 2020 2020 2020 2020 2320 666f 726d  y.        # form
+0002c900: 6174 2e20 4372 6561 7465 6420 7374 6f72  at. Created stor
+0002c910: 6167 6520 6f62 6a65 6374 2077 696c 6c20  age object will 
+0002c920: 636f 6e74 6169 6e20 7468 6520 6669 6c65  contain the file
+0002c930: 2073 7472 7563 7475 7265 2061 6c6f 6e67   structure along
+0002c940: 0a20 2020 2020 2020 2023 2077 6974 6820  .        # with 
+0002c950: 2e67 6974 6967 6e6f 7265 2061 6e64 202e  .gitignore and .
+0002c960: 6769 742f 696e 666f 2f65 7863 6c75 6465  git/info/exclude
+0002c970: 2066 696c 6573 2074 6f20 7465 7374 2065   files to test e
+0002c980: 7863 6c75 6465 2066 696c 7465 722e 0a20  xclude filter.. 
+0002c990: 2020 2020 2020 2023 2053 746f 7265 7320         # Stores 
+0002c9a0: 6d75 7374 2062 6520 6164 6465 6420 696e  must be added in
+0002c9b0: 2074 6865 2074 6573 742e 0a20 2020 2020   the test..     
+0002c9c0: 2020 2077 6974 6820 7465 6d70 6669 6c65     with tempfile
+0002c9d0: 2e54 656d 706f 7261 7279 4469 7265 6374  .TemporaryDirect
+0002c9e0: 6f72 7928 2920 6173 2074 6d70 6469 723a  ory() as tmpdir:
+0002c9f0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0002ca00: 7265 6174 6573 2066 696c 6520 7374 7275  reates file stru
+0002ca10: 6374 7572 6520 746f 2062 6520 7570 6c6f  cture to be uplo
+0002ca20: 6164 6564 2069 6e20 7468 6520 5374 6f72  aded in the Stor
+0002ca30: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+0002ca40: 7365 6c66 2e63 7265 6174 655f 6469 725f  self.create_dir_
+0002ca50: 7374 7275 6374 7572 6528 746d 7064 6972  structure(tmpdir
+0002ca60: 2c20 6769 7469 676e 6f72 655f 7374 7275  , gitignore_stru
+0002ca70: 6374 7572 6529 0a0a 2020 2020 2020 2020  cture)..        
+0002ca80: 2020 2020 2320 4372 6561 7465 202e 6769      # Create .gi
+0002ca90: 7469 676e 6f72 6520 616e 6420 6c69 7374  tignore and list
+0002caa0: 2066 696c 6573 2f64 6972 7320 746f 2062   files/dirs to b
+0002cab0: 6520 6578 636c 7564 6564 2069 6e20 6974  e excluded in it
+0002cac0: 0a20 2020 2020 2020 2020 2020 2073 6b79  .            sky
+0002cad0: 7069 6c6f 745f 7061 7468 203d 206f 732e  pilot_path = os.
+0002cae0: 7061 7468 2e64 6972 6e61 6d65 286f 732e  path.dirname(os.
+0002caf0: 7061 7468 2e64 6972 6e61 6d65 2873 6b79  path.dirname(sky
+0002cb00: 2e5f 5f66 696c 655f 5f29 290a 2020 2020  .__file__)).    
+0002cb10: 2020 2020 2020 2020 7465 6d70 5f70 6174          temp_pat
+0002cb20: 6820 3d20 6627 7b74 6d70 6469 727d 2f2e  h = f'{tmpdir}/.
+0002cb30: 6769 7469 676e 6f72 6527 0a20 2020 2020  gitignore'.     
+0002cb40: 2020 2020 2020 2066 696c 655f 7061 7468         file_path
+0002cb50: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0002cb60: 736b 7970 696c 6f74 5f70 6174 682c 2027  skypilot_path, '
+0002cb70: 7465 7374 732f 6769 7469 676e 6f72 655f  tests/gitignore_
+0002cb80: 7465 7374 2729 0a20 2020 2020 2020 2020  test').         
+0002cb90: 2020 2073 6875 7469 6c2e 636f 7079 6669     shutil.copyfi
+0002cba0: 6c65 2866 696c 655f 7061 7468 2c20 7465  le(file_path, te
+0002cbb0: 6d70 5f70 6174 6829 0a0a 2020 2020 2020  mp_path)..      
+0002cbc0: 2020 2020 2020 2320 4372 6561 7465 202e        # Create .
+0002cbd0: 6769 742f 696e 666f 2f65 7863 6c75 6465  git/info/exclude
+0002cbe0: 2061 6e64 206c 6973 7420 6669 6c65 732f   and list files/
+0002cbf0: 6469 7273 2074 6f20 6265 2065 7863 6c75  dirs to be exclu
+0002cc00: 6465 6420 696e 2069 740a 2020 2020 2020  ded in it.      
+0002cc10: 2020 2020 2020 7465 6d70 5f70 6174 6820        temp_path 
+0002cc20: 3d20 6627 7b74 6d70 6469 727d 2f2e 6769  = f'{tmpdir}/.gi
+0002cc30: 742f 696e 666f 2f27 0a20 2020 2020 2020  t/info/'.       
+0002cc40: 2020 2020 206f 732e 6d61 6b65 6469 7273       os.makedirs
+0002cc50: 2874 656d 705f 7061 7468 290a 2020 2020  (temp_path).    
+0002cc60: 2020 2020 2020 2020 7465 6d70 5f65 7863          temp_exc
+0002cc70: 6c75 6465 5f70 6174 6820 3d20 6f73 2e70  lude_path = os.p
+0002cc80: 6174 682e 6a6f 696e 2874 656d 705f 7061  ath.join(temp_pa
+0002cc90: 7468 2c20 2765 7863 6c75 6465 2729 0a20  th, 'exclude'). 
+0002cca0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+0002ccb0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+0002ccc0: 6f69 6e28 736b 7970 696c 6f74 5f70 6174  oin(skypilot_pat
+0002ccd0: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0002cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002ccf0: 2020 2020 2020 2020 2774 6573 7473 2f67          'tests/g
+0002cd00: 6974 5f69 6e66 6f5f 6578 636c 7564 655f  it_info_exclude_
+0002cd10: 7465 7374 2729 0a20 2020 2020 2020 2020  test').         
+0002cd20: 2020 2073 6875 7469 6c2e 636f 7079 6669     shutil.copyfi
+0002cd30: 6c65 2866 696c 655f 7061 7468 2c20 7465  le(file_path, te
+0002cd40: 6d70 5f65 7863 6c75 6465 5f70 6174 6829  mp_exclude_path)
+0002cd50: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0002cd60: 4372 6561 7465 2073 6b79 2053 746f 7261  Create sky Stora
+0002cd70: 6765 2077 6974 6820 7468 6520 6669 6c65  ge with the file
+0002cd80: 7320 6372 6561 7465 640a 2020 2020 2020  s created.      
+0002cd90: 2020 2020 2020 7969 656c 6420 6672 6f6d        yield from
+0002cda0: 2073 656c 662e 7969 656c 645f 7374 6f72   self.yield_stor
+0002cdb0: 6167 655f 6f62 6a65 6374 280a 2020 2020  age_object(.    
+0002cdc0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0002cdd0: 3d74 6d70 5f62 7563 6b65 745f 6e61 6d65  =tmp_bucket_name
+0002cde0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002cdf0: 2020 736f 7572 6365 3d74 6d70 6469 722c    source=tmpdir,
+0002ce00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002ce10: 206d 6f64 653d 7374 6f72 6167 655f 6c69   mode=storage_li
+0002ce20: 622e 5374 6f72 6167 654d 6f64 652e 434f  b.StorageMode.CO
+0002ce30: 5059 290a 0a20 2020 2040 7079 7465 7374  PY)..    @pytest
+0002ce40: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+0002ce50: 2074 6d70 5f61 7773 636c 695f 6275 636b   tmp_awscli_buck
+0002ce60: 6574 2873 656c 662c 2074 6d70 5f62 7563  et(self, tmp_buc
+0002ce70: 6b65 745f 6e61 6d65 293a 0a20 2020 2020  ket_name):.     
+0002ce80: 2020 2023 2043 7265 6174 6573 2061 2074     # Creates a t
+0002ce90: 656d 706f 7261 7279 2062 7563 6b65 7420  emporary bucket 
+0002cea0: 7573 696e 6720 6177 7363 6c69 0a20 2020  using awscli.   
+0002ceb0: 2020 2020 2062 7563 6b65 745f 7572 6920       bucket_uri 
+0002cec0: 3d20 6627 7333 3a2f 2f7b 746d 705f 6275  = f's3://{tmp_bu
+0002ced0: 636b 6574 5f6e 616d 657d 270a 2020 2020  cket_name}'.    
+0002cee0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+0002cef0: 6865 636b 5f63 616c 6c28 5b27 6177 7327  heck_call(['aws'
+0002cf00: 2c20 2773 3327 2c20 276d 6227 2c20 6275  , 's3', 'mb', bu
+0002cf10: 636b 6574 5f75 7269 5d29 0a20 2020 2020  cket_uri]).     
+0002cf20: 2020 2079 6965 6c64 2074 6d70 5f62 7563     yield tmp_buc
+0002cf30: 6b65 745f 6e61 6d65 2c20 6275 636b 6574  ket_name, bucket
+0002cf40: 5f75 7269 0a20 2020 2020 2020 2073 7562  _uri.        sub
+0002cf50: 7072 6f63 6573 732e 6368 6563 6b5f 6361  process.check_ca
+0002cf60: 6c6c 285b 2761 7773 272c 2027 7333 272c  ll(['aws', 's3',
+0002cf70: 2027 7262 272c 2062 7563 6b65 745f 7572   'rb', bucket_ur
+0002cf80: 692c 2027 2d2d 666f 7263 6527 5d29 0a0a  i, '--force'])..
+0002cf90: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+0002cfa0: 7572 650a 2020 2020 6465 6620 746d 705f  ure.    def tmp_
+0002cfb0: 6773 7574 696c 5f62 7563 6b65 7428 7365  gsutil_bucket(se
+0002cfc0: 6c66 2c20 746d 705f 6275 636b 6574 5f6e  lf, tmp_bucket_n
+0002cfd0: 616d 6529 3a0a 2020 2020 2020 2020 2320  ame):.        # 
+0002cfe0: 4372 6561 7465 7320 6120 7465 6d70 6f72  Creates a tempor
+0002cff0: 6172 7920 6275 636b 6574 2075 7369 6e67  ary bucket using
+0002d000: 2067 7375 7469 6c0a 2020 2020 2020 2020   gsutil.        
+0002d010: 6275 636b 6574 5f75 7269 203d 2066 2767  bucket_uri = f'g
+0002d020: 733a 2f2f 7b74 6d70 5f62 7563 6b65 745f  s://{tmp_bucket_
+0002d030: 6e61 6d65 7d27 0a20 2020 2020 2020 2073  name}'.        s
+0002d040: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0002d050: 6361 6c6c 285b 2767 7375 7469 6c27 2c20  call(['gsutil', 
+0002d060: 276d 6227 2c20 6275 636b 6574 5f75 7269  'mb', bucket_uri
+0002d070: 5d29 0a20 2020 2020 2020 2079 6965 6c64  ]).        yield
+0002d080: 2074 6d70 5f62 7563 6b65 745f 6e61 6d65   tmp_bucket_name
+0002d090: 2c20 6275 636b 6574 5f75 7269 0a20 2020  , bucket_uri.   
+0002d0a0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+0002d0b0: 6368 6563 6b5f 6361 6c6c 285b 2767 7375  check_call(['gsu
+0002d0c0: 7469 6c27 2c20 2772 6d27 2c20 272d 7227  til', 'rm', '-r'
+0002d0d0: 2c20 6275 636b 6574 5f75 7269 5d29 0a0a  , bucket_uri])..
+0002d0e0: 2020 2020 4070 7974 6573 742e 6669 7874      @pytest.fixt
+0002d0f0: 7572 650a 2020 2020 6465 6620 746d 705f  ure.    def tmp_
+0002d100: 6177 7363 6c69 5f62 7563 6b65 745f 7232  awscli_bucket_r2
+0002d110: 2873 656c 662c 2074 6d70 5f62 7563 6b65  (self, tmp_bucke
+0002d120: 745f 6e61 6d65 293a 0a20 2020 2020 2020  t_name):.       
+0002d130: 2023 2043 7265 6174 6573 2061 2074 656d   # Creates a tem
+0002d140: 706f 7261 7279 2062 7563 6b65 7420 7573  porary bucket us
+0002d150: 696e 6720 6177 7363 6c69 0a20 2020 2020  ing awscli.     
+0002d160: 2020 2065 6e64 706f 696e 745f 7572 6c20     endpoint_url 
+0002d170: 3d20 636c 6f75 6466 6c61 7265 2e63 7265  = cloudflare.cre
+0002d180: 6174 655f 656e 6470 6f69 6e74 2829 0a20  ate_endpoint(). 
+0002d190: 2020 2020 2020 2062 7563 6b65 745f 7572         bucket_ur
+0002d1a0: 6920 3d20 6627 7333 3a2f 2f7b 746d 705f  i = f's3://{tmp_
+0002d1b0: 6275 636b 6574 5f6e 616d 657d 270a 2020  bucket_name}'.  
+0002d1c0: 2020 2020 2020 7375 6270 726f 6365 7373        subprocess
+0002d1d0: 2e63 6865 636b 5f63 616c 6c28 0a20 2020  .check_call(.   
+0002d1e0: 2020 2020 2020 2020 2066 2741 5753 5f53           f'AWS_S
+0002d1f0: 4841 5245 445f 4352 4544 454e 5449 414c  HARED_CREDENTIAL
+0002d200: 535f 4649 4c45 3d7b 636c 6f75 6466 6c61  S_FILE={cloudfla
+0002d210: 7265 2e52 325f 4352 4544 454e 5449 414c  re.R2_CREDENTIAL
+0002d220: 535f 5041 5448 7d20 6177 7320 7333 206d  S_PATH} aws s3 m
+0002d230: 6220 7b62 7563 6b65 745f 7572 697d 202d  b {bucket_uri} -
+0002d240: 2d65 6e64 706f 696e 7420 7b65 6e64 706f  -endpoint {endpo
+0002d250: 696e 745f 7572 6c7d 202d 2d70 726f 6669  int_url} --profi
+0002d260: 6c65 3d72 3227 2c0a 2020 2020 2020 2020  le=r2',.        
+0002d270: 2020 2020 7368 656c 6c3d 5472 7565 290a      shell=True).
+0002d280: 2020 2020 2020 2020 7969 656c 6420 746d          yield tm
+0002d290: 705f 6275 636b 6574 5f6e 616d 652c 2062  p_bucket_name, b
+0002d2a0: 7563 6b65 745f 7572 690a 2020 2020 2020  ucket_uri.      
+0002d2b0: 2020 7375 6270 726f 6365 7373 2e63 6865    subprocess.che
+0002d2c0: 636b 5f63 616c 6c28 0a20 2020 2020 2020  ck_call(.       
+0002d2d0: 2020 2020 2066 2741 5753 5f53 4841 5245       f'AWS_SHARE
+0002d2e0: 445f 4352 4544 454e 5449 414c 535f 4649  D_CREDENTIALS_FI
+0002d2f0: 4c45 3d7b 636c 6f75 6466 6c61 7265 2e52  LE={cloudflare.R
+0002d300: 325f 4352 4544 454e 5449 414c 535f 5041  2_CREDENTIALS_PA
+0002d310: 5448 7d20 6177 7320 7333 2072 6220 7b62  TH} aws s3 rb {b
+0002d320: 7563 6b65 745f 7572 697d 202d 2d66 6f72  ucket_uri} --for
+0002d330: 6365 202d 2d65 6e64 706f 696e 7420 7b65  ce --endpoint {e
+0002d340: 6e64 706f 696e 745f 7572 6c7d 202d 2d70  ndpoint_url} --p
+0002d350: 726f 6669 6c65 3d72 3227 2c0a 2020 2020  rofile=r2',.    
+0002d360: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
+0002d370: 7565 290a 0a20 2020 2040 7079 7465 7374  ue)..    @pytest
+0002d380: 2e66 6978 7475 7265 0a20 2020 2064 6566  .fixture.    def
+0002d390: 2074 6d70 5f69 626d 5f63 6f73 5f62 7563   tmp_ibm_cos_buc
+0002d3a0: 6b65 7428 7365 6c66 2c20 746d 705f 6275  ket(self, tmp_bu
+0002d3b0: 636b 6574 5f6e 616d 6529 3a0a 2020 2020  cket_name):.    
+0002d3c0: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
+0002d3d0: 7465 6d70 6f72 6172 7920 6275 636b 6574  temporary bucket
+0002d3e0: 2075 7369 6e67 2049 424d 2043 4f53 2041   using IBM COS A
+0002d3f0: 5049 0a20 2020 2020 2020 2073 746f 7261  PI.        stora
+0002d400: 6765 5f6f 626a 203d 2073 746f 7261 6765  ge_obj = storage
+0002d410: 5f6c 6962 2e49 424d 436f 7353 746f 7265  _lib.IBMCosStore
+0002d420: 2873 6f75 7263 653d 2222 2c20 6e61 6d65  (source="", name
+0002d430: 3d74 6d70 5f62 7563 6b65 745f 6e61 6d65  =tmp_bucket_name
+0002d440: 290a 2020 2020 2020 2020 7969 656c 6420  ).        yield 
+0002d450: 746d 705f 6275 636b 6574 5f6e 616d 650a  tmp_bucket_name.
+0002d460: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0002d470: 6f62 6a2e 6465 6c65 7465 2829 0a0a 2020  obj.delete()..  
+0002d480: 2020 4070 7974 6573 742e 6669 7874 7572    @pytest.fixtur
+0002d490: 650a 2020 2020 6465 6620 746d 705f 7075  e.    def tmp_pu
+0002d4a0: 626c 6963 5f73 746f 7261 6765 5f6f 626a  blic_storage_obj
+0002d4b0: 2873 656c 662c 2072 6571 7565 7374 293a  (self, request):
+0002d4c0: 0a20 2020 2020 2020 2023 2049 6e69 7469  .        # Initi
+0002d4d0: 616c 697a 6573 2061 2073 746f 7261 6765  alizes a storage
+0002d4e0: 206f 626a 6563 7420 7769 7468 2061 2070   object with a p
+0002d4f0: 7562 6c69 6320 6275 636b 6574 0a20 2020  ublic bucket.   
+0002d500: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+0002d510: 203d 2073 746f 7261 6765 5f6c 6962 2e53   = storage_lib.S
+0002d520: 746f 7261 6765 2873 6f75 7263 653d 7265  torage(source=re
+0002d530: 7175 6573 742e 7061 7261 6d29 0a20 2020  quest.param).   
+0002d540: 2020 2020 2079 6965 6c64 2073 746f 7261       yield stora
+0002d550: 6765 5f6f 626a 0a20 2020 2020 2020 2023  ge_obj.        #
+0002d560: 2054 6869 7320 646f 6573 206e 6f74 2072   This does not r
+0002d570: 6571 7569 7265 2061 6e79 2064 656c 6574  equire any delet
+0002d580: 696f 6e20 6c6f 6769 6320 6265 6361 7573  ion logic becaus
+0002d590: 6520 6974 2069 7320 6120 7075 626c 6963  e it is a public
+0002d5a0: 2062 7563 6b65 740a 2020 2020 2020 2020   bucket.        
+0002d5b0: 2320 616e 6420 7368 6f75 6c64 206e 6f74  # and should not
+0002d5c0: 2067 6574 2061 6464 6564 2074 6f20 676c   get added to gl
+0002d5d0: 6f62 616c 5f75 7365 725f 7374 6174 652e  obal_user_state.
+0002d5e0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0002d5f0: 726b 2e6e 6f5f 666c 7569 6473 7461 636b  rk.no_fluidstack
+0002d600: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0002d610: 6b2e 7061 7261 6d65 7472 697a 6528 2773  k.parametrize('s
+0002d620: 746f 7265 5f74 7970 6527 2c20 5b0a 2020  tore_type', [.  
+0002d630: 2020 2020 2020 7374 6f72 6167 655f 6c69        storage_li
+0002d640: 622e 5374 6f72 6554 7970 652e 5333 2c20  b.StoreType.S3, 
+0002d650: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002d660: 6554 7970 652e 4743 532c 0a20 2020 2020  eType.GCS,.     
+0002d670: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+0002d680: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002d690: 6554 7970 652e 4942 4d2c 206d 6172 6b73  eType.IBM, marks
+0002d6a0: 3d70 7974 6573 742e 6d61 726b 2e69 626d  =pytest.mark.ibm
+0002d6b0: 292c 0a20 2020 2020 2020 2070 7974 6573  ),.        pytes
+0002d6c0: 742e 7061 7261 6d28 7374 6f72 6167 655f  t.param(storage_
+0002d6d0: 6c69 622e 5374 6f72 6554 7970 652e 5232  lib.StoreType.R2
+0002d6e0: 2c20 6d61 726b 733d 7079 7465 7374 2e6d  , marks=pytest.m
+0002d6f0: 6172 6b2e 636c 6f75 6466 6c61 7265 290a  ark.cloudflare).
+0002d700: 2020 2020 5d29 0a20 2020 2064 6566 2074      ]).    def t
+0002d710: 6573 745f 6e65 775f 6275 636b 6574 5f63  est_new_bucket_c
+0002d720: 7265 6174 696f 6e5f 616e 645f 6465 6c65  reation_and_dele
+0002d730: 7469 6f6e 2873 656c 662c 2074 6d70 5f6c  tion(self, tmp_l
+0002d740: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+0002d750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d780: 7374 6f72 655f 7479 7065 293a 0a20 2020  store_type):.   
+0002d790: 2020 2020 2023 2043 7265 6174 6573 2061       # Creates a
+0002d7a0: 206e 6577 2062 7563 6b65 7420 7769 7468   new bucket with
+0002d7b0: 2061 206c 6f63 616c 2073 6f75 7263 652c   a local source,
+0002d7c0: 2075 706c 6f61 6473 2066 696c 6573 2074   uploads files t
+0002d7d0: 6f20 6974 0a20 2020 2020 2020 2023 2061  o it.        # a
+0002d7e0: 6e64 2064 656c 6574 6573 2069 742e 0a20  nd deletes it.. 
+0002d7f0: 2020 2020 2020 2074 6d70 5f6c 6f63 616c         tmp_local
+0002d800: 5f73 746f 7261 6765 5f6f 626a 2e61 6464  _storage_obj.add
+0002d810: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
+0002d820: 6529 0a0a 2020 2020 2020 2020 2320 5275  e)..        # Ru
+0002d830: 6e20 736b 7920 7374 6f72 6167 6520 6c73  n sky storage ls
+0002d840: 2074 6f20 6368 6563 6b20 6966 2073 746f   to check if sto
+0002d850: 7261 6765 206f 626a 6563 7420 6578 6973  rage object exis
+0002d860: 7473 2069 6e20 7468 6520 6f75 7470 7574  ts in the output
+0002d870: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+0002d880: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0002d890: 6f75 7470 7574 285b 2773 6b79 272c 2027  output(['sky', '
+0002d8a0: 7374 6f72 6167 6527 2c20 276c 7327 5d29  storage', 'ls'])
+0002d8b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0002d8c0: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
+0002d8d0: 655f 6f62 6a2e 6e61 6d65 2069 6e20 6f75  e_obj.name in ou
+0002d8e0: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+0002d8f0: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
+0002d900: 2073 6b79 2073 746f 7261 6765 2064 656c   sky storage del
+0002d910: 6574 6520 746f 2064 656c 6574 6520 7468  ete to delete th
+0002d920: 6520 7374 6f72 6167 6520 6f62 6a65 6374  e storage object
+0002d930: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+0002d940: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0002d950: 280a 2020 2020 2020 2020 2020 2020 5b27  (.            ['
+0002d960: 736b 7927 2c20 2773 746f 7261 6765 272c  sky', 'storage',
+0002d970: 2027 6465 6c65 7465 272c 2074 6d70 5f6c   'delete', tmp_l
+0002d980: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+0002d990: 2e6e 616d 652c 2027 2d2d 7965 7327 5d29  .name, '--yes'])
+0002d9a0: 0a0a 2020 2020 2020 2020 2320 5275 6e20  ..        # Run 
+0002d9b0: 736b 7920 7374 6f72 6167 6520 6c73 2074  sky storage ls t
+0002d9c0: 6f20 6368 6563 6b20 6966 2073 746f 7261  o check if stora
+0002d9d0: 6765 206f 626a 6563 7420 6973 2064 656c  ge object is del
+0002d9e0: 6574 6564 0a20 2020 2020 2020 206f 7574  eted.        out
+0002d9f0: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0002da00: 6563 6b5f 6f75 7470 7574 285b 2773 6b79  eck_output(['sky
+0002da10: 272c 2027 7374 6f72 6167 6527 2c20 276c  ', 'storage', 'l
+0002da20: 7327 5d29 0a20 2020 2020 2020 2061 7373  s']).        ass
+0002da30: 6572 7420 746d 705f 6c6f 6361 6c5f 7374  ert tmp_local_st
+0002da40: 6f72 6167 655f 6f62 6a2e 6e61 6d65 206e  orage_obj.name n
+0002da50: 6f74 2069 6e20 6f75 742e 6465 636f 6465  ot in out.decode
+0002da60: 2827 7574 662d 3827 290a 0a20 2020 2040  ('utf-8')..    @
+0002da70: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f66  pytest.mark.no_f
+0002da80: 6c75 6964 7374 6163 6b0a 2020 2020 4070  luidstack.    @p
+0002da90: 7974 6573 742e 6d61 726b 2e78 6469 7374  ytest.mark.xdist
+0002daa0: 5f67 726f 7570 2827 6d75 6c74 6970 6c65  _group('multiple
+0002dab0: 5f62 7563 6b65 745f 6465 6c65 7469 6f6e  _bucket_deletion
+0002dac0: 2729 0a20 2020 2040 7079 7465 7374 2e6d  ').    @pytest.m
+0002dad0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+0002dae0: 2773 746f 7265 5f74 7970 6527 2c20 5b0a  'store_type', [.
+0002daf0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0002db00: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
+0002db10: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
+0002db20: 6f72 6554 7970 652e 4743 532c 0a20 2020  oreType.GCS,.   
+0002db30: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
+0002db40: 6d28 7374 6f72 6167 655f 6c69 622e 5374  m(storage_lib.St
+0002db50: 6f72 6554 7970 652e 5232 2c20 6d61 726b  oreType.R2, mark
+0002db60: 733d 7079 7465 7374 2e6d 6172 6b2e 636c  s=pytest.mark.cl
+0002db70: 6f75 6466 6c61 7265 292c 0a20 2020 2020  oudflare),.     
+0002db80: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+0002db90: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002dba0: 6554 7970 652e 4942 4d2c 206d 6172 6b73  eType.IBM, marks
+0002dbb0: 3d70 7974 6573 742e 6d61 726b 2e69 626d  =pytest.mark.ibm
+0002dbc0: 290a 2020 2020 5d29 0a20 2020 2064 6566  ).    ]).    def
+0002dbd0: 2074 6573 745f 6d75 6c74 6970 6c65 5f62   test_multiple_b
+0002dbe0: 7563 6b65 7473 5f63 7265 6174 696f 6e5f  uckets_creation_
+0002dbf0: 616e 645f 6465 6c65 7469 6f6e 280a 2020  and_deletion(.  
+0002dc00: 2020 2020 2020 2020 2020 7365 6c66 2c20            self, 
+0002dc10: 746d 705f 6d75 6c74 6970 6c65 5f73 6372  tmp_multiple_scr
+0002dc20: 6174 6368 5f73 746f 7261 6765 5f6f 626a  atch_storage_obj
+0002dc30: 2c20 7374 6f72 655f 7479 7065 293a 0a20  , store_type):. 
+0002dc40: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+0002dc50: 206d 756c 7469 706c 6520 6e65 7720 6275   multiple new bu
+0002dc60: 636b 6574 7328 3520 6275 636b 6574 7329  ckets(5 buckets)
+0002dc70: 2077 6974 6820 6120 6c6f 6361 6c20 736f   with a local so
+0002dc80: 7572 6365 0a20 2020 2020 2020 2023 2061  urce.        # a
+0002dc90: 6e64 2064 656c 6574 6573 2074 6865 6d2e  nd deletes them.
+0002dca0: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+0002dcb0: 5f6f 626a 5f6e 616d 6520 3d20 5b5d 0a20  _obj_name = []. 
+0002dcc0: 2020 2020 2020 2066 6f72 2073 746f 7265         for store
+0002dcd0: 5f6f 626a 2069 6e20 746d 705f 6d75 6c74  _obj in tmp_mult
+0002dce0: 6970 6c65 5f73 6372 6174 6368 5f73 746f  iple_scratch_sto
+0002dcf0: 7261 6765 5f6f 626a 3a0a 2020 2020 2020  rage_obj:.      
+0002dd00: 2020 2020 2020 7374 6f72 655f 6f62 6a2e        store_obj.
+0002dd10: 6164 645f 7374 6f72 6528 7374 6f72 655f  add_store(store_
+0002dd20: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
+0002dd30: 2020 7374 6f72 6167 655f 6f62 6a5f 6e61    storage_obj_na
+0002dd40: 6d65 2e61 7070 656e 6428 7374 6f72 655f  me.append(store_
+0002dd50: 6f62 6a2e 6e61 6d65 290a 0a20 2020 2020  obj.name)..     
+0002dd60: 2020 2023 2052 756e 2073 6b79 2073 746f     # Run sky sto
+0002dd70: 7261 6765 206c 7320 746f 2063 6865 636b  rage ls to check
+0002dd80: 2069 6620 616c 6c20 7374 6f72 6167 6520   if all storage 
+0002dd90: 6f62 6a65 6374 7320 6578 6973 7473 2069  objects exists i
+0002dda0: 6e20 7468 650a 2020 2020 2020 2020 2320  n the.        # 
+0002ddb0: 6f75 7470 7574 2066 696c 7465 7265 6420  output filtered 
+0002ddc0: 6279 2073 746f 7265 2074 7970 650a 2020  by store type.  
+0002ddd0: 2020 2020 2020 6f75 745f 616c 6c20 3d20        out_all = 
+0002dde0: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
+0002ddf0: 5f6f 7574 7075 7428 5b27 736b 7927 2c20  _output(['sky', 
+0002de00: 2773 746f 7261 6765 272c 2027 6c73 275d  'storage', 'ls']
+0002de10: 290a 2020 2020 2020 2020 6f75 7420 3d20  ).        out = 
+0002de20: 5b0a 2020 2020 2020 2020 2020 2020 6974  [.            it
+0002de30: 656d 2e73 706c 6974 2829 5b30 5d0a 2020  em.split()[0].  
+0002de40: 2020 2020 2020 2020 2020 666f 7220 6974            for it
+0002de50: 656d 2069 6e20 6f75 745f 616c 6c2e 6465  em in out_all.de
+0002de60: 636f 6465 2827 7574 662d 3827 292e 7370  code('utf-8').sp
+0002de70: 6c69 746c 696e 6573 2829 0a20 2020 2020  litlines().     
+0002de80: 2020 2020 2020 2069 6620 7374 6f72 655f         if store_
+0002de90: 7479 7065 2e76 616c 7565 2069 6e20 6974  type.value in it
+0002dea0: 656d 0a20 2020 2020 2020 205d 0a20 2020  em.        ].   
+0002deb0: 2020 2020 2061 7373 6572 7420 616c 6c28       assert all(
+0002dec0: 5b69 7465 6d20 696e 206f 7574 2066 6f72  [item in out for
+0002ded0: 2069 7465 6d20 696e 2073 746f 7261 6765   item in storage
+0002dee0: 5f6f 626a 5f6e 616d 655d 290a 0a20 2020  _obj_name])..   
+0002def0: 2020 2020 2023 2052 756e 2073 6b79 2073       # Run sky s
+0002df00: 746f 7261 6765 2064 656c 6574 6520 616c  torage delete al
+0002df10: 6c20 746f 2064 656c 6574 6520 616c 6c20  l to delete all 
+0002df20: 7374 6f72 6167 6520 6f62 6a65 6374 730a  storage objects.
+0002df30: 2020 2020 2020 2020 6465 6c65 7465 5f63          delete_c
+0002df40: 6d64 203d 205b 2773 6b79 272c 2027 7374  md = ['sky', 'st
+0002df50: 6f72 6167 6527 2c20 2764 656c 6574 6527  orage', 'delete'
+0002df60: 2c20 272d 2d79 6573 275d 0a20 2020 2020  , '--yes'].     
+0002df70: 2020 2064 656c 6574 655f 636d 6420 2b3d     delete_cmd +=
+0002df80: 2073 746f 7261 6765 5f6f 626a 5f6e 616d   storage_obj_nam
+0002df90: 650a 2020 2020 2020 2020 7375 6270 726f  e.        subpro
+0002dfa0: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
+0002dfb0: 7428 6465 6c65 7465 5f63 6d64 290a 0a20  t(delete_cmd).. 
+0002dfc0: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
+0002dfd0: 2073 746f 7261 6765 206c 7320 746f 2063   storage ls to c
+0002dfe0: 6865 636b 2069 6620 616c 6c20 7374 6f72  heck if all stor
+0002dff0: 6167 6520 6f62 6a65 6374 7320 6669 6c74  age objects filt
+0002e000: 6572 6564 2062 7920 7374 6f72 650a 2020  ered by store.  
+0002e010: 2020 2020 2020 2320 7479 7065 2061 7265        # type are
+0002e020: 2064 656c 6574 6564 0a20 2020 2020 2020   deleted.       
+0002e030: 206f 7574 5f61 6c6c 203d 2073 7562 7072   out_all = subpr
+0002e040: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+0002e050: 7574 285b 2773 6b79 272c 2027 7374 6f72  ut(['sky', 'stor
+0002e060: 6167 6527 2c20 276c 7327 5d29 0a20 2020  age', 'ls']).   
+0002e070: 2020 2020 206f 7574 203d 205b 0a20 2020       out = [.   
+0002e080: 2020 2020 2020 2020 2069 7465 6d2e 7370           item.sp
+0002e090: 6c69 7428 295b 305d 0a20 2020 2020 2020  lit()[0].       
+0002e0a0: 2020 2020 2066 6f72 2069 7465 6d20 696e       for item in
+0002e0b0: 206f 7574 5f61 6c6c 2e64 6563 6f64 6528   out_all.decode(
+0002e0c0: 2775 7466 2d38 2729 2e73 706c 6974 6c69  'utf-8').splitli
+0002e0d0: 6e65 7328 290a 2020 2020 2020 2020 2020  nes().          
+0002e0e0: 2020 6966 2073 746f 7265 5f74 7970 652e    if store_type.
+0002e0f0: 7661 6c75 6520 696e 2069 7465 6d0a 2020  value in item.  
+0002e100: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0002e110: 6173 7365 7274 2061 6c6c 285b 6974 656d  assert all([item
+0002e120: 206e 6f74 2069 6e20 6f75 7420 666f 7220   not in out for 
+0002e130: 6974 656d 2069 6e20 7374 6f72 6167 655f  item in storage_
+0002e140: 6f62 6a5f 6e61 6d65 5d29 0a0a 2020 2020  obj_name])..    
+0002e150: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0002e160: 666c 7569 6473 7461 636b 0a20 2020 2040  fluidstack.    @
+0002e170: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+0002e180: 6d65 7472 697a 6528 2773 746f 7265 5f74  metrize('store_t
+0002e190: 7970 6527 2c20 5b0a 2020 2020 2020 2020  ype', [.        
+0002e1a0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002e1b0: 6554 7970 652e 5333 2c20 7374 6f72 6167  eType.S3, storag
+0002e1c0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0002e1d0: 4743 532c 0a20 2020 2020 2020 2070 7974  GCS,.        pyt
+0002e1e0: 6573 742e 7061 7261 6d28 7374 6f72 6167  est.param(storag
+0002e1f0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+0002e200: 4942 4d2c 206d 6172 6b73 3d70 7974 6573  IBM, marks=pytes
+0002e210: 742e 6d61 726b 2e69 626d 292c 0a20 2020  t.mark.ibm),.   
+0002e220: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
+0002e230: 6d28 7374 6f72 6167 655f 6c69 622e 5374  m(storage_lib.St
+0002e240: 6f72 6554 7970 652e 5232 2c20 6d61 726b  oreType.R2, mark
+0002e250: 733d 7079 7465 7374 2e6d 6172 6b2e 636c  s=pytest.mark.cl
+0002e260: 6f75 6466 6c61 7265 290a 2020 2020 5d29  oudflare).    ])
+0002e270: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
+0002e280: 6c6f 6164 5f73 6f75 7263 655f 7769 7468  load_source_with
+0002e290: 5f73 7061 6365 7328 7365 6c66 2c20 7374  _spaces(self, st
+0002e2a0: 6f72 655f 7479 7065 2c0a 2020 2020 2020  ore_type,.      
+0002e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e2d0: 2074 6d70 5f6d 756c 7469 706c 655f 6375   tmp_multiple_cu
+0002e2e0: 7374 6f6d 5f73 6f75 7263 655f 7374 6f72  stom_source_stor
+0002e2f0: 6167 655f 6f62 6a29 3a0a 2020 2020 2020  age_obj):.      
+0002e300: 2020 2320 4372 6561 7465 7320 7477 6f20    # Creates two 
+0002e310: 6275 636b 6574 7320 7769 7468 2073 7065  buckets with spe
+0002e320: 6369 6669 6564 206c 6f63 616c 2073 6f75  cified local sou
+0002e330: 7263 6573 0a20 2020 2020 2020 2023 2077  rces.        # w
+0002e340: 6974 6820 7370 6163 6573 2069 6e20 7468  ith spaces in th
+0002e350: 6520 6e61 6d65 0a20 2020 2020 2020 2073  e name.        s
+0002e360: 746f 7261 6765 5f6f 626a 5f6e 616d 6573  torage_obj_names
+0002e370: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+0002e380: 7220 7374 6f72 6167 655f 6f62 6a20 696e  r storage_obj in
+0002e390: 2074 6d70 5f6d 756c 7469 706c 655f 6375   tmp_multiple_cu
+0002e3a0: 7374 6f6d 5f73 6f75 7263 655f 7374 6f72  stom_source_stor
+0002e3b0: 6167 655f 6f62 6a3a 0a20 2020 2020 2020  age_obj:.       
+0002e3c0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+0002e3d0: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
+0002e3e0: 5f74 7970 6529 0a20 2020 2020 2020 2020  _type).         
+0002e3f0: 2020 2073 746f 7261 6765 5f6f 626a 5f6e     storage_obj_n
+0002e400: 616d 6573 2e61 7070 656e 6428 7374 6f72  ames.append(stor
+0002e410: 6167 655f 6f62 6a2e 6e61 6d65 290a 0a20  age_obj.name).. 
+0002e420: 2020 2020 2020 2023 2052 756e 2073 6b79         # Run sky
+0002e430: 2073 746f 7261 6765 206c 7320 746f 2063   storage ls to c
+0002e440: 6865 636b 2069 6620 616c 6c20 7374 6f72  heck if all stor
+0002e450: 6167 6520 6f62 6a65 6374 7320 6578 6973  age objects exis
+0002e460: 7473 2069 6e20 7468 650a 2020 2020 2020  ts in the.      
+0002e470: 2020 2320 6f75 7470 7574 2066 696c 7465    # output filte
+0002e480: 7265 6420 6279 2073 746f 7265 2074 7970  red by store typ
+0002e490: 650a 2020 2020 2020 2020 6f75 745f 616c  e.        out_al
+0002e4a0: 6c20 3d20 7375 6270 726f 6365 7373 2e63  l = subprocess.c
+0002e4b0: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
+0002e4c0: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
+0002e4d0: 6c73 275d 290a 2020 2020 2020 2020 6f75  ls']).        ou
+0002e4e0: 7420 3d20 5b0a 2020 2020 2020 2020 2020  t = [.          
+0002e4f0: 2020 6974 656d 2e73 706c 6974 2829 5b30    item.split()[0
+0002e500: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+0002e510: 7220 6974 656d 2069 6e20 6f75 745f 616c  r item in out_al
+0002e520: 6c2e 6465 636f 6465 2827 7574 662d 3827  l.decode('utf-8'
+0002e530: 292e 7370 6c69 746c 696e 6573 2829 0a20  ).splitlines(). 
+0002e540: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+0002e550: 6f72 655f 7479 7065 2e76 616c 7565 2069  ore_type.value i
+0002e560: 6e20 6974 656d 0a20 2020 2020 2020 205d  n item.        ]
+0002e570: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0002e580: 616c 6c28 5b69 7465 6d20 696e 206f 7574  all([item in out
+0002e590: 2066 6f72 2069 7465 6d20 696e 2073 746f   for item in sto
+0002e5a0: 7261 6765 5f6f 626a 5f6e 616d 6573 5d29  rage_obj_names])
+0002e5b0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
+0002e5c0: 726b 2e6e 6f5f 666c 7569 6473 7461 636b  rk.no_fluidstack
+0002e5d0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0002e5e0: 6b2e 7061 7261 6d65 7472 697a 6528 2773  k.parametrize('s
+0002e5f0: 746f 7265 5f74 7970 6527 2c20 5b0a 2020  tore_type', [.  
+0002e600: 2020 2020 2020 7374 6f72 6167 655f 6c69        storage_li
+0002e610: 622e 5374 6f72 6554 7970 652e 5333 2c20  b.StoreType.S3, 
+0002e620: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002e630: 6554 7970 652e 4743 532c 0a20 2020 2020  eType.GCS,.     
+0002e640: 2020 2070 7974 6573 742e 7061 7261 6d28     pytest.param(
+0002e650: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+0002e660: 6554 7970 652e 4942 4d2c 206d 6172 6b73  eType.IBM, marks
+0002e670: 3d70 7974 6573 742e 6d61 726b 2e69 626d  =pytest.mark.ibm
+0002e680: 292c 0a20 2020 2020 2020 2070 7974 6573  ),.        pytes
+0002e690: 742e 7061 7261 6d28 7374 6f72 6167 655f  t.param(storage_
+0002e6a0: 6c69 622e 5374 6f72 6554 7970 652e 5232  lib.StoreType.R2
+0002e6b0: 2c20 6d61 726b 733d 7079 7465 7374 2e6d  , marks=pytest.m
+0002e6c0: 6172 6b2e 636c 6f75 6466 6c61 7265 290a  ark.cloudflare).
+0002e6d0: 2020 2020 5d29 0a20 2020 2064 6566 2074      ]).    def t
+0002e6e0: 6573 745f 6275 636b 6574 5f65 7874 6572  est_bucket_exter
+0002e6f0: 6e61 6c5f 6465 6c65 7469 6f6e 2873 656c  nal_deletion(sel
+0002e700: 662c 2074 6d70 5f73 6372 6174 6368 5f73  f, tmp_scratch_s
+0002e710: 746f 7261 6765 5f6f 626a 2c0a 2020 2020  torage_obj,.    
+0002e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002e740: 2020 7374 6f72 655f 7479 7065 293a 0a20    store_type):. 
+0002e750: 2020 2020 2020 2023 2043 7265 6174 6573         # Creates
+0002e760: 2061 2062 7563 6b65 742c 2064 656c 6574   a bucket, delet
+0002e770: 6573 2069 7420 6578 7465 726e 616c 6c79  es it externally
+0002e780: 2075 7369 6e67 2063 6c6f 7564 2063 6c69   using cloud cli
+0002e790: 2063 6f6d 6d61 6e64 730a 2020 2020 2020   commands.      
+0002e7a0: 2020 2320 616e 6420 7468 656e 2074 7269    # and then tri
+0002e7b0: 6573 2074 6f20 6465 6c65 7465 2069 7420  es to delete it 
+0002e7c0: 7573 696e 6720 736b 7920 7374 6f72 6167  using sky storag
+0002e7d0: 6520 6465 6c65 7465 2e0a 2020 2020 2020  e delete..      
+0002e7e0: 2020 746d 705f 7363 7261 7463 685f 7374    tmp_scratch_st
+0002e7f0: 6f72 6167 655f 6f62 6a2e 6164 645f 7374  orage_obj.add_st
+0002e800: 6f72 6528 7374 6f72 655f 7479 7065 290a  ore(store_type).
+0002e810: 0a20 2020 2020 2020 2023 2052 756e 2073  .        # Run s
+0002e820: 6b79 2073 746f 7261 6765 206c 7320 746f  ky storage ls to
+0002e830: 2063 6865 636b 2069 6620 7374 6f72 6167   check if storag
+0002e840: 6520 6f62 6a65 6374 2065 7869 7374 7320  e object exists 
+0002e850: 696e 2074 6865 206f 7574 7075 740a 2020  in the output.  
+0002e860: 2020 2020 2020 6f75 7420 3d20 7375 6270        out = subp
+0002e870: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+0002e880: 7075 7428 5b27 736b 7927 2c20 2773 746f  put(['sky', 'sto
+0002e890: 7261 6765 272c 2027 6c73 275d 290a 2020  rage', 'ls']).  
+0002e8a0: 2020 2020 2020 6173 7365 7274 2074 6d70        assert tmp
+0002e8b0: 5f73 6372 6174 6368 5f73 746f 7261 6765  _scratch_storage
+0002e8c0: 5f6f 626a 2e6e 616d 6520 696e 206f 7574  _obj.name in out
+0002e8d0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+0002e8e0: 0a0a 2020 2020 2020 2020 2320 4465 6c65  ..        # Dele
+0002e8f0: 7465 2062 7563 6b65 7420 6578 7465 726e  te bucket extern
+0002e900: 616c 6c79 0a20 2020 2020 2020 2063 6d64  ally.        cmd
+0002e910: 203d 2073 656c 662e 636c 695f 6465 6c65   = self.cli_dele
+0002e920: 7465 5f63 6d64 2873 746f 7265 5f74 7970  te_cmd(store_typ
+0002e930: 652c 2074 6d70 5f73 6372 6174 6368 5f73  e, tmp_scratch_s
+0002e940: 746f 7261 6765 5f6f 626a 2e6e 616d 6529  torage_obj.name)
+0002e950: 0a20 2020 2020 2020 2073 7562 7072 6f63  .        subproc
+0002e960: 6573 732e 6368 6563 6b5f 6f75 7470 7574  ess.check_output
+0002e970: 2863 6d64 2c20 7368 656c 6c3d 5472 7565  (cmd, shell=True
+0002e980: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
+0002e990: 2073 6b79 2073 746f 7261 6765 2064 656c   sky storage del
+0002e9a0: 6574 6520 746f 2064 656c 6574 6520 7468  ete to delete th
+0002e9b0: 6520 7374 6f72 6167 6520 6f62 6a65 6374  e storage object
+0002e9c0: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+0002e9d0: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+0002e9e0: 6f75 7470 7574 280a 2020 2020 2020 2020  output(.        
+0002e9f0: 2020 2020 5b27 736b 7927 2c20 2773 746f      ['sky', 'sto
+0002ea00: 7261 6765 272c 2027 6465 6c65 7465 272c  rage', 'delete',
+0002ea10: 2074 6d70 5f73 6372 6174 6368 5f73 746f   tmp_scratch_sto
+0002ea20: 7261 6765 5f6f 626a 2e6e 616d 652c 2027  rage_obj.name, '
+0002ea30: 2d2d 7965 7327 5d29 0a20 2020 2020 2020  --yes']).       
+0002ea40: 2023 204d 616b 6520 7375 7265 2062 7563   # Make sure buc
+0002ea50: 6b65 7420 7761 7320 6e6f 7420 6372 6561  ket was not crea
+0002ea60: 7465 6420 6475 7269 6e67 2064 656c 6574  ted during delet
+0002ea70: 696f 6e20 2873 6565 2069 7373 7565 2023  ion (see issue #
+0002ea80: 3133 3232 290a 2020 2020 2020 2020 6173  1322).        as
+0002ea90: 7365 7274 2027 6372 6561 7465 6427 206e  sert 'created' n
+0002eaa0: 6f74 2069 6e20 6f75 742e 6465 636f 6465  ot in out.decode
+0002eab0: 2827 7574 662d 3827 292e 6c6f 7765 7228  ('utf-8').lower(
+0002eac0: 290a 0a20 2020 2020 2020 2023 2052 756e  )..        # Run
+0002ead0: 2073 6b79 2073 746f 7261 6765 206c 7320   sky storage ls 
+0002eae0: 746f 2063 6865 636b 2069 6620 7374 6f72  to check if stor
+0002eaf0: 6167 6520 6f62 6a65 6374 2069 7320 6465  age object is de
+0002eb00: 6c65 7465 640a 2020 2020 2020 2020 6f75  leted.        ou
+0002eb10: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
+0002eb20: 6865 636b 5f6f 7574 7075 7428 5b27 736b  heck_output(['sk
+0002eb30: 7927 2c20 2773 746f 7261 6765 272c 2027  y', 'storage', '
+0002eb40: 6c73 275d 290a 2020 2020 2020 2020 6173  ls']).        as
+0002eb50: 7365 7274 2074 6d70 5f73 6372 6174 6368  sert tmp_scratch
+0002eb60: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+0002eb70: 6520 6e6f 7420 696e 206f 7574 2e64 6563  e not in out.dec
+0002eb80: 6f64 6528 2775 7466 2d38 2729 0a0a 2020  ode('utf-8')..  
+0002eb90: 2020 4070 7974 6573 742e 6d61 726b 2e6e    @pytest.mark.n
+0002eba0: 6f5f 666c 7569 6473 7461 636b 0a20 2020  o_fluidstack.   
+0002ebb0: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
+0002ebc0: 7261 6d65 7472 697a 6528 2773 746f 7265  rametrize('store
+0002ebd0: 5f74 7970 6527 2c20 5b0a 2020 2020 2020  _type', [.      
+0002ebe0: 2020 7374 6f72 6167 655f 6c69 622e 5374    storage_lib.St
+0002ebf0: 6f72 6554 7970 652e 5333 2c20 7374 6f72  oreType.S3, stor
+0002ec00: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002ec10: 652e 4743 532c 0a20 2020 2020 2020 2070  e.GCS,.        p
+0002ec20: 7974 6573 742e 7061 7261 6d28 7374 6f72  ytest.param(stor
+0002ec30: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002ec40: 652e 4942 4d2c 206d 6172 6b73 3d70 7974  e.IBM, marks=pyt
+0002ec50: 6573 742e 6d61 726b 2e69 626d 292c 0a20  est.mark.ibm),. 
+0002ec60: 2020 2020 2020 2070 7974 6573 742e 7061         pytest.pa
+0002ec70: 7261 6d28 7374 6f72 6167 655f 6c69 622e  ram(storage_lib.
+0002ec80: 5374 6f72 6554 7970 652e 5232 2c20 6d61  StoreType.R2, ma
+0002ec90: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
+0002eca0: 636c 6f75 6466 6c61 7265 290a 2020 2020  cloudflare).    
+0002ecb0: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
+0002ecc0: 6275 636b 6574 5f62 756c 6b5f 6465 6c65  bucket_bulk_dele
+0002ecd0: 7469 6f6e 2873 656c 662c 2073 746f 7265  tion(self, store
+0002ece0: 5f74 7970 652c 2074 6d70 5f62 756c 6b5f  _type, tmp_bulk_
+0002ecf0: 6465 6c5f 7374 6f72 6167 655f 6f62 6a29  del_storage_obj)
+0002ed00: 3a0a 2020 2020 2020 2020 2320 4372 6561  :.        # Crea
+0002ed10: 7465 7320 6120 7465 6d70 2066 6f6c 6465  tes a temp folde
+0002ed20: 7220 7769 7468 206f 7665 7220 3235 3620  r with over 256 
+0002ed30: 6669 6c65 7320 616e 6420 666f 6c64 6572  files and folder
+0002ed40: 732c 2075 706c 6f61 640a 2020 2020 2020  s, upload.      
+0002ed50: 2020 2320 6669 6c65 7320 616e 6420 666f    # files and fo
+0002ed60: 6c64 6572 7320 746f 2061 206e 6577 2062  lders to a new b
+0002ed70: 7563 6b65 742c 2074 6865 6e20 6465 6c65  ucket, then dele
+0002ed80: 7465 2062 7563 6b65 742e 0a20 2020 2020  te bucket..     
+0002ed90: 2020 2074 6d70 5f62 756c 6b5f 6465 6c5f     tmp_bulk_del_
+0002eda0: 7374 6f72 6167 655f 6f62 6a2e 6164 645f  storage_obj.add_
+0002edb0: 7374 6f72 6528 7374 6f72 655f 7479 7065  store(store_type
+0002edc0: 290a 0a20 2020 2020 2020 2073 7562 7072  )..        subpr
+0002edd0: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+0002ede0: 7574 285b 0a20 2020 2020 2020 2020 2020  ut([.           
+0002edf0: 2027 736b 7927 2c20 2773 746f 7261 6765   'sky', 'storage
+0002ee00: 272c 2027 6465 6c65 7465 272c 2074 6d70  ', 'delete', tmp
+0002ee10: 5f62 756c 6b5f 6465 6c5f 7374 6f72 6167  _bulk_del_storag
+0002ee20: 655f 6f62 6a2e 6e61 6d65 2c20 272d 2d79  e_obj.name, '--y
+0002ee30: 6573 270a 2020 2020 2020 2020 5d29 0a0a  es'.        ])..
+0002ee40: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+0002ee50: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+0002ee60: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
+0002ee70: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
+0002ee80: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
+0002ee90: 7420 746d 705f 6275 6c6b 5f64 656c 5f73  t tmp_bulk_del_s
+0002eea0: 746f 7261 6765 5f6f 626a 2e6e 616d 6520  torage_obj.name 
+0002eeb0: 6e6f 7420 696e 206f 7574 7075 742e 6465  not in output.de
+0002eec0: 636f 6465 2827 7574 662d 3827 290a 0a20  code('utf-8').. 
+0002eed0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+0002eee0: 6e6f 5f66 6c75 6964 7374 6163 6b0a 2020  no_fluidstack.  
+0002eef0: 2020 4070 7974 6573 742e 6d61 726b 2e70    @pytest.mark.p
+0002ef00: 6172 616d 6574 7269 7a65 280a 2020 2020  arametrize(.    
+0002ef10: 2020 2020 2774 6d70 5f70 7562 6c69 635f      'tmp_public_
+0002ef20: 7374 6f72 6167 655f 6f62 6a2c 2073 746f  storage_obj, sto
+0002ef30: 7265 5f74 7970 6527 2c0a 2020 2020 2020  re_type',.      
+0002ef40: 2020 5b28 2773 333a 2f2f 7463 6761 2d32    [('s3://tcga-2
+0002ef50: 2d6f 7065 6e27 2c20 7374 6f72 6167 655f  -open', storage_
+0002ef60: 6c69 622e 5374 6f72 6554 7970 652e 5333  lib.StoreType.S3
+0002ef70: 292c 0a20 2020 2020 2020 2020 2827 7333  ),.         ('s3
+0002ef80: 3a2f 2f64 6967 6974 616c 636f 7270 6f72  ://digitalcorpor
+0002ef90: 6127 2c20 7374 6f72 6167 655f 6c69 622e  a', storage_lib.
+0002efa0: 5374 6f72 6554 7970 652e 5333 292c 0a20  StoreType.S3),. 
+0002efb0: 2020 2020 2020 2020 2827 6773 3a2f 2f67          ('gs://g
+0002efc0: 6370 2d70 7562 6c69 632d 6461 7461 2d73  cp-public-data-s
+0002efd0: 656e 7469 6e65 6c2d 3227 2c20 7374 6f72  entinel-2', stor
+0002efe0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+0002eff0: 652e 4743 5329 5d2c 0a20 2020 2020 2020  e.GCS)],.       
+0002f000: 2069 6e64 6972 6563 743d 5b27 746d 705f   indirect=['tmp_
+0002f010: 7075 626c 6963 5f73 746f 7261 6765 5f6f  public_storage_o
+0002f020: 626a 275d 290a 2020 2020 6465 6620 7465  bj']).    def te
+0002f030: 7374 5f70 7562 6c69 635f 6275 636b 6574  st_public_bucket
+0002f040: 2873 656c 662c 2074 6d70 5f70 7562 6c69  (self, tmp_publi
+0002f050: 635f 7374 6f72 6167 655f 6f62 6a2c 2073  c_storage_obj, s
+0002f060: 746f 7265 5f74 7970 6529 3a0a 2020 2020  tore_type):.    
+0002f070: 2020 2020 2320 4372 6561 7465 7320 6120      # Creates a 
+0002f080: 6e65 7720 6275 636b 6574 2077 6974 6820  new bucket with 
+0002f090: 6120 7075 626c 6963 2073 6f75 7263 6520  a public source 
+0002f0a0: 616e 6420 7665 7269 6669 6573 2074 6861  and verifies tha
+0002f0b0: 7420 6974 2069 7320 6e6f 740a 2020 2020  t it is not.    
+0002f0c0: 2020 2020 2320 6164 6465 6420 746f 2067      # added to g
+0002f0d0: 6c6f 6261 6c5f 7573 6572 5f73 7461 7465  lobal_user_state
+0002f0e0: 2e0a 2020 2020 2020 2020 746d 705f 7075  ..        tmp_pu
+0002f0f0: 626c 6963 5f73 746f 7261 6765 5f6f 626a  blic_storage_obj
+0002f100: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
+0002f110: 5f74 7970 6529 0a0a 2020 2020 2020 2020  _type)..        
+0002f120: 2320 5275 6e20 736b 7920 7374 6f72 6167  # Run sky storag
+0002f130: 6520 6c73 2074 6f20 6368 6563 6b20 6966  e ls to check if
+0002f140: 2073 746f 7261 6765 206f 626a 6563 7420   storage object 
+0002f150: 6578 6973 7473 2069 6e20 7468 6520 6f75  exists in the ou
+0002f160: 7470 7574 0a20 2020 2020 2020 206f 7574  tput.        out
+0002f170: 203d 2073 7562 7072 6f63 6573 732e 6368   = subprocess.ch
+0002f180: 6563 6b5f 6f75 7470 7574 285b 2773 6b79  eck_output(['sky
+0002f190: 272c 2027 7374 6f72 6167 6527 2c20 276c  ', 'storage', 'l
+0002f1a0: 7327 5d29 0a20 2020 2020 2020 2061 7373  s']).        ass
+0002f1b0: 6572 7420 746d 705f 7075 626c 6963 5f73  ert tmp_public_s
+0002f1c0: 746f 7261 6765 5f6f 626a 2e6e 616d 6520  torage_obj.name 
+0002f1d0: 6e6f 7420 696e 206f 7574 2e64 6563 6f64  not in out.decod
+0002f1e0: 6528 2775 7466 2d38 2729 0a0a 2020 2020  e('utf-8')..    
+0002f1f0: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+0002f200: 666c 7569 6473 7461 636b 0a20 2020 2040  fluidstack.    @
+0002f210: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
+0002f220: 6d65 7472 697a 6528 276e 6f6e 6578 6973  metrize('nonexis
+0002f230: 745f 6275 636b 6574 5f75 726c 272c 205b  t_bucket_url', [
+0002f240: 0a20 2020 2020 2020 2027 7333 3a2f 2f7b  .        's3://{
+0002f250: 7261 6e64 6f6d 5f6e 616d 657d 272c 2027  random_name}', '
+0002f260: 6773 3a2f 2f7b 7261 6e64 6f6d 5f6e 616d  gs://{random_nam
+0002f270: 657d 272c 0a20 2020 2020 2020 2070 7974  e}',.        pyt
+0002f280: 6573 742e 7061 7261 6d28 2763 6f73 3a2f  est.param('cos:/
+0002f290: 2f75 732d 6561 7374 2f7b 7261 6e64 6f6d  /us-east/{random
+0002f2a0: 5f6e 616d 657d 272c 206d 6172 6b73 3d70  _name}', marks=p
+0002f2b0: 7974 6573 742e 6d61 726b 2e69 626d 292c  ytest.mark.ibm),
+0002f2c0: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
+0002f2d0: 7061 7261 6d28 2772 323a 2f2f 7b72 616e  param('r2://{ran
+0002f2e0: 646f 6d5f 6e61 6d65 7d27 2c20 6d61 726b  dom_name}', mark
+0002f2f0: 733d 7079 7465 7374 2e6d 6172 6b2e 636c  s=pytest.mark.cl
+0002f300: 6f75 6466 6c61 7265 290a 2020 2020 5d29  oudflare).    ])
+0002f310: 0a20 2020 2064 6566 2074 6573 745f 6e6f  .    def test_no
+0002f320: 6e65 7869 7374 656e 745f 6275 636b 6574  nexistent_bucket
+0002f330: 2873 656c 662c 206e 6f6e 6578 6973 745f  (self, nonexist_
+0002f340: 6275 636b 6574 5f75 726c 293a 0a20 2020  bucket_url):.   
+0002f350: 2020 2020 2023 2041 7474 656d 7074 7320       # Attempts 
+0002f360: 746f 2063 7265 6174 6520 6665 7463 6820  to create fetch 
+0002f370: 6120 7374 726f 6167 6520 7769 7468 2061  a stroage with a
+0002f380: 206e 6f6e 2d65 7869 7374 656e 7420 736f   non-existent so
+0002f390: 7572 6365 2e0a 2020 2020 2020 2020 2320  urce..        # 
+0002f3a0: 4765 6e65 7261 7465 2061 2072 616e 646f  Generate a rando
+0002f3b0: 6d20 6275 636b 6574 206e 616d 6520 616e  m bucket name an
+0002f3c0: 6420 7665 7269 6679 2069 7420 646f 6573  d verify it does
+0002f3d0: 6e27 7420 6578 6973 743a 0a20 2020 2020  n't exist:.     
+0002f3e0: 2020 2072 6574 7279 5f63 6f75 6e74 203d     retry_count =
+0002f3f0: 2030 0a20 2020 2020 2020 2077 6869 6c65   0.        while
+0002f400: 2054 7275 653a 0a20 2020 2020 2020 2020   True:.         
+0002f410: 2020 206e 6f6e 6578 6973 745f 6275 636b     nonexist_buck
+0002f420: 6574 5f6e 616d 6520 3d20 7374 7228 7575  et_name = str(uu
+0002f430: 6964 2e75 7569 6434 2829 290a 2020 2020  id.uuid4()).    
+0002f440: 2020 2020 2020 2020 6966 206e 6f6e 6578          if nonex
+0002f450: 6973 745f 6275 636b 6574 5f75 726c 2e73  ist_bucket_url.s
+0002f460: 7461 7274 7377 6974 6828 2773 3327 293a  tartswith('s3'):
+0002f470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002f480: 2063 6f6d 6d61 6e64 203d 2066 2761 7773   command = f'aws
+0002f490: 2073 3361 7069 2068 6561 642d 6275 636b   s3api head-buck
+0002f4a0: 6574 202d 2d62 7563 6b65 7420 7b6e 6f6e  et --bucket {non
+0002f4b0: 6578 6973 745f 6275 636b 6574 5f6e 616d  exist_bucket_nam
+0002f4c0: 657d 270a 2020 2020 2020 2020 2020 2020  e}'.            
+0002f4d0: 2020 2020 6578 7065 6374 6564 5f6f 7574      expected_out
+0002f4e0: 7075 7420 3d20 2734 3034 270a 2020 2020  put = '404'.    
+0002f4f0: 2020 2020 2020 2020 656c 6966 206e 6f6e          elif non
+0002f500: 6578 6973 745f 6275 636b 6574 5f75 726c  exist_bucket_url
+0002f510: 2e73 7461 7274 7377 6974 6828 2767 7327  .startswith('gs'
+0002f520: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002f530: 2020 2063 6f6d 6d61 6e64 203d 2066 2767     command = f'g
+0002f540: 7375 7469 6c20 6c73 207b 6e6f 6e65 7869  sutil ls {nonexi
+0002f550: 7374 5f62 7563 6b65 745f 7572 6c2e 666f  st_bucket_url.fo
+0002f560: 726d 6174 2872 616e 646f 6d5f 6e61 6d65  rmat(random_name
+0002f570: 3d6e 6f6e 6578 6973 745f 6275 636b 6574  =nonexist_bucket
+0002f580: 5f6e 616d 6529 7d27 0a20 2020 2020 2020  _name)}'.       
+0002f590: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
+0002f5a0: 645f 6f75 7470 7574 203d 2027 4275 636b  d_output = 'Buck
+0002f5b0: 6574 4e6f 7446 6f75 6e64 4578 6365 7074  etNotFoundExcept
+0002f5c0: 696f 6e27 0a20 2020 2020 2020 2020 2020  ion'.           
+0002f5d0: 2065 6c69 6620 6e6f 6e65 7869 7374 5f62   elif nonexist_b
+0002f5e0: 7563 6b65 745f 7572 6c2e 7374 6172 7473  ucket_url.starts
+0002f5f0: 7769 7468 2827 7232 2729 3a0a 2020 2020  with('r2'):.    
+0002f600: 2020 2020 2020 2020 2020 2020 656e 6470              endp
+0002f610: 6f69 6e74 5f75 726c 203d 2063 6c6f 7564  oint_url = cloud
+0002f620: 666c 6172 652e 6372 6561 7465 5f65 6e64  flare.create_end
+0002f630: 706f 696e 7428 290a 2020 2020 2020 2020  point().        
+0002f640: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+0002f650: 3d20 6627 4157 535f 5348 4152 4544 5f43  = f'AWS_SHARED_C
+0002f660: 5245 4445 4e54 4941 4c53 5f46 494c 453d  REDENTIALS_FILE=
+0002f670: 7b63 6c6f 7564 666c 6172 652e 5232 5f43  {cloudflare.R2_C
+0002f680: 5245 4445 4e54 4941 4c53 5f50 4154 487d  REDENTIALS_PATH}
+0002f690: 2061 7773 2073 3361 7069 2068 6561 642d   aws s3api head-
+0002f6a0: 6275 636b 6574 202d 2d62 7563 6b65 7420  bucket --bucket 
+0002f6b0: 7b6e 6f6e 6578 6973 745f 6275 636b 6574  {nonexist_bucket
+0002f6c0: 5f6e 616d 657d 202d 2d65 6e64 706f 696e  _name} --endpoin
+0002f6d0: 7420 7b65 6e64 706f 696e 745f 7572 6c7d  t {endpoint_url}
+0002f6e0: 202d 2d70 726f 6669 6c65 3d72 3227 0a20   --profile=r2'. 
+0002f6f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0002f700: 7870 6563 7465 645f 6f75 7470 7574 203d  xpected_output =
+0002f710: 2027 3430 3427 0a20 2020 2020 2020 2020   '404'.         
+0002f720: 2020 2065 6c69 6620 6e6f 6e65 7869 7374     elif nonexist
+0002f730: 5f62 7563 6b65 745f 7572 6c2e 7374 6172  _bucket_url.star
+0002f740: 7473 7769 7468 2827 636f 7327 293a 0a20  tswith('cos'):. 
+0002f750: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0002f760: 2055 7369 6e67 2041 5049 2063 616c 6c73   Using API calls
+0002f770: 2c20 7369 6e63 6520 7573 696e 6720 7263  , since using rc
+0002f780: 6c6f 6e65 2072 6571 7569 7265 7320 6120  lone requires a 
+0002f790: 7072 6f66 696c 6527 7320 6e61 6d65 0a20  profile's name. 
+0002f7a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0002f7b0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0002f7c0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+0002f7d0: 5f6f 7574 7075 7420 3d20 636f 6d6d 616e  _output = comman
+0002f7e0: 6420 3d20 2265 6368 6f22 2020 2320 6176  d = "echo"  # av
+0002f7f0: 6f69 6420 756e 7265 6c61 7465 6420 6578  oid unrelated ex
+0002f800: 6365 7074 696f 6e20 696e 2063 6173 6520  ception in case 
+0002f810: 6f66 2066 6169 6c75 7265 2e0a 2020 2020  of failure..    
+0002f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f830: 6275 636b 6574 5f6e 616d 6520 3d20 7572  bucket_name = ur
+0002f840: 6c6c 6962 2e70 6172 7365 2e75 726c 7370  llib.parse.urlsp
+0002f850: 6c69 7428 0a20 2020 2020 2020 2020 2020  lit(.           
+0002f860: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+0002f870: 6578 6973 745f 6275 636b 6574 5f75 726c  exist_bucket_url
+0002f880: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+0002f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f8a0: 2020 2020 2072 616e 646f 6d5f 6e61 6d65       random_name
+0002f8b0: 3d6e 6f6e 6578 6973 745f 6275 636b 6574  =nonexist_bucket
+0002f8c0: 5f6e 616d 6529 292e 7061 7468 2e73 7472  _name)).path.str
+0002f8d0: 6970 2827 2f27 290a 2020 2020 2020 2020  ip('/').        
+0002f8e0: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+0002f8f0: 6e74 203d 2069 626d 2e67 6574 5f63 6f73  nt = ibm.get_cos
+0002f900: 5f63 6c69 656e 7428 2775 732d 6561 7374  _client('us-east
+0002f910: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+0002f920: 2020 2020 2020 2063 6c69 656e 742e 6865         client.he
+0002f930: 6164 5f62 7563 6b65 7428 4275 636b 6574  ad_bucket(Bucket
+0002f940: 3d62 7563 6b65 745f 6e61 6d65 290a 2020  =bucket_name).  
+0002f950: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0002f960: 6365 7074 2069 626d 2e69 626d 5f62 6f74  cept ibm.ibm_bot
+0002f970: 6f63 6f72 652e 6578 6365 7074 696f 6e73  ocore.exceptions
+0002f980: 2e43 6c69 656e 7445 7272 6f72 2061 7320  .ClientError as 
+0002f990: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002f9a0: 2020 2020 2020 2069 6620 652e 7265 7370         if e.resp
+0002f9b0: 6f6e 7365 5b27 4572 726f 7227 5d5b 2743  onse['Error']['C
+0002f9c0: 6f64 6527 5d20 3d3d 2027 3430 3427 3a0a  ode'] == '404':.
+0002f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f9e0: 2020 2020 2020 2020 2320 7375 6363 6573          # succes
+0002f9f0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0002fa00: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002fa10: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0002fa20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0002fa30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0002fa40: 726f 7228 2755 6e73 7570 706f 7274 6564  ror('Unsupported
+0002fa50: 2062 7563 6b65 7420 7479 7065 2027 0a20   bucket type '. 
+0002fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fa80: 6627 7b6e 6f6e 6578 6973 745f 6275 636b  f'{nonexist_buck
+0002fa90: 6574 5f75 726c 7d27 290a 0a20 2020 2020  et_url}')..     
+0002faa0: 2020 2020 2020 2023 2043 6865 636b 2069         # Check i
+0002fab0: 6620 6275 636b 6574 2065 7869 7374 7320  f bucket exists 
+0002fac0: 7573 696e 6720 7468 6520 636c 693a 0a20  using the cli:. 
+0002fad0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
 0002fae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002faf0: 2020 2020 2027 6368 6563 6b20 6966 2074       'check if t
-0002fb00: 6865 2074 6573 7473 2061 7265 2063 6f72  he tests are cor
-0002fb10: 7265 6374 2e27 290a 0a20 2020 2020 2020  rect.')..       
-0002fb20: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-0002fb30: 7365 7328 0a20 2020 2020 2020 2020 2020  ses(.           
-0002fb40: 2020 2020 2073 6b79 2e65 7863 6570 7469       sky.excepti
-0002fb50: 6f6e 732e 5374 6f72 6167 6542 7563 6b65  ons.StorageBucke
-0002fb60: 7447 6574 4572 726f 722c 0a20 2020 2020  tGetError,.     
-0002fb70: 2020 2020 2020 2020 2020 206d 6174 6368             match
-0002fb80: 3d27 4174 7465 6d70 7465 6420 746f 2075  ='Attempted to u
-0002fb90: 7365 2061 206e 6f6e 2d65 7869 7374 656e  se a non-existen
-0002fba0: 7420 6275 636b 6574 2061 7320 6120 736f  t bucket as a so
-0002fbb0: 7572 6365 2729 3a0a 2020 2020 2020 2020  urce'):.        
-0002fbc0: 2020 2020 7374 6f72 6167 655f 6f62 6a20      storage_obj 
-0002fbd0: 3d20 7374 6f72 6167 655f 6c69 622e 5374  = storage_lib.St
-0002fbe0: 6f72 6167 6528 736f 7572 6365 3d6e 6f6e  orage(source=non
-0002fbf0: 6578 6973 745f 6275 636b 6574 5f75 726c  exist_bucket_url
-0002fc00: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0002fc10: 2020 2020 2020 2020 2072 616e 646f 6d5f           random_
-0002fc20: 6e61 6d65 3d6e 6f6e 6578 6973 745f 6275  name=nonexist_bu
-0002fc30: 636b 6574 5f6e 616d 6529 290a 0a20 2020  cket_name))..   
-0002fc40: 2040 7079 7465 7374 2e6d 6172 6b2e 6e6f   @pytest.mark.no
-0002fc50: 5f66 6c75 6964 7374 6163 6b0a 2020 2020  _fluidstack.    
-0002fc60: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-0002fc70: 616d 6574 7269 7a65 2827 7072 6976 6174  ametrize('privat
-0002fc80: 655f 6275 636b 6574 272c 205b 0a20 2020  e_bucket', [.   
-0002fc90: 2020 2020 2066 2773 333a 2f2f 696d 6167       f's3://imag
-0002fca0: 656e 6574 272c 2066 2767 733a 2f2f 696d  enet', f'gs://im
-0002fcb0: 6167 656e 6574 272c 0a20 2020 2020 2020  agenet',.       
-0002fcc0: 2070 7974 6573 742e 7061 7261 6d28 2763   pytest.param('c
-0002fcd0: 6f73 3a2f 2f75 732d 6561 7374 2f62 7563  os://us-east/buc
-0002fce0: 6b65 7431 272c 206d 6172 6b73 3d70 7974  ket1', marks=pyt
-0002fcf0: 6573 742e 6d61 726b 2e69 626d 290a 2020  est.mark.ibm).  
-0002fd00: 2020 5d29 0a20 2020 2064 6566 2074 6573    ]).    def tes
-0002fd10: 745f 7072 6976 6174 655f 6275 636b 6574  t_private_bucket
-0002fd20: 2873 656c 662c 2070 7269 7661 7465 5f62  (self, private_b
-0002fd30: 7563 6b65 7429 3a0a 2020 2020 2020 2020  ucket):.        
-0002fd40: 2320 4174 7465 6d70 7473 2074 6f20 6163  # Attempts to ac
-0002fd50: 6365 7373 2070 7269 7661 7465 2062 7563  cess private buc
-0002fd60: 6b65 7473 206e 6f74 2062 656c 6f6e 6769  kets not belongi
-0002fd70: 6e67 2074 6f20 7468 6520 7573 6572 2e0a  ng to the user..
-0002fd80: 2020 2020 2020 2020 2320 5468 6573 6520          # These 
-0002fd90: 6275 636b 6574 7320 6172 6520 6b6e 6f77  buckets are know
-0002fda0: 6e20 746f 2062 6520 7072 6976 6174 652c  n to be private,
-0002fdb0: 2062 7574 206d 6179 206e 6565 6420 746f   but may need to
-0002fdc0: 2062 6520 7570 6461 7465 6420 6966 0a20   be updated if. 
-0002fdd0: 2020 2020 2020 2023 2074 6865 7920 6172         # they ar
-0002fde0: 6520 7265 6d6f 7665 6420 6279 2074 6865  e removed by the
-0002fdf0: 6972 206f 776e 6572 732e 0a20 2020 2020  ir owners..     
-0002fe00: 2020 2070 7269 7661 7465 5f62 7563 6b65     private_bucke
-0002fe10: 745f 6e61 6d65 203d 2075 726c 6c69 622e  t_name = urllib.
-0002fe20: 7061 7273 652e 7572 6c73 706c 6974 2870  parse.urlsplit(p
-0002fe30: 7269 7661 7465 5f62 7563 6b65 7429 2e6e  rivate_bucket).n
-0002fe40: 6574 6c6f 6320 6966 205c 0a20 2020 2020  etloc if \.     
-0002fe50: 2020 2020 2020 2020 2075 726c 6c69 622e           urllib.
-0002fe60: 7061 7273 652e 7572 6c73 706c 6974 2870  parse.urlsplit(p
-0002fe70: 7269 7661 7465 5f62 7563 6b65 7429 2e73  rivate_bucket).s
-0002fe80: 6368 656d 6520 213d 2027 636f 7327 2065  cheme != 'cos' e
-0002fe90: 6c73 6520 5c0a 2020 2020 2020 2020 2020  lse \.          
-0002fea0: 2020 2020 2020 2020 7572 6c6c 6962 2e70          urllib.p
-0002feb0: 6172 7365 2e75 726c 7370 6c69 7428 7072  arse.urlsplit(pr
-0002fec0: 6976 6174 655f 6275 636b 6574 292e 7061  ivate_bucket).pa
-0002fed0: 7468 2e73 7472 6970 2827 2f27 290a 2020  th.strip('/').  
-0002fee0: 2020 2020 2020 7769 7468 2070 7974 6573        with pytes
-0002fef0: 742e 7261 6973 6573 280a 2020 2020 2020  t.raises(.      
-0002ff00: 2020 2020 2020 2020 2020 736b 792e 6578            sky.ex
-0002ff10: 6365 7074 696f 6e73 2e53 746f 7261 6765  ceptions.Storage
-0002ff20: 4275 636b 6574 4765 7445 7272 6f72 2c0a  BucketGetError,.
-0002ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ff40: 6d61 7463 683d 7374 6f72 6167 655f 6c69  match=storage_li
-0002ff50: 622e 5f42 5543 4b45 545f 4641 494c 5f54  b._BUCKET_FAIL_T
-0002ff60: 4f5f 434f 4e4e 4543 545f 4d45 5353 4147  O_CONNECT_MESSAG
-0002ff70: 452e 666f 726d 6174 280a 2020 2020 2020  E.format(.      
-0002ff80: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0002ff90: 6d65 3d70 7269 7661 7465 5f62 7563 6b65  me=private_bucke
-0002ffa0: 745f 6e61 6d65 2929 3a0a 2020 2020 2020  t_name)):.      
-0002ffb0: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
-0002ffc0: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
-0002ffd0: 5374 6f72 6167 6528 736f 7572 6365 3d70  Storage(source=p
-0002ffe0: 7269 7661 7465 5f62 7563 6b65 7429 0a0a  rivate_bucket)..
-0002fff0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00030000: 2e6e 6f5f 666c 7569 6473 7461 636b 0a20  .no_fluidstack. 
-00030010: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00030020: 7061 7261 6d65 7472 697a 6528 2765 7874  parametrize('ext
-00030030: 5f62 7563 6b65 745f 6669 7874 7572 652c  _bucket_fixture,
-00030040: 2073 746f 7265 5f74 7970 6527 2c0a 2020   store_type',.  
-00030050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030060: 2020 2020 2020 2020 2020 205b 2827 746d             [('tm
-00030070: 705f 6177 7363 6c69 5f62 7563 6b65 7427  p_awscli_bucket'
-00030080: 2c20 7374 6f72 6167 655f 6c69 622e 5374  , storage_lib.St
-00030090: 6f72 6554 7970 652e 5333 292c 0a20 2020  oreType.S3),.   
-000300a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000300b0: 2020 2020 2020 2020 2020 2028 2774 6d70             ('tmp
-000300c0: 5f67 7375 7469 6c5f 6275 636b 6574 272c  _gsutil_bucket',
-000300d0: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-000300e0: 7265 5479 7065 2e47 4353 292c 0a20 2020  reType.GCS),.   
-000300f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030100: 2020 2020 2020 2020 2020 2070 7974 6573             pytes
-00030110: 742e 7061 7261 6d28 2774 6d70 5f69 626d  t.param('tmp_ibm
-00030120: 5f63 6f73 5f62 7563 6b65 7427 2c0a 2020  _cos_bucket',.  
-00030130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030150: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-00030160: 5f6c 6962 2e53 746f 7265 5479 7065 2e49  _lib.StoreType.I
-00030170: 424d 2c0a 2020 2020 2020 2020 2020 2020  BM,.            
-00030180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030190: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000301a0: 6172 6b73 3d70 7974 6573 742e 6d61 726b  arks=pytest.mark
-000301b0: 2e69 626d 292c 0a20 2020 2020 2020 2020  .ibm),.         
-000301c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000301d0: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
-000301e0: 6d28 2774 6d70 5f61 7773 636c 695f 6275  m('tmp_awscli_bu
-000301f0: 636b 6574 5f72 3227 2c0a 2020 2020 2020  cket_r2',.      
-00030200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030220: 2020 2020 2073 746f 7261 6765 5f6c 6962       storage_lib
-00030230: 2e53 746f 7265 5479 7065 2e52 322c 0a20  .StoreType.R2,. 
-00030240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030260: 2020 2020 2020 2020 2020 6d61 726b 733d            marks=
-00030270: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
-00030280: 6466 6c61 7265 295d 290a 2020 2020 6465  dflare)]).    de
-00030290: 6620 7465 7374 5f75 706c 6f61 645f 746f  f test_upload_to
-000302a0: 5f65 7869 7374 696e 675f 6275 636b 6574  _existing_bucket
-000302b0: 2873 656c 662c 2065 7874 5f62 7563 6b65  (self, ext_bucke
-000302c0: 745f 6669 7874 7572 652c 2072 6571 7565  t_fixture, reque
-000302d0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
-000302e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000302f0: 2020 2020 2020 2020 2020 2074 6d70 5f73             tmp_s
-00030300: 6f75 7263 652c 2073 746f 7265 5f74 7970  ource, store_typ
-00030310: 6529 3a0a 2020 2020 2020 2020 2320 5472  e):.        # Tr
-00030320: 6965 7320 7570 6c6f 6164 696e 6720 6578  ies uploading ex
-00030330: 6973 7469 6e67 2066 696c 6573 2074 6f20  isting files to 
-00030340: 6e65 776c 7920 6372 6561 7465 6420 6275  newly created bu
-00030350: 636b 6574 2028 6f75 7473 6964 6520 6f66  cket (outside of
-00030360: 0a20 2020 2020 2020 2023 2073 6b79 2920  .        # sky) 
-00030370: 616e 6420 7665 7269 6669 6573 2074 6861  and verifies tha
-00030380: 7420 6669 6c65 7320 6172 6520 7772 6974  t files are writ
-00030390: 7465 6e2e 0a20 2020 2020 2020 2062 7563  ten..        buc
-000303a0: 6b65 745f 6e61 6d65 2c20 5f20 3d20 7265  ket_name, _ = re
-000303b0: 7175 6573 742e 6765 7466 6978 7475 7265  quest.getfixture
-000303c0: 7661 6c75 6528 6578 745f 6275 636b 6574  value(ext_bucket
-000303d0: 5f66 6978 7475 7265 290a 2020 2020 2020  _fixture).      
-000303e0: 2020 7374 6f72 6167 655f 6f62 6a20 3d20    storage_obj = 
-000303f0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-00030400: 6167 6528 6e61 6d65 3d62 7563 6b65 745f  age(name=bucket_
-00030410: 6e61 6d65 2c20 736f 7572 6365 3d74 6d70  name, source=tmp
-00030420: 5f73 6f75 7263 6529 0a20 2020 2020 2020  _source).       
-00030430: 2073 746f 7261 6765 5f6f 626a 2e61 6464   storage_obj.add
-00030440: 5f73 746f 7265 2873 746f 7265 5f74 7970  _store(store_typ
-00030450: 6529 0a0a 2020 2020 2020 2020 2320 4368  e)..        # Ch
-00030460: 6563 6b20 6966 2074 6d70 5f73 6f75 7263  eck if tmp_sourc
-00030470: 652f 746d 702d 6669 6c65 2065 7869 7374  e/tmp-file exist
-00030480: 7320 696e 2074 6865 2062 7563 6b65 7420  s in the bucket 
-00030490: 7573 696e 6720 6177 7320 636c 690a 2020  using aws cli.  
-000304a0: 2020 2020 2020 6f75 7420 3d20 7375 6270        out = subp
-000304b0: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
-000304c0: 7075 7428 7365 6c66 2e63 6c69 5f6c 735f  put(self.cli_ls_
-000304d0: 636d 6428 7374 6f72 655f 7479 7065 2c20  cmd(store_type, 
-000304e0: 6275 636b 6574 5f6e 616d 6529 2c0a 2020  bucket_name),.  
-000304f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030510: 2020 2020 7368 656c 6c3d 5472 7565 290a      shell=True).
-00030520: 2020 2020 2020 2020 6173 7365 7274 2027          assert '
-00030530: 746d 702d 6669 6c65 2720 696e 206f 7574  tmp-file' in out
-00030540: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00030550: 2c20 5c0a 2020 2020 2020 2020 2020 2020  , \.            
-00030560: 2746 696c 6520 6e6f 7420 666f 756e 6420  'File not found 
-00030570: 696e 2062 7563 6b65 7420 2d20 6f75 7470  in bucket - outp
-00030580: 7574 2077 6173 203a 207b 7d27 2e66 6f72  ut was : {}'.for
-00030590: 6d61 7428 6f75 742e 6465 636f 6465 0a20  mat(out.decode. 
-000305a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000305b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000305c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000305d0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000305e0: 2775 7466 2d38 2729 290a 0a20 2020 2020  'utf-8'))..     
-000305f0: 2020 2023 2043 6865 636b 2073 796d 6c69     # Check symli
-00030600: 6e6b 7320 2d20 7379 6d6c 696e 6b73 2064  nks - symlinks d
-00030610: 6f6e 2774 2067 6574 2063 6f70 6965 6420  on't get copied 
-00030620: 6279 2073 6b79 2073 746f 7261 6765 0a20  by sky storage. 
-00030630: 2020 2020 2020 2061 7373 6572 7420 2870         assert (p
-00030640: 6174 686c 6962 2e50 6174 6828 746d 705f  athlib.Path(tmp_
-00030650: 736f 7572 6365 2920 2f20 2763 6972 636c  source) / 'circl
-00030660: 652d 6c69 6e6b 2729 2e69 735f 7379 6d6c  e-link').is_syml
-00030670: 696e 6b28 292c 2028 0a20 2020 2020 2020  ink(), (.       
-00030680: 2020 2020 2027 6369 7263 6c65 2d6c 696e       'circle-lin
-00030690: 6b20 7761 7320 6e6f 7420 666f 756e 6420  k was not found 
-000306a0: 696e 2074 6865 2075 706c 6f61 6420 736f  in the upload so
-000306b0: 7572 6365 202d 2027 0a20 2020 2020 2020  urce - '.       
-000306c0: 2020 2020 2027 6172 6520 7468 6520 7465       'are the te
-000306d0: 7374 2066 6978 7475 7265 7320 636f 7272  st fixtures corr
-000306e0: 6563 743f 2729 0a20 2020 2020 2020 2061  ect?').        a
-000306f0: 7373 6572 7420 2763 6972 636c 652d 6c69  ssert 'circle-li
-00030700: 6e6b 2720 6e6f 7420 696e 206f 7574 2e64  nk' not in out.d
-00030710: 6563 6f64 6528 2775 7466 2d38 2729 2c20  ecode('utf-8'), 
-00030720: 280a 2020 2020 2020 2020 2020 2020 2753  (.            'S
-00030730: 796d 6c69 6e6b 2066 6f75 6e64 2069 6e20  ymlink found in 
-00030740: 6275 636b 6574 202d 206c 7320 6f75 7470  bucket - ls outp
-00030750: 7574 2077 6173 203a 207b 7d27 2e66 6f72  ut was : {}'.for
-00030760: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00030770: 2020 2020 206f 7574 2e64 6563 6f64 6528       out.decode(
-00030780: 2775 7466 2d38 2729 2929 0a0a 2020 2020  'utf-8')))..    
-00030790: 2020 2020 2320 5275 6e20 736b 7920 7374      # Run sky st
-000307a0: 6f72 6167 6520 6c73 2074 6f20 6368 6563  orage ls to chec
-000307b0: 6b20 6966 2073 746f 7261 6765 206f 626a  k if storage obj
-000307c0: 6563 7420 6578 6973 7473 2069 6e20 7468  ect exists in th
-000307d0: 6520 6f75 7470 7574 2e0a 2020 2020 2020  e output..      
-000307e0: 2020 2320 4974 2073 686f 756c 6420 6e6f    # It should no
-000307f0: 7420 6578 6973 7420 6265 6361 7573 6520  t exist because 
-00030800: 7468 6520 6275 636b 6574 2077 6173 2063  the bucket was c
-00030810: 7265 6174 6564 2065 7874 6572 6e61 6c6c  reated externall
-00030820: 792e 0a20 2020 2020 2020 206f 7574 203d  y..        out =
-00030830: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-00030840: 6b5f 6f75 7470 7574 285b 2773 6b79 272c  k_output(['sky',
-00030850: 2027 7374 6f72 6167 6527 2c20 276c 7327   'storage', 'ls'
-00030860: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-00030870: 7420 7374 6f72 6167 655f 6f62 6a2e 6e61  t storage_obj.na
-00030880: 6d65 206e 6f74 2069 6e20 6f75 742e 6465  me not in out.de
-00030890: 636f 6465 2827 7574 662d 3827 290a 0a20  code('utf-8').. 
-000308a0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-000308b0: 6e6f 5f66 6c75 6964 7374 6163 6b0a 2020  no_fluidstack.  
-000308c0: 2020 6465 6620 7465 7374 5f63 6f70 795f    def test_copy_
-000308d0: 6d6f 756e 745f 6578 6973 7469 6e67 5f73  mount_existing_s
-000308e0: 746f 7261 6765 2873 656c 662c 0a20 2020  torage(self,.   
-000308f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030910: 2020 2020 2020 746d 705f 636f 7079 5f6d        tmp_copy_m
-00030920: 6e74 5f65 7869 7374 696e 675f 7374 6f72  nt_existing_stor
-00030930: 6167 655f 6f62 6a29 3a0a 2020 2020 2020  age_obj):.      
-00030940: 2020 2320 4372 6561 7465 7320 6120 6275    # Creates a bu
-00030950: 636b 6574 2077 6974 6820 6e6f 2073 6f75  cket with no sou
-00030960: 7263 6520 696e 204d 4f55 4e54 206d 6f64  rce in MOUNT mod
-00030970: 6520 2865 6d70 7479 2062 7563 6b65 7429  e (empty bucket)
-00030980: 2c20 616e 640a 2020 2020 2020 2020 2320  , and.        # 
-00030990: 7468 656e 2074 7269 6573 2074 6f20 6c6f  then tries to lo
-000309a0: 6164 2074 6865 2073 616d 6520 7374 6f72  ad the same stor
-000309b0: 6167 6520 696e 2043 4f50 5920 6d6f 6465  age in COPY mode
-000309c0: 2e0a 2020 2020 2020 2020 746d 705f 636f  ..        tmp_co
-000309d0: 7079 5f6d 6e74 5f65 7869 7374 696e 675f  py_mnt_existing_
-000309e0: 7374 6f72 6167 655f 6f62 6a2e 6164 645f  storage_obj.add_
-000309f0: 7374 6f72 6528 7374 6f72 6167 655f 6c69  store(storage_li
-00030a00: 622e 5374 6f72 6554 7970 652e 5333 290a  b.StoreType.S3).
-00030a10: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-00030a20: 6e61 6d65 203d 2074 6d70 5f63 6f70 795f  name = tmp_copy_
-00030a30: 6d6e 745f 6578 6973 7469 6e67 5f73 746f  mnt_existing_sto
-00030a40: 7261 6765 5f6f 626a 2e6e 616d 650a 0a20  rage_obj.name.. 
-00030a50: 2020 2020 2020 2023 2043 6865 636b 2060         # Check `
-00030a60: 736b 7920 7374 6f72 6167 6520 6c73 6020  sky storage ls` 
-00030a70: 746f 2065 6e73 7572 6520 7374 6f72 6167  to ensure storag
-00030a80: 6520 6f62 6a65 6374 2065 7869 7374 730a  e object exists.
-00030a90: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
-00030aa0: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
-00030ab0: 7574 7075 7428 5b27 736b 7927 2c20 2773  utput(['sky', 's
-00030ac0: 746f 7261 6765 272c 2027 6c73 275d 292e  torage', 'ls']).
-00030ad0: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
-00030ae0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00030af0: 746f 7261 6765 5f6e 616d 6520 696e 206f  torage_name in o
-00030b00: 7574 2c20 6627 5374 6f72 6167 6520 7b73  ut, f'Storage {s
-00030b10: 746f 7261 6765 5f6e 616d 657d 206e 6f74  torage_name} not
-00030b20: 2066 6f75 6e64 2069 6e20 736b 7920 7374   found in sky st
-00030b30: 6f72 6167 6520 6c73 2e27 0a0a 2020 2020  orage ls.'..    
-00030b40: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
-00030b50: 666c 7569 6473 7461 636b 0a20 2020 2040  fluidstack.    @
-00030b60: 7079 7465 7374 2e6d 6172 6b2e 7061 7261  pytest.mark.para
-00030b70: 6d65 7472 697a 6528 2773 746f 7265 5f74  metrize('store_t
-00030b80: 7970 6527 2c20 5b0a 2020 2020 2020 2020  ype', [.        
-00030b90: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-00030ba0: 6554 7970 652e 5333 2c20 7374 6f72 6167  eType.S3, storag
-00030bb0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-00030bc0: 4743 532c 0a20 2020 2020 2020 2070 7974  GCS,.        pyt
-00030bd0: 6573 742e 7061 7261 6d28 7374 6f72 6167  est.param(storag
-00030be0: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-00030bf0: 4942 4d2c 206d 6172 6b73 3d70 7974 6573  IBM, marks=pytes
-00030c00: 742e 6d61 726b 2e69 626d 292c 0a20 2020  t.mark.ibm),.   
-00030c10: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
-00030c20: 6d28 7374 6f72 6167 655f 6c69 622e 5374  m(storage_lib.St
-00030c30: 6f72 6554 7970 652e 5232 2c20 6d61 726b  oreType.R2, mark
-00030c40: 733d 7079 7465 7374 2e6d 6172 6b2e 636c  s=pytest.mark.cl
-00030c50: 6f75 6466 6c61 7265 290a 2020 2020 5d29  oudflare).    ])
-00030c60: 0a20 2020 2064 6566 2074 6573 745f 6c69  .    def test_li
-00030c70: 7374 5f73 6f75 7263 6528 7365 6c66 2c20  st_source(self, 
-00030c80: 746d 705f 6c6f 6361 6c5f 6c69 7374 5f73  tmp_local_list_s
-00030c90: 746f 7261 6765 5f6f 626a 2c20 7374 6f72  torage_obj, stor
-00030ca0: 655f 7479 7065 293a 0a20 2020 2020 2020  e_type):.       
-00030cb0: 2023 2055 7365 7320 6120 6c69 7374 2069   # Uses a list i
-00030cc0: 6e20 7468 6520 736f 7572 6365 2066 6965  n the source fie
-00030cd0: 6c64 2074 6f20 7370 6563 6966 7920 6120  ld to specify a 
-00030ce0: 6669 6c65 2061 6e64 2061 2064 6972 6563  file and a direc
-00030cf0: 746f 7279 2074 6f0a 2020 2020 2020 2020  tory to.        
-00030d00: 2320 6265 2075 706c 6f61 6465 6420 746f  # be uploaded to
-00030d10: 2074 6865 2073 746f 7261 6765 206f 626a   the storage obj
-00030d20: 6563 742e 0a20 2020 2020 2020 2074 6d70  ect..        tmp
-00030d30: 5f6c 6f63 616c 5f6c 6973 745f 7374 6f72  _local_list_stor
-00030d40: 6167 655f 6f62 6a2e 6164 645f 7374 6f72  age_obj.add_stor
-00030d50: 6528 7374 6f72 655f 7479 7065 290a 0a20  e(store_type).. 
-00030d60: 2020 2020 2020 2023 2043 6865 636b 2069         # Check i
-00030d70: 6620 746d 702d 6669 6c65 2065 7869 7374  f tmp-file exist
-00030d80: 7320 696e 2074 6865 2062 7563 6b65 7420  s in the bucket 
-00030d90: 726f 6f74 2075 7369 6e67 2063 6c69 0a20  root using cli. 
-00030da0: 2020 2020 2020 206f 7574 203d 2073 7562         out = sub
-00030db0: 7072 6f63 6573 732e 6368 6563 6b5f 6f75  process.check_ou
-00030dc0: 7470 7574 2873 656c 662e 636c 695f 6c73  tput(self.cli_ls
-00030dd0: 5f63 6d64 280a 2020 2020 2020 2020 2020  _cmd(.          
-00030de0: 2020 7374 6f72 655f 7479 7065 2c20 746d    store_type, tm
-00030df0: 705f 6c6f 6361 6c5f 6c69 7374 5f73 746f  p_local_list_sto
-00030e00: 7261 6765 5f6f 626a 2e6e 616d 6529 2c0a  rage_obj.name),.
-00030e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030e30: 2020 2020 2020 7368 656c 6c3d 5472 7565        shell=True
-00030e40: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-00030e50: 2027 746d 702d 6669 6c65 2720 696e 206f   'tmp-file' in o
-00030e60: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
-00030e70: 2729 2c20 5c0a 2020 2020 2020 2020 2020  '), \.          
-00030e80: 2020 2746 696c 6520 6e6f 7420 666f 756e    'File not foun
-00030e90: 6420 696e 2062 7563 6b65 7420 2d20 6f75  d in bucket - ou
-00030ea0: 7470 7574 2077 6173 203a 207b 7d27 2e66  tput was : {}'.f
-00030eb0: 6f72 6d61 7428 6f75 742e 6465 636f 6465  ormat(out.decode
-00030ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00030ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030f00: 2028 2775 7466 2d38 2729 290a 0a20 2020   ('utf-8'))..   
-00030f10: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
-00030f20: 746d 702d 6669 6c65 2065 7869 7374 7320  tmp-file exists 
-00030f30: 696e 2074 6865 2062 7563 6b65 742f 746d  in the bucket/tm
-00030f40: 702d 736f 7572 6365 2075 7369 6e67 2063  p-source using c
-00030f50: 6c69 0a20 2020 2020 2020 206f 7574 203d  li.        out =
-00030f60: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-00030f70: 6b5f 6f75 7470 7574 2873 656c 662e 636c  k_output(self.cl
-00030f80: 695f 6c73 5f63 6d64 280a 2020 2020 2020  i_ls_cmd(.      
-00030f90: 2020 2020 2020 7374 6f72 655f 7479 7065        store_type
-00030fa0: 2c20 746d 705f 6c6f 6361 6c5f 6c69 7374  , tmp_local_list
-00030fb0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-00030fc0: 652c 2027 746d 702d 736f 7572 6365 2f27  e, 'tmp-source/'
-00030fd0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00030fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ff0: 2020 2020 2020 2020 2073 6865 6c6c 3d54           shell=T
-00031000: 7275 6529 0a20 2020 2020 2020 2061 7373  rue).        ass
-00031010: 6572 7420 2774 6d70 2d66 696c 6527 2069  ert 'tmp-file' i
-00031020: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-00031030: 662d 3827 292c 205c 0a20 2020 2020 2020  f-8'), \.       
-00031040: 2020 2020 2027 4669 6c65 206e 6f74 2066       'File not f
-00031050: 6f75 6e64 2069 6e20 6275 636b 6574 202d  ound in bucket -
-00031060: 206f 7574 7075 7420 7761 7320 3a20 7b7d   output was : {}
-00031070: 272e 666f 726d 6174 286f 7574 2e64 6563  '.format(out.dec
-00031080: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
+0002faf0: 6f75 7420 3d20 7375 6270 726f 6365 7373  out = subprocess
+0002fb00: 2e63 6865 636b 5f6f 7574 7075 7428 636f  .check_output(co
+0002fb10: 6d6d 616e 642c 0a20 2020 2020 2020 2020  mmand,.         
+0002fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb40: 2020 2020 2073 7464 6572 723d 7375 6270       stderr=subp
+0002fb50: 726f 6365 7373 2e53 5444 4f55 542c 0a20  rocess.STDOUT,. 
+0002fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fb80: 2020 2020 2020 2020 2020 2020 2073 6865               she
+0002fb90: 6c6c 3d54 7275 6529 0a20 2020 2020 2020  ll=True).       
+0002fba0: 2020 2020 2065 7863 6570 7420 7375 6270       except subp
+0002fbb0: 726f 6365 7373 2e43 616c 6c65 6450 726f  rocess.CalledPro
+0002fbc0: 6365 7373 4572 726f 7220 6173 2065 3a0a  cessError as e:.
+0002fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fbe0: 6f75 7420 3d20 652e 6f75 7470 7574 0a20  out = e.output. 
+0002fbf0: 2020 2020 2020 2020 2020 206f 7574 203d             out =
+0002fc00: 206f 7574 2e64 6563 6f64 6528 2775 7466   out.decode('utf
+0002fc10: 2d38 2729 0a20 2020 2020 2020 2020 2020  -8').           
+0002fc20: 2069 6620 6578 7065 6374 6564 5f6f 7574   if expected_out
+0002fc30: 7075 7420 696e 206f 7574 3a0a 2020 2020  put in out:.    
+0002fc40: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0002fc50: 6b0a 2020 2020 2020 2020 2020 2020 656c  k.            el
+0002fc60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0002fc70: 2020 2020 7265 7472 795f 636f 756e 7420      retry_count 
+0002fc80: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
+0002fc90: 2020 2020 2069 6620 7265 7472 795f 636f       if retry_co
+0002fca0: 756e 7420 3e20 333a 0a20 2020 2020 2020  unt > 3:.       
+0002fcb0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0002fcc0: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
+0002fcd0: 2755 6e61 626c 6520 746f 2066 696e 6420  'Unable to find 
+0002fce0: 6120 6e6f 6e65 7869 7374 656e 7420 6275  a nonexistent bu
+0002fcf0: 636b 6574 2027 0a20 2020 2020 2020 2020  cket '.         
+0002fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fd10: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0002fd20: 6f20 7573 652e 2054 6869 7320 6973 2068  o use. This is h
+0002fd30: 6967 6c79 2075 6e6c 696b 656c 7920 2d20  igly unlikely - 
+0002fd40: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0002fd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002fd60: 2020 2020 2020 2020 2027 6368 6563 6b20           'check 
+0002fd70: 6966 2074 6865 2074 6573 7473 2061 7265  if the tests are
+0002fd80: 2063 6f72 7265 6374 2e27 290a 0a20 2020   correct.')..   
+0002fd90: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
+0002fda0: 2e72 6169 7365 7328 0a20 2020 2020 2020  .raises(.       
+0002fdb0: 2020 2020 2020 2020 2073 6b79 2e65 7863           sky.exc
+0002fdc0: 6570 7469 6f6e 732e 5374 6f72 6167 6542  eptions.StorageB
+0002fdd0: 7563 6b65 7447 6574 4572 726f 722c 0a20  ucketGetError,. 
+0002fde0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0002fdf0: 6174 6368 3d27 4174 7465 6d70 7465 6420  atch='Attempted 
+0002fe00: 746f 2075 7365 2061 206e 6f6e 2d65 7869  to use a non-exi
+0002fe10: 7374 656e 7420 6275 636b 6574 2061 7320  stent bucket as 
+0002fe20: 6120 736f 7572 6365 2729 3a0a 2020 2020  a source'):.    
+0002fe30: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
+0002fe40: 6f62 6a20 3d20 7374 6f72 6167 655f 6c69  obj = storage_li
+0002fe50: 622e 5374 6f72 6167 6528 736f 7572 6365  b.Storage(source
+0002fe60: 3d6e 6f6e 6578 6973 745f 6275 636b 6574  =nonexist_bucket
+0002fe70: 5f75 726c 2e66 6f72 6d61 7428 0a20 2020  _url.format(.   
+0002fe80: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+0002fe90: 646f 6d5f 6e61 6d65 3d6e 6f6e 6578 6973  dom_name=nonexis
+0002fea0: 745f 6275 636b 6574 5f6e 616d 6529 290a  t_bucket_name)).
+0002feb0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+0002fec0: 6b2e 6e6f 5f66 6c75 6964 7374 6163 6b0a  k.no_fluidstack.
+0002fed0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+0002fee0: 2e70 6172 616d 6574 7269 7a65 2827 7072  .parametrize('pr
+0002fef0: 6976 6174 655f 6275 636b 6574 272c 205b  ivate_bucket', [
+0002ff00: 0a20 2020 2020 2020 2066 2773 333a 2f2f  .        f's3://
+0002ff10: 696d 6167 656e 6574 272c 2066 2767 733a  imagenet', f'gs:
+0002ff20: 2f2f 696d 6167 656e 6574 272c 0a20 2020  //imagenet',.   
+0002ff30: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
+0002ff40: 6d28 2763 6f73 3a2f 2f75 732d 6561 7374  m('cos://us-east
+0002ff50: 2f62 7563 6b65 7431 272c 206d 6172 6b73  /bucket1', marks
+0002ff60: 3d70 7974 6573 742e 6d61 726b 2e69 626d  =pytest.mark.ibm
+0002ff70: 290a 2020 2020 5d29 0a20 2020 2064 6566  ).    ]).    def
+0002ff80: 2074 6573 745f 7072 6976 6174 655f 6275   test_private_bu
+0002ff90: 636b 6574 2873 656c 662c 2070 7269 7661  cket(self, priva
+0002ffa0: 7465 5f62 7563 6b65 7429 3a0a 2020 2020  te_bucket):.    
+0002ffb0: 2020 2020 2320 4174 7465 6d70 7473 2074      # Attempts t
+0002ffc0: 6f20 6163 6365 7373 2070 7269 7661 7465  o access private
+0002ffd0: 2062 7563 6b65 7473 206e 6f74 2062 656c   buckets not bel
+0002ffe0: 6f6e 6769 6e67 2074 6f20 7468 6520 7573  onging to the us
+0002fff0: 6572 2e0a 2020 2020 2020 2020 2320 5468  er..        # Th
+00030000: 6573 6520 6275 636b 6574 7320 6172 6520  ese buckets are 
+00030010: 6b6e 6f77 6e20 746f 2062 6520 7072 6976  known to be priv
+00030020: 6174 652c 2062 7574 206d 6179 206e 6565  ate, but may nee
+00030030: 6420 746f 2062 6520 7570 6461 7465 6420  d to be updated 
+00030040: 6966 0a20 2020 2020 2020 2023 2074 6865  if.        # the
+00030050: 7920 6172 6520 7265 6d6f 7665 6420 6279  y are removed by
+00030060: 2074 6865 6972 206f 776e 6572 732e 0a20   their owners.. 
+00030070: 2020 2020 2020 2070 7269 7661 7465 5f62         private_b
+00030080: 7563 6b65 745f 6e61 6d65 203d 2075 726c  ucket_name = url
+00030090: 6c69 622e 7061 7273 652e 7572 6c73 706c  lib.parse.urlspl
+000300a0: 6974 2870 7269 7661 7465 5f62 7563 6b65  it(private_bucke
+000300b0: 7429 2e6e 6574 6c6f 6320 6966 205c 0a20  t).netloc if \. 
+000300c0: 2020 2020 2020 2020 2020 2020 2075 726c               url
+000300d0: 6c69 622e 7061 7273 652e 7572 6c73 706c  lib.parse.urlspl
+000300e0: 6974 2870 7269 7661 7465 5f62 7563 6b65  it(private_bucke
+000300f0: 7429 2e73 6368 656d 6520 213d 2027 636f  t).scheme != 'co
+00030100: 7327 2065 6c73 6520 5c0a 2020 2020 2020  s' else \.      
+00030110: 2020 2020 2020 2020 2020 2020 7572 6c6c              urll
+00030120: 6962 2e70 6172 7365 2e75 726c 7370 6c69  ib.parse.urlspli
+00030130: 7428 7072 6976 6174 655f 6275 636b 6574  t(private_bucket
+00030140: 292e 7061 7468 2e73 7472 6970 2827 2f27  ).path.strip('/'
+00030150: 290a 2020 2020 2020 2020 7769 7468 2070  ).        with p
+00030160: 7974 6573 742e 7261 6973 6573 280a 2020  ytest.raises(.  
+00030170: 2020 2020 2020 2020 2020 2020 2020 736b                sk
+00030180: 792e 6578 6365 7074 696f 6e73 2e53 746f  y.exceptions.Sto
+00030190: 7261 6765 4275 636b 6574 4765 7445 7272  rageBucketGetErr
+000301a0: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+000301b0: 2020 2020 6d61 7463 683d 7374 6f72 6167      match=storag
+000301c0: 655f 6c69 622e 5f42 5543 4b45 545f 4641  e_lib._BUCKET_FA
+000301d0: 494c 5f54 4f5f 434f 4e4e 4543 545f 4d45  IL_TO_CONNECT_ME
+000301e0: 5353 4147 452e 666f 726d 6174 280a 2020  SSAGE.format(.  
+000301f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030200: 2020 6e61 6d65 3d70 7269 7661 7465 5f62    name=private_b
+00030210: 7563 6b65 745f 6e61 6d65 2929 3a0a 2020  ucket_name)):.  
+00030220: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+00030230: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
+00030240: 6c69 622e 5374 6f72 6167 6528 736f 7572  lib.Storage(sour
+00030250: 6365 3d70 7269 7661 7465 5f62 7563 6b65  ce=private_bucke
+00030260: 7429 0a0a 2020 2020 4070 7974 6573 742e  t)..    @pytest.
+00030270: 6d61 726b 2e6e 6f5f 666c 7569 6473 7461  mark.no_fluidsta
+00030280: 636b 0a20 2020 2040 7079 7465 7374 2e6d  ck.    @pytest.m
+00030290: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+000302a0: 2765 7874 5f62 7563 6b65 745f 6669 7874  'ext_bucket_fixt
+000302b0: 7572 652c 2073 746f 7265 5f74 7970 6527  ure, store_type'
+000302c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000302d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000302e0: 2827 746d 705f 6177 7363 6c69 5f62 7563  ('tmp_awscli_buc
+000302f0: 6b65 7427 2c20 7374 6f72 6167 655f 6c69  ket', storage_li
+00030300: 622e 5374 6f72 6554 7970 652e 5333 292c  b.StoreType.S3),
+00030310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030320: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00030330: 2774 6d70 5f67 7375 7469 6c5f 6275 636b  'tmp_gsutil_buck
+00030340: 6574 272c 2073 746f 7261 6765 5f6c 6962  et', storage_lib
+00030350: 2e53 746f 7265 5479 7065 2e47 4353 292c  .StoreType.GCS),
+00030360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030370: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00030380: 7974 6573 742e 7061 7261 6d28 2774 6d70  ytest.param('tmp
+00030390: 5f69 626d 5f63 6f73 5f62 7563 6b65 7427  _ibm_cos_bucket'
+000303a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000303b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000303c0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+000303d0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+000303e0: 7065 2e49 424d 2c0a 2020 2020 2020 2020  pe.IBM,.        
+000303f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030410: 2020 206d 6172 6b73 3d70 7974 6573 742e     marks=pytest.
+00030420: 6d61 726b 2e69 626d 292c 0a20 2020 2020  mark.ibm),.     
+00030430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030440: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
+00030450: 7061 7261 6d28 2774 6d70 5f61 7773 636c  param('tmp_awscl
+00030460: 695f 6275 636b 6574 5f72 3227 2c0a 2020  i_bucket_r2',.  
+00030470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030490: 2020 2020 2020 2020 2073 746f 7261 6765           storage
+000304a0: 5f6c 6962 2e53 746f 7265 5479 7065 2e52  _lib.StoreType.R
+000304b0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+000304c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000304d0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+000304e0: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
+000304f0: 636c 6f75 6466 6c61 7265 295d 290a 2020  cloudflare)]).  
+00030500: 2020 6465 6620 7465 7374 5f75 706c 6f61    def test_uploa
+00030510: 645f 746f 5f65 7869 7374 696e 675f 6275  d_to_existing_bu
+00030520: 636b 6574 2873 656c 662c 2065 7874 5f62  cket(self, ext_b
+00030530: 7563 6b65 745f 6669 7874 7572 652c 2072  ucket_fixture, r
+00030540: 6571 7565 7374 2c0a 2020 2020 2020 2020  equest,.        
+00030550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00030570: 6d70 5f73 6f75 7263 652c 2073 746f 7265  mp_source, store
+00030580: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+00030590: 2320 5472 6965 7320 7570 6c6f 6164 696e  # Tries uploadin
+000305a0: 6720 6578 6973 7469 6e67 2066 696c 6573  g existing files
+000305b0: 2074 6f20 6e65 776c 7920 6372 6561 7465   to newly create
+000305c0: 6420 6275 636b 6574 2028 6f75 7473 6964  d bucket (outsid
+000305d0: 6520 6f66 0a20 2020 2020 2020 2023 2073  e of.        # s
+000305e0: 6b79 2920 616e 6420 7665 7269 6669 6573  ky) and verifies
+000305f0: 2074 6861 7420 6669 6c65 7320 6172 6520   that files are 
+00030600: 7772 6974 7465 6e2e 0a20 2020 2020 2020  written..       
+00030610: 2062 7563 6b65 745f 6e61 6d65 2c20 5f20   bucket_name, _ 
+00030620: 3d20 7265 7175 6573 742e 6765 7466 6978  = request.getfix
+00030630: 7475 7265 7661 6c75 6528 6578 745f 6275  turevalue(ext_bu
+00030640: 636b 6574 5f66 6978 7475 7265 290a 2020  cket_fixture).  
+00030650: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+00030660: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
+00030670: 5374 6f72 6167 6528 6e61 6d65 3d62 7563  Storage(name=buc
+00030680: 6b65 745f 6e61 6d65 2c20 736f 7572 6365  ket_name, source
+00030690: 3d74 6d70 5f73 6f75 7263 6529 0a20 2020  =tmp_source).   
+000306a0: 2020 2020 2073 746f 7261 6765 5f6f 626a       storage_obj
+000306b0: 2e61 6464 5f73 746f 7265 2873 746f 7265  .add_store(store
+000306c0: 5f74 7970 6529 0a0a 2020 2020 2020 2020  _type)..        
+000306d0: 2320 4368 6563 6b20 6966 2074 6d70 5f73  # Check if tmp_s
+000306e0: 6f75 7263 652f 746d 702d 6669 6c65 2065  ource/tmp-file e
+000306f0: 7869 7374 7320 696e 2074 6865 2062 7563  xists in the buc
+00030700: 6b65 7420 7573 696e 6720 6177 7320 636c  ket using aws cl
+00030710: 690a 2020 2020 2020 2020 6f75 7420 3d20  i.        out = 
+00030720: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
+00030730: 5f6f 7574 7075 7428 7365 6c66 2e63 6c69  _output(self.cli
+00030740: 5f6c 735f 636d 6428 7374 6f72 655f 7479  _ls_cmd(store_ty
+00030750: 7065 2c20 6275 636b 6574 5f6e 616d 6529  pe, bucket_name)
+00030760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00030770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030780: 2020 2020 2020 2020 7368 656c 6c3d 5472          shell=Tr
+00030790: 7565 290a 2020 2020 2020 2020 6173 7365  ue).        asse
+000307a0: 7274 2027 746d 702d 6669 6c65 2720 696e  rt 'tmp-file' in
+000307b0: 206f 7574 2e64 6563 6f64 6528 2775 7466   out.decode('utf
+000307c0: 2d38 2729 2c20 5c0a 2020 2020 2020 2020  -8'), \.        
+000307d0: 2020 2020 2746 696c 6520 6e6f 7420 666f      'File not fo
+000307e0: 756e 6420 696e 2062 7563 6b65 7420 2d20  und in bucket - 
+000307f0: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
+00030800: 2e66 6f72 6d61 7428 6f75 742e 6465 636f  .format(out.deco
+00030810: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+00030820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030850: 2020 2028 2775 7466 2d38 2729 290a 0a20     ('utf-8')).. 
+00030860: 2020 2020 2020 2023 2043 6865 636b 2073         # Check s
+00030870: 796d 6c69 6e6b 7320 2d20 7379 6d6c 696e  ymlinks - symlin
+00030880: 6b73 2064 6f6e 2774 2067 6574 2063 6f70  ks don't get cop
+00030890: 6965 6420 6279 2073 6b79 2073 746f 7261  ied by sky stora
+000308a0: 6765 0a20 2020 2020 2020 2061 7373 6572  ge.        asser
+000308b0: 7420 2870 6174 686c 6962 2e50 6174 6828  t (pathlib.Path(
+000308c0: 746d 705f 736f 7572 6365 2920 2f20 2763  tmp_source) / 'c
+000308d0: 6972 636c 652d 6c69 6e6b 2729 2e69 735f  ircle-link').is_
+000308e0: 7379 6d6c 696e 6b28 292c 2028 0a20 2020  symlink(), (.   
+000308f0: 2020 2020 2020 2020 2027 6369 7263 6c65           'circle
+00030900: 2d6c 696e 6b20 7761 7320 6e6f 7420 666f  -link was not fo
+00030910: 756e 6420 696e 2074 6865 2075 706c 6f61  und in the uploa
+00030920: 6420 736f 7572 6365 202d 2027 0a20 2020  d source - '.   
+00030930: 2020 2020 2020 2020 2027 6172 6520 7468           'are th
+00030940: 6520 7465 7374 2066 6978 7475 7265 7320  e test fixtures 
+00030950: 636f 7272 6563 743f 2729 0a20 2020 2020  correct?').     
+00030960: 2020 2061 7373 6572 7420 2763 6972 636c     assert 'circl
+00030970: 652d 6c69 6e6b 2720 6e6f 7420 696e 206f  e-link' not in o
+00030980: 7574 2e64 6563 6f64 6528 2775 7466 2d38  ut.decode('utf-8
+00030990: 2729 2c20 280a 2020 2020 2020 2020 2020  '), (.          
+000309a0: 2020 2753 796d 6c69 6e6b 2066 6f75 6e64    'Symlink found
+000309b0: 2069 6e20 6275 636b 6574 202d 206c 7320   in bucket - ls 
+000309c0: 6f75 7470 7574 2077 6173 203a 207b 7d27  output was : {}'
+000309d0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+000309e0: 2020 2020 2020 2020 206f 7574 2e64 6563           out.dec
+000309f0: 6f64 6528 2775 7466 2d38 2729 2929 0a0a  ode('utf-8')))..
+00030a00: 2020 2020 2020 2020 2320 5275 6e20 736b          # Run sk
+00030a10: 7920 7374 6f72 6167 6520 6c73 2074 6f20  y storage ls to 
+00030a20: 6368 6563 6b20 6966 2073 746f 7261 6765  check if storage
+00030a30: 206f 626a 6563 7420 6578 6973 7473 2069   object exists i
+00030a40: 6e20 7468 6520 6f75 7470 7574 2e0a 2020  n the output..  
+00030a50: 2020 2020 2020 2320 4974 2073 686f 756c        # It shoul
+00030a60: 6420 6e6f 7420 6578 6973 7420 6265 6361  d not exist beca
+00030a70: 7573 6520 7468 6520 6275 636b 6574 2077  use the bucket w
+00030a80: 6173 2063 7265 6174 6564 2065 7874 6572  as created exter
+00030a90: 6e61 6c6c 792e 0a20 2020 2020 2020 206f  nally..        o
+00030aa0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+00030ab0: 6368 6563 6b5f 6f75 7470 7574 285b 2773  check_output(['s
+00030ac0: 6b79 272c 2027 7374 6f72 6167 6527 2c20  ky', 'storage', 
+00030ad0: 276c 7327 5d29 0a20 2020 2020 2020 2061  'ls']).        a
+00030ae0: 7373 6572 7420 7374 6f72 6167 655f 6f62  ssert storage_ob
+00030af0: 6a2e 6e61 6d65 206e 6f74 2069 6e20 6f75  j.name not in ou
+00030b00: 742e 6465 636f 6465 2827 7574 662d 3827  t.decode('utf-8'
+00030b10: 290a 0a20 2020 2040 7079 7465 7374 2e6d  )..    @pytest.m
+00030b20: 6172 6b2e 6e6f 5f66 6c75 6964 7374 6163  ark.no_fluidstac
+00030b30: 6b0a 2020 2020 6465 6620 7465 7374 5f63  k.    def test_c
+00030b40: 6f70 795f 6d6f 756e 745f 6578 6973 7469  opy_mount_existi
+00030b50: 6e67 5f73 746f 7261 6765 2873 656c 662c  ng_storage(self,
+00030b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00030b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030b80: 2020 2020 2020 2020 2020 746d 705f 636f            tmp_co
+00030b90: 7079 5f6d 6e74 5f65 7869 7374 696e 675f  py_mnt_existing_
+00030ba0: 7374 6f72 6167 655f 6f62 6a29 3a0a 2020  storage_obj):.  
+00030bb0: 2020 2020 2020 2320 4372 6561 7465 7320        # Creates 
+00030bc0: 6120 6275 636b 6574 2077 6974 6820 6e6f  a bucket with no
+00030bd0: 2073 6f75 7263 6520 696e 204d 4f55 4e54   source in MOUNT
+00030be0: 206d 6f64 6520 2865 6d70 7479 2062 7563   mode (empty buc
+00030bf0: 6b65 7429 2c20 616e 640a 2020 2020 2020  ket), and.      
+00030c00: 2020 2320 7468 656e 2074 7269 6573 2074    # then tries t
+00030c10: 6f20 6c6f 6164 2074 6865 2073 616d 6520  o load the same 
+00030c20: 7374 6f72 6167 6520 696e 2043 4f50 5920  storage in COPY 
+00030c30: 6d6f 6465 2e0a 2020 2020 2020 2020 746d  mode..        tm
+00030c40: 705f 636f 7079 5f6d 6e74 5f65 7869 7374  p_copy_mnt_exist
+00030c50: 696e 675f 7374 6f72 6167 655f 6f62 6a2e  ing_storage_obj.
+00030c60: 6164 645f 7374 6f72 6528 7374 6f72 6167  add_store(storag
+00030c70: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
+00030c80: 5333 290a 2020 2020 2020 2020 7374 6f72  S3).        stor
+00030c90: 6167 655f 6e61 6d65 203d 2074 6d70 5f63  age_name = tmp_c
+00030ca0: 6f70 795f 6d6e 745f 6578 6973 7469 6e67  opy_mnt_existing
+00030cb0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+00030cc0: 650a 0a20 2020 2020 2020 2023 2043 6865  e..        # Che
+00030cd0: 636b 2060 736b 7920 7374 6f72 6167 6520  ck `sky storage 
+00030ce0: 6c73 6020 746f 2065 6e73 7572 6520 7374  ls` to ensure st
+00030cf0: 6f72 6167 6520 6f62 6a65 6374 2065 7869  orage object exi
+00030d00: 7374 730a 2020 2020 2020 2020 6f75 7420  sts.        out 
+00030d10: 3d20 7375 6270 726f 6365 7373 2e63 6865  = subprocess.che
+00030d20: 636b 5f6f 7574 7075 7428 5b27 736b 7927  ck_output(['sky'
+00030d30: 2c20 2773 746f 7261 6765 272c 2027 6c73  , 'storage', 'ls
+00030d40: 275d 292e 6465 636f 6465 2827 7574 662d  ']).decode('utf-
+00030d50: 3827 290a 2020 2020 2020 2020 6173 7365  8').        asse
+00030d60: 7274 2073 746f 7261 6765 5f6e 616d 6520  rt storage_name 
+00030d70: 696e 206f 7574 2c20 6627 5374 6f72 6167  in out, f'Storag
+00030d80: 6520 7b73 746f 7261 6765 5f6e 616d 657d  e {storage_name}
+00030d90: 206e 6f74 2066 6f75 6e64 2069 6e20 736b   not found in sk
+00030da0: 7920 7374 6f72 6167 6520 6c73 2e27 0a0a  y storage ls.'..
+00030db0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00030dc0: 2e6e 6f5f 666c 7569 6473 7461 636b 0a20  .no_fluidstack. 
+00030dd0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
+00030de0: 7061 7261 6d65 7472 697a 6528 2773 746f  parametrize('sto
+00030df0: 7265 5f74 7970 6527 2c20 5b0a 2020 2020  re_type', [.    
+00030e00: 2020 2020 7374 6f72 6167 655f 6c69 622e      storage_lib.
+00030e10: 5374 6f72 6554 7970 652e 5333 2c20 7374  StoreType.S3, st
+00030e20: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+00030e30: 7970 652e 4743 532c 0a20 2020 2020 2020  ype.GCS,.       
+00030e40: 2070 7974 6573 742e 7061 7261 6d28 7374   pytest.param(st
+00030e50: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+00030e60: 7970 652e 4942 4d2c 206d 6172 6b73 3d70  ype.IBM, marks=p
+00030e70: 7974 6573 742e 6d61 726b 2e69 626d 292c  ytest.mark.ibm),
+00030e80: 0a20 2020 2020 2020 2070 7974 6573 742e  .        pytest.
+00030e90: 7061 7261 6d28 7374 6f72 6167 655f 6c69  param(storage_li
+00030ea0: 622e 5374 6f72 6554 7970 652e 5232 2c20  b.StoreType.R2, 
+00030eb0: 6d61 726b 733d 7079 7465 7374 2e6d 6172  marks=pytest.mar
+00030ec0: 6b2e 636c 6f75 6466 6c61 7265 290a 2020  k.cloudflare).  
+00030ed0: 2020 5d29 0a20 2020 2064 6566 2074 6573    ]).    def tes
+00030ee0: 745f 6c69 7374 5f73 6f75 7263 6528 7365  t_list_source(se
+00030ef0: 6c66 2c20 746d 705f 6c6f 6361 6c5f 6c69  lf, tmp_local_li
+00030f00: 7374 5f73 746f 7261 6765 5f6f 626a 2c20  st_storage_obj, 
+00030f10: 7374 6f72 655f 7479 7065 293a 0a20 2020  store_type):.   
+00030f20: 2020 2020 2023 2055 7365 7320 6120 6c69       # Uses a li
+00030f30: 7374 2069 6e20 7468 6520 736f 7572 6365  st in the source
+00030f40: 2066 6965 6c64 2074 6f20 7370 6563 6966   field to specif
+00030f50: 7920 6120 6669 6c65 2061 6e64 2061 2064  y a file and a d
+00030f60: 6972 6563 746f 7279 2074 6f0a 2020 2020  irectory to.    
+00030f70: 2020 2020 2320 6265 2075 706c 6f61 6465      # be uploade
+00030f80: 6420 746f 2074 6865 2073 746f 7261 6765  d to the storage
+00030f90: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00030fa0: 2074 6d70 5f6c 6f63 616c 5f6c 6973 745f   tmp_local_list_
+00030fb0: 7374 6f72 6167 655f 6f62 6a2e 6164 645f  storage_obj.add_
+00030fc0: 7374 6f72 6528 7374 6f72 655f 7479 7065  store(store_type
+00030fd0: 290a 0a20 2020 2020 2020 2023 2043 6865  )..        # Che
+00030fe0: 636b 2069 6620 746d 702d 6669 6c65 2065  ck if tmp-file e
+00030ff0: 7869 7374 7320 696e 2074 6865 2062 7563  xists in the buc
+00031000: 6b65 7420 726f 6f74 2075 7369 6e67 2063  ket root using c
+00031010: 6c69 0a20 2020 2020 2020 206f 7574 203d  li.        out =
+00031020: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
+00031030: 6b5f 6f75 7470 7574 2873 656c 662e 636c  k_output(self.cl
+00031040: 695f 6c73 5f63 6d64 280a 2020 2020 2020  i_ls_cmd(.      
+00031050: 2020 2020 2020 7374 6f72 655f 7479 7065        store_type
+00031060: 2c20 746d 705f 6c6f 6361 6c5f 6c69 7374  , tmp_local_list
+00031070: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+00031080: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
 00031090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000310a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000310b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000310c0: 2020 2020 2827 7574 662d 3827 2929 0a0a      ('utf-8'))..
-000310d0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-000310e0: 2e6e 6f5f 666c 7569 6473 7461 636b 0a20  .no_fluidstack. 
-000310f0: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00031100: 7061 7261 6d65 7472 697a 6528 2769 6e76  parametrize('inv
-00031110: 616c 6964 5f6e 616d 655f 6c69 7374 2c20  alid_name_list, 
-00031120: 7374 6f72 655f 7479 7065 272c 0a20 2020  store_type',.   
-00031130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031140: 2020 2020 2020 2020 2020 5b28 4157 535f            [(AWS_
-00031150: 494e 5641 4c49 445f 4e41 4d45 532c 2073  INVALID_NAMES, s
-00031160: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-00031170: 5479 7065 2e53 3329 2c0a 2020 2020 2020  Type.S3),.      
-00031180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031190: 2020 2020 2020 2020 2847 4353 5f49 4e56          (GCS_INV
-000311a0: 414c 4944 5f4e 414d 4553 2c20 7374 6f72  ALID_NAMES, stor
-000311b0: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-000311c0: 652e 4743 5329 2c0a 2020 2020 2020 2020  e.GCS),.        
-000311d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000311e0: 2020 2020 2020 7079 7465 7374 2e70 6172        pytest.par
-000311f0: 616d 2849 424d 5f49 4e56 414c 4944 5f4e  am(IBM_INVALID_N
-00031200: 414d 4553 2c0a 2020 2020 2020 2020 2020  AMES,.          
-00031210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031230: 2073 746f 7261 6765 5f6c 6962 2e53 746f   storage_lib.Sto
-00031240: 7265 5479 7065 2e49 424d 2c0a 2020 2020  reType.IBM,.    
+000310a0: 2020 2020 2020 2020 2020 7368 656c 6c3d            shell=
+000310b0: 5472 7565 290a 2020 2020 2020 2020 6173  True).        as
+000310c0: 7365 7274 2027 746d 702d 6669 6c65 2720  sert 'tmp-file' 
+000310d0: 696e 206f 7574 2e64 6563 6f64 6528 2775  in out.decode('u
+000310e0: 7466 2d38 2729 2c20 5c0a 2020 2020 2020  tf-8'), \.      
+000310f0: 2020 2020 2020 2746 696c 6520 6e6f 7420        'File not 
+00031100: 666f 756e 6420 696e 2062 7563 6b65 7420  found in bucket 
+00031110: 2d20 6f75 7470 7574 2077 6173 203a 207b  - output was : {
+00031120: 7d27 2e66 6f72 6d61 7428 6f75 742e 6465  }'.format(out.de
+00031130: 636f 6465 0a20 2020 2020 2020 2020 2020  code.           
+00031140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031170: 2020 2020 2028 2775 7466 2d38 2729 290a       ('utf-8')).
+00031180: 0a20 2020 2020 2020 2023 2043 6865 636b  .        # Check
+00031190: 2069 6620 746d 702d 6669 6c65 2065 7869   if tmp-file exi
+000311a0: 7374 7320 696e 2074 6865 2062 7563 6b65  sts in the bucke
+000311b0: 742f 746d 702d 736f 7572 6365 2075 7369  t/tmp-source usi
+000311c0: 6e67 2063 6c69 0a20 2020 2020 2020 206f  ng cli.        o
+000311d0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+000311e0: 6368 6563 6b5f 6f75 7470 7574 2873 656c  check_output(sel
+000311f0: 662e 636c 695f 6c73 5f63 6d64 280a 2020  f.cli_ls_cmd(.  
+00031200: 2020 2020 2020 2020 2020 7374 6f72 655f            store_
+00031210: 7479 7065 2c20 746d 705f 6c6f 6361 6c5f  type, tmp_local_
+00031220: 6c69 7374 5f73 746f 7261 6765 5f6f 626a  list_storage_obj
+00031230: 2e6e 616d 652c 2027 746d 702d 736f 7572  .name, 'tmp-sour
+00031240: 6365 2f27 292c 0a20 2020 2020 2020 2020  ce/'),.         
 00031250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031270: 2020 2020 2020 206d 6172 6b73 3d70 7974         marks=pyt
-00031280: 6573 742e 6d61 726b 2e69 626d 292c 0a20  est.mark.ibm),. 
-00031290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000312a0: 2020 2020 2020 2020 2020 2020 2070 7974               pyt
-000312b0: 6573 742e 7061 7261 6d28 4157 535f 494e  est.param(AWS_IN
-000312c0: 5641 4c49 445f 4e41 4d45 532c 0a20 2020  VALID_NAMES,.   
-000312d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000312e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000312f0: 2020 2020 2020 2020 7374 6f72 6167 655f          storage_
-00031300: 6c69 622e 5374 6f72 6554 7970 652e 5232  lib.StoreType.R2
-00031310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00031260: 2020 2020 2020 2020 2020 2020 2073 6865               she
+00031270: 6c6c 3d54 7275 6529 0a20 2020 2020 2020  ll=True).       
+00031280: 2061 7373 6572 7420 2774 6d70 2d66 696c   assert 'tmp-fil
+00031290: 6527 2069 6e20 6f75 742e 6465 636f 6465  e' in out.decode
+000312a0: 2827 7574 662d 3827 292c 205c 0a20 2020  ('utf-8'), \.   
+000312b0: 2020 2020 2020 2020 2027 4669 6c65 206e           'File n
+000312c0: 6f74 2066 6f75 6e64 2069 6e20 6275 636b  ot found in buck
+000312d0: 6574 202d 206f 7574 7075 7420 7761 7320  et - output was 
+000312e0: 3a20 7b7d 272e 666f 726d 6174 286f 7574  : {}'.format(out
+000312f0: 2e64 6563 6f64 650a 2020 2020 2020 2020  .decode.        
+00031300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00031320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031330: 2020 2020 2020 2020 2020 2020 206d 6172               mar
-00031340: 6b73 3d70 7974 6573 742e 6d61 726b 2e63  ks=pytest.mark.c
-00031350: 6c6f 7564 666c 6172 6529 5d29 0a20 2020  loudflare)]).   
-00031360: 2064 6566 2074 6573 745f 696e 7661 6c69   def test_invali
-00031370: 645f 6e61 6d65 7328 7365 6c66 2c20 696e  d_names(self, in
-00031380: 7661 6c69 645f 6e61 6d65 5f6c 6973 742c  valid_name_list,
-00031390: 2073 746f 7265 5f74 7970 6529 3a0a 2020   store_type):.  
-000313a0: 2020 2020 2020 2320 5573 6573 2061 206c        # Uses a l
-000313b0: 6973 7420 696e 2074 6865 2073 6f75 7263  ist in the sourc
-000313c0: 6520 6669 656c 6420 746f 2073 7065 6369  e field to speci
-000313d0: 6679 2061 2066 696c 6520 616e 6420 6120  fy a file and a 
-000313e0: 6469 7265 6374 6f72 7920 746f 0a20 2020  directory to.   
-000313f0: 2020 2020 2023 2062 6520 7570 6c6f 6164       # be upload
-00031400: 6564 2074 6f20 7468 6520 7374 6f72 6167  ed to the storag
-00031410: 6520 6f62 6a65 6374 2e0a 2020 2020 2020  e object..      
-00031420: 2020 666f 7220 6e61 6d65 2069 6e20 696e    for name in in
-00031430: 7661 6c69 645f 6e61 6d65 5f6c 6973 743a  valid_name_list:
-00031440: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00031450: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-00031460: 736b 792e 6578 6365 7074 696f 6e73 2e53  sky.exceptions.S
-00031470: 746f 7261 6765 4e61 6d65 4572 726f 7229  torageNameError)
-00031480: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00031490: 2020 7374 6f72 6167 655f 6f62 6a20 3d20    storage_obj = 
-000314a0: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
-000314b0: 6167 6528 6e61 6d65 3d6e 616d 6529 0a20  age(name=name). 
-000314c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000314d0: 746f 7261 6765 5f6f 626a 2e61 6464 5f73  torage_obj.add_s
-000314e0: 746f 7265 2873 746f 7265 5f74 7970 6529  tore(store_type)
-000314f0: 0a0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00031500: 726b 2e6e 6f5f 666c 7569 6473 7461 636b  rk.no_fluidstack
-00031510: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00031520: 6b2e 7061 7261 6d65 7472 697a 6528 0a20  k.parametrize(. 
-00031530: 2020 2020 2020 2027 6769 7469 676e 6f72         'gitignor
-00031540: 655f 7374 7275 6374 7572 652c 2073 746f  e_structure, sto
-00031550: 7265 5f74 7970 6527 2c0a 2020 2020 2020  re_type',.      
-00031560: 2020 5b28 4749 5449 474e 4f52 455f 5359    [(GITIGNORE_SY
-00031570: 4e43 5f54 4553 545f 4449 525f 5354 5255  NC_TEST_DIR_STRU
-00031580: 4354 5552 452c 2073 746f 7261 6765 5f6c  CTURE, storage_l
-00031590: 6962 2e53 746f 7265 5479 7065 2e53 3329  ib.StoreType.S3)
-000315a0: 2c0a 2020 2020 2020 2020 2028 4749 5449  ,.         (GITI
-000315b0: 474e 4f52 455f 5359 4e43 5f54 4553 545f  GNORE_SYNC_TEST_
-000315c0: 4449 525f 5354 5255 4354 5552 452c 2073  DIR_STRUCTURE, s
-000315d0: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
-000315e0: 5479 7065 2e47 4353 292c 0a20 2020 2020  Type.GCS),.     
-000315f0: 2020 2020 7079 7465 7374 2e70 6172 616d      pytest.param
-00031600: 2847 4954 4947 4e4f 5245 5f53 594e 435f  (GITIGNORE_SYNC_
-00031610: 5445 5354 5f44 4952 5f53 5452 5543 5455  TEST_DIR_STRUCTU
-00031620: 5245 2c0a 2020 2020 2020 2020 2020 2020  RE,.            
-00031630: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
-00031640: 655f 6c69 622e 5374 6f72 6554 7970 652e  e_lib.StoreType.
-00031650: 5232 2c0a 2020 2020 2020 2020 2020 2020  R2,.            
-00031660: 2020 2020 2020 2020 2020 6d61 726b 733d            marks=
-00031670: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
-00031680: 6466 6c61 7265 295d 290a 2020 2020 6465  dflare)]).    de
-00031690: 6620 7465 7374 5f65 7863 6c75 6465 645f  f test_excluded_
-000316a0: 6669 6c65 5f63 6c6f 7564 5f73 746f 7261  file_cloud_stora
-000316b0: 6765 5f75 706c 6f61 645f 636f 7079 2873  ge_upload_copy(s
-000316c0: 656c 662c 2067 6974 6967 6e6f 7265 5f73  elf, gitignore_s
-000316d0: 7472 7563 7475 7265 2c0a 2020 2020 2020  tructure,.      
-000316e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000316f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00031710: 746f 7265 5f74 7970 652c 0a20 2020 2020  tore_type,.     
-00031720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031750: 746d 705f 6769 7469 676e 6f72 655f 7374  tmp_gitignore_st
-00031760: 6f72 6167 655f 6f62 6a29 3a0a 2020 2020  orage_obj):.    
-00031770: 2020 2020 2320 7465 7374 7320 6966 2066      # tests if f
-00031780: 696c 6573 2069 6e63 6c75 6465 6420 696e  iles included in
-00031790: 202e 6769 7469 676e 6f72 6520 616e 6420   .gitignore and 
-000317a0: 2e67 6974 2f69 6e66 6f2f 6578 636c 7564  .git/info/exclud
-000317b0: 6520 6172 650a 2020 2020 2020 2020 2320  e are.        # 
-000317c0: 6578 636c 7564 6564 2066 726f 6d20 6265  excluded from be
-000317d0: 696e 6720 7472 616e 7366 6572 7265 6420  ing transferred 
-000317e0: 746f 2053 746f 7261 6765 0a0a 2020 2020  to Storage..    
-000317f0: 2020 2020 746d 705f 6769 7469 676e 6f72      tmp_gitignor
-00031800: 655f 7374 6f72 6167 655f 6f62 6a2e 6164  e_storage_obj.ad
-00031810: 645f 7374 6f72 6528 7374 6f72 655f 7479  d_store(store_ty
-00031820: 7065 290a 0a20 2020 2020 2020 2075 706c  pe)..        upl
-00031830: 6f61 645f 6669 6c65 5f6e 616d 6520 3d20  oad_file_name = 
-00031840: 2769 6e63 6c75 6465 6427 0a20 2020 2020  'included'.     
-00031850: 2020 2023 2043 6f75 6e74 2074 6865 206e     # Count the n
-00031860: 756d 6265 7220 6f66 2066 696c 6573 2077  umber of files w
-00031870: 6974 6820 7468 6520 6769 7665 6e20 6669  ith the given fi
-00031880: 6c65 206e 616d 650a 2020 2020 2020 2020  le name.        
-00031890: 7570 5f63 6d64 203d 2073 656c 662e 636c  up_cmd = self.cl
-000318a0: 695f 636f 756e 745f 6e61 6d65 5f69 6e5f  i_count_name_in_
-000318b0: 6275 636b 6574 2873 746f 7265 5f74 7970  bucket(store_typ
-000318c0: 652c 205c 0a20 2020 2020 2020 2020 2020  e, \.           
-000318d0: 2074 6d70 5f67 6974 6967 6e6f 7265 5f73   tmp_gitignore_s
-000318e0: 746f 7261 6765 5f6f 626a 2e6e 616d 652c  torage_obj.name,
-000318f0: 2066 696c 655f 6e61 6d65 3d75 706c 6f61   file_name=uploa
-00031900: 645f 6669 6c65 5f6e 616d 6529 0a20 2020  d_file_name).   
-00031910: 2020 2020 2067 6974 5f65 7863 6c75 6465       git_exclude
-00031920: 5f63 6d64 203d 2073 656c 662e 636c 695f  _cmd = self.cli_
-00031930: 636f 756e 745f 6e61 6d65 5f69 6e5f 6275  count_name_in_bu
-00031940: 636b 6574 2873 746f 7265 5f74 7970 652c  cket(store_type,
-00031950: 205c 0a20 2020 2020 2020 2020 2020 2074   \.            t
-00031960: 6d70 5f67 6974 6967 6e6f 7265 5f73 746f  mp_gitignore_sto
-00031970: 7261 6765 5f6f 626a 2e6e 616d 652c 2066  rage_obj.name, f
-00031980: 696c 655f 6e61 6d65 3d27 2e67 6974 2729  ile_name='.git')
-00031990: 0a20 2020 2020 2020 2063 6e74 5f6e 756d  .        cnt_num
-000319a0: 5f66 696c 655f 636d 6420 3d20 7365 6c66  _file_cmd = self
-000319b0: 2e63 6c69 5f63 6f75 6e74 5f66 696c 655f  .cli_count_file_
-000319c0: 696e 5f62 7563 6b65 7428 0a20 2020 2020  in_bucket(.     
-000319d0: 2020 2020 2020 2073 746f 7265 5f74 7970         store_typ
-000319e0: 652c 2074 6d70 5f67 6974 6967 6e6f 7265  e, tmp_gitignore
-000319f0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-00031a00: 6529 0a0a 2020 2020 2020 2020 7570 5f6f  e)..        up_o
-00031a10: 7574 7075 7420 3d20 7375 6270 726f 6365  utput = subproce
-00031a20: 7373 2e63 6865 636b 5f6f 7574 7075 7428  ss.check_output(
-00031a30: 7570 5f63 6d64 2c20 7368 656c 6c3d 5472  up_cmd, shell=Tr
-00031a40: 7565 290a 2020 2020 2020 2020 6769 745f  ue).        git_
-00031a50: 6578 636c 7564 655f 6f75 7470 7574 203d  exclude_output =
-00031a60: 2073 7562 7072 6f63 6573 732e 6368 6563   subprocess.chec
-00031a70: 6b5f 6f75 7470 7574 2867 6974 5f65 7863  k_output(git_exc
-00031a80: 6c75 6465 5f63 6d64 2c0a 2020 2020 2020  lude_cmd,.      
-00031a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031ab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00031ac0: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
-00031ad0: 2020 2063 6e74 5f6f 7574 7075 7420 3d20     cnt_output = 
-00031ae0: 7375 6270 726f 6365 7373 2e63 6865 636b  subprocess.check
-00031af0: 5f6f 7574 7075 7428 636e 745f 6e75 6d5f  _output(cnt_num_
-00031b00: 6669 6c65 5f63 6d64 2c20 7368 656c 6c3d  file_cmd, shell=
-00031b10: 5472 7565 290a 0a20 2020 2020 2020 2061  True)..        a
-00031b20: 7373 6572 7420 2733 2720 696e 2075 705f  ssert '3' in up_
-00031b30: 6f75 7470 7574 2e64 6563 6f64 6528 2775  output.decode('u
-00031b40: 7466 2d38 2729 2c20 5c0a 2020 2020 2020  tf-8'), \.      
-00031b50: 2020 2020 2020 2020 2020 2746 696c 6573            'Files
-00031b60: 2074 6f20 6265 2069 6e63 6c75 6465 6420   to be included 
-00031b70: 6172 6520 6e6f 7420 636f 6d70 6c65 7465  are not complete
-00031b80: 6c79 2075 706c 6f61 6465 642e 270a 2020  ly uploaded.'.  
-00031b90: 2020 2020 2020 2320 3120 6973 2072 6561        # 1 is rea
-00031ba0: 6420 6173 202e 6769 7469 676e 6f72 6520  d as .gitignore 
-00031bb0: 6973 2075 706c 6f61 6465 640a 2020 2020  is uploaded.    
-00031bc0: 2020 2020 6173 7365 7274 2027 3127 2069      assert '1' i
-00031bd0: 6e20 6769 745f 6578 636c 7564 655f 6f75  n git_exclude_ou
-00031be0: 7470 7574 2e64 6563 6f64 6528 2775 7466  tput.decode('utf
-00031bf0: 2d38 2729 2c20 5c0a 2020 2020 2020 2020  -8'), \.        
-00031c00: 2020 2020 2020 2027 2e67 6974 2064 6972         '.git dir
-00031c10: 6563 746f 7279 2073 686f 756c 6420 6e6f  ectory should no
-00031c20: 7420 6265 2075 706c 6f61 6465 642e 270a  t be uploaded.'.
-00031c30: 2020 2020 2020 2020 2320 3420 6669 6c65          # 4 file
-00031c40: 7320 696e 636c 7564 6520 2e67 6974 6967  s include .gitig
-00031c50: 6e6f 7265 2c20 696e 636c 7564 6564 2e6c  nore, included.l
-00031c60: 6f67 2c20 696e 636c 7564 6564 2e74 7874  og, included.txt
-00031c70: 2c20 696e 636c 7564 655f 6469 722f 696e  , include_dir/in
-00031c80: 636c 7564 6564 2e6c 6f67 0a20 2020 2020  cluded.log.     
-00031c90: 2020 2061 7373 6572 7420 2734 2720 696e     assert '4' in
-00031ca0: 2063 6e74 5f6f 7574 7075 742e 6465 636f   cnt_output.deco
-00031cb0: 6465 2827 7574 662d 3827 292c 205c 0a20  de('utf-8'), \. 
-00031cc0: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00031cd0: 6f6d 6520 6974 656d 7320 6c69 7374 6564  ome items listed
-00031ce0: 2069 6e20 2e67 6974 6967 6e6f 7265 2061   in .gitignore a
-00031cf0: 6e64 202e 6769 742f 696e 666f 2f65 7863  nd .git/info/exc
-00031d00: 6c75 6465 2061 7265 206e 6f74 2065 7863  lude are not exc
-00031d10: 6c75 6465 642e 270a 0a20 2020 2040 7079  luded.'..    @py
-00031d20: 7465 7374 2e6d 6172 6b2e 7061 7261 6d65  test.mark.parame
-00031d30: 7472 697a 6528 2765 7874 5f62 7563 6b65  trize('ext_bucke
-00031d40: 745f 6669 7874 7572 652c 2073 746f 7265  t_fixture, store
-00031d50: 5f74 7970 6527 2c0a 2020 2020 2020 2020  _type',.        
-00031d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031d70: 2020 2020 205b 2827 746d 705f 6177 7363       [('tmp_awsc
-00031d80: 6c69 5f62 7563 6b65 7427 2c20 7374 6f72  li_bucket', stor
-00031d90: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
-00031da0: 652e 5333 292c 0a20 2020 2020 2020 2020  e.S3),.         
-00031db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031dc0: 2020 2020 2028 2774 6d70 5f67 7375 7469       ('tmp_gsuti
-00031dd0: 6c5f 6275 636b 6574 272c 2073 746f 7261  l_bucket', stora
-00031de0: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
-00031df0: 2e47 4353 292c 0a20 2020 2020 2020 2020  .GCS),.         
-00031e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031e10: 2020 2020 2070 7974 6573 742e 7061 7261       pytest.para
-00031e20: 6d28 2774 6d70 5f61 7773 636c 695f 6275  m('tmp_awscli_bu
-00031e30: 636b 6574 5f72 3227 2c0a 2020 2020 2020  cket_r2',.      
-00031e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031e60: 2020 2020 2073 746f 7261 6765 5f6c 6962       storage_lib
-00031e70: 2e53 746f 7265 5479 7065 2e52 322c 0a20  .StoreType.R2,. 
-00031e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00031ea0: 2020 2020 2020 2020 2020 6d61 726b 733d            marks=
-00031eb0: 7079 7465 7374 2e6d 6172 6b2e 636c 6f75  pytest.mark.clou
-00031ec0: 6466 6c61 7265 295d 290a 2020 2020 6465  dflare)]).    de
-00031ed0: 6620 7465 7374 5f65 7874 6572 6e61 6c6c  f test_externall
-00031ee0: 795f 6372 6561 7465 645f 6275 636b 6574  y_created_bucket
-00031ef0: 5f6d 6f75 6e74 5f77 6974 686f 7574 5f73  _mount_without_s
-00031f00: 6f75 7263 6528 0a20 2020 2020 2020 2020  ource(.         
-00031f10: 2020 2073 656c 662c 2065 7874 5f62 7563     self, ext_buc
-00031f20: 6b65 745f 6669 7874 7572 652c 2072 6571  ket_fixture, req
-00031f30: 7565 7374 2c20 7374 6f72 655f 7479 7065  uest, store_type
-00031f40: 293a 0a20 2020 2020 2020 2023 204e 6f6e  ):.        # Non
-00031f50: 2d73 6b79 206d 616e 6167 6564 2062 7563  -sky managed buc
-00031f60: 6b65 7473 2862 7563 6b65 7473 2063 7265  kets(buckets cre
-00031f70: 6174 6564 206f 7574 7369 6465 206f 6620  ated outside of 
-00031f80: 536b 7970 696c 6f74 2043 4c49 290a 2020  Skypilot CLI).  
-00031f90: 2020 2020 2020 2320 6172 6520 616c 6c6f        # are allo
-00031fa0: 7765 6420 746f 2062 6520 4d4f 554e 5465  wed to be MOUNTe
-00031fb0: 6420 6279 2073 7065 6369 6679 696e 6720  d by specifying 
-00031fc0: 7468 6520 5552 4920 6f66 2074 6865 2062  the URI of the b
-00031fd0: 7563 6b65 7420 746f 0a20 2020 2020 2020  ucket to.       
-00031fe0: 2023 2073 6f75 7263 6520 6669 656c 6420   # source field 
-00031ff0: 6f6e 6c79 2e20 5768 656e 2069 7420 6973  only. When it is
-00032000: 2061 7474 656d 7074 6564 2062 7920 7370   attempted by sp
-00032010: 6563 6966 7969 6e67 2074 6865 206e 616d  ecifying the nam
-00032020: 6520 6f66 0a20 2020 2020 2020 2023 2074  e of.        # t
-00032030: 6865 2062 7563 6b65 7420 6f6e 6c79 2c20  he bucket only, 
-00032040: 6974 2073 686f 756c 6420 6572 726f 7220  it should error 
-00032050: 6f75 742e 0a20 2020 2020 2020 2023 0a20  out..        #. 
-00032060: 2020 2020 2020 2023 2054 4f44 4f28 646f         # TODO(do
-00032070: 796f 756e 6729 3a20 4164 6420 7465 7374  young): Add test
-00032080: 2066 6f72 2049 424d 2043 4f53 2e20 4375   for IBM COS. Cu
-00032090: 7272 656e 746c 792c 2074 6869 7320 6973  rrently, this is
-000320a0: 2062 6c6f 636b 6564 0a20 2020 2020 2020   blocked.       
-000320b0: 2023 2061 7320 7263 6c6f 6e65 2075 7365   # as rclone use
-000320c0: 6420 746f 2069 6e74 6572 6163 7420 7769  d to interact wi
-000320d0: 7468 2049 424d 2043 4f53 2064 6f65 7320  th IBM COS does 
-000320e0: 6e6f 7420 7375 7070 6f72 7420 6665 6174  not support feat
-000320f0: 7572 6520 746f 0a20 2020 2020 2020 2023  ure to.        #
-00032100: 2063 7265 6174 6520 6120 6275 636b 6574   create a bucket
-00032110: 2c20 616e 6420 7468 6520 6962 6d63 6c6f  , and the ibmclo
-00032120: 7564 2043 4c49 2069 7320 6e6f 7420 7375  ud CLI is not su
-00032130: 7070 6f72 7465 6420 696e 2053 6b79 7069  pported in Skypi
-00032140: 6c6f 742e 0a20 2020 2020 2020 2023 2045  lot..        # E
-00032150: 6974 6865 7220 6f66 2074 6865 2066 6561  ither of the fea
-00032160: 7475 7265 2069 7320 6e65 6365 7373 6172  ture is necessar
-00032170: 7920 746f 2073 696d 756c 6174 6520 616e  y to simulate an
-00032180: 2065 7874 6572 6e61 6c20 6275 636b 6574   external bucket
-00032190: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
-000321a0: 696f 6e20 666f 7220 4942 4d20 434f 532e  ion for IBM COS.
-000321b0: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-000321c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 736b  ://github.com/sk
-000321d0: 7970 696c 6f74 2d6f 7267 2f73 6b79 7069  ypilot-org/skypi
-000321e0: 6c6f 742f 7075 6c6c 2f31 3936 362f 6669  lot/pull/1966/fi
-000321f0: 6c65 7323 7231 3235 3334 3339 3833 370a  les#r1253439837.
-00032200: 0a20 2020 2020 2020 2065 7874 5f62 7563  .        ext_buc
-00032210: 6b65 745f 6e61 6d65 2c20 6578 745f 6275  ket_name, ext_bu
-00032220: 636b 6574 5f75 7269 203d 2072 6571 7565  cket_uri = reque
-00032230: 7374 2e67 6574 6669 7874 7572 6576 616c  st.getfixtureval
-00032240: 7565 280a 2020 2020 2020 2020 2020 2020  ue(.            
-00032250: 6578 745f 6275 636b 6574 5f66 6978 7475  ext_bucket_fixtu
-00032260: 7265 290a 2020 2020 2020 2020 2320 696e  re).        # in
-00032270: 7661 6c69 6420 7370 6563 0a20 2020 2020  valid spec.     
-00032280: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
-00032290: 6169 7365 7328 736b 792e 6578 6365 7074  aises(sky.except
-000322a0: 696f 6e73 2e53 746f 7261 6765 5370 6563  ions.StorageSpec
-000322b0: 4572 726f 7229 2061 7320 653a 0a20 2020  Error) as e:.   
-000322c0: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-000322d0: 5f6f 626a 203d 2073 746f 7261 6765 5f6c  _obj = storage_l
-000322e0: 6962 2e53 746f 7261 6765 280a 2020 2020  ib.Storage(.    
-000322f0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00032300: 3d65 7874 5f62 7563 6b65 745f 6e61 6d65  =ext_bucket_name
-00032310: 2c20 6d6f 6465 3d73 746f 7261 6765 5f6c  , mode=storage_l
-00032320: 6962 2e53 746f 7261 6765 4d6f 6465 2e4d  ib.StorageMode.M
-00032330: 4f55 4e54 290a 2020 2020 2020 2020 2020  OUNT).          
-00032340: 2020 7374 6f72 6167 655f 6f62 6a2e 6164    storage_obj.ad
-00032350: 645f 7374 6f72 6528 7374 6f72 655f 7479  d_store(store_ty
-00032360: 7065 290a 0a20 2020 2020 2020 2061 7373  pe)..        ass
-00032370: 6572 7420 2741 7474 656d 7074 6564 2074  ert 'Attempted t
-00032380: 6f20 6d6f 756e 7420 6120 6e6f 6e2d 736b  o mount a non-sk
-00032390: 7920 6d61 6e61 6765 6420 6275 636b 6574  y managed bucket
-000323a0: 2720 696e 2073 7472 2865 290a 0a20 2020  ' in str(e)..   
-000323b0: 2020 2020 2023 2076 616c 6964 2073 7065       # valid spe
-000323c0: 630a 2020 2020 2020 2020 7374 6f72 6167  c.        storag
-000323d0: 655f 6f62 6a20 3d20 7374 6f72 6167 655f  e_obj = storage_
-000323e0: 6c69 622e 5374 6f72 6167 6528 736f 7572  lib.Storage(sour
-000323f0: 6365 3d65 7874 5f62 7563 6b65 745f 7572  ce=ext_bucket_ur
-00032400: 692c 0a20 2020 2020 2020 2020 2020 2020  i,.             
-00032410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00032420: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00032430: 653d 7374 6f72 6167 655f 6c69 622e 5374  e=storage_lib.St
-00032440: 6f72 6167 654d 6f64 652e 4d4f 554e 5429  orageMode.MOUNT)
-00032450: 0a20 2020 2020 2020 2068 616e 646c 6520  .        handle 
-00032460: 3d20 676c 6f62 616c 5f75 7365 725f 7374  = global_user_st
-00032470: 6174 652e 6765 745f 6861 6e64 6c65 5f66  ate.get_handle_f
-00032480: 726f 6d5f 7374 6f72 6167 655f 6e61 6d65  rom_storage_name
-00032490: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-000324a0: 6f72 6167 655f 6f62 6a2e 6e61 6d65 290a  orage_obj.name).
-000324b0: 2020 2020 2020 2020 6966 2068 616e 646c          if handl
-000324c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000324d0: 746f 7261 6765 5f6f 626a 2e64 656c 6574  torage_obj.delet
-000324e0: 6528 290a 0a20 2020 2040 7079 7465 7374  e()..    @pytest
-000324f0: 2e6d 6172 6b2e 6e6f 5f66 6c75 6964 7374  .mark.no_fluidst
-00032500: 6163 6b0a 2020 2020 4070 7974 6573 742e  ack.    @pytest.
-00032510: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00032520: 2827 7265 6769 6f6e 272c 205b 0a20 2020  ('region', [.   
-00032530: 2020 2020 2027 6170 2d6e 6f72 7468 6561       'ap-northea
-00032540: 7374 2d31 272c 2027 6170 2d6e 6f72 7468  st-1', 'ap-north
-00032550: 6561 7374 2d32 272c 2027 6170 2d6e 6f72  east-2', 'ap-nor
-00032560: 7468 6561 7374 2d33 272c 2027 6170 2d73  theast-3', 'ap-s
-00032570: 6f75 7468 2d31 272c 0a20 2020 2020 2020  outh-1',.       
-00032580: 2027 6170 2d73 6f75 7468 6561 7374 2d31   'ap-southeast-1
-00032590: 272c 2027 6170 2d73 6f75 7468 6561 7374  ', 'ap-southeast
-000325a0: 2d32 272c 2027 6575 2d63 656e 7472 616c  -2', 'eu-central
-000325b0: 2d31 272c 2027 6575 2d6e 6f72 7468 2d31  -1', 'eu-north-1
-000325c0: 272c 0a20 2020 2020 2020 2027 6575 2d77  ',.        'eu-w
-000325d0: 6573 742d 3127 2c20 2765 752d 7765 7374  est-1', 'eu-west
-000325e0: 2d32 272c 2027 6575 2d77 6573 742d 3327  -2', 'eu-west-3'
-000325f0: 2c20 2773 612d 6561 7374 2d31 272c 2027  , 'sa-east-1', '
-00032600: 7573 2d65 6173 742d 3127 2c0a 2020 2020  us-east-1',.    
-00032610: 2020 2020 2775 732d 6561 7374 2d32 272c      'us-east-2',
-00032620: 2027 7573 2d77 6573 742d 3127 2c20 2775   'us-west-1', 'u
-00032630: 732d 7765 7374 2d32 270a 2020 2020 5d29  s-west-2'.    ])
-00032640: 0a20 2020 2064 6566 2074 6573 745f 6177  .    def test_aw
-00032650: 735f 7265 6769 6f6e 7328 7365 6c66 2c20  s_regions(self, 
-00032660: 746d 705f 6c6f 6361 6c5f 7374 6f72 6167  tmp_local_storag
-00032670: 655f 6f62 6a2c 2072 6567 696f 6e29 3a0a  e_obj, region):.
-00032680: 2020 2020 2020 2020 2320 5468 6973 2074          # This t
-00032690: 6573 7473 2063 7265 6174 696f 6e20 616e  ests creation an
-000326a0: 6420 7570 6c6f 6164 2074 6f20 6275 636b  d upload to buck
-000326b0: 6574 2069 6e20 616c 6c20 4157 5320 7333  et in all AWS s3
-000326c0: 2072 6567 696f 6e73 0a20 2020 2020 2020   regions.       
-000326d0: 2023 2054 6f20 7465 7374 2066 756c 6c20   # To test full 
-000326e0: 6675 6e63 7469 6f6e 616c 6974 792c 2075  functionality, u
-000326f0: 7365 2074 6573 745f 6d61 6e61 6765 645f  se test_managed_
-00032700: 6a6f 6273 5f73 746f 7261 6765 2061 626f  jobs_storage abo
-00032710: 7665 2e0a 2020 2020 2020 2020 7374 6f72  ve..        stor
-00032720: 655f 7479 7065 203d 2073 746f 7261 6765  e_type = storage
-00032730: 5f6c 6962 2e53 746f 7265 5479 7065 2e53  _lib.StoreType.S
-00032740: 330a 2020 2020 2020 2020 746d 705f 6c6f  3.        tmp_lo
-00032750: 6361 6c5f 7374 6f72 6167 655f 6f62 6a2e  cal_storage_obj.
-00032760: 6164 645f 7374 6f72 6528 7374 6f72 655f  add_store(store_
-00032770: 7479 7065 2c20 7265 6769 6f6e 3d72 6567  type, region=reg
-00032780: 696f 6e29 0a20 2020 2020 2020 2062 7563  ion).        buc
-00032790: 6b65 745f 6e61 6d65 203d 2074 6d70 5f6c  ket_name = tmp_l
-000327a0: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
-000327b0: 2e6e 616d 650a 0a20 2020 2020 2020 2023  .name..        #
-000327c0: 2043 6f6e 6669 726d 2074 6861 7420 7468   Confirm that th
-000327d0: 6520 6275 636b 6574 2077 6173 2063 7265  e bucket was cre
-000327e0: 6174 6564 2069 6e20 7468 6520 636f 7272  ated in the corr
-000327f0: 6563 7420 7265 6769 6f6e 0a20 2020 2020  ect region.     
-00032800: 2020 2072 6567 696f 6e5f 636d 6420 3d20     region_cmd = 
-00032810: 7365 6c66 2e63 6c69 5f72 6567 696f 6e5f  self.cli_region_
-00032820: 636d 6428 7374 6f72 655f 7479 7065 2c20  cmd(store_type, 
-00032830: 6275 636b 6574 5f6e 616d 6529 0a20 2020  bucket_name).   
-00032840: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
-00032850: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
-00032860: 7574 2872 6567 696f 6e5f 636d 642c 2073  ut(region_cmd, s
-00032870: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
-00032880: 2020 206f 7574 7075 7420 3d20 6f75 742e     output = out.
-00032890: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
-000328a0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-000328b0: 5f6f 7574 7075 745f 7265 6769 6f6e 203d  _output_region =
-000328c0: 2072 6567 696f 6e0a 2020 2020 2020 2020   region.        
-000328d0: 6966 2072 6567 696f 6e20 3d3d 2027 7573  if region == 'us
-000328e0: 2d65 6173 742d 3127 3a0a 2020 2020 2020  -east-1':.      
-000328f0: 2020 2020 2020 6578 7065 6374 6564 5f6f        expected_o
-00032900: 7574 7075 745f 7265 6769 6f6e 203d 2027  utput_region = '
-00032910: 4e6f 6e65 2720 2023 2075 732d 6561 7374  None'  # us-east
-00032920: 2d31 2069 7320 7468 6520 6465 6661 756c  -1 is the defaul
-00032930: 7420 7265 6769 6f6e 0a20 2020 2020 2020  t region.       
-00032940: 2061 7373 6572 7420 6578 7065 6374 6564   assert expected
-00032950: 5f6f 7574 7075 745f 7265 6769 6f6e 2069  _output_region i
-00032960: 6e20 6f75 742e 6465 636f 6465 2827 7574  n out.decode('ut
-00032970: 662d 3827 292c 2028 0a20 2020 2020 2020  f-8'), (.       
-00032980: 2020 2020 2066 2742 7563 6b65 7420 7761       f'Bucket wa
-00032990: 7320 6e6f 7420 666f 756e 6420 696e 2072  s not found in r
-000329a0: 6567 696f 6e20 7b72 6567 696f 6e7d 202d  egion {region} -
-000329b0: 2027 0a20 2020 2020 2020 2020 2020 2066   '.            f
-000329c0: 276f 7574 7075 7420 6f66 207b 7265 6769  'output of {regi
-000329d0: 6f6e 5f63 6d64 7d20 7761 733a 207b 6f75  on_cmd} was: {ou
-000329e0: 7470 7574 7d27 290a 0a20 2020 2020 2020  tput}')..       
-000329f0: 2023 2043 6865 636b 2069 6620 746d 705f   # Check if tmp_
-00032a00: 736f 7572 6365 2f74 6d70 2d66 696c 6520  source/tmp-file 
-00032a10: 6578 6973 7473 2069 6e20 7468 6520 6275  exists in the bu
-00032a20: 636b 6574 2075 7369 6e67 2063 6c69 0a20  cket using cli. 
-00032a30: 2020 2020 2020 206c 735f 636d 6420 3d20         ls_cmd = 
-00032a40: 7365 6c66 2e63 6c69 5f6c 735f 636d 6428  self.cli_ls_cmd(
-00032a50: 7374 6f72 655f 7479 7065 2c20 6275 636b  store_type, buck
-00032a60: 6574 5f6e 616d 6529 0a20 2020 2020 2020  et_name).       
-00032a70: 206f 7574 203d 2073 7562 7072 6f63 6573   out = subproces
-00032a80: 732e 6368 6563 6b5f 6f75 7470 7574 286c  s.check_output(l
-00032a90: 735f 636d 642c 2073 6865 6c6c 3d54 7275  s_cmd, shell=Tru
-00032aa0: 6529 0a20 2020 2020 2020 206f 7574 7075  e).        outpu
-00032ab0: 7420 3d20 6f75 742e 6465 636f 6465 2827  t = out.decode('
-00032ac0: 7574 662d 3827 290a 2020 2020 2020 2020  utf-8').        
-00032ad0: 6173 7365 7274 2027 746d 702d 6669 6c65  assert 'tmp-file
-00032ae0: 2720 696e 206f 7574 7075 742c 2028 0a20  ' in output, (. 
-00032af0: 2020 2020 2020 2020 2020 2066 2774 6d70             f'tmp
-00032b00: 2d66 696c 6520 6e6f 7420 666f 756e 6420  -file not found 
-00032b10: 696e 2062 7563 6b65 7420 2d20 6f75 7470  in bucket - outp
-00032b20: 7574 206f 6620 7b6c 735f 636d 647d 2077  ut of {ls_cmd} w
-00032b30: 6173 3a20 7b6f 7574 7075 747d 2729 0a0a  as: {output}')..
-00032b40: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00032b50: 2e6e 6f5f 666c 7569 6473 7461 636b 0a20  .no_fluidstack. 
-00032b60: 2020 2040 7079 7465 7374 2e6d 6172 6b2e     @pytest.mark.
-00032b70: 7061 7261 6d65 7472 697a 6528 2772 6567  parametrize('reg
-00032b80: 696f 6e27 2c20 5b0a 2020 2020 2020 2020  ion', [.        
-00032b90: 276e 6f72 7468 616d 6572 6963 612d 6e6f  'northamerica-no
-00032ba0: 7274 6865 6173 7431 272c 2027 6e6f 7274  rtheast1', 'nort
-00032bb0: 6861 6d65 7269 6361 2d6e 6f72 7468 6561  hamerica-northea
-00032bc0: 7374 3227 2c20 2775 732d 6365 6e74 7261  st2', 'us-centra
-00032bd0: 6c31 272c 0a20 2020 2020 2020 2027 7573  l1',.        'us
-00032be0: 2d65 6173 7431 272c 2027 7573 2d65 6173  -east1', 'us-eas
-00032bf0: 7434 272c 2027 7573 2d65 6173 7435 272c  t4', 'us-east5',
-00032c00: 2027 7573 2d73 6f75 7468 3127 2c20 2775   'us-south1', 'u
-00032c10: 732d 7765 7374 3127 2c20 2775 732d 7765  s-west1', 'us-we
-00032c20: 7374 3227 2c0a 2020 2020 2020 2020 2775  st2',.        'u
-00032c30: 732d 7765 7374 3327 2c20 2775 732d 7765  s-west3', 'us-we
-00032c40: 7374 3427 2c20 2773 6f75 7468 616d 6572  st4', 'southamer
-00032c50: 6963 612d 6561 7374 3127 2c20 2773 6f75  ica-east1', 'sou
-00032c60: 7468 616d 6572 6963 612d 7765 7374 3127  thamerica-west1'
-00032c70: 2c0a 2020 2020 2020 2020 2765 7572 6f70  ,.        'europ
-00032c80: 652d 6365 6e74 7261 6c32 272c 2027 6575  e-central2', 'eu
-00032c90: 726f 7065 2d6e 6f72 7468 3127 2c20 2765  rope-north1', 'e
-00032ca0: 7572 6f70 652d 736f 7574 6877 6573 7431  urope-southwest1
-00032cb0: 272c 2027 6575 726f 7065 2d77 6573 7431  ', 'europe-west1
-00032cc0: 272c 0a20 2020 2020 2020 2027 6575 726f  ',.        'euro
-00032cd0: 7065 2d77 6573 7432 272c 2027 6575 726f  pe-west2', 'euro
-00032ce0: 7065 2d77 6573 7433 272c 2027 6575 726f  pe-west3', 'euro
-00032cf0: 7065 2d77 6573 7434 272c 2027 6575 726f  pe-west4', 'euro
-00032d00: 7065 2d77 6573 7436 272c 0a20 2020 2020  pe-west6',.     
-00032d10: 2020 2027 6575 726f 7065 2d77 6573 7438     'europe-west8
-00032d20: 272c 2027 6575 726f 7065 2d77 6573 7439  ', 'europe-west9
-00032d30: 272c 2027 6575 726f 7065 2d77 6573 7431  ', 'europe-west1
-00032d40: 3027 2c20 2765 7572 6f70 652d 7765 7374  0', 'europe-west
-00032d50: 3132 272c 0a20 2020 2020 2020 2027 6173  12',.        'as
-00032d60: 6961 2d65 6173 7431 272c 2027 6173 6961  ia-east1', 'asia
-00032d70: 2d65 6173 7432 272c 2027 6173 6961 2d6e  -east2', 'asia-n
-00032d80: 6f72 7468 6561 7374 3127 2c20 2761 7369  ortheast1', 'asi
-00032d90: 612d 6e6f 7274 6865 6173 7432 272c 0a20  a-northeast2',. 
-00032da0: 2020 2020 2020 2027 6173 6961 2d6e 6f72         'asia-nor
-00032db0: 7468 6561 7374 3327 2c20 2761 7369 612d  theast3', 'asia-
-00032dc0: 736f 7574 6865 6173 7431 272c 2027 6173  southeast1', 'as
-00032dd0: 6961 2d73 6f75 7468 3127 2c20 2761 7369  ia-south1', 'asi
-00032de0: 612d 736f 7574 6832 272c 0a20 2020 2020  a-south2',.     
-00032df0: 2020 2027 6173 6961 2d73 6f75 7468 6561     'asia-southea
-00032e00: 7374 3227 2c20 276d 652d 6365 6e74 7261  st2', 'me-centra
-00032e10: 6c31 272c 2027 6d65 2d63 656e 7472 616c  l1', 'me-central
-00032e20: 3227 2c20 276d 652d 7765 7374 3127 2c0a  2', 'me-west1',.
-00032e30: 2020 2020 2020 2020 2761 7573 7472 616c          'austral
-00032e40: 6961 2d73 6f75 7468 6561 7374 3127 2c20  ia-southeast1', 
-00032e50: 2761 7573 7472 616c 6961 2d73 6f75 7468  'australia-south
-00032e60: 6561 7374 3227 2c20 2761 6672 6963 612d  east2', 'africa-
-00032e70: 736f 7574 6831 270a 2020 2020 5d29 0a20  south1'.    ]). 
-00032e80: 2020 2064 6566 2074 6573 745f 6763 735f     def test_gcs_
-00032e90: 7265 6769 6f6e 7328 7365 6c66 2c20 746d  regions(self, tm
-00032ea0: 705f 6c6f 6361 6c5f 7374 6f72 6167 655f  p_local_storage_
-00032eb0: 6f62 6a2c 2072 6567 696f 6e29 3a0a 2020  obj, region):.  
-00032ec0: 2020 2020 2020 2320 5468 6973 2074 6573        # This tes
-00032ed0: 7473 2063 7265 6174 696f 6e20 616e 6420  ts creation and 
-00032ee0: 7570 6c6f 6164 2074 6f20 6275 636b 6574  upload to bucket
-00032ef0: 2069 6e20 616c 6c20 4743 5320 7265 6769   in all GCS regi
-00032f00: 6f6e 730a 2020 2020 2020 2020 2320 546f  ons.        # To
-00032f10: 2074 6573 7420 6675 6c6c 2066 756e 6374   test full funct
-00032f20: 696f 6e61 6c69 7479 2c20 7573 6520 7465  ionality, use te
-00032f30: 7374 5f6d 616e 6167 6564 5f6a 6f62 735f  st_managed_jobs_
-00032f40: 7374 6f72 6167 6520 6162 6f76 652e 0a20  storage above.. 
-00032f50: 2020 2020 2020 2073 746f 7265 5f74 7970         store_typ
-00032f60: 6520 3d20 7374 6f72 6167 655f 6c69 622e  e = storage_lib.
-00032f70: 5374 6f72 6554 7970 652e 4743 530a 2020  StoreType.GCS.  
-00032f80: 2020 2020 2020 746d 705f 6c6f 6361 6c5f        tmp_local_
-00032f90: 7374 6f72 6167 655f 6f62 6a2e 6164 645f  storage_obj.add_
-00032fa0: 7374 6f72 6528 7374 6f72 655f 7479 7065  store(store_type
-00032fb0: 2c20 7265 6769 6f6e 3d72 6567 696f 6e29  , region=region)
-00032fc0: 0a20 2020 2020 2020 2062 7563 6b65 745f  .        bucket_
-00032fd0: 6e61 6d65 203d 2074 6d70 5f6c 6f63 616c  name = tmp_local
-00032fe0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
-00032ff0: 650a 0a20 2020 2020 2020 2023 2043 6f6e  e..        # Con
-00033000: 6669 726d 2074 6861 7420 7468 6520 6275  firm that the bu
-00033010: 636b 6574 2077 6173 2063 7265 6174 6564  cket was created
-00033020: 2069 6e20 7468 6520 636f 7272 6563 7420   in the correct 
-00033030: 7265 6769 6f6e 0a20 2020 2020 2020 2072  region.        r
-00033040: 6567 696f 6e5f 636d 6420 3d20 7365 6c66  egion_cmd = self
-00033050: 2e63 6c69 5f72 6567 696f 6e5f 636d 6428  .cli_region_cmd(
-00033060: 7374 6f72 655f 7479 7065 2c20 6275 636b  store_type, buck
-00033070: 6574 5f6e 616d 6529 0a20 2020 2020 2020  et_name).       
-00033080: 206f 7574 203d 2073 7562 7072 6f63 6573   out = subproces
-00033090: 732e 6368 6563 6b5f 6f75 7470 7574 2872  s.check_output(r
-000330a0: 6567 696f 6e5f 636d 642c 2073 6865 6c6c  egion_cmd, shell
-000330b0: 3d54 7275 6529 0a20 2020 2020 2020 206f  =True).        o
-000330c0: 7574 7075 7420 3d20 6f75 742e 6465 636f  utput = out.deco
-000330d0: 6465 2827 7574 662d 3827 290a 2020 2020  de('utf-8').    
-000330e0: 2020 2020 6173 7365 7274 2072 6567 696f      assert regio
-000330f0: 6e20 696e 206f 7574 2e64 6563 6f64 6528  n in out.decode(
-00033100: 2775 7466 2d38 2729 2c20 280a 2020 2020  'utf-8'), (.    
-00033110: 2020 2020 2020 2020 6627 4275 636b 6574          f'Bucket
-00033120: 2077 6173 206e 6f74 2066 6f75 6e64 2069   was not found i
-00033130: 6e20 7265 6769 6f6e 207b 7265 6769 6f6e  n region {region
-00033140: 7d20 2d20 270a 2020 2020 2020 2020 2020  } - '.          
-00033150: 2020 6627 6f75 7470 7574 206f 6620 7b72    f'output of {r
-00033160: 6567 696f 6e5f 636d 647d 2077 6173 3a20  egion_cmd} was: 
-00033170: 7b6f 7574 7075 747d 2729 0a0a 2020 2020  {output}')..    
-00033180: 2020 2020 2320 4368 6563 6b20 6966 2074      # Check if t
-00033190: 6d70 5f73 6f75 7263 652f 746d 702d 6669  mp_source/tmp-fi
-000331a0: 6c65 2065 7869 7374 7320 696e 2074 6865  le exists in the
-000331b0: 2062 7563 6b65 7420 7573 696e 6720 636c   bucket using cl
-000331c0: 690a 2020 2020 2020 2020 6c73 5f63 6d64  i.        ls_cmd
-000331d0: 203d 2073 656c 662e 636c 695f 6c73 5f63   = self.cli_ls_c
-000331e0: 6d64 2873 746f 7265 5f74 7970 652c 2062  md(store_type, b
-000331f0: 7563 6b65 745f 6e61 6d65 290a 2020 2020  ucket_name).    
-00033200: 2020 2020 6f75 7420 3d20 7375 6270 726f      out = subpro
-00033210: 6365 7373 2e63 6865 636b 5f6f 7574 7075  cess.check_outpu
-00033220: 7428 6c73 5f63 6d64 2c20 7368 656c 6c3d  t(ls_cmd, shell=
-00033230: 5472 7565 290a 2020 2020 2020 2020 6f75  True).        ou
-00033240: 7470 7574 203d 206f 7574 2e64 6563 6f64  tput = out.decod
-00033250: 6528 2775 7466 2d38 2729 0a20 2020 2020  e('utf-8').     
-00033260: 2020 2061 7373 6572 7420 2774 6d70 2d66     assert 'tmp-f
-00033270: 696c 6527 2069 6e20 6f75 7470 7574 2c20  ile' in output, 
-00033280: 280a 2020 2020 2020 2020 2020 2020 6627  (.            f'
-00033290: 746d 702d 6669 6c65 206e 6f74 2066 6f75  tmp-file not fou
-000332a0: 6e64 2069 6e20 6275 636b 6574 202d 206f  nd in bucket - o
-000332b0: 7574 7075 7420 6f66 207b 6c73 5f63 6d64  utput of {ls_cmd
-000332c0: 7d20 7761 733a 207b 6f75 7470 7574 7d27  } was: {output}'
-000332d0: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
-000332e0: 2054 6573 7469 6e67 2059 414d 4c20 5370   Testing YAML Sp
-000332f0: 6563 7320 2d2d 2d2d 2d2d 2d2d 2d2d 0a23  ecs ----------.#
-00033300: 204f 7572 2073 6b79 2073 746f 7261 6765   Our sky storage
-00033310: 2072 6571 7569 7265 7320 6372 6564 656e   requires creden
-00033320: 7469 616c 7320 746f 2063 6865 636b 2074  tials to check t
-00033330: 6865 2062 7563 6b65 7420 6578 6973 7461  he bucket exista
-00033340: 6e63 6520 7768 656e 0a23 206c 6f61 6469  nce when.# loadi
-00033350: 6e67 2061 2074 6173 6b20 6672 6f6d 2074  ng a task from t
-00033360: 6865 2079 616d 6c20 6669 6c65 2c20 736f  he yaml file, so
-00033370: 2077 6520 6361 6e6e 6f74 206d 616b 6520   we cannot make 
-00033380: 6974 2061 2075 6e69 7420 7465 7374 2e0a  it a unit test..
-00033390: 636c 6173 7320 5465 7374 5961 6d6c 5370  class TestYamlSp
-000333a0: 6563 733a 0a20 2020 2023 2054 4f44 4f28  ecs:.    # TODO(
-000333b0: 7a68 7775 293a 2041 6464 2074 6573 7420  zhwu): Add test 
-000333c0: 666f 7220 6074 6f5f 7961 6d6c 5f63 6f6e  for `to_yaml_con
-000333d0: 6669 6760 2066 6f72 2074 6865 2053 746f  fig` for the Sto
-000333e0: 7261 6765 206f 626a 6563 742e 0a20 2020  rage object..   
-000333f0: 2023 2020 5765 2073 686f 756c 6420 6e6f   #  We should no
-00033400: 7420 7573 6520 6065 7861 6d70 6c65 732f  t use `examples/
-00033410: 7374 6f72 6167 655f 6465 6d6f 2e79 616d  storage_demo.yam
-00033420: 6c60 2068 6572 652c 2073 696e 6365 2069  l` here, since i
-00033430: 7420 7265 7175 6972 6573 0a20 2020 2023  t requires.    #
-00033440: 2020 7573 6572 7320 746f 2065 6e73 7572    users to ensur
-00033450: 6520 6275 636b 6574 206e 616d 6573 2074  e bucket names t
-00033460: 6f20 6e6f 7420 6578 6973 7420 616e 642f  o not exist and/
-00033470: 6f72 2062 6520 756e 6971 7565 2e0a 2020  or be unique..  
-00033480: 2020 5f54 4553 545f 5941 4d4c 5f50 4154    _TEST_YAML_PAT
-00033490: 4853 203d 205b 0a20 2020 2020 2020 2027  HS = [.        '
-000334a0: 6578 616d 706c 6573 2f6d 696e 696d 616c  examples/minimal
-000334b0: 2e79 616d 6c27 2c20 2765 7861 6d70 6c65  .yaml', 'example
-000334c0: 732f 6d61 6e61 6765 645f 6a6f 622e 7961  s/managed_job.ya
-000334d0: 6d6c 272c 0a20 2020 2020 2020 2027 6578  ml',.        'ex
-000334e0: 616d 706c 6573 2f75 7369 6e67 5f66 696c  amples/using_fil
-000334f0: 655f 6d6f 756e 7473 2e79 616d 6c27 2c20  e_mounts.yaml', 
-00033500: 2765 7861 6d70 6c65 732f 7265 736e 6574  'examples/resnet
-00033510: 5f61 7070 2e79 616d 6c27 2c0a 2020 2020  _app.yaml',.    
-00033520: 2020 2020 2765 7861 6d70 6c65 732f 6d75      'examples/mu
-00033530: 6c74 695f 686f 7374 6e61 6d65 2e79 616d  lti_hostname.yam
-00033540: 6c27 0a20 2020 205d 0a0a 2020 2020 6465  l'.    ]..    de
-00033550: 6620 5f69 735f 6469 6374 5f73 7562 7365  f _is_dict_subse
-00033560: 7428 7365 6c66 2c20 6431 2c20 6432 293a  t(self, d1, d2):
-00033570: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
-00033580: 6b20 6966 2064 3120 6973 2074 6865 2073  k if d1 is the s
-00033590: 7562 7365 7420 6f66 2064 322e 2222 220a  ubset of d2.""".
-000335a0: 2020 2020 2020 2020 666f 7220 6b2c 2076          for k, v
-000335b0: 2069 6e20 6431 2e69 7465 6d73 2829 3a0a   in d1.items():.
-000335c0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-000335d0: 206e 6f74 2069 6e20 6432 3a0a 2020 2020   not in d2:.    
-000335e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000335f0: 7369 6e73 7461 6e63 6528 762c 206c 6973  sinstance(v, lis
-00033600: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00033610: 2876 2c20 6469 6374 293a 0a20 2020 2020  (v, dict):.     
-00033620: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00033630: 7373 6572 7420 6c65 6e28 7629 203d 3d20  ssert len(v) == 
-00033640: 302c 2028 6b2c 2076 290a 2020 2020 2020  0, (k, v).      
-00033650: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00033660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033670: 2020 2020 6173 7365 7274 2046 616c 7365      assert False
-00033680: 2c20 286b 2c20 7629 0a20 2020 2020 2020  , (k, v).       
-00033690: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-000336a0: 616e 6365 2876 2c20 6469 6374 293a 0a20  ance(v, dict):. 
-000336b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000336c0: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-000336d0: 2864 325b 6b5d 2c20 6469 6374 292c 2028  (d2[k], dict), (
-000336e0: 6b2c 2076 2c20 6432 290a 2020 2020 2020  k, v, d2).      
-000336f0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00033700: 6973 5f64 6963 745f 7375 6273 6574 2876  is_dict_subset(v
-00033710: 2c20 6432 5b6b 5d29 0a20 2020 2020 2020  , d2[k]).       
-00033720: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00033730: 616e 6365 2876 2c20 7374 7229 3a0a 2020  ance(v, str):.  
-00033740: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00033750: 206b 203d 3d20 2761 6363 656c 6572 6174   k == 'accelerat
-00033760: 6f72 7327 3a0a 2020 2020 2020 2020 2020  ors':.          
-00033770: 2020 2020 2020 2020 2020 7265 736f 7572            resour
-00033780: 6365 7320 3d20 736b 792e 5265 736f 7572  ces = sky.Resour
-00033790: 6365 7328 290a 2020 2020 2020 2020 2020  ces().          
-000337a0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
-000337b0: 6365 732e 5f73 6574 5f61 6363 656c 6572  ces._set_acceler
-000337c0: 6174 6f72 7328 762c 204e 6f6e 6529 0a20  ators(v, None). 
-000337d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000337e0: 2020 2061 7373 6572 7420 7265 736f 7572     assert resour
-000337f0: 6365 732e 6163 6365 6c65 7261 746f 7273  ces.accelerators
-00033800: 203d 3d20 6432 5b6b 5d2c 2028 6b2c 2076   == d2[k], (k, v
-00033810: 2c20 6432 290a 2020 2020 2020 2020 2020  , d2).          
-00033820: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00033830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033840: 6173 7365 7274 2076 2e6c 6f77 6572 2829  assert v.lower()
-00033850: 203d 3d20 6432 5b6b 5d2e 6c6f 7765 7228   == d2[k].lower(
-00033860: 292c 2028 6b2c 2076 2c20 6432 5b6b 5d29  ), (k, v, d2[k])
-00033870: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00033880: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00033890: 2020 2061 7373 6572 7420 7620 3d3d 2064     assert v == d
-000338a0: 325b 6b5d 2c20 286b 2c20 762c 2064 325b  2[k], (k, v, d2[
-000338b0: 6b5d 290a 0a20 2020 2064 6566 205f 6368  k])..    def _ch
-000338c0: 6563 6b5f 6571 7569 7661 6c65 6e74 2873  eck_equivalent(s
-000338d0: 656c 662c 2079 616d 6c5f 7061 7468 293a  elf, yaml_path):
-000338e0: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
-000338f0: 6b20 6966 2074 6865 2079 616d 6c20 6973  k if the yaml is
-00033900: 2065 7175 6976 616c 656e 7420 6166 7465   equivalent afte
-00033910: 7220 6c6f 6164 2061 6e64 2064 756d 7020  r load and dump 
-00033920: 6167 6169 6e2e 2222 220a 2020 2020 2020  again.""".      
-00033930: 2020 6f72 6967 696e 5f74 6173 6b5f 636f    origin_task_co
-00033940: 6e66 6967 203d 2063 6f6d 6d6f 6e5f 7574  nfig = common_ut
-00033950: 696c 732e 7265 6164 5f79 616d 6c28 7961  ils.read_yaml(ya
-00033960: 6d6c 5f70 6174 6829 0a0a 2020 2020 2020  ml_path)..      
-00033970: 2020 7461 736b 203d 2073 6b79 2e54 6173    task = sky.Tas
-00033980: 6b2e 6672 6f6d 5f79 616d 6c28 7961 6d6c  k.from_yaml(yaml
-00033990: 5f70 6174 6829 0a20 2020 2020 2020 206e  _path).        n
-000339a0: 6577 5f74 6173 6b5f 636f 6e66 6967 203d  ew_task_config =
-000339b0: 2074 6173 6b2e 746f 5f79 616d 6c5f 636f   task.to_yaml_co
-000339c0: 6e66 6967 2829 0a20 2020 2020 2020 2023  nfig().        #
-000339d0: 2064 3120 3c3d 2064 320a 2020 2020 2020   d1 <= d2.      
-000339e0: 2020 7072 696e 7428 6f72 6967 696e 5f74    print(origin_t
-000339f0: 6173 6b5f 636f 6e66 6967 2c20 6e65 775f  ask_config, new_
-00033a00: 7461 736b 5f63 6f6e 6669 6729 0a20 2020  task_config).   
-00033a10: 2020 2020 2073 656c 662e 5f69 735f 6469       self._is_di
-00033a20: 6374 5f73 7562 7365 7428 6f72 6967 696e  ct_subset(origin
-00033a30: 5f74 6173 6b5f 636f 6e66 6967 2c20 6e65  _task_config, ne
-00033a40: 775f 7461 736b 5f63 6f6e 6669 6729 0a0a  w_task_config)..
-00033a50: 2020 2020 6465 6620 7465 7374 5f6c 6f61      def test_loa
-00033a60: 645f 6475 6d70 5f79 616d 6c5f 636f 6e66  d_dump_yaml_conf
-00033a70: 6967 5f65 7175 6976 616c 656e 7428 7365  ig_equivalent(se
-00033a80: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00033a90: 5465 7374 2069 6620 7468 6520 7961 6d6c  Test if the yaml
-00033aa0: 2063 6f6e 6669 6720 6973 2065 7175 6976   config is equiv
-00033ab0: 616c 656e 7420 6166 7465 7220 6c6f 6164  alent after load
-00033ac0: 2061 6e64 2064 756d 7020 6167 6169 6e2e   and dump again.
-00033ad0: 2222 220a 2020 2020 2020 2020 7061 7468  """.        path
-00033ae0: 6c69 622e 5061 7468 2827 7e2f 6461 7461  lib.Path('~/data
-00033af0: 7365 7473 2729 2e65 7870 616e 6475 7365  sets').expanduse
-00033b00: 7228 292e 6d6b 6469 7228 6578 6973 745f  r().mkdir(exist_
-00033b10: 6f6b 3d54 7275 6529 0a20 2020 2020 2020  ok=True).       
-00033b20: 2070 6174 686c 6962 2e50 6174 6828 277e   pathlib.Path('~
-00033b30: 2f74 6d70 6669 6c65 2729 2e65 7870 616e  /tmpfile').expan
-00033b40: 6475 7365 7228 292e 746f 7563 6828 290a  duser().touch().
-00033b50: 2020 2020 2020 2020 7061 7468 6c69 622e          pathlib.
-00033b60: 5061 7468 2827 7e2f 2e73 7368 2729 2e65  Path('~/.ssh').e
-00033b70: 7870 616e 6475 7365 7228 292e 6d6b 6469  xpanduser().mkdi
-00033b80: 7228 6578 6973 745f 6f6b 3d54 7275 6529  r(exist_ok=True)
-00033b90: 0a20 2020 2020 2020 2070 6174 686c 6962  .        pathlib
-00033ba0: 2e50 6174 6828 277e 2f2e 7373 682f 6964  .Path('~/.ssh/id
-00033bb0: 5f72 7361 2e70 7562 2729 2e65 7870 616e  _rsa.pub').expan
-00033bc0: 6475 7365 7228 292e 746f 7563 6828 290a  duser().touch().
-00033bd0: 2020 2020 2020 2020 7061 7468 6c69 622e          pathlib.
-00033be0: 5061 7468 2827 7e2f 746d 702d 776f 726b  Path('~/tmp-work
-00033bf0: 6469 7227 292e 6578 7061 6e64 7573 6572  dir').expanduser
-00033c00: 2829 2e6d 6b64 6972 2865 7869 7374 5f6f  ().mkdir(exist_o
-00033c10: 6b3d 5472 7565 290a 2020 2020 2020 2020  k=True).        
-00033c20: 7061 7468 6c69 622e 5061 7468 2827 7e2f  pathlib.Path('~/
-00033c30: 446f 776e 6c6f 6164 732f 7470 7527 292e  Downloads/tpu').
-00033c40: 6578 7061 6e64 7573 6572 2829 2e6d 6b64  expanduser().mkd
-00033c50: 6972 2870 6172 656e 7473 3d54 7275 652c  ir(parents=True,
-00033c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00033c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00033c90: 2020 2020 2020 2020 2020 2020 6578 6973              exis
-00033ca0: 745f 6f6b 3d54 7275 6529 0a20 2020 2020  t_ok=True).     
-00033cb0: 2020 2066 6f72 2079 616d 6c5f 7061 7468     for yaml_path
-00033cc0: 2069 6e20 7365 6c66 2e5f 5445 5354 5f59   in self._TEST_Y
-00033cd0: 414d 4c5f 5041 5448 533a 0a20 2020 2020  AML_PATHS:.     
-00033ce0: 2020 2020 2020 2073 656c 662e 5f63 6865         self._che
-00033cf0: 636b 5f65 7175 6976 616c 656e 7428 7961  ck_equivalent(ya
-00033d00: 6d6c 5f70 6174 6829 0a0a 0a23 202d 2d2d  ml_path)...# ---
-00033d10: 2d2d 2d2d 2d2d 2d20 5465 7374 696e 6720  ------- Testing 
-00033d20: 4d75 6c74 6970 6c65 2041 6363 656c 6572  Multiple Acceler
-00033d30: 6174 6f72 7320 2d2d 2d2d 2d2d 2d2d 2d2d  ators ----------
-00033d40: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00033d50: 5f66 6c75 6964 7374 6163 6b20 2023 2046  _fluidstack  # F
-00033d60: 6c75 6964 7374 6163 6b20 646f 6573 206e  luidstack does n
-00033d70: 6f74 2073 7570 706f 7274 204b 3830 2067  ot support K80 g
-00033d80: 7075 7320 666f 7220 6e6f 770a 4070 7974  pus for now.@pyt
-00033d90: 6573 742e 6d61 726b 2e6e 6f5f 7061 7065  est.mark.no_pape
-00033da0: 7273 7061 6365 2020 2320 5061 7065 7273  rspace  # Papers
-00033db0: 7061 6365 2064 6f65 7320 6e6f 7420 7375  pace does not su
-00033dc0: 7070 6f72 7420 4b38 3020 6770 7573 0a64  pport K80 gpus.d
-00033dd0: 6566 2074 6573 745f 6d75 6c74 6970 6c65  ef test_multiple
-00033de0: 5f61 6363 656c 6572 6174 6f72 735f 6f72  _accelerators_or
-00033df0: 6465 7265 6428 293a 0a20 2020 206e 616d  dered():.    nam
-00033e00: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
-00033e10: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
-00033e20: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
-00033e30: 2027 6d75 6c74 6970 6c65 2d61 6363 656c   'multiple-accel
-00033e40: 6572 6174 6f72 732d 6f72 6465 7265 6427  erators-ordered'
-00033e50: 2c0a 2020 2020 2020 2020 5b0a 2020 2020  ,.        [.    
-00033e60: 2020 2020 2020 2020 6627 736b 7920 6c61          f'sky la
-00033e70: 756e 6368 202d 7920 2d63 207b 6e61 6d65  unch -y -c {name
-00033e80: 7d20 7465 7374 732f 7465 7374 5f79 616d  } tests/test_yam
-00033e90: 6c73 2f74 6573 745f 6d75 6c74 6970 6c65  ls/test_multiple
-00033ea0: 5f61 6363 656c 6572 6174 6f72 735f 6f72  _accelerators_or
-00033eb0: 6465 7265 642e 7961 6d6c 207c 2067 7265  dered.yaml | gre
-00033ec0: 7020 2255 7369 6e67 2075 7365 722d 7370  p "Using user-sp
-00033ed0: 6563 6966 6965 6420 6163 6365 6c65 7261  ecified accelera
-00033ee0: 746f 7273 206c 6973 7422 272c 0a20 2020  tors list"',.   
-00033ef0: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-00033f00: 6f67 7320 7b6e 616d 657d 2031 202d 2d73  ogs {name} 1 --s
-00033f10: 7461 7475 7327 2c20 2023 2045 6e73 7572  tatus',  # Ensur
-00033f20: 6520 7468 6520 6a6f 6220 7375 6363 6565  e the job succee
-00033f30: 6465 642e 0a20 2020 2020 2020 205d 2c0a  ded..        ],.
-00033f40: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
-00033f50: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
-00033f60: 2020 2020 2020 2074 696d 656f 7574 3d32         timeout=2
-00033f70: 3020 2a20 3630 2c0a 2020 2020 290a 2020  0 * 60,.    ).  
-00033f80: 2020 7275 6e5f 6f6e 655f 7465 7374 2874    run_one_test(t
-00033f90: 6573 7429 0a0a 0a40 7079 7465 7374 2e6d  est)...@pytest.m
-00033fa0: 6172 6b2e 6e6f 5f66 6c75 6964 7374 6163  ark.no_fluidstac
-00033fb0: 6b20 2023 2046 6c75 6964 7374 6163 6b20  k  # Fluidstack 
-00033fc0: 6861 7320 6c6f 7720 6176 6169 6c61 6269  has low availabi
-00033fd0: 6c69 7479 2066 6f72 2054 3420 4750 5573  lity for T4 GPUs
-00033fe0: 0a40 7079 7465 7374 2e6d 6172 6b2e 6e6f  .@pytest.mark.no
-00033ff0: 5f70 6170 6572 7370 6163 6520 2023 2050  _paperspace  # P
-00034000: 6170 6572 7370 6163 6520 646f 6573 206e  aperspace does n
-00034010: 6f74 2073 7570 706f 7274 2054 3420 4750  ot support T4 GP
-00034020: 5573 0a64 6566 2074 6573 745f 6d75 6c74  Us.def test_mult
-00034030: 6970 6c65 5f61 6363 656c 6572 6174 6f72  iple_accelerator
-00034040: 735f 6f72 6465 7265 645f 7769 7468 5f64  s_ordered_with_d
-00034050: 6566 6175 6c74 2829 3a0a 2020 2020 6e61  efault():.    na
-00034060: 6d65 203d 205f 6765 745f 636c 7573 7465  me = _get_cluste
-00034070: 725f 6e61 6d65 2829 0a20 2020 2074 6573  r_name().    tes
-00034080: 7420 3d20 5465 7374 280a 2020 2020 2020  t = Test(.      
-00034090: 2020 276d 756c 7469 706c 652d 6163 6365    'multiple-acce
-000340a0: 6c65 7261 746f 7273 2d6f 7264 6572 6564  lerators-ordered
-000340b0: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-000340c0: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-000340d0: 6175 6e63 6820 2d79 202d 6320 7b6e 616d  aunch -y -c {nam
-000340e0: 657d 2074 6573 7473 2f74 6573 745f 7961  e} tests/test_ya
-000340f0: 6d6c 732f 7465 7374 5f6d 756c 7469 706c  mls/test_multipl
-00034100: 655f 6163 6365 6c65 7261 746f 7273 5f6f  e_accelerators_o
-00034110: 7264 6572 6564 5f77 6974 685f 6465 6661  rdered_with_defa
-00034120: 756c 742e 7961 6d6c 207c 2067 7265 7020  ult.yaml | grep 
-00034130: 2255 7369 6e67 2075 7365 722d 7370 6563  "Using user-spec
-00034140: 6966 6965 6420 6163 6365 6c65 7261 746f  ified accelerato
-00034150: 7273 206c 6973 7422 272c 0a20 2020 2020  rs list"',.     
-00034160: 2020 2020 2020 2066 2773 6b79 206c 6f67         f'sky log
-00034170: 7320 7b6e 616d 657d 2031 202d 2d73 7461  s {name} 1 --sta
-00034180: 7475 7327 2c20 2023 2045 6e73 7572 6520  tus',  # Ensure 
-00034190: 7468 6520 6a6f 6220 7375 6363 6565 6465  the job succeede
-000341a0: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
-000341b0: 2773 6b79 2073 7461 7475 7320 7b6e 616d  'sky status {nam
-000341c0: 657d 207c 2067 7265 7020 5370 6f74 272c  e} | grep Spot',
-000341d0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-000341e0: 2020 2020 6627 736b 7920 646f 776e 202d      f'sky down -
-000341f0: 7920 7b6e 616d 657d 272c 0a20 2020 2029  y {name}',.    )
-00034200: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
-00034210: 7428 7465 7374 290a 0a0a 4070 7974 6573  t(test)...@pytes
-00034220: 742e 6d61 726b 2e6e 6f5f 666c 7569 6473  t.mark.no_fluids
-00034230: 7461 636b 2020 2320 466c 7569 6473 7461  tack  # Fluidsta
-00034240: 636b 2068 6173 206c 6f77 2061 7661 696c  ck has low avail
-00034250: 6162 696c 6974 7920 666f 7220 5434 2047  ability for T4 G
-00034260: 5055 730a 4070 7974 6573 742e 6d61 726b  PUs.@pytest.mark
-00034270: 2e6e 6f5f 7061 7065 7273 7061 6365 2020  .no_paperspace  
-00034280: 2320 5061 7065 7273 7061 6365 2064 6f65  # Paperspace doe
-00034290: 7320 6e6f 7420 7375 7070 6f72 7420 5434  s not support T4
-000342a0: 2047 5055 730a 6465 6620 7465 7374 5f6d   GPUs.def test_m
-000342b0: 756c 7469 706c 655f 6163 6365 6c65 7261  ultiple_accelera
-000342c0: 746f 7273 5f75 6e6f 7264 6572 6564 2829  tors_unordered()
-000342d0: 3a0a 2020 2020 6e61 6d65 203d 205f 6765  :.    name = _ge
-000342e0: 745f 636c 7573 7465 725f 6e61 6d65 2829  t_cluster_name()
-000342f0: 0a20 2020 2074 6573 7420 3d20 5465 7374  .    test = Test
-00034300: 280a 2020 2020 2020 2020 276d 756c 7469  (.        'multi
-00034310: 706c 652d 6163 6365 6c65 7261 746f 7273  ple-accelerators
-00034320: 2d75 6e6f 7264 6572 6564 272c 0a20 2020  -unordered',.   
-00034330: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00034340: 2020 2066 2773 6b79 206c 6175 6e63 6820     f'sky launch 
-00034350: 2d79 202d 6320 7b6e 616d 657d 2074 6573  -y -c {name} tes
-00034360: 7473 2f74 6573 745f 7961 6d6c 732f 7465  ts/test_yamls/te
-00034370: 7374 5f6d 756c 7469 706c 655f 6163 6365  st_multiple_acce
-00034380: 6c65 7261 746f 7273 5f75 6e6f 7264 6572  lerators_unorder
-00034390: 6564 2e79 616d 6c27 2c0a 2020 2020 2020  ed.yaml',.      
-000343a0: 2020 2020 2020 6627 736b 7920 6c6f 6773        f'sky logs
-000343b0: 207b 6e61 6d65 7d20 3120 2d2d 7374 6174   {name} 1 --stat
-000343c0: 7573 272c 2020 2320 456e 7375 7265 2074  us',  # Ensure t
-000343d0: 6865 206a 6f62 2073 7563 6365 6564 6564  he job succeeded
-000343e0: 2e0a 2020 2020 2020 2020 5d2c 0a20 2020  ..        ],.   
-000343f0: 2020 2020 2066 2773 6b79 2064 6f77 6e20       f'sky down 
-00034400: 2d79 207b 6e61 6d65 7d27 2c0a 2020 2020  -y {name}',.    
-00034410: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
-00034420: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
-00034430: 7374 2e6d 6172 6b2e 6e6f 5f66 6c75 6964  st.mark.no_fluid
-00034440: 7374 6163 6b20 2023 2046 6c75 6964 7374  stack  # Fluidst
-00034450: 6163 6b20 6861 7320 6c6f 7720 6176 6169  ack has low avai
-00034460: 6c61 6269 6c69 7479 2066 6f72 2054 3420  lability for T4 
-00034470: 4750 5573 0a40 7079 7465 7374 2e6d 6172  GPUs.@pytest.mar
-00034480: 6b2e 6e6f 5f70 6170 6572 7370 6163 6520  k.no_paperspace 
-00034490: 2023 2050 6170 6572 7370 6163 6520 646f   # Paperspace do
-000344a0: 6573 206e 6f74 2073 7570 706f 7274 2054  es not support T
-000344b0: 3420 4750 5573 0a64 6566 2074 6573 745f  4 GPUs.def test_
-000344c0: 6d75 6c74 6970 6c65 5f61 6363 656c 6572  multiple_acceler
-000344d0: 6174 6f72 735f 756e 6f72 6465 7265 645f  ators_unordered_
-000344e0: 7769 7468 5f64 6566 6175 6c74 2829 3a0a  with_default():.
-000344f0: 2020 2020 6e61 6d65 203d 205f 6765 745f      name = _get_
-00034500: 636c 7573 7465 725f 6e61 6d65 2829 0a20  cluster_name(). 
-00034510: 2020 2074 6573 7420 3d20 5465 7374 280a     test = Test(.
-00034520: 2020 2020 2020 2020 276d 756c 7469 706c          'multipl
-00034530: 652d 6163 6365 6c65 7261 746f 7273 2d75  e-accelerators-u
-00034540: 6e6f 7264 6572 6564 272c 0a20 2020 2020  nordered',.     
-00034550: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00034560: 2066 2773 6b79 206c 6175 6e63 6820 2d79   f'sky launch -y
-00034570: 202d 6320 7b6e 616d 657d 2074 6573 7473   -c {name} tests
-00034580: 2f74 6573 745f 7961 6d6c 732f 7465 7374  /test_yamls/test
-00034590: 5f6d 756c 7469 706c 655f 6163 6365 6c65  _multiple_accele
-000345a0: 7261 746f 7273 5f75 6e6f 7264 6572 6564  rators_unordered
-000345b0: 5f77 6974 685f 6465 6661 756c 742e 7961  _with_default.ya
-000345c0: 6d6c 272c 0a20 2020 2020 2020 2020 2020  ml',.           
-000345d0: 2066 2773 6b79 206c 6f67 7320 7b6e 616d   f'sky logs {nam
-000345e0: 657d 2031 202d 2d73 7461 7475 7327 2c20  e} 1 --status', 
-000345f0: 2023 2045 6e73 7572 6520 7468 6520 6a6f   # Ensure the jo
-00034600: 6220 7375 6363 6565 6465 642e 0a20 2020  b succeeded..   
-00034610: 2020 2020 2020 2020 2066 2773 6b79 2073           f'sky s
-00034620: 7461 7475 7320 7b6e 616d 657d 207c 2067  tatus {name} | g
-00034630: 7265 7020 5370 6f74 272c 0a20 2020 2020  rep Spot',.     
-00034640: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
-00034650: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
-00034660: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
-00034670: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00034680: 290a 0a0a 4070 7974 6573 742e 6d61 726b  )...@pytest.mark
-00034690: 2e6e 6f5f 666c 7569 6473 7461 636b 2020  .no_fluidstack  
-000346a0: 2320 5265 7175 6972 6573 206f 7468 6572  # Requires other
-000346b0: 2063 6c6f 7564 7320 746f 2062 6520 656e   clouds to be en
-000346c0: 6162 6c65 640a 6465 6620 7465 7374 5f6d  abled.def test_m
-000346d0: 756c 7469 706c 655f 7265 736f 7572 6365  ultiple_resource
-000346e0: 7328 293a 0a20 2020 206e 616d 6520 3d20  s():.    name = 
-000346f0: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
-00034700: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
-00034710: 6573 7428 0a20 2020 2020 2020 2027 6d75  est(.        'mu
-00034720: 6c74 6970 6c65 2d72 6573 6f75 7263 6573  ltiple-resources
-00034730: 272c 0a20 2020 2020 2020 205b 0a20 2020  ',.        [.   
-00034740: 2020 2020 2020 2020 2066 2773 6b79 206c           f'sky l
-00034750: 6175 6e63 6820 2d79 202d 6320 7b6e 616d  aunch -y -c {nam
-00034760: 657d 2074 6573 7473 2f74 6573 745f 7961  e} tests/test_ya
-00034770: 6d6c 732f 7465 7374 5f6d 756c 7469 706c  mls/test_multipl
-00034780: 655f 7265 736f 7572 6365 732e 7961 6d6c  e_resources.yaml
-00034790: 272c 0a20 2020 2020 2020 2020 2020 2066  ',.            f
-000347a0: 2773 6b79 206c 6f67 7320 7b6e 616d 657d  'sky logs {name}
-000347b0: 2031 202d 2d73 7461 7475 7327 2c20 2023   1 --status',  #
-000347c0: 2045 6e73 7572 6520 7468 6520 6a6f 6220   Ensure the job 
-000347d0: 7375 6363 6565 6465 642e 0a20 2020 2020  succeeded..     
-000347e0: 2020 205d 2c0a 2020 2020 2020 2020 6627     ],.        f'
-000347f0: 736b 7920 646f 776e 202d 7920 7b6e 616d  sky down -y {nam
-00034800: 657d 272c 0a20 2020 2029 0a20 2020 2072  e}',.    ).    r
-00034810: 756e 5f6f 6e65 5f74 6573 7428 7465 7374  un_one_test(test
-00034820: 290a 0a0a 2320 2d2d 2d2d 2d2d 2d2d 2d2d  )...# ----------
-00034830: 2053 6b79 2042 656e 6368 6d61 726b 202d   Sky Benchmark -
-00034840: 2d2d 2d2d 2d2d 2d2d 2d0a 4070 7974 6573  ---------.@pytes
-00034850: 742e 6d61 726b 2e6e 6f5f 666c 7569 6473  t.mark.no_fluids
-00034860: 7461 636b 2020 2320 5265 7175 6972 6573  tack  # Requires
-00034870: 206f 7468 6572 2063 6c6f 7564 7320 746f   other clouds to
-00034880: 2062 6520 656e 6162 6c65 640a 4070 7974   be enabled.@pyt
-00034890: 6573 742e 6d61 726b 2e6e 6f5f 7061 7065  est.mark.no_pape
-000348a0: 7273 7061 6365 2020 2320 5265 7175 6972  rspace  # Requir
-000348b0: 6573 206f 7468 6572 2063 6c6f 7564 7320  es other clouds 
-000348c0: 746f 2062 6520 656e 6162 6c65 640a 4070  to be enabled.@p
-000348d0: 7974 6573 742e 6d61 726b 2e6e 6f5f 6b75  ytest.mark.no_ku
-000348e0: 6265 726e 6574 6573 0a64 6566 2074 6573  bernetes.def tes
-000348f0: 745f 736b 795f 6265 6e63 6828 6765 6e65  t_sky_bench(gene
-00034900: 7269 635f 636c 6f75 643a 2073 7472 293a  ric_cloud: str):
-00034910: 0a20 2020 206e 616d 6520 3d20 5f67 6574  .    name = _get
-00034920: 5f63 6c75 7374 6572 5f6e 616d 6528 290a  _cluster_name().
-00034930: 2020 2020 7465 7374 203d 2054 6573 7428      test = Test(
-00034940: 0a20 2020 2020 2020 2027 736b 792d 6265  .        'sky-be
-00034950: 6e63 6827 2c0a 2020 2020 2020 2020 5b0a  nch',.        [.
-00034960: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
-00034970: 7920 6265 6e63 6820 6c61 756e 6368 202d  y bench launch -
-00034980: 7920 2d62 207b 6e61 6d65 7d20 2d2d 636c  y -b {name} --cl
-00034990: 6f75 6420 7b67 656e 6572 6963 5f63 6c6f  oud {generic_clo
-000349a0: 7564 7d20 2d69 3020 7465 7374 732f 7465  ud} -i0 tests/te
-000349b0: 7374 5f79 616d 6c73 2f6d 696e 696d 616c  st_yamls/minimal
-000349c0: 2e79 616d 6c27 2c0a 2020 2020 2020 2020  .yaml',.        
-000349d0: 2020 2020 2773 6c65 6570 2031 3230 272c      'sleep 120',
-000349e0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
-000349f0: 6b79 2062 656e 6368 2073 686f 7720 7b6e  ky bench show {n
-00034a00: 616d 657d 207c 2067 7265 7020 736b 792d  ame} | grep sky-
-00034a10: 6265 6e63 682d 7b6e 616d 657d 207c 2067  bench-{name} | g
-00034a20: 7265 7020 4649 4e49 5348 4544 272c 0a20  rep FINISHED',. 
-00034a30: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00034a40: 2020 6627 736b 7920 6265 6e63 6820 646f    f'sky bench do
-00034a50: 776e 207b 6e61 6d65 7d20 2d79 3b20 736b  wn {name} -y; sk
-00034a60: 7920 6265 6e63 6820 6465 6c65 7465 207b  y bench delete {
-00034a70: 6e61 6d65 7d20 2d79 272c 0a20 2020 2029  name} -y',.    )
-00034a80: 0a20 2020 2072 756e 5f6f 6e65 5f74 6573  .    run_one_tes
-00034a90: 7428 7465 7374 290a                      t(test).
+00031330: 2020 2020 2020 2020 2827 7574 662d 3827          ('utf-8'
+00031340: 2929 0a0a 2020 2020 4070 7974 6573 742e  ))..    @pytest.
+00031350: 6d61 726b 2e6e 6f5f 666c 7569 6473 7461  mark.no_fluidsta
+00031360: 636b 0a20 2020 2040 7079 7465 7374 2e6d  ck.    @pytest.m
+00031370: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00031380: 2769 6e76 616c 6964 5f6e 616d 655f 6c69  'invalid_name_li
+00031390: 7374 2c20 7374 6f72 655f 7479 7065 272c  st, store_type',
+000313a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000313b0: 2020 2020 2020 2020 2020 2020 2020 5b28                [(
+000313c0: 4157 535f 494e 5641 4c49 445f 4e41 4d45  AWS_INVALID_NAME
+000313d0: 532c 2073 746f 7261 6765 5f6c 6962 2e53  S, storage_lib.S
+000313e0: 746f 7265 5479 7065 2e53 3329 2c0a 2020  toreType.S3),.  
+000313f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031400: 2020 2020 2020 2020 2020 2020 2847 4353              (GCS
+00031410: 5f49 4e56 414c 4944 5f4e 414d 4553 2c20  _INVALID_NAMES, 
+00031420: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+00031430: 6554 7970 652e 4743 5329 2c0a 2020 2020  eType.GCS),.    
+00031440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031450: 2020 2020 2020 2020 2020 7079 7465 7374            pytest
+00031460: 2e70 6172 616d 2849 424d 5f49 4e56 414c  .param(IBM_INVAL
+00031470: 4944 5f4e 414d 4553 2c0a 2020 2020 2020  ID_NAMES,.      
+00031480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000314a0: 2020 2020 2073 746f 7261 6765 5f6c 6962       storage_lib
+000314b0: 2e53 746f 7265 5479 7065 2e49 424d 2c0a  .StoreType.IBM,.
+000314c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000314d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000314e0: 2020 2020 2020 2020 2020 206d 6172 6b73             marks
+000314f0: 3d70 7974 6573 742e 6d61 726b 2e69 626d  =pytest.mark.ibm
+00031500: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00031510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031520: 2070 7974 6573 742e 7061 7261 6d28 4157   pytest.param(AW
+00031530: 535f 494e 5641 4c49 445f 4e41 4d45 532c  S_INVALID_NAMES,
+00031540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00031550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031560: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00031570: 6167 655f 6c69 622e 5374 6f72 6554 7970  age_lib.StoreTyp
+00031580: 652e 5232 2c0a 2020 2020 2020 2020 2020  e.R2,.          
+00031590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000315a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000315b0: 206d 6172 6b73 3d70 7974 6573 742e 6d61   marks=pytest.ma
+000315c0: 726b 2e63 6c6f 7564 666c 6172 6529 5d29  rk.cloudflare)])
+000315d0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
+000315e0: 7661 6c69 645f 6e61 6d65 7328 7365 6c66  valid_names(self
+000315f0: 2c20 696e 7661 6c69 645f 6e61 6d65 5f6c  , invalid_name_l
+00031600: 6973 742c 2073 746f 7265 5f74 7970 6529  ist, store_type)
+00031610: 3a0a 2020 2020 2020 2020 2320 5573 6573  :.        # Uses
+00031620: 2061 206c 6973 7420 696e 2074 6865 2073   a list in the s
+00031630: 6f75 7263 6520 6669 656c 6420 746f 2073  ource field to s
+00031640: 7065 6369 6679 2061 2066 696c 6520 616e  pecify a file an
+00031650: 6420 6120 6469 7265 6374 6f72 7920 746f  d a directory to
+00031660: 0a20 2020 2020 2020 2023 2062 6520 7570  .        # be up
+00031670: 6c6f 6164 6564 2074 6f20 7468 6520 7374  loaded to the st
+00031680: 6f72 6167 6520 6f62 6a65 6374 2e0a 2020  orage object..  
+00031690: 2020 2020 2020 666f 7220 6e61 6d65 2069        for name i
+000316a0: 6e20 696e 7661 6c69 645f 6e61 6d65 5f6c  n invalid_name_l
+000316b0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+000316c0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+000316d0: 7365 7328 736b 792e 6578 6365 7074 696f  ses(sky.exceptio
+000316e0: 6e73 2e53 746f 7261 6765 4e61 6d65 4572  ns.StorageNameEr
+000316f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+00031700: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+00031710: 6a20 3d20 7374 6f72 6167 655f 6c69 622e  j = storage_lib.
+00031720: 5374 6f72 6167 6528 6e61 6d65 3d6e 616d  Storage(name=nam
+00031730: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00031740: 2020 2073 746f 7261 6765 5f6f 626a 2e61     storage_obj.a
+00031750: 6464 5f73 746f 7265 2873 746f 7265 5f74  dd_store(store_t
+00031760: 7970 6529 0a0a 2020 2020 4070 7974 6573  ype)..    @pytes
+00031770: 742e 6d61 726b 2e6e 6f5f 666c 7569 6473  t.mark.no_fluids
+00031780: 7461 636b 0a20 2020 2040 7079 7465 7374  tack.    @pytest
+00031790: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+000317a0: 6528 0a20 2020 2020 2020 2027 6769 7469  e(.        'giti
+000317b0: 676e 6f72 655f 7374 7275 6374 7572 652c  gnore_structure,
+000317c0: 2073 746f 7265 5f74 7970 6527 2c0a 2020   store_type',.  
+000317d0: 2020 2020 2020 5b28 4749 5449 474e 4f52        [(GITIGNOR
+000317e0: 455f 5359 4e43 5f54 4553 545f 4449 525f  E_SYNC_TEST_DIR_
+000317f0: 5354 5255 4354 5552 452c 2073 746f 7261  STRUCTURE, stora
+00031800: 6765 5f6c 6962 2e53 746f 7265 5479 7065  ge_lib.StoreType
+00031810: 2e53 3329 2c0a 2020 2020 2020 2020 2028  .S3),.         (
+00031820: 4749 5449 474e 4f52 455f 5359 4e43 5f54  GITIGNORE_SYNC_T
+00031830: 4553 545f 4449 525f 5354 5255 4354 5552  EST_DIR_STRUCTUR
+00031840: 452c 2073 746f 7261 6765 5f6c 6962 2e53  E, storage_lib.S
+00031850: 746f 7265 5479 7065 2e47 4353 292c 0a20  toreType.GCS),. 
+00031860: 2020 2020 2020 2020 7079 7465 7374 2e70          pytest.p
+00031870: 6172 616d 2847 4954 4947 4e4f 5245 5f53  aram(GITIGNORE_S
+00031880: 594e 435f 5445 5354 5f44 4952 5f53 5452  YNC_TEST_DIR_STR
+00031890: 5543 5455 5245 2c0a 2020 2020 2020 2020  UCTURE,.        
+000318a0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000318b0: 6f72 6167 655f 6c69 622e 5374 6f72 6554  orage_lib.StoreT
+000318c0: 7970 652e 5232 2c0a 2020 2020 2020 2020  ype.R2,.        
+000318d0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+000318e0: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
+000318f0: 636c 6f75 6466 6c61 7265 295d 290a 2020  cloudflare)]).  
+00031900: 2020 6465 6620 7465 7374 5f65 7863 6c75    def test_exclu
+00031910: 6465 645f 6669 6c65 5f63 6c6f 7564 5f73  ded_file_cloud_s
+00031920: 746f 7261 6765 5f75 706c 6f61 645f 636f  torage_upload_co
+00031930: 7079 2873 656c 662c 2067 6974 6967 6e6f  py(self, gitigno
+00031940: 7265 5f73 7472 7563 7475 7265 2c0a 2020  re_structure,.  
+00031950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031980: 2020 2073 746f 7265 5f74 7970 652c 0a20     store_type,. 
+00031990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000319a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000319b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000319c0: 2020 2020 746d 705f 6769 7469 676e 6f72      tmp_gitignor
+000319d0: 655f 7374 6f72 6167 655f 6f62 6a29 3a0a  e_storage_obj):.
+000319e0: 2020 2020 2020 2020 2320 7465 7374 7320          # tests 
+000319f0: 6966 2066 696c 6573 2069 6e63 6c75 6465  if files include
+00031a00: 6420 696e 202e 6769 7469 676e 6f72 6520  d in .gitignore 
+00031a10: 616e 6420 2e67 6974 2f69 6e66 6f2f 6578  and .git/info/ex
+00031a20: 636c 7564 6520 6172 650a 2020 2020 2020  clude are.      
+00031a30: 2020 2320 6578 636c 7564 6564 2066 726f    # excluded fro
+00031a40: 6d20 6265 696e 6720 7472 616e 7366 6572  m being transfer
+00031a50: 7265 6420 746f 2053 746f 7261 6765 0a0a  red to Storage..
+00031a60: 2020 2020 2020 2020 746d 705f 6769 7469          tmp_giti
+00031a70: 676e 6f72 655f 7374 6f72 6167 655f 6f62  gnore_storage_ob
+00031a80: 6a2e 6164 645f 7374 6f72 6528 7374 6f72  j.add_store(stor
+00031a90: 655f 7479 7065 290a 0a20 2020 2020 2020  e_type)..       
+00031aa0: 2075 706c 6f61 645f 6669 6c65 5f6e 616d   upload_file_nam
+00031ab0: 6520 3d20 2769 6e63 6c75 6465 6427 0a20  e = 'included'. 
+00031ac0: 2020 2020 2020 2023 2043 6f75 6e74 2074         # Count t
+00031ad0: 6865 206e 756d 6265 7220 6f66 2066 696c  he number of fil
+00031ae0: 6573 2077 6974 6820 7468 6520 6769 7665  es with the give
+00031af0: 6e20 6669 6c65 206e 616d 650a 2020 2020  n file name.    
+00031b00: 2020 2020 7570 5f63 6d64 203d 2073 656c      up_cmd = sel
+00031b10: 662e 636c 695f 636f 756e 745f 6e61 6d65  f.cli_count_name
+00031b20: 5f69 6e5f 6275 636b 6574 2873 746f 7265  _in_bucket(store
+00031b30: 5f74 7970 652c 205c 0a20 2020 2020 2020  _type, \.       
+00031b40: 2020 2020 2074 6d70 5f67 6974 6967 6e6f       tmp_gitigno
+00031b50: 7265 5f73 746f 7261 6765 5f6f 626a 2e6e  re_storage_obj.n
+00031b60: 616d 652c 2066 696c 655f 6e61 6d65 3d75  ame, file_name=u
+00031b70: 706c 6f61 645f 6669 6c65 5f6e 616d 6529  pload_file_name)
+00031b80: 0a20 2020 2020 2020 2067 6974 5f65 7863  .        git_exc
+00031b90: 6c75 6465 5f63 6d64 203d 2073 656c 662e  lude_cmd = self.
+00031ba0: 636c 695f 636f 756e 745f 6e61 6d65 5f69  cli_count_name_i
+00031bb0: 6e5f 6275 636b 6574 2873 746f 7265 5f74  n_bucket(store_t
+00031bc0: 7970 652c 205c 0a20 2020 2020 2020 2020  ype, \.         
+00031bd0: 2020 2074 6d70 5f67 6974 6967 6e6f 7265     tmp_gitignore
+00031be0: 5f73 746f 7261 6765 5f6f 626a 2e6e 616d  _storage_obj.nam
+00031bf0: 652c 2066 696c 655f 6e61 6d65 3d27 2e67  e, file_name='.g
+00031c00: 6974 2729 0a20 2020 2020 2020 2063 6e74  it').        cnt
+00031c10: 5f6e 756d 5f66 696c 655f 636d 6420 3d20  _num_file_cmd = 
+00031c20: 7365 6c66 2e63 6c69 5f63 6f75 6e74 5f66  self.cli_count_f
+00031c30: 696c 655f 696e 5f62 7563 6b65 7428 0a20  ile_in_bucket(. 
+00031c40: 2020 2020 2020 2020 2020 2073 746f 7265             store
+00031c50: 5f74 7970 652c 2074 6d70 5f67 6974 6967  _type, tmp_gitig
+00031c60: 6e6f 7265 5f73 746f 7261 6765 5f6f 626a  nore_storage_obj
+00031c70: 2e6e 616d 6529 0a0a 2020 2020 2020 2020  .name)..        
+00031c80: 7570 5f6f 7574 7075 7420 3d20 7375 6270  up_output = subp
+00031c90: 726f 6365 7373 2e63 6865 636b 5f6f 7574  rocess.check_out
+00031ca0: 7075 7428 7570 5f63 6d64 2c20 7368 656c  put(up_cmd, shel
+00031cb0: 6c3d 5472 7565 290a 2020 2020 2020 2020  l=True).        
+00031cc0: 6769 745f 6578 636c 7564 655f 6f75 7470  git_exclude_outp
+00031cd0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+00031ce0: 6368 6563 6b5f 6f75 7470 7574 2867 6974  check_output(git
+00031cf0: 5f65 7863 6c75 6465 5f63 6d64 2c0a 2020  _exclude_cmd,.  
+00031d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031d30: 2020 2073 6865 6c6c 3d54 7275 6529 0a20     shell=True). 
+00031d40: 2020 2020 2020 2063 6e74 5f6f 7574 7075         cnt_outpu
+00031d50: 7420 3d20 7375 6270 726f 6365 7373 2e63  t = subprocess.c
+00031d60: 6865 636b 5f6f 7574 7075 7428 636e 745f  heck_output(cnt_
+00031d70: 6e75 6d5f 6669 6c65 5f63 6d64 2c20 7368  num_file_cmd, sh
+00031d80: 656c 6c3d 5472 7565 290a 0a20 2020 2020  ell=True)..     
+00031d90: 2020 2061 7373 6572 7420 2733 2720 696e     assert '3' in
+00031da0: 2075 705f 6f75 7470 7574 2e64 6563 6f64   up_output.decod
+00031db0: 6528 2775 7466 2d38 2729 2c20 5c0a 2020  e('utf-8'), \.  
+00031dc0: 2020 2020 2020 2020 2020 2020 2020 2746                'F
+00031dd0: 696c 6573 2074 6f20 6265 2069 6e63 6c75  iles to be inclu
+00031de0: 6465 6420 6172 6520 6e6f 7420 636f 6d70  ded are not comp
+00031df0: 6c65 7465 6c79 2075 706c 6f61 6465 642e  letely uploaded.
+00031e00: 270a 2020 2020 2020 2020 2320 3120 6973  '.        # 1 is
+00031e10: 2072 6561 6420 6173 202e 6769 7469 676e   read as .gitign
+00031e20: 6f72 6520 6973 2075 706c 6f61 6465 640a  ore is uploaded.
+00031e30: 2020 2020 2020 2020 6173 7365 7274 2027          assert '
+00031e40: 3127 2069 6e20 6769 745f 6578 636c 7564  1' in git_exclud
+00031e50: 655f 6f75 7470 7574 2e64 6563 6f64 6528  e_output.decode(
+00031e60: 2775 7466 2d38 2729 2c20 5c0a 2020 2020  'utf-8'), \.    
+00031e70: 2020 2020 2020 2020 2020 2027 2e67 6974             '.git
+00031e80: 2064 6972 6563 746f 7279 2073 686f 756c   directory shoul
+00031e90: 6420 6e6f 7420 6265 2075 706c 6f61 6465  d not be uploade
+00031ea0: 642e 270a 2020 2020 2020 2020 2320 3420  d.'.        # 4 
+00031eb0: 6669 6c65 7320 696e 636c 7564 6520 2e67  files include .g
+00031ec0: 6974 6967 6e6f 7265 2c20 696e 636c 7564  itignore, includ
+00031ed0: 6564 2e6c 6f67 2c20 696e 636c 7564 6564  ed.log, included
+00031ee0: 2e74 7874 2c20 696e 636c 7564 655f 6469  .txt, include_di
+00031ef0: 722f 696e 636c 7564 6564 2e6c 6f67 0a20  r/included.log. 
+00031f00: 2020 2020 2020 2061 7373 6572 7420 2734         assert '4
+00031f10: 2720 696e 2063 6e74 5f6f 7574 7075 742e  ' in cnt_output.
+00031f20: 6465 636f 6465 2827 7574 662d 3827 292c  decode('utf-8'),
+00031f30: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00031f40: 2020 2753 6f6d 6520 6974 656d 7320 6c69    'Some items li
+00031f50: 7374 6564 2069 6e20 2e67 6974 6967 6e6f  sted in .gitigno
+00031f60: 7265 2061 6e64 202e 6769 742f 696e 666f  re and .git/info
+00031f70: 2f65 7863 6c75 6465 2061 7265 206e 6f74  /exclude are not
+00031f80: 2065 7863 6c75 6465 642e 270a 0a20 2020   excluded.'..   
+00031f90: 2040 7079 7465 7374 2e6d 6172 6b2e 7061   @pytest.mark.pa
+00031fa0: 7261 6d65 7472 697a 6528 2765 7874 5f62  rametrize('ext_b
+00031fb0: 7563 6b65 745f 6669 7874 7572 652c 2073  ucket_fixture, s
+00031fc0: 746f 7265 5f74 7970 6527 2c0a 2020 2020  tore_type',.    
+00031fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00031fe0: 2020 2020 2020 2020 205b 2827 746d 705f           [('tmp_
+00031ff0: 6177 7363 6c69 5f62 7563 6b65 7427 2c20  awscli_bucket', 
+00032000: 7374 6f72 6167 655f 6c69 622e 5374 6f72  storage_lib.Stor
+00032010: 6554 7970 652e 5333 292c 0a20 2020 2020  eType.S3),.     
+00032020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032030: 2020 2020 2020 2020 2028 2774 6d70 5f67           ('tmp_g
+00032040: 7375 7469 6c5f 6275 636b 6574 272c 2073  sutil_bucket', s
+00032050: 746f 7261 6765 5f6c 6962 2e53 746f 7265  torage_lib.Store
+00032060: 5479 7065 2e47 4353 292c 0a20 2020 2020  Type.GCS),.     
+00032070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032080: 2020 2020 2020 2020 2070 7974 6573 742e           pytest.
+00032090: 7061 7261 6d28 2774 6d70 5f61 7773 636c  param('tmp_awscl
+000320a0: 695f 6275 636b 6574 5f72 3227 2c0a 2020  i_bucket_r2',.  
+000320b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000320c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000320d0: 2020 2020 2020 2020 2073 746f 7261 6765           storage
+000320e0: 5f6c 6962 2e53 746f 7265 5479 7065 2e52  _lib.StoreType.R
+000320f0: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
+00032100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032110: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00032120: 726b 733d 7079 7465 7374 2e6d 6172 6b2e  rks=pytest.mark.
+00032130: 636c 6f75 6466 6c61 7265 295d 290a 2020  cloudflare)]).  
+00032140: 2020 6465 6620 7465 7374 5f65 7874 6572    def test_exter
+00032150: 6e61 6c6c 795f 6372 6561 7465 645f 6275  nally_created_bu
+00032160: 636b 6574 5f6d 6f75 6e74 5f77 6974 686f  cket_mount_witho
+00032170: 7574 5f73 6f75 7263 6528 0a20 2020 2020  ut_source(.     
+00032180: 2020 2020 2020 2073 656c 662c 2065 7874         self, ext
+00032190: 5f62 7563 6b65 745f 6669 7874 7572 652c  _bucket_fixture,
+000321a0: 2072 6571 7565 7374 2c20 7374 6f72 655f   request, store_
+000321b0: 7479 7065 293a 0a20 2020 2020 2020 2023  type):.        #
+000321c0: 204e 6f6e 2d73 6b79 206d 616e 6167 6564   Non-sky managed
+000321d0: 2062 7563 6b65 7473 2862 7563 6b65 7473   buckets(buckets
+000321e0: 2063 7265 6174 6564 206f 7574 7369 6465   created outside
+000321f0: 206f 6620 536b 7970 696c 6f74 2043 4c49   of Skypilot CLI
+00032200: 290a 2020 2020 2020 2020 2320 6172 6520  ).        # are 
+00032210: 616c 6c6f 7765 6420 746f 2062 6520 4d4f  allowed to be MO
+00032220: 554e 5465 6420 6279 2073 7065 6369 6679  UNTed by specify
+00032230: 696e 6720 7468 6520 5552 4920 6f66 2074  ing the URI of t
+00032240: 6865 2062 7563 6b65 7420 746f 0a20 2020  he bucket to.   
+00032250: 2020 2020 2023 2073 6f75 7263 6520 6669       # source fi
+00032260: 656c 6420 6f6e 6c79 2e20 5768 656e 2069  eld only. When i
+00032270: 7420 6973 2061 7474 656d 7074 6564 2062  t is attempted b
+00032280: 7920 7370 6563 6966 7969 6e67 2074 6865  y specifying the
+00032290: 206e 616d 6520 6f66 0a20 2020 2020 2020   name of.       
+000322a0: 2023 2074 6865 2062 7563 6b65 7420 6f6e   # the bucket on
+000322b0: 6c79 2c20 6974 2073 686f 756c 6420 6572  ly, it should er
+000322c0: 726f 7220 6f75 742e 0a20 2020 2020 2020  ror out..       
+000322d0: 2023 0a20 2020 2020 2020 2023 2054 4f44   #.        # TOD
+000322e0: 4f28 646f 796f 756e 6729 3a20 4164 6420  O(doyoung): Add 
+000322f0: 7465 7374 2066 6f72 2049 424d 2043 4f53  test for IBM COS
+00032300: 2e20 4375 7272 656e 746c 792c 2074 6869  . Currently, thi
+00032310: 7320 6973 2062 6c6f 636b 6564 0a20 2020  s is blocked.   
+00032320: 2020 2020 2023 2061 7320 7263 6c6f 6e65       # as rclone
+00032330: 2075 7365 6420 746f 2069 6e74 6572 6163   used to interac
+00032340: 7420 7769 7468 2049 424d 2043 4f53 2064  t with IBM COS d
+00032350: 6f65 7320 6e6f 7420 7375 7070 6f72 7420  oes not support 
+00032360: 6665 6174 7572 6520 746f 0a20 2020 2020  feature to.     
+00032370: 2020 2023 2063 7265 6174 6520 6120 6275     # create a bu
+00032380: 636b 6574 2c20 616e 6420 7468 6520 6962  cket, and the ib
+00032390: 6d63 6c6f 7564 2043 4c49 2069 7320 6e6f  mcloud CLI is no
+000323a0: 7420 7375 7070 6f72 7465 6420 696e 2053  t supported in S
+000323b0: 6b79 7069 6c6f 742e 0a20 2020 2020 2020  kypilot..       
+000323c0: 2023 2045 6974 6865 7220 6f66 2074 6865   # Either of the
+000323d0: 2066 6561 7475 7265 2069 7320 6e65 6365   feature is nece
+000323e0: 7373 6172 7920 746f 2073 696d 756c 6174  ssary to simulat
+000323f0: 6520 616e 2065 7874 6572 6e61 6c20 6275  e an external bu
+00032400: 636b 6574 0a20 2020 2020 2020 2023 2063  cket.        # c
+00032410: 7265 6174 696f 6e20 666f 7220 4942 4d20  reation for IBM 
+00032420: 434f 532e 0a20 2020 2020 2020 2023 2068  COS..        # h
+00032430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00032440: 6d2f 736b 7970 696c 6f74 2d6f 7267 2f73  m/skypilot-org/s
+00032450: 6b79 7069 6c6f 742f 7075 6c6c 2f31 3936  kypilot/pull/196
+00032460: 362f 6669 6c65 7323 7231 3235 3334 3339  6/files#r1253439
+00032470: 3833 370a 0a20 2020 2020 2020 2065 7874  837..        ext
+00032480: 5f62 7563 6b65 745f 6e61 6d65 2c20 6578  _bucket_name, ex
+00032490: 745f 6275 636b 6574 5f75 7269 203d 2072  t_bucket_uri = r
+000324a0: 6571 7565 7374 2e67 6574 6669 7874 7572  equest.getfixtur
+000324b0: 6576 616c 7565 280a 2020 2020 2020 2020  evalue(.        
+000324c0: 2020 2020 6578 745f 6275 636b 6574 5f66      ext_bucket_f
+000324d0: 6978 7475 7265 290a 2020 2020 2020 2020  ixture).        
+000324e0: 2320 696e 7661 6c69 6420 7370 6563 0a20  # invalid spec. 
+000324f0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+00032500: 7374 2e72 6169 7365 7328 736b 792e 6578  st.raises(sky.ex
+00032510: 6365 7074 696f 6e73 2e53 746f 7261 6765  ceptions.Storage
+00032520: 5370 6563 4572 726f 7229 2061 7320 653a  SpecError) as e:
+00032530: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
+00032540: 7261 6765 5f6f 626a 203d 2073 746f 7261  rage_obj = stora
+00032550: 6765 5f6c 6962 2e53 746f 7261 6765 280a  ge_lib.Storage(.
+00032560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032570: 6e61 6d65 3d65 7874 5f62 7563 6b65 745f  name=ext_bucket_
+00032580: 6e61 6d65 2c20 6d6f 6465 3d73 746f 7261  name, mode=stora
+00032590: 6765 5f6c 6962 2e53 746f 7261 6765 4d6f  ge_lib.StorageMo
+000325a0: 6465 2e4d 4f55 4e54 290a 2020 2020 2020  de.MOUNT).      
+000325b0: 2020 2020 2020 7374 6f72 6167 655f 6f62        storage_ob
+000325c0: 6a2e 6164 645f 7374 6f72 6528 7374 6f72  j.add_store(stor
+000325d0: 655f 7479 7065 290a 0a20 2020 2020 2020  e_type)..       
+000325e0: 2061 7373 6572 7420 2741 7474 656d 7074   assert 'Attempt
+000325f0: 6564 2074 6f20 6d6f 756e 7420 6120 6e6f  ed to mount a no
+00032600: 6e2d 736b 7920 6d61 6e61 6765 6420 6275  n-sky managed bu
+00032610: 636b 6574 2720 696e 2073 7472 2865 290a  cket' in str(e).
+00032620: 0a20 2020 2020 2020 2023 2076 616c 6964  .        # valid
+00032630: 2073 7065 630a 2020 2020 2020 2020 7374   spec.        st
+00032640: 6f72 6167 655f 6f62 6a20 3d20 7374 6f72  orage_obj = stor
+00032650: 6167 655f 6c69 622e 5374 6f72 6167 6528  age_lib.Storage(
+00032660: 736f 7572 6365 3d65 7874 5f62 7563 6b65  source=ext_bucke
+00032670: 745f 7572 692c 0a20 2020 2020 2020 2020  t_uri,.         
+00032680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00032690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000326a0: 206d 6f64 653d 7374 6f72 6167 655f 6c69   mode=storage_li
+000326b0: 622e 5374 6f72 6167 654d 6f64 652e 4d4f  b.StorageMode.MO
+000326c0: 554e 5429 0a20 2020 2020 2020 2068 616e  UNT).        han
+000326d0: 646c 6520 3d20 676c 6f62 616c 5f75 7365  dle = global_use
+000326e0: 725f 7374 6174 652e 6765 745f 6861 6e64  r_state.get_hand
+000326f0: 6c65 5f66 726f 6d5f 7374 6f72 6167 655f  le_from_storage_
+00032700: 6e61 6d65 280a 2020 2020 2020 2020 2020  name(.          
+00032710: 2020 7374 6f72 6167 655f 6f62 6a2e 6e61    storage_obj.na
+00032720: 6d65 290a 2020 2020 2020 2020 6966 2068  me).        if h
+00032730: 616e 646c 653a 0a20 2020 2020 2020 2020  andle:.         
+00032740: 2020 2073 746f 7261 6765 5f6f 626a 2e64     storage_obj.d
+00032750: 656c 6574 6528 290a 0a20 2020 2040 7079  elete()..    @py
+00032760: 7465 7374 2e6d 6172 6b2e 6e6f 5f66 6c75  test.mark.no_flu
+00032770: 6964 7374 6163 6b0a 2020 2020 4070 7974  idstack.    @pyt
+00032780: 6573 742e 6d61 726b 2e70 6172 616d 6574  est.mark.paramet
+00032790: 7269 7a65 2827 7265 6769 6f6e 272c 205b  rize('region', [
+000327a0: 0a20 2020 2020 2020 2027 6170 2d6e 6f72  .        'ap-nor
+000327b0: 7468 6561 7374 2d31 272c 2027 6170 2d6e  theast-1', 'ap-n
+000327c0: 6f72 7468 6561 7374 2d32 272c 2027 6170  ortheast-2', 'ap
+000327d0: 2d6e 6f72 7468 6561 7374 2d33 272c 2027  -northeast-3', '
+000327e0: 6170 2d73 6f75 7468 2d31 272c 0a20 2020  ap-south-1',.   
+000327f0: 2020 2020 2027 6170 2d73 6f75 7468 6561       'ap-southea
+00032800: 7374 2d31 272c 2027 6170 2d73 6f75 7468  st-1', 'ap-south
+00032810: 6561 7374 2d32 272c 2027 6575 2d63 656e  east-2', 'eu-cen
+00032820: 7472 616c 2d31 272c 2027 6575 2d6e 6f72  tral-1', 'eu-nor
+00032830: 7468 2d31 272c 0a20 2020 2020 2020 2027  th-1',.        '
+00032840: 6575 2d77 6573 742d 3127 2c20 2765 752d  eu-west-1', 'eu-
+00032850: 7765 7374 2d32 272c 2027 6575 2d77 6573  west-2', 'eu-wes
+00032860: 742d 3327 2c20 2773 612d 6561 7374 2d31  t-3', 'sa-east-1
+00032870: 272c 2027 7573 2d65 6173 742d 3127 2c0a  ', 'us-east-1',.
+00032880: 2020 2020 2020 2020 2775 732d 6561 7374          'us-east
+00032890: 2d32 272c 2027 7573 2d77 6573 742d 3127  -2', 'us-west-1'
+000328a0: 2c20 2775 732d 7765 7374 2d32 270a 2020  , 'us-west-2'.  
+000328b0: 2020 5d29 0a20 2020 2064 6566 2074 6573    ]).    def tes
+000328c0: 745f 6177 735f 7265 6769 6f6e 7328 7365  t_aws_regions(se
+000328d0: 6c66 2c20 746d 705f 6c6f 6361 6c5f 7374  lf, tmp_local_st
+000328e0: 6f72 6167 655f 6f62 6a2c 2072 6567 696f  orage_obj, regio
+000328f0: 6e29 3a0a 2020 2020 2020 2020 2320 5468  n):.        # Th
+00032900: 6973 2074 6573 7473 2063 7265 6174 696f  is tests creatio
+00032910: 6e20 616e 6420 7570 6c6f 6164 2074 6f20  n and upload to 
+00032920: 6275 636b 6574 2069 6e20 616c 6c20 4157  bucket in all AW
+00032930: 5320 7333 2072 6567 696f 6e73 0a20 2020  S s3 regions.   
+00032940: 2020 2020 2023 2054 6f20 7465 7374 2066       # To test f
+00032950: 756c 6c20 6675 6e63 7469 6f6e 616c 6974  ull functionalit
+00032960: 792c 2075 7365 2074 6573 745f 6d61 6e61  y, use test_mana
+00032970: 6765 645f 6a6f 6273 5f73 746f 7261 6765  ged_jobs_storage
+00032980: 2061 626f 7665 2e0a 2020 2020 2020 2020   above..        
+00032990: 7374 6f72 655f 7479 7065 203d 2073 746f  store_type = sto
+000329a0: 7261 6765 5f6c 6962 2e53 746f 7265 5479  rage_lib.StoreTy
+000329b0: 7065 2e53 330a 2020 2020 2020 2020 746d  pe.S3.        tm
+000329c0: 705f 6c6f 6361 6c5f 7374 6f72 6167 655f  p_local_storage_
+000329d0: 6f62 6a2e 6164 645f 7374 6f72 6528 7374  obj.add_store(st
+000329e0: 6f72 655f 7479 7065 2c20 7265 6769 6f6e  ore_type, region
+000329f0: 3d72 6567 696f 6e29 0a20 2020 2020 2020  =region).       
+00032a00: 2062 7563 6b65 745f 6e61 6d65 203d 2074   bucket_name = t
+00032a10: 6d70 5f6c 6f63 616c 5f73 746f 7261 6765  mp_local_storage
+00032a20: 5f6f 626a 2e6e 616d 650a 0a20 2020 2020  _obj.name..     
+00032a30: 2020 2023 2043 6f6e 6669 726d 2074 6861     # Confirm tha
+00032a40: 7420 7468 6520 6275 636b 6574 2077 6173  t the bucket was
+00032a50: 2063 7265 6174 6564 2069 6e20 7468 6520   created in the 
+00032a60: 636f 7272 6563 7420 7265 6769 6f6e 0a20  correct region. 
+00032a70: 2020 2020 2020 2072 6567 696f 6e5f 636d         region_cm
+00032a80: 6420 3d20 7365 6c66 2e63 6c69 5f72 6567  d = self.cli_reg
+00032a90: 696f 6e5f 636d 6428 7374 6f72 655f 7479  ion_cmd(store_ty
+00032aa0: 7065 2c20 6275 636b 6574 5f6e 616d 6529  pe, bucket_name)
+00032ab0: 0a20 2020 2020 2020 206f 7574 203d 2073  .        out = s
+00032ac0: 7562 7072 6f63 6573 732e 6368 6563 6b5f  ubprocess.check_
+00032ad0: 6f75 7470 7574 2872 6567 696f 6e5f 636d  output(region_cm
+00032ae0: 642c 2073 6865 6c6c 3d54 7275 6529 0a20  d, shell=True). 
+00032af0: 2020 2020 2020 206f 7574 7075 7420 3d20         output = 
+00032b00: 6f75 742e 6465 636f 6465 2827 7574 662d  out.decode('utf-
+00032b10: 3827 290a 2020 2020 2020 2020 6578 7065  8').        expe
+00032b20: 6374 6564 5f6f 7574 7075 745f 7265 6769  cted_output_regi
+00032b30: 6f6e 203d 2072 6567 696f 6e0a 2020 2020  on = region.    
+00032b40: 2020 2020 6966 2072 6567 696f 6e20 3d3d      if region ==
+00032b50: 2027 7573 2d65 6173 742d 3127 3a0a 2020   'us-east-1':.  
+00032b60: 2020 2020 2020 2020 2020 6578 7065 6374            expect
+00032b70: 6564 5f6f 7574 7075 745f 7265 6769 6f6e  ed_output_region
+00032b80: 203d 2027 4e6f 6e65 2720 2023 2075 732d   = 'None'  # us-
+00032b90: 6561 7374 2d31 2069 7320 7468 6520 6465  east-1 is the de
+00032ba0: 6661 756c 7420 7265 6769 6f6e 0a20 2020  fault region.   
+00032bb0: 2020 2020 2061 7373 6572 7420 6578 7065       assert expe
+00032bc0: 6374 6564 5f6f 7574 7075 745f 7265 6769  cted_output_regi
+00032bd0: 6f6e 2069 6e20 6f75 742e 6465 636f 6465  on in out.decode
+00032be0: 2827 7574 662d 3827 292c 2028 0a20 2020  ('utf-8'), (.   
+00032bf0: 2020 2020 2020 2020 2066 2742 7563 6b65           f'Bucke
+00032c00: 7420 7761 7320 6e6f 7420 666f 756e 6420  t was not found 
+00032c10: 696e 2072 6567 696f 6e20 7b72 6567 696f  in region {regio
+00032c20: 6e7d 202d 2027 0a20 2020 2020 2020 2020  n} - '.         
+00032c30: 2020 2066 276f 7574 7075 7420 6f66 207b     f'output of {
+00032c40: 7265 6769 6f6e 5f63 6d64 7d20 7761 733a  region_cmd} was:
+00032c50: 207b 6f75 7470 7574 7d27 290a 0a20 2020   {output}')..   
+00032c60: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
+00032c70: 746d 705f 736f 7572 6365 2f74 6d70 2d66  tmp_source/tmp-f
+00032c80: 696c 6520 6578 6973 7473 2069 6e20 7468  ile exists in th
+00032c90: 6520 6275 636b 6574 2075 7369 6e67 2063  e bucket using c
+00032ca0: 6c69 0a20 2020 2020 2020 206c 735f 636d  li.        ls_cm
+00032cb0: 6420 3d20 7365 6c66 2e63 6c69 5f6c 735f  d = self.cli_ls_
+00032cc0: 636d 6428 7374 6f72 655f 7479 7065 2c20  cmd(store_type, 
+00032cd0: 6275 636b 6574 5f6e 616d 6529 0a20 2020  bucket_name).   
+00032ce0: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
+00032cf0: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+00032d00: 7574 286c 735f 636d 642c 2073 6865 6c6c  ut(ls_cmd, shell
+00032d10: 3d54 7275 6529 0a20 2020 2020 2020 206f  =True).        o
+00032d20: 7574 7075 7420 3d20 6f75 742e 6465 636f  utput = out.deco
+00032d30: 6465 2827 7574 662d 3827 290a 2020 2020  de('utf-8').    
+00032d40: 2020 2020 6173 7365 7274 2027 746d 702d      assert 'tmp-
+00032d50: 6669 6c65 2720 696e 206f 7574 7075 742c  file' in output,
+00032d60: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+00032d70: 2774 6d70 2d66 696c 6520 6e6f 7420 666f  'tmp-file not fo
+00032d80: 756e 6420 696e 2062 7563 6b65 7420 2d20  und in bucket - 
+00032d90: 6f75 7470 7574 206f 6620 7b6c 735f 636d  output of {ls_cm
+00032da0: 647d 2077 6173 3a20 7b6f 7574 7075 747d  d} was: {output}
+00032db0: 2729 0a0a 2020 2020 4070 7974 6573 742e  ')..    @pytest.
+00032dc0: 6d61 726b 2e6e 6f5f 666c 7569 6473 7461  mark.no_fluidsta
+00032dd0: 636b 0a20 2020 2040 7079 7465 7374 2e6d  ck.    @pytest.m
+00032de0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00032df0: 2772 6567 696f 6e27 2c20 5b0a 2020 2020  'region', [.    
+00032e00: 2020 2020 276e 6f72 7468 616d 6572 6963      'northameric
+00032e10: 612d 6e6f 7274 6865 6173 7431 272c 2027  a-northeast1', '
+00032e20: 6e6f 7274 6861 6d65 7269 6361 2d6e 6f72  northamerica-nor
+00032e30: 7468 6561 7374 3227 2c20 2775 732d 6365  theast2', 'us-ce
+00032e40: 6e74 7261 6c31 272c 0a20 2020 2020 2020  ntral1',.       
+00032e50: 2027 7573 2d65 6173 7431 272c 2027 7573   'us-east1', 'us
+00032e60: 2d65 6173 7434 272c 2027 7573 2d65 6173  -east4', 'us-eas
+00032e70: 7435 272c 2027 7573 2d73 6f75 7468 3127  t5', 'us-south1'
+00032e80: 2c20 2775 732d 7765 7374 3127 2c20 2775  , 'us-west1', 'u
+00032e90: 732d 7765 7374 3227 2c0a 2020 2020 2020  s-west2',.      
+00032ea0: 2020 2775 732d 7765 7374 3327 2c20 2775    'us-west3', 'u
+00032eb0: 732d 7765 7374 3427 2c20 2773 6f75 7468  s-west4', 'south
+00032ec0: 616d 6572 6963 612d 6561 7374 3127 2c20  america-east1', 
+00032ed0: 2773 6f75 7468 616d 6572 6963 612d 7765  'southamerica-we
+00032ee0: 7374 3127 2c0a 2020 2020 2020 2020 2765  st1',.        'e
+00032ef0: 7572 6f70 652d 6365 6e74 7261 6c32 272c  urope-central2',
+00032f00: 2027 6575 726f 7065 2d6e 6f72 7468 3127   'europe-north1'
+00032f10: 2c20 2765 7572 6f70 652d 736f 7574 6877  , 'europe-southw
+00032f20: 6573 7431 272c 2027 6575 726f 7065 2d77  est1', 'europe-w
+00032f30: 6573 7431 272c 0a20 2020 2020 2020 2027  est1',.        '
+00032f40: 6575 726f 7065 2d77 6573 7432 272c 2027  europe-west2', '
+00032f50: 6575 726f 7065 2d77 6573 7433 272c 2027  europe-west3', '
+00032f60: 6575 726f 7065 2d77 6573 7434 272c 2027  europe-west4', '
+00032f70: 6575 726f 7065 2d77 6573 7436 272c 0a20  europe-west6',. 
+00032f80: 2020 2020 2020 2027 6575 726f 7065 2d77         'europe-w
+00032f90: 6573 7438 272c 2027 6575 726f 7065 2d77  est8', 'europe-w
+00032fa0: 6573 7439 272c 2027 6575 726f 7065 2d77  est9', 'europe-w
+00032fb0: 6573 7431 3027 2c20 2765 7572 6f70 652d  est10', 'europe-
+00032fc0: 7765 7374 3132 272c 0a20 2020 2020 2020  west12',.       
+00032fd0: 2027 6173 6961 2d65 6173 7431 272c 2027   'asia-east1', '
+00032fe0: 6173 6961 2d65 6173 7432 272c 2027 6173  asia-east2', 'as
+00032ff0: 6961 2d6e 6f72 7468 6561 7374 3127 2c20  ia-northeast1', 
+00033000: 2761 7369 612d 6e6f 7274 6865 6173 7432  'asia-northeast2
+00033010: 272c 0a20 2020 2020 2020 2027 6173 6961  ',.        'asia
+00033020: 2d6e 6f72 7468 6561 7374 3327 2c20 2761  -northeast3', 'a
+00033030: 7369 612d 736f 7574 6865 6173 7431 272c  sia-southeast1',
+00033040: 2027 6173 6961 2d73 6f75 7468 3127 2c20   'asia-south1', 
+00033050: 2761 7369 612d 736f 7574 6832 272c 0a20  'asia-south2',. 
+00033060: 2020 2020 2020 2027 6173 6961 2d73 6f75         'asia-sou
+00033070: 7468 6561 7374 3227 2c20 276d 652d 6365  theast2', 'me-ce
+00033080: 6e74 7261 6c31 272c 2027 6d65 2d63 656e  ntral1', 'me-cen
+00033090: 7472 616c 3227 2c20 276d 652d 7765 7374  tral2', 'me-west
+000330a0: 3127 2c0a 2020 2020 2020 2020 2761 7573  1',.        'aus
+000330b0: 7472 616c 6961 2d73 6f75 7468 6561 7374  tralia-southeast
+000330c0: 3127 2c20 2761 7573 7472 616c 6961 2d73  1', 'australia-s
+000330d0: 6f75 7468 6561 7374 3227 2c20 2761 6672  outheast2', 'afr
+000330e0: 6963 612d 736f 7574 6831 270a 2020 2020  ica-south1'.    
+000330f0: 5d29 0a20 2020 2064 6566 2074 6573 745f  ]).    def test_
+00033100: 6763 735f 7265 6769 6f6e 7328 7365 6c66  gcs_regions(self
+00033110: 2c20 746d 705f 6c6f 6361 6c5f 7374 6f72  , tmp_local_stor
+00033120: 6167 655f 6f62 6a2c 2072 6567 696f 6e29  age_obj, region)
+00033130: 3a0a 2020 2020 2020 2020 2320 5468 6973  :.        # This
+00033140: 2074 6573 7473 2063 7265 6174 696f 6e20   tests creation 
+00033150: 616e 6420 7570 6c6f 6164 2074 6f20 6275  and upload to bu
+00033160: 636b 6574 2069 6e20 616c 6c20 4743 5320  cket in all GCS 
+00033170: 7265 6769 6f6e 730a 2020 2020 2020 2020  regions.        
+00033180: 2320 546f 2074 6573 7420 6675 6c6c 2066  # To test full f
+00033190: 756e 6374 696f 6e61 6c69 7479 2c20 7573  unctionality, us
+000331a0: 6520 7465 7374 5f6d 616e 6167 6564 5f6a  e test_managed_j
+000331b0: 6f62 735f 7374 6f72 6167 6520 6162 6f76  obs_storage abov
+000331c0: 652e 0a20 2020 2020 2020 2073 746f 7265  e..        store
+000331d0: 5f74 7970 6520 3d20 7374 6f72 6167 655f  _type = storage_
+000331e0: 6c69 622e 5374 6f72 6554 7970 652e 4743  lib.StoreType.GC
+000331f0: 530a 2020 2020 2020 2020 746d 705f 6c6f  S.        tmp_lo
+00033200: 6361 6c5f 7374 6f72 6167 655f 6f62 6a2e  cal_storage_obj.
+00033210: 6164 645f 7374 6f72 6528 7374 6f72 655f  add_store(store_
+00033220: 7479 7065 2c20 7265 6769 6f6e 3d72 6567  type, region=reg
+00033230: 696f 6e29 0a20 2020 2020 2020 2062 7563  ion).        buc
+00033240: 6b65 745f 6e61 6d65 203d 2074 6d70 5f6c  ket_name = tmp_l
+00033250: 6f63 616c 5f73 746f 7261 6765 5f6f 626a  ocal_storage_obj
+00033260: 2e6e 616d 650a 0a20 2020 2020 2020 2023  .name..        #
+00033270: 2043 6f6e 6669 726d 2074 6861 7420 7468   Confirm that th
+00033280: 6520 6275 636b 6574 2077 6173 2063 7265  e bucket was cre
+00033290: 6174 6564 2069 6e20 7468 6520 636f 7272  ated in the corr
+000332a0: 6563 7420 7265 6769 6f6e 0a20 2020 2020  ect region.     
+000332b0: 2020 2072 6567 696f 6e5f 636d 6420 3d20     region_cmd = 
+000332c0: 7365 6c66 2e63 6c69 5f72 6567 696f 6e5f  self.cli_region_
+000332d0: 636d 6428 7374 6f72 655f 7479 7065 2c20  cmd(store_type, 
+000332e0: 6275 636b 6574 5f6e 616d 6529 0a20 2020  bucket_name).   
+000332f0: 2020 2020 206f 7574 203d 2073 7562 7072       out = subpr
+00033300: 6f63 6573 732e 6368 6563 6b5f 6f75 7470  ocess.check_outp
+00033310: 7574 2872 6567 696f 6e5f 636d 642c 2073  ut(region_cmd, s
+00033320: 6865 6c6c 3d54 7275 6529 0a20 2020 2020  hell=True).     
+00033330: 2020 206f 7574 7075 7420 3d20 6f75 742e     output = out.
+00033340: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
+00033350: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
+00033360: 6567 696f 6e20 696e 206f 7574 2e64 6563  egion in out.dec
+00033370: 6f64 6528 2775 7466 2d38 2729 2c20 280a  ode('utf-8'), (.
+00033380: 2020 2020 2020 2020 2020 2020 6627 4275              f'Bu
+00033390: 636b 6574 2077 6173 206e 6f74 2066 6f75  cket was not fou
+000333a0: 6e64 2069 6e20 7265 6769 6f6e 207b 7265  nd in region {re
+000333b0: 6769 6f6e 7d20 2d20 270a 2020 2020 2020  gion} - '.      
+000333c0: 2020 2020 2020 6627 6f75 7470 7574 206f        f'output o
+000333d0: 6620 7b72 6567 696f 6e5f 636d 647d 2077  f {region_cmd} w
+000333e0: 6173 3a20 7b6f 7574 7075 747d 2729 0a0a  as: {output}')..
+000333f0: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00033400: 6966 2074 6d70 5f73 6f75 7263 652f 746d  if tmp_source/tm
+00033410: 702d 6669 6c65 2065 7869 7374 7320 696e  p-file exists in
+00033420: 2074 6865 2062 7563 6b65 7420 7573 696e   the bucket usin
+00033430: 6720 636c 690a 2020 2020 2020 2020 6c73  g cli.        ls
+00033440: 5f63 6d64 203d 2073 656c 662e 636c 695f  _cmd = self.cli_
+00033450: 6c73 5f63 6d64 2873 746f 7265 5f74 7970  ls_cmd(store_typ
+00033460: 652c 2062 7563 6b65 745f 6e61 6d65 290a  e, bucket_name).
+00033470: 2020 2020 2020 2020 6f75 7420 3d20 7375          out = su
+00033480: 6270 726f 6365 7373 2e63 6865 636b 5f6f  bprocess.check_o
+00033490: 7574 7075 7428 6c73 5f63 6d64 2c20 7368  utput(ls_cmd, sh
+000334a0: 656c 6c3d 5472 7565 290a 2020 2020 2020  ell=True).      
+000334b0: 2020 6f75 7470 7574 203d 206f 7574 2e64    output = out.d
+000334c0: 6563 6f64 6528 2775 7466 2d38 2729 0a20  ecode('utf-8'). 
+000334d0: 2020 2020 2020 2061 7373 6572 7420 2774         assert 't
+000334e0: 6d70 2d66 696c 6527 2069 6e20 6f75 7470  mp-file' in outp
+000334f0: 7574 2c20 280a 2020 2020 2020 2020 2020  ut, (.          
+00033500: 2020 6627 746d 702d 6669 6c65 206e 6f74    f'tmp-file not
+00033510: 2066 6f75 6e64 2069 6e20 6275 636b 6574   found in bucket
+00033520: 202d 206f 7574 7075 7420 6f66 207b 6c73   - output of {ls
+00033530: 5f63 6d64 7d20 7761 733a 207b 6f75 7470  _cmd} was: {outp
+00033540: 7574 7d27 290a 0a0a 2320 2d2d 2d2d 2d2d  ut}')...# ------
+00033550: 2d2d 2d2d 2054 6573 7469 6e67 2059 414d  ---- Testing YAM
+00033560: 4c20 5370 6563 7320 2d2d 2d2d 2d2d 2d2d  L Specs --------
+00033570: 2d2d 0a23 204f 7572 2073 6b79 2073 746f  --.# Our sky sto
+00033580: 7261 6765 2072 6571 7569 7265 7320 6372  rage requires cr
+00033590: 6564 656e 7469 616c 7320 746f 2063 6865  edentials to che
+000335a0: 636b 2074 6865 2062 7563 6b65 7420 6578  ck the bucket ex
+000335b0: 6973 7461 6e63 6520 7768 656e 0a23 206c  istance when.# l
+000335c0: 6f61 6469 6e67 2061 2074 6173 6b20 6672  oading a task fr
+000335d0: 6f6d 2074 6865 2079 616d 6c20 6669 6c65  om the yaml file
+000335e0: 2c20 736f 2077 6520 6361 6e6e 6f74 206d  , so we cannot m
+000335f0: 616b 6520 6974 2061 2075 6e69 7420 7465  ake it a unit te
+00033600: 7374 2e0a 636c 6173 7320 5465 7374 5961  st..class TestYa
+00033610: 6d6c 5370 6563 733a 0a20 2020 2023 2054  mlSpecs:.    # T
+00033620: 4f44 4f28 7a68 7775 293a 2041 6464 2074  ODO(zhwu): Add t
+00033630: 6573 7420 666f 7220 6074 6f5f 7961 6d6c  est for `to_yaml
+00033640: 5f63 6f6e 6669 6760 2066 6f72 2074 6865  _config` for the
+00033650: 2053 746f 7261 6765 206f 626a 6563 742e   Storage object.
+00033660: 0a20 2020 2023 2020 5765 2073 686f 756c  .    #  We shoul
+00033670: 6420 6e6f 7420 7573 6520 6065 7861 6d70  d not use `examp
+00033680: 6c65 732f 7374 6f72 6167 655f 6465 6d6f  les/storage_demo
+00033690: 2e79 616d 6c60 2068 6572 652c 2073 696e  .yaml` here, sin
+000336a0: 6365 2069 7420 7265 7175 6972 6573 0a20  ce it requires. 
+000336b0: 2020 2023 2020 7573 6572 7320 746f 2065     #  users to e
+000336c0: 6e73 7572 6520 6275 636b 6574 206e 616d  nsure bucket nam
+000336d0: 6573 2074 6f20 6e6f 7420 6578 6973 7420  es to not exist 
+000336e0: 616e 642f 6f72 2062 6520 756e 6971 7565  and/or be unique
+000336f0: 2e0a 2020 2020 5f54 4553 545f 5941 4d4c  ..    _TEST_YAML
+00033700: 5f50 4154 4853 203d 205b 0a20 2020 2020  _PATHS = [.     
+00033710: 2020 2027 6578 616d 706c 6573 2f6d 696e     'examples/min
+00033720: 696d 616c 2e79 616d 6c27 2c20 2765 7861  imal.yaml', 'exa
+00033730: 6d70 6c65 732f 6d61 6e61 6765 645f 6a6f  mples/managed_jo
+00033740: 622e 7961 6d6c 272c 0a20 2020 2020 2020  b.yaml',.       
+00033750: 2027 6578 616d 706c 6573 2f75 7369 6e67   'examples/using
+00033760: 5f66 696c 655f 6d6f 756e 7473 2e79 616d  _file_mounts.yam
+00033770: 6c27 2c20 2765 7861 6d70 6c65 732f 7265  l', 'examples/re
+00033780: 736e 6574 5f61 7070 2e79 616d 6c27 2c0a  snet_app.yaml',.
+00033790: 2020 2020 2020 2020 2765 7861 6d70 6c65          'example
+000337a0: 732f 6d75 6c74 695f 686f 7374 6e61 6d65  s/multi_hostname
+000337b0: 2e79 616d 6c27 0a20 2020 205d 0a0a 2020  .yaml'.    ]..  
+000337c0: 2020 6465 6620 5f69 735f 6469 6374 5f73    def _is_dict_s
+000337d0: 7562 7365 7428 7365 6c66 2c20 6431 2c20  ubset(self, d1, 
+000337e0: 6432 293a 0a20 2020 2020 2020 2022 2222  d2):.        """
+000337f0: 4368 6563 6b20 6966 2064 3120 6973 2074  Check if d1 is t
+00033800: 6865 2073 7562 7365 7420 6f66 2064 322e  he subset of d2.
+00033810: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
+00033820: 6b2c 2076 2069 6e20 6431 2e69 7465 6d73  k, v in d1.items
+00033830: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00033840: 6966 206b 206e 6f74 2069 6e20 6432 3a0a  if k not in d2:.
+00033850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033860: 6966 2069 7369 6e73 7461 6e63 6528 762c  if isinstance(v,
+00033870: 206c 6973 7429 206f 7220 6973 696e 7374   list) or isinst
+00033880: 616e 6365 2876 2c20 6469 6374 293a 0a20  ance(v, dict):. 
+00033890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000338a0: 2020 2061 7373 6572 7420 6c65 6e28 7629     assert len(v)
+000338b0: 203d 3d20 302c 2028 6b2c 2076 290a 2020   == 0, (k, v).  
+000338c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000338d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000338e0: 2020 2020 2020 2020 6173 7365 7274 2046          assert F
+000338f0: 616c 7365 2c20 286b 2c20 7629 0a20 2020  alse, (k, v).   
+00033900: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00033910: 696e 7374 616e 6365 2876 2c20 6469 6374  instance(v, dict
+00033920: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00033930: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+00033940: 616e 6365 2864 325b 6b5d 2c20 6469 6374  ance(d2[k], dict
+00033950: 292c 2028 6b2c 2076 2c20 6432 290a 2020  ), (k, v, d2).  
+00033960: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00033970: 6c66 2e5f 6973 5f64 6963 745f 7375 6273  lf._is_dict_subs
+00033980: 6574 2876 2c20 6432 5b6b 5d29 0a20 2020  et(v, d2[k]).   
+00033990: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+000339a0: 696e 7374 616e 6365 2876 2c20 7374 7229  instance(v, str)
+000339b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000339c0: 2020 6966 206b 203d 3d20 2761 6363 656c    if k == 'accel
+000339d0: 6572 6174 6f72 7327 3a0a 2020 2020 2020  erators':.      
+000339e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000339f0: 736f 7572 6365 7320 3d20 736b 792e 5265  sources = sky.Re
+00033a00: 736f 7572 6365 7328 290a 2020 2020 2020  sources().      
+00033a10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00033a20: 736f 7572 6365 732e 5f73 6574 5f61 6363  sources._set_acc
+00033a30: 656c 6572 6174 6f72 7328 762c 204e 6f6e  elerators(v, Non
+00033a40: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00033a50: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+00033a60: 736f 7572 6365 732e 6163 6365 6c65 7261  sources.accelera
+00033a70: 746f 7273 203d 3d20 6432 5b6b 5d2c 2028  tors == d2[k], (
+00033a80: 6b2c 2076 2c20 6432 290a 2020 2020 2020  k, v, d2).      
+00033a90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00033aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033ab0: 2020 2020 6173 7365 7274 2076 2e6c 6f77      assert v.low
+00033ac0: 6572 2829 203d 3d20 6432 5b6b 5d2e 6c6f  er() == d2[k].lo
+00033ad0: 7765 7228 292c 2028 6b2c 2076 2c20 6432  wer(), (k, v, d2
+00033ae0: 5b6b 5d29 0a20 2020 2020 2020 2020 2020  [k]).           
+00033af0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00033b00: 2020 2020 2020 2061 7373 6572 7420 7620         assert v 
+00033b10: 3d3d 2064 325b 6b5d 2c20 286b 2c20 762c  == d2[k], (k, v,
+00033b20: 2064 325b 6b5d 290a 0a20 2020 2064 6566   d2[k])..    def
+00033b30: 205f 6368 6563 6b5f 6571 7569 7661 6c65   _check_equivale
+00033b40: 6e74 2873 656c 662c 2079 616d 6c5f 7061  nt(self, yaml_pa
+00033b50: 7468 293a 0a20 2020 2020 2020 2022 2222  th):.        """
+00033b60: 4368 6563 6b20 6966 2074 6865 2079 616d  Check if the yam
+00033b70: 6c20 6973 2065 7175 6976 616c 656e 7420  l is equivalent 
+00033b80: 6166 7465 7220 6c6f 6164 2061 6e64 2064  after load and d
+00033b90: 756d 7020 6167 6169 6e2e 2222 220a 2020  ump again.""".  
+00033ba0: 2020 2020 2020 6f72 6967 696e 5f74 6173        origin_tas
+00033bb0: 6b5f 636f 6e66 6967 203d 2063 6f6d 6d6f  k_config = commo
+00033bc0: 6e5f 7574 696c 732e 7265 6164 5f79 616d  n_utils.read_yam
+00033bd0: 6c28 7961 6d6c 5f70 6174 6829 0a0a 2020  l(yaml_path)..  
+00033be0: 2020 2020 2020 7461 736b 203d 2073 6b79        task = sky
+00033bf0: 2e54 6173 6b2e 6672 6f6d 5f79 616d 6c28  .Task.from_yaml(
+00033c00: 7961 6d6c 5f70 6174 6829 0a20 2020 2020  yaml_path).     
+00033c10: 2020 206e 6577 5f74 6173 6b5f 636f 6e66     new_task_conf
+00033c20: 6967 203d 2074 6173 6b2e 746f 5f79 616d  ig = task.to_yam
+00033c30: 6c5f 636f 6e66 6967 2829 0a20 2020 2020  l_config().     
+00033c40: 2020 2023 2064 3120 3c3d 2064 320a 2020     # d1 <= d2.  
+00033c50: 2020 2020 2020 7072 696e 7428 6f72 6967        print(orig
+00033c60: 696e 5f74 6173 6b5f 636f 6e66 6967 2c20  in_task_config, 
+00033c70: 6e65 775f 7461 736b 5f63 6f6e 6669 6729  new_task_config)
+00033c80: 0a20 2020 2020 2020 2073 656c 662e 5f69  .        self._i
+00033c90: 735f 6469 6374 5f73 7562 7365 7428 6f72  s_dict_subset(or
+00033ca0: 6967 696e 5f74 6173 6b5f 636f 6e66 6967  igin_task_config
+00033cb0: 2c20 6e65 775f 7461 736b 5f63 6f6e 6669  , new_task_confi
+00033cc0: 6729 0a0a 2020 2020 6465 6620 7465 7374  g)..    def test
+00033cd0: 5f6c 6f61 645f 6475 6d70 5f79 616d 6c5f  _load_dump_yaml_
+00033ce0: 636f 6e66 6967 5f65 7175 6976 616c 656e  config_equivalen
+00033cf0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00033d00: 2022 2222 5465 7374 2069 6620 7468 6520   """Test if the 
+00033d10: 7961 6d6c 2063 6f6e 6669 6720 6973 2065  yaml config is e
+00033d20: 7175 6976 616c 656e 7420 6166 7465 7220  quivalent after 
+00033d30: 6c6f 6164 2061 6e64 2064 756d 7020 6167  load and dump ag
+00033d40: 6169 6e2e 2222 220a 2020 2020 2020 2020  ain.""".        
+00033d50: 7061 7468 6c69 622e 5061 7468 2827 7e2f  pathlib.Path('~/
+00033d60: 6461 7461 7365 7473 2729 2e65 7870 616e  datasets').expan
+00033d70: 6475 7365 7228 292e 6d6b 6469 7228 6578  duser().mkdir(ex
+00033d80: 6973 745f 6f6b 3d54 7275 6529 0a20 2020  ist_ok=True).   
+00033d90: 2020 2020 2070 6174 686c 6962 2e50 6174       pathlib.Pat
+00033da0: 6828 277e 2f74 6d70 6669 6c65 2729 2e65  h('~/tmpfile').e
+00033db0: 7870 616e 6475 7365 7228 292e 746f 7563  xpanduser().touc
+00033dc0: 6828 290a 2020 2020 2020 2020 7061 7468  h().        path
+00033dd0: 6c69 622e 5061 7468 2827 7e2f 2e73 7368  lib.Path('~/.ssh
+00033de0: 2729 2e65 7870 616e 6475 7365 7228 292e  ').expanduser().
+00033df0: 6d6b 6469 7228 6578 6973 745f 6f6b 3d54  mkdir(exist_ok=T
+00033e00: 7275 6529 0a20 2020 2020 2020 2070 6174  rue).        pat
+00033e10: 686c 6962 2e50 6174 6828 277e 2f2e 7373  hlib.Path('~/.ss
+00033e20: 682f 6964 5f72 7361 2e70 7562 2729 2e65  h/id_rsa.pub').e
+00033e30: 7870 616e 6475 7365 7228 292e 746f 7563  xpanduser().touc
+00033e40: 6828 290a 2020 2020 2020 2020 7061 7468  h().        path
+00033e50: 6c69 622e 5061 7468 2827 7e2f 746d 702d  lib.Path('~/tmp-
+00033e60: 776f 726b 6469 7227 292e 6578 7061 6e64  workdir').expand
+00033e70: 7573 6572 2829 2e6d 6b64 6972 2865 7869  user().mkdir(exi
+00033e80: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
+00033e90: 2020 2020 7061 7468 6c69 622e 5061 7468      pathlib.Path
+00033ea0: 2827 7e2f 446f 776e 6c6f 6164 732f 7470  ('~/Downloads/tp
+00033eb0: 7527 292e 6578 7061 6e64 7573 6572 2829  u').expanduser()
+00033ec0: 2e6d 6b64 6972 2870 6172 656e 7473 3d54  .mkdir(parents=T
+00033ed0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00033ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00033f10: 6578 6973 745f 6f6b 3d54 7275 6529 0a20  exist_ok=True). 
+00033f20: 2020 2020 2020 2066 6f72 2079 616d 6c5f         for yaml_
+00033f30: 7061 7468 2069 6e20 7365 6c66 2e5f 5445  path in self._TE
+00033f40: 5354 5f59 414d 4c5f 5041 5448 533a 0a20  ST_YAML_PATHS:. 
+00033f50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00033f60: 5f63 6865 636b 5f65 7175 6976 616c 656e  _check_equivalen
+00033f70: 7428 7961 6d6c 5f70 6174 6829 0a0a 0a23  t(yaml_path)...#
+00033f80: 202d 2d2d 2d2d 2d2d 2d2d 2d20 5465 7374   ---------- Test
+00033f90: 696e 6720 4d75 6c74 6970 6c65 2041 6363  ing Multiple Acc
+00033fa0: 656c 6572 6174 6f72 7320 2d2d 2d2d 2d2d  elerators ------
+00033fb0: 2d2d 2d2d 0a40 7079 7465 7374 2e6d 6172  ----.@pytest.mar
+00033fc0: 6b2e 6e6f 5f66 6c75 6964 7374 6163 6b20  k.no_fluidstack 
+00033fd0: 2023 2046 6c75 6964 7374 6163 6b20 646f   # Fluidstack do
+00033fe0: 6573 206e 6f74 2073 7570 706f 7274 204b  es not support K
+00033ff0: 3830 2067 7075 7320 666f 7220 6e6f 770a  80 gpus for now.
+00034000: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+00034010: 7061 7065 7273 7061 6365 2020 2320 5061  paperspace  # Pa
+00034020: 7065 7273 7061 6365 2064 6f65 7320 6e6f  perspace does no
+00034030: 7420 7375 7070 6f72 7420 4b38 3020 6770  t support K80 gp
+00034040: 7573 0a64 6566 2074 6573 745f 6d75 6c74  us.def test_mult
+00034050: 6970 6c65 5f61 6363 656c 6572 6174 6f72  iple_accelerator
+00034060: 735f 6f72 6465 7265 6428 293a 0a20 2020  s_ordered():.   
+00034070: 206e 616d 6520 3d20 5f67 6574 5f63 6c75   name = _get_clu
+00034080: 7374 6572 5f6e 616d 6528 290a 2020 2020  ster_name().    
+00034090: 7465 7374 203d 2054 6573 7428 0a20 2020  test = Test(.   
+000340a0: 2020 2020 2027 6d75 6c74 6970 6c65 2d61       'multiple-a
+000340b0: 6363 656c 6572 6174 6f72 732d 6f72 6465  ccelerators-orde
+000340c0: 7265 6427 2c0a 2020 2020 2020 2020 5b0a  red',.        [.
+000340d0: 2020 2020 2020 2020 2020 2020 6627 736b              f'sk
+000340e0: 7920 6c61 756e 6368 202d 7920 2d63 207b  y launch -y -c {
+000340f0: 6e61 6d65 7d20 7465 7374 732f 7465 7374  name} tests/test
+00034100: 5f79 616d 6c73 2f74 6573 745f 6d75 6c74  _yamls/test_mult
+00034110: 6970 6c65 5f61 6363 656c 6572 6174 6f72  iple_accelerator
+00034120: 735f 6f72 6465 7265 642e 7961 6d6c 207c  s_ordered.yaml |
+00034130: 2067 7265 7020 2255 7369 6e67 2075 7365   grep "Using use
+00034140: 722d 7370 6563 6966 6965 6420 6163 6365  r-specified acce
+00034150: 6c65 7261 746f 7273 206c 6973 7422 272c  lerators list"',
+00034160: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00034170: 6b79 206c 6f67 7320 7b6e 616d 657d 2031  ky logs {name} 1
+00034180: 202d 2d73 7461 7475 7327 2c20 2023 2045   --status',  # E
+00034190: 6e73 7572 6520 7468 6520 6a6f 6220 7375  nsure the job su
+000341a0: 6363 6565 6465 642e 0a20 2020 2020 2020  cceeded..       
+000341b0: 205d 2c0a 2020 2020 2020 2020 6627 736b   ],.        f'sk
+000341c0: 7920 646f 776e 202d 7920 7b6e 616d 657d  y down -y {name}
+000341d0: 272c 0a20 2020 2020 2020 2074 696d 656f  ',.        timeo
+000341e0: 7574 3d32 3020 2a20 3630 2c0a 2020 2020  ut=20 * 60,.    
+000341f0: 290a 2020 2020 7275 6e5f 6f6e 655f 7465  ).    run_one_te
+00034200: 7374 2874 6573 7429 0a0a 0a40 7079 7465  st(test)...@pyte
+00034210: 7374 2e6d 6172 6b2e 6e6f 5f66 6c75 6964  st.mark.no_fluid
+00034220: 7374 6163 6b20 2023 2046 6c75 6964 7374  stack  # Fluidst
+00034230: 6163 6b20 6861 7320 6c6f 7720 6176 6169  ack has low avai
+00034240: 6c61 6269 6c69 7479 2066 6f72 2054 3420  lability for T4 
+00034250: 4750 5573 0a40 7079 7465 7374 2e6d 6172  GPUs.@pytest.mar
+00034260: 6b2e 6e6f 5f70 6170 6572 7370 6163 6520  k.no_paperspace 
+00034270: 2023 2050 6170 6572 7370 6163 6520 646f   # Paperspace do
+00034280: 6573 206e 6f74 2073 7570 706f 7274 2054  es not support T
+00034290: 3420 4750 5573 0a64 6566 2074 6573 745f  4 GPUs.def test_
+000342a0: 6d75 6c74 6970 6c65 5f61 6363 656c 6572  multiple_acceler
+000342b0: 6174 6f72 735f 6f72 6465 7265 645f 7769  ators_ordered_wi
+000342c0: 7468 5f64 6566 6175 6c74 2829 3a0a 2020  th_default():.  
+000342d0: 2020 6e61 6d65 203d 205f 6765 745f 636c    name = _get_cl
+000342e0: 7573 7465 725f 6e61 6d65 2829 0a20 2020  uster_name().   
+000342f0: 2074 6573 7420 3d20 5465 7374 280a 2020   test = Test(.  
+00034300: 2020 2020 2020 276d 756c 7469 706c 652d        'multiple-
+00034310: 6163 6365 6c65 7261 746f 7273 2d6f 7264  accelerators-ord
+00034320: 6572 6564 272c 0a20 2020 2020 2020 205b  ered',.        [
+00034330: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00034340: 6b79 206c 6175 6e63 6820 2d79 202d 6320  ky launch -y -c 
+00034350: 7b6e 616d 657d 2074 6573 7473 2f74 6573  {name} tests/tes
+00034360: 745f 7961 6d6c 732f 7465 7374 5f6d 756c  t_yamls/test_mul
+00034370: 7469 706c 655f 6163 6365 6c65 7261 746f  tiple_accelerato
+00034380: 7273 5f6f 7264 6572 6564 5f77 6974 685f  rs_ordered_with_
+00034390: 6465 6661 756c 742e 7961 6d6c 207c 2067  default.yaml | g
+000343a0: 7265 7020 2255 7369 6e67 2075 7365 722d  rep "Using user-
+000343b0: 7370 6563 6966 6965 6420 6163 6365 6c65  specified accele
+000343c0: 7261 746f 7273 206c 6973 7422 272c 0a20  rators list"',. 
+000343d0: 2020 2020 2020 2020 2020 2066 2773 6b79             f'sky
+000343e0: 206c 6f67 7320 7b6e 616d 657d 2031 202d   logs {name} 1 -
+000343f0: 2d73 7461 7475 7327 2c20 2023 2045 6e73  -status',  # Ens
+00034400: 7572 6520 7468 6520 6a6f 6220 7375 6363  ure the job succ
+00034410: 6565 6465 642e 0a20 2020 2020 2020 2020  eeded..         
+00034420: 2020 2066 2773 6b79 2073 7461 7475 7320     f'sky status 
+00034430: 7b6e 616d 657d 207c 2067 7265 7020 5370  {name} | grep Sp
+00034440: 6f74 272c 0a20 2020 2020 2020 205d 2c0a  ot',.        ],.
+00034450: 2020 2020 2020 2020 6627 736b 7920 646f          f'sky do
+00034460: 776e 202d 7920 7b6e 616d 657d 272c 0a20  wn -y {name}',. 
+00034470: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
+00034480: 5f74 6573 7428 7465 7374 290a 0a0a 4070  _test(test)...@p
+00034490: 7974 6573 742e 6d61 726b 2e6e 6f5f 666c  ytest.mark.no_fl
+000344a0: 7569 6473 7461 636b 2020 2320 466c 7569  uidstack  # Flui
+000344b0: 6473 7461 636b 2068 6173 206c 6f77 2061  dstack has low a
+000344c0: 7661 696c 6162 696c 6974 7920 666f 7220  vailability for 
+000344d0: 5434 2047 5055 730a 4070 7974 6573 742e  T4 GPUs.@pytest.
+000344e0: 6d61 726b 2e6e 6f5f 7061 7065 7273 7061  mark.no_paperspa
+000344f0: 6365 2020 2320 5061 7065 7273 7061 6365  ce  # Paperspace
+00034500: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
+00034510: 7420 5434 2047 5055 730a 6465 6620 7465  t T4 GPUs.def te
+00034520: 7374 5f6d 756c 7469 706c 655f 6163 6365  st_multiple_acce
+00034530: 6c65 7261 746f 7273 5f75 6e6f 7264 6572  lerators_unorder
+00034540: 6564 2829 3a0a 2020 2020 6e61 6d65 203d  ed():.    name =
+00034550: 205f 6765 745f 636c 7573 7465 725f 6e61   _get_cluster_na
+00034560: 6d65 2829 0a20 2020 2074 6573 7420 3d20  me().    test = 
+00034570: 5465 7374 280a 2020 2020 2020 2020 276d  Test(.        'm
+00034580: 756c 7469 706c 652d 6163 6365 6c65 7261  ultiple-accelera
+00034590: 746f 7273 2d75 6e6f 7264 6572 6564 272c  tors-unordered',
+000345a0: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+000345b0: 2020 2020 2020 2066 2773 6b79 206c 6175         f'sky lau
+000345c0: 6e63 6820 2d79 202d 6320 7b6e 616d 657d  nch -y -c {name}
+000345d0: 2074 6573 7473 2f74 6573 745f 7961 6d6c   tests/test_yaml
+000345e0: 732f 7465 7374 5f6d 756c 7469 706c 655f  s/test_multiple_
+000345f0: 6163 6365 6c65 7261 746f 7273 5f75 6e6f  accelerators_uno
+00034600: 7264 6572 6564 2e79 616d 6c27 2c0a 2020  rdered.yaml',.  
+00034610: 2020 2020 2020 2020 2020 6627 736b 7920            f'sky 
+00034620: 6c6f 6773 207b 6e61 6d65 7d20 3120 2d2d  logs {name} 1 --
+00034630: 7374 6174 7573 272c 2020 2320 456e 7375  status',  # Ensu
+00034640: 7265 2074 6865 206a 6f62 2073 7563 6365  re the job succe
+00034650: 6564 6564 2e0a 2020 2020 2020 2020 5d2c  eded..        ],
+00034660: 0a20 2020 2020 2020 2066 2773 6b79 2064  .        f'sky d
+00034670: 6f77 6e20 2d79 207b 6e61 6d65 7d27 2c0a  own -y {name}',.
+00034680: 2020 2020 290a 2020 2020 7275 6e5f 6f6e      ).    run_on
+00034690: 655f 7465 7374 2874 6573 7429 0a0a 0a40  e_test(test)...@
+000346a0: 7079 7465 7374 2e6d 6172 6b2e 6e6f 5f66  pytest.mark.no_f
+000346b0: 6c75 6964 7374 6163 6b20 2023 2046 6c75  luidstack  # Flu
+000346c0: 6964 7374 6163 6b20 6861 7320 6c6f 7720  idstack has low 
+000346d0: 6176 6169 6c61 6269 6c69 7479 2066 6f72  availability for
+000346e0: 2054 3420 4750 5573 0a40 7079 7465 7374   T4 GPUs.@pytest
+000346f0: 2e6d 6172 6b2e 6e6f 5f70 6170 6572 7370  .mark.no_papersp
+00034700: 6163 6520 2023 2050 6170 6572 7370 6163  ace  # Paperspac
+00034710: 6520 646f 6573 206e 6f74 2073 7570 706f  e does not suppo
+00034720: 7274 2054 3420 4750 5573 0a64 6566 2074  rt T4 GPUs.def t
+00034730: 6573 745f 6d75 6c74 6970 6c65 5f61 6363  est_multiple_acc
+00034740: 656c 6572 6174 6f72 735f 756e 6f72 6465  elerators_unorde
+00034750: 7265 645f 7769 7468 5f64 6566 6175 6c74  red_with_default
+00034760: 2829 3a0a 2020 2020 6e61 6d65 203d 205f  ():.    name = _
+00034770: 6765 745f 636c 7573 7465 725f 6e61 6d65  get_cluster_name
+00034780: 2829 0a20 2020 2074 6573 7420 3d20 5465  ().    test = Te
+00034790: 7374 280a 2020 2020 2020 2020 276d 756c  st(.        'mul
+000347a0: 7469 706c 652d 6163 6365 6c65 7261 746f  tiple-accelerato
+000347b0: 7273 2d75 6e6f 7264 6572 6564 272c 0a20  rs-unordered',. 
+000347c0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+000347d0: 2020 2020 2066 2773 6b79 206c 6175 6e63       f'sky launc
+000347e0: 6820 2d79 202d 6320 7b6e 616d 657d 2074  h -y -c {name} t
+000347f0: 6573 7473 2f74 6573 745f 7961 6d6c 732f  ests/test_yamls/
+00034800: 7465 7374 5f6d 756c 7469 706c 655f 6163  test_multiple_ac
+00034810: 6365 6c65 7261 746f 7273 5f75 6e6f 7264  celerators_unord
+00034820: 6572 6564 5f77 6974 685f 6465 6661 756c  ered_with_defaul
+00034830: 742e 7961 6d6c 272c 0a20 2020 2020 2020  t.yaml',.       
+00034840: 2020 2020 2066 2773 6b79 206c 6f67 7320       f'sky logs 
+00034850: 7b6e 616d 657d 2031 202d 2d73 7461 7475  {name} 1 --statu
+00034860: 7327 2c20 2023 2045 6e73 7572 6520 7468  s',  # Ensure th
+00034870: 6520 6a6f 6220 7375 6363 6565 6465 642e  e job succeeded.
+00034880: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+00034890: 6b79 2073 7461 7475 7320 7b6e 616d 657d  ky status {name}
+000348a0: 207c 2067 7265 7020 5370 6f74 272c 0a20   | grep Spot',. 
+000348b0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000348c0: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
+000348d0: 7b6e 616d 657d 272c 0a20 2020 2029 0a20  {name}',.    ). 
+000348e0: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+000348f0: 7465 7374 290a 0a0a 4070 7974 6573 742e  test)...@pytest.
+00034900: 6d61 726b 2e6e 6f5f 666c 7569 6473 7461  mark.no_fluidsta
+00034910: 636b 2020 2320 5265 7175 6972 6573 206f  ck  # Requires o
+00034920: 7468 6572 2063 6c6f 7564 7320 746f 2062  ther clouds to b
+00034930: 6520 656e 6162 6c65 640a 6465 6620 7465  e enabled.def te
+00034940: 7374 5f6d 756c 7469 706c 655f 7265 736f  st_multiple_reso
+00034950: 7572 6365 7328 293a 0a20 2020 206e 616d  urces():.    nam
+00034960: 6520 3d20 5f67 6574 5f63 6c75 7374 6572  e = _get_cluster
+00034970: 5f6e 616d 6528 290a 2020 2020 7465 7374  _name().    test
+00034980: 203d 2054 6573 7428 0a20 2020 2020 2020   = Test(.       
+00034990: 2027 6d75 6c74 6970 6c65 2d72 6573 6f75   'multiple-resou
+000349a0: 7263 6573 272c 0a20 2020 2020 2020 205b  rces',.        [
+000349b0: 0a20 2020 2020 2020 2020 2020 2066 2773  .            f's
+000349c0: 6b79 206c 6175 6e63 6820 2d79 202d 6320  ky launch -y -c 
+000349d0: 7b6e 616d 657d 2074 6573 7473 2f74 6573  {name} tests/tes
+000349e0: 745f 7961 6d6c 732f 7465 7374 5f6d 756c  t_yamls/test_mul
+000349f0: 7469 706c 655f 7265 736f 7572 6365 732e  tiple_resources.
+00034a00: 7961 6d6c 272c 0a20 2020 2020 2020 2020  yaml',.         
+00034a10: 2020 2066 2773 6b79 206c 6f67 7320 7b6e     f'sky logs {n
+00034a20: 616d 657d 2031 202d 2d73 7461 7475 7327  ame} 1 --status'
+00034a30: 2c20 2023 2045 6e73 7572 6520 7468 6520  ,  # Ensure the 
+00034a40: 6a6f 6220 7375 6363 6565 6465 642e 0a20  job succeeded.. 
+00034a50: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00034a60: 2020 6627 736b 7920 646f 776e 202d 7920    f'sky down -y 
+00034a70: 7b6e 616d 657d 272c 0a20 2020 2029 0a20  {name}',.    ). 
+00034a80: 2020 2072 756e 5f6f 6e65 5f74 6573 7428     run_one_test(
+00034a90: 7465 7374 290a 0a0a 2320 2d2d 2d2d 2d2d  test)...# ------
+00034aa0: 2d2d 2d2d 2053 6b79 2042 656e 6368 6d61  ---- Sky Benchma
+00034ab0: 726b 202d 2d2d 2d2d 2d2d 2d2d 2d0a 4070  rk ----------.@p
+00034ac0: 7974 6573 742e 6d61 726b 2e6e 6f5f 666c  ytest.mark.no_fl
+00034ad0: 7569 6473 7461 636b 2020 2320 5265 7175  uidstack  # Requ
+00034ae0: 6972 6573 206f 7468 6572 2063 6c6f 7564  ires other cloud
+00034af0: 7320 746f 2062 6520 656e 6162 6c65 640a  s to be enabled.
+00034b00: 4070 7974 6573 742e 6d61 726b 2e6e 6f5f  @pytest.mark.no_
+00034b10: 7061 7065 7273 7061 6365 2020 2320 5265  paperspace  # Re
+00034b20: 7175 6972 6573 206f 7468 6572 2063 6c6f  quires other clo
+00034b30: 7564 7320 746f 2062 6520 656e 6162 6c65  uds to be enable
+00034b40: 640a 4070 7974 6573 742e 6d61 726b 2e6e  d.@pytest.mark.n
+00034b50: 6f5f 6b75 6265 726e 6574 6573 0a64 6566  o_kubernetes.def
+00034b60: 2074 6573 745f 736b 795f 6265 6e63 6828   test_sky_bench(
+00034b70: 6765 6e65 7269 635f 636c 6f75 643a 2073  generic_cloud: s
+00034b80: 7472 293a 0a20 2020 206e 616d 6520 3d20  tr):.    name = 
+00034b90: 5f67 6574 5f63 6c75 7374 6572 5f6e 616d  _get_cluster_nam
+00034ba0: 6528 290a 2020 2020 7465 7374 203d 2054  e().    test = T
+00034bb0: 6573 7428 0a20 2020 2020 2020 2027 736b  est(.        'sk
+00034bc0: 792d 6265 6e63 6827 2c0a 2020 2020 2020  y-bench',.      
+00034bd0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00034be0: 6627 736b 7920 6265 6e63 6820 6c61 756e  f'sky bench laun
+00034bf0: 6368 202d 7920 2d62 207b 6e61 6d65 7d20  ch -y -b {name} 
+00034c00: 2d2d 636c 6f75 6420 7b67 656e 6572 6963  --cloud {generic
+00034c10: 5f63 6c6f 7564 7d20 2d69 3020 7465 7374  _cloud} -i0 test
+00034c20: 732f 7465 7374 5f79 616d 6c73 2f6d 696e  s/test_yamls/min
+00034c30: 696d 616c 2e79 616d 6c27 2c0a 2020 2020  imal.yaml',.    
+00034c40: 2020 2020 2020 2020 2773 6c65 6570 2031          'sleep 1
+00034c50: 3230 272c 0a20 2020 2020 2020 2020 2020  20',.           
+00034c60: 2066 2773 6b79 2062 656e 6368 2073 686f   f'sky bench sho
+00034c70: 7720 7b6e 616d 657d 207c 2067 7265 7020  w {name} | grep 
+00034c80: 736b 792d 6265 6e63 682d 7b6e 616d 657d  sky-bench-{name}
+00034c90: 207c 2067 7265 7020 4649 4e49 5348 4544   | grep FINISHED
+00034ca0: 272c 0a20 2020 2020 2020 205d 2c0a 2020  ',.        ],.  
+00034cb0: 2020 2020 2020 6627 736b 7920 6265 6e63        f'sky benc
+00034cc0: 6820 646f 776e 207b 6e61 6d65 7d20 2d79  h down {name} -y
+00034cd0: 3b20 736b 7920 6265 6e63 6820 6465 6c65  ; sky bench dele
+00034ce0: 7465 207b 6e61 6d65 7d20 2d79 272c 0a20  te {name} -y',. 
+00034cf0: 2020 2029 0a20 2020 2072 756e 5f6f 6e65     ).    run_one
+00034d00: 5f74 6573 7428 7465 7374 290a            _test(test).
```

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240514/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240515/tests/test_yaml_parser.py`

 * *Files identical despite different names*

