# Comparing `tmp/b2luigi-0.9.1.tar.gz` & `tmp/b2luigi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2luigi-0.9.1.tar", last modified: Wed Mar 29 22:14:16 2023, max compression
+gzip compressed data, was "b2luigi-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `b2luigi-0.9.1.tar` & `b2luigi-1.0.0.tar`

### file list

```diff
@@ -1,105 +1,102 @@
--rw-r--r--   0        0        0      136 2023-03-29 22:11:46.367240 b2luigi-0.9.1/.bumpversion.cfg
--rw-r--r--   0        0        0      168 2022-04-05 19:08:00.604171 b2luigi-0.9.1/.github/labeler.yml
--rw-r--r--   0        0        0      606 2021-04-19 15:35:29.820283 b2luigi-0.9.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      229 2022-04-05 19:08:00.604171 b2luigi-0.9.1/.github/workflows/pr.yml
--rw-r--r--   0        0        0     1539 2021-04-19 15:35:29.823616 b2luigi-0.9.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1233 2020-05-12 18:06:28.503934 b2luigi-0.9.1/.gitignore
--rw-r--r--   0        0        0      477 2023-01-13 18:37:12.195881 b2luigi-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       51 2020-02-06 08:03:49.471804 b2luigi-0.9.1/.readthedocs.yml
--rw-r--r--   0        0        0    19777 2023-03-29 22:11:46.370573 b2luigi-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     3358 2020-02-06 08:03:49.471804 b2luigi-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       91 2020-02-06 08:03:49.471804 b2luigi-0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    32422 2020-02-06 08:03:49.475137 b2luigi-0.9.1/LICENSE
--rw-r--r--   0        0        0     1858 2021-11-16 14:01:26.170412 b2luigi-0.9.1/README.rst
--rw-r--r--   0        0        0     5859 2023-03-29 22:11:46.370573 b2luigi-0.9.1/b2luigi/__init__.py
--rw-r--r--   0        0        0      242 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/__init__.py
--rw-r--r--   0        0        0     6754 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/data.py
--rw-r--r--   0        0        0      282 2021-04-19 15:35:29.823616 b2luigi-0.9.1/b2luigi/basf2_helper/targets.py
--rw-r--r--   0        0        0     3627 2021-09-15 12:07:31.577226 b2luigi-0.9.1/b2luigi/basf2_helper/tasks.py
--rw-r--r--   0        0        0      377 2021-04-19 15:35:29.826950 b2luigi-0.9.1/b2luigi/basf2_helper/utils.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/batch/__init__.py
--rw-r--r--   0        0        0     1110 2022-01-08 01:24:00.082163 b2luigi-0.9.1/b2luigi/batch/cache.py
--rw-r--r--   0        0        0     7470 2021-04-19 15:35:29.826950 b2luigi-0.9.1/b2luigi/batch/processes/__init__.py
--rw-r--r--   0        0        0    64579 2023-03-29 17:06:46.273750 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2.py
--rwxr-xr-x   0        0        0      968 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py
--rwxr-xr-x   0        0        0     2593 2022-11-14 11:09:44.556064 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py
--rwxr-xr-x   0        0        0     1061 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py
--rw-r--r--   0        0        0     1431 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py
--rw-r--r--   0        0        0    11061 2022-08-25 15:07:10.097728 b2luigi-0.9.1/b2luigi/batch/processes/htcondor.py
--rw-r--r--   0        0        0     3649 2021-04-19 15:35:29.830283 b2luigi-0.9.1/b2luigi/batch/processes/lsf.py
--rwxr-xr-x   0        0        0     1540 2022-10-07 15:37:00.857191 b2luigi-0.9.1/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2
--rw-r--r--   0        0        0     1347 2021-04-19 15:35:29.830283 b2luigi-0.9.1/b2luigi/batch/processes/test.py
--rw-r--r--   0        0        0     1684 2023-03-17 14:41:39.044701 b2luigi-0.9.1/b2luigi/batch/workers.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/cli/__init__.py
--rw-r--r--   0        0        0     2515 2021-11-16 14:01:26.173745 b2luigi-0.9.1/b2luigi/cli/arguments.py
--rw-r--r--   0        0        0     4310 2021-04-19 15:35:29.833616 b2luigi-0.9.1/b2luigi/cli/process.py
--rw-r--r--   0        0        0     3888 2021-04-19 15:35:29.833616 b2luigi-0.9.1/b2luigi/cli/runner.py
--rw-r--r--   0        0        0        0 2020-02-06 08:03:49.475137 b2luigi-0.9.1/b2luigi/core/__init__.py
--rw-r--r--   0        0        0     3041 2021-11-23 15:40:39.312670 b2luigi-0.9.1/b2luigi/core/dispatchable_task.py
--rw-r--r--   0        0        0     3636 2021-04-19 15:35:29.836950 b2luigi-0.9.1/b2luigi/core/executable.py
--rw-r--r--   0        0        0     1939 2023-03-29 15:56:55.436388 b2luigi-0.9.1/b2luigi/core/parameter.py
--rw-r--r--   0        0        0     5338 2021-04-19 15:35:29.836950 b2luigi-0.9.1/b2luigi/core/settings.py
--rw-r--r--   0        0        0     8924 2021-07-14 19:39:19.067382 b2luigi-0.9.1/b2luigi/core/task.py
--rw-r--r--   0        0        0     3178 2021-11-18 14:40:16.375973 b2luigi-0.9.1/b2luigi/core/temporary_wrapper.py
--rw-r--r--   0        0        0    11487 2023-03-20 13:02:23.915837 b2luigi-0.9.1/b2luigi/core/utils.py
--rw-r--r--   0        0        0      605 2021-04-19 15:35:29.836950 b2luigi-0.9.1/docs/Makefile
--rw-r--r--   0        0        0     5417 2021-08-03 10:35:07.243570 b2luigi-0.9.1/docs/advanced/basf2-examples.rst
--rw-r--r--   0        0        0     4278 2022-11-14 11:16:46.018025 b2luigi-0.9.1/docs/advanced/development.rst
--rw-r--r--   0        0        0     4248 2021-04-19 15:35:29.840283 b2luigi-0.9.1/docs/advanced/faq.rst
--rw-r--r--   0        0        0     5130 2023-03-29 22:11:46.370573 b2luigi-0.9.1/docs/conf.py
--rw-r--r--   0        0        0     2526 2021-04-19 15:35:29.840283 b2luigi-0.9.1/docs/documentation/api.rst
--rw-r--r--   0        0        0      751 2021-03-26 16:18:36.506513 b2luigi-0.9.1/docs/documentation/b2luigi.basf2_helper.rst
--rw-r--r--   0        0        0     3528 2021-07-14 12:29:39.595620 b2luigi-0.9.1/docs/documentation/run_modes.rst
--rw-r--r--   0        0        0     6114 2023-03-20 13:02:23.919170 b2luigi-0.9.1/docs/index.rst
--rw-r--r--   0        0        0     6275 2020-05-27 12:08:37.450453 b2luigi-0.9.1/docs/usage/batch.rst
--rw-r--r--   0        0        0     2114 2021-11-16 14:01:26.173745 b2luigi-0.9.1/docs/usage/installation.rst
--rw-r--r--   0        0        0     7852 2021-11-23 15:40:39.312670 b2luigi-0.9.1/docs/usage/quickstart.rst
--rw-r--r--   0        0        0     4453 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/basf2/basf2_chain_example.py
--rw-r--r--   0        0        0     2620 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/example_mdst_analysis.py
--rw-r--r--   0        0        0     2193 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/gbasf2_example.py
--rw-r--r--   0        0        0      133 2022-10-07 15:37:00.857191 b2luigi-0.9.1/examples/gbasf2/settings.json
--rw-r--r--   0        0        0     1466 2021-11-23 15:40:39.312670 b2luigi-0.9.1/examples/htcondor/htcondor_example.py
--rw-r--r--   0        0        0      182 2021-11-23 16:24:47.181004 b2luigi-0.9.1/examples/htcondor/settings.json
--rw-r--r--   0        0        0       50 2021-11-03 15:23:14.408281 b2luigi-0.9.1/examples/htcondor/setup_script.sh
--rw-r--r--   0        0        0      442 2022-08-25 15:07:10.097728 b2luigi-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      392 2021-04-19 15:35:29.846949 b2luigi-0.9.1/setup.cfg
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.106721 b2luigi-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/__init__.py
--rw-r--r--   0        0        0    17959 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json
--rw-r--r--   0        0        0    17971 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json
--rw-r--r--   0        0        0     5690 2021-10-20 18:18:44.110055 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json
--rw-r--r--   0        0        0   164412 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json
--rw-r--r--   0        0        0      858 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/batch_task_1.py
--rw-r--r--   0        0        0      782 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/batch_task_2.py
--rw-r--r--   0        0        0      880 2021-10-20 18:18:44.113388 b2luigi-0.9.1/tests/batch/test_batch_process.py
--rw-r--r--   0        0        0    18499 2023-03-20 14:18:09.989608 b2luigi-0.9.1/tests/batch/test_gbasf2_helper_functions.py
--rw-r--r--   0        0        0    10865 2023-03-20 14:18:09.989608 b2luigi-0.9.1/tests/batch/test_gbasf2_process.py
--rw-r--r--   0        0        0     5689 2022-01-08 01:24:00.085497 b2luigi-0.9.1/tests/batch/test_htcondor_processs.py
--rw-r--r--   0        0        0        0 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     1397 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/process_with_user_args_ignored_by_b2luigi.py
--rw-r--r--   0        0        0      562 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py
--rw-r--r--   0        0        0     1003 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/cli/test_ignore_additional_command_line_args.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/__init__.py
--rw-r--r--   0        0        0      662 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_1.py
--rw-r--r--   0        0        0      668 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_2.py
--rw-r--r--   0        0        0      602 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/dispatch_with_env_and_script.py
--rw-r--r--   0        0        0      368 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/folder_structures.py
--rw-r--r--   0        0        0      350 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/temporary_task_1.py
--rw-r--r--   0        0        0      319 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/temporary_task_2.py
--rw-r--r--   0        0        0     1750 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/test_dispatch_task.py
--rw-r--r--   0        0        0      824 2021-10-20 18:18:44.116721 b2luigi-0.9.1/tests/core/test_folder_structures.py
--rw-r--r--   0        0        0     2168 2023-03-29 15:56:55.446388 b2luigi-0.9.1/tests/core/test_parameter.py
--rw-r--r--   0        0        0     3984 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_requires.py
--rw-r--r--   0        0        0     3079 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_settings.py
--rw-r--r--   0        0        0     3493 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_task.py
--rw-r--r--   0        0        0      930 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/core/test_temporary_files.py
--rw-r--r--   0        0        0     9422 2023-03-20 13:02:23.919170 b2luigi-0.9.1/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/__init__.py
--rw-r--r--   0        0        0     1876 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/dict_requirement_example.py
--rw-r--r--   0        0        0       29 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/settings.json
--rw-r--r--   0        0        0      547 2021-10-20 18:18:44.120055 b2luigi-0.9.1/tests/doc_examples/simple_example.py
--rw-r--r--   0        0        0      547 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi.py
--rw-r--r--   0        0        0     1149 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi_2.py
--rw-r--r--   0        0        0      482 2021-10-20 18:18:44.123388 b2luigi-0.9.1/tests/doc_examples/test_examples.py
--rw-r--r--   0        0        0      906 2021-11-16 14:01:26.173745 b2luigi-0.9.1/tests/helpers.py
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 b2luigi-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      129 2024-03-22 10:06:22.765548 b2luigi-1.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1233 2024-03-22 10:06:22.765548 b2luigi-1.0.0/.gitignore
+-rw-r--r--   0        0        0     2356 2024-03-22 10:06:22.765548 b2luigi-1.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      585 2024-03-22 10:06:22.765548 b2luigi-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       51 2024-03-22 10:06:22.765548 b2luigi-1.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0      813 2024-03-22 10:06:22.765548 b2luigi-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    32422 2024-03-22 10:06:22.765548 b2luigi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1791 2024-03-22 10:06:22.765548 b2luigi-1.0.0/README.rst
+-rw-r--r--   0        0        0     5815 2024-03-22 10:06:22.765548 b2luigi-1.0.0/b2luigi/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-22 10:06:22.765548 b2luigi-1.0.0/b2luigi/basf2_helper/__init__.py
+-rw-r--r--   0        0        0     6616 2024-03-22 10:06:22.765548 b2luigi-1.0.0/b2luigi/basf2_helper/data.py
+-rw-r--r--   0        0        0      283 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/basf2_helper/targets.py
+-rw-r--r--   0        0        0     3566 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/basf2_helper/tasks.py
+-rw-r--r--   0        0        0      767 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/basf2_helper/utils.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.837550 b2luigi-1.0.0/b2luigi/batch/__init__.py
+-rw-r--r--   0        0        0     1111 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/cache.py
+-rw-r--r--   0        0        0     7557 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/__init__.py
+-rw-r--r--   0        0        0    66483 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/gbasf2.py
+-rwxr-xr-x   0        0        0     1041 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py
+-rwxr-xr-x   0        0        0     3033 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py
+-rwxr-xr-x   0        0        0     1156 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py
+-rw-r--r--   0        0        0     1479 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py
+-rw-r--r--   0        0        0    11226 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/htcondor.py
+-rw-r--r--   0        0        0     3653 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/lsf.py
+-rwxr-xr-x   0        0        0     1889 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2
+-rw-r--r--   0        0        0     1352 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/processes/test.py
+-rw-r--r--   0        0        0     1714 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/batch/workers.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.837550 b2luigi-1.0.0/b2luigi/cli/__init__.py
+-rw-r--r--   0        0        0     2308 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/cli/arguments.py
+-rw-r--r--   0        0        0     4276 2024-03-22 10:06:22.769548 b2luigi-1.0.0/b2luigi/cli/process.py
+-rw-r--r--   0        0        0     3901 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/cli/runner.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.837550 b2luigi-1.0.0/b2luigi/core/__init__.py
+-rw-r--r--   0        0        0     3064 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/dispatchable_task.py
+-rw-r--r--   0        0        0     3579 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/executable.py
+-rw-r--r--   0        0        0     1924 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/parameter.py
+-rw-r--r--   0        0        0     5333 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/settings.py
+-rw-r--r--   0        0        0     9060 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/task.py
+-rw-r--r--   0        0        0     3220 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/temporary_wrapper.py
+-rw-r--r--   0        0        0    11587 2024-03-22 10:06:22.773548 b2luigi-1.0.0/b2luigi/core/utils.py
+-rw-r--r--   0        0        0      605 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0     5410 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/advanced/basf2-examples.rst
+-rw-r--r--   0        0        0     4861 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/advanced/development.rst
+-rw-r--r--   0        0        0     4243 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/advanced/faq.rst
+-rw-r--r--   0        0        0     6661 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0     2530 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/documentation/api.rst
+-rw-r--r--   0        0        0      751 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/documentation/b2luigi.basf2_helper.rst
+-rw-r--r--   0        0        0     3528 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/documentation/run_modes.rst
+-rw-r--r--   0        0        0     6554 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/index.rst
+-rw-r--r--   0        0        0     6305 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/usage/batch.rst
+-rw-r--r--   0        0        0     2114 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/usage/installation.rst
+-rw-r--r--   0        0        0     7771 2024-03-22 10:06:22.773548 b2luigi-1.0.0/docs/usage/quickstart.rst
+-rw-r--r--   0        0        0     4468 2024-03-22 10:06:22.773548 b2luigi-1.0.0/examples/basf2/basf2_chain_example.py
+-rw-r--r--   0        0        0     2564 2024-03-22 10:06:22.773548 b2luigi-1.0.0/examples/gbasf2/example_mdst_analysis.py
+-rw-r--r--   0        0        0     2178 2024-03-22 10:06:22.777548 b2luigi-1.0.0/examples/gbasf2/gbasf2_example.py
+-rw-r--r--   0        0        0      133 2024-03-22 10:06:22.777548 b2luigi-1.0.0/examples/gbasf2/settings.json
+-rw-r--r--   0        0        0     1422 2024-03-22 10:06:22.777548 b2luigi-1.0.0/examples/htcondor/htcondor_example.py
+-rw-r--r--   0        0        0      182 2024-03-22 10:06:22.777548 b2luigi-1.0.0/examples/htcondor/settings.json
+-rw-r--r--   0        0        0       50 2024-03-22 10:06:22.777548 b2luigi-1.0.0/examples/htcondor/setup_script.sh
+-rw-r--r--   0        0        0      652 2024-03-22 10:06:22.777548 b2luigi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-03-22 10:06:22.777548 b2luigi-1.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.841549 b2luigi-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.841549 b2luigi-1.0.0/tests/basf2_helper/__init__.py
+-rw-r--r--   0        0        0     2626 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/basf2_helper/test_utils.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.841549 b2luigi-1.0.0/tests/batch/__init__.py
+-rw-r--r--   0        0        0    17959 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json
+-rw-r--r--   0        0        0    17971 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json
+-rw-r--r--   0        0        0     5690 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json
+-rw-r--r--   0        0        0   164412 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json
+-rw-r--r--   0        0        0      858 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/batch_task_1.py
+-rw-r--r--   0        0        0      782 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/batch_task_2.py
+-rw-r--r--   0        0        0      880 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/test_batch_process.py
+-rw-r--r--   0        0        0    18159 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/test_gbasf2_helper_functions.py
+-rw-r--r--   0        0        0    10620 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/test_gbasf2_process.py
+-rw-r--r--   0        0        0     5729 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/batch/test_htcondor_processs.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.845550 b2luigi-1.0.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     1397 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/cli/process_with_user_args_ignored_by_b2luigi.py
+-rw-r--r--   0        0        0      562 2024-03-22 10:06:22.777548 b2luigi-1.0.0/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py
+-rw-r--r--   0        0        0     1003 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/cli/test_ignore_additional_command_line_args.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.845550 b2luigi-1.0.0/tests/core/__init__.py
+-rw-r--r--   0        0        0      663 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/dispatch_1.py
+-rw-r--r--   0        0        0      669 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/dispatch_2.py
+-rw-r--r--   0        0        0      602 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/dispatch_with_env_and_script.py
+-rw-r--r--   0        0        0      368 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/folder_structures.py
+-rw-r--r--   0        0        0      350 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/temporary_task_1.py
+-rw-r--r--   0        0        0      319 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/temporary_task_2.py
+-rw-r--r--   0        0        0     1780 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_dispatch_task.py
+-rw-r--r--   0        0        0      824 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_folder_structures.py
+-rw-r--r--   0        0        0     2214 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_parameter.py
+-rw-r--r--   0        0        0     4028 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_requires.py
+-rw-r--r--   0        0        0     2957 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_settings.py
+-rw-r--r--   0        0        0     3493 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_task.py
+-rw-r--r--   0        0        0      929 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_temporary_files.py
+-rw-r--r--   0        0        0    10839 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-03-22 10:06:22.845550 b2luigi-1.0.0/tests/doc_examples/__init__.py
+-rw-r--r--   0        0        0     1874 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/dict_requirement_example.py
+-rw-r--r--   0        0        0       29 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/settings.json
+-rw-r--r--   0        0        0      527 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/simple_example.py
+-rw-r--r--   0        0        0      527 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/simple_example_b2luigi.py
+-rw-r--r--   0        0        0     1149 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/simple_example_b2luigi_2.py
+-rw-r--r--   0        0        0      482 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/doc_examples/test_examples.py
+-rw-r--r--   0        0        0      906 2024-03-22 10:06:22.781548 b2luigi-1.0.0/tests/helpers.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 b2luigi-1.0.0/PKG-INFO
```

### Comparing `b2luigi-0.9.1/.gitignore` & `b2luigi-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/LICENSE` & `b2luigi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/README.rst` & `b2luigi-1.0.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 b2luigi
 =======
 
-.. image:: https://img.shields.io/readthedocs/b2luigi
-           :target: https://b2luigi.readthedocs.io/en/stable/
-.. image:: https://img.shields.io/github/license/nils-braun/b2luigi
-           :target: https://github.com/nils-braun/b2luigi/blob/main/LICENSE
-.. image:: https://img.shields.io/codecov/c/github/nils-braun/b2luigi?logo=codecov
-           :target: https://codecov.io/gh/nils-braun/b2luigi
-.. image:: https://img.shields.io/github/workflow/status/nils-braun/b2luigi/Test%20Default%20Branch?logo=github
-           :target: https://github.com/nils-braun/b2luigi/actions
+.. image:: https://img.shields.io/badge/sphinx-latest-009682
+           :target: https://software.belle2.org/b2luigi/
+.. image:: https://img.shields.io/github/license/belle2/b2luigi
+           :target: https://github.com/belle2/b2luigi/blob/main/LICENSE
 .. image:: https://img.shields.io/pypi/v/b2luigi?logo=pypi
            :target: https://pypi.python.org/pypi/b2luigi/
 
 
 ``b2luigi`` is a helper package constructed around ``luigi`` that helps you schedule working packages (so-called tasks)
 locally or on a batch system.
 Apart from the very powerful dependency management system by ``luigi``, ``b2luigi`` extends the user interface
-and has a build-in support for the queue systems, e.g. LSF and HTCondor.
+and has a built-in support for the queue systems, e.g. LSF and HTCondor.
 
-You can find more information in the `documentation <https://b2luigi.readthedocs.io/en/stable/>`_.
-
-Please note that most of the core features are handled by ``luigi``, so you might want to have a look into
-the `luigi documentation <https://luigi.readthedocs.io/en/latest/>`_.
+You can find more information in the `documentation <https://software.belle2.org/b2luigi/>`_.
+Please note that most of the core features are handled by ``luigi``, which is described in the
+separate `luigi documentation <https://luigi.readthedocs.io/en/latest/>`_,
+where you can find a lot of useful information.
 
 If you find any bugs or want to add a feature or improve the documentation, please send me a pull request!
+Check the `development documentation <https://software.belle2.org/b2luigi/advanced/development.html>`_
+on information how to contribute.
+
+Contributors are listed `here <https://software.belle2.org/b2luigi/index.html#the-team>`_.
 
 This project is in still beta. Please be extra cautious when using in production mode.
 
-To get notified about new features, (potentiall breaking) changes, bugs and
+To get notified about new features, (potentially breaking) changes, bugs and
 their fixes, I recommend using the ``Watch`` button on github to get
 notifications for new releases and/or issues or to subscribe the `releases feed
-<https://github.com/nils-braun/b2luigi/releases.atom>`_ (requires no github
+<https://github.com/belle2/b2luigi/releases.atom>`_ (requires no GitHub
 account, just a feed reader).
```

### Comparing `b2luigi-0.9.1/b2luigi/__init__.py` & `b2luigi-1.0.0/b2luigi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Task scheduling and batch running for basf2 jobs made simple"""
 from luigi import *
 from luigi.util import copies
 
 # version must be defined after importing the luigi namespace,
 # otherwise the b2luigi.__version__ gets overwritten by the one from luigi
-__version__ = "0.9.1"
+__version__ = "1.0.0"
 
 from b2luigi.core.parameter import wrap_parameter, BoolParameter
 from typing import Optional, Union, Collection
 
 wrap_parameter()
 
 from b2luigi.core.task import Task, ExternalTask, WrapperTask
@@ -139,17 +139,16 @@
 
         # Make sure we're only removing parameters that exist
         assert not self.without, f"You're trying to remove parameter(s) {self.without} which do(es) not exist."
 
         # Modify task_that_inherits by adding methods
         def clone_parent(_self, **kwargs):
             return _self.clone(cls=self.tasks_to_inherit[0], **kwargs)
+
         task_that_inherits.clone_parent = clone_parent
 
         def clone_parents(_self, **kwargs):
-            return [
-                _self.clone(cls=task_to_inherit, **kwargs)
-                for task_to_inherit in self.tasks_to_inherit
-            ]
+            return [_self.clone(cls=task_to_inherit, **kwargs) for task_to_inherit in self.tasks_to_inherit]
+
         task_that_inherits.clone_parents = clone_parents
 
         return task_that_inherits
```

### Comparing `b2luigi-0.9.1/b2luigi/basf2_helper/data.py` & `b2luigi-1.0.0/b2luigi/basf2_helper/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,32 +65,40 @@
 requires_skimmed_raw_data = b2luigi.requires(SkimmedRawDataTask)
 requires_mdst_data = b2luigi.requires(MdstDataTask)
 requires_cdst_data = b2luigi.requires(CdstDataTask)
 
 
 def _get_dir_structure(data_mode):
     if data_mode == DataMode.mdst:
-        return b2luigi.get_setting("mdst_dir_structure",
-                                   "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/" +
-                                   "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/mdst/sub00/" +
-                                   "mdst.{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root")
+        return b2luigi.get_setting(
+            "mdst_dir_structure",
+            "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/"
+            + "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/mdst/sub00/"
+            + "mdst.{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root",
+        )
     if data_mode == DataMode.cdst:
-        return b2luigi.get_setting("cdst_dir_structure",
-                                   "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/" +
-                                   "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/cdst/sub00/" +
-                                   "cdst.{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root")
+        return b2luigi.get_setting(
+            "cdst_dir_structure",
+            "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/"
+            + "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/cdst/sub00/"
+            + "cdst.{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root",
+        )
     if data_mode == DataMode.skimmed_raw:
-        return b2luigi.get_setting("skimmed_raw_dir_structure",
-                                   "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/" +
-                                   "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/raw/sub00/" +
-                                   "raw.{p.prefix}.{p.file_name}.{p.experiment_number:04d}.{p.run_number:05d}.root")
+        return b2luigi.get_setting(
+            "skimmed_raw_dir_structure",
+            "/hsm/belle2/bdata/Data/release-{p.release}/DB{p.database:08d}/prod{p.prod:08d}/"
+            + "e{p.experiment_number:04d}/4S/r{p.run_number:05d}/all/raw/sub00/"
+            + "raw.{p.prefix}.{p.file_name}.{p.experiment_number:04d}.{p.run_number:05d}.root",
+        )
     if data_mode == DataMode.raw:
-        return b2luigi.get_setting("raw_dir_structure",
-                                   "/ghi/fs01/belle2/bdata/Data/Raw/e{p.experiment_number:04d}/r{p.run_number:05d}/sub00/" +
-                                   "{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root")
+        return b2luigi.get_setting(
+            "raw_dir_structure",
+            "/ghi/fs01/belle2/bdata/Data/Raw/e{p.experiment_number:04d}/r{p.run_number:05d}/sub00/"
+            + "{p.prefix}.{p.experiment_number:04d}.{p.run_number:05d}.{p.file_name}.root",
+        )
 
 
 def _build_data_path(parameters):
     mode = parameters.data_mode
 
     dir_structure = _get_dir_structure(mode)
     return dir_structure.format(p=parameters)
@@ -111,49 +119,109 @@
 def _get_data_kwargs(data_mode, experiment_number, run_number, prefix=None, file_name=None, **other_kwargs):
     if file_name is None:
         file_name = "*"
 
     if prefix is None:
         prefix = "*"
 
-    all_kwargs = fill_kwargs_with_lists(data_mode=data_mode, experiment_number=experiment_number, run_number=run_number,
-                                        prefix=prefix,
-                                        file_name=file_name, **other_kwargs)
+    all_kwargs = fill_kwargs_with_lists(
+        data_mode=data_mode,
+        experiment_number=experiment_number,
+        run_number=run_number,
+        prefix=prefix,
+        file_name=file_name,
+        **other_kwargs,
+    )
     for kwargs in product_dict(**all_kwargs):
         # The build_data_path wants an object, so lets convert the dict to a named tuple
-        kwargs = namedtuple('GenericDict', kwargs.keys())(**kwargs)
+        kwargs = namedtuple("GenericDict", kwargs.keys())(**kwargs)
         for data_file in glob(_build_data_path(kwargs)):
             yield _parse_data_path(data_mode, data_file)
 
 
-def clone_on_mdst(self, task_class, experiment_number, run_number, release, prod, database, prefix=None, file_name=None,
-                  **additional_kwargs):
+def clone_on_mdst(
+    self,
+    task_class,
+    experiment_number,
+    run_number,
+    release,
+    prod,
+    database,
+    prefix=None,
+    file_name=None,
+    **additional_kwargs,
+):
     # TODO: make database not needed
-    for kwargs in _get_data_kwargs(data_mode=DataMode.mdst, experiment_number=experiment_number, run_number=run_number,
-                                   release=release,
-                                   prod=prod, database=database, prefix=prefix, file_name=file_name):
+    for kwargs in _get_data_kwargs(
+        data_mode=DataMode.mdst,
+        experiment_number=experiment_number,
+        run_number=run_number,
+        release=release,
+        prod=prod,
+        database=database,
+        prefix=prefix,
+        file_name=file_name,
+    ):
         yield self.clone(task_class, **kwargs, **additional_kwargs)
 
 
-def clone_on_cdst(self, task_class, experiment_number, run_number, release, prod, database, prefix=None, file_name=None,
-                  **additional_kwargs):
+def clone_on_cdst(
+    self,
+    task_class,
+    experiment_number,
+    run_number,
+    release,
+    prod,
+    database,
+    prefix=None,
+    file_name=None,
+    **additional_kwargs,
+):
     # TODO: make database not needed
-    for kwargs in _get_data_kwargs(data_mode=DataMode.cdst, experiment_number=experiment_number, run_number=run_number,
-                                   release=release,
-                                   prod=prod, database=database, prefix=prefix, file_name=file_name):
+    for kwargs in _get_data_kwargs(
+        data_mode=DataMode.cdst,
+        experiment_number=experiment_number,
+        run_number=run_number,
+        release=release,
+        prod=prod,
+        database=database,
+        prefix=prefix,
+        file_name=file_name,
+    ):
         yield self.clone(task_class, **kwargs, **additional_kwargs)
 
 
-def clone_on_skimmed_raw(self, task_class, experiment_number, run_number, release, prod, database, prefix=None, file_name=None,
-                         **additional_kwargs):
+def clone_on_skimmed_raw(
+    self,
+    task_class,
+    experiment_number,
+    run_number,
+    release,
+    prod,
+    database,
+    prefix=None,
+    file_name=None,
+    **additional_kwargs,
+):
     # TODO: make database not needed
-    for kwargs in _get_data_kwargs(data_mode=DataMode.skimmed_raw, experiment_number=experiment_number, run_number=run_number,
-                                   release=release,
-                                   prod=prod, database=database, prefix=prefix, file_name=file_name):
+    for kwargs in _get_data_kwargs(
+        data_mode=DataMode.skimmed_raw,
+        experiment_number=experiment_number,
+        run_number=run_number,
+        release=release,
+        prod=prod,
+        database=database,
+        prefix=prefix,
+        file_name=file_name,
+    ):
         yield self.clone(task_class, **kwargs, **additional_kwargs)
 
 
 def clone_on_raw(self, task_class, experiment_number, run_number, prefix=None, file_name=None, **additional_kwargs):
-    for kwargs in _get_data_kwargs(data_mode=DataMode.raw, experiment_number=experiment_number, run_number=run_number,
-                                   prefix=prefix,
-                                   file_name=file_name):
+    for kwargs in _get_data_kwargs(
+        data_mode=DataMode.raw,
+        experiment_number=experiment_number,
+        run_number=run_number,
+        prefix=prefix,
+        file_name=file_name,
+    ):
         yield self.clone(task_class, **kwargs, **additional_kwargs)
```

### Comparing `b2luigi-0.9.1/b2luigi/basf2_helper/tasks.py` & `b2luigi-1.0.0/b2luigi/basf2_helper/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,26 @@
 
     @b2luigi.on_temporary_files
     def process(self):
         assert get_basf2_git_hash() == self.git_hash
 
         try:
             import basf2
-            import ROOT
         except ImportError:
-            raise ImportError("Can not find ROOT or basf2. Can not use the basf2 task.")
+            raise ImportError("Can not find basf2. Can not use the basf2 task.")
 
         if self.num_processes:
             basf2.set_nprocesses(self.num_processes)
 
-        if self.max_event:
-            ROOT.Belle2.Environment.Instance().setNumberEventsOverride(self.max_event)
-
         path = self.create_path()
 
         path.add_module("Progress")
         basf2.print_path(path)
-        basf2.process(path)
+        max_event = self.max_event if self.max_event else 0
+        basf2.process(path=path, max_event=max_event)
 
         print(basf2.statistics)
 
 
 class SimplifiedOutputBasf2Task(Basf2PathTask):
     def create_path(self):
         raise NotImplementedError()
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/cache.py` & `b2luigi-1.0.0/b2luigi/batch/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     Override the function _ask_for_job_status, which should
     set the job status for the specific job if
     specified or for all accessible jobs (e.g. for all of this user).
     Having too much information (e.g. information on jobs
     which are not started by this b2luigi instance) does not matter.
     """
