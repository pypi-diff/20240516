# Comparing `tmp/swebench-1.1.1.tar.gz` & `tmp/swebench-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.1.1.tar", last modified: Wed May 15 17:02:20 2024, max compression
+gzip compressed data, was "swebench-1.1.2.tar", last modified: Thu May 16 13:25:57 2024, max compression
```

## Comparing `swebench-1.1.1.tar` & `swebench-1.1.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455605 swebench-1.1.1/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.1.1/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-15 17:02:20.455538 swebench-1.1.1/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     6152 2024-05-14 14:58:38.000000 swebench-1.1.1/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.449327 swebench-1.1.1/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.449721 swebench-1.1.1/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.450725 swebench-1.1.1/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.1.1/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.1.1/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.1.1/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-05-15 17:02:20.455807 swebench-1.1.1/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1345 2024-04-11 15:11:14.000000 swebench-1.1.1/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.450894 swebench-1.1.1/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-05-15 17:02:09.000000 swebench-1.1.1/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.452420 swebench-1.1.1/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.453459 swebench-1.1.1/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    22289 2024-05-15 16:59:23.000000 swebench-1.1.1/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    31433 2024-04-24 17:18:05.000000 swebench-1.1.1/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     8028 2024-04-16 16:21:16.000000 swebench-1.1.1/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6420 2024-04-12 18:57:04.000000 swebench-1.1.1/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10412 2024-04-10 19:23:48.000000 swebench-1.1.1/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14757 2024-05-15 16:59:46.000000 swebench-1.1.1/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.454583 swebench-1.1.1/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      430 2024-04-11 01:17:37.000000 swebench-1.1.1/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4504 2024-04-11 01:17:58.000000 swebench-1.1.1/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.1.1/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4339 2024-04-11 01:18:16.000000 swebench-1.1.1/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    12244 2024-04-12 18:57:17.000000 swebench-1.1.1/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455104 swebench-1.1.1/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455262 swebench-1.1.1/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       81 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.219023 swebench-1.1.2/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.1.2/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-16 13:25:57.218955 swebench-1.1.2/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6152 2024-05-14 14:58:38.000000 swebench-1.1.2/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.211563 swebench-1.1.2/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.2/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.212116 swebench-1.1.2/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.2/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.213263 swebench-1.1.2/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.2/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.1.2/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.1.2/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.1.2/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.1.2/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.1.2/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.1.2/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-05-16 13:25:57.219233 swebench-1.1.2/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1345 2024-04-11 15:11:14.000000 swebench-1.1.2/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.213458 swebench-1.1.2/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-05-16 13:25:28.000000 swebench-1.1.2/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.215203 swebench-1.1.2/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.216410 swebench-1.1.2/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    22329 2024-05-16 13:22:25.000000 swebench-1.1.2/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31433 2024-05-15 22:20:48.000000 swebench-1.1.2/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     8028 2024-05-15 22:20:48.000000 swebench-1.1.2/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6420 2024-04-12 18:57:04.000000 swebench-1.1.2/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10412 2024-04-10 19:23:48.000000 swebench-1.1.2/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14757 2024-05-15 22:20:48.000000 swebench-1.1.2/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.217679 swebench-1.1.2/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      430 2024-04-11 01:17:37.000000 swebench-1.1.2/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4504 2024-04-11 01:17:58.000000 swebench-1.1.2/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.1.2/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4339 2024-04-11 01:18:16.000000 swebench-1.1.2/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    12244 2024-04-12 18:57:17.000000 swebench-1.1.2/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.218337 swebench-1.1.2/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.1.2/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-16 13:25:57.218659 swebench-1.1.2/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-16 13:25:57.000000 swebench-1.1.2/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-05-16 13:25:57.000000 swebench-1.1.2/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-05-16 13:25:57.000000 swebench-1.1.2/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       81 2024-05-16 13:25:57.000000 swebench-1.1.2/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-05-16 13:25:57.000000 swebench-1.1.2/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.1.1/LICENSE` & `swebench-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/PKG-INFO` & `swebench-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.1.1
+Version: 1.1.2
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.1.1 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.2 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.1.1/README.md` & `swebench-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/llamao/distributed_attention.py` & `swebench-1.1.2/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/llamao/modeling_flash_llama.py` & `swebench-1.1.2/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/bm25_retrieval.py` & `swebench-1.1.2/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/create_instance.py` & `swebench-1.1.2/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/create_text_dataset.py` & `swebench-1.1.2/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/eval_retrieval.py` & `swebench-1.1.2/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/tokenize_dataset.py` & `swebench-1.1.2/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/make_datasets/utils.py` & `swebench-1.1.2/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/run_api.py` & `swebench-1.1.2/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/run_live.py` & `swebench-1.1.2/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/inference/run_llama.py` & `swebench-1.1.2/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/setup.py` & `swebench-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/__init__.py` & `swebench-1.1.2/swebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.1.1/swebench/collect/build_dataset.py` & `swebench-1.1.2/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/collect/build_dataset_ft.py` & `swebench-1.1.2/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/collect/get_tasks_pipeline.py` & `swebench-1.1.2/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/collect/get_top_pypi.py` & `swebench-1.1.2/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/collect/print_pulls.py` & `swebench-1.1.2/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/collect/utils.py` & `swebench-1.1.2/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/harness/constants.py` & `swebench-1.1.2/swebench/harness/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,16 +540,16 @@
     "pylint-dev/astroid": MAP_VERSION_TO_INSTALL_ASTROID,
     "pylint-dev/pylint": MAP_VERSION_TO_INSTALL_PYLINT,
     "pytest-dev/pytest": MAP_VERSION_TO_INSTALL_PYTEST,
     "pyvista/pyvista": MAP_VERSION_TO_INSTALL_PYVISTA,
     "scikit-learn/scikit-learn": MAP_VERSION_TO_INSTALL_SKLEARN,
     "sphinx-doc/sphinx": MAP_VERSION_TO_INSTALL_SPHINX,
     "sqlfluff/sqlfluff": MAP_VERSION_TO_INSTALL_SQLFLUFF,
