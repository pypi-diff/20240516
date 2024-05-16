# Comparing `tmp/bigflow-1.8.0.tar.gz` & `tmp/bigflow-1.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigflow-1.8.0.tar", last modified: Thu Jul 13 06:45:08 2023, max compression
+gzip compressed data, was "bigflow-1.9.0.dev1.tar", last modified: Thu May 16 15:23:28 2024, max compression
```

## Comparing `bigflow-1.8.0.tar` & `bigflow-1.9.0.dev1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-13 06:44:09.000000 bigflow-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 06:44:09.000000 bigflow-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 06:44:09.000000 bigflow-1.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-13 06:45:08.158999 bigflow-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-13 06:44:09.000000 bigflow-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/dataset_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21110 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/bigquery/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/build/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow/build/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/build/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    35088 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dagbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/dataflow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/infra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/migrate-11/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/.gitignore.j2
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/pyproject.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.150999 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/scaffold/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/bigflow/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/testing/isolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-07-13 06:44:09.000000 bigflow-1.8.0/bigflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.146999 bigflow-1.8.0/bigflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 06:45:08.000000 bigflow-1.8.0/bigflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-13 06:44:09.000000 bigflow-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 06:44:09.000000 bigflow-1.8.0/scripts/bf
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 06:44:09.000000 bigflow-1.8.0/scripts/bigflow
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 06:45:08.158999 bigflow-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 06:44:09.000000 bigflow-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/buildd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/buildd/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_operate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_reflect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/buildd/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_duplicated_workflows/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_log_name_workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.154999 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/cli_logs_regular_workflows/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    41823 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/cli/test_module/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused1.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused2.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/Unused3.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/cli/test_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/dagbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/dagbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/dagbuilder/test_dagbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23905 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_konfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/test_user_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_user_commons/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 06:45:08.158999 bigflow-1.8.0/test/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/nonpure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-13 06:44:09.000000 bigflow-1.8.0/test/testing/test_isolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/dataset_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21110 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/bigquery/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.360075 bigflow-1.9.0.dev1/bigflow/build/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/operate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/build/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35173 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dagbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10006 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/dataflow/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/konfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/migrate-11/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/migrate-11/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/pyproject.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/resources/requirements.in.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.364075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/config.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/processing.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/scaffold/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/bigflow/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/testing/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13832 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/bigflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/bigflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 15:23:28.000000 bigflow-1.9.0.dev1/bigflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.368075 bigflow-1.9.0.dev1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/scripts/bf
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/scripts/bigflow
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:23:28.384075 bigflow-1.9.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/buildd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/buildd/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_operate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_reflect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/buildd/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_duplicated_workflows/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.372075 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_log_name_workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/cli_logs_regular_workflows/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42553 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/cli/test_module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/Unused3.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/cli/test_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/dagbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/dagbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/dagbuilder/test_dagbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14048 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23905 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_konfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/test_user_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_user_commons/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:23:28.376075 bigflow-1.9.0.dev1/test/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/nonpure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-16 15:22:40.000000 bigflow-1.9.0.dev1/test/testing/test_isolate.py
```

### Comparing `bigflow-1.8.0/LICENSE` & `bigflow-1.9.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/NOTICE` & `bigflow-1.9.0.dev1/NOTICE`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/PKG-INFO` & `bigflow-1.9.0.dev1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: bigflow
-Version: 1.8.0
-Summary: BigQuery client wrapper with clean API
-Home-page: https://github.com/allegro/bigflow
-Author: Pogranicze
-Author-email: pogranicze-team@allegro.pl
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: bigquery
-Provides-Extra: dataflow
-Provides-Extra: base_frozen
-License-File: LICENSE
-License-File: NOTICE
-
 # BigFlow
 
 ## Documentation
 
 1. [What is BigFlow?](#what-is-bigflow)
 1. [Getting started](#getting-started)
 1. [Installing Bigflow](#installing-bigflow)
```

### Comparing `bigflow-1.8.0/bigflow/__init__.py` & `bigflow-1.9.0.dev1/bigflow/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/__init__.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/dataset_configuration.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/dataset_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/dataset_manager.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/interactive.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/interface.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/interface.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/bigquery/job.py` & `bigflow-1.9.0.dev1/bigflow/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/dev.py` & `bigflow-1.9.0.dev1/bigflow/build/dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/dist.py` & `bigflow-1.9.0.dev1/bigflow/build/dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/legacy.py` & `bigflow-1.9.0.dev1/bigflow/build/legacy.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/operate.py` & `bigflow-1.9.0.dev1/bigflow/build/operate.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     cmd = ["docker", "build", project_spec.project_dir, "--tag", tag]
 
     if cache_params:
 
         logger.debug("Authenticate to docker registry")
         bigflow.deploy.authenticate_to_registry(
             auth_method=cache_params.auth_method or bigflow.deploy.AuthorizationType.LOCAL_ACCOUNT,
+            docker_repository=project_spec.docker_repository,
             vault_endpoint=cache_params.vault_endpoint,
             vault_secret=cache_params.vault_secret,
             vault_endpoint_verify=cache_params.vault_endpoint_verify
         )
 
         for image in (cache_params.cache_from_image or []):
             logger.debug("Add --cache-from=%s to `docker build`", image)
