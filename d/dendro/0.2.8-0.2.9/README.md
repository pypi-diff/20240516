# Comparing `tmp/dendro-0.2.8.tar.gz` & `tmp/dendro-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dendro-0.2.8.tar", last modified: Mon Feb 19 21:13:21 2024, max compression
+gzip compressed data, was "dendro-0.2.9.tar", last modified: Tue Feb 20 13:19:07 2024, max compression
```

## Comparing `dendro-0.2.8.tar` & `dendro-0.2.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.332998 dendro-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-19 21:13:21.332998 dendro-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-19 21:12:27.000000 dendro-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.316998 dendro-0.2.8/dendro/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.316998 dendro-0.2.8/dendro/api_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.316998 dendro-0.2.8/dendro/api_helpers/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/MockMongoClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/_get_mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/_remove_id_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/clients/pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/_create_random_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/_get_project_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/_hide_secret_params_in_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/_model_dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/routers/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/client/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/routers/compute_resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/compute_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/compute_resource/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/routers/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/_authenticate_gui_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/compute_resource_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/create_job_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/file_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/find_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/github_auth_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/job_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12528 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/project_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/script_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/usage_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/gui/user_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.320998 dendro-0.2.8/dendro/api_helpers/routers/processor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/routers/processor/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/api_helpers/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/_create_output_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/_crypto_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/_remove_detached_files_and_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/api_helpers/services/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/gui/create_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/gui/delete_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/gui/get_compute_resource_user_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/gui/set_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/api_helpers/services/processor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/processor/_get_signed_upload_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/processor/get_upload_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/api_helpers/services/processor/update_job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/aws_batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/aws_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/aws_batch/aws_batch_job_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/client/
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/Project.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/client/_interim/
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/_interim/NwbRecording.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/_interim/NwbSorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/_interim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/client/submit_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.324998 dendro-0.2.8/dendro/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/common/_api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/common/_crypto_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/common/dendro_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.328998 dendro-0.2.8/dendro/compute_resource/
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/AppManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/ComputeResourceException.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/JobManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/PubsubClient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/SlurmJobHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/_run_job_in_aws_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/_start_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/register_compute_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/compute_resource/start_compute_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.328998 dendro-0.2.8/dendro/internal_job_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/internal_job_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/internal_job_monitoring/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/internal_job_monitoring/console_output_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/internal_job_monitoring/job_status_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/internal_job_monitoring/resource_utilization_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.332998 dendro-0.2.8/dendro/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/App.py
--rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/AppProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/FileManifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/InputFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/InputFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/Job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/OutputFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/OutputFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/ProcessorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/_load_spec_from_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/_make_spec_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/_run_job_child_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/_run_job_parent_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/_test_app_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/sdk/get_project_file_from_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 21:12:27.000000 dendro-0.2.8/dendro/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.332998 dendro-0.2.8/dendro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 21:13:21.000000 dendro-0.2.8/dendro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 21:13:21.332998 dendro-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-19 21:12:27.000000 dendro-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:13:21.332998 dendro-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_api_request_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_compute_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_crypto_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_github_auth_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-19 21:12:27.000000 dendro-0.2.8/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.449369 dendro-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-20 13:19:07.449369 dendro-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 13:18:06.000000 dendro-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.433369 dendro-0.2.9/dendro/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.433369 dendro-0.2.9/dendro/api_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.433369 dendro-0.2.9/dendro/api_helpers/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/MockMongoClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/_get_mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/_remove_id_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17509 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/clients/pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.433369 dendro-0.2.9/dendro/api_helpers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/_create_random_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/_get_project_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/_hide_secret_params_in_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/_model_dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/routers/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/client/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/routers/compute_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/compute_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/compute_resource/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/routers/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/_authenticate_gui_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/compute_resource_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/create_job_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/file_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/find_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/github_auth_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/job_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12528 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/project_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/script_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/usage_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/gui/user_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/routers/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/routers/processor/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.437369 dendro-0.2.9/dendro/api_helpers/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/_create_output_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/_crypto_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/_remove_detached_files_and_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/api_helpers/services/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/gui/create_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/gui/delete_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/gui/get_compute_resource_user_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/gui/set_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/api_helpers/services/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/processor/_get_signed_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/processor/get_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/api_helpers/services/processor/update_job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/aws_batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/aws_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/aws_batch/aws_batch_job_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/client/_interim/
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/_interim/NwbRecording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/_interim/NwbSorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/_interim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/client/submit_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.441369 dendro-0.2.9/dendro/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/common/_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/common/_crypto_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/common/dendro_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.445369 dendro-0.2.9/dendro/compute_resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/AppManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/ComputeResourceException.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/JobManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/PubsubClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/SlurmJobHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/_run_job_in_aws_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/_start_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/register_compute_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/compute_resource/start_compute_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.445369 dendro-0.2.9/dendro/internal_job_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/internal_job_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/internal_job_monitoring/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/internal_job_monitoring/console_output_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/internal_job_monitoring/job_status_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/internal_job_monitoring/resource_utilization_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.449369 dendro-0.2.9/dendro/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/App.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/AppProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/FileManifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/InputFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/InputFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/Job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/OutputFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/OutputFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/ProcessorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/_load_spec_from_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/_make_spec_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/_run_job_child_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/_run_job_parent_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/_test_app_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/sdk/get_project_file_from_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-20 13:18:06.000000 dendro-0.2.9/dendro/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.449369 dendro-0.2.9/dendro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-20 13:19:07.000000 dendro-0.2.9/dendro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 13:19:07.449369 dendro-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-20 13:18:06.000000 dendro-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:19:07.449369 dendro-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_api_request_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_compute_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_crypto_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_github_auth_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-20 13:18:06.000000 dendro-0.2.9/tests/test_sdk.py
```

### Comparing `dendro-0.2.8/PKG-INFO` & `dendro-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dendro
-Version: 0.2.8
+Version: 0.2.9
 Summary: Web framework for neurophysiology data analysis
 Home-page: https://github.com/flatironinstitute/dendro
 Author: Jeremy Magland, Luiz Tauffer
 Author-email: jmagland@flatironinstitute.org
 Requires-Dist: click
 Requires-Dist: simplejson
 Requires-Dist: numpy
