# Comparing `tmp/outsystems-pipeline-0.8.0.tar.gz` & `tmp/outsystems-pipeline-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outsystems-pipeline-0.8.0.tar", last modified: Wed Nov 15 12:55:34 2023, max compression
+gzip compressed data, was "outsystems-pipeline-0.9.0.tar", last modified: Thu May 16 11:44:00 2024, max compression
```

## Comparing `outsystems-pipeline-0.8.0.tar` & `outsystems-pipeline-0.9.0.tar`

### file list

```diff
@@ -1,90 +1,98 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/
--rw-r--r--   0 vsts      (1001) docker     (127)    11358 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      574 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/NOTICE.md
--rw-r--r--   0 vsts      (1001) docker     (127)     2951 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2111 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.743539 outsystems-pipeline-0.8.0/outsystems/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.747539 outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1166 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/ad_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5992 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/ad_tech_debt.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.747539 outsystems-pipeline-0.8.0/outsystems/bdd_framework/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/bdd_framework/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1965 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/bdd_framework/bdd_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)      586 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/bdd_framework/bdd_runner.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.747539 outsystems-pipeline-0.8.0/outsystems/cicd_probe/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/cicd_probe/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1555 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_dependencies.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1546 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_scan.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.751539 outsystems-pipeline-0.8.0/outsystems/exceptions/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/app_does_not_exist.py
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/app_version_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/deployment_not_found.py
--rw-r--r--   0 vsts      (1001) docker     (127)       52 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/environment_not_found.py
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/impossible_action_deployment.py
--rw-r--r--   0 vsts      (1001) docker     (127)       52 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/invalid_json_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/invalid_parameters.py
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/manifest_does_not_exist.py
--rw-r--r--   0 vsts      (1001) docker     (127)       48 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/no_apps_available.py
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/no_deployments.py
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/not_enough_permissions.py
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/osptool_error.py
--rw-r--r--   0 vsts      (1001) docker     (127)       39 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/exceptions/server_error.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.751539 outsystems-pipeline-0.8.0/outsystems/file_helpers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/file_helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/file_helpers/file.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.751539 outsystems-pipeline-0.8.0/outsystems/lifetime/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/lifetime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17341 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_applications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3485 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17096 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_deployments.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11819 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_environments.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.751539 outsystems-pipeline-0.8.0/outsystems/manifest/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/manifest/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2632 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/manifest/manifest_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.751539 outsystems-pipeline-0.8.0/outsystems/osp_tool/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/osp_tool/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/osp_tool/osp_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.755539 outsystems-pipeline-0.8.0/outsystems/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7213 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/apply_configuration_values_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7192 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/continue_deployment_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13734 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18841 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22180 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3372 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/evaluate_test_results.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10653 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_apps_packages.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3546 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_lifetime_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3903 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_tech_debt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7611 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/generate_unit_testing_assembly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11847 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/scan_test_endpoints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10292 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/start_deployment_to_target_env.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7601 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8911 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/pipeline/tag_modified_apps.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.755539 outsystems-pipeline-0.8.0/outsystems/properties/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/properties/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1825 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/properties/properties_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3042 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/properties/properties_set_value.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/outsystems/vars/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      752 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/ad_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      372 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/bdd_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/cicd_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1786 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/file_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3520 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/lifetime_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1055 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/manifest_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      656 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/pipeline_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/properties_vars.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1340 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/outsystems/vars/vars_base.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2951 2023-11-15 12:55:34.000000 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2878 2023-11-15 12:55:34.000000 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-15 12:55:34.000000 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      125 2023-11-15 12:55:34.000000 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2023-11-15 12:55:34.000000 outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     4163 2023-11-15 12:55:33.000000 outsystems-pipeline-0.8.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-15 12:55:34.759539 outsystems-pipeline-0.8.0/test/
--rw-r--r--   0 vsts      (1001) docker     (127)       47 2023-11-15 12:55:30.000000 outsystems-pipeline-0.8.0/test/test_deploy_latest_tags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11358 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      574 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/NOTICE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2111 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.154750 outsystems-pipeline-0.9.0/outsystems/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.154750 outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1166 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/ad_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5992 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/ad_tech_debt.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.154750 outsystems-pipeline-0.9.0/outsystems/bdd_framework/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/bdd_framework/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/bdd_framework/bdd_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      586 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/bdd_framework/bdd_runner.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.154750 outsystems-pipeline-0.9.0/outsystems/cicd_probe/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/cicd_probe/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1555 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_dependencies.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1546 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_scan.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.158750 outsystems-pipeline-0.9.0/outsystems/exceptions/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/app_does_not_exist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/app_version_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/deployment_not_found.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/environment_not_found.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/impossible_action_deployment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/invalid_json_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/invalid_os_package.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/invalid_parameters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/manifest_does_not_exist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       48 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/no_apps_available.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/no_deployments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/not_enough_permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/osptool_error.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       39 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/exceptions/server_error.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.158750 outsystems-pipeline-0.9.0/outsystems/file_helpers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/file_helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1560 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/file_helpers/file.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.158750 outsystems-pipeline-0.9.0/outsystems/lifetime/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17458 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_applications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5304 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18583 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_deployments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2238 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_downloads.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17035 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_environments.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4944 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_solutions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.158750 outsystems-pipeline-0.9.0/outsystems/manifest/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/manifest/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2632 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/manifest/manifest_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.158750 outsystems-pipeline-0.9.0/outsystems/osp_tool/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/osp_tool/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2384 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/osp_tool/osp_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.162750 outsystems-pipeline-0.9.0/outsystems/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7213 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/apply_configuration_values_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7192 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/continue_deployment_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13734 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18841 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10968 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_package_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4601 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_package_to_target_env_with_osptool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22180 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3372 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/evaluate_test_results.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10653 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_apps_packages.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17307 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_apps_source_code.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3546 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_lifetime_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11205 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_lifetime_solution_from_manifest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3903 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_tech_debt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7611 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/generate_unit_testing_assembly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11847 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/scan_test_endpoints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10292 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/start_deployment_to_target_env.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7601 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8911 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/pipeline/tag_modified_apps.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.162750 outsystems-pipeline-0.9.0/outsystems/properties/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/properties/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/properties/properties_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3042 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/properties/properties_set_value.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/outsystems/vars/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      752 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/ad_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      372 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/bdd_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/cicd_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/dotnet_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2187 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/file_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4725 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/lifetime_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/manifest_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1324 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/pipeline_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/properties_vars.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1340 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/outsystems/vars/vars_base.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2989 2024-05-16 11:44:00.000000 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3261 2024-05-16 11:44:00.000000 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-16 11:44:00.000000 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      131 2024-05-16 11:44:00.000000 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-16 11:44:00.000000 outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     4207 2024-05-16 11:43:57.000000 outsystems-pipeline-0.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 11:44:00.166750 outsystems-pipeline-0.9.0/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)       47 2024-05-16 11:43:52.000000 outsystems-pipeline-0.9.0/test/test_deploy_latest_tags.py
```

### Comparing `outsystems-pipeline-0.8.0/LICENSE` & `outsystems-pipeline-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/NOTICE.md` & `outsystems-pipeline-0.9.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/PKG-INFO` & `outsystems-pipeline-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outsystems-pipeline
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package to accelerate the integration of OutSystems with third-party CI/CD tools
 Home-page: https://github.com/OutSystems/outsystems-pipeline
 Author: OutSystems
 Author-email: cicd.integrations@outsystems.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,40 +26,42 @@
 
 Visit the `project repository <https://github.com/OutSystems/outsystems-pipeline>`_ on GitHub for instructions on how to build example OutSystems CI/CD pipelines with common DevOps automation tools, as well as documentation that will help you adapt the examples to your particular scenarios.
 
 
 What's new
 ==========
 