```

### Comparing `bigflow-1.8.0/bigflow/build/pip.py` & `bigflow-1.9.0.dev1/bigflow/build/pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/reflect.py` & `bigflow-1.9.0.dev1/bigflow/build/reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/build/spec.py` & `bigflow-1.9.0.dev1/bigflow/build/spec.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/cli.py` & `bigflow-1.9.0.dev1/bigflow/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,28 +428,34 @@
                              'If not set, {current_dir}/deployment_config.py will be used.')
 
 
 def _add_deploy_parsers_common_arguments(parser):
     _add_auth_parsers_arguments(parser)
     _add_parsers_common_arguments(parser)
 
+    parser.add_argument('-r', '--docker-repository',
+                        type=str,
+                        help='Name of a local and target Docker repository. Typically, a target repository is hosted by Google Cloud Artifact Registry.'
+                             ' If so, with the following naming schema: {HOSTNAME}/{PROJECT-ID}/{IMAGE}.'
+                        )
+
 
 def _create_deploy_parser(subparsers):
     parser = subparsers.add_parser('deploy',
                                    description='Performs complete deployment. Uploads DAG files from local DAGs folder '
-                                               'to Composer and uploads Docker image to Container Registry.')
+                                               'to Composer and uploads Docker image to Artifact Registry.')
 
     _add_deploy_dags_parser_arguments(parser)
     _add_deploy_image_parser_arguments(parser)
     _add_deploy_parsers_common_arguments(parser)
 
 
 def _create_deploy_image_parser(subparsers):
     parser = subparsers.add_parser('deploy-image',
-                                   description='Uploads Docker image to Container Registry.'
+                                   description='Uploads Docker image to Artifact Registry.'
                                    )
 
     _add_deploy_image_parser_arguments(parser)
     _add_deploy_parsers_common_arguments(parser)
 
 
 def _create_deploy_dags_parser(subparsers):
@@ -477,19 +483,14 @@
                              " If not specified, default ssh configuration will be used.")
 
 
 def _add_deploy_image_parser_arguments(parser):
     parser.add_argument('-i', '--image-tar-path',
                         type=str,
                         help='Path to a Docker image file. The file name must contain version number with the following naming schema: image-{version}.tar')
