# Comparing `tmp/dbt_af-0.4.2.tar.gz` & `tmp/dbt_af-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_af-0.4.2.tar", max compression
+gzip compressed data, was "dbt_af-0.4.3.tar", max compression
```

## Comparing `dbt_af-0.4.2.tar` & `dbt_af-0.4.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      193 2024-04-22 15:17:05.887171 dbt_af-0.4.2/AUTHORS
--rw-r--r--   0        0        0      580 2024-04-22 15:17:05.887171 dbt_af-0.4.2/LICENSE
--rw-r--r--   0        0        0     3551 2024-04-22 15:17:05.887171 dbt_af-0.4.2/README.md
--rw-r--r--   0        0        0       95 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/__init__.py
--rw-r--r--   0        0        0      809 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/backfill_dag_components.py
--rw-r--r--   0        0        0    15978 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/dag_components.py
--rw-r--r--   0        0        0    10831 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/dbt_af_builder.py
--rw-r--r--   0        0        0     2695 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/dbt_model_path_graph_builder.py
--rw-r--r--   0        0        0     5878 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/domain_dag.py
--rw-r--r--   0        0        0     1507 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/maintenance_dag_components.py
--rw-r--r--   0        0        0     4504 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/builder/task_dependencies.py
--rw-r--r--   0        0        0        0 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/common/__init__.py
--rw-r--r--   0        0        0      552 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/common/constants.py
--rw-r--r--   0        0        0     7473 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/common/scheduling.py
--rw-r--r--   0        0        0     1703 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/common/utils.py
--rw-r--r--   0        0        0      240 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/conf/__init__.py
--rw-r--r--   0        0        0     8134 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/conf/config.py
--rw-r--r--   0        0        0     4238 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/dags.py
--rw-r--r--   0        0        0        0 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/integrations/__init__.py
--rw-r--r--   0        0        0      200 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/integrations/mcd/__init__.py
--rw-r--r--   0        0        0      864 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/integrations/mcd/callbacks.py
--rw-r--r--   0        0        0     1610 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/integrations/mcd/dbt_core.py
--rw-r--r--   0        0        0        0 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/__init__.py
--rw-r--r--   0        0        0     9544 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/base.py
--rw-r--r--   0        0        0     1804 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/branch.py
--rw-r--r--   0        0        0     4865 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/kubernetes_pod.py
--rw-r--r--   0        0        0     6238 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/macros.py
--rw-r--r--   0        0        0     2416 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/run.py
--rw-r--r--   0        0        0    18787 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/operators/sensors.py
--rw-r--r--   0        0        0        0 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/parser/__init__.py
--rw-r--r--   0        0        0    13163 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/parser/dbt_node_model.py
--rw-r--r--   0        0        0     1731 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/parser/dbt_profiles.py
--rw-r--r--   0        0        0     2023 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af/parser/dbt_source_model.py
--rw-r--r--   0        0        0       56 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/conftest.py
--rw-r--r--   0        0        0      791 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/main.py
--rw-r--r--   0        0        0      316 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/pyproject.toml
--rw-r--r--   0        0        0      923 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/test_af_wait_name_too_long.py
--rw-r--r--   0        0        0     2242 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/test_all_dbt_models_exist.py
--rw-r--r--   0        0        0      183 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/test_dbt_node_model.py
--rw-r--r--   0        0        0      924 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
--rw-r--r--   0        0        0      717 2024-04-22 15:17:05.887171 dbt_af-0.4.2/dbt_af_functional_tests/test_kubernetes_profiles.py
--rw-r--r--   0        0        0     2541 2024-04-22 15:17:05.907171 dbt_af-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 15:17:05.907171 dbt_af-0.4.2/scripts/__init__.py
--rw-r--r--   0        0        0     3492 2024-04-22 15:17:05.907171 dbt_af-0.4.2/scripts/mini_dbt_project_generator.py
--rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 dbt_af-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      193 2024-05-16 14:49:41.064149 dbt_af-0.4.3/AUTHORS
+-rw-r--r--   0        0        0      580 2024-05-16 14:49:41.064149 dbt_af-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3551 2024-05-16 14:49:41.064149 dbt_af-0.4.3/README.md
+-rw-r--r--   0        0        0       95 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/backfill_dag_components.py
+-rw-r--r--   0        0        0    15978 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dag_components.py
+-rw-r--r--   0        0        0    10831 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dbt_af_builder.py
+-rw-r--r--   0        0        0     2695 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/dbt_model_path_graph_builder.py
+-rw-r--r--   0        0        0     5878 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/domain_dag.py
+-rw-r--r--   0        0        0     1507 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/maintenance_dag_components.py
+-rw-r--r--   0        0        0     4504 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/builder/task_dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/constants.py
+-rw-r--r--   0        0        0     7473 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/scheduling.py
+-rw-r--r--   0        0        0     1703 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/common/utils.py
+-rw-r--r--   0        0        0      240 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/conf/__init__.py
+-rw-r--r--   0        0        0     8134 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/conf/config.py
+-rw-r--r--   0        0        0     4238 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/dags.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/__init__.py
+-rw-r--r--   0        0        0      200 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/callbacks.py
+-rw-r--r--   0        0        0     1610 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/integrations/mcd/dbt_core.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/__init__.py
+-rw-r--r--   0        0        0     9544 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/base.py
+-rw-r--r--   0        0        0     1804 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/branch.py
+-rw-r--r--   0        0        0     4865 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0     6238 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/macros.py
+-rw-r--r--   0        0        0     2416 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/run.py
+-rw-r--r--   0        0        0    18787 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/operators/sensors.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/parser/__init__.py
+-rw-r--r--   0        0        0    13163 2024-05-16 14:49:41.064149 dbt_af-0.4.3/dbt_af/parser/dbt_node_model.py
+-rw-r--r--   0        0        0     1731 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af/parser/dbt_profiles.py
+-rw-r--r--   0        0        0     2023 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af/parser/dbt_source_model.py
+-rw-r--r--   0        0        0       56 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/conftest.py
+-rw-r--r--   0        0        0      791 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/main.py
+-rw-r--r--   0        0        0      316 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_af_wait_name_too_long.py
+-rw-r--r--   0        0        0     2242 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_all_dbt_models_exist.py
+-rw-r--r--   0        0        0      183 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_node_model.py
+-rw-r--r--   0        0        0      924 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py
+-rw-r--r--   0        0        0      717 2024-05-16 14:49:41.068149 dbt_af-0.4.3/dbt_af_functional_tests/test_kubernetes_profiles.py
+-rw-r--r--   0        0        0     2555 2024-05-16 14:49:41.084149 dbt_af-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 14:49:41.084149 dbt_af-0.4.3/scripts/__init__.py
+-rw-r--r--   0        0        0     3492 2024-05-16 14:49:41.084149 dbt_af-0.4.3/scripts/mini_dbt_project_generator.py
+-rw-r--r--   0        0        0     5003 1970-01-01 00:00:00.000000 dbt_af-0.4.3/PKG-INFO
```

### Comparing `dbt_af-0.4.2/LICENSE` & `dbt_af-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/README.md` & `dbt_af-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/__init__.py` & `dbt_af-0.4.3/dbt_af/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/backfill_dag_components.py` & `dbt_af-0.4.3/dbt_af/builder/backfill_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/dag_components.py` & `dbt_af-0.4.3/dbt_af/builder/dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/dbt_af_builder.py` & `dbt_af-0.4.3/dbt_af/builder/dbt_af_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/dbt_model_path_graph_builder.py` & `dbt_af-0.4.3/dbt_af/builder/dbt_model_path_graph_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/domain_dag.py` & `dbt_af-0.4.3/dbt_af/builder/domain_dag.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/maintenance_dag_components.py` & `dbt_af-0.4.3/dbt_af/builder/maintenance_dag_components.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/builder/task_dependencies.py` & `dbt_af-0.4.3/dbt_af/builder/task_dependencies.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/common/constants.py` & `dbt_af-0.4.3/dbt_af/common/constants.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/common/scheduling.py` & `dbt_af-0.4.3/dbt_af/common/scheduling.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/common/utils.py` & `dbt_af-0.4.3/dbt_af/common/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/conf/config.py` & `dbt_af-0.4.3/dbt_af/conf/config.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/dags.py` & `dbt_af-0.4.3/dbt_af/dags.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/integrations/mcd/callbacks.py` & `dbt_af-0.4.3/dbt_af/integrations/mcd/callbacks.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/integrations/mcd/dbt_core.py` & `dbt_af-0.4.3/dbt_af/integrations/mcd/dbt_core.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/base.py` & `dbt_af-0.4.3/dbt_af/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/branch.py` & `dbt_af-0.4.3/dbt_af/operators/branch.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/kubernetes_pod.py` & `dbt_af-0.4.3/dbt_af/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/macros.py` & `dbt_af-0.4.3/dbt_af/operators/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/run.py` & `dbt_af-0.4.3/dbt_af/operators/run.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/operators/sensors.py` & `dbt_af-0.4.3/dbt_af/operators/sensors.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/parser/dbt_node_model.py` & `dbt_af-0.4.3/dbt_af/parser/dbt_node_model.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/parser/dbt_profiles.py` & `dbt_af-0.4.3/dbt_af/parser/dbt_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af/parser/dbt_source_model.py` & `dbt_af-0.4.3/dbt_af/parser/dbt_source_model.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/conftest.py` & `dbt_af-0.4.3/dbt_af_functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/main.py` & `dbt_af-0.4.3/dbt_af_functional_tests/main.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/test_af_wait_name_too_long.py` & `dbt_af-0.4.3/dbt_af_functional_tests/test_af_wait_name_too_long.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/test_all_dbt_models_exist.py` & `dbt_af-0.4.3/dbt_af_functional_tests/test_all_dbt_models_exist.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py` & `dbt_af-0.4.3/dbt_af_functional_tests/test_dbt_nodes_general_constrains.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/dbt_af_functional_tests/test_kubernetes_profiles.py` & `dbt_af-0.4.3/dbt_af_functional_tests/test_kubernetes_profiles.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/pyproject.toml` & `dbt_af-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-af"
-version = "0.4.2"
+version = "0.4.3"
 description = "Distibuted dbt runs on Apache Airflow"
 authors = [
     "Nikita Yurasov <nikitayurasov@toloka.ai>",
     "Igor Safonov <igsaf@toloka.ai>",
     "Evgeny Ermakov <jkermakov@toloka.ai>",
     "Leonid Kozhinov <lkozhinov@toloka.ai>",
 ]