```

### Comparing `dendro-0.2.8/dendro/api_helpers/clients/MockMongoClient.py` & `dendro-0.2.9/dendro/api_helpers/clients/MockMongoClient.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/clients/_get_mongo_client.py` & `dendro-0.2.9/dendro/api_helpers/clients/_get_mongo_client.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/clients/db.py` & `dendro-0.2.9/dendro/api_helpers/clients/db.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/clients/pubsub.py` & `dendro-0.2.9/dendro/api_helpers/clients/pubsub.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/core/_get_project_role.py` & `dendro-0.2.9/dendro/api_helpers/core/_get_project_role.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/core/settings.py` & `dendro-0.2.9/dendro/api_helpers/core/settings.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/client/router.py` & `dendro-0.2.9/dendro/api_helpers/routers/client/router.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/common.py` & `dendro-0.2.9/dendro/api_helpers/routers/common.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/compute_resource/router.py` & `dendro-0.2.9/dendro/api_helpers/routers/compute_resource/router.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/_authenticate_gui_request.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/_authenticate_gui_request.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/compute_resource_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/compute_resource_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/create_job_route.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/create_job_route.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/file_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/file_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/find_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/find_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/github_auth_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/github_auth_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/job_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/job_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/project_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/project_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/router.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/router.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/script_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/script_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/usage_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/usage_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/gui/user_routes.py` & `dendro-0.2.9/dendro/api_helpers/routers/gui/user_routes.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/routers/processor/router.py` & `dendro-0.2.9/dendro/api_helpers/routers/processor/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,20 +139,22 @@
 
         outputs: List[ProcessorGetJobResponseOutput] = []
         output_folders: List[ProcessorGetJobResponseOutputFolder] = []
         for output in job.outputFiles:
             if not output.isFolder:
                 # regular file
                 outputs.append(ProcessorGetJobResponseOutput(
-                    name=output.name
+                    name=output.name,
+                    skipCloudUpload=output.skipCloudUpload
                 ))
             else:
                 # folder
                 output_folders.append(ProcessorGetJobResponseOutputFolder(
-                    name=output.name
+                    name=output.name,
+                    skipCloudUpload=output.skipCloudUpload
                 ))
 
         parameters: List[ProcessorGetJobResponseParameter] = []
         for parameter in job.inputParameters:
             parameters.append(ProcessorGetJobResponseParameter(
                 name=parameter.name,
                 value=parameter.value
@@ -184,28 +186,29 @@
         return url
 
 # update job status
 class ProcessorUpdateJobStatusRequest(BaseModel):
     status: str
     error: Union[str, None] = None
     force_update: Union[bool, None] = None
+    output_file_sizes: Union[dict, None] = None
 
 class ProcessorUpdateJobStatusResponse(BaseModel):
     success: bool
 
 @router.put("/jobs/{job_id}/status")
 async def processor_update_job_status(job_id: str, data: ProcessorUpdateJobStatusRequest, job_private_key: str = Header(...)) -> ProcessorUpdateJobStatusResponse:
     try:
         job = await fetch_job(job_id, include_private_key=True)
         if job is None:
             raise Exception(f"No job with ID {job_id}")
         if job.jobPrivateKey != job_private_key:
             raise Exception(f"Invalid job private key for job {job_id}")
 
-        await update_job_status(job=job, status=data.status, error=data.error, force_update=data.force_update)
+        await update_job_status(job=job, status=data.status, error=data.error, force_update=data.force_update, output_file_sizes=data.output_file_sizes)
 
         return ProcessorUpdateJobStatusResponse(success=True)
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 # get job status
```

### Comparing `dendro-0.2.8/dendro/api_helpers/services/_create_output_file.py` & `dendro-0.2.9/dendro/api_helpers/services/_create_output_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     replace_pending: bool = False
 ) -> str: # returns the ID of the created file
     if url == 'pending':
         if replace_pending:
             raise Exception('Cannot replace pending file with another pending file')
         # this is the output of a job that has not completed yet
         size = 0
+    elif url.startswith('dendro:?'):  # case of skipCloudUpload3
+        size = _parse_size_from_dendro_uri(url)
     else:
         if not using_mock():
             if not is_folder:
                 size = await _get_size_for_remote_file(url)
             else:
                 size = await _get_size_from_file_manifest_json(url)
         else:
@@ -59,22 +61,29 @@
                 'fileName': file_name
             })
     else:
         if replace_pending:
             raise Exception('Cannot replace pending file because it does not exist')
         file_id = _create_random_id(8)
 
