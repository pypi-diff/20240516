# Comparing `tmp/mlcvzoo_util-0.4.1.tar.gz` & `tmp/mlcvzoo_util-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_util-0.4.1.tar", max compression
+gzip compressed data, was "mlcvzoo_util-0.4.2.tar", last modified: Thu May 16 06:41:17 2024, max compression
```

## Comparing `mlcvzoo_util-0.4.1.tar` & `mlcvzoo_util-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,242 @@
--rw-r--r--   0        0        0    11412 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/LICENSE
--rw-r--r--   0        0        0      337 2024-02-19 09:48:32.049907 mlcvzoo_util-0.4.1/README.md
--rw-r--r--   0        0        0      244 2024-02-19 09:48:32.049907 mlcvzoo_util-0.4.1/mlcvzoo_util/__init__.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/__init__.py
--rw-r--r--   0        0        0     7348 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/configuration.py
--rw-r--r--   0        0        0     6110 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
--rw-r--r--   0        0        0     8392 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
--rw-r--r--   0        0        0     9831 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
--rw-r--r--   0        0        0     1123 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/utils.py
--rw-r--r--   0        0        0    12973 2024-02-19 09:48:32.049907 mlcvzoo_util-0.4.1/mlcvzoo_util/image_io_utils.py
--rw-r--r--   0        0        0      246 2024-02-07 12:51:46.803540 mlcvzoo_util-0.4.1/mlcvzoo_util/logger/__init__.py
--rw-r--r--   0        0        0     3923 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/logger/logger.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/ls_tracking_task_converter/__init__.py
--rw-r--r--   0        0        0    11102 2024-02-16 17:19:15.906701 mlcvzoo_util-0.4.1/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py
--rw-r--r--   0        0        0     4220 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/mlcvzoo_cli_tool.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/__init__.py
--rw-r--r--   0        0        0     3032 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/configuration.py
--rw-r--r--   0        0        0     8565 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/metric_factory.py
--rw-r--r--   0        0        0    16860 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/model_evaluator.py
--rw-r--r--   0        0        0      615 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/structs.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_timer/__init__.py
--rw-r--r--   0        0        0     1185 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_timer/configuration.py
--rw-r--r--   0        0        0     9776 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_timer/model_timer.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_trainer/__init__.py
--rw-r--r--   0        0        0      741 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_trainer/configuration.py
--rw-r--r--   0        0        0     6628 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/model_trainer/model_trainer.py
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/pre_annotation_tool/__init__.py
--rw-r--r--   0        0        0     1380 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/pre_annotation_tool/configuration.py
--rw-r--r--   0        0        0    12686 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
--rw-r--r--   0        0        0        0 2024-02-19 09:49:27.560027 mlcvzoo_util-0.4.1/mlcvzoo_util/py.typed
--rw-r--r--   0        0        0      196 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/video_image_creator/__init__.py
--rw-r--r--   0        0        0     1273 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/video_image_creator/configuration.py
--rw-r--r--   0        0        0    14452 2024-02-07 12:51:46.807541 mlcvzoo_util-0.4.1/mlcvzoo_util/video_image_creator/video_image_creator.py
--rw-r--r--   0        0        0     4230 2024-02-19 09:48:32.049907 mlcvzoo_util-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 mlcvzoo_util-0.4.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Implementation.md
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/issue_templates/Refactoring.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/.gitlab/merge_request_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/.gitlab/merge_request_templates/Default.md
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2240 2024-05-16 05:39:15.000000 mlcvzoo_util-0.4.2/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    11412 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2317 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     1584 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/config/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/config/templates/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.915985 mlcvzoo_util-0.4.2/config/templates/tools/cvat_annotation_handler/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/cvat_annotation_handler/cvat-client-config_template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/model-timer_config_template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/model-trainer_config_template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/config/templates/tools/video-image-creator_template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.919985 mlcvzoo_util-0.4.2/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/01_introduction_and_goals.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/02_architecture_constraints.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/03_system_scope_and_context.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/04_solution_strategy.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     1684 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/05_building_block_view.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/06_runtime_view.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/08_concepts.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/09_design_decisions.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/10_quality_scenarios.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/11_technical_risks.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/documentation/12_tutorial.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/about-arc42.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/glossary.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/documentation/index.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.919985 mlcvzoo_util-0.4.2/mlcvzoo_util/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8392 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9831 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/image_io_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11102 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4220 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/mlcvzoo_cli_tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.923985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     8565 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/metric_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    16735 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/model_evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     9776 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/model_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6628 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/model_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    12700 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:41:12.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.927985 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    28509 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_cvat_annotation_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_image_io_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    27110 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_evaluator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_model_trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6003 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_pre_annotation_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)    20745 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_tracking_task_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4754 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/tests/test_video_image_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)    14451 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/video_image_creator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2317 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9873 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 06:41:17.000000 mlcvzoo_util-0.4.2/mlcvzoo_util.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)   196676 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/poetry.lock
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/requirements_locked/
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/requirements_locked/requirements-lock-uv-py310-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/requirements_locked/requirements-lock-uv-py310-without-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 06:41:17.963986 mlcvzoo_util-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.931985 mlcvzoo_util-0.4.2/test_data/annotations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/coco/
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco.json
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco_alternate.json
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/coco/coco_evaluation.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-evaluation.csv
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-task_eval.csv
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/csv_annotations/test-task_train.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/cvat/
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat-for-clean-annotations.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3973 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat-for-images-annotations.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/cvat/cvat.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.935985 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/cars
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/person
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task/truck
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_class_mapping_not_found
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_forbidden_class
+-rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_no_json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_image_path
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/label_studio_s3/dummy_task_errors/error_wrong_label_studio_format
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/mot/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/custom_labels.txt
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_2015.txt
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_201617.txt
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_ground-truth_2020.txt
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/mot/mot_predictions_2020.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.907984 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 06:41:12.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/empty.xml
+-rw-rw-rw-   0 root         (0) root         (0)      716 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.939985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_clean_predictions/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/cars.xml
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/empty.xml
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/person.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_predictions/dummy_task/truck.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/3b09afbd59ed52a9b82a92856c0e2e82.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/636ae56768d7733bc65d1b1b543bfb4e.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1205 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/pascal_voc_read_from_file/dummy_task/6e443ec586208278605e6829dbdf94fd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/annotations/test_inference_task/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/test_inference_task/test_object-detection_inference_image.xml
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/annotations/text_recognition_test_label.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/checkpoints/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/checkpoints/model.pth
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/checkpoints/model_2.pth
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.911985 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class1/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class1/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class2/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class2/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class3/
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/classification_test_dataset/class3/black_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.943986 mlcvzoo_util-0.4.2/test_data/images/dummy_task/
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/cars.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/empty.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/person.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/dummy_task/truck.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/
+-rw-rw-rw-   0 root         (0) root         (0)  2270306 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/test_object-detection_inference_image.jpg
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/images/test_inference_task/test_text-recognition_inference_image.jpg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_coco.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    61627 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_imagenet.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      806 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_test-default-lp.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ClassMapping/class-mapping_test-default.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_coco_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_cvat_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      477 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal-voc_test_annotations_only.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_ReadFromFileObjectDetectionModel/read-from-file_pascal_voc_clean.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/cvat_password.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test-download-and-upload-task.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.951986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/mlcvzoo-test.zip
+-rw-rw-rw-   0 root         (0) root         (0)      762 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_download/test-download-task.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/mlcvzoo-test.zip
+-rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task-predictions.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task-predictions_only-create.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_cvat_annotation_handler/test_upload/test-upload-task.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test-checkpoint.pth
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_no_factory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_no_object_detection_model.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      953 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_tensorboard.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_all-checkpoint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      989 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_best-checkpoint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_wrong-checkpoint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_with_mlflow_wrong-model.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_evaluator/test_model_evaluator_without_mlflow.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_timer/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_timer/model_timer-read-from-file-with-mlfow-logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_timer/model_timer-read-from-file-without-mlfow-logging.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_model_trainer/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_model_trainer/test_model-trainer_config_read-from-file_coco_test.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.955986 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool_with_visualization.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_pre_annotation_tool/test_pre_annotation_tool_wrong_model.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations.json
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_empty.json
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_annotations.json
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_file_upload.json
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_labels.json
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_result.json
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_no_sequence.json
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_task_missing.json
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_wrong_annotation_format.json
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_tracking_task_converter/tracking_annotations_wrong_frame_count.json
+-rw-rw-rw-   0 root         (0) root         (0)     3999 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video.mp4
+-rw-rw-rw-   0 root         (0) root         (0)     3999 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_2.mp4
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_no-video-files.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_video-dir.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-05-13 11:00:17.000000 mlcvzoo_util-0.4.2/test_data/test_video_image_creator/test_video-image-creator_video-path.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 06:41:17.959986 mlcvzoo_util-0.4.2/third-party-licenses/
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-13 18:45:11.000000 mlcvzoo_util-0.4.2/third-party-licenses/third-party-licenses-complementary.csv
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2024-05-14 14:07:26.000000 mlcvzoo_util-0.4.2/third-party-licenses/third-party-licenses.csv
```

### Comparing `mlcvzoo_util-0.4.1/LICENSE` & `mlcvzoo_util-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/cvat_annotation_handler/utils.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/cvat_annotation_handler/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/image_io_utils.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/image_io_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/logger/logger.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/logger/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,13 +111,13 @@
 
         Returns:
             The matched logging level
         """
         if log_level is None:
             return logging.INFO
 
-        _log_level = logging.getLevelName(log_level)
+        _log_level: Union[str, int] = logging.getLevelName(log_level)
 
         if isinstance(_log_level, str) and "Level " in _log_level:
             return logging.INFO
 
         return _log_level
```

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/ls_tracking_task_converter/ls_tracking_task_converter.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/mlcvzoo_cli_tool.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/mlcvzoo_cli_tool.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/metric_factory.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/metric_factory.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/model_evaluator.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/model_evaluator.py`

 * *Files 10% similar despite different names*

```diff
@@ -250,44 +250,43 @@
         evaluated_checkpoint_metrics: Dict[str, EvaluationMetricType] = {}
         if checkpoint_paths:
             for ckpt in checkpoint_paths:
                 ModelEvaluator._restore_checkpoint(
                     checkpoint_path=ckpt, model=inference_model
                 )
 
-                evaluated_checkpoint_metrics[ckpt] = metric_factory.compute_metrics(  # type: ignore[assignment]
-                    inference_model=inference_model,  # type: ignore[arg-type]
+                evaluated_checkpoint_metrics[ckpt] = metric_factory.compute_metrics(
+                    inference_model=inference_model,
                     gt_annotations=gt_annotations,
                     model_evaluator_config=model_evaluator_config,
                 )
 
                 self._post_evaluation_step(
                     checkpoint_path=ckpt,
                     evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,
                     inference_model=inference_model,
                 )
         else:
             # TODO: Use interface method for getting the checkpoint-path of the model
-            evaluated_checkpoint_metrics[
-                MetricFactory.MODEL_STATE_INDICATOR
-            ] = metric_factory.compute_metrics(
-                # type: ignore[assignment]
-                inference_model=inference_model,  # type: ignore[arg-type]
-                gt_annotations=gt_annotations,
-                model_evaluator_config=model_evaluator_config,
+            evaluated_checkpoint_metrics[MetricFactory.MODEL_STATE_INDICATOR] = (
+                metric_factory.compute_metrics(
+                    inference_model=inference_model,
+                    gt_annotations=gt_annotations,
+                    model_evaluator_config=model_evaluator_config,
+                )
             )
 
             self._post_evaluation_step(
                 checkpoint_path=MetricFactory.MODEL_STATE_INDICATOR,
                 evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,
                 inference_model=inference_model,
             )
 
         best_checkpoint_info = metric_factory.determine_best_checkpoint(
-            evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,  # type: ignore[arg-type]
+            evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,
         )
 
         logger.info(
             "Evaluation finished, best checkpoint:\n" "\t- ckpt='%s'\n" "\t- ap='%s'\n",
             best_checkpoint_info.path,
             best_checkpoint_info.score,
         )
@@ -302,19 +301,21 @@
                     model_evaluator_config.mlflow_config.checkpoint_log_mode
                 )
             else:
                 checkpoint_log_mode = CheckpointLoggingModes.BEST.value
 
             metric_factory.log_results(
                 checkpoint_log_mode=checkpoint_log_mode,
-                evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,  # type: ignore[arg-type]
+                evaluated_checkpoint_metrics=evaluated_checkpoint_metrics,
                 best_checkpoint=best_checkpoint_info,
-                logging_configs=[model_evaluator_config.tensorboard_logging_config]
-                if model_evaluator_config.tensorboard_logging_config
-                else [],
+                logging_configs=(
+                    [model_evaluator_config.tensorboard_logging_config]
+                    if model_evaluator_config.tensorboard_logging_config
+                    else []
+                ),
             )
             if model_evaluator_config.mlflow_config is not None:
                 mlflow.end_run()
 
         return evaluated_checkpoint_metrics, best_checkpoint_info
 
     @staticmethod
@@ -368,19 +369,19 @@
     if not isinstance(model, Classifiable) or not isinstance(model, Model):
         raise ValueError(
             "This evaluation can only be used with models that "
             "inherit from 'mlcvzoo.api.model.Model' and 'mlcvzoo.api.interfaces.Classifiable"
         )
 
     assert isinstance(model, Classifiable) and isinstance(model, Model)
-    gt_annotations: List[
-        BaseAnnotation
-    ] = ModelEvaluator.generate_evaluation_annotations(
-        annotation_handler_config=configuration.annotation_handler_config,
-        mapper=model.mapper,
+    gt_annotations: List[BaseAnnotation] = (
+        ModelEvaluator.generate_evaluation_annotations(
+            annotation_handler_config=configuration.annotation_handler_config,
+            mapper=model.mapper,
+        )
     )
 
     checkpoint_paths: Optional[List[str]]
 
     if single_mode:
         checkpoint_paths = __get_model_checkpoint(model=model)
     else:
@@ -390,15 +391,15 @@
 
     if checkpoint_paths is None:
         logger.warning(
             "Could not determine any model checkpoints, therefore model"
             "will be used as is for the evaluation"
         )
 
-    return ModelEvaluator().evaluate_checkpoints(  # type: ignore[return-value]
+    return ModelEvaluator().evaluate_checkpoints(
         model_evaluator_config=configuration,
         inference_model=model,  # type: ignore[arg-type]
         gt_annotations=gt_annotations,
         checkpoint_paths=checkpoint_paths,
         log_results=True,
     )
```

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_evaluator/structs.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_evaluator/structs.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_timer/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_timer/model_timer.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_timer/model_timer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_trainer/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/model_trainer/model_trainer.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/model_trainer/model_trainer.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/pre_annotation_tool/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,19 +201,19 @@
         Generate PASCAL-VOC annotations using the configured model and
         store these annotations at the configured location
 
         Returns:
             None
         """
 