+
     def __init__(self):
         super().__init__(maxsize=1000, ttl=20)
 
     @abc.abstractmethod
     def _ask_for_job_status(self, job_id=None):
         pass
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/__init__.py` & `b2luigi-1.0.0/b2luigi/batch/processes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,34 @@
     idle = "idle"
 
 
 class BatchProcess:
     """
     This is the base class for all batch algorithms that allow luigi to run on a specific batch system.
     This is an abstract base class and inheriting classes need to supply functionalities for
-    * starting a job using the commands in self.task_cmd
+
+    * starting a job using the commands in ``self.task_cmd``
     * getting the job status of a running, finished or failed job
-    * and killing a job
+    * and terminating a job
+
     All those commands are called from the main process, which is not running on the batch system.
-    Every batch system that is capable of these functions can in principle work together with b2luigi.
+    Every batch system that is capable of these functions can in principle work together with ``b2luigi``.
 
     Implementation note:
         In principle, using the batch system is transparent to the user. In case of problems, it
         may however be useful to understand how it is working.
 
-        When you start your luigi dependency tree with ``process(..., batch=True)``, the normal
-        luigi process is started looking for unfinished tasks and running them etc.
+        When you start your ``luigi`` dependency tree with ``process(..., batch=True)``, the normal
+        ``luigi`` process is started looking for unfinished tasks and running them etc.
         Normally, luigi creates a process for each running task and runs them either directly
         or on a different core (if you have enabled more than one worker).
         In the batch case, this process is not a normal python multiprocessing process,
-        but this BatchProcess, which has the same interface (one can check the status of the process,
-        start or kill it). The process does not need to wait for the batch job to finish but
-        is asked repeatedly for the job status. By this, most of the core functionality of luigi
+        but this ``BatchProcess``, which has the same interface (one can check the status of the process,
+        start or terminate it). The process does not need to wait for the batch job to finish but
+        is asked repeatedly for the job status. By this, most of the core functionality of ``luigi``
         is kept and reused.
         This also means, that every batch job only includes a single task and is finished whenever
         this task is done decreasing the batch runtime. You will need exactly as many batch jobs
         as you have tasks and no batch job will idle waiting for input data as all are scheduled
         only when the task they should run is actually runnable (the input files are there).
 
         What is the batch command now? In each job, we call a specific executable bash script
@@ -48,21 +50,22 @@
         python script or a specified directory by the user) and a call of this script with the
         current python interpreter (the one you used to call this main file or given by the
         setting ``executable``) . However, we give this call an additional parameter, which tells it
         to only run one single task. Task can be identified by their task id. A typical task command may look like::
 
             /<path-to-your-exec>/python /your-project/some-file.py --batch-runner --task-id MyTask_38dsf879w3
 
-        if the batch job should run the MyTask. The implementation of the
+        if the batch job should run the ``MyTask``. The implementation of the
         abstract functions is responsible for creating an running the executable file and writing the log of
         the job into appropriate locations. You can use the functions ``create_executable_wrapper``
         and ``get_log_file_dir`` to get the needed information.
 
-        Checkout the implementation of the lsf task for some implementation example.
+        Checkout the implementation of the ``lsf`` task for some implementation example.
     """
+
     def __init__(self, task, scheduler, result_queue, worker_timeout):
         self.use_multiprocessing = False
         self.task = task
         self.timeout_time = time.time() + worker_timeout if worker_timeout else None
         self._terminated = False
 
         self._result_queue = result_queue
@@ -80,16 +83,16 @@
         How you identify exactly your job is dependent on the implementation and needs to
         be handled by your own child class.
 
         Must return one item of the JobStatus enumeration: running, aborted, successful or idle.
         Will only be called after the job is started but may also be called when
         the job is finished already.
         If the task status is unknown, return aborted. If the task has not started already but
-        is scheduled, return running nevertheless (for b2luigi it makes no difference).
-        No matter if aborted via a call to kill_job, by the batch system or by an exception in the
+        is scheduled, return running nevertheless (for ``b2luigi`` it makes no difference).
+        No matter if aborted via a call to ``terminate_job``, by the batch system or by an exception in the
         job itself, you should return aborted if the job is not finished successfully
         (maybe you need to check the exit code of your job).
         """
         raise NotImplementedError
 
     def start_job(self):
         """
@@ -97,40 +100,40 @@
         It is called exactly once. You need to store any information identifying
         your batch job on your own.
 
         You can use the ``b2luigi.core.utils.get_log_file_dir`` and the
         ``b2luigi.core.executable.create_executable_wrapper`` functions to get the log base name
         and to create the executable script which you should call in your batch job.
 
-        After the start_job function is called by the framework (and no exception is thrown),
+        After the ``start_job`` function is called by the framework (and no exception is thrown),
         it is assumed that a batch job is started or scheduled.
 
         After the job is finished (no matter if aborted or successful) we assume the stdout and stderr
-        is written into the two files given by b2luigi.core.utils.get_log_file_dir(self.task).
+        is written into the two files given by ``b2luigi.core.utils.get_log_file_dir(self.task)``.
         """
         raise NotImplementedError
 
-    def kill_job(self):
+    def terminate_job(self):
         """
-        This command is used to abort a job started by the start_job function.
+        This command is used to abort a job started by the ``start_job`` function.
         It is only called once to abort a job, so make sure to either block until the job is really
         gone or be sure that it will go down soon. Especially, do not wait until the job is finished.
-        It is called for example when the user presses Ctrl-C.
+        It is called for example when the user presses ``Ctrl-C``.
 
         In some strange corner cases it may happen that this function is called even before the
-        job is started (the start_job function is called). In this case, you do not need to do anything
+        job is started (the ``start_job`` function is called). In this case, you do not need to do anything
         (but also not raise an exception).
         """
         raise NotImplementedError
 
     def run(self):
         self.start_job()
 
     def terminate(self):
-        self.kill_job()
+        self.terminate_job()
 
     def is_alive(self):
         if self._terminated:
             return False
 
         job_status = self.get_job_status()
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2.py` & `b2luigi-1.0.0/b2luigi/batch/processes/gbasf2.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 from glob import glob
 from itertools import groupby
 from typing import Iterable, List, Optional, Set, Tuple
 
 from b2luigi.basf2_helper.utils import get_basf2_git_hash
 from b2luigi.batch.processes import BatchProcess, JobStatus
 from b2luigi.core.settings import get_setting
-from b2luigi.core.utils import (flatten_to_dict, get_log_file_dir,
-                                get_task_file_dir)
+from b2luigi.core.utils import flatten_to_dict, get_log_file_dir, get_task_file_dir
 from jinja2 import Template
 from luigi.target import Target
 from retry import retry
 
 
 class Gbasf2Process(BatchProcess):
     """
@@ -33,26 +32,26 @@
 
     Features
         - **gbasf2 project submission**
 
           The gbasf2 batch process takes the basf2 path returned by the
           ``create_path()`` method of the task, saves it into a pickle file to
           the disk and creates a wrapper steering file that executes the saved
-          path. Any basf2 variable aliases added in the ``create_path()`` method
+          path. Any basf2 variable aliases added in the ``Path()`` or ``create_path()`` method
           are also stored in the pickle file. It then sends both the pickle file
-          and the steering file wrapper to the grid via the BelleII-specific
-          Dirac-wrapper gbasf2.
+          and the steering file wrapper to the grid via the Belle II-specific
+          DIRAC-wrapper gbasf2.
 
         - **Project status monitoring**
 
           After the project submission, the gbasf batch process regularly checks the status
           of all the jobs belonging to a gbasf2 project returns a success if
           all jobs had been successful, while a single failed job results in a failed project.
-          You can close a running b2luigi process and then start your script again and if a
-          task with the same project name is running, this b2luigi gbasf2 wrapper will recognize that
+          You can close a running ``b2luigi`` process and then start your script again and if a
+          task with the same project name is running, this ``b2luigi`` gbasf2 wrapper will recognize that
           and instead of resubmitting a new project, continue monitoring the running project.
 
           .. hint::
             The outputs of gbasf2 tasks can be a bit overwhelming, so I recommend using the
             :ref:`central scheduler <central-scheduler-label>`
             which provides a nice overview of all tasks in the browser, including a status/progress
             indicator how many jobs in a gbasf2 project are already done.
@@ -64,15 +63,15 @@
           before moving the data to the final location. On failure, it only downloads the logs.
           The dataset download can be optionally disabled.
 
         - **Automatic rescheduling of failed jobs**
 
           Whenever a job fails, gbasf2 reschedules it as long as the number of retries is below the
           value of the setting ``gbasf2_max_retries``. It keeps track of the number of retries in a
-          local file in the ``log_file_dir``, so that it does not change if you close b2luigi and start it again.
+          local file in the ``log_file_dir``, so that it does not change if you close ``b2luigi`` and start it again.
           Of course it does not persist if you remove that file or move to a different machine.
 
     .. note::
        Despite all the automatization that this gbasf2 wrapper provides, the user is expected to
        have a basic understanding of how the grid works and know the basics of working
        with gbasf2 commands manually.
 
@@ -134,16 +133,16 @@
            class MyTask(Basf2PathTask):
                batch_system = "gbasf2"
                gbasf2_project_name_prefix = b2luigi.Parameter(significant=False)
                gbasf2_input_dataset = b2luigi.Parameter(hashed=True)
 
         Other not required, but noteworthy settings are:
 
-        - ``gbasf2_install_directory``: Directory where gbasf2 is installed.
-            Defaults to ``/cvmfs/belle.kek.jp/grid/gbasf2/pro/../..``, which should point to the latest gbasf2 release.
+        - ``gbasf2_setup_path``: Path to gbasf2 environment setup script that needs so be sourced to run gbasf2 commands.
+          Defaults to ``/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc``.
         - ``gbasf2_release``: Defaults to the release of your currently set up basf2 release.
           Set this if you want the jobs to use another release on the grid.
         - ``gbasf2_proxy_lifetime``: Defaults to 24. When initializing a proxy, set the
           lifetime to this number of hours.
         - ``gbasf2_min_proxy_lifetime``: Defaults to 0. During processing, prompt user
           to reinitialize proxy if remaining proxy lifetime drops below this number of
           hours.
@@ -164,15 +163,15 @@
 
             from b2luigi.batch.processes.gbasf2 import get_unique_project_name, Gbasf2GridProjectTarget
 
             class MyTask(Basf2PathTask):
                 # [...]
                 def output(self):
                     project_name = get_unique_project_name(self)
-                    return Gbasf2GridProjectTarget(project_name, task=self)
+                    return Gbasf2GridProjectTarget(project_name)
 
           This is useful when chaining gbasf2 tasks together,
           as they don't need the output locally but take the grid datasets as input. Also useful when you just want
           to produce data on the grid for other people to use.
 
         - ``gbasf2_download_logs``: Whether to automatically download the log output of gbasf2 projects when the
           task succeeds or fails. Having the logs is important for reproducibility, but k
@@ -227,39 +226,65 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         #: gbasf2 project name, must be property/attribute, e.g. a luigi parameter
         # Setting it via a setting.json file is not supported to make sure users set unique project names
         self.gbasf2_project_name = get_unique_project_name(self.task)
 
+        self.gbasf2_setup_path = get_setting(
+            "gbasf2_setup_path",
+            default="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+            task=self.task,
+        )
+
+        if not os.path.isfile(self.gbasf2_setup_path):
+            raise FileNotFoundError(
+                errno.ENOENT,
+                os.strerror(errno.ENOENT),
+                f"File not found: {self.gbasf2_setup_path}.\n"
+                "Maybe you need to customize the `gbasf2_setup_path` setting?\n"
+                "That is sometimes necessary when file location changed between gbasf2 releases.",
+            )
+
+        if get_setting(
+            "gbasf2_install_directory",
+            default=False,
+            task=self.task,
+        ):
+            warnings.warn(
+                "IGNORING deprecated setting `gbasf2_install_directory`"
+                + "Instead set the path to the setup file directly with the `gbasf2_setup_path` setting.",
+                DeprecationWarning,
+            )
+
         #: Output file directory of the task to wrap with gbasf2, where we will
         # store the pickled basf2 path and the created steerinfile to execute
         # that path.
         task_file_dir = get_task_file_dir(self.task)
         os.makedirs(task_file_dir, exist_ok=True)
         #: file name in which the pickled basf2 path from ``self.task.create_path()`` will be stored
         self.pickle_file_path = os.path.join(task_file_dir, "serialized_basf2_path.pkl")
         #: file name for steering file that executes pickled path, which will be send to the grid
         self.wrapper_file_path = os.path.join(task_file_dir, "steering_file_wrapper.py")
 
         self.log_file_dir = get_log_file_dir(self.task)
         os.makedirs(self.log_file_dir, exist_ok=True)
 
-        self.dirac_user = get_dirac_user()
+        self.dirac_user = get_dirac_user(self.gbasf2_setup_path)
         #: Maximum number of times that each job in the project can be rescheduled until the project is declared as failed.
         self.max_retries = get_setting("gbasf2_max_retries", default=0, task=self.task)
 
+        #: Setting to incorporate custom steering files into b2luigi.
+        self.gbasf2_custom_steering_file = get_setting("gbasf2_custom_steering_file", default="", task=self.task)
         #: Store number of times each job had been rescheduled
         self.n_retries_by_job = Counter()
 
         #: Local storage for ``n_retries_by_job`` counter
-        # so that it persists even if luigi process is killed and restarted.
-        self.retries_file_path = os.path.join(
-            self.log_file_dir, "n_retries_by_grid_job.json"
-        )
+        # so that it persists even if luigi process is terminated and restarted.
+        self.retries_file_path = os.path.join(self.log_file_dir, "n_retries_by_grid_job.json")
         if os.path.isfile(self.retries_file_path):
             with open(self.retries_file_path, "r") as retries_file:
                 retries_from_file = json.load(retries_file)
                 self.n_retries_by_job.update(retries_from_file)
 
         # Store dictionary with n_jobs_by_status in attribute to check if it changed,
         # useful for printing job status on change only
@@ -276,40 +301,38 @@
 
         First obtain the status of all (sub-) jobs in a gbasf2 project, similar
         to ``gb2_job_status``, and return an overall project status, e.g. when
         all jobs are done, return ``JobStatus.successful`` to show that the
         gbasf2 project succeeded.
         """
         job_status_dict = get_gbasf2_project_job_status_dict(
-            self.gbasf2_project_name, dirac_user=self.dirac_user
+            self.gbasf2_project_name,
+            dirac_user=self.dirac_user,
+            gbasf2_setup_path=self.gbasf2_setup_path,
         )
         n_jobs_by_status = Counter()
         for _, job_info in job_status_dict.items():
             n_jobs_by_status[job_info["Status"]] += 1
 
         # recheck the status more closely, and correct
         # reason: sometimes 'Status' marked as 'Done',
         # while 'ApplicationStatus' is not 'Done'
         for _, job_info in job_status_dict.items():
-            if job_info["Status"] == "Done" and (
-                job_info["ApplicationStatus"] != "Done"
-            ):
+            if job_info["Status"] == "Done" and (job_info["ApplicationStatus"] != "Done"):
                 n_jobs_by_status["Done"] -= 1
                 n_jobs_by_status["Failed"] += 1
 
         # print summary of jobs in project if setting is set and job status changed
         if (
             get_setting("gbasf2_print_status_updates", default=True, task=self.task)
             and n_jobs_by_status != self._n_jobs_by_status
         ):
             time_string = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             job_status_string = str(dict(sorted(n_jobs_by_status.items()))).strip("{}")
-            print(
-                f'Jobs in gbasf2 project "{self.gbasf2_project_name}" at {time_string}: {job_status_string}'
-            )
+            print(f'Jobs in gbasf2 project "{self.gbasf2_project_name}" at {time_string}: {job_status_string}')
         self._n_jobs_by_status = n_jobs_by_status
 
         n_jobs = len(job_status_dict)
         n_done = n_jobs_by_status["Done"]
         # note: "Killed" jobs also get moved to "Failed" after a while
         n_failed = n_jobs_by_status["Failed"]
         n_in_final_state = n_done + n_failed
@@ -325,17 +348,15 @@
 
         # task is running
         if n_in_final_state < n_jobs:
             # try updating progressbar for central scheduler web view
             percentage = n_done / n_jobs * 100
             self._scheduler.set_task_progress_percentage(self.task.task_id, percentage)
 
-            status_message = "\n".join(
-                f"{status}: {n_jobs}" for status, n_jobs in n_jobs_by_status.items()
-            )
+            status_message = "\n".join(f"{status}: {n_jobs}" for status, n_jobs in n_jobs_by_status.items())
             self._scheduler.set_task_status_message(self.task.task_id, status_message)
 
             return JobStatus.running
 
         # Require all jobs to be done for project success, any job failure results in a failed project
         if n_done == n_jobs:
             # download dataset only the first time that we return JobStatus.successful
@@ -363,38 +384,38 @@
             self._download_dataset()
 
     def _on_failure_action(self):
         """
         Things to do after the project failed
         """
         job_status_dict = get_gbasf2_project_job_status_dict(
-            self.gbasf2_project_name, dirac_user=self.dirac_user
+            self.gbasf2_project_name, dirac_user=self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path
         )
         failed_job_dict = {
             job_id: job_info
             for job_id, job_info in job_status_dict.items()
             if job_info["Status"] == "Failed"
-            or (
-                job_info["Status"] == "Done" and job_info["ApplicationStatus"] != "Done"
-            )
+            or (job_info["Status"] == "Done" and job_info["ApplicationStatus"] != "Done")
         }
         n_failed = len(failed_job_dict)
         print(f"{n_failed} failed jobs:\n{failed_job_dict}")
         if get_setting("gbasf2_download_logs", default=True, task=self.task):
             self._download_logs()
 
     def _reschedule_failed_jobs(self):
         """
         Tries to reschedule failed jobs in the project if ``self.max_retries`` has not been reached
         and returns ``True`` if rescheduling has been successful.
         """
         jobs_to_be_rescheduled = []
         jobs_hitting_max_n_retries = []
         job_status_dict = get_gbasf2_project_job_status_dict(
-            self.gbasf2_project_name, dirac_user=self.dirac_user
+            self.gbasf2_project_name,
+            dirac_user=self.dirac_user,
+            gbasf2_setup_path=self.gbasf2_setup_path,
         )
 
         for job_id, job_info in job_status_dict.items():
             if job_info["Status"] == "Failed" or (
                 job_info["Status"] == "Done" and job_info["ApplicationStatus"] != "Done"
             ):
                 if self.n_retries_by_job[job_id] < self.max_retries:
@@ -420,44 +441,38 @@
         return True
 
     def _reschedule_jobs(self, job_ids):
         """
         Reschedule chosen list of jobs.
         """
         print("Rescheduling jobs:")
-        print(
-            "\t"
-            + "\n\t".join(
-                f"{job_id} ({self.n_retries_by_job[job_id]} retries)"
-                for job_id in job_ids
-            )
-        )
+        print("\t" + "\n\t".join(f"{job_id} ({self.n_retries_by_job[job_id]} retries)" for job_id in job_ids))
 
-        reschedule_command = shlex.split(
-            f"gb2_job_reschedule --jobid {' '.join(job_ids)} --force"
-        )
-        run_with_gbasf2(reschedule_command)
+        reschedule_command = shlex.split(f"gb2_job_reschedule --jobid {' '.join(job_ids)} --force")
+        run_with_gbasf2(reschedule_command, gbasf2_setup_path=self.gbasf2_setup_path)
 
     def start_job(self):
-        """
-        Submit new gbasf2 project to grid
-        """
-        if check_project_exists(self.gbasf2_project_name, self.dirac_user):
+        """Submit new gbasf2 project to grid."""
+        if check_project_exists(self.gbasf2_project_name, self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path):
             print(
                 f"\nProject with name {self.gbasf2_project_name} already exists on grid, "
                 "therefore not submitting new project. If you want to submit a new project, "
                 "change the project name."
             )
             return
 
-        self._write_path_to_file()
-        self._create_wrapper_steering_file()
+        if self.gbasf2_custom_steering_file:
+            self._copy_custom_steering_script()
+        else:
+            self._write_path_to_file()
+            self._create_wrapper_steering_file()
 
         # submit gbasf2 project
         gbasf2_command = self._build_gbasf2_submit_command()
+
         print(f"\nSubmitting gbasf2 project: {self.gbasf2_project_name}")
         print("\nUsing command:\n" + " ".join(gbasf2_command) + "\n")
 
         # Symlink the pickle_file from the ``task_file_dir`` (where it is store
         # for reproducibility) to the current working directory, so that gbasf2
         # copies it into the same directory in the grid input sandbox as the
         # steering file.
@@ -466,110 +481,86 @@
             os.remove(pickle_file_symlink_destination)
         try:
             os.symlink(
                 self.pickle_file_path,
                 pickle_file_symlink_destination,
                 target_is_directory=False,
             )
-            run_with_gbasf2(gbasf2_command)
+            run_with_gbasf2(gbasf2_command, gbasf2_setup_path=self.gbasf2_setup_path)
         finally:
             os.unlink(pickle_file_symlink_destination)
 
-    def kill_job(self):
-        """
-        Kill gbasf2 project
-        """
+    def terminate_job(self):
+        """Terminate gbasf2 project."""
         if not check_project_exists(
-            self.gbasf2_project_name, dirac_user=self.dirac_user
+            self.gbasf2_project_name, dirac_user=self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path
         ):
             return
         # Note: The two commands ``gb2_job_delete`` and ``gb2_job_kill`` differ
-        # in that deleted jobs are killed and removed from the job database,
-        # while only killed jobs can be restarted.
-        command = shlex.split(
-            f"gb2_job_kill --force --user {self.dirac_user} -p {self.gbasf2_project_name}"
-        )
-        run_with_gbasf2(command)
+        # in that deleted jobs are terminated and removed from the job database,
+        # while only terminated jobs can be restarted.
+        command = shlex.split(f"gb2_job_kill --force --user {self.dirac_user} -p {self.gbasf2_project_name}")
+        run_with_gbasf2(command, gbasf2_setup_path=self.gbasf2_setup_path)
 
     def _build_gbasf2_submit_command(self):
         """
         Function to create the gbasf2 submit command to pass to run_with_gbasf2
         from the task options and attributes.
         """
-        gbasf2_release = get_setting(
-            "gbasf2_release", default=get_basf2_git_hash(), task=self.task
-        )
-        gbasf2_additional_files = get_setting(
-            "gbasf2_additional_files", default=[], task=self.task
-        )
-        if not isinstance(gbasf2_additional_files, Iterable) or isinstance(
-            gbasf2_additional_files, str
-        ):
-            raise ValueError(
-                "``gbasf2_additional_files`` is not an iterable or strings."
-            )
-        gbasf2_input_sandbox_files = [os.path.basename(self.pickle_file_path)] + list(
-            gbasf2_additional_files
-        )
-        gbasf2_command_str = (
-            f"gbasf2 {self.wrapper_file_path} -f {' '.join(gbasf2_input_sandbox_files)} "
-            + f"-p {self.gbasf2_project_name} -s {gbasf2_release} "
-        )
+        gbasf2_release = get_setting("gbasf2_release", default=get_basf2_git_hash(), task=self.task)
+
+        gbasf2_command_str = f"gbasf2 {self.wrapper_file_path} -p {self.gbasf2_project_name} -s {gbasf2_release} "
+
+        gbasf2_additional_files = get_setting("gbasf2_additional_files", default=[], task=self.task)
+
+        if not isinstance(gbasf2_additional_files, Iterable) or isinstance(gbasf2_additional_files, str):
+            raise ValueError("``gbasf2_additional_files`` is not an iterable or strings.")
+
+        input_sandboxfiles = []
+
+        if self.gbasf2_custom_steering_file:
+            input_sandboxfiles.extend(gbasf2_additional_files)
+        else:
+            gbasf2_input_sandbox_files = [os.path.basename(self.pickle_file_path)] + list(gbasf2_additional_files)
+            input_sandboxfiles.extend(gbasf2_input_sandbox_files)
+
+        if input_sandboxfiles:
+            gbasf2_command_str += f"-f {' '.join(input_sandboxfiles)}"
 
         gbasf2_noscout = get_setting("gbasf2_noscout", default=False, task=self.task)
         if gbasf2_noscout:
             gbasf2_command_str += " --noscout "
 
-        gbasf2_input_dataset = get_setting(
-            "gbasf2_input_dataset", default=False, task=self.task
-        )
-        gbasf2_input_dslist = get_setting(
-            "gbasf2_input_dslist", default=False, task=self.task
-        )
+        gbasf2_input_dataset = get_setting("gbasf2_input_dataset", default=False, task=self.task)
+        gbasf2_input_dslist = get_setting("gbasf2_input_dslist", default=False, task=self.task)
 
         if gbasf2_input_dataset is not False and gbasf2_input_dslist is not False:
-            raise RuntimeError(
-                "Can't use both `gbasf2_input_dataset` and `gbasf2_input_dslist` simultaneously."
-            )
+            raise RuntimeError("Can't use both `gbasf2_input_dataset` and `gbasf2_input_dslist` simultaneously.")
 
         if gbasf2_input_dataset is not False:
             gbasf2_command_str += f" -i {gbasf2_input_dataset} "
         elif gbasf2_input_dslist is not False:
             if not os.path.isfile(gbasf2_input_dslist):
-                raise FileNotFoundError(
-                    errno.ENOTDIR, os.strerror(errno.ENOTDIR), gbasf2_input_dslist
-                )
-            gbasf2_command_str += (
-                f" --input_dslist {os.path.abspath(gbasf2_input_dslist)} "
-            )
+                raise FileNotFoundError(errno.ENOTDIR, os.strerror(errno.ENOTDIR), gbasf2_input_dslist)
+            gbasf2_command_str += f" --input_dslist {os.path.abspath(gbasf2_input_dslist)} "
         else:
-            raise RuntimeError(
-                "Must set either `gbasf2_input_dataset` or `gbasf2_input_dslist`."
-            )
+            raise RuntimeError("Must set either `gbasf2_input_dataset` or `gbasf2_input_dslist`.")
 
-        gbasf2_n_repition_jobs = get_setting(
-            "gbasf2_n_repition_job", default=False, task=self.task
-        )
+        gbasf2_n_repition_jobs = get_setting("gbasf2_n_repition_job", default=False, task=self.task)
         if gbasf2_n_repition_jobs is not False:
             gbasf2_command_str += f" --repetition {gbasf2_n_repition_jobs} "
 
-        gbasf2_input_datafiles = get_setting(
-            "gbasf2_input_datafiles", default=[], task=self.task
-        )
+        gbasf2_input_datafiles = get_setting("gbasf2_input_datafiles", default=[], task=self.task)
         if gbasf2_input_datafiles:
-            gbasf2_command_str += (
-                f" --input_datafiles {' '.join(gbasf2_input_datafiles)}"
-            )
+            gbasf2_command_str += f" --input_datafiles {' '.join(gbasf2_input_datafiles)}"
 
         # now add some additional optional options to the gbasf2 job submission string
 
         # whether to ask user for confirmation before submitting job
-        force_submission = get_setting(
-            "gbasf2_force_submission", default=True, task=self.task
-        )
+        force_submission = get_setting("gbasf2_force_submission", default=True, task=self.task)
         if force_submission:
             gbasf2_command_str += " --force "
 
         # estimated cpu time per sub-job in minutes
         cpu_minutes = get_setting("gbasf2_cputime", default=False, task=self.task)
         if cpu_minutes is not False:
             gbasf2_command_str += f" --cputime {cpu_minutes} "
@@ -596,21 +587,17 @@
         if basf2opt is not False:
             gbasf2_command_str += f" --basf2opt='{basf2opt}' "
 
         # Provide a output_ds parameter if the group is not belle
         group_name = get_setting("gbasf2_proxy_group", default="belle")
         if group_name != "belle":
             output_lpn_dir = get_setting("gbasf2_project_lpn_path")
-            gbasf2_command_str += (
-                f" --output_ds {output_lpn_dir}/{self.gbasf2_project_name}"
-            )
+            gbasf2_command_str += f" --output_ds {output_lpn_dir}/{self.gbasf2_project_name}"
         # optional string of additional parameters to append to gbasf2 command
-        gbasf2_additional_params = get_setting(
-            "gbasf2_additional_params", default=False, task=self.task
-        )
+        gbasf2_additional_params = get_setting("gbasf2_additional_params", default=False, task=self.task)
         if gbasf2_additional_params is not False:
             gbasf2_command_str += f" {gbasf2_additional_params} "
 
         gbasf2_command = shlex.split(gbasf2_command_str)
         return gbasf2_command
 
     def _write_path_to_file(self):
@@ -622,38 +609,44 @@
         try:
             basf2_path = self.task.create_path()
         except AttributeError as err:
             raise Exception(
                 "Gbasf2 batch process can only used with tasks that generate basf2 paths with "
                 "a ``create_path()`` method, e.g. are an instance of ``Basf2PathTask``."
             ) from err
-        from b2luigi.batch.processes.gbasf2_utils.pickle_utils import \
-            write_path_and_state_to_file
+        from b2luigi.batch.processes.gbasf2_utils.pickle_utils import write_path_and_state_to_file
 
         write_path_and_state_to_file(basf2_path, self.pickle_file_path)
 
     def _create_wrapper_steering_file(self):
         """
         Create a steering file to send to the grid that executes the pickled
         basf2 path from ``self.task.create_path()``.
         """
         # read a jinja2 template for the steerinfile that should execute the pickled path
-        template_file_path = os.path.join(
-            self._file_dir, "templates/gbasf2_steering_file_wrapper.jinja2"
-        )
+        template_file_path = os.path.join(self._file_dir, "templates/gbasf2_steering_file_wrapper.jinja2")
         with open(template_file_path, "r") as template_file:
             template = Template(template_file.read())
             # replace some variable values in the templates
             steering_file_stream = template.stream(
                 pickle_file_path=os.path.basename(self.pickle_file_path),
                 max_event=get_setting("max_event", default=0, task=self.task),
             )
             # write the template with the replacements to a new file which should be sent to the grid
             steering_file_stream.dump(self.wrapper_file_path)
 
+    def _copy_custom_steering_script(self):
+        if os.path.exists(self.gbasf2_custom_steering_file):
+            shutil.copy(src=self.gbasf2_custom_steering_file, dst=self.wrapper_file_path)
+        else:
+            raise ValueError(
+                f"Custom gbasf2 output file does not exists at {self.gbasf2_custom_steering_file}. "
+                "Ensure this file exists and try again."
+            )
+
     def _get_gbasf2_dataset_query(self, output_file_name: str) -> str:
         """
         Helper method that returns the gbasf2 query string with the correct wildcard pattern
         to get the subset of all files for ``output_file_name`` from the grid project associated with this task,
         either, e.g. via the ``gb2_ds_list`` or ``gb2_ds_get`` commands.
 
         Args:
@@ -662,31 +655,27 @@
                 the :py:func:`b2luigi.Task.output` method.
         """
         if output_file_name != os.path.basename(output_file_name):
             raise ValueError(
                 f'For grid projects, the output file name must be a basename, not a path, but is "{output_file_name}"'
             )
         # split file basename into stem and all extensions (e.g. "file.udst.root" into "file" and ".udst.root")
-        output_file_stem, output_file_extensions = _split_all_extensions(
-            output_file_name
-        )
+        output_file_stem, output_file_extensions = _split_all_extensions(output_file_name)
         if not output_file_extensions.endswith(".root"):
             raise ValueError(
                 f'Output file name extensions "{output_file_extensions}" do not '
                 'end with ".root", but gbasf2 batch only supports root outputs.'
             )
         output_lpn_dir = f"/belle/user/{self.dirac_user}"
         group_name = get_setting("gbasf2_proxy_group", default="belle")
         if group_name != "belle":
             output_lpn_dir = get_setting("gbasf2_project_lpn_path")
         return f"{output_lpn_dir}/{self.gbasf2_project_name}/sub*/{output_file_stem}_*{output_file_extensions}"
 
-    def _local_gb2_dataset_is_complete(
-        self, output_file_name: str, check_temp_dir: bool = False
-    ) -> bool:
+    def _local_gb2_dataset_is_complete(self, output_file_name: str, check_temp_dir: bool = False) -> bool:
         """
         Helper method that returns ``True`` if the download of the gbasf2
         dataset for the output ``output_file_name`` is complete.
 
         Args:
             output_file_name: Output file name, must be a root file, e.g. ``ntuple.root``.
                 Usually defined by the user via :py:func:`b2luigi.Task.add_to_output` in
@@ -697,53 +686,46 @@
         """
         # first get the local set of files in the dataset for `output_file_name`
         task_output_dict = flatten_to_dict(self.task.output())
         output_target = task_output_dict[output_file_name]
         output_dir_path = output_target.path
         if check_temp_dir:
             # files in the temporary download directory
-            glob_expression = os.path.join(
-                f"{output_dir_path}.partial", self.gbasf2_project_name, "sub*", "*.root"
-            )
-            downloaded_dataset_basenames = [
-                os.path.basename(fpath) for fpath in glob(glob_expression)
-            ]
+            glob_expression = os.path.join(f"{output_dir_path}.partial", self.gbasf2_project_name, "sub*", "*.root")
+            downloaded_dataset_basenames = [os.path.basename(fpath) for fpath in glob(glob_expression)]
         else:
             # file in the final output directory
             downloaded_dataset_basenames = os.listdir(output_dir_path)
         if not downloaded_dataset_basenames:
             return False
 
-        # get the remote set of grid file names for the gbasf2 project output matching output_file_name
+        # get the remote set of grid file names for the gbasf2 project output
+        # matching output_file_name
         ds_query_string = self._get_gbasf2_dataset_query(output_file_name)
-        output_dataset_grid_filepaths = query_lpns(ds_query_string)
-        output_dataset_basenames = [
-            os.path.basename(grid_path) for grid_path in output_dataset_grid_filepaths
-        ]
+        output_dataset_grid_filepaths = query_lpns(
+            ds_query_string,
+            dirac_user=self.dirac_user,
+            gbasf2_setup_path=self.gbasf2_setup_path,
+        )
+        output_dataset_basenames = [os.path.basename(grid_path) for grid_path in output_dataset_grid_filepaths]
         # remove duplicate LFNs that gb2_ds_list returns for outputs from rescheduled jobs
         output_dataset_basenames = get_unique_lfns(output_dataset_basenames)
         # check if local and remote datasets are equal
         if set(output_dataset_basenames) == set(downloaded_dataset_basenames):
             return True
-        missing_files = list(
-            set(output_dataset_basenames).difference(downloaded_dataset_basenames)
-        )
-        superfluous_files = list(
-            set(downloaded_dataset_basenames).difference(output_dataset_basenames)
-        )
+        missing_files = list(set(output_dataset_basenames).difference(downloaded_dataset_basenames))
+        superfluous_files = list(set(downloaded_dataset_basenames).difference(output_dataset_basenames))
         if missing_files:
             warnings.warn(
                 "\nFiles missing in download:\n{}".format("\n".join(missing_files)),
                 RuntimeWarning,
             )
         if superfluous_files:
             warnings.warn(
-                "\nFiles superfluous in download:\n{}".format(
-                    "\n".join(superfluous_files)
-                ),
+                "\nFiles superfluous in download:\n{}".format("\n".join(superfluous_files)),
                 RuntimeWarning,
             )
         return False
 
     def _download_dataset(self):
         """
         Download the task outputs from the gbasf2 project dataset.
@@ -751,63 +733,58 @@
         For each task output defined via ``self.add_to_output(<name>.root)`` a
         directory will be created, into which all files named ``name_*.root`` on
         the grid dataset corresponding to the project name will be downloaded.
         The download is ensured to be automatic by first downloading into
         temporary directories.
         """
         if not check_dataset_exists_on_grid(
-            self.gbasf2_project_name, dirac_user=self.dirac_user
+            self.gbasf2_project_name, dirac_user=self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path
         ):
-            raise RuntimeError(
-                f"Not dataset to download under project name {self.gbasf2_project_name}"
-            )
+            raise RuntimeError(f"Not dataset to download under project name {self.gbasf2_project_name}")
         task_output_dict = flatten_to_dict(self.task.output())
         for output_file_name, output_target in task_output_dict.items():
             dataset_query_string = self._get_gbasf2_dataset_query(output_file_name)
             output_dir_path = output_target.path
             # check if dataset had been already downloaded and if so, skip downloading
-            if os.path.isdir(output_dir_path) and self._local_gb2_dataset_is_complete(
-                output_file_name
-            ):
-                print(
-                    f"Dataset already exists in {output_dir_path}, skipping download."
-                )
+            if os.path.isdir(output_dir_path) and self._local_gb2_dataset_is_complete(output_file_name):
+                print(f"Dataset already exists in {output_dir_path}, skipping download.")
                 continue
 
             # To prevent from task being accidentally marked as complete when the gbasf2 dataset download failed,
             # we create a temporary directory and first download the dataset there.
             # If the download had been successful and the local files are identical to the list of files on the grid,
             # we move the downloaded dataset to the location specified by ``output_dir_path``.
             tmp_output_dir_path = f"{output_dir_path}.partial"
-            tmp_project_dir = os.path.join(
-                tmp_output_dir_path, self.gbasf2_project_name
-            )
+            tmp_project_dir = os.path.join(tmp_output_dir_path, self.gbasf2_project_name)
             # if custom group is given we need to append the project name
             group_name = get_setting("gbasf2_proxy_group", default="belle")
             if group_name != "belle":
                 tmp_output_dir_path += f"/{self.gbasf2_project_name}"
                 tmp_project_dir = tmp_output_dir_path
             os.makedirs(tmp_output_dir_path, exist_ok=True)
 
             # Need a set files to repeat download for FAILED ones only
-            monitoring_failed_downloads_file = os.path.abspath(
-                os.path.join(tmp_output_dir_path, "failed_files.txt")
-            )
+            monitoring_failed_downloads_file = os.path.abspath(os.path.join(tmp_output_dir_path, "failed_files.txt"))
             (
                 monitoring_download_file_stem,
                 monitoring_downloads_file_ext,
             ) = os.path.splitext(monitoring_failed_downloads_file)
-            old_monitoring_failed_downloads_file = (
-                f"{monitoring_download_file_stem}_old{monitoring_downloads_file_ext}"
-            )
+            old_monitoring_failed_downloads_file = f"{monitoring_download_file_stem}_old{monitoring_downloads_file_ext}"
+
+            # gbasf2 uses a different folder structure when using the `--new` flag with a
+            # proxy_group other than `belle`. Therefore don't use the flag in this case for now.
+            new_flag = "--new" if group_name == "belle" else ""
+
+            # TODO: always use downloads with --new to avoid having to support
+            # two download types and because --new might become the default
 
             # In case of first download, the file 'monitoring_failed_downloads_file' does not exist
             if not os.path.isfile(monitoring_failed_downloads_file):
                 ds_get_command = shlex.split(
-                    f"gb2_ds_get --new --force {dataset_query_string} "
+                    f"gb2_ds_get {new_flag} --force {dataset_query_string} "
                     f"--failed_lfns {monitoring_failed_downloads_file}"
                 )
                 print(
                     f"Downloading dataset into\n  {tmp_output_dir_path}\n  with command\n  ",
                     " ".join(ds_get_command),
                 )
 
@@ -815,66 +792,59 @@
             else:
                 # Rename current 'monitoring_failed_downloads_file' to reuse the path in case the download fails again
                 os.rename(
                     monitoring_failed_downloads_file,
                     old_monitoring_failed_downloads_file,
                 )
                 ds_get_command = shlex.split(
-                    f"gb2_ds_get --new --force {dataset_query_string} "
+                    f"gb2_ds_get {new_flag} --force {dataset_query_string} "
                     f"--input_dslist {old_monitoring_failed_downloads_file} "
                     f"--failed_lfns {monitoring_failed_downloads_file}"
                 )
                 print(
                     f"Downloading remaining files into\n  {tmp_output_dir_path}\n  with command\n  ",
                     " ".join(ds_get_command),
                 )
 
             stdout = run_with_gbasf2(
-                ds_get_command, cwd=tmp_output_dir_path, capture_output=True
+                ds_get_command,
+                cwd=tmp_output_dir_path,
+                capture_output=True,
+                gbasf2_setup_path=self.gbasf2_setup_path,
             ).stdout
             print(stdout)
             if "No file found" in stdout:
-                raise RuntimeError(
-                    f"No output data for gbasf2 project {self.gbasf2_project_name} found."
-                )
+                raise RuntimeError(f"No output data for gbasf2 project {self.gbasf2_project_name} found.")
 
             # Check, whether a file with failed lfns was created
             failed_files = []
             if os.path.isfile(monitoring_failed_downloads_file):
-                with open(
-                    monitoring_failed_downloads_file, "r"
-                ) as failed_downloads_fileobj:
-                    failed_files = [
-                        f.strip() for f in failed_downloads_fileobj.readlines()
-                    ]
+                with open(monitoring_failed_downloads_file, "r") as failed_downloads_fileobj:
+                    failed_files = [f.strip() for f in failed_downloads_fileobj.readlines()]
 
             if not failed_files:
                 # In case all downloads were successful:
                 # remove 'old_monitoring_failed_downloads_file' and 'monitoring_failed_downloads_file'
                 if os.path.isfile(old_monitoring_failed_downloads_file):
                     os.remove(old_monitoring_failed_downloads_file)
                 if os.path.isfile(monitoring_failed_downloads_file):
                     os.remove(monitoring_failed_downloads_file)
 
-            if not self._local_gb2_dataset_is_complete(
-                output_file_name, check_temp_dir=True
-            ):
+            if not self._local_gb2_dataset_is_complete(output_file_name, check_temp_dir=True):
                 raise RuntimeError(
                     f"Download incomplete. The downloaded set of files in {tmp_project_dir} is not equal to the "
                     + f"list of dataset files on the grid for project {self.gbasf2_project_name}.",
                 )
 
             print(
                 f"Download of {self.gbasf2_project_name} files successful.\n"
                 f"Moving output files to directory: {output_dir_path}"
             )
             # sub00 and other sub<xy> directories in case of other datasets
-            _move_downloaded_dataset_to_output_dir(
-                project_download_path=tmp_project_dir, output_path=output_dir_path
-            )
+            _move_downloaded_dataset_to_output_dir(project_download_path=tmp_project_dir, output_path=output_dir_path)
 
     def _download_logs(self):
         """
         Download sandbox files from grid with logs for each job in the gbasf2 project.
 
         It wraps ``gb2_job_output``, which downloads the job sandbox, which has the following structure:
 
@@ -897,21 +867,22 @@
         # new log download, but then the download fails and the user might be
         # left with no logs, first the log download is performed to a temporary
         # directory and then moved to the final location
         with tempfile.TemporaryDirectory(dir=self.log_file_dir) as tmpdir_path:
             download_logs_command = shlex.split(
                 f"gb2_job_output --user {self.dirac_user} -p {self.gbasf2_project_name}"
             )