+    if url == 'pending':
+        content = 'pending'
+    elif url.startswith('dendro:?'):
+        # replace $file_id$ with file_id
+        content = url.replace('$file_id$', file_id)
+    else:
+        content = f'url:{url}'
     new_file = DendroFile(
         projectId=project_id,
         fileId=file_id,
         userId=user_id,
         fileName=file_name,
         size=size,
         timestampCreated=time.time(),
-        content=f'url:{url}' if url != 'pending' else 'pending',
+        content=content,
         metadata={},
         isFolder=is_folder,
         jobId=job_id
     )
     await files_collection.insert_one(_model_dump(new_file, exclude_none=True))
 
     if deleted_old_file:
@@ -119,7 +128,18 @@
         size = 0
         for f in file_manifest['files']:
             size += f['size']
         return size
     except Exception as e:
         print(f'Problem reading file manifest at {file_manifest_url}: {e}')
         return 0
+
+def _parse_size_from_dendro_uri(uri: str) -> int:
+    if not uri.startswith('dendro:?'):
+        raise Exception(f'Unexpected uri: {uri}')
+    query = uri[len('dendro:?'):]
+    parts = query.split('&')
+    for part in parts:
+        if part.startswith('size='):
+            size_str = part[len('size='):]
+            return int(size_str)
+    return 0
```

### Comparing `dendro-0.2.8/dendro/api_helpers/services/_crypto_keys.py` & `dendro-0.2.9/dendro/api_helpers/services/_crypto_keys.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/_remove_detached_files_and_jobs.py` & `dendro-0.2.9/dendro/api_helpers/services/_remove_detached_files_and_jobs.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/gui/create_job.py` & `dendro-0.2.9/dendro/api_helpers/services/gui/create_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
     output_files: List[DendroJobOutputFile] = []
     for output_file in output_files_from_request:
         output_files.append(
             DendroJobOutputFile(
                 name=output_file.name,
                 fileName=filter_output_file_name(output_file.fileName),
-                isFolder=output_file.isFolder
+                isFolder=output_file.isFolder,
+                skipCloudUpload=output_file.skipCloudUpload
             )
         )
 
     something_was_deleted = False
 
     # delete any existing output files
     for output_file in output_files:
```

### Comparing `dendro-0.2.8/dendro/api_helpers/services/gui/get_compute_resource_user_usage.py` & `dendro-0.2.9/dendro/api_helpers/services/gui/get_compute_resource_user_usage.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/gui/set_file.py` & `dendro-0.2.9/dendro/api_helpers/services/gui/set_file.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/processor/_get_signed_upload_url.py` & `dendro-0.2.9/dendro/api_helpers/services/processor/_get_signed_upload_url.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/processor/get_upload_url.py` & `dendro-0.2.9/dendro/api_helpers/services/processor/get_upload_url.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/api_helpers/services/processor/update_job_status.py` & `dendro-0.2.9/dendro/api_helpers/services/processor/update_job_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 from ...core.settings import get_settings
 from ...core._model_dump import _model_dump
 from .._create_output_file import _create_output_file
 from ...clients.db import update_job
 from ...clients.pubsub import publish_pubsub_message
 
 