-**Config File Support**
- Load configuration values from a custom file to override default values. To use this feature, use the new `--config_file` parameter to specify the configuration file path.
- This enhancement is available in the following scripts:
-
- * `apply_configuration_values_to_target_env.py`
- * `continue_deployment_to_target_env.py`
- * `deploy_apps_to_target_env_with_airgap.py`
- * `deploy_latest_tags_to_target_env.py`
- * `deploy_tags_to_target_env_with_manifest.py`
- * `evaluate_test_results.py`
- * `fetch_apps_packages.py`
- * `fetch_lifetime_data.py`
- * `scan_test_endpoints.py`
- * `start_deployment_to_target_env.py`
- * `tag_apps_based_on_manifest_data.py`
- * `tag_modified_apps.py`
-
-**SSL Certificate Verification**
- The Python `requests` module verifies SSL certificates for HTTPS requests.
- Now there's a flag to enable (default value) or disable SSL certificate verification.
+**Download Application Source Code**
 
-**Fetch Technical Debt**
- Enhanced the `fetch_tech_debt` script to prevent failures when all modules of an app are marked as 'ignored' in AI Mentor Studio and when an app has no security findings.
+ A new script was added to download platform-generated source code:
 
-**Tag Modified Applications**
- Updated `tag_modified_apps` script to tag applications based on a app_list parameter or from the trigger_manifest artifact
+ * `fetch_apps_source_code.py`
+
+ Use the following parameters to generate more human-readable outputs and facilitate the compilation of the source code:
+
+ * --friendly_package_names: source code packages with user-friendly names.
+ * --include_all_refs: adds to .csproj file all assemblies in the bin folder as references.
+ * --remove_resources_files: removes references to embedded resources files from the.csproj file.
+
+**Solution Download and Deploy**
+
+ Added new functions to leverage the recently released/improved APIs to download and deploy outsystems packages:
+
+ * `fetch_lifetime_solution_from_manifest.py` - downloads a solution file based on manifest data.
+ * `deploy_package_to_target_env.py` - deploys an outsystems package (solution or application) to a target environment.
+ * `deploy_package_to_target_env_with_osptool.py` - deploys an outsystems package (solution or application) using OSP Tool.
+
+**Improved OSPTool Operations**
+
+ OSPTool command line calls now have live output callback and catalog mapping support.
+
+**Updated Package Dependencies**
+
+ * Updated python-dateutil dependency to version 2.9.0.post0
+ * Updated python-dotenv dependency to version 1.0.1
 
 Installing and upgrading
 ========================
 
 Install or upgrade outsystems-pipeline to the latest available version as follows:
 ::
```

### Comparing `outsystems-pipeline-0.8.0/README.md` & `outsystems-pipeline-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/ad_base.py` & `outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/ad_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/architecture_dashboard/ad_tech_debt.py` & `outsystems-pipeline-0.9.0/outsystems/architecture_dashboard/ad_tech_debt.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/bdd_framework/bdd_base.py` & `outsystems-pipeline-0.9.0/outsystems/bdd_framework/bdd_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/bdd_framework/bdd_runner.py` & `outsystems-pipeline-0.9.0/outsystems/bdd_framework/bdd_runner.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_base.py` & `outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_dependencies.py` & `outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_dependencies.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/cicd_probe/cicd_scan.py` & `outsystems-pipeline-0.9.0/outsystems/cicd_probe/cicd_scan.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/file_helpers/file.py` & `outsystems-pipeline-0.9.0/outsystems/file_helpers/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,10 @@
 # Python Modules
 import json
 import os
-import requests
-
-
-def download_oap(file_path: str, auth_token: str, oap_url: str):
-    response = requests.get(oap_url, headers={"Authorization": auth_token})
-    # Makes sure that, if a directory is in the filename, that directory exists
-    os.makedirs(os.path.dirname(file_path), exist_ok=True)
-    with open(file_path, "wb") as f:
-        f.write(response.content)
 
 
 def store_data(artifact_dir: str, filename: str, data: str):
     filename = os.path.join(artifact_dir, filename)
     # Remove the spaces in the filename
     filename = filename.replace(" ", "_")
     # Makes sure that, if a directory is in the filename, that directory exists
@@ -39,7 +30,16 @@
 
 
 def clear_cache(artifact_dir: str, filename: str):
     if not check_file(artifact_dir, filename):
         return
     filename = os.path.join(artifact_dir, filename)
     os.remove(filename)