-            run_with_gbasf2(download_logs_command, cwd=tmpdir_path)
-            tmp_gbasf2_log_path = os.path.join(
-                tmpdir_path, "log", self.gbasf2_project_name
-            )
-            gbasf2_project_log_dir = os.path.join(
-                self.log_file_dir, "gbasf2_logs", self.gbasf2_project_name
+            run_with_gbasf2(
+                download_logs_command,
+                cwd=tmpdir_path,
+                gbasf2_setup_path=self.gbasf2_setup_path,
             )
+
+            tmp_gbasf2_log_path = os.path.join(tmpdir_path, "log", self.gbasf2_project_name)
+            gbasf2_project_log_dir = os.path.join(self.log_file_dir, "gbasf2_logs", self.gbasf2_project_name)
             print(
                 f"Download of logs for gbasf2 project {self.gbasf2_project_name} successful.\n"
                 f" Moving logs to {gbasf2_project_log_dir}"
             )
             if os.path.exists(gbasf2_project_log_dir):
                 shutil.rmtree(gbasf2_project_log_dir)
             shutil.move(tmp_gbasf2_log_path, gbasf2_project_log_dir)
@@ -919,65 +890,80 @@
 
 class Gbasf2GridProjectTarget(Target):
     """
     Target exists if an output dataset for the project exists on the grid and is
     not being written to, i.e. all jobs that produced the dataset are done.
     """
 
-    def __init__(self, project_name, dirac_user=None):
+    def __init__(
+        self,
+        project_name,
+        dirac_user=None,
+        gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+    ):
         """
         :param project_name: Name of the gbasf2 grid project that produced the
             dataset and under which the dataset is stored
         :param dirac_user: Dirac user, who produced the output dataset.  When
             ``None``, the current user is used.
+        :param gbasf2_setup_path: Path to the gbasf2 setup file.
         """
         self.project_name = project_name
         self.dirac_user = dirac_user
+        self.gbasf2_setup_path = gbasf2_setup_path
 
     def exists(self):
         if not check_dataset_exists_on_grid(
-            self.project_name, dirac_user=self.dirac_user
+            self.project_name, dirac_user=self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path
         ):
             # there's no dataset associated with that name on the grid
             return False
-        if check_project_exists(self.project_name, dirac_user=self.dirac_user):
+        if check_project_exists(
+            self.project_name, dirac_user=self.dirac_user, gbasf2_setup_path=self.gbasf2_setup_path
+        ):
             # if there's data named after that project on the grid, ensure there are no jobs writig to it
             project_status_dict = get_gbasf2_project_job_status_dict(
-                self.project_name, self.dirac_user
+                gbasf2_project_name=self.project_name,
+                dirac_user=self.dirac_user,
+                gbasf2_setup_path=self.gbasf2_setup_path,
             )
             all_jobs_done = all(
                 job_info["Status"] == "Done" and job_info["ApplicationStatus"] == "Done"
                 for job_info in project_status_dict.values()
             )
             if not all_jobs_done:
                 return False
         return True
 
 
-def check_dataset_exists_on_grid(gbasf2_project_name, dirac_user=None):
-    """
-    Check if an output dataset exists for the gbasf2 project
-    """
+def check_dataset_exists_on_grid(
+    gbasf2_project_name,
+    dirac_user=None,
+    gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+):
+    """Check if an output dataset exists for the gbasf2 project."""
     output_lpn_dir = gbasf2_project_name
     group_name = get_setting("gbasf2_proxy_group", default="belle")
     if group_name != "belle":
-        output_lpn_dir = (
-            get_setting("gbasf2_project_lpn_path") + f"/{gbasf2_project_name}"
-        )
-    lpns = query_lpns(output_lpn_dir, dirac_user=dirac_user)
+        output_lpn_dir = get_setting("gbasf2_project_lpn_path") + f"/{gbasf2_project_name}"
+    lpns = query_lpns(output_lpn_dir, dirac_user=dirac_user, gbasf2_setup_path=gbasf2_setup_path)
     return len(lpns) > 0
 
 
 @retry(
     (json.decoder.JSONDecodeError, subprocess.CalledProcessError),
     tries=4,
     delay=2,
     backoff=3,  # retry after 2,6,18,108 s
 )
-def get_gbasf2_project_job_status_dict(gbasf2_project_name, dirac_user=None):
+def get_gbasf2_project_job_status_dict(
+    gbasf2_project_name,
+    dirac_user=None,
+    gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+):
     """
     Returns a dictionary for all jobs in the project with a structure like the
     following, which I have taken and adapted from an example output::
 
         {
             "<JobID>": {
                 "SubmissionTime": "2020-03-27 13:08:49",
@@ -995,53 +981,67 @@
 
     For that purpose, the script in ``gbasf2_job_status.py`` is called.  That
     script directly interfaces with Dirac via its API, but it only works with
     the gbasf2 environment and python2, which is why it is called as a
     subprocess.  The job status dictionary is passed to this function via json.
     """
     if dirac_user is None:
-        dirac_user = get_dirac_user()
+        dirac_user = get_dirac_user(gbasf2_setup_path=gbasf2_setup_path)
     job_status_script_path = os.path.join(
         os.path.dirname(os.path.realpath(__file__)), "gbasf2_utils/gbasf2_job_status.py"
     )
     group_arg = ""
     group_name = get_setting("gbasf2_proxy_group", default="belle")
     if group_name != "belle":
         group_arg = f" --group {group_name}"
     job_status_command = shlex.split(
         f"{job_status_script_path} -p {gbasf2_project_name} --user {dirac_user}{group_arg}"
     )
-    proc = run_with_gbasf2(job_status_command, capture_output=True, check=False)
+    proc = run_with_gbasf2(
+        job_status_command,
+        capture_output=True,
+        check=False,
+        gbasf2_setup_path=gbasf2_setup_path,
+    )
     # FIXME: use enum or similar to define my own return codes
     if proc.returncode == 3:  # return code 3 means project does not exist yet
         raise RuntimeError(
             f"\nCould not find any jobs for project {gbasf2_project_name} on the grid.\n"
             + "Probably there was an error during the project submission when running the gbasf2 command.\n"
         )
+    if proc.returncode > 0:
+        raise subprocess.CalledProcessError(proc.returncode, job_status_command, output=proc.stdout, stderr=proc.stderr)
     job_status_json_string = proc.stdout
     return json.loads(job_status_json_string)
 
 
-def check_project_exists(gbasf2_project_name, dirac_user=None):
-    """
-    Check if we can find the gbasf2 project on the grid with ``gb2_job_status``.
-    """
+def check_project_exists(
+    gbasf2_project_name,
+    dirac_user=None,
+    gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+):
+    """Check if we can find the gbasf2 project on the grid with ``gb2_job_status``."""
     try:
-        return bool(get_gbasf2_project_job_status_dict(gbasf2_project_name, dirac_user))
+        return bool(
+            get_gbasf2_project_job_status_dict(
+                gbasf2_project_name, dirac_user=dirac_user, gbasf2_setup_path=gbasf2_setup_path
+            )
+        )
     except RuntimeError:
         return False
 
 
 def run_with_gbasf2(
     cmd,
     *args,
     ensure_proxy_initialized=True,
     check=True,
     encoding="utf-8",
     capture_output=False,
+    gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
     **kwargs,
 ):
     """
     Call ``cmd`` in a subprocess with the gbasf2 environment.
 
     :param ensure_proxy_initialized: If this is True, check if the dirac proxy is initalized and alive and if not,
                                      initialize it.
@@ -1051,118 +1051,92 @@
     :param capture_output: Whether to capture the ``stdout`` and ``stdin``.
                            Same as setting them to in ``subprocess.PIPE``.
                            The implementation of this argument was taken from the ``subprocess.run()`` in python3.8.
     :param encoding: Encoding to use for the interpretation of the command output.
                      Different from normal subprocess commands, it by default assumes "utf-8". In that case, the returned
                      ``stdout`` and ``stderr`` are strings and not byte-strings and the user doesn't have to decode them
                      manually.
+    :param gbasf2_setup_path: Path to the gbasf2 setup file.
     :return: ``CompletedProcess`` instance
     """
     if capture_output:
         if kwargs.get("stdout") is not None or kwargs.get("stderr") is not None:
-            raise ValueError(
-                "stdout and stderr arguments may not be used " "with capture_output."
-            )
+            raise ValueError("stdout and stderr arguments may not be used " "with capture_output.")
         kwargs["stdout"] = subprocess.PIPE
         kwargs["stderr"] = subprocess.PIPE
-    gbasf2_env = get_gbasf2_env()
+
+    gbasf2_env = get_gbasf2_env(gbasf2_setup_path)
+
     if ensure_proxy_initialized:
-        setup_dirac_proxy()
-    proc = subprocess.run(
-        cmd, *args, check=check, encoding=encoding, env=gbasf2_env, **kwargs
-    )
+        setup_dirac_proxy(gbasf2_setup_path=gbasf2_setup_path)
+
+    proc = subprocess.run(cmd, *args, check=check, encoding=encoding, env=gbasf2_env, **kwargs)
     return proc
 
 
 @lru_cache(maxsize=None)
-def get_gbasf2_env(gbasf2_install_directory=None):
+def get_gbasf2_env(gbasf2_setup_path):
     """
     Return the gbasf2 environment dict which can be used to run gbasf2 commands.
 
-    :param gbasf2_install_directory: Directory into which gbasf2 has been
-        installed.  When set to the default value ``None``, it looks for the
-        value of the ``gbasf2_install_directory`` setting and when that is not
-        set, it uses the default of most installation instructions, which is
-        ``~/gbasf2KEK``.
-    :return: Dictionary containing the  environment that you get from sourcing the gbasf2 setup script.
-    """
-    if gbasf2_install_directory is None:
-        # Use the latest gbasf2 release on CVMFS as the default gbasf2 install directory.
-        # To get the directory of the latest release, take the parent of the "pro"
-        # symlink which points to a sub-directory of the latest release.
-        default_gbasf2_install_directory = os.path.realpath(
-            os.path.join("/cvmfs/belle.kek.jp/grid/gbasf2/pro", os.pardir, os.pardir)
-        )
-        gbasf2_install_directory = get_setting(
-            "gbasf2_install_directory", default=default_gbasf2_install_directory
-        )
-    gbasf2_setup_path = os.path.join(
-        gbasf2_install_directory, "BelleDIRAC/gbasf2/tools/setup.sh"
-    )
+    :param gbasf2_setup_path: Path to the gbasf2 setup file.
+    """
     if not os.path.isfile(gbasf2_setup_path):
-        raise FileNotFoundError(
-            f"Could not find gbasf2 setup file at:\n{gbasf2_setup_path}.\n"
-            f"Make sure that `gbasf2_install_directory` is set correctly. Current setting:\n{gbasf2_install_directory}.\n"
-        )
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), gbasf2_setup_path)
     # complete bash command to set up the gbasf2 environment
+    group_name = get_setting("gbasf2_proxy_group", default="belle")
     # piping output to /dev/null, because we want that our final script only prints the ``env`` output
-    gbasf2_setup_command_str = f"source {gbasf2_setup_path} > /dev/null"
+    gbasf2_setup_command_str = f"source {gbasf2_setup_path} -g {group_name} > /dev/null"
+    home = os.environ["HOME"]  # I want to run gbasf2 setup from empty env, but HOME is required
     # command to execute the gbasf2 setup command in a fresh shell and output the produced environment
     echo_gbasf2_env_command = shlex.split(
-        f"env -i bash -c '{gbasf2_setup_command_str} > /dev/null && env'"
+        f"env -i HOME='{home}' bash -c '{gbasf2_setup_command_str} > /dev/null && env'"
     )
     gbasf2_env_string = subprocess.run(
         echo_gbasf2_env_command, check=True, stdout=subprocess.PIPE, encoding="utf-8"
     ).stdout
     gbasf2_env = dict(line.split("=", 1) for line in gbasf2_env_string.splitlines())
-    # The gbasf2 setup script on sets HOME to /ext/home/ueda if it's unset,
-    # which later causes problems in the gb2_proxy_init subprocess. Therefore,
-    # reset it to the caller's HOME.
-    try:
-        gbasf2_env["HOME"] = os.environ["HOME"]
-    except KeyError:
-        pass
     return gbasf2_env
 
 
-def get_proxy_info():
+def get_proxy_info(gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc"):
     """Run ``gbasf2_proxy_info.py`` to retrieve a dict of the proxy status."""
     proxy_info_script_path = os.path.join(
         os.path.dirname(os.path.realpath(__file__)), "gbasf2_utils/gbasf2_proxy_info.py"
     )
 
     # Setting ``ensure_proxy_initialized=False`` is vital here, otherwise we get
     # an infinite loop because run_with_gbasf2 will then check for the proxy info
     proc = run_with_gbasf2(
         [proxy_info_script_path],
         capture_output=True,
         ensure_proxy_initialized=False,
+        gbasf2_setup_path=gbasf2_setup_path,
     )
     return json.loads(proc.stdout)
 
 
 @lru_cache(maxsize=None)
-def get_dirac_user():
+def get_dirac_user(gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc"):
     """Get dirac user name."""
     # ensure proxy is initialized, because get_proxy_info can't do it, otherwise
     # it causes an infinite loop
-    setup_dirac_proxy()
+    setup_dirac_proxy(gbasf2_setup_path)
     try:
-        return get_proxy_info()["username"]
+        proxy_info = get_proxy_info(gbasf2_setup_path)
+        return proxy_info["username"]
     except KeyError as err:
-        raise RuntimeError(
-            "Could not obtain dirac user name from `gb2_proxy_init` output."
-        ) from err
+        raise RuntimeError("Could not obtain dirac user name from `gb2_proxy_init` output.") from err
 
 
-def setup_dirac_proxy():
+def setup_dirac_proxy(gbasf2_setup_path="/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc"):
     """Run ``gb2_proxy_init -g belle`` if there's no active dirac proxy. If there is, do nothing."""
     # first run script to check if proxy is already alive or needs to be initalized
     try:
-        if get_proxy_info()["secondsLeft"] > 3600 * get_setting(
+        if get_proxy_info(gbasf2_setup_path)["secondsLeft"] > 3600 * get_setting(
             "gbasf2_min_proxy_lifetime", default=0
         ):
             return
     #  error is raised if proxy hasn't been initialized yet, in that case also process with initialization
     except subprocess.CalledProcessError:
         pass
 
@@ -1171,75 +1145,72 @@
     group_name = get_setting("gbasf2_proxy_group", default="belle")
     if not isinstance(lifetime, int) or lifetime <= 0:
         warnings.warn(
             "Setting 'gbasf2_proxy_lifetime' should be a positive integer.",
             RuntimeWarning,
         )
     hours = int(lifetime)
-    proxy_init_cmd = shlex.split(
-        f"gb2_proxy_init -g {group_name} -v {hours}:00 --pwstdin"
-    )
+    proxy_init_cmd = shlex.split(f"gb2_proxy_init -g {group_name} -v {hours}:00 --pwstdin")
 
     while True:
         pwd = getpass("Certificate password: ")
         try:
             proc = run_with_gbasf2(
                 proxy_init_cmd,
                 input=pwd,
                 ensure_proxy_initialized=False,
                 capture_output=True,
                 check=True,
+                gbasf2_setup_path=gbasf2_setup_path,
             )
         finally:
             del pwd
         # Check if there were any errors, since gb2_proxy_init often still exits without errorcode and sends messages to stdout
         out, err = proc.stdout, proc.stderr
-        all_output = (
-            out + err
-        )  # gb2_proxy_init errors are usually in stdout, but for future-proofing also check stderr
+        all_output = out + err  # gb2_proxy_init errors are usually in stdout, but for future-proofing also check stderr
 
         # if wrong password, retry password entry
         # usually the output then contains "Bad passphrase", but for future-proofing we check "bad pass"
         if "bad pass" in all_output.lower():
             print("Wrong certificate password, please try again.", file=sys.stderr)
             continue
 
         # for all other errors, raise an exception and abort
         # Usually for errors, the output contains the line: "Error: Operation not permitted ( 1 : )"
         if "error" in all_output.lower():
             raise subprocess.CalledProcessError(
                 returncode=errno.EPERM,
                 cmd=proxy_init_cmd,
-                output=(
-                    "There seems to be an error in the output of gb2_proxy_init."
-                    f"\nCommand output:\n{out}"
-                ),
+                output=("There seems to be an error in the output of gb2_proxy_init." f"\nCommand output:\n{out}"),
             )
         # if no  wrong password and no other errors, stop loop and return
         return
 
 
-def query_lpns(ds_query: str, dirac_user: Optional[str] = None) -> List[str]:
+def query_lpns(
+    ds_query: str,
+    dirac_user: Optional[str] = None,
+    gbasf2_setup_path: str = "/cvmfs/belle.kek.jp/grid/gbasf2/pro/bashrc",
+) -> List[str]:
     """
     Query DIRAC for LPNs matching query, and return them as a list.
 
     This function exists to avoid manual string parsing of ``gb2_ds_list``.
     """
     if dirac_user is None:
-        dirac_user = get_dirac_user()
+        dirac_user = get_dirac_user(gbasf2_setup_path=gbasf2_setup_path)
 
-    ds_list_script_path = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "gbasf2_utils/gbasf2_ds_list.py"
-    )
+    ds_list_script_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "gbasf2_utils/gbasf2_ds_list.py")
 
     query_cmd = [ds_list_script_path, "--dataset", ds_query, "--user", dirac_user]
     proc = run_with_gbasf2(
         query_cmd,
         capture_output=True,
         ensure_proxy_initialized=True,
+        gbasf2_setup_path=gbasf2_setup_path,
     )
 
     lpns = json.loads(proc.stdout)
     if not isinstance(lpns, list):
         raise TypeError(
             f"Expected gbasf2 dataset query to return list, but instead the command\n{query_cmd}\n"
             + f"returned: {lpns}"
@@ -1254,17 +1225,15 @@
 
     This is done to make sure that different instances of a task with different
     luigi parameters result in different gbasf2 project names. When trying to
     redoing a task on the grid with identical parameters, rename the project
     name prefix, to ensure that you get a new project.
     """
     try:
-        gbasf2_project_name_prefix = get_setting(
-            "gbasf2_project_name_prefix", task=task
-        )
+        gbasf2_project_name_prefix = get_setting("gbasf2_project_name_prefix", task=task)
     except AttributeError as err:
         raise Exception(
             "Task can only be used with the gbasf2 batch process if it has ``gbasf2_project_name_prefix`` "
             + "as a luigi parameter, attribute or setting."
         ) from err
     # luigi interally assings a hash to a task by calling the builtin ``hash(task.task_id)``,
     # but that returns a signed integer. I prefer a hex string to get more information per character,
@@ -1333,23 +1302,18 @@
     # if dataset does not follow gbasf2 v5 convention, assume it was produced
     # with old release and does not contain duplicates
     if not all(lfn_follows_gb2v5_convention(lfn) for lfn in lfns):
         return set(lfns)
     # if it is of the gbasf v5 form, group the outputs by the substring upto the
     # reschedule number and return list of maximums of each group
     lfns = sorted(lfns, key=_get_lfn_upto_reschedule_number)
-    return {
-        max(lfn_group)
-        for _, lfn_group in groupby(lfns, key=_get_lfn_upto_reschedule_number)
-    }
+    return {max(lfn_group) for _, lfn_group in groupby(lfns, key=_get_lfn_upto_reschedule_number)}
 
 
-def _move_downloaded_dataset_to_output_dir(
-    project_download_path: str, output_path: str
-) -> None:
+def _move_downloaded_dataset_to_output_dir(project_download_path: str, output_path: str) -> None:
     """
     Move files downloaded downloaded to the grid to their final output location.
 
     In the ``Gbasf2Process``, the outputs are usually downloaded with ``gb2_ds_get`` to
     a temporary directory (``project_download_path``)  with a structure like
 
         <result_dir>/B.root.partial/<project_name>
@@ -1409,13 +1373,11 @@
     if len(ext_split_output) == 1:
         base_stem_no_leading_dots = ext_split_output[0]
         extensions = ""
     elif len(ext_split_output) == 2:
         base_stem_no_leading_dots, extensions_no_leading_dot = ext_split_output
         extensions = "." + extensions_no_leading_dot
     else:
-        raise RuntimeError(
-            f"split_output {ext_split_output} can only contain 1 or 2 elements."
-        )
+        raise RuntimeError(f"split_output {ext_split_output} can only contain 1 or 2 elements.")
     base_stem = leading_dots + base_stem_no_leading_dots
     stem = os.path.join(dirname, base_stem)
     return stem, extensions
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py` & `b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_ds_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Script to run as subprocess in a gbasf2 environment (with ``run_with_gbasf``) to
 list LFNs. If successful, prints matched LFNs as a list in JSON format.
 """
 
 from __future__ import print_function
 
 import argparse
 import json
 import sys
 
-from BelleDIRAC.Client.helpers.auth import userCreds
+from BelleDIRAC.gbasf2.lib.auth import userCreds
+from BelleDIRAC.Client.helpers.common import initializeCS
 from BelleDIRAC.gbasf2.lib.ds.manager import Manager
 
 
 @userCreds
 def get_lfns(dataset, user):
     """
     If successful, returns a list of matched LFNs.
@@ -29,9 +30,10 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--dataset", help="Dataset query.")
     parser.add_argument("--user", help="DIRAC username.")
     args = parser.parse_args()
+    initializeCS()
     lfns = get_lfns(args.dataset, args.user)
     print(json.dumps(lfns))
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py` & `b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_job_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python3
 
 """
 Script that calls gbasf/Dirac API dictionary with status and other information
 on all jobs in a project.  If executed, outputs the information as json.  Can
 only be executed in a gbasf2 environment with python2.  It is therefore called
 by the gbasf2 batch process in a subprocess with the correct environment.
 
@@ -11,17 +11,30 @@
 """
 from __future__ import print_function
 
 import argparse
 import os
 import json
 import sys
+import datetime
 
 from BelleDIRAC.gbasf2.lib.job.information_collector import InformationCollector
-from BelleDIRAC.Client.helpers.auth import userCreds
+from BelleDIRAC.gbasf2.lib.auth import userCreds
+from BelleDIRAC.Client.helpers.common import initializeCS
+
+
+class JobStatusEncoder(json.JSONEncoder):
+    """
+    JSON encoder for data structures that can be returned by the job status information collector.
+    """
+
+    def default(self, obj):
+        if isinstance(obj, (datetime.date, datetime.datetime)):
+            return obj.isoformat()
+        return json.JSONEncoder.default(self, obj)
 
 
 @userCreds
 def get_job_status_dict(project_name, user_name, group_name):
     """
     If successful, returns a dictionary for all jobs in the project with a structure like the following,
     which I have taken and adapted from an example output::
@@ -40,28 +53,28 @@
             }
         ...
         }
     """
     if user_name is None:
         user_name = os.getenv("BELLE2_USER")
     login = [user_name, group_name]
-    newer_than = '1970-01-01'
+    newer_than = "1970-01-01"
     projects = [project_name]
     info_collector = InformationCollector()
-    result = info_collector.getAllJobsInProjects(
-        projects, date=newer_than, login=login, statuses={'Status': ['all']})
-    project_items = result['Value'][projects[0]]
+    result = info_collector.getAllJobsInProjects(projects, date=newer_than, login=login, statuses={"Status": ["all"]})
+    project_items = result["Value"][projects[0]]
     status = info_collector.getJobSummary(project_items)
-    if not status['OK']:
+    if not status["OK"]:
         # info_collector returned with False status, probably means project does not exist
         raise sys.exit(3)
-    return status['Value']
+    return status["Value"]
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument('-p', '--project', type=str, required=True, help="gbasf2 project name")
-    parser.add_argument('-u', '--user', type=str, default=None, help="grid username")
-    parser.add_argument('-g', '--group', type=str, default="belle", help="gbasf2 group name")
+    parser.add_argument("-p", "--project", type=str, required=True, help="gbasf2 project name")
+    parser.add_argument("-u", "--user", type=str, default=None, help="grid username")
+    parser.add_argument("-g", "--group", type=str, default="belle", help="gbasf2 group name")
     args = parser.parse_args()
+    initializeCS()
     job_status_dict = get_job_status_dict(args.project, args.user, args.group)
-    print(json.dumps(job_status_dict))
+    print(json.dumps(job_status_dict, cls=JobStatusEncoder))
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py` & `b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/gbasf2_proxy_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python3
 
 """
 Script to run as subprocess in a gbasf2 environment (with ``run_with_gbasf``) to
 query the proxy status. If successful, prints proxy info in JSON format.
 """
 
 from __future__ import print_function
@@ -19,15 +19,17 @@
 class CertEncoder(json.JSONEncoder):
     """
     JSON encoder for data structures possibly including certificate objects.
     """
 
     def default(self, obj):
         if isinstance(obj, X509Chain):
-            return obj.dumpAllToString()
+            x509_dict = obj.dumpAllToString()
+            x509_dict["Value"] = x509_dict["Value"].decode()
+            return x509_dict
         return json.JSONEncoder.default(self, obj)
 
 
 if __name__ == "__main__":
     # Suppress error messages, since stdout of this script is expected to be in JSON format
     gLogger.setLevel("FATAL")
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py` & `b2luigi-1.0.0/b2luigi/batch/processes/gbasf2_utils/pickle_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pickle
 
-from basf2 import conditions as b2conditions
+from basf2 import conditions as b2conditions, logging
 from basf2.pickle_path import serialize_path
 from variables import variables as vm
 
 
 def get_alias_dict_from_variable_manager():
     """
     Extracts a dictionary with the alias names as keys and their values from the
@@ -12,25 +12,26 @@
     """
     alias_dictionary = {str(alias_name): vm.getVariable(str(alias_name)).name for alias_name in vm.getAliasNames()}
     return alias_dictionary
 
 
 def write_path_and_state_to_file(basf2_path, file_path):
     """
-    Serialize basf2 path and variables from variable manager to file.
+    Serialize basf2 path, aliases and log_level to file.
 
     Variant of ``basf2.pickle_path.write_path_to_file``, only with additional
     serialization of the basf2 variable aliases and global tags.
 
     The aliases are extracted from the current state of the variable manager singleton
     and thus have to be added in the python/basf2 process before calling this function.
     Likewise for the global tags.
 
     :param path: Basf2 path object to serialize
     :param file_path: File path to write the serialized pickle object to.
     """
-    with open(file_path, 'bw') as pickle_file:
+    with open(file_path, "bw") as pickle_file:
         serialized = serialize_path(basf2_path)
         serialized["aliases"] = get_alias_dict_from_variable_manager()
         serialized["globaltags"] = b2conditions.globaltags
+        serialized["log_level"] = logging.log_level
         # serialized["conditions"] = b2conditions
         pickle.dump(serialized, pickle_file)
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/htcondor.py` & `b2luigi-1.0.0/b2luigi/batch/processes/htcondor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from b2luigi.batch.processes import BatchProcess, JobStatus
 from b2luigi.batch.cache import BatchJobStatusCache
 from b2luigi.core.utils import get_log_file_dir, get_task_file_dir
 from b2luigi.core.executable import create_executable_wrapper
 
 
 class HTCondorJobStatusCache(BatchJobStatusCache):
-
     @retry(subprocess.CalledProcessError, tries=3, delay=2, backoff=3)  # retry after 2,6,18 seconds
     def _ask_for_job_status(self, job_id: int = None):
         """
         With HTCondor, you can check the progress of your jobs using the `condor_q` command.
         If no `JobId` is given as argument, this command shows you the status of all queued jobs
         (usually only your own by default).
 
@@ -49,15 +48,23 @@
             output = subprocess.check_output(q_cmd)
 
         seen_ids = self._fill_from_output(output)
 
         # If the specified job can not be found in the condor_q output, we need to request its history
         if job_id and job_id not in seen_ids:
             # https://htcondor.readthedocs.io/en/latest/man-pages/condor_history.html
-            history_cmd = ["condor_history", "-json", "-attributes", "ClusterId,JobStatus,ExitCode", "-match", "1", str(job_id)]
+            history_cmd = [
+                "condor_history",
+                "-json",
+                "-attributes",
+                "ClusterId,JobStatus,ExitCode",
+                "-match",
+                "1",
+                str(job_id),
+            ]
             output = subprocess.check_output(history_cmd)
 
             self._fill_from_output(output)
 
     def _fill_from_output(self, output):
         output = output.decode()
 
@@ -77,14 +84,15 @@
         return seen_ids
 
 
 class HTCondorJobStatus(enum.IntEnum):
     """
     See https://htcondor.readthedocs.io/en/latest/classad-attributes/job-classad-attributes.html
     """
+
     idle = 1
     running = 2
     removed = 3
     completed = 4
     held = 5
     transferring_output = 6
     suspended = 7
@@ -127,15 +135,15 @@
 
     * Via the ``htcondor_settings`` setting you can provide a dict as
       a for additional options, such as requested memory etc. Its value has to be a dictionary
       containing HTCondor settings as key/value pairs. These options will be written into the job
       submission file. For an overview of possible settings refer to the `HTCondor documentation
       <https://htcondor.readthedocs.io/en/latest/users-manual/submitting-a-job.html#>`_.
 
-    * Same as for the :ref:`LSF`, the ``job_name`` setting allows giving a meaningful name to a
+    * Same as for the :ref:`lsf`, the ``job_name`` setting allows giving a meaningful name to a
       group of jobs. If you want to be htcondor-specific, you can provide the ``JobBatchName`` as an
       entry in the ``htcondor_settings`` dict, which will override the global ``job_name`` setting.
       This is useful for manually checking the status of specific jobs with
 
       .. code-block:: bash
 
         condor_q -batch <job name>
@@ -158,16 +166,20 @@
         try:
             job_status = _batch_job_status_cache[self._batch_job_id]
         except KeyError:
             return JobStatus.aborted
 
         if job_status in [HTCondorJobStatus.completed]:
             return JobStatus.successful
-        if job_status in [HTCondorJobStatus.idle, HTCondorJobStatus.running, HTCondorJobStatus.transferring_output,
-                          HTCondorJobStatus.suspended]:
+        if job_status in [
+            HTCondorJobStatus.idle,
+            HTCondorJobStatus.running,
+            HTCondorJobStatus.transferring_output,
+            HTCondorJobStatus.suspended,
+        ]:
             return JobStatus.running
         if job_status in [HTCondorJobStatus.removed, HTCondorJobStatus.held, HTCondorJobStatus.failed]:
             return JobStatus.aborted
         raise ValueError(f"Unknown HTCondor Job status: {job_status}")
 
     def start_job(self):
         submit_file = self._create_htcondor_submit_file()
@@ -179,15 +191,15 @@
         output = output.decode()
         match = re.search(r"[0-9]+\.", output)
         if not match:
             raise RuntimeError("Batch submission failed with output " + output)
 
         self._batch_job_id = int(match.group(0)[:-1])
 
-    def kill_job(self):
+    def terminate_job(self):
         if not self._batch_job_id:
             return
 
         subprocess.run(["condor_rm", str(self._batch_job_id)], stdout=subprocess.DEVNULL)
 
     def _create_htcondor_submit_file(self):
         submit_file_content = []
@@ -226,16 +238,16 @@
             general_settings.setdefault("when_to_transfer_output", "ON_EXIT")
 
             transfer_files = set(transfer_files)
 
             for transfer_file in transfer_files:
                 if os.path.abspath(transfer_file) != transfer_file:
                     raise ValueError(
-                        "You should only give absolute file names in transfer_files!" +
-                        f"{os.path.abspath(transfer_file)} != {transfer_file}"
+                        "You should only give absolute file names in transfer_files!"
+                        + f"{os.path.abspath(transfer_file)} != {transfer_file}"
                     )
 
             env_setup_script = get_setting("env_script", task=self.task, default="")
             if env_setup_script:
                 # TODO: make sure to call it relatively
                 transfer_files.add(os.path.abspath(env_setup_script))
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/lsf.py` & `b2luigi-1.0.0/b2luigi/batch/processes/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from b2luigi.batch.cache import BatchJobStatusCache
 from b2luigi.core.utils import get_log_file_dir
 from b2luigi.core.executable import create_executable_wrapper
 from b2luigi.core.settings import get_setting
 
 
 class LSFJobStatusCache(BatchJobStatusCache):
-
     def _ask_for_job_status(self, job_id=None):
         if job_id:
             output = subprocess.check_output(["bjobs", "-json", "-o", "jobid stat", str(job_id)])
         else:
             output = subprocess.check_output(["bjobs", "-json", "-o", "jobid stat"])
         output = output.decode()
         output = json.loads(output)["RECORDS"]
@@ -108,12 +107,12 @@
         # Output of the form Job <72065926> is submitted to default queue <s>.
         match = re.search(r"<[0-9]+>", output)
         if not match:
             raise RuntimeError("Batch submission failed with output " + output)
 
         self._batch_job_id = match.group(0)[1:-1]
 
-    def kill_job(self):
+    def terminate_job(self):
         if not self._batch_job_id:
             return
 
         subprocess.run(["bkill", self._batch_job_id], stdout=subprocess.DEVNULL, check=False)
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2` & `b2luigi-1.0.0/b2luigi/batch/processes/templates/gbasf2_steering_file_wrapper.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,31 @@
     with open(file_path, 'br') as pickle_file:
         serialized = pickle.load(pickle_file)
     try:
         basf2.conditions.globaltags += serialized["globaltags"]
     except KeyError:
         pass
 
+def set_log_level_from_file(file_path):
+    """
+    Extract and set global basf2 log level from pickle file.
+    """
+    with open(file_path, 'br') as pickle_file:
+        serialized = pickle.load(pickle_file)
+    try:
+        basf2.set_log_level(serialized["log_level"])
+    except KeyError:
+        pass
 
 pickle_file_path = "{{ pickle_file_path }}"
 if not os.path.isfile(pickle_file_path):
     raise FileNotFoundError(f"No pickle file found in {pickle_file_path}")
 
 apply_alias_dict_from_file(pickle_file_path)
 get_global_tags_from_file(pickle_file_path)
+set_log_level_from_file(pickle_file_path)
+
 path = b2pp.get_path_from_file(pickle_file_path)
 
 basf2.print_path(path)
 basf2.process(path, max_event={{ max_event }})
 print(basf2.statistics)
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/processes/test.py` & `b2luigi-1.0.0/b2luigi/batch/processes/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         executable_file = create_executable_wrapper(self.task)
 
         with open(stdout_log_file, "w") as stdout_file:
             with open(stderr_log_file, "w") as stderr_file:
                 self._process = subprocess.Popen([executable_file], stdout=stdout_file, stderr=stderr_file)
 
-    def kill_job(self):
+    def terminate_job(self):
         if not self._process:
             return
 
         self._process.kill()
 
     def get_job_output(self):
         return ""
```

### Comparing `b2luigi-0.9.1/b2luigi/batch/workers.py` & `b2luigi-1.0.0/b2luigi/batch/workers.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,18 @@
             process_class = TestProcess
         elif batch_system == BatchSystems.local:
             create_output_dirs(task)
             return super()._create_task_process(task)
         else:
             raise NotImplementedError
 
-        return process_class(task=task, scheduler=self._scheduler,
-                             result_queue=self._task_result_queue, worker_timeout=self._config.timeout)
+        return process_class(
+            task=task,
+            scheduler=self._scheduler,
+            result_queue=self._task_result_queue,
+            worker_timeout=self._config.timeout,
+        )
 
 
 class SendJobWorkerSchedulerFactory(luigi.interface._WorkerSchedulerFactory):
     def create_worker(self, scheduler, worker_processes, assistant=False):
         return SendJobWorker(scheduler=scheduler, worker_processes=worker_processes, assistant=assistant)
```

### Comparing `b2luigi-0.9.1/b2luigi/cli/arguments.py` & `b2luigi-1.0.0/b2luigi/cli/arguments.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,39 +7,47 @@
     Args:
         ignore_additional_command_line_args (bool, optional, default False): Ignore additional
             command line arguments. This is useful if you want to use this function in a file
             that also does some command line parsing.
     """
     parser = argparse.ArgumentParser()
 
-    parser.add_argument("--show-output",
-                        help="Instead of running the tasks, show which output files will/are created.",
-                        action="store_true")
-    parser.add_argument("--test",
-                        help="Run the task list in test mode by printing the log directly to the screen instead"
-                             " of storing it in a file.",
-                        action="store_true")
-    parser.add_argument("--batch",
-                        help="Instead of running locally, try to submit the tasks to the batch system.",
-                        action="store_true")
-    parser.add_argument("--batch-runner",
-                        help="Expert option to mark this worker as a batch runner.",
-                        action="store_true")
-    parser.add_argument("--dry-run",
-                        help="Do not run any task but set the return value to 0, if the tasks are complete.",
-                        action="store_true")
-    parser.add_argument("--scheduler-host",
-                        help="If given, use this host as a central scheduler instead of a local one.", default="")
-    parser.add_argument("--scheduler-port",
-                        help="If given, use the port on this host as a central scheduler instead of a local one.",
-                        type=int,
-                        default=0)
+    parser.add_argument(
+        "--show-output",
+        help="Instead of running the tasks, show which output files will/are created.",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--test",
+        help="Run the task list in test mode by printing the log directly to the screen instead"
+        " of storing it in a file.",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--batch", help="Instead of running locally, try to submit the tasks to the batch system.", action="store_true"
+    )
+    parser.add_argument(
+        "--batch-runner", help="Expert option to mark this worker as a batch runner.", action="store_true"
+    )
+    parser.add_argument(
+        "--dry-run",
+        help="Do not run any task but set the return value to 0, if the tasks are complete.",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--scheduler-host", help="If given, use this host as a central scheduler instead of a local one.", default=""
+    )
+    parser.add_argument(
+        "--scheduler-port",
+        help="If given, use the port on this host as a central scheduler instead of a local one.",
+        type=int,
+        default=0,
+    )
 
-    parser.add_argument("--task-id",
-                        help="EXPERT.", default="")
+    parser.add_argument("--task-id", help="EXPERT.", default="")
 
     if not ignore_additional_command_line_args:
         args = parser.parse_args()
     else:
         args, _ = parser.parse_known_args()
 
     if (args.test or args.dry_run) and (args.scheduler_host or args.scheduler_port):
```

### Comparing `b2luigi-0.9.1/b2luigi/cli/process.py` & `b2luigi-1.0.0/b2luigi/cli/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 from b2luigi.cli import runner
 
 
 __has_run_already = False
 
 
 def process(
-        task_like_elements,
-        show_output=False,
-        dry_run=False,
-        test=False,
-        batch=False,
-        ignore_additional_command_line_args=False,
-        **kwargs
+    task_like_elements,
+    show_output=False,
+    dry_run=False,
+    test=False,
+    batch=False,
+    ignore_additional_command_line_args=False,
+    **kwargs,
 ):
     """
     Call this function in your main method to tell ``b2luigi`` where your entry
     point of the task graph is.
     It is very similar to ``luigi.build`` with some additional configuration options.
 
     Example:
         This example defines a simple task and tells ``b2luigi`` to execute it 100 times
-        with different parametes::
+        with different parametes:
 
-            import b2luigi
-            import random
+        .. code-block:: python
 
+          import b2luigi
+          import random
 
-            class MyNumberTask(b2luigi.Task):
-                some_parameter = b2luigi.Parameter()
+          class MyNumberTask(b2luigi.Task):
+              some_parameter = b2luigi.Parameter()
 
-                def output(self):
-                    return b2luigi.LocalTarget(f"results/output_file_{self.some_parameter}.txt")
+              def output(self):
+                  return b2luigi.LocalTarget(f"results/output_file_{self.some_parameter}.txt")
 
-                def run(self):
-                    random_number = random.random()
-                    with self.output().open("w") as f:
-                        f.write(f"{random_number}\\n")
+              def run(self):
+                  random_number = random.random()
+                  with self.output().open("w") as f:
+                      f.write(f"{random_number}\\n")
 
-            if __name__ == "__main__":
-                b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)])
+          if __name__ == "__main__":
+              b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)])
 
     All flag arguments can also be given as command line arguments.
     This means the call with::
 
         b2luigi.process(tasks, batch=True)
 
     is equivalent to calling the script with::
@@ -82,16 +83,15 @@
         If you need to have multiple calls, either use a :class:`b2luigi.WrapperTask`
         or two scripts.
 
     """
     # Assert, that process is only run once
     global __has_run_already
     if __has_run_already:
-        raise RuntimeError(
-            "You are not allowed to call process twice in your code!")
+        raise RuntimeError("You are not allowed to call process twice in your code!")
     __has_run_already = True
 
     # Create Task List
     if not isinstance(task_like_elements, list):
         task_list = [task_like_elements]
     else:
         task_list = task_like_elements
```

### Comparing `b2luigi-0.9.1/b2luigi/cli/runner.py` & `b2luigi-1.0.0/b2luigi/cli/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,18 @@
             except BaseException as ex:
                 task.on_failure(ex)
                 raise ex
 
             return
 
     if not found_task:
-        raise ValueError(f"The task id {task.task_id} to be executed by this batch worker "
-                         f"does not exist in the locally reproduced task graph.")
+        raise ValueError(
+            f"The task id {cli_args.task_id} to be executed by this batch worker "
+            f"does not exist in the locally reproduced task graph."
+        )
 
 
 def run_batched(task_list, cli_args, kwargs):
     run_luigi(task_list, cli_args, kwargs)
 
 
 def run_local(task_list, cli_args, kwargs):
@@ -100,15 +102,15 @@
     non_completed_tasks = 0
     for task_class in sorted(nonfinished_task_list):
         print(task_class)
         for task in nonfinished_task_list[task_class]:
             print("\tWould run", task)
 
             # execute the dry_run method of the task if it is implemented
-            if hasattr(task, 'dry_run'):
+            if hasattr(task, "dry_run"):
                 print("\tcall: dry_run()")
                 task.dry_run()
             print()
 
             non_completed_tasks += 1
 
     if non_completed_tasks:
```

### Comparing `b2luigi-0.9.1/b2luigi/core/dispatchable_task.py` & `b2luigi-1.0.0/b2luigi/core/dispatchable_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,32 +16,34 @@
 
     Example:
         The run function can include any code you want. When the task runs,
         it is started in a subprocess and monitored by the parent process.
         When it dies unexpectedly (e.g. because of a segfault etc.)
         the task will be marked as failed. If not, it is successful.
         The log output will be written to two files in the log folder (marked with
-        the parameters of the task), which you can check afterwards::
+        the parameters of the task), which you can check afterwards:
 