-async def update_job_status(job: DendroJob, status: str, error: Union[str, None], force_update: Union[bool, None] = None):
+async def update_job_status(
+    job: DendroJob,
+    status: str,
+    error: Union[str, None],
+    force_update: Union[bool, None] = None,
+    output_file_sizes: Union[dict, None] = None
+):
     old_status = job.status
 
     new_status = status
     new_error = error
 
     if not force_update:
         if new_status == 'starting':
@@ -39,15 +45,24 @@
         output_bucket_base_url = get_settings().OUTPUT_BUCKET_BASE_URL
         if using_mock():
             output_bucket_base_url = 'https://mock-bucket'
         if output_bucket_base_url is None:
             raise Exception('Environment variable not set: OUTPUT_BUCKET_BASE_URL')
         output_file_ids = []
         for output_file in job.outputFiles:
-            output_file_url = f"{output_bucket_base_url}/dendro-outputs/{job.jobId}/{output_file.name}"
+            if not output_file.skipCloudUpload:
+                output_file_url = f"{output_bucket_base_url}/dendro-outputs/{job.jobId}/{output_file.name}"
+            else:
+                # file_id will be filled in
+                output_file_url = f'dendro:?project={job.projectId}&file_id=$file_id$&label={output_file.fileName}&compute_resource={job.computeResourceId}'
+                if output_file_sizes is not None:
+                    if output_file.name in output_file_sizes:
+                        output_file_url += f'&size={output_file_sizes[output_file.name]}'
+                if output_file.isFolder:
+                    output_file_url += '&folder=true'
             output_file_id = await _create_output_file(
                 file_name=output_file.fileName,
                 url=output_file_url,
                 project_id=job.projectId,
                 user_id=job.userId,
                 job_id=job.jobId,
                 replace_pending=True,
```

### Comparing `dendro-0.2.8/dendro/aws_batch/aws_batch_job_definition.py` & `dendro-0.2.9/dendro/aws_batch/aws_batch_job_definition.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/cli.py` & `dendro-0.2.9/dendro/cli.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/client/Project.py` & `dendro-0.2.9/dendro/client/Project.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/client/_interim/NwbRecording.py` & `dendro-0.2.9/dendro/client/_interim/NwbRecording.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/client/_interim/NwbSorting.py` & `dendro-0.2.9/dendro/client/_interim/NwbSorting.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/client/submit_job.py` & `dendro-0.2.9/dendro/client/submit_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     file_name: str
     is_folder: Union[bool, None] = None
 
 class SubmitJobOutputFile(BaseModel):
     name: str
     file_name: str
     is_folder: Union[bool, None] = None
+    skip_cloud_upload: Union[bool, None] = None
 
 class SubmitJobParameter(BaseModel):
     name: str
     value: Any
 
 def submit_job(*,
     project: Project,
@@ -79,15 +80,16 @@
         )
         for x in input_files
     ]
     request_output_files = [
         CreateJobRequestOutputFile(
             name=x.name,
             fileName=x.file_name,
-            isFolder=x.is_folder
+            isFolder=x.is_folder,
+            skipCloudUpload=x.skip_cloud_upload
         )
         for x in output_files
     ]
     request_parameters = [
         CreateJobRequestInputParameter(
             name=x.name,
             value=x.value
```

### Comparing `dendro-0.2.8/dendro/common/_api_request.py` & `dendro-0.2.9/dendro/common/_api_request.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/common/_crypto_keys.py` & `dendro-0.2.9/dendro/common/_crypto_keys.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/common/dendro_types.py` & `dendro-0.2.9/dendro/common/dendro_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     secret: Union[bool, None] = None
 
 class DendroJobOutputFile(BaseModel):
     name: str
     fileName: str
     fileId: Union[str, None] = None
     isFolder: Union[bool, None] = None
+    skipCloudUpload: Union[bool, None] = None
 
 class ComputeResourceSpecProcessorParameter(BaseModel):
     name: str
     description: str
     type: str
     default: Union[Any, None] = None
     options: Union[List[str], List[int], None] = None
@@ -203,17 +204,19 @@
 
 class ProcessorGetJobResponseInputFolder(BaseModel):
     name: str
     files: List[ProcessorGetJobResponseInputFolderFile]
 
 class ProcessorGetJobResponseOutput(BaseModel):
     name: str
+    skipCloudUpload: Union[bool, None] = None
 
 class ProcessorGetJobResponseOutputFolder(BaseModel):
     name: str
+    skipCloudUpload: Union[bool, None] = None
 
 class ProcessorGetJobResponseParameter(BaseModel):
     name: str
     value: Any
 
 class ProcessorGetJobResponse(BaseModel):
     jobId: str
@@ -257,14 +260,15 @@
     fileName: str
     isFolder: Union[bool, None] = None
 
 class CreateJobRequestOutputFile(BaseModel):
     name: str
     fileName: str
     isFolder: Union[bool, None] = None
+    skipCloudUpload: Union[bool, None] = None
 
 class CreateJobRequestInputParameter(BaseModel):
     name: str
     value: Union[Any, None]
 
 class CreateJobRequest(BaseModel):
     projectId: str
```

### Comparing `dendro-0.2.8/dendro/compute_resource/AppManager.py` & `dendro-0.2.9/dendro/compute_resource/AppManager.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/JobManager.py` & `dendro-0.2.9/dendro/compute_resource/JobManager.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/PubsubClient.py` & `dendro-0.2.9/dendro/compute_resource/PubsubClient.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/SlurmJobHandler.py` & `dendro-0.2.9/dendro/compute_resource/SlurmJobHandler.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/_run_job_in_aws_batch.py` & `dendro-0.2.9/dendro/compute_resource/_run_job_in_aws_batch.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/_start_job.py` & `dendro-0.2.9/dendro/compute_resource/_start_job.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/register_compute_resource.py` & `dendro-0.2.9/dendro/compute_resource/register_compute_resource.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/compute_resource/start_compute_resource.py` & `dendro-0.2.9/dendro/compute_resource/start_compute_resource.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/internal_job_monitoring/common.py` & `dendro-0.2.9/dendro/internal_job_monitoring/common.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/internal_job_monitoring/console_output_monitor.py` & `dendro-0.2.9/dendro/internal_job_monitoring/console_output_monitor.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/internal_job_monitoring/job_status_monitor.py` & `dendro-0.2.9/dendro/internal_job_monitoring/job_status_monitor.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/internal_job_monitoring/resource_utilization_monitor.py` & `dendro-0.2.9/dendro/internal_job_monitoring/resource_utilization_monitor.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/App.py` & `dendro-0.2.9/dendro/sdk/App.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/AppProcessor.py` & `dendro-0.2.9/dendro/sdk/AppProcessor.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/InputFile.py` & `dendro-0.2.9/dendro/sdk/InputFile.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/InputFolder.py` & `dendro-0.2.9/dendro/sdk/InputFolder.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/Job.py` & `dendro-0.2.9/dendro/sdk/Job.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     ) -> None:
         self._job_id = job_id
         self._job_private_key = job_private_key
         resp = _job_info_manager.get_job_info_v2(job_id=job_id, job_private_key=job_private_key)
         # important to set these only once here because these objects will be passed into the processor function
         self._inputs = [InputFile(name=i.name, job_id=self._job_id, job_private_key=self._job_private_key) for i in resp.inputs]
         self._input_folders = [InputFolder(name=i.name, job_id=self._job_id, job_private_key=self._job_private_key) for i in resp.inputFolders] if resp.inputFolders else None
-        self._outputs = [OutputFile(name=o.name, job_id=self._job_id, job_private_key=self._job_private_key) for o in resp.outputs]
-        self._output_folders = [OutputFolder(name=o.name, job_id=self._job_id, job_private_key=self._job_private_key) for o in resp.outputFolders] if resp.outputFolders else None
+        self._outputs = [OutputFile(name=o.name, job_id=self._job_id, job_private_key=self._job_private_key, skip_cloud_upload=o.skipCloudUpload) for o in resp.outputs]
+        self._output_folders = [OutputFolder(name=o.name, job_id=self._job_id, job_private_key=self._job_private_key, skip_cloud_upload=o.skipCloudUpload) for o in resp.outputFolders] if resp.outputFolders else None
         self._parameters = [JobParameter(name=p.name, value=p.value) for p in resp.parameters]
         self._processor_name = resp.processorName
 
         for input in self._inputs:
             input._check_file_cache()
     @property
     def job_id(self) -> str:
```

### Comparing `dendro-0.2.8/dendro/sdk/OutputFile.py` & `dendro-0.2.9/dendro/sdk/OutputFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 class SetOutputFileException(Exception):
     pass
 
 class OutputFile(BaseModel):
     name: Union[str, None] = None # the name of the output within the context of the processor (not needed when output_file_name is specified for local testing)
     job_id: Union[str, None] = None
     job_private_key: Union[str, None] = None
+    skip_cloud_upload: Union[bool, None] = None
     was_uploaded: bool = False
     output_file_name: Union[str, None] = None # for local testing
+    size: Union[int, None] = None
     def set(self, local_file_name: str):
         print('output.set() is deprecated. Please use output.upload() instead.')
         self.upload(local_file_name)
     def upload(self, local_file_name: str):
         from .Job import _get_upload_url_for_output_file # avoid circular import
         from .Job import _get_file_id_for_output_file # avoid circular import
 
@@ -43,33 +45,43 @@
         else:
             if self.name is None:
                 raise Exception('Unexpected: name is None in OutputFile')
             if self.job_id is None:
                 raise Exception('Unexpected: job_id is None in OutputFile')
             if self.job_private_key is None:
                 raise Exception('Unexpected: job_private_key is None in OutputFile')
-            upload_url = _get_upload_url_for_output_file(name=self.name, job_id=self.job_id, job_private_key=self.job_private_key)
+            if not self.skip_cloud_upload:
+                upload_url = _get_upload_url_for_output_file(name=self.name, job_id=self.job_id, job_private_key=self.job_private_key)
 
-            # Upload the file to the URL
-            print(f'Uploading output file {self.name}') # it could be a security issue to provide the url in this print statement
-            with open(local_file_name, 'rb') as f:
-                if not using_mock():
-                    resp_upload = requests.put(upload_url, data=f, timeout=60 * 60 * 24 * 7)
-                    if resp_upload.status_code != 200:
-                        print(upload_url)
-                        raise SetOutputFileException(f'Error uploading file to bucket ({resp_upload.status_code}) {resp_upload.reason}: {resp_upload.text}')
+                # Upload the file to the URL
+                print(f'Uploading output file {self.name}') # it could be a security issue to provide the url in this print statement
+                with open(local_file_name, 'rb') as f:
+                    if not using_mock():
+                        resp_upload = requests.put(upload_url, data=f, timeout=60 * 60 * 24 * 7)
+                        if resp_upload.status_code != 200:
+                            print(upload_url)
+                            raise SetOutputFileException(f'Error uploading file to bucket ({resp_upload.status_code}) {resp_upload.reason}: {resp_upload.text}')
+            else:
+                print(f'Skipping cloud upload for output file {self.name}')
 
             # Write to the file cache
             if FILE_CACHE_DIR:
                 file_id = _get_file_id_for_output_file(name=self.name, job_id=self.job_id, job_private_key=self.job_private_key)
                 file_cache_path = os.path.join(FILE_CACHE_DIR, file_id)
                 if not os.path.exists(file_cache_path):
                     print(f'Moving {local_file_name} to {file_cache_path}')
                     shutil.move(local_file_name, file_cache_path)
 
+            # Determine the size of the file
+            # This is important for the case of skipCloudUpload=True
+            if os.path.exists(local_file_name):
+                self.size = os.path.getsize(local_file_name)
+            else:
+                self.size = 0
+
             # In all cases we delete the local file because then we don't have different behavior in different cases
             print(f'Deleting local file {local_file_name}')
             if os.path.exists(local_file_name):
                 os.remove(local_file_name)
 
         self.was_uploaded = True
```

### Comparing `dendro-0.2.8/dendro/sdk/OutputFolder.py` & `dendro-0.2.9/dendro/sdk/OutputFolder.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 class SetOutputFolderException(Exception):
     pass
 
 class OutputFolder(BaseModel):
     name: Union[str, None] = None # the name of the output within the context of the processor (not needed when output_folder_name is specified for local testing)
     job_id: Union[str, None] = None
     job_private_key: Union[str, None] = None
+    skip_cloud_upload: Union[bool, None] = None
     was_uploaded: bool = False
     output_folder_name: Union[str, None] = None # for local testing
+    size: Union[int, None] = None
     def upload(self, local_folder_name: str):
         from .Job import _get_upload_url_for_output_folder_file # avoid circular import
 
+        self.size = _recursive_compute_size_of_folder(local_folder_name)
+
         if self.output_folder_name is not None:
             if self.job_id is not None:
                 raise Exception('Cannot specify both output_folder_name and job_id in OutputFolder')
             if self.job_private_key is not None:
                 raise Exception('Cannot specify both output_folder_name and job_private_key in OutputFolder')
             # copy local_folder_name to output_folder_name
             print(f'Copying output {self.name} to {self.output_folder_name}')
@@ -46,27 +50,30 @@
                     for relative_file_name in all_relative_file_names
                 ]
             }
             with open(local_folder_name + '/file_manifest.json', 'w') as f:
                 import json
                 json.dump(file_manifest, f)
             all_relative_file_names.append('file_manifest.json')