-        object_detection_model: ObjectDetectionModel[
-            Any, Any
-        ] = PreAnnotationTool.create_model(
-            model_config=self.configuration.model_config,
-            string_replacement_map=self.configuration.string_replacement_map,
+        object_detection_model: ObjectDetectionModel[Any, Any] = (
+            PreAnnotationTool.create_model(
+                model_config=self.configuration.model_config,
+                string_replacement_map=self.configuration.string_replacement_map,
+            )
         )
 
         image_paths: List[str] = self.__gather_image_paths()
 
         process_bar = tqdm(image_paths, desc="Generate predictions")
 
         if self.configuration.show_predictions:
```

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/video_image_creator/configuration.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_util-0.4.1/mlcvzoo_util/video_image_creator/video_image_creator.py` & `mlcvzoo_util-0.4.2/mlcvzoo_util/video_image_creator/video_image_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from mlcvzoo_util.mlcvzoo_cli_tool import MLCVZooCLITool
 from mlcvzoo_util.video_image_creator.configuration import VideoImageCreatorConfig
 
 logger = logging.getLogger(__name__)
 
 
 class VideoImageCreator(MLCVZooCLITool[VideoImageCreatorConfig]):
-
     """
     Tool to step through video and manually sort out frames to use as training data.
     When executed, displays every frame in given video separately. User is able to
     execute following commands:
     - Exit: 'q', 'Q', 'Esc'
     - Save current frame as .jpg: 's'
     - Change step size: '1' for 1 step, '2' for step, ...
```

### Comparing `mlcvzoo_util-0.4.1/pyproject.toml` & `mlcvzoo_util-0.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,90 @@
-[tool.poetry]
+[project]
 name = "mlcvzoo_util"
 description = "MLCVZoo Util Package"
-version = "0.4.1"
-license = "Open Logistics Foundation License v1.3"
+dynamic = ["version"]
+license = { text = "Open Logistics Foundation License 1.3" }
 readme = "README.md"
-homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util"
-repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util"
-documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
 ]
 authors = [
-    "Maximilian Otten <maximilian.otten@iml.fraunhofer.de>",
-    "Christian Hoppe <christian.hoppe@iml.fraunhofer.de>",
-    "Oliver Bredtmann <oliver.bredtmann@dbschenker.com>",
-    "Thilo Bauer <thilo.bauer@dbschenker.com>",
-    "Oliver Urbann <oliver.urbann@iml.fraunhofer.de>",
-    "Jan Basrawi <jan.basrawi@dbschenker.com>",
-    "Luise Weickhmann <luise.weickhmann@iml.fraunhofer.de>",
-    "Luca Kotulla <luca.kotulla@iml.fraunhofer.de>",
+    {name = "Maximilian Otten, email =  <maximilian.otten@iml.fraunhofer.de>"},
+    {name = "Christian Hoppe, email =  <christian.hoppe@iml.fraunhofer.de>"},
+    {name = "Oliver Bredtmann, email =  <oliver.bredtmann@dbschenker.com>"},
+    {name = "Thilo Bauer, email =  <thilo.bauer@dbschenker.com>"},
+    {name = "Oliver Urbann, email =  <oliver.urbann@iml.fraunhofer.de>"},
+    {name = "Jan Basrawi, email =  <jan.basrawi@dbschenker.com>"},
+    {name = "Luise Weickhmann, email =  <luise.weickhmann@iml.fraunhofer.de>"},
+    {name = "Luca Kotulla, email =  <luca.kotulla@iml.fraunhofer.de>"},
 ]
 