-    "humaneval": MAP_VERSION_TO_INSTALL_HUMANEVAL,
-    "humanevalfix-python": MAP_VERSION_TO_INSTALL_HUMANEVALFIX_PYTHON,
+    "swe-bench/humaneval": MAP_VERSION_TO_INSTALL_HUMANEVAL,
+    "swe-bench/humanevalfix-python": MAP_VERSION_TO_INSTALL_HUMANEVALFIX_PYTHON,
     "sympy/sympy": MAP_VERSION_TO_INSTALL_SYMPY,
 }
 
 # Constants - Repository Specific Installation Instructions
 MAP_REPO_TO_INSTALL = {}
 
 # Constants - Task Instance Test Frameworks
@@ -568,16 +568,16 @@
     "pylint-dev/astroid": TEST_PYTEST,
     "pylint-dev/pylint": TEST_PYTEST,
     "pytest-dev/pytest": "pytest -rA",
     "pyvista/pyvista": TEST_PYTEST,
     "scikit-learn/scikit-learn": TEST_PYTEST,
     "sphinx-doc/sphinx": "tox -epy39 -v --",
     "sqlfluff/sqlfluff": TEST_PYTEST,
-    "humaneval": "python",
-    "humanevalfix-python": "python",
+    "swe-bench/humaneval": "python",
+    "swe-bench/humanevalfix-python": "python",
     "sympy/sympy": "bin/test -C --verbose",
 }
 
 # Constants - Task Instance Requirements File Paths
 MAP_REPO_TO_REQS_PATHS = {
     "django/django": ["tests/requirements/py3.txt"],
     "matplotlib/matplotlib": ["requirements/dev/dev-requirements.txt", "requirements/testing/travis_all.txt"],
```

### Comparing `swebench-1.1.1/swebench/harness/context_manager.py` & `swebench-1.1.2/swebench/harness/context_manager.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/harness/engine_evaluation.py` & `swebench-1.1.2/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/harness/engine_validation.py` & `swebench-1.1.2/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/harness/run_evaluation.py` & `swebench-1.1.2/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/harness/utils.py` & `swebench-1.1.2/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/conversion.py` & `swebench-1.1.2/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/getters.py` & `swebench-1.1.2/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/log_parsers.py` & `swebench-1.1.2/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/metrics.py` & `swebench-1.1.2/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/monitor.py` & `swebench-1.1.2/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/metrics/report.py` & `swebench-1.1.2/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/versioning/constants.py` & `swebench-1.1.2/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/versioning/get_versions.py` & `swebench-1.1.2/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench/versioning/utils.py` & `swebench-1.1.2/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.1/swebench.egg-info/PKG-INFO` & `swebench-1.1.2/swebench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.1.1
+Version: 1.1.2
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.1.1 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.2 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.1.1/swebench.egg-info/SOURCES.txt` & `swebench-1.1.2/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*