-    parser.add_argument('-r', '--docker-repository',
-                        type=str,
-                        help='Name of a local and target Docker repository. Typically, a target repository is hosted by Google Cloud Container Registry.'
-                             ' If so, with the following naming schema: {HOSTNAME}/{PROJECT-ID}/{IMAGE}.'
-                        )
 
 def _add_deploy_dags_parser_arguments(parser):
     parser.add_argument('-dd', '--dags-dir',
                         type=str,
                         help="Path to the folder with DAGs to deploy."
                              " If not set, {current_dir}/.dags will be used.")
     parser.add_argument('-cdf', '--clear-dags-folder',
@@ -549,15 +550,16 @@
     bigflow.deploy.deploy_dags_folder(dags_dir=_resolve_dags_dir(args),
                        dags_bucket=_resolve_property(args, 'dags_bucket'),
                        clear_dags_folder=args.clear_dags_folder,
                        auth_method=args.auth_method,
                        vault_endpoint=_resolve_vault_endpoint(args),
                        vault_endpoint_verify=_resolve_property(args, 'vault_endpoint_verify', ignore_value_error=True),
                        vault_secret=vault_secret,
-                       project_id=_resolve_property(args, 'gcp_project_id')
+                       project_id=_resolve_property(args, 'gcp_project_id'),
+                       docker_repository=_resolve_property(args, 'docker_repository')
                        )
 
 
 def _cli_deploy_image(args):
 
     docker_repository = _resolve_property(args, 'docker_repository')
     vault_secret = _resolve_property(args, 'vault_secret', ignore_value_error=True)
```

### Comparing `bigflow-1.8.0/bigflow/commons.py` & `bigflow-1.9.0.dev1/bigflow/commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/configuration.py` & `bigflow-1.9.0.dev1/bigflow/configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/dagbuilder.py` & `bigflow-1.9.0.dev1/bigflow/dagbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     dag_chunks = []
     dag_chunks.append(dedent(f"""\
         # This file was generated by `bigflow build-dags`
         # bigflow-workflow:  \t{workflow.workflow_id}
         # bigflow-build-ver: \t{build_ver}
         # bigflow-startdate: \t{start_from.isoformat()}
-        # biglfow-imageid:   \t{image_version}
+        # bigflow-imageid:   \t{image_version}
 
         import datetime
         from airflow import DAG
         from airflow import version
         
         try:
             from airflow.kubernetes.secret import Secret
```

### Comparing `bigflow-1.8.0/bigflow/dataflow/io.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/io.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/dataflow/job.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/dataflow/ml.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/ml.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/dataflow/options.py` & `bigflow-1.9.0.dev1/bigflow/dataflow/options.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/deploy.py` & `bigflow-1.9.0.dev1/bigflow/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,51 +127,56 @@
     vault_endpoint_verify: str | bool | None = None,
     vault_secret: str | None = None,
 ) -> str:
     docker_image = docker_repository + ":" + build_ver
     docker_image_latest = docker_repository + ":latest"
     tag_image(image_id, docker_repository, "latest")
 
-    logger.info("Deploying docker image tag=%s auth_method=%s", docker_image, auth_method)
-    authenticate_to_registry(auth_method, vault_endpoint, vault_secret, vault_endpoint_verify)
+    logger.info(
+        "Deploying docker image tag=%s auth_method=%s docker_repository=%s",
+        docker_image, auth_method, docker_repository)
+    authenticate_to_registry(auth_method, docker_repository, vault_endpoint, vault_secret, vault_endpoint_verify)
     bf_commons.run_process(['docker', 'push', docker_image])
     bf_commons.run_process(['docker', 'push', docker_image_latest])
 
     return docker_image
 
 
 def authenticate_to_registry(
         auth_method: AuthorizationType,
+        docker_repository: str,
         vault_endpoint: T.Optional[str] = None,
         vault_secret: T.Optional[str] = None,
         vault_endpoint_verify: str | bool | None = None,
 ):
     logger.info("Authenticating to registry with auth_method=%s", auth_method)
 
     if auth_method == AuthorizationType.LOCAL_ACCOUNT:
         bf_commons.run_process(['gcloud', 'auth', 'configure-docker'])
     elif auth_method == AuthorizationType.VAULT:
         oauthtoken = get_vault_token(vault_endpoint, vault_secret, vault_endpoint_verify)
+        docker_repository_host = docker_repository.split('/', 1)[0]
         bf_commons.run_process(
-            ['docker', 'login', '-u', 'oauth2accesstoken', '--password-stdin', 'https://eu.gcr.io'],
+            ['docker', 'login', '-u', 'oauth2accesstoken', '--password-stdin', f"https://{docker_repository_host}"],
             input=oauthtoken,
         )
     else:
         raise ValueError(f"unsupported auth_method: {auth_method!r}")
 
 
 def check_images_exist(
         images: T.Set[str],
         auth_method: AuthorizationType,
+        docker_repository: str,
         vault_endpoint: T.Optional[str] = None,
         vault_secret: T.Optional[str] = None,
         vault_endpoint_verify: str | bool | None = None
 ):
     logger.info("Checking if images used in DAGs exist in the registry")
-    authenticate_to_registry(auth_method, vault_endpoint, vault_secret, vault_endpoint_verify)
+    authenticate_to_registry(auth_method, docker_repository, vault_endpoint, vault_secret, vault_endpoint_verify)
     missing_images = set()
     for image in images:
         found_images = bf_commons.run_process(['docker', 'manifest', 'inspect', image], check=False, verbose=False)
         if not found_images:
             missing_images.add(image)
     if missing_images:
         raise ValueError(f"Some of the images used in dags do not exist, images: {missing_images}")
@@ -191,28 +196,30 @@
     return versions
 
 
 def deploy_dags_folder(
         dags_dir: str,
         dags_bucket: str,
         project_id: str,
+        docker_repository: str,
         clear_dags_folder: bool = False,
         auth_method: AuthorizationType = AuthorizationType.LOCAL_ACCOUNT,
         vault_endpoint: T.Optional[str] = None,
         vault_endpoint_verify: str | bool | None = None,
         vault_secret: T.Optional[str] = None,
         gs_client: T.Optional[storage.Client] = None,
 ) -> str:
     images = get_image_tags_from_image_version_file(dags_dir)
     if images:
         check_images_exist(auth_method=auth_method,
                            vault_endpoint=vault_endpoint,
                            vault_endpoint_verify=vault_endpoint_verify,
                            vault_secret=vault_secret,
-                           images=images)
+                           images=images,
+                           docker_repository=docker_repository,)
 
     logger.info("Deploying DAGs folder, auth_method=%s, clear_dags_folder=%s, dags_dir=%s", auth_method, clear_dags_folder, dags_dir)
 
     client = gs_client or create_storage_client(auth_method, project_id, vault_endpoint, vault_secret, vault_endpoint_verify)
     bucket = client.bucket(dags_bucket)
 
     if clear_dags_folder:
```

### Comparing `bigflow-1.8.0/bigflow/konfig.py` & `bigflow-1.9.0.dev1/bigflow/konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/migrate.py` & `bigflow-1.9.0.dev1/bigflow/migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/resources.py` & `bigflow-1.9.0.dev1/bigflow/resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/infra.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/infra.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/scaffold.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/README.txt` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/README.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/.gitignore.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/Dockerfile` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/Dockerfile`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/README.md` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/README.md`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/deployment_config.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/deployment_config.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/pi_estimator/test_processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/test/test_wordcount_workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/internationalports/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/processing.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/pi_estimator/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2` & `bigflow-1.9.0.dev1/bigflow/scaffold/templates/new-project/{{project_name}}/wordcount/workflow.py.j2`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/scaffold/templating.py` & `bigflow-1.9.0.dev1/bigflow/scaffold/templating.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/testing/isolate.py` & `bigflow-1.9.0.dev1/bigflow/testing/isolate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/version.py` & `bigflow-1.9.0.dev1/bigflow/version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow/workflow.py` & `bigflow-1.9.0.dev1/bigflow/workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow.egg-info/SOURCES.txt` & `bigflow-1.9.0.dev1/bigflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/bigflow.egg-info/requires.txt` & `bigflow-1.9.0.dev1/bigflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/setup.py` & `bigflow-1.9.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_dev.py` & `bigflow-1.9.0.dev1/test/buildd/test_dev.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_dist.py` & `bigflow-1.9.0.dev1/test/buildd/test_dist.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_operate.py` & `bigflow-1.9.0.dev1/test/buildd/test_operate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_pip.py` & `bigflow-1.9.0.dev1/test/buildd/test_pip.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_reflect.py` & `bigflow-1.9.0.dev1/test/buildd/test_reflect.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/buildd/test_spec.py` & `bigflow-1.9.0.dev1/test/buildd/test_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     __test__ = False
 
     expected_name: str
     expected_packages: List[str]
     expected_metainfo: Dict[str, Any]
 
     expected_requires: List[str] = [
-        "datetime_truncate==1.1.0",
+        "datetime-truncate==1.1.0",
         "six==1.15.0",
         "typing==3.7.4.3",
     ]
 
     def test_read_spec_from_setuppy(self):
 
         # when
```

### Comparing `bigflow-1.8.0/test/cli/test_cli.py` & `bigflow-1.9.0.dev1/test/cli/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -295,15 +295,16 @@
         '''
 from bigflow import Config
 
 deployment_config = Config(name='dev',
                            properties={
                                'gcp_project_id': 'my-gcp-project-id',
                                'dags_bucket': 'my-dags-bucket',
-                               'vault_secret': 'secret'
+                               'vault_secret': 'secret',
+                               'docker_repository': 'my-docker--repository'
                            })
         ''')
 
         # when
         cli(['deploy-dags'])
 
         # then
@@ -311,29 +312,31 @@
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             clear_dags_folder=False,
             dags_bucket='my-dags-bucket',
             dags_dir=self._expected_default_dags_dir(),
             project_id='my-gcp-project-id',
             vault_endpoint=None,
             vault_secret='secret',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
     @mock.patch('bigflow.deploy.deploy_dags_folder')
     def test_should_call_cli_deploy_dags_command_for_different_environments(self, deploy_dags_folder_mock):
         # given
         self._touch_file('deployment_config.py',
         '''
 from bigflow import Config
 
 deployment_config = Config(name='dev',
                           properties={
                               'gcp_project_id': 'my-gcp-dev-project-id',
                               'dags_bucket': 'my-dags-dev-bucket',
-                              'vault_secret': 'secret-dev'
+                              'vault_secret': 'secret-dev',
+                              'docker_repository': 'my-docker--repository'
                           })\
     .add_configuration(name='prod',
                           properties={
                               'gcp_project_id': 'my-gcp-prod-project-id',
                               'dags_bucket': 'my-dags-prod-bucket',
                               'vault_secret': 'secret-prod'
                           })
@@ -348,45 +351,48 @@
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             clear_dags_folder=False,
             dags_bucket='my-dags-dev-bucket',
             dags_dir=self._expected_default_dags_dir(),
             project_id='my-gcp-dev-project-id',
             vault_endpoint=None,
             vault_secret='secret-dev',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
         # when
         cli(['deploy-dags', '--config', 'dev'])
 
         # then
         deploy_dags_folder_mock.assert_called_with(
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             clear_dags_folder=False,
             dags_bucket='my-dags-dev-bucket',
             dags_dir=self._expected_default_dags_dir(),
             project_id='my-gcp-dev-project-id',
             vault_endpoint=None,
             vault_secret='secret-dev',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
         # when
         cli(['deploy-dags', '--config', 'prod'])
 
         # then
         deploy_dags_folder_mock.assert_called_with(
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             clear_dags_folder=False,
             dags_bucket='my-dags-prod-bucket',
             dags_dir=self._expected_default_dags_dir(),
             project_id='my-gcp-prod-project-id',
             vault_endpoint=None,
             vault_secret='secret-prod',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
     @mock.patch('bigflow.deploy.deploy_dags_folder')
     def test_should_call_cli_deploy_dags_command__when_parameters_are_given_by_explicit_deployment_config_file(self,
                                                                                                                deploy_dags_folder_mock):
         # given
         dc_file = self._touch_file('deployment_config_another.py',
@@ -394,15 +400,16 @@
 from bigflow import Config
 
 deployment_config = Config(name='dev',
                         properties={
                                'gcp_project_id': 'my-another-gcp-project-id',
                                'vault_endpoint': 'my-another-vault-endpoint',
                                'dags_bucket': 'my-another-dags-bucket',
-                               'vault_secret': 'secrett'
+                               'vault_secret': 'secrett',
+                               'docker_repository': 'my-docker--repository'
                         })
         ''')
 
         # when
         cli(['deploy-dags',
              '--deployment-config-path', dc_file.as_posix(),
              '--dags-dir', '/tmp/my-dags-dir',
@@ -414,41 +421,44 @@
             auth_method=AuthorizationType.VAULT,
             clear_dags_folder=False,
             dags_bucket='my-another-dags-bucket',
             dags_dir='/tmp/my-dags-dir',
             project_id='my-another-gcp-project-id',
             vault_endpoint='my-another-vault-endpoint',
             vault_secret='secrett',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
     @mock.patch('bigflow.deploy.deploy_dags_folder')
     def test_should_call_cli_deploy_dags_command__when_all_parameters_are_given_by_cli_arguments(self,
                                                                                                  deploy_dags_folder_mock):
         # when
         cli(['deploy-dags',
              '--dags-bucket', 'my-dags-bucket',
              '--dags-dir', '/tmp/my-dags-dir',
              '--vault-endpoint', 'my-vault-endpoint',
              '--gcp-project-id', 'my-gcp-project-id',
              '--auth-method', 'vault',
              '--clear-dags-folder',
-             '--vault-secret', 'secrett'
+             '--vault-secret', 'secrett',
+             '--docker-repository', 'my-docker--repository'
              ])
 
         # then
         deploy_dags_folder_mock.assert_called_with(
             auth_method=AuthorizationType.VAULT,
             clear_dags_folder=True,
             dags_bucket='my-dags-bucket',
             dags_dir='/tmp/my-dags-dir',
             project_id='my-gcp-project-id',
             vault_endpoint='my-vault-endpoint',
             vault_secret='secrett',
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
     @mock.patch('bigflow.deploy.deploy_docker_image')
     def test_should_call_cli_deploy_image_command__with_defaults_and_with_implicit_deployment_config_file(self,
                                                                                                           deploy_docker_image_mock):
         # given
         self._touch_file('deployment_config.py',
@@ -603,15 +613,16 @@
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             clear_dags_folder=False,
             dags_bucket='my-dags-bucket',
             dags_dir=self._expected_default_dags_dir(),
             project_id='my-gcp-project-id',
             vault_endpoint=None,
             vault_secret=None,
-            vault_endpoint_verify=True
+            vault_endpoint_verify=True,
+            docker_repository='my-docker--repository'
         )
 
         deploy_docker_image_mock.assert_called_with(
             auth_method=AuthorizationType.LOCAL_ACCOUNT,
             docker_repository='my-docker--repository',
             image_tar_path='my-images/image-version',
             vault_endpoint=None,
@@ -650,15 +661,16 @@
             auth_method=AuthorizationType.VAULT,
             clear_dags_folder=True,
             dags_bucket='my-dags-bucket',
             dags_dir='/tmp/my-dags-dir',
             project_id='my-gcp-project-id',
             vault_endpoint='my-vault-endpoint',
             vault_secret='secrett',
-            vault_endpoint_verify=expected_verify
+            vault_endpoint_verify=expected_verify,
+            docker_repository='my-docker-repository'
         )
 
         deploy_docker_image_mock.assert_called_with(
             auth_method=AuthorizationType.VAULT,
             docker_repository='my-docker-repository',
             image_tar_path='.image/imageinfo-123.toml',
             vault_endpoint='my-vault-endpoint',
```

### Comparing `bigflow-1.8.0/test/cli/test_module/Unused1.py` & `bigflow-1.9.0.dev1/test/cli/test_module/Unused1.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/dagbuilder/test_dagbuilder.py` & `bigflow-1.9.0.dev1/test/dagbuilder/test_dagbuilder.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from bigflow.bigquery.job import Job
 from bigflow.build.operate import create_image_version_file
 from bigflow.dagbuilder import get_dags_output_dir, clear_dags_output_dir, generate_dag_file
 from bigflow.workflow import WorkflowJob, Workflow, Definition, get_timezone_offset_seconds, hourly_start_time
 
 from test import mixins
 
+TEST_IMAGE_VERSION = '0.3.0'
+TEST_DOCKER_REPOSITORY = 'europe-west1-docker.pkg.dev/my_docker_repository_project/my-project'
+TEST_DOCKER_IMAGE = f'{TEST_DOCKER_REPOSITORY}:{TEST_IMAGE_VERSION}'
+
 
 class DagBuilderTestCase(mixins.TempCwdMixin, TestCase):
 
     def test_should_get_DAGs_output_dir(self):
 
         # when
         dags_dir = get_dags_output_dir(self.cwd / "subdir")
@@ -36,31 +40,27 @@
 
         # then
         self.assertFalse(f.exists())
 
     def test_should_generate_image_version_file(self):
         # given
         workdir = self.cwd
-        image = 'repository:version'
 
         # when
-        create_image_version_file(workdir, image)
+        create_image_version_file(workdir, TEST_DOCKER_IMAGE)
 
         # then
-        self.assertEqual((workdir / '.dags' / 'image_version.txt').read_text(), image)
+        self.assertEqual((workdir / '.dags' / 'image_version.txt').read_text(), TEST_DOCKER_IMAGE)
 
     @mock.patch('bigflow.workflow.get_timezone_offset_seconds')
     def test_should_generate_DAG_file_from_workflow_with_hourly_scheduling(self, get_timezone_offset_seconds_mock):
 
         # given
         workdir = self.cwd
         get_timezone_offset_seconds_mock.return_value = 2 * 3600
-        docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
-        version = '0.3.0'
-        image = f'{docker_repository}:{version}'
 
         # given
         job1 = Job(
             id='job1',
             component=mock.Mock(),
             retry_count=10,
             retry_pause_sec=20
@@ -87,29 +87,26 @@
         workflow = Workflow(
             workflow_id='my_workflow',
             definition=Definition(graph),
             start_time_factory=hourly_start_time,
             schedule_interval='@hourly')
 
         # when
-        dag_file_path = generate_dag_file(workdir, image, workflow, '2020-07-02 10:00:00', version, 'ca')
+        dag_file_path = generate_dag_file(workdir, TEST_DOCKER_IMAGE, workflow, '2020-07-02 10:00:00', TEST_IMAGE_VERSION, 'ca')
 
         # then
         self.assertEqual(dag_file_path, str(workdir / '.dags' / 'my_workflow__v0_3_0__2020_07_02_10_00_00_dag.py'))
 
         dag_file_content = Path(dag_file_path).read_text()
         expected_dag_content = (Path(__file__).parent / "my_workflow__dag.py.txt").read_text()
         self.assert_files_are_equal(expected_dag_content, dag_file_content)
 
     def test_should_pass_workflow_properties_to_airflow_dag(self):
         # given
         workdir = self.cwd
-        docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
-        version = '0.3.0'
-        image = f'{docker_repository}:{version}'
 
         # given
         job1 = Job(
             id='job1',
             component=mock.Mock(),
             retry_count=10,
             retry_pause_sec=20
@@ -122,29 +119,26 @@
             workflow_id='my_parametrized_workflow',
             definition=Definition(graph),
             depends_on_past=False,
             schedule_interval='@daily',
             secrets=['bf_secret_password', 'bf_secret_token'])
 
         # when
-        dag_file_path = generate_dag_file(workdir, image, workflow, '2020-07-02', version, 'ca')
+        dag_file_path = generate_dag_file(workdir, TEST_DOCKER_IMAGE, workflow, '2020-07-02', TEST_IMAGE_VERSION, 'ca')
 
         # then passes the depends_on_past parameter value
         self.assertEqual(dag_file_path, str(workdir / '.dags/my_parametrized_workflow__v0_3_0__2020_07_02_00_00_00_dag.py'))
 
         dag_file_content = Path(dag_file_path).read_text()
         expected_dag_content = (Path(__file__).parent / "my_parametrized_workflow__dag.py.txt").read_text()
         self.assert_files_are_equal(expected_dag_content, dag_file_content)
 
     def test_should_set_different_env_variable_name_for_dag(self):
         # given
         workdir = self.cwd
-        docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
-        version = '0.3.0'
-        image = f'{docker_repository}:{version}'
 
         # given
         job1 = Job(
             id='job1',
             component=mock.Mock(),
             retry_count=10,
             retry_pause_sec=20
@@ -159,29 +153,26 @@
             depends_on_past=False,
             schedule_interval='@daily',
             secrets=['bf_secret_password', 'bf_secret_token'],
             env_variable='prod_env',
         )
 
         # when
-        dag_file_path = generate_dag_file(workdir, image, workflow, '2020-07-02', version, 'ca')
+        dag_file_path = generate_dag_file(workdir, TEST_DOCKER_IMAGE, workflow, '2020-07-02', TEST_IMAGE_VERSION, 'ca')
 
         # then passes the depends_on_past parameter value
         self.assertEqual(dag_file_path, str(workdir / '.dags/my_parametrized_env_workflow__v0_3_0__2020_07_02_00_00_00_dag.py'))
 
         dag_file_content = Path(dag_file_path).read_text()
         expected_dag_content = (Path(__file__).parent / "my_parametrized_env_workflow__dag.py.txt").read_text()
         self.assert_files_are_equal(expected_dag_content, dag_file_content)
 
     def test_should_generate_DAG_file_from_workflow_with_daily_scheduling(self):
         # given
         workdir = self.cwd
-        docker_repository = 'eu.gcr.io/my_docker_repository_project/my-project'
-        version = '0.3.0'
-        image = f'{docker_repository}:{version}'
 
         # given
         job1 = Job(
             id='job1',
             component=mock.Mock(),
             retry_count=10,
             retry_pause_sec=20
@@ -192,15 +183,15 @@
         }
         workflow = Workflow(
             workflow_id='my_daily_workflow',
             definition=Definition(graph),
             schedule_interval='@daily')
 
         # when
-        dag_file_path = generate_dag_file(workdir, image, workflow, '2020-07-02', version, 'ca')
+        dag_file_path = generate_dag_file(workdir, TEST_DOCKER_IMAGE, workflow, '2020-07-02', TEST_IMAGE_VERSION, 'ca')
 
         # then
         self.assertEqual(dag_file_path, str(workdir / '.dags/my_daily_workflow__v0_3_0__2020_07_02_00_00_00_dag.py'))
 
         dag_file_content = Path(dag_file_path).read_text()
         expected_dag_content = (Path(__file__).parent / "my_daily_workflow__dag.py.txt").read_text()
         self.assert_files_are_equal(expected_dag_content, dag_file_content)
```

### Comparing `bigflow-1.8.0/test/test_commons.py` & `bigflow-1.9.0.dev1/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_configuration.py` & `bigflow-1.9.0.dev1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_dataflow.py` & `bigflow-1.9.0.dev1/test/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_deploy.py` & `bigflow-1.9.0.dev1/test/test_deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from test.mixins import TempCwdMixin, BaseTestCase
 
 TEST_VAULT_ENDPOINT = 'https://example.com/v1/gcp/token'
 TEST_VAULT_SECRET = 'secret'
 VAULT_TOKEN_HEADER = 'X-Vault-Token'
 TEST_VAULT_GET_HEADERS = {VAULT_TOKEN_HEADER: TEST_VAULT_SECRET}
+TEST_DOCKER_REPOSITORY = 'europe-west1-docker.pkg.dev/myproject/myrepository'
 
 
 class DeployTestCase(TempCwdMixin, BaseTestCase):
 
     @mock.patch('bigflow.deploy.check_images_exist')
     def test_should_clear_GCS_DAGs_folder(self, check_images_exist):
 
@@ -44,15 +45,15 @@
         dags_dir = os.path.join(self.cwd, '.dags')
         os.mkdir(dags_dir)
 
         # when
         with self.assertLogs(level='ERROR') as cm:
             deploy_dags_folder(dags_dir=dags_dir, dags_bucket='europe-west1-1-bucket', project_id='',
                                clear_dags_folder=True, auth_method=AuthorizationType.LOCAL_ACCOUNT,
-                               gs_client=gs_client_mock)
+                               gs_client=gs_client_mock, docker_repository=TEST_DOCKER_REPOSITORY)
             self.assertIn(
                 'ERROR:bigflow.deploy:The image_version.txt file not found, the image check '
                 'will not be performed. To perform the check regenerate DAG files with the '
                 'new version of BigFlow', cm.output)
 
         # then
         gs_client_mock.bucket.assert_called_with('europe-west1-1-bucket')
@@ -83,16 +84,22 @@
         f2 = dags_dir / 'zonk_2.txt'
         f2.touch()
 
         gs_client_mock.bucket.return_value = bucket_mock
         bucket_mock.blob.side_effect = blobs
 
         # when
-        deploy_dags_folder(dags_dir=os.path.join(self.cwd, '.dags'), dags_bucket='europe-west1-1-bucket', project_id='',
-                           clear_dags_folder=False, auth_method=AuthorizationType.LOCAL_ACCOUNT, gs_client=gs_client_mock)
+        deploy_dags_folder(
+            dags_dir=os.path.join(self.cwd, '.dags'),
+            dags_bucket='europe-west1-1-bucket',
+            project_id='',
+            clear_dags_folder=False,
+            auth_method=AuthorizationType.LOCAL_ACCOUNT,
+            gs_client=gs_client_mock,
+            docker_repository=TEST_DOCKER_REPOSITORY,)
 
         # then
         gs_client_mock.bucket.assert_called_with('europe-west1-1-bucket')
         f1_blob_mock.upload_from_filename.assert_called_with(f1.as_posix(), content_type='application/octet-stream')
         f2_blob_mock.upload_from_filename.assert_called_with(f2.as_posix(), content_type='application/octet-stream')
 
     @responses.activate
@@ -224,15 +231,15 @@
 
         # then
         load_image_from_tar.assert_called_with('image-version123.tar')
         remove_docker_image_from_local_registry.assert_called_with('docker_repository:version123')
 
     def test_should_parse_image_versions_from_files(self):
         # given
-        docker_repository = 'eu.gcr.io/project/name'
+        docker_repository = 'myregion-docker.pkg.dev/myproject/myrepository'
         version1 = '0.74.dev1-g4ef53366'
         version2 = '0.74'
         dags_path = Path(self.cwd, '.dags')
         dags_path.mkdir(exist_ok=True)
         with (dags_path / 'image_version.txt').open(mode='w') as f:
             for version in [version1, version2]:
                 f.write(f'{docker_repository}:{version}\n')
@@ -244,59 +251,66 @@
         self.assertEqual(tags, {f'{docker_repository}:{version1}', f'{docker_repository}:{version2}'})
 
     @mock.patch('bigflow.deploy.authenticate_to_registry')
     @mock.patch('bigflow.deploy.bf_commons.run_process', return_value='')
     def test_should_raise_error_when_image_doesnt_exist(self, authenticate_to_registry, run_process):
         with self.assertRaises(ValueError):
             check_images_exist(auth_method=AuthorizationType.LOCAL_ACCOUNT,
-                               images={f'eu.gcr.io/non-existing-project/name:some-version'})
+                               docker_repository=TEST_DOCKER_REPOSITORY,
+                               images={f'europe-west1-docker.pkg.dev/non-existing-project/name:some-version'},)
 
     @mock.patch('bigflow.deploy.authenticate_to_registry')
     @mock.patch('bigflow.commons.run_process', return_value='[{"name": "some_image"}]')
     def test_should_not_raise_error_if_the_image_exists(self, authenticate_to_registry, run_process):
         check_images_exist(auth_method=AuthorizationType.LOCAL_ACCOUNT,
-                           images={f'eu.gcr.io/non-existing-project/name:some-version'})
+                           docker_repository=TEST_DOCKER_REPOSITORY,
+                           images={f'europe-west1-docker.pkg.dev/non-existing-project/name:some-version'})
 
     @mock.patch('bigflow.deploy.authenticate_to_registry')
     @mock.patch('bigflow.deploy.upload_dags_folder')
     @mock.patch('bigflow.commons.run_process', return_value=None)
     def test_should_not_upload_dags_if_image_is_missing(self, authenticate_to_registry,
                                                         upload_dags_folder, run_process):
         # given
         gs_client = mock.Mock()
-        docker_repository = 'eu.gcr.io/project/name'
         version = '0.74.dev1-g4ef53366'
-        create_image_version_file(self.cwd, f'{docker_repository}:{version}')
+        create_image_version_file(self.cwd, f'{TEST_DOCKER_REPOSITORY}:{version}')
 
         # when/then
         with self.assertRaises(ValueError):
-            deploy_dags_folder(dags_dir=os.path.join(self.cwd, '.dags'), dags_bucket='europe-west1-1-bucket', project_id='',
-                               clear_dags_folder=False, auth_method=AuthorizationType.LOCAL_ACCOUNT, gs_client=gs_client)
+            deploy_dags_folder(
+                dags_dir=os.path.join(self.cwd, '.dags'),
+                dags_bucket='europe-west1-1-bucket',
+                project_id='',
+                clear_dags_folder=False,
+                auth_method=AuthorizationType.LOCAL_ACCOUNT,
+                gs_client=gs_client,
+                docker_repository=TEST_DOCKER_REPOSITORY)
 
         authenticate_to_registry.assert_called_once()
         gs_client.bucket.assert_not_called()
         upload_dags_folder.assert_not_called()
 
     def test_deploy_image_pushes_tags(self):
         # given
         authenticate_to_registry_mock = self.addMock(mock.patch('bigflow.deploy.authenticate_to_registry'))
         run_process_mock = self.addMock(mock.patch('bigflow.commons.run_process'))
 
         # when
         bf_deploy._deploy_image_loaded_to_local_registry(
             build_ver="1.2",
-            docker_repository="docker_repository",
+            docker_repository=TEST_DOCKER_REPOSITORY,
             image_id="image123",
             auth_method=AuthorizationType.VAULT,
             vault_endpoint=TEST_VAULT_ENDPOINT,
             vault_secret=TEST_VAULT_SECRET,
         )
 
         # then
         authenticate_to_registry_mock.assert_called_once_with(
-            AuthorizationType.VAULT, TEST_VAULT_ENDPOINT, TEST_VAULT_SECRET, None)
+            AuthorizationType.VAULT, TEST_DOCKER_REPOSITORY, TEST_VAULT_ENDPOINT, TEST_VAULT_SECRET, None)
 
         run_process_mock.assert_has_calls([
-            mock.call(["docker", "tag", "image123", "docker_repository:latest"]),
-            mock.call(["docker", "push", "docker_repository:1.2"]),
-            mock.call(["docker", "push", "docker_repository:latest"]),
+            mock.call(["docker", "tag", "image123", f"{TEST_DOCKER_REPOSITORY}:latest"]),
+            mock.call(["docker", "push", f"{TEST_DOCKER_REPOSITORY}:1.2"]),
+            mock.call(["docker", "push", f"{TEST_DOCKER_REPOSITORY}:latest"]),
         ])
```

### Comparing `bigflow-1.8.0/test/test_interactive.py` & `bigflow-1.9.0.dev1/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_job.py` & `bigflow-1.9.0.dev1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_konfig.py` & `bigflow-1.9.0.dev1/test/test_konfig.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_migrate.py` & `bigflow-1.9.0.dev1/test/test_migrate.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_resources.py` & `bigflow-1.9.0.dev1/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_scaffold.py` & `bigflow-1.9.0.dev1/test/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_user_commons/test_labels.py` & `bigflow-1.9.0.dev1/test/test_user_commons/test_labels.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_user_commons/test_sensor.py` & `bigflow-1.9.0.dev1/test/test_user_commons/test_sensor.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_version.py` & `bigflow-1.9.0.dev1/test/test_version.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/test_workflow.py` & `bigflow-1.9.0.dev1/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `bigflow-1.8.0/test/testing/test_isolate.py` & `bigflow-1.9.0.dev1/test/testing/test_isolate.py`

 * *Files identical despite different names*