-            import b2luigi
+        .. code-block:: python
 
-            class MyTask(b2luigi.Task):
-                @b2luigi.dispatch
-                def run(self):
-                    call_some_evil_function()
+          import b2luigi
+
+          class MyTask(b2luigi.Task):
+              @b2luigi.dispatch
+              def run(self):
+                  call_some_evil_function()
 
     Note:
         We are reusing the batch system implementation here, with all its settings
         and nobs to setup the environment etc.
         If you want to control it in more detail, please check out :ref:`batch-label`.
 
     Implementation note:
         In the subprocess we are calling the current executable (which should by python)
         with the current input file as a parameter, but let it only run this
-        specific task (by handing over the task id and the `--batch-worker` option).
+        specific task (by handing over the task id and the ``--batch-worker`` option).
         The run function notices this and actually runs the task instead of dispatching again.
 
     Additionally, you can add a ``cmd_prefix`` parameter to your class, which also
     needs to be a list of strings, which are prefixed to the current command (e.g.
     if you want to add a profiler to all your tasks).
     """
```

### Comparing `b2luigi-0.9.1/b2luigi/core/executable.py` & `b2luigi-1.0.0/b2luigi/core/executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import os
 import stat
 import subprocess
 
 from b2luigi.core.settings import get_setting
-from b2luigi.core.utils import (add_on_failure_function, create_cmd_from_task, get_filename, get_log_file_dir,
-                                get_task_file_dir, map_folder)
+from b2luigi.core.utils import (
+    add_on_failure_function,
+    create_cmd_from_task,
+    get_filename,
+    get_log_file_dir,
+    get_task_file_dir,
+    map_folder,
+)
 
 
 def create_executable_wrapper(task):
     """
     To incorporate all settings (environment, working paths, remote or locally)
     we create an executable bash script which is called instead of the application
     and which will setup everything accordingly before doing the actual work.
@@ -32,31 +38,30 @@
         if not os.path.isfile(map_folder(env_setup_script)):
             raise FileNotFoundError(f"Environment setup script {env_setup_script} does not exist.")
         executable_wrapper_content.append(f"source {env_setup_script}")
 
     # (b) Now override with any environment from the task or settings
     env_overrides = get_setting("env", task=task, default={})
     for key, value in env_overrides.items():
-        value = value.replace("'", "'\''")
+        value = value.replace("'", "'''")
         value = f"'{value}'"
         executable_wrapper_content.append(f"export {key}={value}")
 
     executable_wrapper_content.append("echo 'Current environment:'; env")
 
     # 3. Third part is to call the actual program
     command = " ".join(create_cmd_from_task(task))
     executable_wrapper_content.append("echo 'Will now execute the program'")
     executable_wrapper_content.append(f"exec {command}")
 
     # Now we can write the file
     executable_file_dir = get_task_file_dir(task)
     os.makedirs(executable_file_dir, exist_ok=True)
 
-    executable_wrapper_path = os.path.join(
-        executable_file_dir, "executable_wrapper.sh")
+    executable_wrapper_path = os.path.join(executable_file_dir, "executable_wrapper.sh")
 
     with open(executable_wrapper_path, "w") as f:
         f.write("\n".join(executable_wrapper_content))
 
     # make wrapper executable
     st = os.stat(executable_wrapper_path)
     os.chmod(executable_wrapper_path, st.st_mode | stat.S_IEXEC)
@@ -77,12 +82,11 @@
 
     executable_file = create_executable_wrapper(task)
 
     add_on_failure_function(task)
 
     with open(stdout_log_file, "w") as stdout_file:
         with open(stderr_log_file, "w") as stderr_file:
-            return_code = subprocess.call([executable_file],
-                                          stdout=stdout_file, stderr=stderr_file)
+            return_code = subprocess.call([executable_file], stdout=stdout_file, stderr=stderr_file)
 
     if return_code:
         raise RuntimeError(f"Execution failed with return code {return_code}")
```

### Comparing `b2luigi-0.9.1/b2luigi/core/parameter.py` & `b2luigi-1.0.0/b2luigi/core/parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     function should take one input, the value of the parameter. It is up
     to the user to ensure a unique string is created from the input.
 
     This is especially useful when you have list, string or dict parameters,
     where the resulting file path may include "/" or "{}".
     """
     import b2luigi
+
     parameter_class = b2luigi.Parameter
 
     def serialize_hashed(self, x):
         if self.hash_function is None:
             return "hashed_" + hashlib.md5(str(x).encode()).hexdigest()
         else:
             return self.hash_function(x)
@@ -33,23 +34,23 @@
     old_init = parameter_class.__init__
 
     def __init__(self, hashed=False, hash_function=None, *args, **kwargs):
         old_init(self, *args, **kwargs)
 
         if hash_function is not None:
             n_params = len(signature(hash_function).parameters)
-            assert n_params == 1, "Custom hash function can have only"\
-                f" 1 argument, found {n_params}"
+            assert n_params == 1, "Custom hash function can have only" f" 1 argument, found {n_params}"
 
         self.hash_function = hash_function
 
         if hashed:
             self.serialize_hashed = lambda x: serialize_hashed(self, x)
 
     parameter_class.__init__ = __init__
 
 
 class BoolParameter(luigi.BoolParameter):
     """Copied BoolParameter without default value"""
+
     def __init__(self, **kwargs):
         kwargs.setdefault("default", _no_value)
         luigi.Parameter.__init__(self, **kwargs)
```

### Comparing `b2luigi-0.9.1/b2luigi/core/settings.py` & `b2luigi-1.0.0/b2luigi/core/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,10 +162,12 @@
 
 
 class DeprecatedSettingsWarning(DeprecationWarning):
     pass
 
 
 def _warn_deprecated_setting(setting_name, new_name):
-    warnings.warn(f"The setting with the name {setting_name} is deprecated. "
-                  f"Please use {new_name} instead. Future versions might remove this setting.",
-                  DeprecatedSettingsWarning)
+    warnings.warn(
+        f"The setting with the name {setting_name} is deprecated. "
+        f"Please use {new_name} instead. Future versions might remove this setting.",
+        DeprecatedSettingsWarning,
+    )
```

### Comparing `b2luigi-0.9.1/b2luigi/core/task.py` & `b2luigi-1.0.0/b2luigi/core/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     """
     Drop in replacement for ``luigi.Task`` which is 100% API compatible.
     It just adds some useful methods for handling output file name generation using
     the parameters of the task.
     See :ref:`quick-start-label` on information on how to use the methods.
 
     Example:
+
         .. code-block:: python
 
           class MyAverageTask(b2luigi.Task):
               def requires(self):
                   for i in range(100):
                       yield self.clone(MyNumberTask, some_parameter=i)
 
@@ -36,31 +37,33 @@
 
                   with self.get_output_file("average.txt").open("w") as f:
                       f.write(f"{average}\\n")
     """
 
     def add_to_output(self, output_file_name):
         """
-        Call this in your output() function to add a target to the list of files,
+        Call this in your ``output()`` function to add a target to the list of files,
         this task will output.
-        Always use in combination with `yield`.
+        Always use in combination with ``yield``.
         This function will automatically add all current parameter values to
-        the file name when used in the form
+        the file name when used in the form::
 
-            result_dir/param_1=value/param_2=value/output_file_name
+            <result-path>/param1=value1/param2=value2/.../<output-file-name.ext>
 
         This function will automatically use a ``LocalTarget``.
         If you do not want this, you can override the :obj:`_get_output_file_target` function.
 
         Example:
-            This adds two files called ``some_file.txt`` and ``some_other_file.txt`` to the output::
+            This adds two files called ``some_file.txt`` and ``some_other_file.txt`` to the output:
 
-                def output(self):
-                    yield self.add_to_output("some_file.txt")
-                    yield self.add_to_output("some_other_file.txt")
+            .. code-block:: python
+
+              def output(self):
+                  yield self.add_to_output("some_file.txt")
+                  yield self.add_to_output("some_other_file.txt")
 
         Args:
             output_file_name (:obj:`str`): the file name of the output file.
                 Refer to this file name as a key when using :obj:`get_input_file_names`,
                 :obj:`get_output_file_names` or :obj:`get_output_file`.
         """
         return {output_file_name: self._get_output_file_target(output_file_name)}
@@ -75,18 +78,22 @@
         return file_paths
 
     def get_all_input_file_names(self):
         """
         Return all file paths required by this task.
 
         Example:
-            class TheSuperFancyTask(b2luigi.Task):
-                def dry_run(self):
-                    for name in self.get_all_output_file_names():
-                        print(f"\t\toutput:\t{name}")
+
+            .. code-block:: python
+
+              class TheSuperFancyTask(b2luigi.Task):
+                  def dry_run(self):
+                      for name in self.get_all_output_file_names():
+                          print(f"\t\toutput:\t{name}")
+
         """
         for file_names in self._transform_input(self.input()).values():
             for file_name in file_names:
                 yield file_name
 
     def get_input_file_names(self, key=None):
         """
@@ -107,14 +114,15 @@
         """
         Get a dictionary of input file names of the tasks, which are defined in our requirements.
 
         The requirement method should return a dict whose values are generator expressions (!)
         yielding required task objects.
 
         Example:
+
             .. code-block:: python
 
               class TaskB(luigi.Task):
 
                   def requires(self):
                       return {
                           "a": (TaskA(5.0, i) for i in range(100)),
@@ -134,17 +142,16 @@
                           result_b,
                           self.get_output_file_name("combined_results.txt")
                       )
 
                   def output(self):
                       yield self.add_to_output("combined_results.txt")
 
-
-            Either use the key argument or dictionary indexing with the key given to :obj:`add_to_output`
-            to get back a list (!) of file paths.
+        Either use the key argument or dictionary indexing with the key given to :obj:`add_to_output`
+        to get back a list (!) of file paths.
 
         Args:
             requirement_key (:obj:`str`): Specifies the required task expression.
             key (:obj:`str`, optional): If given, only return a list of file paths with this given key.
 
         Return:
             If key is none, returns a dictionary of keys to list of file paths.
@@ -162,18 +169,21 @@
         return file_paths
 
     def get_all_output_file_names(self):
         """
         Return all file paths created by this task.
 
         Example:
-            class TheSuperFancyTask(b2luigi.Task):
-                def dry_run(self):
-                    for name in self.get_all_output_file_names():
-                        print(f"\t\toutput:\t{name}")
+
+            .. code-block:: python
+
+              class TheSuperFancyTask(b2luigi.Task):
+                  def dry_run(self):
+                      for name in self.get_all_output_file_names():
+                          print(f"\t\toutput:\t{name}")
         """
         for file_names in self._transform_output(self.output()).values():
             for file_name in file_names:
                 yield file_name
 
     def get_output_file_name(self, key):
         """
@@ -208,19 +218,21 @@
     def _get_output_file_target(self, base_filename, **kwargs):
         file_name = create_output_file_name(self, base_filename, **kwargs)
         return luigi.LocalTarget(file_name)
 
 
 class ExternalTask(Task, luigi.ExternalTask):
     """Direct copy of :obj:`luigi.ExternalTask`, but with the capabilities of :obj:`Task` added."""
+
     pass
 
 
 class WrapperTask(Task, luigi.WrapperTask):
     """Direct copy of :obj:`luigi.WrapperTask`, but with the capabilities of :obj:`Task` added."""
+
     pass
 
 
 class NotCompletedTask(Task):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `b2luigi-0.9.1/b2luigi/core/temporary_wrapper.py` & `b2luigi-1.0.0/b2luigi/core/temporary_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,55 +28,57 @@
         self._task.get_output_file_name = self._task_output_function
 
 
 def on_temporary_files(run_function):
     """
     Wrapper for decorating a task's run function to use temporary files as outputs.
 
-    A common problem when using long running tasks in luigi is the so called thanksgiving bug
+    A common problem when using long running tasks in ``luigi`` is the so called thanksgiving bug
     (see https://www.arashrouhani.com/luigi-budapest-bi-oct-2015/#/21).
     It occurs, when you define an output of a task and in its run function,
     you create this output before filling it with content
     (maybe even only after a long lasting calculation).
     It may happen, that during the creation of the output and the finish of the calculation
     some other tasks checks if the output is already there, finds it and assumes,
     that the task is already finished (although there is probably only non-sense in the file
     so far).
 
-    A solution is already given by luigi itself, when using the temporary_path() function
+    A solution is already given by luigi itself, when using the ``temporary_path()`` function
     of the file system targets, which is really nice!
     Unfortunately, this means you have to open all your output files with a context manager
     and this is very hard to do if you have external tasks also (because they will
     probably use the output file directly instead of the temporary file version of if).
 
-    This wrapper simplifies the usage of the temporary files::
+    This wrapper simplifies the usage of the temporary files:
 
-        import b2luigi
+    .. code-block:: python
 
-        class MyTask(b2luigi.Task):
-            def output(self):
-                yield self.add_to_output("test.txt")
-
-            @b2luigi.on_temporary_files
-            def run(self):
-                with open(self.get_output_file_name("test.txt"), "w") as f:
-                    raise ValueError()
-                    f.write("Test")
+      import b2luigi
+
+      class MyTask(b2luigi.Task):
+          def output(self):
+              yield self.add_to_output("test.txt")
+
+          @b2luigi.on_temporary_files
+          def run(self):
+              with open(self.get_output_file_name("test.txt"), "w") as f:
+                  raise ValueError()
+                  f.write("Test")
 
     Instead of creating the file "test.txt" at the beginning and filling it with content
     later (which will never happen because of the exception thrown, which makes the file
     existing but the task actually not finished), the file will be written to a temporary
     file first and copied to its final location at the end of the run function (but only if there
     was no error).
 
-    *Attention*:
-
-    The decorator only edits the function get_output_file_name. If you are using
-    the output directly, you have to take care of using the temporary path correctly by yourself!
+    Warning:
+        The decorator only edits the function :meth:`b2luigi.Task.get_output_file_name`. If you are using
+        the output directly, you have to take care of using the temporary path correctly by yourself!
 
     """
+
     @wraps(run_function)
     def run(self):
         with TemporaryFileContextManager(self):
             run_function(self)
 
     return run
```

### Comparing `b2luigi-0.9.1/b2luigi/core/utils.py` & `b2luigi-1.0.0/b2luigi/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import importlib
 
 import itertools
 import os
 import collections
 import sys
 import types
-import warnings
 
 import colorama
 
 from b2luigi.core.settings import get_setting
 
 
 @contextlib.contextmanager
@@ -91,16 +90,17 @@
 
     try:
         return inputs.path
     except AttributeError:
         pass
 
     if isinstance(inputs, dict):