-            for relative_file_name in all_relative_file_names:
-                local_file_name = local_folder_name + '/' + relative_file_name
-                upload_url = _get_upload_url_for_output_folder_file(name=self.name, relative_file_name=relative_file_name, job_id=self.job_id, job_private_key=self.job_private_key)
-
-                # Upload the file to the URL
-                print(f'Uploading output file {self.name} {relative_file_name}')
-
-                with open(local_file_name, 'rb') as f:
-                    if not using_mock():
-                        resp_upload = requests.put(upload_url, data=f, timeout=60 * 60 * 24 * 7)
-                        if resp_upload.status_code != 200:
-                            print(upload_url)
-                            raise SetOutputFolderException(f'Error uploading folder file to bucket ({resp_upload.status_code}) {resp_upload.reason}: {resp_upload.text}')
+            if not self.skip_cloud_upload:
+                for relative_file_name in all_relative_file_names:
+                    local_file_name = local_folder_name + '/' + relative_file_name
+                    upload_url = _get_upload_url_for_output_folder_file(name=self.name, relative_file_name=relative_file_name, job_id=self.job_id, job_private_key=self.job_private_key)
+
+                    # Upload the file to the URL
+                    print(f'Uploading output file {self.name} {relative_file_name}')
+
+                    with open(local_file_name, 'rb') as f:
+                        if not using_mock():
+                            resp_upload = requests.put(upload_url, data=f, timeout=60 * 60 * 24 * 7)
+                            if resp_upload.status_code != 200:
+                                print(upload_url)
+                                raise SetOutputFolderException(f'Error uploading folder file to bucket ({resp_upload.status_code}) {resp_upload.reason}: {resp_upload.text}')
+            else:
+                print(f'Skipping cloud upload for output folder {self.name}')
 
         self.was_uploaded = True
 
     # validator is needed to be an allowed pydantic type
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
@@ -82,7 +89,16 @@
     import os
     ret: List[str] = []
     for root, dirs, files in os.walk(local_folder_name):
         for file in files:
             relative_file_name = os.path.relpath(os.path.join(root, file), local_folder_name)
             ret.append(relative_file_name)
     return ret