@@ -17,17 +17,17 @@
 packages = [
     { include = "dbt_af" },
     { include = "dbt_af_functional_tests" },
     { include = "scripts" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.10,<3.12"
 attrs = "~23.1"
-apache-airflow = ">=2.6,<2.8.0"
+apache-airflow = ">=2.6"
 pydantic = ">=1.10,<3.0.0"
 apache-airflow-providers-cncf-kubernetes = ">=7.0.0"
 cachetools = "~5.3"
 typer = "~0.9"
 dbt-core = "~1.7"
 pendulum = "^2"
 
@@ -44,14 +44,15 @@
 [tool.poetry.group.dev.dependencies]
 isort = "~5.12"
 black = "~23.7"
 ruff = "^0.3"
 twine = "*"
 pytest = "^8"
 pytest-env = "*"
+pytest-cov = "~4.1"
 pytest-socket = "*"
 pytest-mock = "*"
 dbt-postgres = "~1.7"
 dbt-databricks = "1.7.8"
 pre-commit = "3.6.2"
 
 [tool.poetry.extras]
```

### Comparing `dbt_af-0.4.2/scripts/mini_dbt_project_generator.py` & `dbt_af-0.4.3/scripts/mini_dbt_project_generator.py`

 * *Files identical despite different names*

### Comparing `dbt_af-0.4.2/PKG-INFO` & `dbt_af-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: dbt-af
-Version: 0.4.2
+Version: 0.4.3
 Summary: Distibuted dbt runs on Apache Airflow
 Home-page: https://github.com/Toloka/dbt-af
 License: Apache-2.0
 Keywords: python,airflow,dbt
 Author: Nikita Yurasov
 Author-email: nikitayurasov@toloka.ai
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: examples
 Provides-Extra: mcd
 Provides-Extra: minidbt
 Provides-Extra: tests
 Requires-Dist: airflow-mcd (>=0.2,<0.3) ; extra == "mcd"
-Requires-Dist: apache-airflow (>=2.6,<2.8.0)
+Requires-Dist: apache-airflow (>=2.6)
 Requires-Dist: apache-airflow-providers-cncf-kubernetes (>=7.0.0)
 Requires-Dist: attrs (>=23.1,<23.2)
 Requires-Dist: cachetools (>=5.3,<5.4)
 Requires-Dist: dbt-core (>=1.7,<1.8)
 Requires-Dist: dbt-postgres (>=1.7,<1.8) ; extra == "examples"
 Requires-Dist: pendulum (>=2,<3)
 Requires-Dist: pycarlo (>=0.8,<0.9) ; extra == "mcd"
```