-        return {os.path.basename(flatten_to_file_paths(key)):
-                flatten_to_file_paths(value) for key, value in inputs.items()}
+        return {
+            os.path.basename(flatten_to_file_paths(key)): flatten_to_file_paths(value) for key, value in inputs.items()
+        }
     if isinstance(inputs, list):
         return [flatten_to_file_paths(value) for value in inputs]
     return inputs
 
 
 def flatten_to_dict(inputs):
     """
@@ -171,17 +171,21 @@
         if not output_dict:
             continue
 
         for target_key, target in output_dict.items():
             converted_dict = flatten_to_file_paths({target_key: target})
             file_key, file_name = converted_dict.popitem()
 
-            all_output_files[file_key].append(dict(exists=target.exists(),
-                                                   parameters=get_serialized_parameters(task),
-                                                   file_name=os.path.abspath(file_name)))
+            all_output_files[file_key].append(
+                dict(
+                    exists=target.exists(),
+                    parameters=get_serialized_parameters(task),
+                    file_name=os.path.abspath(file_name),
+                )
+            )
 
     return all_output_files
 
 
 def filter_from_params(output_files, **kwargs):
     kwargs_list = fill_kwargs_with_lists(**kwargs)
 
@@ -241,50 +245,54 @@
     serialized_parameters = get_serialized_parameters(task)
 
     if not result_dir:
         # Be sure to evaluate things relative to the current executed file, not to where we are now
         result_dir = map_folder(get_setting("result_dir", task=task, default=".", deprecated_keys=["result_path"]))
 
     for key, value in serialized_parameters.items():
-        if isinstance(key, str) and "/" in value:
-            warnings.warn(f"Value of parameter ``{key}`` contains forward slash \"/\". "
-                          "This will result in an additional subdirectory in the output path. "
-                          "Consider using a hashed parameter (e.g. ``b2luigi.Parameter(hashed=True)``)")
+        # Raise error if parameter value contains path separator "/" ("\" on Windows)
+        # or is not interpretable as basename due to other reasons.
+        if value != os.path.basename(value):
+            raise ValueError(
+                f"Parameter `{key}={value}` cannot be interpreted as directory name. "
+                f"Make sure it does not contain the path separators ``{os.path.sep}``. "
+                "Consider using a hashed parameter (e.g. ``b2luigi.Parameter(hashed=True)``)."
+            )
 
     param_list = [f"{key}={value}" for key, value in serialized_parameters.items()]
     output_path = os.path.join(result_dir, *param_list)
 
     return os.path.join(output_path, base_filename)
 
 
 def get_log_file_dir(task):
-    if hasattr(task, 'get_log_file_dir'):
+    if hasattr(task, "get_log_file_dir"):
         log_file_dir = task.get_log_file_dir()
         return log_file_dir
 
     # Be sure to evaluate things relative to the current executed file, not to where we are now
-    base_log_file_dir = map_folder(get_setting("log_dir", task=task, default="logs",
-                                               deprecated_keys=["log_folder"]))
+    base_log_file_dir = map_folder(get_setting("log_dir", task=task, default="logs", deprecated_keys=["log_folder"]))
     log_file_dir = create_output_file_name(task, task.get_task_family() + "/", result_dir=base_log_file_dir)
 
     return log_file_dir
 
 
 def get_task_file_dir(task):
-    if hasattr(task, 'get_task_file_dir'):
+    if hasattr(task, "get_task_file_dir"):
         task_file_dir = task.get_task_file_dir()
         return task_file_dir
 
     task_file_dir = create_output_file_name(task, task.get_task_family() + "/")
 
     return task_file_dir
 
 
 def get_filename():
     import __main__
+
     return __main__.__file__
 
 
 def map_folder(input_folder):
     if os.path.isabs(input_folder):
         return input_folder
 
@@ -342,16 +350,15 @@
 def add_on_failure_function(task):
     task.on_failure = types.MethodType(on_failure, task)
 
 
 def create_cmd_from_task(task):
     filename = os.path.basename(get_filename())
 
-    prefix = get_setting("executable_prefix", task=task, default=[],
-                         deprecated_keys=["cmd_prefix"])
+    prefix = get_setting("executable_prefix", task=task, default=[], deprecated_keys=["cmd_prefix"])
 
     if isinstance(prefix, str):
         raise ValueError("Your specified executable_prefix needs to be a list of strings, e.g. [strace]")
 
     cmd = prefix
 
     executable = get_setting("executable", task=task, default=[sys.executable])
```

### Comparing `b2luigi-0.9.1/docs/Makefile` & `b2luigi-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/docs/advanced/basf2-examples.rst` & `b2luigi-1.0.0/docs/advanced/basf2-examples.rst`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         def create_path(self):
             # somehow create filenames from parameters
             # self.experiment_number, self.run_number,
             # self.mode and self.file_number
             # (parameters just examples)
             input_file_names = ..
 
-            path = basf2.create_path()
+            path = basf2.Path()
             modularAnalysis.inputMdstList('default', input_file_names, path=path)
 
             # Now fill your particle lists, just examples
             modularAnalysis.fillParticleLists([('K+', 'kaonID > 0.1'), ('pi+', 'pionID > 0.1')],
                                               path=path)
             modularAnalysis.reconstructDecay('D0 -> K- pi+', '1.7 < M < 1.9', path=path)
             modularAnalysis.fitVertex('D0', 0.1, path=path)
```

### Comparing `b2luigi-0.9.1/docs/advanced/development.rst` & `b2luigi-1.0.0/docs/advanced/development.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 .. _development-label:
 
 Development and TODOs
 =====================
 
-You want to help developing ``b2luigi``? Great! Have your github account ready and let's go!
+You want to help developing ``b2luigi``? Great! Have your GitHub account ready and let's go!
+
+If you are a Belle II collaborator, you can contribute directly on the
+`DESY GitLab <https://gitlab.desy.de/belle2/software/b2luigi>`_.
 
 
 Local Development
 -----------------
 
 You want to help developing ``b2luigi``? Great! Here are some first steps to help you dive in:
 
-1.  Make sure you uninstall ``b2luigi`` if you have installed if from pypi
+1.  Make sure you uninstall ``b2luigi`` if you have installed if from PyPi
 
     .. code-block:: bash
 
         python -m pip uninstall b2luigi
 
-2.  Clone the repository from github
+2.  Clone the repository from GitHub
 
     .. code-block:: bash
 
-        git clone https://github.com/nils-braun/b2luigi
+        git clone https://github.com/belle2/b2luigi
+
+    or, for Belle II collaborators, clone the repository from DESY GitLab
+
+    .. code-block:: bash
+
+        git clone git@gitlab.desy.de:belle2/software/b2luigi.git
 
 3.  ``b2luigi`` is not using ``setuptools`` but the newer (and better) flit_ as a a builder.
     Install it via
 
     .. code-block:: bash
 
         python -m pip [ --user ] install flit
@@ -34,35 +43,35 @@
 
     .. code-block:: bash
 
         flit install -s
 
     Now you can start hacking and your changes will be immediately available to you.
 
-4. Install `pre-commit`_, which automatically checks your code
+4.  Install `pre-commit`_, which automatically checks your code
 
     .. code-block:: bash
 
         python -m pip [ --user ] install pre-commit
         pre-commit install  # install the pre-commit hooks
         pre-commit  # run pre-commit manually, checks all staged ("added") changes
 
-   In particular, the python files are checked with `flake8`_ for syntax and
-   `PEP 8`_ style errors. I recommend using an IDE or editor which
-   automatically highlights errors with flake8 or a similar python linter (e.g.
-   pylint).
+    In particular, the python files are checked with `flake8`_ for syntax and
+    `PEP 8`_ style errors. I recommend using an IDE or editor which
+    automatically highlights errors with flake8 or a similar python linter (e.g.
+    pylint).
 
-5. We use the unittest_ package for testing some parts of the code. All tests reside in the
-   ``tests/`` sub-directory. To run all tests, run the command
+5.  We use the unittest_ package for testing some parts of the code. All tests reside in the
+    ``tests/`` sub-directory. To run all tests, run the command
 
     .. code-block:: bash
 
         python -m unittest
 
-   in the root of ``b2luigi`` repository. If you add some functionality, try to add some tests for it.
+    in the root of ``b2luigi`` repository. If you add some functionality, try to add some tests for it.
 
 6.  The documentation is hosted on `readthedocs`_ and build automatically on every commit to main.
     You can (and should) also build the documentation locally by installing ``sphinx``
 
     .. code-block:: bash
 
         python -m pip [ --user ] install sphinx sphinx-autobuild
@@ -73,55 +82,58 @@
 
         sphinx-autobuild docs build
 
     The autobuild will rebuild the project whenever you change something. It displays a URL where to find
     the created docs now (most likely http://127.0.0.1:8000).
     Please make sure the documentation looks fine before creating a pull request.
 
-7.  Add a summary of your changes to the ``[Unreleased]`` section of the ``CHANGELOG.md``.
+7.  Add a summary of your changes to the ``[Unreleased]`` section of the ``CHANGELOG.md``,
+    following the `Keep a Changelog`_ format.
 
 8.  If you are a core developer and want to release a new version:
 
     a.  Make sure all changes are committed and merged on main
-    b.  Use the `bump2version`_ package to update the version in the python file ``b2luigi/__init__.py`` as well
+
+    b.  Change the ``[Unreleased]`` heading in the ``CHANGELOG.md`` file to the new version number and commit the change.
+        Then use the `bump-my-version`_ package to update the version in ``b2luigi/__init__.py``, ``.bumpversion.cfg``, ``docs/conf.py`` as well
         as the git tag. ``flit`` will automatically use this.
 
         .. code-block:: bash
 
-            bumpversion patch/minor/major
+            python3 -m pip install --upgrade bump-my-version
+            bump-my-version bump --no-commit [patch|minor|major]
 
     c.  Push the new commit and the tags
 
         .. code-block:: bash
 
             git push
             git push --tags
 
-    d.  Update the ``CHANGELOG.md`` following the `Keep a Changelog`_ format.
-
-    e.  Create a new `release`_ on github, with the description copied from the ``CHANGELOG.md``.
+    d.  Create a new `release`_ on GitLab, with the description copied from the ``CHANGELOG.md``.
 
-    f. Check that the new release had been published to PyPi, which should happen automatically via
-       github `actions`_. Alternatively, you can also manually publish a release via
+    e.  Check that the new release had been published to PyPi, which should happen automatically via
+        GitLab `pipeline`_. Alternatively, you can also manually publish a release via
 
         .. code-block:: bash
 
             flit publish
 
 
 Open TODOs
 ----------
 
-For a list of potential features, improvements and bugfixes see the `github issues`_. Help is
-welcome, so feel free to pick one, e.g. with the ``good first issue`` or ``help wanted`` tags.
+For the Belle II collaborators: for a list of potential features, improvements and bugfixes see the
+`GitLab issues`_. Help is welcome, so feel free to pick one, e.g. with the ``good first issue`` or
+``help wanted`` tags.
 
 .. _flit: https://pypi.org/project/flit/
-.. _github issues: https://github.com/nils-braun/b2luigi/issues
+.. _gitlab issues: https://gitlab.desy.de/belle2/software/b2luigi/-/issues
 .. _unittest: https://docs.python.org/3/library/unittest.html
 .. _readthedocs: https://readthedocs.org
 .. _pre-commit: https://pre-commit.com
 .. _flake8: https://flake8.pycqa.org
 .. _PEP 8: https://www.python.org/dev/peps/pep-0008/
-.. _bump2version: https://github.com/c4urself/bump2version
-.. _release: https://github.com/nils-braun/b2luigi/releases
-.. _actions: https://github.com/nils-braun/b2luigi/actions
+.. _bump-my-version: https://github.com/callowayproject/bump-my-version
+.. _release: https://github.com/belle2/b2luigi/releases
+.. _pipeline: https://github.com/belle2/b2luigi/blob/main/.gitlab-ci.yml
 .. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
```

### Comparing `b2luigi-0.9.1/docs/advanced/faq.rst` & `b2luigi-1.0.0/docs/advanced/faq.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 ---------------------------------------------------------------------------------
 
 ``b2luigi`` will automatically create log files for the ``stdout`` and ``stderr``
 output of a task processed on a batch system. The paths of these log files are defined
 relative to the location of the executed python file and contain the parameter of
 the task.
 In some cases one might one to specify other paths for the log files. To achieve this,
-a own :meth:`get_log_file_dir()` method of the task class must be implemented. This method
+a own ``get_log_file_dir()`` method of the task class must be implemented. This method
 must return a directory path for the stdout and the stderr files, for example:
 
 .. code-block:: python
 
-    class MyBatchTask(b2luigi.Task):
-        ...
-        def get_log_file_dir(self):
-            filename = os.path.realpath(sys.argv[0])
-            path = os.path.join(os.path.dirname(filename), "logs")
-            return path
+  class MyBatchTask(b2luigi.Task):
+      ...
+      def get_log_file_dir(self):
+          filename = os.path.realpath(sys.argv[0])
+          path = os.path.join(os.path.dirname(filename), "logs")
+          return path
 
 ``b2luigi`` will use this method if it is defined and write the log output in the respective
 files. Be careful, though, as these log files will of course be overwritten if more than one
 task receive the same paths to write to!
 
 
 Can I exclude one job from batch processing
@@ -48,25 +48,25 @@
 
 How do I handle parameter values which include "/" (or other unusual characters)?
 ---------------------------------------------------------------------------------
 
 ``b2luigi`` automatically generates the filenames for your output or log files out of
 the current tasks values in the form::
 
-    <result-path>/param1=value1/param2=value2/..../filename.ext
+    <result-path>/param1=value1/param2=value2/.../<output-file-name.ext>
 
 The values are given by the serialisation of your parameter, which is basically its string representation.
 Sometimes, this representation may include characters not suitable for their usage as a path name,
 e.g. "/".
 Especially when you use a :obj:`DictParameter` or a :obj:`ListParameter`, you might not
 want to have its value in your output.
 Also, if you have credentials in the parameter (what you should never do of course!), you do not
 want to show them to everyone.
 
-When using a parameter in `b2luigi` (or any of its derivatives), they have a new flag called ``hashed``
+When using a parameter in ``b2luigi`` (or any of its derivatives), they have a new flag called ``hashed``
 in their constructor, which makes the path creation only using a hashed version of your parameter value.
 
 For example will this task::
 
     class MyTask(b2luigi.Task):
         my_parameter = b2luigi.ListParameter(hashed=True)
```

### Comparing `b2luigi-0.9.1/docs/conf.py` & `b2luigi-1.0.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,83 +7,120 @@
 # http://www.sphinx-doc.org/en/stable/config
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
+
+import os
+import pathlib
+import sys
+
+sys.path.insert(0, pathlib.Path(__file__).parents[1].resolve().as_posix())
 
 
 # -- Project information -----------------------------------------------------
 
-import os
 
-project = 'b2luigi'
-copyright = '2018, Nils Braun'
-author = 'Nils Braun'
+def get_latest_tag():
+    """
+    Helper function thar returns the name of the tag if the latest commit is tagged,
+    otherwise it simply returns "latest"
+    """
+
+    default = "latest"
+
+    try:
+        import git
+    except ImportError:
+        print("GitPython module is not installed")
+        return default
+
+    current_directory = os.getcwd()
+
+    while True:
+        try:
+            repo = git.Repo(current_directory)
+            latest_commit = repo.head.commit
+            tags = repo.tags
+            for tag in tags:
+                if tag.commit == latest_commit:
+                    return tag.name
+            # If the latest commit has not tags, then it's the latest version
+            return default
+        except git.InvalidGitRepositoryError:
+            # No Git repository found in the current directory
+            parent_directory = os.path.dirname(current_directory)
+            # Check if we have reached the root directory: if yes, break the loop and then return
+            if parent_directory == current_directory:
+                break
+            # Move to the parent directory
+            current_directory = parent_directory
+
+    print("GitPython did not find a valid repository")
+    return default
+
+
+project = "b2luigi"
+copyright = "2018-2023, Nils Braun, Michael Eliachevitch, The Belle II Collaboration"
+author = "Nils Braun, Michael Eliachevitch, The Belle II Collaboration"
 
 # The short X.Y version
-version = ''
+_version = get_latest_tag()
+version = _version
 # The full version, including alpha/beta/rc tags
-release = '0.9.1'
+release = _version
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = [
-    "sphinx.ext.doctest",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.napoleon"
-]
+extensions = ["sphinx.ext.doctest", "sphinx.ext.autodoc", "sphinx.ext.napoleon"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_book_theme"
 
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
@@ -103,67 +140,73 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'b2luigidoc'
+htmlhelp_basename = "b2luigidoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'b2luigi.tex', 'b2luigi Documentation',
-     'Nils Braun', 'manual'),
+    (
+        master_doc,
+        "b2luigi.tex",
+        "b2luigi Documentation",
+        "Nils Braun, Michael Eliachevitch, The Belle II Collaboration",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'b2luigi', 'b2luigi Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "b2luigi", "b2luigi Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'b2luigi', 'b2luigi Documentation',
-     author, 'b2luigi', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "b2luigi",
+        "b2luigi Documentation",
+        author,
+        "b2luigi",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Cheating around read the docs: we need to install our project which is not possible because we
 # have no setup.py. But this should work...
 
 if os.getenv("READTHEDOCS"):
     import subprocess
+
     subprocess.check_call(["pip", "install", "flit"])
     subprocess.check_call(["flit", "install", "-s"], cwd="../")
```

### Comparing `b2luigi-0.9.1/docs/documentation/api.rst` & `b2luigi-1.0.0/docs/documentation/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Super-hero Task Classes
 -----------------------
 
 If you want to use the default ``luigi.Task`` class or any derivative of it,
 you are totally fine.
 No need to change any of your scripts!
 But if you want to take advantage of some of the recipies we have developed
-to work with large luigi task sets, you can use the drop in replacements
+to work with large ``luigi`` task sets, you can use the drop in replacements
 from the ``b2luigi`` package.
 All task classes (except the :class:`b2luigi.DispatchableTask`, see below) are superclasses of
 a ``luigi`` class.
 As we import ``luigi`` into ``b2luigi``, you just need to replace
 
 .. code-block:: python
```

### Comparing `b2luigi-0.9.1/docs/documentation/b2luigi.basf2_helper.rst` & `b2luigi-1.0.0/docs/documentation/b2luigi.basf2_helper.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/docs/documentation/run_modes.rst` & `b2luigi-1.0.0/docs/documentation/run_modes.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/docs/index.rst` & `b2luigi-1.0.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 b2luigi
 =======
 
 ``b2luigi`` — bringing batch 2 luigi!
 
 
-``b2luigi`` is a helper package for ``luigi`` for scheduling large luigi workflows on a batch system.
+``b2luigi`` is a helper package for ``luigi`` for scheduling large ``luigi`` workflows on a batch system.
 It is as simple as
 
 .. code-block:: python
 
     import b2luigi
 
 
@@ -34,19 +34,19 @@
     The API of ``b2luigi`` is still under construction.
     Please remember this when using the package in production!
 
 
 Why not use the already created batch tasks?
 --------------------------------------------
 
-Luigi already contains a large set of tasks for scheduling and monitoring batch jobs [1]_.
+``luigi`` already contains a large set of tasks for scheduling and monitoring batch jobs [1]_.
 But for thousands of tasks in very large projects with different task-defining libraries, you have some problems:
 
 *   **You want to run many (many many!) batch jobs in parallel**
-    In other luigi batch implementations, for every running batch job you also need a running task that monitors it.
+    In other ``luigi`` batch implementations, for every running batch job you also need a running task that monitors it.
     On most of the systems, the maximal number of processes is limited per user, so you will not be able to run more
     batch jobs than this.
     But what do you do if you have thousands of tasks to do?
 *   **You have already a large set of luigi tasks in your project**
     In other implementations you either have to override a ``work`` function (and you are not allowed to touch
     the ``run`` function) or they can only run an external command, which you need to define.
     The first approach plays not well when mixing non-batch and batch task libraries and the second
@@ -61,30 +61,30 @@
     on your submission machine.
 *   No need to rewrite your tasks! Just call them with ``b2luigi.process(.., batch=True)`` or with
     ``python file.py --batch`` and you are ready to go!
 *   Switching the batch system is just a single change in a config file or one line in python.
     In the future, there will even be an automatic discovery of the batch system to use.
 
 
-Is this the only thing I can do with b2luigi?
----------------------------------------------
+Is this the only thing I can do with ``b2luigi``?
+-------------------------------------------------
 
-As ``b2luigi`` should help you with large luigi projects, we have also included some helper functionalities for
+As ``b2luigi`` should help you with large ``luigi`` projects, we have also included some helper functionalities for
 ``luigi`` tasks and task handling.
 ``b2luigi`` task is a super-hero version of ``luigi`` task, with simpler handling for output and input files.
 Also, we give you working examples and best-practices for better data management and how to accomplish your goals,
 that we have learned with time.
 
 
 Why are you still talking, lets use it!
 ---------------------------------------
 
 Have a look into the :ref:`quick-start-label`.
 
-You can also start reading the :ref:`api-documentation-label` or the code on github_.
+You can also start reading the :ref:`api-documentation-label` or the code on GitHub_.
 
 If you find any bugs or want to improve the documentation, please send me a pull request.
 
 This project is in beta. Please be extra cautious when using in production mode.
 You can help me by working with one of the todo items described in :ref:`development-label`.
 
 Content
@@ -104,63 +104,74 @@
 
 
 The name
 --------
 
 ``b2luigi`` stands for multiple things at the same time:
 
-*   It brings **b**\ atch to (**2**\ ) luigi.
-*   It helps you with the **b**\ read and **b**\ utter work in luigi (e.g. proper data management)
+*   It brings **b**\ atch to (**2**\ ) ``luigi``.
+*   It helps you with the **b**\ read and **b**\ utter work in ``luigi`` (e.g. proper data management)
 *   It was developed for the `Belle II`_ experiment.
 
 
 The team
 --------
 
-Main developer
-    Michael Eliachevitch (`meliache`_)
+Current developer and maintainer
+    The Belle II Collaboration (`belle2`_)
 
 Original author
     Nils Braun (`nils-braun`_)
 
+Former developer and maintainer
+    Michael Eliachevitch (`meliache`_)
+
 Features, fixing, help and testing
     * Felix Metzner (`FelixMetzner`_)
     * Patrick Ecker (`eckerpatrick`_)
     * Jochen Gemmler
     * Maximilian Welsch (`welschma`_)
     * Kilian Lieret (`klieret`_)
     * Sviatoslav Bilokin (`bilokin`_)
     * Phil Grace (`philiptgrace`_)
     * Anselm Baur (`anselmbaur`_)
     * Moritz Bauer (`sognetic`_)
     * Matthias Schnepf  (`mschnepf`_)
     * Artur Gottmann (`ArturAkh`_)
     * Caspar Schmitt (`schmitca`_)
-    * Marcel Hohmann (`MarcelHoh_`)
+    * Marcel Hohmann (`MarcelHoh`_)
+    * Giacomo De Pietro (`GiacomoXT`_)
+    * Alex Heidelbach (`AlexanderHeidelbach`_)
+    * Tristan Fillinger (`0ctagon`_)
 
 Stolen ideas
     * Implementation of SGE batch system (`sge`_).
     * Implementation of LSF batch system (`lsf`_).
 
 
-.. _github: https://github.com/nils-braun/b2luigi
+.. _github: https://github.com/belle2/b2luigi
 .. _`luigi documentation`: https://luigi.readthedocs.io/en/stable
 .. _`Belle II`: https://www.belle2.org
+.. _`belle2`: https://github.com/belle2
 .. _`nils-braun`: https://github.com/nils-braun
 .. _`meliache`: https://github.com/meliache
 .. _`welschma`: https://github.com/welschma
 .. _`FelixMetzner`: https://github.com/FelixMetzner
 .. _`eckerpatrick`: https://github.com/eckerpatrick
 .. _`klieret`: https://github.com/klieret
 .. _`bilokin`: https://github.com/bilokin
 .. _`philiptgrace`: https://github.com/philiptgrace
 .. _`anselmbaur`: https://github.com/anselm-baur
 .. _`sognetic`: https://github.com/sognetic
 .. _`ArturAkh`: https://github.com/ArturAkh
 .. _`mschnepf`: https://github.com/mschnepf
 .. _`schmitca`: https://github.com/schmitca
 .. _`MarcelHoh`: https://github.com/MarcelHoh
+.. _`GiacomoXT`: https://github.com/GiacomoXT
+.. _`AlexanderHeidelbach`: https://github.com/AlexanderHeidelbach
+.. _`0ctagon`: https://github.com/0ctagon
 .. _`sge`: https://github.com/spotify/luigi/blob/master/luigi/contrib/sge.py
 .. _`lsf`: https://github.com/spotify/luigi/pull/2373/files
 
 
+
 .. [1] https://github.com/spotify/luigi/blob/master/luigi/contrib/sge.py
```

### Comparing `b2luigi-0.9.1/docs/usage/batch.rst` & `b2luigi-1.0.0/docs/usage/batch.rst`

 * *Files 1% similar despite different names*

```diff
@@ -67,37 +67,37 @@
 Different batch systems and batch systems implementations treat this fact differently.
 In the following, the basic procedure and assumption is explained.
 Any deviation from this is described in the next section.
 
 By default, ``b2luigi`` needs at least two folders to be accessible from the scheduling as well as worker machine:
 the result folder and the folder of your script(s).
 If possible, use absolute paths for the result and log directory to prevent any problems.
-Some batch systems (e.g. htcondor) support file copy mechanisms from the scheduler to the worker systems.
+Some batch systems (e.g. ``htcondor``) support file copy mechanisms from the scheduler to the worker systems.
 Please checkout the specifics below.
 
 .. hint::
 
     All relative paths given to e.g. the ``result_dir`` or the ``log_dir`` are always evaluated
     relative to the folder where your script lives.
     To prevent any disambiguities, try to use absolute paths whenever possible.
 
 Some batch system starts the job in an arbitrary folder on the workers instead of the current folder on the scheduler.
 That is why ``b2luigi`` will change the directory into the path of your called script before starting the job.
 
 In case your script is accessible from a different location on the worker than on the scheduling machine, you can give the setting ``working_dir``
 to specify where the job should run.
-Your script needs to be in this folder and every relative path (e.g. for results or log) will be evaluated from there.
+Your script needs to be in this folder and every relative path (e.g. for results or log files) will be evaluated from there.
 
 Drawbacks of the batch mode
 ---------------------------
 
 Although the batch mode has many benefits, it would be unfair to not mention its downsides:
 
 *   You have to choose the queue/batch settings/etc. depending in your requirements (e.g. wall clock time) by yourself.
-    So you need to make sure that the tasks will actually finish before the batch system kills them because of timeout.
+    So you need to make sure that the tasks will actually finish before the batch system terminates them because of timeout.
     There is just no way for ``b2luigi`` to know this beforehand.
 *   There is currently no resubmission implemented.
     This means dying jobs because of batch system failures are just dead.
     But because of the dependency checking mechanism of ``luigi`` it is simple to just redo the calculation
     and re-calculate what is missing.
 *   The ``luigi`` feature to request new dependencies while task running (via ``yield``) is not implemented for
     the batch mode so far.
@@ -105,14 +105,16 @@
 
 Batch System Specific Settings
 ------------------------------
 
 Every batch system has special settings.
 You can look them up here:
 
+.. _lsf:
+
 LSF
 ...
 
 .. autoclass:: b2luigi.batch.processes.lsf.LSFProcess
     :show-inheritance:
 
 HTCondor
@@ -130,8 +132,8 @@
 Add your own batch system
 -------------------------
 
 If you want to add a new batch system, all you need to do is to implement the
 abstract functions of ``BatchProcess`` for your system:
 
 .. autoclass:: b2luigi.batch.processes.BatchProcess
-    :members: get_job_status, start_job, kill_job
+    :members: get_job_status, start_job, terminate_job
```

### Comparing `b2luigi-0.9.1/docs/usage/installation.rst` & `b2luigi-1.0.0/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/docs/usage/quickstart.rst` & `b2luigi-1.0.0/docs/usage/quickstart.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 .. hint::
     The default batch system currently is LSF, so if you do not change it, LSF will be
     used. Check out :ref:`batch-label` for more information.
 
 Our task will be very simple: we want to create 100 files with some random number in it.
 Later, we will build the average of those numbers.
 
-1. Open a code editor and create a new file ``simple-example.py`` with the following content:
+1.  Open a code editor and create a new file ``simple-example.py`` with the following content:
 
     .. literalinclude:: ../../tests/doc_examples/simple_example.py
-       :linenos:
 
     Each building block in ``(b2)luigi`` is a :class:`b2luigi.Task`.
     It defines (which its run function), what should be done.
     A task can have parameters, as in our case the ``some_parameter`` defined in line 6.
     Each task needs to define, what it will output in its ``output`` function.
 
     .. note::
@@ -102,15 +101,14 @@
     which will also help you ordering your files at no cost.
     This is especially useful in larger projects, when many people are defining and executing tasks.
 
     This code listing shows the same task, but this time written using the helper
     functions given by ``b2luigi``.
 
     .. literalinclude:: ../../tests/doc_examples/simple_example_b2luigi.py
-       :linenos:
 
     Before continuing, remove the output of the former calculation.
 
     .. code-block:: bash
 
         rm -rf results
 
@@ -118,23 +116,23 @@
 
     .. code-block:: bash
 
         python simple-example.py --batch
 
     you are basically doing the same as before, with some very nice benefits:
 
-        * The parameter values are automatically added to the output file (have a look into the ``results/``
-          folder to see how it works and where the results are stored)
-        * The output for different parameters are stored on different locations, so no need to fear overriding
-          results.
-        * The format of the folder structure makes it easy to work on it using bash commands as well as
-          automated procedures.
-        * Other files related to your job, e.g. the submission files etc. are also placed into this
-          folder (this is why the very first example defined it already).
-        * The default is to use the folder where your script is located.
+    * The parameter values are automatically added to the output file (have a look into the ``results/``
+      folder to see how it works and where the results are stored)
+    * The output for different parameters are stored on different locations, so no need to fear overriding
+      results.
+    * The format of the folder structure makes it easy to work on it using bash commands as well as
+      automated procedures.
+    * Other files related to your job, e.g. the submission files etc. are also placed into this
+      folder (this is why the very first example defined it already).
+    * The default is to use the folder where your script is located.
 
     .. hint::
         In the example, the base path for the results is defined in the python file with
 
         .. code-block:: python
 
             b2luigi.set_setting("result_dir", "results")
@@ -165,26 +163,25 @@
         true for non-batch calculations.
 
 5.  Let's add some more tasks to our little example. We want to use the currently created files
     and add them all together to an average number.
     So edit your example file to include the following content:
 
     .. literalinclude:: ../../tests/doc_examples/simple_example_b2luigi_2.py
-       :linenos:
 
     See how we defined dependencies in line 19 with the ``requires`` function.
     By calling ``clone`` we make sure that any parameters from the current task (which are none in our case)
     are copied to the dependencies.
 
     .. hint::
 
         Again, expert ``luigi`` users will not see anything new here.
 
     By using the helper functions :meth:`b2luigi.Task.get_input_file_names`
-    and :meth:`b2luigi.Task.get_output_file` the output file name generation with parameters
+    and :meth:`b2luigi.Task.get_output_file_name` the output file name generation with parameters
     is transparent to you as a user.
     Super easy!
 
     When you run the script, you will see that ``luigi`` detects your already run files
     from before (the random numbers) and will not run the task again!
     It will only output a file in `results/average.txt` with a number near 0.5.
```

### Comparing `b2luigi-0.9.1/examples/basf2/basf2_chain_example.py` & `b2luigi-1.0.0/examples/basf2/basf2_chain_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,94 +6,111 @@
 import basf2
 
 import modularAnalysis
 import simulation
 import vertex
 import generators
 import reconstruction
-from ROOT import Belle2
+import mdst
 
 
 class SimulationType(Enum):
     y4s = "Y(4S)"
     continuum = "Continuum"
 
 
 class SimulationTask(Basf2PathTask):
     n_events = luigi.IntParameter()
     event_type = luigi.EnumParameter(enum=SimulationType)
 
     def create_path(self):
-        path = basf2.create_path()
+        path = basf2.Path()
         modularAnalysis.setupEventInfo(self.n_events, path)
 
         if self.event_type == SimulationType.y4s:
-            # in current main branch and release 5 the Y(4S)decay file is moved, so try old and new locations
-            find_file_ignore_error = True
-            dec_file = Belle2.FileSystem.findFile('analysis/examples/tutorials/B2A101-Y4SEventGeneration.dec',
-                                                  find_file_ignore_error)
+            # In current main branch and release 5 the Y(4S)decay file is moved,
+            # so try old and new locations.
+
+            # With ``silent=True``, ``find_file`` returns empty string if nothing is
+            # found. With ``silent=False``, a ``FileNotFoundError`` exception is
+            # raised.
+            dec_file = basf2.find_file("analysis/examples/tutorials/B2A101-Y4SEventGeneration.dec", silent=True)
             if not dec_file:
-                dec_file = Belle2.FileSystem.findFile('analysis/examples/simulations/B2A101-Y4SEventGeneration.dec')
+                dec_file = basf2.find_file("analysis/examples/simulations/B2A101-Y4SEventGeneration.dec")
         elif self.event_type == SimulationType.continuum:
-            dec_file = Belle2.FileSystem.findFile('analysis/examples/simulations/B2A102-ccbarEventGeneration.dec')
+            dec_file = basf2.find_file("analysis/examples/simulations/B2A102-ccbarEventGeneration.dec")
         else:
             raise ValueError(f"Event type {self.event_type} is not valid. It should be either 'Y(4S)' or 'Continuum'!")
 
-        generators.add_evtgen_generator(path, 'signal', dec_file)
-        modularAnalysis.loadGearbox(path)
+        generators.add_evtgen_generator(path, "signal", dec_file)
         simulation.add_simulation(path)
 
-        path.add_module('RootOutput', outputFileName=self.get_output_file_name('simulation_full_output.root'))
+        path.add_module("RootOutput", outputFileName=self.get_output_file_name("simulation_full_output.root"))
 
         return path
 
     def output(self):
         yield self.add_to_output("simulation_full_output.root")
 
 
 @luigi.requires(SimulationTask)
 class ReconstructionTask(Basf2PathTask):
     def create_path(self):
         path = basf2.create_path()
 
-        path.add_module('RootInput', inputFileNames=self.get_input_file_names("simulation_full_output.root"))
-        modularAnalysis.loadGearbox(path)
+        path.add_module("RootInput", inputFileNames=self.get_input_file_names("simulation_full_output.root"))
+
+        path.add_module("Gearbox")
+        path.add_module("Geometry")
         reconstruction.add_reconstruction(path)
 
-        modularAnalysis.outputMdst(self.get_output_file_name("reconstructed_output.root"), path=path)
+        mdst.add_mdst_output(path=path, filename=self.get_output_file_name("reconstructed_output.root"))
 
         return path
 
     def output(self):
         yield self.add_to_output("reconstructed_output.root")
 
 
 @luigi.requires(ReconstructionTask)
 class AnalysisTask(Basf2PathTask):
     def create_path(self):
-        path = basf2.create_path()
-        modularAnalysis.inputMdstList('default', self.get_input_file_names("reconstructed_output.root"), path=path)
-        modularAnalysis.fillParticleLists([('K+', 'kaonID > 0.1'), ('pi+', 'pionID > 0.1')], path=path)
-        modularAnalysis.reconstructDecay('D0 -> K- pi+', '1.7 < M < 1.9', path=path)
-        modularAnalysis.matchMCTruth('D0', path=path)
-        modularAnalysis.reconstructDecay('B- -> D0 pi-', '5.2 < Mbc < 5.3', path=path)
+        path = basf2.Path()
+        modularAnalysis.inputMdstList("default", self.get_input_file_names("reconstructed_output.root"), path=path)
+        modularAnalysis.fillParticleLists([("K+", "kaonID > 0.1"), ("pi+", "pionID > 0.1")], path=path)
+        modularAnalysis.reconstructDecay("D0 -> K- pi+", "1.7 < M < 1.9", path=path)
+        modularAnalysis.matchMCTruth("D0", path=path)
+        modularAnalysis.reconstructDecay("B- -> D0 pi-", "5.2 < Mbc < 5.3", path=path)
         try:  # treeFit is the new function name in light releases after release 4 (e.g. light-2002-janus)
-            vertex.treeFit('B+', 0.1, update_all_daughters=True, path=path)
+            vertex.treeFit("B+", 0.1, update_all_daughters=True, path=path)
         except AttributeError:  # vertexTree is the function name in release 4
-            vertex.vertexTree('B+', 0.1, update_all_daughters=True, path=path)
-        modularAnalysis.matchMCTruth('B-', path=path)
-        modularAnalysis.variablesToNtuple('D0',
-                                          ['M', 'p', 'E', 'useCMSFrame(p)', 'useCMSFrame(E)',
-                                           'daughter(0, kaonID)', 'daughter(1, pionID)', 'isSignal', 'mcErrors'],
-                                          filename=self.get_output_file_name("D_n_tuple.root"),
-                                          path=path)
-        modularAnalysis.variablesToNtuple('B-',
-                                          ['Mbc', 'deltaE', 'isSignal', 'mcErrors', 'M'],
-                                          filename=self.get_output_file_name("B_n_tuple.root"),
-                                          path=path)
+            vertex.vertexTree("B+", 0.1, update_all_daughters=True, path=path)
+        modularAnalysis.matchMCTruth("B-", path=path)
+        modularAnalysis.variablesToNtuple(
+            "D0",
+            [
+                "M",
+                "p",
+                "E",
+                "useCMSFrame(p)",
+                "useCMSFrame(E)",
+                "daughter(0, kaonID)",
+                "daughter(1, pionID)",
+                "isSignal",
+                "mcErrors",
+            ],
+            filename=self.get_output_file_name("D_n_tuple.root"),
+            path=path,
+        )
+        modularAnalysis.variablesToNtuple(
+            "B-",
+            ["Mbc", "deltaE", "isSignal", "mcErrors", "M"],
+            filename=self.get_output_file_name("B_n_tuple.root"),
+            path=path,
+        )
         return path
 
     def output(self):
         yield self.add_to_output("D_n_tuple.root")
         yield self.add_to_output("B_n_tuple.root")
```

### Comparing `b2luigi-0.9.1/examples/gbasf2/example_mdst_analysis.py` & `b2luigi-1.0.0/examples/gbasf2/example_mdst_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 #!/usr/bin/env python3
 """
 This file is not a standalone example, but meant to provide a simple example
 analysis path be imported from gbasf2_example.py
 """
 
 import basf2
-import ROOT  # noqa: F401
 import modularAnalysis as mA
 import vertex as vx
 from stdCharged import stdK, stdPi
 from variables import variables as vm
 
 
 def create_analysis_path(
-        b_ntuple_filename="B_ntuple.root",
-        d_ntuple_filename="D_ntuple.root",
-        mbc_range=(5.2, 5.3),
+    b_ntuple_filename="B_ntuple.root",
+    d_ntuple_filename="D_ntuple.root",
+    mbc_range=(5.2, 5.3),
 ):
     """
     Example of a minimal reconstruction with a cut as a changeable function
     parameter, adapted from code in the ``B2T_Basics_3_FirstAnalysis.ipynb``
     notebook from b2 starter kit.
     """
-    path = basf2.create_path()
+    path = basf2.Path()
     # this local inputMdstList will only be used when this steerig file is run locally, gbasf2 overrides it
-    local_input_files = ["/group/belle2/dataprod/MC/MC13a/prod00009434/s00/e1003/4S/r00000/mixed/mdst/sub00/mdst_000001_prod00009434_task10020000001.root"]
+    local_input_files = [
+        "/group/belle2/dataprod/MC/MC13a/prod00009434/s00/e1003/4S/r00000/mixed/mdst/sub00/mdst_000001_prod00009434_task10020000001.root"
+    ]
     mA.inputMdstList(
         environmentType="default",
         filelist=local_input_files,
         path=path,
     )
     stdK("higheff", path=path)
     stdPi("higheff", path=path)
-    mA.reconstructDecay('D0:Kpi -> K-:higheff pi+:higheff', '1.7 < M < 1.9', path=path)
+    mA.reconstructDecay("D0:Kpi -> K-:higheff pi+:higheff", "1.7 < M < 1.9", path=path)
     # use try except to have this code work for both the old and new function names for the tree fit
-    mA.matchMCTruth('D0:Kpi', path=path)
-    mA.reconstructDecay('B- -> D0:Kpi pi-:higheff', f"{mbc_range[0]} < Mbc < {mbc_range[1]}", path=path)
+    mA.matchMCTruth("D0:Kpi", path=path)
+    mA.reconstructDecay("B- -> D0:Kpi pi-:higheff", f"{mbc_range[0]} < Mbc < {mbc_range[1]}", path=path)
     try:
-        vx.treeFit('B+', 0.1, path=path)
+        vx.treeFit("B+", 0.1, path=path)
     except AttributeError:
-        vx.vertexTree('B+', 0.1, path=path)
+        vx.vertexTree("B+", 0.1, path=path)
     mA.setAnalysisConfigParams({"mcMatchingVersion": "BelleII"}, path)
-    mA.matchMCTruth('B-', path=path)
+    mA.matchMCTruth("B-", path=path)
     vm.addAlias("p_cms", "useCMSFrame(p)")  # include aliases to test if they work
     vm.addAlias("E_cms", "useCMSFrame(E)")
-    mA.variablesToNtuple('D0:Kpi', ['M', 'p', 'E', 'E_cms', 'p_cms', 'daughter(0, kaonID)',
-                                    'daughter(1, pionID)', 'isSignal', 'mcErrors'],
-                         filename=d_ntuple_filename, treename="D", path=path)
-    mA.variablesToNtuple('B-', ['Mbc', 'deltaE', 'isSignal', 'mcErrors', 'M'],
-                         filename=b_ntuple_filename, treename="B", path=path)
+    mA.variablesToNtuple(
+        "D0:Kpi",
+        ["M", "p", "E", "E_cms", "p_cms", "daughter(0, kaonID)", "daughter(1, pionID)", "isSignal", "mcErrors"],
+        filename=d_ntuple_filename,
+        treename="D",
+        path=path,
+    )
+    mA.variablesToNtuple(
+        "B-", ["Mbc", "deltaE", "isSignal", "mcErrors", "M"], filename=b_ntuple_filename, treename="B", path=path
+    )
     return path
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Use this to execute the analysis path if this file is called as a main
     # file. It can be used to test the analysis path independently of the gbasf2
     # luigi task. But if this module is only imported, the following is not executed.
     path = create_analysis_path()
     basf2.print_path(path)
     basf2.process(path)
```

### Comparing `b2luigi-0.9.1/examples/gbasf2/gbasf2_example.py` & `b2luigi-1.0.0/examples/gbasf2/gbasf2_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,15 @@
     gbasf2_input_dataset = b2luigi.Parameter(hashed=True)
     # Example luigi cut parameter to facilitate starting multiple projects for different cut values
     mbc_lower_cut = b2luigi.IntParameter()
 
     def create_path(self):
         mbc_range = (self.mbc_lower_cut, 5.3)
         return example_mdst_analysis.create_analysis_path(
-            d_ntuple_filename="D_ntuple.root",
-            b_ntuple_filename="B_ntuple.root",
-            mbc_range=mbc_range
+            d_ntuple_filename="D_ntuple.root", b_ntuple_filename="B_ntuple.root", mbc_range=mbc_range
         )
 
     def output(self):
         yield self.add_to_output("D_ntuple.root")
         yield self.add_to_output("B_ntuple.root")
 
 
@@ -31,25 +29,26 @@
     """
     We use the AnalysisWrapperTask to be able to require multiple analyse tasks with
     different input datasets and cut values. For each parameter combination, a
     different gbasf2 project will be submitted.
     """
 
     def requires(self):
-        input_dataset = \
-            "/belle/MC/release-04-01-04/DB00000774/SkimM13ax1/prod00011778/e1003/4S/r00000/mixed/11180100/udst/sub00/"\
+        input_dataset = (
+            "/belle/MC/release-04-01-04/DB00000774/SkimM13ax1/prod00011778/e1003/4S/r00000/mixed/11180100/udst/sub00/"
             "udst_000006_prod00011778_task10020000006.root"
+        )
         # if you want to iterate over different cuts, just add more values to this list
         mbc_lower_cuts = [5.15, 5.2]
         for mbc_lower_cut in mbc_lower_cuts:
             yield AnalysisTask(
                 mbc_lower_cut=mbc_lower_cut,
                 gbasf2_project_name_prefix="luigiExample",
                 gbasf2_input_dataset=input_dataset,
                 max_event=100,
             )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main_task_instance = AnalysisWrapperTask()
     n_gbasf2_tasks = len(list(main_task_instance.requires()))
     b2luigi.process(main_task_instance, workers=n_gbasf2_tasks)
```

### Comparing `b2luigi-0.9.1/examples/htcondor/htcondor_example.py` & `b2luigi-1.0.0/examples/htcondor/htcondor_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import b2luigi
 import random
 
 
 class MyNumberTask(b2luigi.Task):
     some_parameter = b2luigi.IntParameter()
 
-    htcondor_settings = {
-        "request_cpus": 1,
-        "request_memory": "100 MB"
-    }
+    htcondor_settings = {"request_cpus": 1, "request_memory": "100 MB"}
 
     def output(self):
         yield self.add_to_output("output_file.txt")
 
     def run(self):
         print("I am now starting a task")
         random_number = random.random()
@@ -21,18 +18,15 @@
             raise ValueError
 
         with open(self.get_output_file_name("output_file.txt"), "w") as f:
             f.write(f"{random_number}\n")
 
 
 class MyAverageTask(b2luigi.Task):
-    htcondor_settings = {
-        "request_cpus": 1,
-        "request_memory": "200 MB"
-    }
+    htcondor_settings = {"request_cpus": 1, "request_memory": "200 MB"}
 
     def requires(self):
         for i in range(10):
             yield self.clone(MyNumberTask, some_parameter=i)
 
     def output(self):
         yield self.add_to_output("average.txt")
```

### Comparing `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json` & `b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/all_done_but_application_error.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json` & `b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/done_testjbucket1357828d80b3.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json` & `b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/failed_7663_r03743_10_prod00013766_11x1.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json` & `b2luigi-1.0.0/tests/batch/_gbasf2_project_statuses/running_TrainingFEI_17-04-2021a10a957289.json`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/batch_task_1.py` & `b2luigi-1.0.0/tests/batch/batch_task_1.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/batch_task_2.py` & `b2luigi-1.0.0/tests/batch/batch_task_2.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/test_batch_process.py` & `b2luigi-1.0.0/tests/batch/test_batch_process.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/batch/test_gbasf2_helper_functions.py` & `b2luigi-1.0.0/tests/batch/test_gbasf2_helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,24 @@
 from io import StringIO
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Iterable
 from unittest import mock
 
 from b2luigi.batch.processes.gbasf2 import (
-    _get_lfn_upto_reschedule_number, _move_downloaded_dataset_to_output_dir,
-    _split_all_extensions, get_dirac_user, get_proxy_info, get_unique_lfns,
-    lfn_follows_gb2v5_convention, query_lpns, setup_dirac_proxy)
+    _get_lfn_upto_reschedule_number,
+    _move_downloaded_dataset_to_output_dir,
+    _split_all_extensions,
+    get_dirac_user,
+    get_proxy_info,
+    get_unique_lfns,
+    lfn_follows_gb2v5_convention,
+    query_lpns,
+    setup_dirac_proxy,
+)
 
 # first test utilities for working with logical file names on the grid
 
 
 class TestLFNFollowsGbasf2V5Convention(unittest.TestCase):
     def test_newstyle_lfn_is_true(self):
         lfn = "Upsilon4SBpcandee_00000_job181817516_03.root"
@@ -34,23 +41,19 @@
         lfn = "my_ntuple_0001.root"
         self.assertFalse(lfn_follows_gb2v5_convention(lfn))
 
 
 class TestLFNUptoRescheduleNumber(unittest.TestCase):
     def test_strings_equal_camelcase_lfn(self):
         lfn = "Upsilon4SBpcandee_00000_job181817516_03.root"
-        self.assertEqual(
-            _get_lfn_upto_reschedule_number(lfn), "Upsilon4SBpcandee_00000_job181817516"
-        )
+        self.assertEqual(_get_lfn_upto_reschedule_number(lfn), "Upsilon4SBpcandee_00000_job181817516")
 
     def test_strings_equal_snakecase_lfn(self):
         lfn = "my_ntuple_name_00000_job181817516_03.root"
-        self.assertEqual(
-            _get_lfn_upto_reschedule_number(lfn), "my_ntuple_name_00000_job181817516"
-        )
+        self.assertEqual(_get_lfn_upto_reschedule_number(lfn), "my_ntuple_name_00000_job181817516")
 
     def test_oldstyle_lfn_raises_error(self):
         lfn = "my_ntuple_0001.root"
         with self.assertRaises(ValueError):
             _get_lfn_upto_reschedule_number(lfn)
 
 
@@ -82,16 +85,15 @@
             "Upsilon4SBpcandee_00017_job181817533_02.root",
             "Upsilon4SBpcandee_00018_job181817534_01.root",
             "Upsilon4SBpcandee_00019_job181817535_00.root",
         ]
         # create same input but with more underscores in initial root file name (snake case)
         # to test whether the string splitting logic is stable in that case
         self.lfns_with_duplicates_snake_case = [
-            lfn.replace("Upsilon4SBpcandee", "u4s_Bp_cand_")
-            for lfn in self.lfns_with_duplicates
+            lfn.replace("Upsilon4SBpcandee", "u4s_Bp_cand_") for lfn in self.lfns_with_duplicates
         ]
         self.unique_lfns = {
             "Upsilon4SBpcandee_00000_job181817516_00.root",
             "Upsilon4SBpcandee_00001_job181817517_00.root",
             "Upsilon4SBpcandee_00002_job181817518_00.root",
             "Upsilon4SBpcandee_00003_job181817519_00.root",
             "Upsilon4SBpcandee_00004_job181817520_00.root",
@@ -107,17 +109,15 @@
             "Upsilon4SBpcandee_00014_job181817530_00.root",
             "Upsilon4SBpcandee_00015_job181817531_00.root",
             "Upsilon4SBpcandee_00016_job181817532_00.root",
             "Upsilon4SBpcandee_00017_job181817533_02.root",
             "Upsilon4SBpcandee_00018_job181817534_01.root",
             "Upsilon4SBpcandee_00019_job181817535_00.root",
         }
-        self.unique_lfns_snake_case = {
-            lfn.replace("Upsilon4SBpcandee", "u4s_Bp_cand_") for lfn in self.unique_lfns
-        }
+        self.unique_lfns_snake_case = {lfn.replace("Upsilon4SBpcandee", "u4s_Bp_cand_") for lfn in self.unique_lfns}
 
     def test_sets_equal(self):
         unique_lfns = get_unique_lfns(self.lfns_with_duplicates)
         self.assertSetEqual(unique_lfns, self.unique_lfns)
 
     def test_count_equal(self):
         unique_lfns = get_unique_lfns(self.lfns_with_duplicates)
@@ -128,78 +128,64 @@
         self.assertSetEqual(unique_lfns_snake_case, self.unique_lfns_snake_case)
 
     def test_sets_equal_input_as_set(self):
         unique_lfns = get_unique_lfns(set(self.lfns_with_duplicates))
         self.assertSetEqual(unique_lfns, self.unique_lfns)
 
     def test_sets_equal_underscore_in_file_name_input_as_set(self):
-        unique_lfns_snake_case = get_unique_lfns(
-            set(self.lfns_with_duplicates_snake_case)
-        )
+        unique_lfns_snake_case = get_unique_lfns(set(self.lfns_with_duplicates_snake_case))
         self.assertSetEqual(unique_lfns_snake_case, self.unique_lfns_snake_case)
 
 
 # In many of the tests we mock ``run_with_gbasf2``, which is used to run
 # ``gb2_proxy_init``. Let's define a pseudo process class with stdout and
 # stderr for that and define some common output messages of gb2_proxy_init
 MockProcess = namedtuple("mock_process", ["stdout", "stderr"])
 
 
 class TestSetupDiracProxy(unittest.TestCase):
     success_msg = "Succeed with return value:\n0"
     error_msg = "Error: Operation not permitted ( 1 : )"
-    wrong_pw_msg = (
-        "Generating proxy..." "Enter Certificate password:" "Bad passphrase"
-    ) + f"\n{error_msg}"
+    wrong_pw_msg = ("Generating proxy..." "Enter Certificate password:" "Bad passphrase") + f"\n{error_msg}"
 
     @mock.patch("b2luigi.batch.processes.gbasf2.getpass")
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
-    def test_dont_setup_when_proxy_alive(
-        self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass
-    ):
+    def test_dont_setup_when_proxy_alive(self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass):
         mock_get_proxy_info.return_value = {"secondsLeft": 999}
         setup_dirac_proxy()
         # check that gb2_proxy_init was never called via subprocess
         mock_getpass.return_value = "pwd"
         self.assertEqual(mock_run_with_gbasf2.call_count, 0)
 
     @mock.patch("b2luigi.batch.processes.gbasf2.getpass")
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
-    def test_setup_proxy_on_0_seconds(
-        self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass
-    ):
+    def test_setup_proxy_on_0_seconds(self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass):
         # force setting up of new proxy
         mock_get_proxy_info.return_value = {"secondsLeft": 0}
         mock_getpass.return_value = "pwd"
         mock_run_with_gbasf2.return_value = MockProcess(self.success_msg, "")
         setup_dirac_proxy()
         self.assertEqual(mock_run_with_gbasf2.call_count, 1)
 
     @mock.patch("b2luigi.batch.processes.gbasf2.getpass")
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
-    def test_setup_proxy_when_no_proxy_info(
-        self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass
-    ):
+    def test_setup_proxy_when_no_proxy_info(self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass):
         # pretend proxy is not initalized yet, then get_proxy_info raises CalledProcessError
-        mock_get_proxy_info.side_effect = CalledProcessError(
-            1, ["gb2_proxy_info", "-g", "belle"]
-        )
+        mock_get_proxy_info.side_effect = CalledProcessError(1, ["gb2_proxy_info", "-g", "belle"])
         mock_run_with_gbasf2.return_value = MockProcess(self.success_msg, "")
         setup_dirac_proxy()
         self.assertEqual(mock_run_with_gbasf2.call_count, 1)
 
     @mock.patch("b2luigi.batch.processes.gbasf2.getpass")
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
-    def test_retry_on_wrong_password(
-        self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass
-    ):
+    def test_retry_on_wrong_password(self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass):
         # force setting up of new proxy
         mock_get_proxy_info.return_value = {"secondsLeft": 0}
 
         # mock run_with_gbasf2 to first return wrong PW message a couple of times, before returning successfully
         return_processes = [
             MockProcess(self.wrong_pw_msg, ""),
             MockProcess("", self.wrong_pw_msg),
@@ -218,30 +204,24 @@
             ],
         )
         self.assertEqual(mock_run_with_gbasf2.call_count, len(return_processes))
 
     @mock.patch("b2luigi.batch.processes.gbasf2.getpass")
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
-    def test_raises_error_when_errormsg_in_stdout(
-        self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass
-    ):
+    def test_raises_error_when_errormsg_in_stdout(self, mock_get_proxy_info, mock_run_with_gbasf2, mock_getpass):
         mock_get_proxy_info.return_value = {"secondsLeft": 0}
         # check that gb2_proxy_init was never called via subprocess
         mock_run_with_gbasf2.return_value = MockProcess(self.error_msg, "")
         with self.assertRaises(CalledProcessError):
             setup_dirac_proxy()
 
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
-    def test_get_proxy_info_doesnt_suppress_called_process_error(
-        self, mock_run_with_gbasf2
-    ):
-        mock_run_with_gbasf2.side_effect = CalledProcessError(
-            1, ["gb2_proxy_info", "-g", "belle"]
-        )
+    def test_get_proxy_info_doesnt_suppress_called_process_error(self, mock_run_with_gbasf2):
+        mock_run_with_gbasf2.side_effect = CalledProcessError(1, ["gb2_proxy_info", "-g", "belle"])
         with self.assertRaises(CalledProcessError):
             get_proxy_info()
         self.assertEqual(mock_run_with_gbasf2.call_count, 1)
 
 
 class TestQueryLPNs(unittest.TestCase):
     @mock.patch("b2luigi.batch.processes.gbasf2.run_with_gbasf2")
@@ -273,17 +253,15 @@
 class TestMoveDownloadedDatasetToOutputDir(unittest.TestCase):
     def setUp(self):
         self.test_dir = Path(tempfile.mkdtemp())
 
     def tearDown(self):
         shutil.rmtree(self.test_dir)
 
-    def _create_mock_project_download_dir(
-        self, project_name: str, root_files_per_sub: Iterable[int] = (0,)
-    ) -> Path:
+    def _create_mock_project_download_dir(self, project_name: str, root_files_per_sub: Iterable[int] = (0,)) -> Path:
         downloaded_project_path = self.test_dir / project_name
         downloaded_project_path.mkdir(exist_ok=True)
         for sub_idx, n_files in enumerate(root_files_per_sub):
             assert sub_idx < 100, "There  can't be more than 100 subs"
             # create sub<xy>-directory
             sub_dir = downloaded_project_path / f"sub{sub_idx:02d}"
             sub_dir.mkdir(exist_ok=False)
@@ -294,25 +272,19 @@
         return downloaded_project_path
 
     def test_moving_of_multiple_subs(self):
         root_files_per_sub = [10, 10, 10]
         project_path = self._create_mock_project_download_dir(
             project_name="multiple_subs", root_files_per_sub=root_files_per_sub
         )
-        project_root_fnames = [
-            root_fpath.name for root_fpath in project_path.glob("sub*/*.root")
-        ]
+        project_root_fnames = [root_fpath.name for root_fpath in project_path.glob("sub*/*.root")]
 
         output_path = self.test_dir / "multiple_subs_output.root"
-        _move_downloaded_dataset_to_output_dir(
-            project_path.as_posix(), output_path.as_posix()
-        )
-        output_root_fnames = [
-            root_fpath.name for root_fpath in output_path.glob("*.root")
-        ]
+        _move_downloaded_dataset_to_output_dir(project_path.as_posix(), output_path.as_posix())
+        output_root_fnames = [root_fpath.name for root_fpath in output_path.glob("*.root")]
 
         # check that all root files have been moved to output directory
         self.assertCountEqual(output_root_fnames, project_root_fnames)
         # Test the number of output files is what we expect
         self.assertEqual(len(output_root_fnames), sum(root_files_per_sub))
         # check that input directory is empty after move
         self.assertListEqual(list(project_path.glob("sub*/*.root")), [])
@@ -320,31 +292,27 @@
     def test_error_when_a_sub_is_empty(self):
         root_files_per_sub = [10, 0, 10]
         project_path = self._create_mock_project_download_dir(
             project_name="empty_subs", root_files_per_sub=root_files_per_sub
         )
         output_path = self.test_dir / "empty_subs_output.root"
         with self.assertRaises(RuntimeError):
-            _move_downloaded_dataset_to_output_dir(
-                project_path.as_posix(), output_path.as_posix()
-            )
+            _move_downloaded_dataset_to_output_dir(project_path.as_posix(), output_path.as_posix())
 
 
 class TestGetDiracUser(unittest.TestCase):
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
     @mock.patch("b2luigi.batch.processes.gbasf2.setup_dirac_proxy")
     def test_get_dirac_user_gets_user(self, _, mock_get_proxy_info):
         mock_get_proxy_info.return_value = {"username": "testuser"}
         self.assertEqual(get_dirac_user(), "testuser")
 
     @mock.patch("b2luigi.batch.processes.gbasf2.get_proxy_info")
     @mock.patch("b2luigi.batch.processes.gbasf2.setup_dirac_proxy")
-    def test_get_dirac_user_ensures_proxy_initialized(
-        self, mock_setup_dirac_proxy, mock_get_proxy_info
-    ):
+    def test_get_dirac_user_ensures_proxy_initialized(self, mock_setup_dirac_proxy, mock_get_proxy_info):
         mock_get_proxy_info.return_value = {"username": "testuser"}
         get_dirac_user()
         self.assertEqual(mock_setup_dirac_proxy.call_count, 1)
 
 
 class TestSplitAllExtensions(unittest.TestCase):
     def test_single_ext(self):
```

### Comparing `b2luigi-0.9.1/tests/batch/test_gbasf2_process.py` & `b2luigi-1.0.0/tests/batch/test_gbasf2_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 import tempfile
 import unittest
 from collections import Counter
 from typing import List
 from unittest.mock import MagicMock, Mock, patch
 
 import b2luigi
-from b2luigi.batch.processes.gbasf2 import (Gbasf2Process, JobStatus,
-                                            get_unique_project_name)
+from b2luigi.batch.processes.gbasf2 import Gbasf2Process, JobStatus, get_unique_project_name
 
 from ..helpers import B2LuigiTestCase
 from .batch_task_1 import MyTask
 
 
 class MyGbasf2Task(MyTask):
     gbasf2_project_name_prefix = "my_gb2_task_"
 
 
 class TestGbasf2RescheduleJobs(B2LuigiTestCase):
-
     job_statuses_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "_gbasf2_project_statuses")
     joblist_tmpfile_name = "jobs_to_be_rescheduled.txt"
 
     def setUp(self):
         super().setUp()
         self.gb2_mock_process = MagicMock()
         self.gb2_mock_process.task = MyGbasf2Task("some_parameter")
@@ -37,21 +35,24 @@
         with open(os.path.join(self.job_statuses_dir, job_status_fname)) as job_status_json_file:
             return json.load(job_status_json_file)
 
     def _reschedule_jobs(self, job_ids):
         pass
 
     def assert_rescheduled_jobs(self, job_status_fname, expected_jobs_to_be_rescheduled):
-        with patch("b2luigi.batch.processes.gbasf2.get_gbasf2_project_job_status_dict",
-                   MagicMock(return_value=self._get_job_status_dict(job_status_fname))):
+        with patch(
+            "b2luigi.batch.processes.gbasf2.get_gbasf2_project_job_status_dict",
+            MagicMock(return_value=self._get_job_status_dict(job_status_fname)),
+        ):
             with patch("b2luigi.batch.processes.gbasf2.Gbasf2Process._reschedule_jobs", new=self._reschedule_jobs):
-
                 Gbasf2Process._reschedule_failed_jobs(self.gb2_mock_process)
 
-                self.assertCountEqual(list(self.gb2_mock_process.n_retries_by_job.keys()), expected_jobs_to_be_rescheduled)
+                self.assertCountEqual(
+                    list(self.gb2_mock_process.n_retries_by_job.keys()), expected_jobs_to_be_rescheduled
+                )
                 for jobid in self.gb2_mock_process.n_retries_by_job.keys():
                     self.assertEqual(self.gb2_mock_process.n_retries_by_job[jobid], 1)
 
     def test_reschedule_jobs_all_done(self):
         "Test gbasf2 project rescheduling with dict where all jobs are done"
         self.assert_rescheduled_jobs("done_testjbucket1357828d80b3.json", [])
 
@@ -65,15 +66,14 @@
 
     def test_reschedule_jobs_major_status_done_but_minor_status_not(self):
         "Test gbasf2 project rescheduling with dict where major job status is all done but application status is not ``DONE``"
         self.assert_rescheduled_jobs("all_done_but_application_error.json", ["187522107"])
 
 
 class TestGbasf2GetJobStatus(B2LuigiTestCase):
-
     job_statuses_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "_gbasf2_project_statuses")
 
     def setUp(self):
         super().setUp()
         self.gb2_mock_process = Mock()
         self.gb2_mock_process.task = MyGbasf2Task("some_parameter")
         self.gb2_mock_process.dirac_user = "username"
@@ -82,16 +82,18 @@
         b2luigi.set_setting("gbasf2_print_status_updates", False)
 
     def _get_job_status_dict(self, job_status_fname):
         with open(os.path.join(self.job_statuses_dir, job_status_fname)) as job_status_json_file:
             return json.load(job_status_json_file)
 
     def assert_job_status(self, job_status_fname, expected_job_status):
-        with patch("b2luigi.batch.processes.gbasf2.get_gbasf2_project_job_status_dict",
-                   MagicMock(return_value=self._get_job_status_dict(job_status_fname))):
+        with patch(
+            "b2luigi.batch.processes.gbasf2.get_gbasf2_project_job_status_dict",
+            MagicMock(return_value=self._get_job_status_dict(job_status_fname)),
+        ):
             job_status = Gbasf2Process.get_job_status(self.gb2_mock_process)
             self.assertEqual(job_status, expected_job_status)
 
     def test_get_job_status_all_done(self):
         "Test gbasf2 project status dict where all jobs are done"
         self.assert_job_status("done_testjbucket1357828d80b3.json", JobStatus.successful)
 
@@ -127,109 +129,95 @@
         gb2_mock_process.wrapper_file_path = self.test_dir
         gb2_mock_process.gbasf2_project_name = get_unique_project_name(task)
         gb2_mock_process.task = task
         return Gbasf2Process._build_gbasf2_submit_command(gb2_mock_process)
 
     def test_input_dataset_in_command(self):
         "Test that if the input dataset is set, it occurs once in the command string"
+
         class _Task(MyGbasf2Task):
             gbasf2_input_dataset = b2luigi.Parameter(default=self.dummy_lfn)
+
         gb2_cmd = self._build_gbasf2_submit_command(_Task("some_parameter"))
         gb2_cmd_str = " ".join(gb2_cmd)
         self.assertEqual(gb2_cmd.count(self.dummy_lfn), 1)
         self.assertEqual(gb2_cmd.count("-i"), 1)
         self.assertEqual(gb2_cmd_str.count(f" -i {self.dummy_lfn}"), 1)
         self.assertNotIn("--input_dslist", gb2_cmd_str)
 
     def test_input_dslist_in_command(self):
         "Test that if the input dataset list is set, it occurs once in the command string"
+
         class _Task(MyGbasf2Task):
             gbasf2_input_dslist = self.dummy_lfn_file.name
+
         gb2_cmd = self._build_gbasf2_submit_command(_Task("some_parameter"))
         gb2_cmd_str = " ".join(gb2_cmd)
         self.assertEqual(gb2_cmd.count(self.dummy_lfn_file.name), 1)
         self.assertEqual(gb2_cmd.count("--input_dslist"), 1)
         self.assertEqual(gb2_cmd_str.count(f" --input_dslist {self.dummy_lfn_file.name}"), 1)
         self.assertNotIn("-i", gb2_cmd)
 
     def test_input_dslist_set_but_does_not_exist(self):
         """Test that if the input dataset list is set but the file does not exist, an ``FileNotFoundError`` is raised"""
+
         class _Task(MyGbasf2Task):
             gbasf2_input_dslist = self.dummy_lfn_file.name
+
         self.dummy_lfn_file.close()
         self.assertRaises(FileNotFoundError, lambda: self._build_gbasf2_submit_command(_Task("some_parameter")))
 
     def test_not_dataset_raises_error(self):
         """Test that we get an error when no gbasf2 input dataset is provided"""
         self.assertRaises(RuntimeError, lambda: self._build_gbasf2_submit_command(MyGbasf2Task("some_parameter")))
 
     def test_both_input_dataset_and_dslist_raises_error(self):
         """Test that en error is raise when both gbasf2_input_dataset and gbasf2_inputdslist settings are given"""
+
         class _Task(MyGbasf2Task):
             gbasf2_input_dataset = b2luigi.Parameter(default=self.dummy_lfn)
             gbasf2_input_dslist = self.dummy_lfn_file.name
+
         self.assertRaises(RuntimeError, lambda: self._build_gbasf2_submit_command(MyGbasf2Task("some_parameter")))
 
 
 class TestGetGbasf2DatasetQuery(unittest.TestCase):
     "Run tests for ``Gbasf2Process._get_gbasf2_dataset_query``."
 
     def setUp(self):
         super().setUp()
         self.gb2_mock_process = Mock()
         self.gb2_mock_process.gbasf2_project_name = "projectname"
         self.gb2_mock_process.dirac_user = "username"
         self.gb2_mock_process.task = MyTask("some_parameter")
 
     def test_filename_single_root_extension(self):
-        dataset_query = Gbasf2Process._get_gbasf2_dataset_query(
-            self.gb2_mock_process,
-            output_file_name="output.root"
-        )
-        self.assertEqual(
-            dataset_query,
-            "/belle/user/username/projectname/sub*/output_*.root"
-        )
+        dataset_query = Gbasf2Process._get_gbasf2_dataset_query(self.gb2_mock_process, output_file_name="output.root")
+        self.assertEqual(dataset_query, "/belle/user/username/projectname/sub*/output_*.root")
 
     def test_filename_multi_extension(self):
         dataset_query = Gbasf2Process._get_gbasf2_dataset_query(
-            self.gb2_mock_process,
-            output_file_name="output.mdst.root"
-        )
-        self.assertEqual(
-            dataset_query,
-            "/belle/user/username/projectname/sub*/output_*.mdst.root"
+            self.gb2_mock_process, output_file_name="output.mdst.root"
         )
+        self.assertEqual(dataset_query, "/belle/user/username/projectname/sub*/output_*.mdst.root")
 
     def test_non_root_extension_raises_err(self):
         "Raise an error if gbasf2 output does not end with .root"
         with self.assertRaises(ValueError):
-            Gbasf2Process._get_gbasf2_dataset_query(
-                self.gb2_mock_process,
-                output_file_name="output.mdst"
-            )
+            Gbasf2Process._get_gbasf2_dataset_query(self.gb2_mock_process, output_file_name="output.mdst")
 
     def test_non_basename_raises_err(self):
         """
         Currently we only support simple basenames as gbasf2 job outputs.
         LPN is guessed via dirac username for user projects.
         """
         with self.assertRaises(ValueError):
-            Gbasf2Process._get_gbasf2_dataset_query(
-                self.gb2_mock_process,
-                output_file_name="/path/to/output.root"
-            )
+            Gbasf2Process._get_gbasf2_dataset_query(self.gb2_mock_process, output_file_name="/path/to/output.root")
 
     def test_filename_single_extension(self):
         gb2_mock_process = Mock()
         gb2_mock_process.gbasf2_project_name = "projectname"
         gb2_mock_process.dirac_user = "username"
         gb2_mock_process.task = MyTask("some_parameter")
 
-        dataset_query = Gbasf2Process._get_gbasf2_dataset_query(
-            self=gb2_mock_process,
-            output_file_name="output.root"
-        )
-        self.assertEqual(
-            dataset_query,
-            "/belle/user/username/projectname/sub*/output_*.root"
-        )
+        dataset_query = Gbasf2Process._get_gbasf2_dataset_query(self=gb2_mock_process, output_file_name="output.root")
+        self.assertEqual(dataset_query, "/belle/user/username/projectname/sub*/output_*.root")
```

### Comparing `b2luigi-0.9.1/tests/batch/test_htcondor_processs.py` & `b2luigi-1.0.0/tests/batch/test_htcondor_processs.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class TestHTCondorCreateSubmitFile(B2LuigiTestCase):
     def _get_htcondor_submit_file_string(self, task):
         # the _create_htcondor_submit_file is a method of the ``HTCondorProcess`` class, but it only uses its
         # class to obtain ``self.task``, to it's sufficient to provide a mock class for ``self``, `
         htcondor_mock_process = mock.Mock()
         task.get_task_file_dir = lambda: self.test_dir
+        task.get_log_file_dir = lambda: self.test_dir
         htcondor_mock_process.task = task
         #  create submit file
         HTCondorProcess._create_htcondor_submit_file(htcondor_mock_process)
         # read submit file and return string
         submit_file_path = os.path.join(self.test_dir, "job.submit")
         with open(submit_file_path, "r") as submit_file:
             return submit_file.read()
@@ -102,35 +103,33 @@
 
     @mock.patch("subprocess.check_output")
     def test_ask_for_job_status_does_2_retries(self, mock_check_output):
         """Test the ``_ask_for_job_status`` recovers after two condor_q failures."""
 
         # make check_output fail 2 times before  return status dict
         n_fail = 2
-        mock_check_output.side_effect = n_fail * [
-            subprocess.CalledProcessError(1, ["mock", "command"])
-        ] + [self.mock_status_json]
+        mock_check_output.side_effect = n_fail * [subprocess.CalledProcessError(1, ["mock", "command"])] + [
+            self.mock_status_json
+        ]
         self.htcondor_job_status_cache._ask_for_job_status()
         self.assertEqual(mock_check_output.call_count, 3)
 
     @mock.patch("subprocess.check_output")
     def test_ask_for_job_status_no_retries_on_success(self, mock_check_output):
         """Test the ``_ask_for_job_status`` is only called once (no retries) when everything works."""
 
         # make check_output fail 2 times before  return status dict
         mock_check_output.return_value = self.mock_status_json
         self.htcondor_job_status_cache._ask_for_job_status()
         self.assertEqual(mock_check_output.call_count, 1)
 
     @mock.patch("subprocess.check_output")
-    def test_ask_for_job_status_fails_after_4_condor_q_failures(
-        self, mock_check_output
-    ):
+    def test_ask_for_job_status_fails_after_4_condor_q_failures(self, mock_check_output):
         """Test the ``_ask_for_job_status`` does not do more than 3 retries"""
 
         # make check_output fail 2 times before  return status dict
         n_fail = 4
-        mock_check_output.side_effect = n_fail * [
-            subprocess.CalledProcessError(1, ["mock", "command"])
-        ] + [self.mock_status_json]
+        mock_check_output.side_effect = n_fail * [subprocess.CalledProcessError(1, ["mock", "command"])] + [
+            self.mock_status_json
+        ]
         with self.assertRaises(subprocess.CalledProcessError):
             self.htcondor_job_status_cache._ask_for_job_status()
```

### Comparing `b2luigi-0.9.1/tests/cli/process_with_user_args_ignored_by_b2luigi.py` & `b2luigi-1.0.0/tests/cli/process_with_user_args_ignored_by_b2luigi.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py` & `b2luigi-1.0.0/tests/cli/process_with_user_args_not_ignored_by_b2luigi.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/cli/test_ignore_additional_command_line_args.py` & `b2luigi-1.0.0/tests/cli/test_ignore_additional_command_line_args.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/core/dispatch_1.py` & `b2luigi-1.0.0/tests/core/dispatch_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     def process(self):
         print("Hello!")
         with open(self.get_output_file_name("some_file.txt"), "w") as f:
             f.write("Done")
 
         print("Bye!")
         import sys
+
         sys.stdout.flush()
         os.kill(os.getpid(), 11)
 
         with open(self.get_output_file_name("some_other_file.txt"), "w") as f:
             f.write("Done")
```

### Comparing `b2luigi-0.9.1/tests/core/dispatch_2.py` & `b2luigi-1.0.0/tests/core/dispatch_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     def run(self):
         print("Hello!")
         with open(self.get_output_file_name("some_file.txt"), "w") as f:
             f.write("Done")
 
         print("Bye!")
         import sys
+
         sys.stdout.flush()
         os.kill(os.getpid(), 11)
 
         with open(self.get_output_file_name("some_other_file.txt"), "w") as f:
             f.write("Done")
```

### Comparing `b2luigi-0.9.1/tests/core/dispatch_with_env_and_script.py` & `b2luigi-1.0.0/tests/core/dispatch_with_env_and_script.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/core/test_dispatch_task.py` & `b2luigi-1.0.0/tests/core/test_dispatch_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,8 +32,10 @@
             self.assertTrue(os.path.exists("logs/MyTask/stdout"))
 
             with open("logs/MyTask/stdout", "r") as f:
                 stdout_content = f.readlines()
                 self.assertIn("MY_SECRET_VARIABLE 42\n", stdout_content)
                 self.assertIn("MY_SECOND_SECRET_VARIABLE 47\n", stdout_content)
 
-            self.assertIn(b"This progress looks :) because there were no failed tasks or missing dependencies", out.splitlines())
+            self.assertIn(
+                b"This progress looks :) because there were no failed tasks or missing dependencies", out.splitlines()
+            )
```

### Comparing `b2luigi-0.9.1/tests/core/test_folder_structures.py` & `b2luigi-1.0.0/tests/core/test_folder_structures.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/core/test_parameter.py` & `b2luigi-1.0.0/tests/core/test_parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,11 +39,15 @@
             def run(self):
                 with open(self.get_output_file_name("test.txt"), "w") as f:
                     f.write("test")
 
             def output(self):
                 yield self.add_to_output("test.txt")
 
-        task = MyTask(my_parameter=["Some", "strange", "items", "with", "bad / signs"], custom_hashed_parameter=[0, 1, 2])
+        task = MyTask(
+            my_parameter=["Some", "strange", "items", "with", "bad / signs"], custom_hashed_parameter=[0, 1, 2]
+        )
 
-        expected_path = "results/my_parameter=hashed_08928069d368e4a0f8ac02a0193e443b/custom_hashed_parameter=0_1_2/test.txt"
+        expected_path = (
+            "results/my_parameter=hashed_08928069d368e4a0f8ac02a0193e443b/custom_hashed_parameter=0_1_2/test.txt"
+        )
         self.assertTrue(task.get_output_file_name("test.txt").endswith(expected_path))
```

### Comparing `b2luigi-0.9.1/tests/core/test_requires.py` & `b2luigi-1.0.0/tests/core/test_requires.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,30 @@
         self.assertTrue(input_files[0].endswith("results/some_parameter=3/some_other_parameter=1/test.txt"))
 
         required_task = next(task.requires())
         self.assertEqual(sorted(required_task.get_param_names()), ["some_other_parameter", "some_parameter"])
         self.assertEqual(required_task.some_parameter, 3)
         self.assertEqual(required_task.some_other_parameter, 1)
         self.assertTrue(
-            required_task.get_output_file_name("test.txt").endswith("results/some_parameter=3/some_other_parameter=1/test.txt")
+            required_task.get_output_file_name("test.txt").endswith(
+                "results/some_parameter=3/some_other_parameter=1/test.txt"
+            )
         )
 
 
 class InheritsTestCase(B2LuigiTestCase):
     def test_inherits(self):
         class TaskA(b2luigi.Task):
             some_parameter = b2luigi.IntParameter()
             some_other_parameter = b2luigi.IntParameter()
 
             def output(self):
                 yield self.add_to_output("test.txt")
 
-        @b2luigi.inherits(TaskA, without='some_other_parameter')
+        @b2luigi.inherits(TaskA, without="some_other_parameter")
         class TaskB(b2luigi.Task):
             another_parameter = b2luigi.IntParameter()
 
             def requires(self):
                 for my_other_parameter in range(10):
                     yield self.clone(TaskA, some_other_parameter=my_other_parameter)
 
@@ -65,30 +67,32 @@
             def output(self):
                 yield self.add_to_output("out.dat")
 
         task = TaskB(some_parameter=23, another_parameter=42)
         self.assertEqual(task.get_param_names(), ["some_parameter", "another_parameter"])
         self.assertEqual(task.another_parameter, 42)
         self.assertEqual(task.some_parameter, 23)
-        self.assertFalse(hasattr(task, 'some_other_parameter'))
+        self.assertFalse(hasattr(task, "some_other_parameter"))
 
         self.assertTrue(
             task.get_output_file_name("out.dat").endswith("results/some_parameter=23/another_parameter=42/out.dat")
         )
 
         input_files = task.get_input_file_names("test.txt")
         self.assertEqual(len(input_files), 10)
         for my_other_parameter in range(10):
-            self.assertTrue(input_files[my_other_parameter]
-                            .endswith(f"results/some_parameter=23/some_other_parameter={my_other_parameter}/test.txt")
-                            )
+            self.assertTrue(
+                input_files[my_other_parameter].endswith(
+                    f"results/some_parameter=23/some_other_parameter={my_other_parameter}/test.txt"
+                )
+            )
 
         required_tasks = list(task.requires())
         for some_other_parameter_values, required_task in enumerate(required_tasks):
             self.assertEqual(sorted(required_task.get_param_names()), ["some_other_parameter", "some_parameter"])
             self.assertEqual(required_task.some_other_parameter, some_other_parameter_values)
             self.assertEqual(required_task.some_parameter, 23)
             self.assertTrue(
-                required_task
-                .get_output_file_name("test.txt")
-                .endswith(f"results/some_parameter=23/some_other_parameter={some_other_parameter_values}/test.txt")
+                required_task.get_output_file_name("test.txt").endswith(
+                    f"results/some_parameter=23/some_other_parameter={some_other_parameter_values}/test.txt"
+                )
             )
```

### Comparing `b2luigi-0.9.1/tests/core/test_settings.py` & `b2luigi-1.0.0/tests/core/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,26 @@
         setattr(task, "my_third_setting", "my task value")
 
         self.assertEqual("my file value", b2luigi.get_setting("my_setting", task=task))
         self.assertEqual("my value", b2luigi.get_setting("my_second_setting", task=task))
         self.assertEqual("my task value", b2luigi.get_setting("my_third_setting", task=task))
 
     def test_deprecated_settings(self):
-        self.assertRaises(ValueError, b2luigi.get_setting, key="my_setting",
-                          deprecated_keys=["my_old_setting"])
+        self.assertRaises(ValueError, b2luigi.get_setting, key="my_setting", deprecated_keys=["my_old_setting"])
 
         b2luigi.set_setting("my_old_setting", "my value")
 
         with warnings.catch_warnings(record=True) as w:
-            self.assertEqual("my value", b2luigi.get_setting("my_setting",
-                                                             deprecated_keys=["my_old_setting"]))
+            self.assertEqual("my value", b2luigi.get_setting("my_setting", deprecated_keys=["my_old_setting"]))
 
             self.assertEqual(len(w), 1)
             self.assertIsInstance(w[-1].message, DeprecatedSettingsWarning)
             self.assertIn("deprecated", str(w[-1].message))
 
         b2luigi.set_setting("my_setting", "my new_value")
 
         with warnings.catch_warnings(record=True) as w:
-            self.assertEqual("my new_value", b2luigi.get_setting("my_setting", default="default",
-                                                                 deprecated_keys=["my_old_setting"]))
+            self.assertEqual(
+                "my new_value", b2luigi.get_setting("my_setting", default="default", deprecated_keys=["my_old_setting"])
+            )
 
             self.assertEqual(len(w), 0)
```

### Comparing `b2luigi-0.9.1/tests/core/test_task.py` & `b2luigi-1.0.0/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/core/test_temporary_files.py` & `b2luigi-1.0.0/tests/core/test_temporary_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
         self.assertTrue(os.path.exists("test.txt"))
 
         with open("test.txt", "r") as f:
             self.assertEqual(f.read(), "Test")
 
     def test_reset_output(self):
-
         class MyTask(b2luigi.Task):
             def output(self):
                 yield self.add_to_output("test.txt")
 
             @b2luigi.on_temporary_files
             def run(self):
                 with open(self.get_output_file_name("test.txt"), "w") as f:
```

### Comparing `b2luigi-0.9.1/tests/core/test_utils.py` & `b2luigi-1.0.0/tests/core/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from unittest import TestCase, mock
 
 import b2luigi
 from b2luigi.core import utils
+from ..helpers import B2LuigiTestCase
 
 
 class ProductDictTestCase(TestCase):
     def test_basic_usage(self):
         kwargs = list(utils.product_dict(first_arg=[1, 2, 3], second_arg=["a", "b"]))
 
         self.assertEqual(len(kwargs), 6)
@@ -145,14 +146,52 @@
 
         self.assertIn("key1", outputs)
         self.assertEqual(outputs["key1"], ["value1", "repeated"])
         self.assertIn("key2", outputs)
         self.assertEqual(outputs["key2"], ["value2"])
 
 
+class OutputFileNameTestCase(B2LuigiTestCase):
+    dummy_dir = "/foo/bar/"
+    dummy_filename = "/foo/bar/run.py"
+    dummy_parameter = "foo"
+
+    def _get_dummy_task(self, parameter):
+        class MyTask(b2luigi.Task):
+            parameter = b2luigi.Parameter()
+
+        task = MyTask(parameter)
+        return task
+
+    def test_output_file_name_basename(self):
+        """
+        Test that utils.create_output_file_name will return the expected output filename path
+        """
+        test_task = self._get_dummy_task(self.dummy_parameter)
+        output = utils.create_output_file_name(
+            test_task, base_filename="output.txt", result_dir=f"{self.test_dir}/results"
+        )
+
+        self.assertEqual(output, f"{self.test_dir}/results/parameter={self.dummy_parameter}/output.txt")
+
+    def test_output_file_name_basename_error(self):
+        """
+        Test that utils.create_output_file_name will raise an error if a parameter contains
+        path separator "/" or is not interpretable as basename due to other reasons.
+        """
+
+        test_task_dir = self._get_dummy_task(self.dummy_dir)
+        with self.assertRaises(ValueError):
+            utils.create_output_file_name(test_task_dir, base_filename="output.txt")
+
+        test_task_filename = self._get_dummy_task(self.dummy_filename)
+        with self.assertRaises(ValueError):
+            utils.create_output_file_name(test_task_filename, base_filename="output.txt")
+
+
 class MapFolderTestCase(TestCase):
     dummy_rel_dir = "./some/rel_dir"
     dummy_abs_dir = "/path/to/some/abs_dir"
     main_no_file_file_err_msg = "module '__main__' has no attribute '__file__'"
 
     def test_map_folder_abspath_identity(self):
         """Test that for an absolute path, map_folder returns and identity"""
@@ -160,17 +199,15 @@
 
     def test_map_folder_relpath(self):
         """
         Test map_folder with a relative input_folder, which joins it with ``__main__.__file__``
         """
         with mock.patch("__main__.__file__", self.dummy_abs_dir):
             mapped_folder = utils.map_folder(self.dummy_rel_dir)
-            self.assertEqual(
-                mapped_folder, os.path.join(self.dummy_abs_dir, mapped_folder)
-            )
+            self.assertEqual(mapped_folder, os.path.join(self.dummy_abs_dir, mapped_folder))
 
     def test_map_folder_abspath_identity_when_no_filename(self):
         """
         Test that for an absolute path, map_folder returns and identity even
         if ``get_filename`` would raise an ``AttributeError`` because ``__main__.__file__``
         is not available (e.g. in jupyter)
         """
@@ -221,17 +258,15 @@
 
     def test_additional_info_added_to_error(self):
         """
         Check that the error message of ``map_folder`` adds additional
         information to the ``AttributeError`` raised by ``get_filename``
         """
         message = self._get_map_folder_error_mesage()
-        self.assertTrue(
-            message.startswith("Could not determine the current script location.")
-        )
+        self.assertTrue(message.startswith("Could not determine the current script location."))
 
 
 class TaskIteratorTestCase(TestCase):
     def test_task_iterator_unique_tasks(self):
         """
         Test that even when multiple worker tasks require same common
         dependency task, it appears only once in task iterator output.