+
+def _recursive_compute_size_of_folder(local_folder_name: str):
+    import os
+    total_size = 0
+    for dirpath, dirnames, filenames in os.walk(local_folder_name):
+        for f in filenames:
+            fp = os.path.join(dirpath, f)
+            total_size += os.path.getsize(fp)
+    return total_size
```

### Comparing `dendro-0.2.8/dendro/sdk/_load_spec_from_uri.py` & `dendro-0.2.9/dendro/sdk/_load_spec_from_uri.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/_make_spec_file.py` & `dendro-0.2.9/dendro/sdk/_make_spec_file.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro/sdk/_run_job_child_process.py` & `dendro-0.2.9/dendro/sdk/_run_job_child_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import List
+import os
+import json
 from .InputFile import InputFile
 from .InputFolder import InputFolder
 from .Job import Job
 from .AppProcessor import AppProcessor
 from ..common._api_request import _processor_get_api_request
 
 
@@ -142,14 +144,33 @@
     print('[dendro] Checking outputs')
     for output in processor._outputs:
         output_file = next((o for o in job.outputs if o.name == output.name), None)
         assert output_file is not None, f'Output not found: {output.name}'
         if not output_file.was_uploaded:
             raise Exception(f'Output was not uploaded: {output.name}')
 
+    # Write the output_file_sizes.json file
+    # This is especially important for the case of skipCloudUpload=True
+    print('[dendro] Writing output_file_sizes.json')
+    if os.path.exists('_dendro'):
+        output_file_sizes_fname = '_dendro/output_file_sizes.json'
+        output_file_sizes = {}
+        for output in processor._outputs:
+            output_file = next((o for o in job.outputs if o.name == output.name), None)
+            if output_file is not None and output_file.size is not None:
+                output_file_sizes[output.name] = output_file.size
+        for output in processor._output_folders:
+            output_folder = next((o for o in job.output_folders if o.name == output.name), None)
+            if output_folder is not None and output_folder.size is not None:
+                output_file_sizes[output.name] = output_folder.size
+        with open(output_file_sizes_fname, 'w') as f:
+            json.dump(output_file_sizes, f)
+    else:
+        print(f'WARNING: Cannot write output_file_sizes.json: _dendro directory does not exist in current working directory: {os.getcwd()}')
+
     # Print a message indicating that the job is complete
     print(f'[dendro] Job complete: {job_id}')
 
 def _get_job(*, job_id: str, job_private_key: str) -> Job:
     """Get a job from the dendro API"""
     job = Job(
         job_id=job_id,
```

### Comparing `dendro-0.2.8/dendro/sdk/_run_job_parent_process.py` & `dendro-0.2.9/dendro/sdk/_run_job_parent_process.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import time
+import json
 from typing import Union, Optional, Dict, Any
 import subprocess
 from ..common._api_request import _processor_put_api_request
 from ..mock import using_mock
 from ..internal_job_monitoring.console_output_monitor import do_upload as _upload_final_console_output
 import shutil
 
@@ -164,17 +165,26 @@
             job_id=job_id,
             job_private_key=job_private_key,
             console_out_file=console_out_fname
         )
         if not ok:
             _debug_log('WARNING: problem uploading final console output')
 