+
+
+# Returns a human readable string representation of bytes
+def bytes_human_readable_size(bytes, units=[' bytes', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB']):
+    return str(bytes) + units[0] if bytes < 1024 else bytes_human_readable_size(bytes >> 10, units[1:])
+
+
+def is_valid_os_package(filename: str):
+    return filename.lower().split('.')[-1] in ("osp", "oap")
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_applications.py` & `outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from outsystems.exceptions.invalid_parameters import InvalidParametersError
 from outsystems.exceptions.no_apps_available import NoAppsAvailableError
 from outsystems.exceptions.server_error import ServerError
 from outsystems.exceptions.not_enough_permissions import NotEnoughPermissionsError
 from outsystems.exceptions.environment_not_found import EnvironmentNotFoundError
 from outsystems.exceptions.app_version_error import AppVersionsError
 # Functions
-from outsystems.file_helpers.file import store_data, load_data, clear_cache, download_oap
+from outsystems.file_helpers.file import store_data, load_data, clear_cache
 from outsystems.lifetime.lifetime_base import send_get_request, send_post_request
+from outsystems.lifetime.lifetime_downloads import download_package
 # Variables
 from outsystems.vars.file_vars import APPLICATION_FOLDER, APPLICATIONS_FILE, APPLICATION_FILE, APPLICATION_VERSIONS_FILE, APPLICATION_VERSION_FILE
 from outsystems.vars.lifetime_vars import APPLICATIONS_ENDPOINT, APPLICATION_VERSIONS_ENDPOINT, APPLICATIONS_SUCCESS_CODE, \
     APPLICATIONS_EMPTY_CODE, APPLICATIONS_FLAG_FAILED_CODE, APPLICATIONS_FAILED_CODE, APPLICATION_SUCCESS_CODE, \
     APPLICATION_FLAG_FAILED_CODE, APPLICATION_NO_PERMISSION_CODE, APPLICATION_FAILED_CODE, APPLICATION_VERSION_SUCCESS_CODE, \
     APPLICATION_VERSION_INVALID_CODE, APPLICATION_VERSION_NO_PERMISSION_CODE, APPLICATION_VERSION_FAILED_CODE, \
     APPLICATION_VERSION_FAILED_LIST_CODE, APPLICATION_VERSIONS_CONTENT, APPLICATION_VERSIONS_EMPTY_CODE, \
@@ -154,15 +155,16 @@
     for status_in_env in deployed_app["AppStatusInEnvs"]:
         if status_in_env["EnvironmentKey"] == env_key:
             app_version_data = get_application_version(artifact_dir, endpoint, auth_token, True, status_in_env["BaseApplicationVersionKey"], app_name=app_tuple[0])
             app_data = {
                 "ApplicationName": app_tuple[0],
                 "ApplicationKey": app_tuple[1],
                 "Version": app_version_data["Version"],
-                "VersionKey": status_in_env["BaseApplicationVersionKey"]
+                "VersionKey": status_in_env["BaseApplicationVersionKey"],
+                "IsModified": status_in_env["IsModified"]
             }
             # Since these 2 fields were only introduced in a minor of OS11, we check here if they exist
             # We can't just use the version
             if "CreatedOn" in app_version_data:
                 app_data.update({"CreatedOn": app_version_data["CreatedOn"]})
             if "ChangeLog" in app_version_data:
                 app_data.update({"ChangeLog": app_version_data["ChangeLog"]})
@@ -208,15 +210,15 @@
     response = send_get_request(endpoint, auth_token, query, None)
 
     status_code = int(response["http_status"])
     if status_code == APPLICATIONS_SUCCESS_CODE:
         # Stores the result
         url_string = response["response"]
         url_string = url_string["url"]
-        download_oap(file_path, auth_token, url_string)
+        download_package(file_path, auth_token, url_string)
         return
     elif status_code == APPLICATION_VERSION_NO_PERMISSION_CODE:
         raise NotEnoughPermissionsError(
             "You don't have enough permissions to see the details of that application. Details: {}".format(response["response"]))
     elif status_code == APPLICATION_VERSION_INVALID_CODE:
         raise AppVersionsError(
             "The request is invalid for the given keys. Details: {}".format(response["response"]))
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_base.py` & `outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Custom Modules
 # Exceptions
 from outsystems.exceptions.invalid_json_response import InvalidJsonResponseError
 # Variables
 from outsystems.vars.lifetime_vars import LIFETIME_SSL_CERT_VERIFY
 # Functions
 from outsystems.vars.vars_base import get_configuration_value
+from outsystems.file_helpers.file import check_file
 
 
 # Method that builds the LifeTime endpoint based on the LT host
 def build_lt_endpoint(lt_http_proto: str, lt_url: str, lt_api_endpoint: str, lt_api_version: int):
     # Builds the endpoint for LT and returns it
     return "{}://{}/{}/v{}".format(lt_http_proto, lt_url, lt_api_endpoint, lt_api_version)
 
@@ -51,14 +52,37 @@
             response_obj["response"] = response.json()
         except:
             # Workaround for POST /deployments/ since the response is not JSON, just text
             response_obj["response"] = json.loads('"{}"'.format(response.text))
     return response_obj
 
 
+# Sends a POST request to LT, with binary content.
+def send_binary_post_request(lt_api: str, token: str, api_endpoint: str, dest_env: str, lt_endpont: str, binary_file_path: str):
+    # Auth token + content type octet-stream
+    headers = {'content-type': 'application/octet-stream',
+               'authorization': 'Bearer ' + token}
+    # Format the request URL to include the api endpoint
+    request_string = "{}/{}/{}/{}".format(lt_api, api_endpoint, dest_env, lt_endpont)
+
+    if check_file("", binary_file_path):
+        with open(binary_file_path, 'rb') as f:
+            data = f.read()
+    response = requests.post(request_string, data=data, headers=headers, verify=get_configuration_value("LIFETIME_SSL_CERT_VERIFY", LIFETIME_SSL_CERT_VERIFY))
+    response_obj = {"http_status": response.status_code, "response": {}}
+    # Since LT API POST requests do not reply with native JSON, we have to make it ourselves
+    if len(response.text) > 0:
+        try:
+            response_obj["response"] = response.json()
+        except:
+            # Workaround for POST /deployments/ since the response is not JSON, just text
+            response_obj["response"] = json.loads('"{}"'.format(response.text))
+    return response_obj
+
+
 # Sends a DELETE request to LT
 def send_delete_request(lt_api: str, token: str, api_endpoint: str):
     # Auth token + content type json
     headers = {'content-type': 'application/json',
                'authorization': 'Bearer ' + token}
     # Format the request URL to include the api endpoint
     request_string = "{}/{}".format(lt_api, api_endpoint)
@@ -67,7 +91,18 @@
     if len(response.text) > 0:
         try:
             response_obj["response"] = response.json()
         except:
             raise InvalidJsonResponseError(
                 "DELETE {}: The JSON response could not be parsed. Response: {}".format(request_string, response.text))
     return response_obj
+
+
+# Sends a GET request to LT, with url_params
+def send_download_request(pkg_url: str, token: str):
+    # Auth token + content type json
+    headers = {'content-type': 'application/json',
+               'authorization': token}
+    # Format the request URL to include the api endpoint
+    response = requests.get(pkg_url, headers=headers, verify=get_configuration_value("LIFETIME_SSL_CERT_VERIFY", LIFETIME_SSL_CERT_VERIFY))
+    response_obj = {"http_status": response.status_code, "response": response.content}
+    return response_obj
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_deployments.py` & `outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_deployments.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from outsystems.exceptions.no_deployments import NoDeploymentsError
 from outsystems.exceptions.invalid_parameters import InvalidParametersError
 from outsystems.exceptions.not_enough_permissions import NotEnoughPermissionsError
 from outsystems.exceptions.server_error import ServerError
 from outsystems.exceptions.environment_not_found import EnvironmentNotFoundError
 from outsystems.exceptions.impossible_action_deployment import ImpossibleApplyActionDeploymentError
 # Functions
-from outsystems.lifetime.lifetime_base import send_get_request, send_post_request, send_delete_request
+from outsystems.lifetime.lifetime_base import send_get_request, send_post_request, send_delete_request, send_binary_post_request
 from outsystems.lifetime.lifetime_environments import get_environment_key
 from outsystems.file_helpers.file import store_data
 # Variables
 from outsystems.vars.lifetime_vars import DEPLOYMENTS_ENDPOINT, DEPLOYMENT_STATUS_ENDPOINT, \
     DEPLOYMENT_START_ENDPOINT, DEPLOYMENT_CONTINUE_ENDPOINT, DEPLOYMENTS_SUCCESS_CODE, DEPLOYMENTS_EMPTY_CODE, \
     DEPLOYMENTS_INVALID_CODE, DEPLOYMENTS_NO_PERMISSION_CODE, DEPLOYMENTS_FAILED_CODE, DEPLOYMENT_GET_SUCCESS_CODE, \
     DEPLOYMENT_GET_NO_PERMISSION_CODE, DEPLOYMENT_GET_NO_DEPLOYMENT_CODE, DEPLOYMENT_GET_FAILED_CODE, \
     DEPLOYMENT_STATUS_SUCCESS_CODE, DEPLOYMENT_STATUS_NO_PERMISSION_CODE, DEPLOYMENT_STATUS_NO_DEPLOYMENT_CODE, DEPLOYMENT_STATUS_FAILED_CODE, \
     DEPLOYMENT_SUCCESS_CODE, DEPLOYMENT_INVALID_CODE, DEPLOYMENT_NO_PERMISSION_CODE, DEPLOYMENT_NO_ENVIRONMENT_CODE, DEPLOYMENT_FAILED_CODE, \
     DEPLOYMENT_DELETE_SUCCESS_CODE, DEPLOYMENT_DELETE_IMPOSSIBLE_CODE, DEPLOYMENT_DELETE_NO_PERMISSION_CODE, DEPLOYMENT_DELETE_NO_DEPLOYMENT_CODE, \
     DEPLOYMENT_DELETE_FAILED_CODE, DEPLOYMENT_ACTION_SUCCESS_CODE, DEPLOYMENT_ACTION_IMPOSSIBLE_CODE, DEPLOYMENT_ACTION_NO_PERMISSION_CODE, \
-    DEPLOYMENT_ACTION_NO_DEPLOYMENT_CODE, DEPLOYMENT_ACTION_FAILED_CODE, DEPLOYMENT_PLAN_V1_API_OPS, DEPLOYMENT_PLAN_V2_API_OPS
+    DEPLOYMENT_ACTION_NO_DEPLOYMENT_CODE, DEPLOYMENT_ACTION_FAILED_CODE, DEPLOYMENT_PLAN_V1_API_OPS, DEPLOYMENT_PLAN_V2_API_OPS, \
+    ENVIRONMENTS_ENDPOINT, DEPLOYMENT_ENDPOINT
 from outsystems.vars.file_vars import DEPLOYMENTS_FILE, DEPLOYMENT_FILE, DEPLOYMENT_FOLDER, DEPLOYMENT_STATUS_FILE
 from outsystems.vars.pipeline_vars import DEPLOYMENT_STATUS_LIST, DEPLOYMENT_SAVED_STATUS
 
 
 # Returns a list of deployments ordered by creation date, from newest to oldest.
 def get_deployments(artifact_dir: str, endpoint: str, auth_token: str, date: str):
     # Builds the parameters for the api call
@@ -182,14 +183,40 @@
     elif status_code == DEPLOYMENT_NO_PERMISSION_CODE:
         raise NotEnoughPermissionsError(
             "You don't have enough permissions to create the deployment. Details: {}".format(response["response"]))
     elif status_code == DEPLOYMENT_NO_ENVIRONMENT_CODE:
         raise EnvironmentNotFoundError(
             "Can't find the source or target environment. Details: {}.".format(response["response"]))
     elif status_code == DEPLOYMENT_FAILED_CODE:
+        raise ServerError(
+            "Failed to create the deployment. Details: {}".format(response["response"]))
+    else:
+        raise NotImplementedError(
+            "There was an error. Response from server: {}".format(response))
+
+
+# Creates a deployment to a target environment.
+# The input is a binary file.
+def send_binary_deployment(artifact_dir: str, endpoint: str, auth_token: str, lt_api_version: int, dest_env: str, binary_path: str):
+    # Sends the request
+    response = send_binary_post_request(
+        endpoint, auth_token, ENVIRONMENTS_ENDPOINT, dest_env, DEPLOYMENT_ENDPOINT, binary_path)
+    status_code = int(response["http_status"])
+    if status_code == DEPLOYMENT_SUCCESS_CODE:
+        return response["response"]
+    elif status_code == DEPLOYMENT_INVALID_CODE:
+        raise InvalidParametersError("The request is invalid. Check the body of the request for errors. Details: {}.".format(
+            response["response"]))
+    elif status_code == DEPLOYMENT_NO_PERMISSION_CODE:
+        raise NotEnoughPermissionsError(
+            "You don't have enough permissions to create the deployment. Details: {}".format(response["response"]))
+    elif status_code == DEPLOYMENT_NO_ENVIRONMENT_CODE:
+        raise EnvironmentNotFoundError(
+            "Can't find the source or target environment. Details: {}.".format(response["response"]))
+    elif status_code == DEPLOYMENT_FAILED_CODE:
         raise ServerError(
             "Failed to create the deployment. Details: {}".format(response["response"]))
     else:
         raise NotImplementedError(
             "There was an error. Response from server: {}".format(response))
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/lifetime/lifetime_environments.py` & `outsystems-pipeline-0.9.0/outsystems/lifetime/lifetime_environments.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 # Exceptions
 from outsystems.exceptions.invalid_parameters import InvalidParametersError
 from outsystems.exceptions.environment_not_found import EnvironmentNotFoundError
 from outsystems.exceptions.not_enough_permissions import NotEnoughPermissionsError
 from outsystems.exceptions.app_does_not_exist import AppDoesNotExistError
 from outsystems.exceptions.server_error import ServerError
 # Functions
-from outsystems.lifetime.lifetime_base import send_get_request
+from outsystems.lifetime.lifetime_base import send_get_request, send_post_request
 from outsystems.lifetime.lifetime_applications import _get_application_info
 from outsystems.file_helpers.file import load_data, store_data, clear_cache
 # Variables
 from outsystems.vars.lifetime_vars import ENVIRONMENTS_ENDPOINT, ENVIRONMENT_APPLICATIONS_ENDPOINT, ENVIRONMENTS_SUCCESS_CODE, \
     ENVIRONMENTS_NOT_FOUND_CODE, ENVIRONMENTS_FAILED_CODE, ENVIRONMENT_APP_SUCCESS_CODE, ENVIRONMENT_APP_NOT_STATUS_CODE, \
     ENVIRONMENT_APP_NO_PERMISSION_CODE, ENVIRONMENT_APP_NOT_FOUND, ENVIRONMENT_APP_FAILED_CODE, ENVIRONMENT_DEPLOYMENT_ZONES_ENDPOINT, \
     ENVIRONMENT_ZONES_SUCCESS_CODE, ENVIRONMENT_ZONES_NOT_STATUS_CODE, ENVIRONMENT_ZONES_NO_PERMISSION_CODE, ENVIRONMENT_ZONES_NOT_FOUND, \
-    ENVIRONMENT_ZONES_FAILED_CODE
-from outsystems.vars.file_vars import ENVIRONMENTS_FILE, ENVIRONMENT_FOLDER, ENVIRONMENT_APPLICATION_FILE, ENVIRONMENT_DEPLOYMENT_ZONES_FILE
+    ENVIRONMENT_ZONES_FAILED_CODE, ENVIRONMENT_APPLICATIONS_SOURCECODE_ENDPOINT, ENVIRONMENT_SOURCECODE_PACKAGE_SUCCESS_CODE, \
+    ENVIRONMENT_SOURCECODE_LINK_SUCCESS_CODE, ENVIRONMENT_SOURCECODE_FAILED_CODE
+from outsystems.vars.file_vars import ENVIRONMENTS_FILE, ENVIRONMENT_FOLDER, ENVIRONMENT_APPLICATION_FILE, \
+    ENVIRONMENT_DEPLOYMENT_ZONES_FILE, ENVIRONMENT_SOURCECODE_FOLDER, ENVIRONMENT_SOURCECODE_STATUS_FILE, \
+    ENVIRONMENT_SOURCECODE_LINK_FILE
 
 
 # Lists all the environments in the infrastructure.
 def get_environments(artifact_dir: str, endpoint: str, auth_token: str):
     # Sends the request
     response = send_get_request(
         endpoint, auth_token, ENVIRONMENTS_ENDPOINT, None)
@@ -116,14 +119,99 @@
         raise ServerError(
             "Failed to access the deployment zones of environment. Details: {}".format(response["response"]))
     else:
         raise NotImplementedError(
             "There was an error. Response from server: {}".format(response))
 
 
+# Returns the package key to download the source code of the specified application in a given environment.
+def get_environment_app_source_code(artifact_dir: str, endpoint: str, auth_token: str, **kwargs):
+    # Tuple with (AppName, AppKey): app_tuple[0] = AppName; app_tuple[1] = AppKey
+    app_tuple = _get_application_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Tuple with (EnvName, EnvKey): env_tuple[0] = EnvName; env_tuple[1] = EnvKey
+    env_tuple = _get_environment_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Builds the query and arguments for the call to the API
+    query = "{}/{}/{}/{}/{}".format(ENVIRONMENTS_ENDPOINT, env_tuple[1],
+                                    ENVIRONMENT_APPLICATIONS_ENDPOINT, app_tuple[1],
+                                    ENVIRONMENT_APPLICATIONS_SOURCECODE_ENDPOINT)
+    # Sends the request
+    response = send_post_request(endpoint, auth_token, query, None)
+    status_code = int(response["http_status"])
+    if status_code == ENVIRONMENT_SOURCECODE_PACKAGE_SUCCESS_CODE:
+        return response["response"]
+    elif status_code == ENVIRONMENT_SOURCECODE_FAILED_CODE:
+        raise ServerError("Failed to access the source code of an application. Details: {}".format(
+            response["response"]))
+    else:
+        raise NotImplementedError(
+            "There was an error. Response from server: {}".format(response))
+
+
+# Returns current status of source code package of the specified application in a given environment.
+def get_environment_app_source_code_status(artifact_dir: str, endpoint: str, auth_token: str, **kwargs):
+    # Tuple with (AppName, AppKey): app_tuple[0] = AppName; app_tuple[1] = AppKey
+    app_tuple = _get_application_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Tuple with (EnvName, EnvKey): env_tuple[0] = EnvName; env_tuple[1] = EnvKey
+    env_tuple = _get_environment_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Builds the query and arguments for the call to the API
+    query = "{}/{}/{}/{}/{}/{}/status".format(ENVIRONMENTS_ENDPOINT, env_tuple[1],
+                                              ENVIRONMENT_APPLICATIONS_ENDPOINT, app_tuple[1],
+                                              ENVIRONMENT_APPLICATIONS_SOURCECODE_ENDPOINT, kwargs["pkg_key"])
+    # Sends the request
+    response = send_get_request(endpoint, auth_token, query, None)
+    status_code = int(response["http_status"])
+    if status_code == ENVIRONMENT_SOURCECODE_PACKAGE_SUCCESS_CODE:
+        # Stores the result
+        filename = "{}{}".format(
+            kwargs["pkg_key"], ENVIRONMENT_SOURCECODE_STATUS_FILE)
+        filename = os.path.join(ENVIRONMENT_SOURCECODE_FOLDER, filename)
+        store_data(artifact_dir, filename, response["response"])
+        return response["response"]
+    elif status_code == ENVIRONMENT_SOURCECODE_FAILED_CODE:
+        raise ServerError("Failed to access the source code package status of an application. Details: {}".format(
+            response["response"]))
+    else:
+        raise NotImplementedError(
+            "There was an error. Response from server: {}".format(response))
+
+
+# Returns download link of source code package of the specified application in a given environment.
+def get_environment_app_source_code_link(artifact_dir: str, endpoint: str, auth_token: str, **kwargs):
+    # Tuple with (AppName, AppKey): app_tuple[0] = AppName; app_tuple[1] = AppKey
+    app_tuple = _get_application_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Tuple with (EnvName, EnvKey): env_tuple[0] = EnvName; env_tuple[1] = EnvKey
+    env_tuple = _get_environment_info(
+        artifact_dir, endpoint, auth_token, **kwargs)
+    # Builds the query and arguments for the call to the API
+    query = "{}/{}/{}/{}/{}/{}/download".format(ENVIRONMENTS_ENDPOINT, env_tuple[1],
+                                                ENVIRONMENT_APPLICATIONS_ENDPOINT, app_tuple[1],
+                                                ENVIRONMENT_APPLICATIONS_SOURCECODE_ENDPOINT, kwargs["pkg_key"])
+    # Sends the request
+    response = send_get_request(endpoint, auth_token, query, None)
+    status_code = int(response["http_status"])
+    if status_code == ENVIRONMENT_SOURCECODE_LINK_SUCCESS_CODE:
+        # Stores the result
+        filename = "{}{}".format(
+            kwargs["pkg_key"], ENVIRONMENT_SOURCECODE_LINK_FILE)
+        filename = os.path.join(ENVIRONMENT_SOURCECODE_FOLDER, filename)
+        store_data(artifact_dir, filename, response["response"])
+        return response["response"]
+    elif status_code == ENVIRONMENT_SOURCECODE_FAILED_CODE:
+        raise ServerError("Failed to access the source code package link of an application. Details: {}".format(
+            response["response"]))
+    else:
+        raise NotImplementedError(
+            "There was an error. Response from server: {}".format(response))
+
+
 # ---------------------- PRIVATE METHODS ----------------------
 # Private method to get the App name or key into a tuple (name,key).
 def _get_environment_info(artifact_dir: str, api_url: str, auth_token: str, **kwargs):
     if "env_name" in kwargs:
         env_key = _find_environment_key(
             artifact_dir, api_url, auth_token, kwargs["env_name"])
         env_name = kwargs["env_name"]
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/manifest/manifest_base.py` & `outsystems-pipeline-0.9.0/outsystems/manifest/manifest_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/apply_configuration_values_to_target_env.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/apply_configuration_values_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/continue_deployment_to_target_env.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/continue_deployment_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_latest_tags_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/evaluate_test_results.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/evaluate_test_results.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_apps_packages.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_apps_packages.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_lifetime_data.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_lifetime_data.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/fetch_tech_debt.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/fetch_tech_debt.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/generate_unit_testing_assembly.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/generate_unit_testing_assembly.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/scan_test_endpoints.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/scan_test_endpoints.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/start_deployment_to_target_env.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/start_deployment_to_target_env.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/tag_apps_based_on_manifest_data.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/pipeline/tag_modified_apps.py` & `outsystems-pipeline-0.9.0/outsystems/pipeline/tag_modified_apps.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/properties/properties_base.py` & `outsystems-pipeline-0.9.0/outsystems/properties/properties_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/properties/properties_set_value.py` & `outsystems-pipeline-0.9.0/outsystems/properties/properties_set_value.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/ad_vars.py` & `outsystems-pipeline-0.9.0/outsystems/vars/ad_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/file_vars.py` & `outsystems-pipeline-0.9.0/outsystems/vars/file_vars.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,16 +21,20 @@
 ENVIRONMENTS_FILE = "environments.cache"
 ENVIRONMENT_FILE = ".cache"
 ENVIRONMENT_APPS_FILE = ".applications.cache"
 ENVIRONMENT_APPLICATION_FILE = ".applications.cache"
 ENVIRONMENT_VERSIONS_FILE = ".versions.cache"
 ENVIRONMENT_DEPLOYMENT_ZONES_FILE = ".deploymentzones.cache"
 ENVIRONMENT_FOLDER = "environment_data"
+ENVIRONMENT_SOURCECODE_FOLDER = "sourcecode_data"
+ENVIRONMENT_SOURCECODE_STATUS_FILE = ".status.cache"
+ENVIRONMENT_SOURCECODE_LINK_FILE = ".link.cache"
+ENVIRONMENT_SOURCECODE_DOWNLOAD_FILE = ".source.zip"
 
-# Environments vars
+# Deployments vars
 DEPLOYMENTS_FILE = "deployments.cache"
 DEPLOYMENT_FILE = ".cache"
 DEPLOYMENT_PLAN_FILE = ".plan.cache"
 DEPLOYMENT_MANIFEST_FILE = "deployment_manifest.cache"
 DEPLOYMENT_STATUS_FILE = ".status.cache"
 DEPLOYMENT_FOLDER = "deployment_data"
 
@@ -53,7 +57,14 @@
 AD_CATEGORIES_FILE = ".categories.cache"
 AD_INFRA_FILE = ".infrastructure.cache"
 AD_APP_FILE = ".application.cache"
 AD_FOLDER = "techdebt_data"
 
 # AirGap vars
 DEPLOYMENT_ORDER_FILE = "sorted_oap.list"
+
+# Solutions vars
+SOLUTIONS_OSP_FILE = ".osp"
+SOLUTIONS_LINK_FILE = ".link.cache"
+SOLUTIONS_STATUS_FILE = ".status.cache"
+SOLUTIONS_DEPLOY_FILE = ".deploy.cache"
+SOLUTIONS_FOLDER = "solution_data"
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/lifetime_vars.py` & `outsystems-pipeline-0.9.0/outsystems/vars/lifetime_vars.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 APPLICATION_VERSION_CREATE_INVALID_CODE = 400
 APPLICATION_VERSION_CREATE_NO_PERMISSION_CODE = 403
 APPLICATION_VERSION_CREATE_NO_ENVIRONMENT_CODE = 404
 APPLICATION_VERSION_CREATE_FAILED_CODE = 500
 
 # Deployments Endpoint Variables
 # Deployment list specific
+DEPLOYMENT_ENDPOINT = "deployment"
 DEPLOYMENTS_ENDPOINT = "deployments"
 DEPLOYMENTS_SUCCESS_CODE = 200
 DEPLOYMENTS_EMPTY_CODE = 204
 DEPLOYMENTS_INVALID_CODE = 400
 DEPLOYMENTS_NO_PERMISSION_CODE = 403
 DEPLOYMENTS_FAILED_CODE = 500
 DEPLOYMENT_MESSAGE = "Automated deploy via OutSystems Pipeline"
@@ -92,7 +93,37 @@
 # Environment deployment zones specific
 ENVIRONMENT_DEPLOYMENT_ZONES_ENDPOINT = "deploymentzones"
 ENVIRONMENT_ZONES_SUCCESS_CODE = 200
 ENVIRONMENT_ZONES_NOT_STATUS_CODE = 400
 ENVIRONMENT_ZONES_NO_PERMISSION_CODE = 403
 ENVIRONMENT_ZONES_NOT_FOUND = 404
 ENVIRONMENT_ZONES_FAILED_CODE = 500
+# Environment application source code specific
+ENVIRONMENT_APPLICATIONS_SOURCECODE_ENDPOINT = "sourcecodeaccess"
+ENVIRONMENT_SOURCECODE_LINK_SUCCESS_CODE = 200
+ENVIRONMENT_SOURCECODE_PACKAGE_SUCCESS_CODE = 201
+ENVIRONMENT_SOURCECODE_FAILED_CODE = 500
+# Solutions specific
+ENVIRONMENT_SOLUTION_ENDPOINT = "solution"
+ENVIRONMENT_SOLUTION_SUCCESS_CODE = 200
+ENVIRONMENT_SOLUTION_NOT_STATUS_CODE = 400
+ENVIRONMENT_SOLUTION_NO_PERMISSION_CODE = 403
+ENVIRONMENT_SOLUTION_NOT_FOUND = 404
+ENVIRONMENT_SOLUTION_FAILED_CODE = 500
+# Solutions status specific
+ENVIRONMENT_SOLUTION_STATUS_ENDPOINT = "solutionstatus"
+ENVIRONMENT_SOLUTION_STATUS_SUCCESS_CODE = 200
+ENVIRONMENT_SOLUTION_STATUS_NOT_STATUS_CODE = 400
+ENVIRONMENT_SOLUTION_STATUS_NO_PERMISSION_CODE = 403
+ENVIRONMENT_SOLUTION_STATUS_NOT_FOUND = 404
+ENVIRONMENT_SOLUTION_STATUS_FAILED_CODE = 500
+# Solutions link specific
+ENVIRONMENT_SOLUTION_LINK_SUCCESS_CODE = 200
+ENVIRONMENT_SOLUTION_LINK_FAILED_CODE = 400
+
+# Downloads Endpoint Variables
+DOWNLOADS_ENDPOINT = "downloads"
+DOWNLOAD_SUCCESS_CODE = 200
+DOWNLOAD_INVALID_KEY_CODE = 400
+DOWNLOAD_NO_PERMISSION_CODE = 403
+DOWNLOAD_NOT_FOUND = 404
+DOWNLOAD_FAILED_CODE = 500
```

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/manifest_vars.py` & `outsystems-pipeline-0.9.0/outsystems/vars/manifest_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/properties_vars.py` & `outsystems-pipeline-0.9.0/outsystems/vars/properties_vars.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems/vars/vars_base.py` & `outsystems-pipeline-0.9.0/outsystems/vars/vars_base.py`

 * *Files identical despite different names*

### Comparing `outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/PKG-INFO` & `outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outsystems-pipeline
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package to accelerate the integration of OutSystems with third-party CI/CD tools
 Home-page: https://github.com/OutSystems/outsystems-pipeline
 Author: OutSystems
 Author-email: cicd.integrations@outsystems.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -26,40 +26,42 @@
 
 Visit the `project repository <https://github.com/OutSystems/outsystems-pipeline>`_ on GitHub for instructions on how to build example OutSystems CI/CD pipelines with common DevOps automation tools, as well as documentation that will help you adapt the examples to your particular scenarios.
 
 
 What's new
 ==========
 
-**Config File Support**
- Load configuration values from a custom file to override default values. To use this feature, use the new `--config_file` parameter to specify the configuration file path.
- This enhancement is available in the following scripts:
-
- * `apply_configuration_values_to_target_env.py`
- * `continue_deployment_to_target_env.py`
- * `deploy_apps_to_target_env_with_airgap.py`
- * `deploy_latest_tags_to_target_env.py`
- * `deploy_tags_to_target_env_with_manifest.py`
- * `evaluate_test_results.py`
- * `fetch_apps_packages.py`
- * `fetch_lifetime_data.py`
- * `scan_test_endpoints.py`
- * `start_deployment_to_target_env.py`
- * `tag_apps_based_on_manifest_data.py`
- * `tag_modified_apps.py`
-
-**SSL Certificate Verification**
- The Python `requests` module verifies SSL certificates for HTTPS requests.
- Now there's a flag to enable (default value) or disable SSL certificate verification.
+**Download Application Source Code**
 
-**Fetch Technical Debt**
- Enhanced the `fetch_tech_debt` script to prevent failures when all modules of an app are marked as 'ignored' in AI Mentor Studio and when an app has no security findings.
+ A new script was added to download platform-generated source code:
 
-**Tag Modified Applications**
- Updated `tag_modified_apps` script to tag applications based on a app_list parameter or from the trigger_manifest artifact
+ * `fetch_apps_source_code.py`
+
+ Use the following parameters to generate more human-readable outputs and facilitate the compilation of the source code:
+
+ * --friendly_package_names: source code packages with user-friendly names.
+ * --include_all_refs: adds to .csproj file all assemblies in the bin folder as references.
+ * --remove_resources_files: removes references to embedded resources files from the.csproj file.
+
+**Solution Download and Deploy**
+
+ Added new functions to leverage the recently released/improved APIs to download and deploy outsystems packages:
+
+ * `fetch_lifetime_solution_from_manifest.py` - downloads a solution file based on manifest data.
+ * `deploy_package_to_target_env.py` - deploys an outsystems package (solution or application) to a target environment.
+ * `deploy_package_to_target_env_with_osptool.py` - deploys an outsystems package (solution or application) using OSP Tool.
+
+**Improved OSPTool Operations**
+
+ OSPTool command line calls now have live output callback and catalog mapping support.
+
+**Updated Package Dependencies**
+
+ * Updated python-dateutil dependency to version 2.9.0.post0
+ * Updated python-dotenv dependency to version 1.0.1
 
 Installing and upgrading
 ========================
 
 Install or upgrade outsystems-pipeline to the latest available version as follows:
 ::
```

### Comparing `outsystems-pipeline-0.8.0/outsystems_pipeline.egg-info/SOURCES.txt` & `outsystems-pipeline-0.9.0/outsystems_pipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,54 +15,62 @@
 outsystems/exceptions/__init__.py
 outsystems/exceptions/app_does_not_exist.py
 outsystems/exceptions/app_version_error.py
 outsystems/exceptions/deployment_not_found.py
 outsystems/exceptions/environment_not_found.py
 outsystems/exceptions/impossible_action_deployment.py
 outsystems/exceptions/invalid_json_response.py
+outsystems/exceptions/invalid_os_package.py
 outsystems/exceptions/invalid_parameters.py
 outsystems/exceptions/manifest_does_not_exist.py
 outsystems/exceptions/no_apps_available.py
 outsystems/exceptions/no_deployments.py
 outsystems/exceptions/not_enough_permissions.py
 outsystems/exceptions/osptool_error.py
 outsystems/exceptions/server_error.py
 outsystems/file_helpers/__init__.py
 outsystems/file_helpers/file.py
 outsystems/lifetime/__init__.py
 outsystems/lifetime/lifetime_applications.py
 outsystems/lifetime/lifetime_base.py
 outsystems/lifetime/lifetime_deployments.py
+outsystems/lifetime/lifetime_downloads.py
 outsystems/lifetime/lifetime_environments.py
+outsystems/lifetime/lifetime_solutions.py
 outsystems/manifest/__init__.py
 outsystems/manifest/manifest_base.py
 outsystems/osp_tool/__init__.py
 outsystems/osp_tool/osp_base.py
 outsystems/pipeline/__init__.py
 outsystems/pipeline/apply_configuration_values_to_target_env.py
 outsystems/pipeline/continue_deployment_to_target_env.py
 outsystems/pipeline/deploy_apps_to_target_env_with_airgap.py
 outsystems/pipeline/deploy_latest_tags_to_target_env.py
+outsystems/pipeline/deploy_package_to_target_env.py
+outsystems/pipeline/deploy_package_to_target_env_with_osptool.py
 outsystems/pipeline/deploy_tags_to_target_env_with_manifest.py
 outsystems/pipeline/evaluate_test_results.py
 outsystems/pipeline/fetch_apps_packages.py
+outsystems/pipeline/fetch_apps_source_code.py
 outsystems/pipeline/fetch_lifetime_data.py
+outsystems/pipeline/fetch_lifetime_solution_from_manifest.py
 outsystems/pipeline/fetch_tech_debt.py
 outsystems/pipeline/generate_unit_testing_assembly.py
 outsystems/pipeline/scan_test_endpoints.py
 outsystems/pipeline/start_deployment_to_target_env.py
 outsystems/pipeline/tag_apps_based_on_manifest_data.py
 outsystems/pipeline/tag_modified_apps.py
 outsystems/properties/__init__.py
 outsystems/properties/properties_base.py
 outsystems/properties/properties_set_value.py
 outsystems/vars/__init__.py
 outsystems/vars/ad_vars.py
 outsystems/vars/bdd_vars.py
 outsystems/vars/cicd_vars.py
+outsystems/vars/dotnet_vars.py
 outsystems/vars/file_vars.py
 outsystems/vars/lifetime_vars.py
 outsystems/vars/manifest_vars.py
 outsystems/vars/pipeline_vars.py
 outsystems/vars/properties_vars.py
 outsystems/vars/vars_base.py
 outsystems_pipeline.egg-info/PKG-INFO
```

### Comparing `outsystems-pipeline-0.8.0/setup.py` & `outsystems-pipeline-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,42 @@
 
 Visit the `project repository <https://github.com/OutSystems/outsystems-pipeline>`_ on GitHub for instructions on how to build example OutSystems CI/CD pipelines with common DevOps automation tools, as well as documentation that will help you adapt the examples to your particular scenarios.
 
 
 What's new
 ==========
 
-**Config File Support**
- Load configuration values from a custom file to override default values. To use this feature, use the new `--config_file` parameter to specify the configuration file path.
- This enhancement is available in the following scripts:
-
- * `apply_configuration_values_to_target_env.py`
- * `continue_deployment_to_target_env.py`
- * `deploy_apps_to_target_env_with_airgap.py`
- * `deploy_latest_tags_to_target_env.py`
- * `deploy_tags_to_target_env_with_manifest.py`
- * `evaluate_test_results.py`
- * `fetch_apps_packages.py`
- * `fetch_lifetime_data.py`
- * `scan_test_endpoints.py`
- * `start_deployment_to_target_env.py`
- * `tag_apps_based_on_manifest_data.py`
- * `tag_modified_apps.py`
-
-**SSL Certificate Verification**
- The Python `requests` module verifies SSL certificates for HTTPS requests.
- Now there's a flag to enable (default value) or disable SSL certificate verification.
+**Download Application Source Code**
 
-**Fetch Technical Debt**
- Enhanced the `fetch_tech_debt` script to prevent failures when all modules of an app are marked as 'ignored' in AI Mentor Studio and when an app has no security findings.
+ A new script was added to download platform-generated source code:
 
-**Tag Modified Applications**
- Updated `tag_modified_apps` script to tag applications based on a app_list parameter or from the trigger_manifest artifact
+ * `fetch_apps_source_code.py`
+
+ Use the following parameters to generate more human-readable outputs and facilitate the compilation of the source code:
+
+ * --friendly_package_names: source code packages with user-friendly names.
+ * --include_all_refs: adds to .csproj file all assemblies in the bin folder as references.
+ * --remove_resources_files: removes references to embedded resources files from the.csproj file.
+
+**Solution Download and Deploy**
+
+ Added new functions to leverage the recently released/improved APIs to download and deploy outsystems packages:
+
+ * `fetch_lifetime_solution_from_manifest.py` - downloads a solution file based on manifest data.
+ * `deploy_package_to_target_env.py` - deploys an outsystems package (solution or application) to a target environment.
+ * `deploy_package_to_target_env_with_osptool.py` - deploys an outsystems package (solution or application) using OSP Tool.
+
+**Improved OSPTool Operations**
+
+ OSPTool command line calls now have live output callback and catalog mapping support.
+
+**Updated Package Dependencies**
+
+ * Updated python-dateutil dependency to version 2.9.0.post0
+ * Updated python-dotenv dependency to version 1.0.1
 
 Installing and upgrading
 ========================
 
 Install or upgrade outsystems-pipeline to the latest available version as follows:
 ::
 
@@ -68,20 +70,20 @@
     'Topic :: Software Development :: Testing :: Acceptance',
     'Topic :: Software Development :: Testing :: BDD',
     'Topic :: Software Development :: Testing :: Unit',
     'Topic :: System :: Software Distribution'
 ]
 
 REQUIREMENTS = [
-    'python-dateutil==2.8.2',
+    'python-dateutil==2.9.0.post0',
     'requests==2.31.0',
     'unittest-xml-reporting==3.2.0',
     'xunitparser==1.3.4',
     'toposort==1.10',
-    'python-dotenv==1.0.0'
+    'python-dotenv==1.0.1'
 ]
 
 PACKAGES = [
     'outsystems',
     'outsystems.architecture_dashboard',
     'outsystems.bdd_framework',
     'outsystems.cicd_probe',
@@ -101,15 +103,15 @@
             version = version_file.read().replace('\n', '')
     else:
         # dummy version
         version = '1.0.0'
 
     setup(
         name=NAME,
-        version='0.8.0',
+        version='0.9.0',
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         keywords=' '.join(KEYWORDS),
         author=AUTHOR,
         author_email=EMAIL,
         url=URL,
         license=LICENSE,
```

