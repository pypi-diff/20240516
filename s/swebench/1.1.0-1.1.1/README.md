# Comparing `tmp/swebench-1.1.0.tar.gz` & `tmp/swebench-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.1.0.tar", last modified: Mon Apr 15 22:20:59 2024, max compression
+gzip compressed data, was "swebench-1.1.1.tar", last modified: Wed May 15 17:02:20 2024, max compression
```

## Comparing `swebench-1.1.0.tar` & `swebench-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592880 swebench-1.1.0/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.1.0/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     7060 2024-04-15 22:20:59.592808 swebench-1.1.0/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5984 2024-04-15 22:20:09.000000 swebench-1.1.0/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.585261 swebench-1.1.0/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.585907 swebench-1.1.0/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.587150 swebench-1.1.0/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.1.0/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.1.0/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.1.0/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-15 22:20:59.593083 swebench-1.1.0/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1345 2024-04-11 15:11:14.000000 swebench-1.1.0/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.587362 swebench-1.1.0/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-15 19:56:17.000000 swebench-1.1.0/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.588886 swebench-1.1.0/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.590151 swebench-1.1.0/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    22114 2024-04-15 16:06:14.000000 swebench-1.1.0/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    31433 2024-04-12 18:56:31.000000 swebench-1.1.0/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7725 2024-04-12 18:56:55.000000 swebench-1.1.0/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6420 2024-04-12 18:57:04.000000 swebench-1.1.0/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10412 2024-04-10 19:23:48.000000 swebench-1.1.0/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.1.0/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.591473 swebench-1.1.0/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      430 2024-04-11 01:17:37.000000 swebench-1.1.0/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4504 2024-04-11 01:17:58.000000 swebench-1.1.0/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.1.0/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4339 2024-04-11 01:18:16.000000 swebench-1.1.0/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    12244 2024-04-12 18:57:17.000000 swebench-1.1.0/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592347 swebench-1.1.0/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592542 swebench-1.1.0/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     7060 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       81 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455605 swebench-1.1.1/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.1.1/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-15 17:02:20.455538 swebench-1.1.1/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6152 2024-05-14 14:58:38.000000 swebench-1.1.1/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.449327 swebench-1.1.1/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.449721 swebench-1.1.1/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.450725 swebench-1.1.1/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.1.1/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.1.1/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.1.1/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.1.1/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.1.1/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-05-15 17:02:20.455807 swebench-1.1.1/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1345 2024-04-11 15:11:14.000000 swebench-1.1.1/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.450894 swebench-1.1.1/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-05-15 17:02:09.000000 swebench-1.1.1/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.452420 swebench-1.1.1/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.453459 swebench-1.1.1/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    22289 2024-05-15 16:59:23.000000 swebench-1.1.1/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31433 2024-04-24 17:18:05.000000 swebench-1.1.1/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     8028 2024-04-16 16:21:16.000000 swebench-1.1.1/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6420 2024-04-12 18:57:04.000000 swebench-1.1.1/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10412 2024-04-10 19:23:48.000000 swebench-1.1.1/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14757 2024-05-15 16:59:46.000000 swebench-1.1.1/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.454583 swebench-1.1.1/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      430 2024-04-11 01:17:37.000000 swebench-1.1.1/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4504 2024-04-11 01:17:58.000000 swebench-1.1.1/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.1.1/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4339 2024-04-11 01:18:16.000000 swebench-1.1.1/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    12244 2024-04-12 18:57:17.000000 swebench-1.1.1/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455104 swebench-1.1.1/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.1.1/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-05-15 17:02:20.455262 swebench-1.1.1/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7228 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       81 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-05-15 17:02:20.000000 swebench-1.1.1/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.1.0/LICENSE` & `swebench-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/PKG-INFO` & `swebench-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.1.0
+Version: 1.1.1
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -56,24 +56,30 @@
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 📰 News
-* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240415_eval_bug/README.md).
 * **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
 * **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
