# Comparing `tmp/autogluon.cloud-0.3.1b20240101.tar.gz` & `tmp/autogluon.cloud-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autogluon.cloud-0.3.1b20240101.tar", last modified: Mon Jan  1 09:04:46 2024, max compression
+gzip compressed data, was "autogluon.cloud-0.4.0.tar", last modified: Thu May 16 20:51:58 2024, max compression
```

## Comparing `autogluon.cloud-0.3.1b20240101.tar` & `autogluon.cloud-0.4.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/ray_aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    22735 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    59108 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_cluster_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/data/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/data/format_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/default_cluster_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/default_cluster_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/remote_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/sagemaker_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13008 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/ray_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/ray_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/ray_scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/script_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ag_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/aws_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/dlc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ray_aws_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/sagemaker_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-01-01 09:04:32.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-01-01 09:04:46.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 09:04:45.000000 autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.702626 autogluon.cloud-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 20:51:58.702626 autogluon.cloud-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-16 20:51:58.706626 autogluon.cloud-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.690626 autogluon.cloud-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.694626 autogluon.cloud-0.4.0/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.694626 autogluon.cloud-0.4.0/src/autogluon/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.694626 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/ray_aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22735 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59108 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_cluster_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/data/format_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/default_cluster_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/default_cluster_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/job/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/job/remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/job/sagemaker_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.698626 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.702626 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/ray_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/ray_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/ray_scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.702626 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/script_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.702626 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ag_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/aws_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/dlc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ray_aws_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/sagemaker_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-16 20:51:49.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon/cloud/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:51:58.694626 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:51:58.000000 autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autogluon.cloud-0.3.1b20240101/LICENSE` & `autogluon.cloud-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/PKG-INFO` & `autogluon.cloud-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.3.1b20240101
+Version: 0.4.0
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
@@ -15,14 +15,16 @@
           <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         </div>
         
         # AutoGluon-Cloud
         
         [![Continuous Integration](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml)
         
+        [AutoGluon-Cloud Documentation](https://auto.gluon.ai/cloud/stable/index.html) | [AutoGluon Documentation](https://auto.gluon.ai)
+        
         AutoGluon-Cloud aims to provide user tools to train, fine-tune and deploy [AutoGluon](https://auto.gluon.ai/stable/index.html) backed models on the cloud. With just a few lines of codes, users could train a model and perform inference on the cloud without worrying about MLOps details such as resource management.
         
         Currently, AutoGluon-Cloud supports [AWS SageMaker](https://aws.amazon.com/sagemaker/) as the cloud backend.
         
         ## Installation
         ```bash
         pip install -U pip
```

### Comparing `autogluon.cloud-0.3.1b20240101/README.md` & `autogluon.cloud-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
 </div>
 
 # AutoGluon-Cloud
 
 [![Continuous Integration](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml)
 
+[AutoGluon-Cloud Documentation](https://auto.gluon.ai/cloud/stable/index.html) | [AutoGluon Documentation](https://auto.gluon.ai)
+
 AutoGluon-Cloud aims to provide user tools to train, fine-tune and deploy [AutoGluon](https://auto.gluon.ai/stable/index.html) backed models on the cloud. With just a few lines of codes, users could train a model and perform inference on the cloud without worrying about MLOps details such as resource management.
 
 Currently, AutoGluon-Cloud supports [AWS SageMaker](https://aws.amazon.com/sagemaker/) as the cloud backend.
 
 ## Installation
 ```bash
 pip install -U pip
```

### Comparing `autogluon.cloud-0.3.1b20240101/setup.cfg` & `autogluon.cloud-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/setup.py` & `autogluon.cloud-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,45 +100,43 @@
             "Source": "https://github.com/autogluon/autogluon-cloud/",
             "Contribute!": "https://github.com/autogluon/autogluon-cloud/blob/master/CONTRIBUTING.md",
         },
     )
     return setup_args
 
 
-version = "0.3.1"
+version = "0.4.0"
 version = update_version(version, use_file_if_exists=False, create_file=True)
 
 install_requires = [
     # common module provides utils with stable api across minor version
-    "autogluon.common>=0.7,<1.1",
+    "autogluon.common>=0.7",
     # <2 because unlikely to introduce breaking changes in minor releases. >=1.10 because 1.10 is 3 years old, no need to support older
     "boto3>=1.10,<2.0",
-    "numpy>=1.21,<1.27",
     "packaging>=23.0,<24.0",
-    "pandas>=2.0.0,<2.2.0",
     # updated sagemaker is required to fetch latest container info, so we don't want to cap the version too strict
     # otherwise cloud module needs to be released to support new container
     "sagemaker>=2.126.0,<3.0",
     "pyarrow>=11.0,<11.1",
     "PyYAML~=6.0",
-    "Pillow>=9.3.0,<10.0",  # unlikely to introduce breaking changes in minor releases
-    "ray[default]>=2.6.3,<2.7",
+    "Pillow>=10.2,<11",  # unlikely to introduce breaking changes in minor releases
+    "ray[default]>=2.10.0,<2.11",
 ]
 
 extras_require = dict()
 
-all_requires = ["autogluon>=0.7,<1.0"]  # To allow user to pass ag objects
+all_requires = ["autogluon>=0.7"]  # To allow user to pass ag objects
 extras_require["all"] = all_requires
 
 test_requirements = [
     "tox",
     "pytest",
     "pytest-cov",
     "moto",
-    "autogluon.common>=0.7.0b,<1.1",
+    "autogluon.common>=0.7",
 ]  # Install pre-release of common for testing
 
 test_requirements = list(set(test_requirements))
 extras_require["tests"] = test_requirements
 
 if __name__ == "__main__":
     create_version_file(version=version)
```

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/backend_factory.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/backend_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/ray_aws_backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/ray_aws_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/ray_backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/ray_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/sagemaker_backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/cluster_config_generator.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/cluster_manager.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/constants.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/cluster/ray_cluster_manager.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/cluster/ray_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/data/format_converter.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/data/format_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/endpoint.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/endpoint/sagemaker_endpoint.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/endpoint/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/ray_job.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/job/ray_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/remote_job.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/job/remote_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/job/sagemaker_job.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/job/sagemaker_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/cloud_predictor.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/tabular_cloud_predictor.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/tabular_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,31 @@
 logger = logging.getLogger(__name__)
 
 
 class TimeSeriesCloudPredictor(CloudPredictor):
     predictor_file_name = "TimeSeriesCloudPredictor.pkl"
     backend_map = {SAGEMAKER: TIMESERIES_SAGEMAKER}
 
+    def __init__(
+        self,
+        local_output_path: Optional[str] = None,
+        cloud_output_path: Optional[str] = None,
+        backend: str = SAGEMAKER,
+        verbosity: int = 2,
+    ) -> None:
+        super().__init__(
+            local_output_path=local_output_path,
+            cloud_output_path=cloud_output_path,
+            backend=backend,
+            verbosity=verbosity,
+        )
+        self.target_column: Optional[str] = None
+        self.id_column: Optional[str] = None
+        self.timestamp_column: Optional[str] = None
+
     @property
     def predictor_type(self):
         """
         Type of the underneath AutoGluon Predictor
         """
         return "timeseries"
 
@@ -29,16 +46,16 @@
         return predictor_cls
 
     def fit(
         self,
         *,
         predictor_init_args: Dict[str, Any],
         predictor_fit_args: Dict[str, Any],
-        id_column: str,
-        timestamp_column: str,
+        id_column: str = "item_id",
+        timestamp_column: str = "timestamp",
         static_features: Optional[Union[str, pd.DataFrame]] = None,
         framework_version: str = "latest",
         job_name: Optional[str] = None,
         instance_type: str = "ml.m5.2xlarge",
         instance_count: int = 1,
         volume_size: int = 100,
         custom_image_uri: Optional[str] = None,
@@ -52,18 +69,18 @@
 
         Parameters
         ----------
         predictor_init_args: dict
             Init args for the predictor
         predictor_fit_args: dict
             Fit args for the predictor
-        id_column: str
-            Name of the 'item_id' column
-        timestamp_column: str
-            Name of the 'timestamp' column
+        id_column: str, default = "item_id"
+            Name of the item ID column
+        timestamp_column: str, default = "timestamp"
+            Name of the timestamp column
         static_features: Optional[pd.DataFrame]
              An optional data frame describing the metadata attributes of individual items in the item index.
              For more detail, please refer to `TimeSeriesDataFrame` documentation:
              https://auto.gluon.ai/stable/api/autogluon.predictor.html#timeseriesdataframe
         framework_version: str, default = `latest`
             Training container version of autogluon.
             If `latest`, will use the latest available container version.
@@ -98,14 +115,19 @@
         `TimeSeriesCloudPredictor` object. Returns self.
         """
         assert (
             not self.backend.is_fit
         ), "Predictor is already fit! To fit additional models, create a new `CloudPredictor`"
         if backend_kwargs is None:
             backend_kwargs = {}
+
+        self.target_column = predictor_init_args.get("target", "target")
+        self.id_column = id_column
+        self.timestamp_column = timestamp_column
+
         backend_kwargs = self.backend.parse_backend_fit_kwargs(backend_kwargs)
         self.backend.fit(
             predictor_init_args=predictor_init_args,
             predictor_fit_args=predictor_fit_args,
             id_column=id_column,
             timestamp_column=timestamp_column,
             static_features=static_features,
@@ -120,70 +142,58 @@
         )
 
         return self
 
     def predict_real_time(
         self,
         test_data: Union[str, pd.DataFrame],
-        id_column: str,
-        timestamp_column: str,
-        target: str,
         static_features: Optional[Union[str, pd.DataFrame]] = None,
         accept: str = "application/x-parquet",
         **kwargs,
     ) -> pd.DataFrame:
         """
         Predict with the deployed SageMaker endpoint. A deployed SageMaker endpoint is required.
         This is intended to provide a low latency inference.
         If you want to inference on a large dataset, use `predict()` instead.
 
         Parameters
         ----------
         test_data: Union(str, pandas.DataFrame)
             The test data to be inferenced.
             Can be a pandas.DataFrame or a local path to a csv file.
-        id_column: str
-            Name of the 'item_id' column
-        timestamp_column: str
-            Name of the 'timestamp' column
         static_features: Optional[pd.DataFrame]
              An optional data frame describing the metadata attributes of individual items in the item index.
              For more detail, please refer to `TimeSeriesDataFrame` documentation:
              https://auto.gluon.ai/stable/api/autogluon.predictor.html#timeseriesdataframe
-        target: str
-            Name of column that contains the target values to forecast
         accept: str, default = application/x-parquet
             Type of accept output content.
             Valid options are application/x-parquet, text/csv, application/json
         kwargs:
             Additional args that you would pass to `predict` calls of an AutoGluon logic
 
         Returns
         -------
         Pandas.DataFrame
         Predict results in DataFrame
         """
         return self.backend.predict_real_time(
             test_data=test_data,
-            id_column=id_column,
-            timestamp_column=timestamp_column,
-            target=target,
+            id_column=self.id_column,
+            timestamp_column=self.timestamp_column,
+            target=self.target_column,
             static_features=static_features,
             accept=accept,
         )
 
     def predict_proba_real_time(self, **kwargs) -> pd.DataFrame:
         raise ValueError(f"{self.__class__.__name__} does not support predict_proba operation.")
 
     def predict(
         self,
         test_data: Union[str, pd.DataFrame],
-        id_column: str,
-        timestamp_column: str,
-        target: str,
         static_features: Optional[Union[str, pd.DataFrame]] = None,
         predictor_path: Optional[str] = None,
         framework_version: str = "latest",
         job_name: Optional[str] = None,
         instance_type: str = "ml.m5.2xlarge",
         instance_count: int = 1,
         custom_image_uri: Optional[str] = None,
@@ -199,18 +209,14 @@
         then create a transformer with it, and call transform in the end.
 
         Parameters
         ----------
         test_data: str
             The test data to be inferenced.
             Can be a pandas.DataFrame or a local path to a csv file.
-        id_column: str
-            Name of the 'item_id' column
-        timestamp_column: str
-            Name of the 'timestamp' column
         static_features: Optional[Union[str, pd.DataFrame]]
              An optional data frame describing the metadata attributes of individual items in the item index.
              For more detail, please refer to `TimeSeriesDataFrame` documentation:
              https://auto.gluon.ai/stable/api/autogluon.predictor.html#timeseriesdataframe
         target: str
             Name of column that contains the target values to forecast
         predictor_path: str
@@ -258,17 +264,17 @@
                     https://sagemaker.readthedocs.io/en/stable/api/inference/transformer.html#sagemaker.transformer.Transformer.transform for all options.
         """
         if backend_kwargs is None:
             backend_kwargs = {}
         backend_kwargs = self.backend.parse_backend_predict_kwargs(backend_kwargs)
         return self.backend.predict(
             test_data=test_data,
-            id_column=id_column,
-            timestamp_column=timestamp_column,
-            target=target,
+            id_column=self.id_column,
+            timestamp_column=self.timestamp_column,
+            target=self.target_column,
             static_features=static_features,
             predictor_path=predictor_path,
             framework_version=framework_version,
             job_name=job_name,
             instance_type=instance_type,
             instance_count=instance_count,
             custom_image_uri=custom_image_uri,
```

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/ray_scripts/train.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/ray_scripts/train.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/sagemaker_scripts/train.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/sagemaker_scripts/train.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/scripts/script_manager.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/scripts/script_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ag_sagemaker.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ag_sagemaker.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/aws_utils.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/deserializers.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/deserializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/dlc_utils.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/dlc_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ec2.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ec2.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/iam.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/ray_aws_iam.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/ray_aws_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/s3_utils.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/sagemaker_iam.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/sagemaker_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/serializers.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon/cloud/utils/utils.py` & `autogluon.cloud-0.4.0/src/autogluon/cloud/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/PKG-INFO` & `autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.3.1b20240101
+Version: 0.4.0
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
@@ -15,14 +15,16 @@
           <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         </div>
         
         # AutoGluon-Cloud
         
         [![Continuous Integration](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/autogluon/autogluon-cloud/actions/workflows/continuous_integration.yml)
         
+        [AutoGluon-Cloud Documentation](https://auto.gluon.ai/cloud/stable/index.html) | [AutoGluon Documentation](https://auto.gluon.ai)
+        
         AutoGluon-Cloud aims to provide user tools to train, fine-tune and deploy [AutoGluon](https://auto.gluon.ai/stable/index.html) backed models on the cloud. With just a few lines of codes, users could train a model and perform inference on the cloud without worrying about MLOps details such as resource management.
         
         Currently, AutoGluon-Cloud supports [AWS SageMaker](https://aws.amazon.com/sagemaker/) as the cloud backend.
         
         ## Installation
         ```bash
         pip install -U pip
```

### Comparing `autogluon.cloud-0.3.1b20240101/src/autogluon.cloud.egg-info/SOURCES.txt` & `autogluon.cloud-0.4.0/src/autogluon.cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