@@ -256,11 +291,9 @@
         expected_task_str_order = [
             "AggregatorTask()",
             "WorkerTask(some_parameter=0)",
             "CommonDependencyTask()",
             "WorkerTask(some_parameter=1)",
             "WorkerTask(some_parameter=2)",
         ]
-        resulting_task_str_order = [
-            str(t) for t in utils.task_iterator(AggregatorTask())
-        ]
+        resulting_task_str_order = [str(t) for t in utils.task_iterator(AggregatorTask())]
         self.assertListEqual(expected_task_str_order, resulting_task_str_order)
```

### Comparing `b2luigi-0.9.1/tests/doc_examples/dict_requirement_example.py` & `b2luigi-1.0.0/tests/doc_examples/dict_requirement_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 
 
 class TaskA(luigi.Task):
     central_value = luigi.FloatParameter()
     index = luigi.IntParameter()
 
     def run(self):
-
         with open(self.get_output_file_name("random_numbers.txt"), "w") as f:
             for _ in range(1000):
                 f.write(f"{random.gauss(self.central_value, 0.0)}\n")
 
     def output(self):
         yield self.add_to_output("random_numbers.txt")
 
 
 class TaskB(luigi.Task):
-
     def requires(self):
         self.required_tasks = {
             "a": (TaskA(5.0, i) for i in range(100)),
             "b": (TaskA(1.0, i) for i in range(100)),
         }
         return self.required_tasks