+To access SWE-bench, copy and run the following code:
+```python
+from datasets import load_dataset
+swebench = load_dataset('princeton-nlp/SWE-bench', split='test')
+```
+
 ## 🚀 Set Up
 To build SWE-bench from source, follow these steps:
 1. Clone this repository locally
 2. `cd` into the repository.
 3. Run `conda env create -f environment.yml` to created a conda environment named `swe-bench`
 4. Activate the environment with `conda activate swe-bench`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.1.0 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.1 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -22,42 +22,45 @@
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
 benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
 improvements to resolve issues with the evaluation harness. Read more in our
 [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
-20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+20240415_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
 agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
 the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
 jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
 been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
 openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
 for evaluating large language models on real world software issues collected
 from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
-generating a *patch* that resolves the described problem. [assets/teaser.png]##
-ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
-repository locally 2. `cd` into the repository. 3. Run `conda env create -
-f environment.yml` to created a conda environment named `swe-bench` 4. Activate
-the environment with `conda activate swe-bench` ## ð½ Usage You can download
-the SWE-bench dataset directly ([dev](https://drive.google.com/
-uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
-drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
-or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
-To use SWE-Bench, you can: * Train your own models on our pre-processed
-datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-main/inference/) on existing models (either models you have on-disk like LLaMA,
-or models you have access to through an API like GPT-4). The inference step is
-where you get a repo and an issue and have the model try to generate a fix for
-it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
-harness/) models against SWE-bench. This is where you take a SWE-Bench task and
-a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
-collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
-swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
-â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
+generating a *patch* that resolves the described problem. [assets/teaser.png]To
+access SWE-bench, copy and run the following code: ```python from datasets
+import load_dataset swebench = load_dataset('princeton-nlp/SWE-bench',
+split='test') ``` ## ð Set Up To build SWE-bench from source, follow these
+steps: 1. Clone this repository locally 2. `cd` into the repository. 3. Run
+`conda env create -f environment.yml` to created a conda environment named
+`swe-bench` 4. Activate the environment with `conda activate swe-bench` ## ð½
+Usage You can download the SWE-bench dataset directly ([dev](https://
+drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX),
+[test](https://drive.google.com/
+uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from
+[HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench). To use
+SWE-Bench, you can: * Train your own models on our pre-processed datasets * Run
+[inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on
+existing models (either models you have on-disk like LLaMA, or models you have
+access to through an API like GPT-4). The inference step is where you get a
+repo and an issue and have the model try to generate a fix for it. * [Evaluate]
+(https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models
+against SWE-bench. This is where you take a SWE-Bench task and a model-proposed
+solution and evaluate its correctness. * Run SWE-bench's [data collection
+procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+collect/) on your own repositories, to make new SWE-Bench tasks. ## â¬ï¸
+Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
 Llama-7b) | | [ð¤ BM25 Retrieval 27K](https://huggingface.co/datasets/
```

### Comparing `swebench-1.1.0/README.md` & `swebench-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,24 +26,30 @@
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 📰 News
-* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240415_eval_bug/README.md).
 * **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
 * **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
+To access SWE-bench, copy and run the following code:
+```python
+from datasets import load_dataset
+swebench = load_dataset('princeton-nlp/SWE-bench', split='test')
+```
+
 ## 🚀 Set Up
 To build SWE-bench from source, follow these steps:
 1. Clone this repository locally
 2. `cd` into the repository.
 3. Run `conda env create -f environment.yml` to created a conda environment named `swe-bench`
 4. Activate the environment with `conda activate swe-bench`
```

#### html2text {}

```diff
@@ -8,42 +8,45 @@
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
 benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
 improvements to resolve issues with the evaluation harness. Read more in our
 [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
-20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+20240415_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
 agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
 the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
 jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
 been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
 openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
 for evaluating large language models on real world software issues collected
 from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
-generating a *patch* that resolves the described problem. [assets/teaser.png]##
-ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
-repository locally 2. `cd` into the repository. 3. Run `conda env create -
-f environment.yml` to created a conda environment named `swe-bench` 4. Activate
-the environment with `conda activate swe-bench` ## ð½ Usage You can download
-the SWE-bench dataset directly ([dev](https://drive.google.com/
-uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
-drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
-or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
-To use SWE-Bench, you can: * Train your own models on our pre-processed
-datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-main/inference/) on existing models (either models you have on-disk like LLaMA,
-or models you have access to through an API like GPT-4). The inference step is
-where you get a repo and an issue and have the model try to generate a fix for
-it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
-harness/) models against SWE-bench. This is where you take a SWE-Bench task and
-a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
-collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
-swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
-â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
+generating a *patch* that resolves the described problem. [assets/teaser.png]To
+access SWE-bench, copy and run the following code: ```python from datasets
+import load_dataset swebench = load_dataset('princeton-nlp/SWE-bench',
+split='test') ``` ## ð Set Up To build SWE-bench from source, follow these
+steps: 1. Clone this repository locally 2. `cd` into the repository. 3. Run
+`conda env create -f environment.yml` to created a conda environment named
+`swe-bench` 4. Activate the environment with `conda activate swe-bench` ## ð½
+Usage You can download the SWE-bench dataset directly ([dev](https://
+drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX),
+[test](https://drive.google.com/
+uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from
+[HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench). To use
+SWE-Bench, you can: * Train your own models on our pre-processed datasets * Run
+[inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on
+existing models (either models you have on-disk like LLaMA, or models you have
+access to through an API like GPT-4). The inference step is where you get a
+repo and an issue and have the model try to generate a fix for it. * [Evaluate]
+(https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models
+against SWE-bench. This is where you take a SWE-Bench task and a model-proposed
+solution and evaluate its correctness. * Run SWE-bench's [data collection
+procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+collect/) on your own repositories, to make new SWE-Bench tasks. ## â¬ï¸
+Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
 Llama-7b) | | [ð¤ BM25 Retrieval 27K](https://huggingface.co/datasets/
```

### Comparing `swebench-1.1.0/inference/llamao/distributed_attention.py` & `swebench-1.1.1/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/llamao/modeling_flash_llama.py` & `swebench-1.1.1/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/bm25_retrieval.py` & `swebench-1.1.1/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/create_instance.py` & `swebench-1.1.1/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/create_text_dataset.py` & `swebench-1.1.1/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/eval_retrieval.py` & `swebench-1.1.1/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/tokenize_dataset.py` & `swebench-1.1.1/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/make_datasets/utils.py` & `swebench-1.1.1/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/run_api.py` & `swebench-1.1.1/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/run_live.py` & `swebench-1.1.1/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/inference/run_llama.py` & `swebench-1.1.1/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/setup.py` & `swebench-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/__init__.py` & `swebench-1.1.1/swebench/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.1.0/swebench/collect/build_dataset.py` & `swebench-1.1.1/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/collect/build_dataset_ft.py` & `swebench-1.1.1/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/collect/get_tasks_pipeline.py` & `swebench-1.1.1/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/collect/get_top_pypi.py` & `swebench-1.1.1/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/collect/print_pulls.py` & `swebench-1.1.1/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/collect/utils.py` & `swebench-1.1.1/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/harness/constants.py` & `swebench-1.1.1/swebench/harness/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,14 +519,15 @@
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.9"}
     for k in ['2.1', '2.2']})
 MAP_VERSION_TO_INSTALL_PYDICOM.update({
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.10"}
     for k in ['2.3']})
 
 MAP_VERSION_TO_INSTALL_HUMANEVAL= {k: { "python": "3.9" } for k in ['1.0']}
+MAP_VERSION_TO_INSTALL_HUMANEVALFIX_PYTHON = {k: { "python": "3.9" } for k in ['1.0']}
 
 # Constants - Task Instance Instllation Environment
 MAP_VERSION_TO_INSTALL = {
     "astropy/astropy": MAP_VERSION_TO_INSTALL_ASTROPY,
     "django/django": MAP_VERSION_TO_INSTALL_DJANGO,
     "matplotlib/matplotlib": MAP_VERSION_TO_INSTALL_MATPLOTLIB,
     "marshmallow-code/marshmallow": MAP_VERSION_TO_INSTALL_MARSHMALLOW,
@@ -539,15 +540,16 @@
     "pylint-dev/astroid": MAP_VERSION_TO_INSTALL_ASTROID,
     "pylint-dev/pylint": MAP_VERSION_TO_INSTALL_PYLINT,
     "pytest-dev/pytest": MAP_VERSION_TO_INSTALL_PYTEST,
     "pyvista/pyvista": MAP_VERSION_TO_INSTALL_PYVISTA,
     "scikit-learn/scikit-learn": MAP_VERSION_TO_INSTALL_SKLEARN,
     "sphinx-doc/sphinx": MAP_VERSION_TO_INSTALL_SPHINX,
     "sqlfluff/sqlfluff": MAP_VERSION_TO_INSTALL_SQLFLUFF,
-    "swe-bench/humaneval": MAP_VERSION_TO_INSTALL_HUMANEVAL,
+    "humaneval": MAP_VERSION_TO_INSTALL_HUMANEVAL,
+    "humanevalfix-python": MAP_VERSION_TO_INSTALL_HUMANEVALFIX_PYTHON,
     "sympy/sympy": MAP_VERSION_TO_INSTALL_SYMPY,
 }
 
 # Constants - Repository Specific Installation Instructions
 MAP_REPO_TO_INSTALL = {}
 
 # Constants - Task Instance Test Frameworks
@@ -566,15 +568,16 @@
     "pylint-dev/astroid": TEST_PYTEST,
     "pylint-dev/pylint": TEST_PYTEST,
     "pytest-dev/pytest": "pytest -rA",
     "pyvista/pyvista": TEST_PYTEST,
     "scikit-learn/scikit-learn": TEST_PYTEST,
     "sphinx-doc/sphinx": "tox -epy39 -v --",
     "sqlfluff/sqlfluff": TEST_PYTEST,
-    "swe-bench/humaneval": "python",
+    "humaneval": "python",
+    "humanevalfix-python": "python",
     "sympy/sympy": "bin/test -C --verbose",
 }
 
 # Constants - Task Instance Requirements File Paths
 MAP_REPO_TO_REQS_PATHS = {
     "django/django": ["tests/requirements/py3.txt"],
     "matplotlib/matplotlib": ["requirements/dev/dev-requirements.txt", "requirements/testing/travis_all.txt"],
```

### Comparing `swebench-1.1.0/swebench/harness/context_manager.py` & `swebench-1.1.1/swebench/harness/context_manager.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/harness/engine_evaluation.py` & `swebench-1.1.1/swebench/harness/engine_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,22 +105,27 @@
         ) as tcm:
             # Attempt to set up environment with task instance
             if not tcm.reset_task_env(task_instance):
                 continue
 
             # Attempt to apply prediction
             patch_type = PatchType.PATCH_PRED_TRY.value
+
+            # If prediction patch doesn't apply, try to do some minor patch refactoring and try again
             if not tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type) \
-                and task_instance[KEY_PREDICTION] is not None:
+                and task_instance[KEY_PREDICTION] is not None \
+                and task_instance[KEY_PREDICTION] != "":
                 task_instance[KEY_PREDICTION] = extract_minimal_patch(task_instance[KEY_PREDICTION])
                 patch_type = PatchType.PATCH_PRED_MINIMAL_TRY.value
                 if not tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type):
+                    # Continue if edited patch still doesn't apply
                     continue
             tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type, revert=True)
 
+            # Set prediction patch label based on whether patch was edited
             if patch_type == PatchType.PATCH_PRED_MINIMAL_TRY.value:
                 patch_type = PatchType.PATCH_PRED_MINIMAL.value
             else:
                 patch_type = PatchType.PATCH_PRED.value
 
             # Run installation + testing script
             if (
```

### Comparing `swebench-1.1.0/swebench/harness/engine_validation.py` & `swebench-1.1.1/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/harness/run_evaluation.py` & `swebench-1.1.1/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/harness/utils.py` & `swebench-1.1.1/swebench/harness/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,18 @@
 
     Args:
         instance (dict): task instance
     Returns:
         directives (list): List of test directives
     """
     # For seq2seq code repos, testing command is fixed
-    if instance["repo"] == "swe-bench/humaneval":
+    if any([
+        x == instance["repo"] for x in
+        ["humaneval", "humanevalfix-python"]
+    ]):
         return ["test.py"]
 
     # Get test directives from test patch and remove non-test files
     diff_pat = r"diff --git a/.* b/(.*)"
     test_patch = instance["test_patch"]
     directives = re.findall(diff_pat, test_patch)
     directives = [
```

### Comparing `swebench-1.1.0/swebench/metrics/conversion.py` & `swebench-1.1.1/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/metrics/getters.py` & `swebench-1.1.1/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/metrics/log_parsers.py` & `swebench-1.1.1/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/metrics/metrics.py` & `swebench-1.1.1/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/metrics/monitor.py` & `swebench-1.1.1/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/metrics/report.py` & `swebench-1.1.1/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/versioning/constants.py` & `swebench-1.1.1/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/versioning/get_versions.py` & `swebench-1.1.1/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench/versioning/utils.py` & `swebench-1.1.1/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.1.0/swebench.egg-info/PKG-INFO` & `swebench-1.1.1/swebench.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.1.0
+Version: 1.1.1
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -56,24 +56,30 @@
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 📰 News
-* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240415_eval_bug/README.md).
 * **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
 * **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
+To access SWE-bench, copy and run the following code:
+```python
+from datasets import load_dataset
+swebench = load_dataset('princeton-nlp/SWE-bench', split='test')
+```
+
 ## 🚀 Set Up
 To build SWE-bench from source, follow these steps:
 1. Clone this repository locally
 2. `cd` into the repository.
 3. Run `conda env create -f environment.yml` to created a conda environment named `swe-bench`
 4. Activate the environment with `conda activate swe-bench`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.1.0 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.1 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -22,42 +22,45 @@
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
 benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
 improvements to resolve issues with the evaluation harness. Read more in our
 [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
-20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+20240415_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
 agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
 the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
 jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
 been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
 openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
 for evaluating large language models on real world software issues collected
 from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
-generating a *patch* that resolves the described problem. [assets/teaser.png]##
-ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
-repository locally 2. `cd` into the repository. 3. Run `conda env create -
-f environment.yml` to created a conda environment named `swe-bench` 4. Activate
-the environment with `conda activate swe-bench` ## ð½ Usage You can download
-the SWE-bench dataset directly ([dev](https://drive.google.com/
-uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
-drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
-or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
-To use SWE-Bench, you can: * Train your own models on our pre-processed
-datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
-main/inference/) on existing models (either models you have on-disk like LLaMA,
-or models you have access to through an API like GPT-4). The inference step is
-where you get a repo and an issue and have the model try to generate a fix for
-it. * [Evaluate](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
-harness/) models against SWE-bench. This is where you take a SWE-Bench task and
-a model-proposed solution and evaluate its correctness. * Run SWE-bench's [data
-collection procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/
-swebench/collect/) on your own repositories, to make new SWE-Bench tasks. ##
-â¬ï¸ Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
+generating a *patch* that resolves the described problem. [assets/teaser.png]To
+access SWE-bench, copy and run the following code: ```python from datasets
+import load_dataset swebench = load_dataset('princeton-nlp/SWE-bench',
+split='test') ``` ## ð Set Up To build SWE-bench from source, follow these
+steps: 1. Clone this repository locally 2. `cd` into the repository. 3. Run
+`conda env create -f environment.yml` to created a conda environment named
+`swe-bench` 4. Activate the environment with `conda activate swe-bench` ## ð½
+Usage You can download the SWE-bench dataset directly ([dev](https://
+drive.google.com/uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX),
+[test](https://drive.google.com/
+uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets) or from
+[HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench). To use
+SWE-Bench, you can: * Train your own models on our pre-processed datasets * Run
+[inference](https://github.com/princeton-nlp/SWE-bench/blob/main/inference/) on
+existing models (either models you have on-disk like LLaMA, or models you have
+access to through an API like GPT-4). The inference step is where you get a
+repo and an issue and have the model try to generate a fix for it. * [Evaluate]
+(https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/harness/) models
+against SWE-bench. This is where you take a SWE-Bench task and a model-proposed
+solution and evaluate its correctness. * Run SWE-bench's [data collection
+procedure](https://github.com/princeton-nlp/SWE-bench/blob/main/swebench/
+collect/) on your own repositories, to make new SWE-Bench tasks. ## â¬ï¸
+Downloads | Datasets | Models | | - | - | | [ð¤ SWE-bench](https://
 huggingface.co/datasets/princeton-nlp/SWE-bench) | [ð¦ SWE-Llama 13b](https:/
 /huggingface.co/princeton-nlp/SWE-Llama-13b) | | [ð¤ "Oracle" Retrieval]
 (https://huggingface.co/datasets/princeton-nlp/SWE-bench_oracle) | [ð¦ SWE-
 Llama 13b (PEFT)](https://huggingface.co/princeton-nlp/SWE-Llama-13b-peft) | |
 [ð¤ BM25 Retrieval 13K](https://huggingface.co/datasets/princeton-nlp/SWE-
 bench_bm25_13K) | [ð¦ SWE-Llama 7b](https://huggingface.co/princeton-nlp/SWE-
 Llama-7b) | | [ð¤ BM25 Retrieval 27K](https://huggingface.co/datasets/
```

### Comparing `swebench-1.1.0/swebench.egg-info/SOURCES.txt` & `swebench-1.1.1/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