-exclude = ["mlcvzoo_util/tests/**/*"]
+requires-python = ">=3.8,<4.0"
+
+dependencies = [
+      "yaml-config-builder>=8.0, <9.0",
+      "related-mltoolbox>=1.0, <2.0",
+      "mlcvzoo_base>=5.0, <6.0",
+      "numpy>=1.19.2,!=1.19.5",
+      "opencv-python>=4.5,!=4.5.5.64",
+      "opencv-contrib-python>=4.5,!=4.5.5.64",
+      "tqdm>=4.61",
+      "imageio>=2.9",
+      "mlflow>=1.22"
+]
 
-packages = [
-    { include = "mlcvzoo_util" },
+[project.optional-dependencies]
+dev = [
+        "mock>=4.0",
+        "pytest>=7.0",
+        "pytest-cov>=3.0.0",
+        "black>=22",
+        "mypy>=0.961",
+        "pylint>=2.9.6",
+        "isort>=5.0",
+        "pytest-mock>=3.7",
+        "parametrize>=0.1.1"
 ]
 
-[tool.poetry.scripts]
+[project.scripts]
 mlcvzoo-cvat-handler = "mlcvzoo_util.cvat_annotation_handler.cvat_annotation_handler:main"
 mlcvzoo-preannotator = "mlcvzoo_util.pre_annotation_tool.pre_annotation_tool:main"
 mlcvzoo-modeltimer = "mlcvzoo_util.model_timer.model_timer:main"
 mlcvzoo-modelevaluator = "mlcvzoo_util.model_evaluator.model_evaluator:main"
 mlcvzoo-modeltrainer = "mlcvzoo_util.model_trainer.model_trainer:main"
 mlcvzoo-video-image-creator = "mlcvzoo_util.video_image_creator.video_image_creator:main"
 mlcvzoo-tracking-task-converter = "mlcvzoo_util.tracking_task_converter.tracking_task_converter:main"
 
+[project.urls]
+homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util"
+repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util"
+documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util/-/blob/main/documentation/index.adoc"
 
-[tool.poetry.dependencies]
-python = "^3.8"
+[tool.setuptools.dynamic]
+version = {attr = "mlcvzoo_util.__version__"}
 
-yaml-config-builder = { version = "^8.0" }
-related-mltoolbox = { version = "^1.0" }
-mlcvzoo_base = { version = "^5.0" }
-
-# 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
-numpy = { version = ">=1.19.2,!=1.19.5" }
-opencv-python = { version = ">=4.5,!=4.5.5.64"}
-opencv-contrib-python = { version = ">=4.5,!=4.5.5.64" }
-tqdm = { version = ">=4.61" }
-imageio = { version = ">=2.9" }
-mlflow = { version = ">=1.22" }
-
-[tool.poetry.dev-dependencies]
-mock = { version = ">=4.0" }
-pytest = { version = ">=7.0" }
-pytest-cov = { version = ">=3.0.0" }
-black = { version = ">=22" }
-mypy = { version = ">=0.961" }
-pylint = { version = ">=2.9.6" }
-# Isort guarantees formatting results for 5.X
-isort = { version = "^5.0" }
-pytest-mock = { version = ">=3.7" }
-parametrize = { version = ">=0.1.1" }
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+where = ["."]  # list of folders that contain the packages (["."] by default)
+include = ["mlcvzoo_utile*"]  # package names should match these glob patterns (["*"] by default)
+exclude = ["mlcvzoo_util.tests*"]  # exclude packages matching these glob patterns (empty by default)
+namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
-requires = ["setuptools", "poetry_core>=1.0"]
-build-backend = "poetry.core.masonry.api"
+requires = [
+    "setuptools>=42",
+    "wheel",
+    "setuptools_scm[toml]>=3.4"
+]
+build-backend = "setuptools.build_meta"
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.master]
 extension-pkg-whitelist = ["numpy", "cv2"]
 ignore=["third_party"]