```

### Comparing `b2luigi-0.9.1/tests/doc_examples/simple_example.py` & `b2luigi-1.0.0/tests/doc_examples/simple_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,9 +12,8 @@
         random_number = random.random()
         with self.output().open("w") as f:
             f.write(f"{random_number}\n")
 
 
 if __name__ == "__main__":
     b2luigi.set_setting("result_dir", "results")
-    b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)],
-                    workers=200)
+    b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)], workers=200)
```

### Comparing `b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi.py` & `b2luigi-1.0.0/tests/doc_examples/simple_example_b2luigi.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,8 @@
 
         with open(self.get_output_file_name("output_file.txt"), "w") as f:
             f.write(f"{random_number}\n")
 
 
 if __name__ == "__main__":
     b2luigi.set_setting("result_dir", "results")
-    b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)],
-                    workers=200)
+    b2luigi.process([MyNumberTask(some_parameter=i) for i in range(100)], workers=200)
```

### Comparing `b2luigi-0.9.1/tests/doc_examples/simple_example_b2luigi_2.py` & `b2luigi-1.0.0/tests/doc_examples/simple_example_b2luigi_2.py`

 * *Files identical despite different names*

### Comparing `b2luigi-0.9.1/tests/helpers.py` & `b2luigi-1.0.0/tests/helpers.py`

 * *Files identical despite different names*