+    # get the output file sizes
+    # this is important for the case of skipCloudUpload=True
+    _debug_log('Reading output file sizes')
+    output_file_sizes_fname = f'{dendro_internal_folder}/output_file_sizes.json'
+    output_file_sizes = None
+    if os.path.exists(output_file_sizes_fname):
+        with open(output_file_sizes_fname, 'r') as f:
+            output_file_sizes = json.load(f)
+
     # Set the final job status
     _debug_log('Finalizing job')
-    _finalize_job(job_id=job_id, job_private_key=job_private_key, succeeded=succeeded, error_message=error_message)
+    _finalize_job(job_id=job_id, job_private_key=job_private_key, succeeded=succeeded, error_message=error_message, output_file_sizes=output_file_sizes)
 
     _debug_log('Exiting')
 
 def _launch_job_child_process(*, job_id: str, job_private_key: str, app_executable: str, console_out_file: Any):
     if not using_mock(): # pragma: no cover
         # Set the appropriate environment variables and launch the job in a background process
         cmd = app_executable
@@ -227,47 +237,55 @@
 
             return proc
         finally:
             os.chdir(old_working_dir)
             if 'main' in sys.modules:
                 del sys.modules['main'] # important to do this so that at a later time we can load a different main.py
 
-def _finalize_job(*, job_id: str, job_private_key: str, succeeded: bool, error_message: str):
+def _finalize_job(*, job_id: str, job_private_key: str, succeeded: bool, error_message: str, output_file_sizes: Union[dict, None] = None):
     try:
         if succeeded:
             # The job has completed successfully - update the status accordingly
             _debug_log('Setting job status to completed')
             print('Job completed')