```

### Comparing `mlcvzoo_util-0.4.1/PKG-INFO` & `mlcvzoo_util-0.4.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
-Name: mlcvzoo-util
-Version: 0.4.1
+Name: mlcvzoo_util
+Version: 0.4.2
 Summary: MLCVZoo Util Package
-Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
-License: Open Logistics Foundation License v1.3
-Author: Maximilian Otten
-Author-email: maximilian.otten@iml.fraunhofer.de
-Requires-Python: >=3.8,<4.0
+Author: Maximilian Otten, email =  <maximilian.otten@iml.fraunhofer.de>, Christian Hoppe, email =  <christian.hoppe@iml.fraunhofer.de>, Oliver Bredtmann, email =  <oliver.bredtmann@dbschenker.com>, Thilo Bauer, email =  <thilo.bauer@dbschenker.com>, Oliver Urbann, email =  <oliver.urbann@iml.fraunhofer.de>, Jan Basrawi, email =  <jan.basrawi@dbschenker.com>, Luise Weickhmann, email =  <luise.weickhmann@iml.fraunhofer.de>, Luca Kotulla, email =  <luca.kotulla@iml.fraunhofer.de>
+License: Open Logistics Foundation License 1.3
+Project-URL: homepage, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
+Project-URL: repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
+Project-URL: documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util/-/blob/main/documentation/index.adoc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: imageio (>=2.9)
-Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
-Requires-Dist: mlflow (>=1.22)
-Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64)
-Requires-Dist: opencv-python (>=4.5,!=4.5.5.64)
-Requires-Dist: related-mltoolbox (>=1.0,<2.0)
-Requires-Dist: tqdm (>=4.61)
-Requires-Dist: yaml-config-builder (>=8.0,<9.0)
-Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util/-/blob/main/documentation/index.adoc
-Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-util
+Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: yaml-config-builder<9.0,>=8.0
+Requires-Dist: related-mltoolbox<2.0,>=1.0
+Requires-Dist: mlcvzoo_base<6.0,>=5.0
+Requires-Dist: numpy!=1.19.5,>=1.19.2
+Requires-Dist: opencv-python!=4.5.5.64,>=4.5
+Requires-Dist: opencv-contrib-python!=4.5.5.64,>=4.5
+Requires-Dist: tqdm>=4.61
+Requires-Dist: imageio>=2.9
+Requires-Dist: mlflow>=1.22
+Provides-Extra: dev
+Requires-Dist: mock>=4.0; extra == "dev"
+Requires-Dist: pytest>=7.0; extra == "dev"
+Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
+Requires-Dist: black>=22; extra == "dev"
+Requires-Dist: mypy>=0.961; extra == "dev"
+Requires-Dist: pylint>=2.9.6; extra == "dev"
+Requires-Dist: isort>=5.0; extra == "dev"
+Requires-Dist: pytest-mock>=3.7; extra == "dev"
+Requires-Dist: parametrize>=0.1.1; extra == "dev"
 
 # MLCVZoo Util
 
 The MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)
 computer vision algorithms. The package **mlcvzoo_util** provides additional utility functions for downstream developments and tools for convenience and CLI usage.
 
 ## Install
 `
 pip install mlcvzoo-util
 `
 
 ## Technology stack
 
 - Python
-
```