-            _set_job_status(job_id=job_id, job_private_key=job_private_key, status='completed')
+            _set_job_status(job_id=job_id, job_private_key=job_private_key, status='completed', output_file_sizes=output_file_sizes)
         else:
             # The job has failed - update the status accordingly and set the error message
             _debug_log('Setting job status to failed: ' + error_message)
             print('Job failed: ' + error_message)
             _set_job_status(job_id=job_id, job_private_key=job_private_key, status='failed', error=error_message)
     except Exception as e: # pylint: disable=broad-except
         # This is unfortunate - we completed the job, but somehow failed to update the status in the dendro system - maybe there was a network error (maybe we should retry?)
         _debug_log('WARNING: problem setting final job status: ' + str(e))
         print('WARNING: problem setting final job status: ' + str(e))
 
 class SetJobStatusError(Exception):
     pass
 
-def _set_job_status(*, job_id: str, job_private_key: str, status: str, error: Optional[str] = None):
+def _set_job_status(*,
+    job_id: str,
+    job_private_key: str,
+    status: str,
+    error: Optional[str] = None,
+    output_file_sizes: Union[dict, None] = None
+):
     """Set the status of a job in the dendro API"""
     url_path = f'/api/processor/jobs/{job_id}/status'
     headers = {
         'job-private-key': job_private_key
     }
     data: Dict[str, Any] = {
         'status': status
     }
     if error is not None:
         data['error'] = error
     if os.environ.get('DENDRO_FORCE_STATUS_UPDATES', None) == '1':
         data['force_update'] = True
+    if output_file_sizes is not None:
+        data['output_file_sizes'] = output_file_sizes
     resp = _processor_put_api_request(
         url_path=url_path,
         headers=headers,
         data=data
     )
     if not resp['success']:
         raise SetJobStatusError(f'Error setting job status: {resp["error"]}')
```

### Comparing `dendro-0.2.8/dendro/sdk/get_project_file_from_uri.py` & `dendro-0.2.9/dendro/sdk/get_project_file_from_uri.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/dendro.egg-info/PKG-INFO` & `dendro-0.2.9/dendro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dendro
-Version: 0.2.8
+Version: 0.2.9
 Summary: Web framework for neurophysiology data analysis
 Home-page: https://github.com/flatironinstitute/dendro
 Author: Jeremy Magland, Luiz Tauffer
 Author-email: jmagland@flatironinstitute.org
 Requires-Dist: click
 Requires-Dist: simplejson
 Requires-Dist: numpy
```

### Comparing `dendro-0.2.8/dendro.egg-info/SOURCES.txt` & `dendro-0.2.9/dendro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/setup.py` & `dendro-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_api_request_failures.py` & `dendro-0.2.9/tests/test_api_request_failures.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_client.py` & `dendro-0.2.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_compute_resource.py` & `dendro-0.2.9/tests/test_compute_resource.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_integration.py` & `dendro-0.2.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_misc.py` & `dendro-0.2.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dendro-0.2.8/tests/test_sdk.py` & `dendro-0.2.9/tests/test_sdk.py`

 * *Files identical despite different names*

