# Comparing `tmp/vectordb-bench-0.0.7.tar.gz` & `tmp/vectordb_bench-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectordb-bench-0.0.7.tar", last modified: Wed Mar 13 09:55:39 2024, max compression
+gzip compressed data, was "vectordb_bench-0.0.8.tar", last modified: Tue Apr 23 06:25:46 2024, max compression
```

## Comparing `vectordb-bench-0.0.7.tar` & `vectordb_bench-0.0.8.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.954230 vectordb-bench-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.934230 vectordb-bench-0.0.7/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.926230 vectordb-bench-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.934230 vectordb-bench-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.github/workflows/publish_package_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/OWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-03-13 09:55:39.954230 vectordb-bench-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20178 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.934230 vectordb-bench-0.0.7/install/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/install/requirements_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 09:55:39.954230 vectordb-bench-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.938230 vectordb-bench-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_bench_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_chroma.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_elasticsearch_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/tests/ut_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.938230 vectordb-bench-0.0.7/vectordb_bench/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/chroma/
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/chroma/chroma.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/chroma/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/elastic_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/elastic_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/milvus/
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/milvus/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/milvus/milvus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvecto_rs/
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvecto_rs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvecto_rs/pgvecto_rs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvector/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvector/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvector/pgvector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pinecone/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pinecone/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/pinecone/pinecone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/qdrant_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/qdrant_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/redis/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.942230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/weaviate_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/weaviate_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.946230 vectordb-bench-0.0.7/vectordb_bench/backend/clients/zilliz_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/zilliz_cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/result_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.946230 vectordb-bench-0.0.7/vectordb_bench/backend/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/runner/mp_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/runner/serial_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/task_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/backend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.946230 vectordb-bench-0.0.7/vectordb_bench/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.930230 vectordb-bench-0.0.7/vectordb_bench/frontend/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.946230 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/expanderStyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/headerIcon.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/priceTable.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/stPageConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.946230 vectordb-bench-0.0.7/vectordb_bench/frontend/components/get_results/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/get_results/saveAsImage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/autoRefresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/caseSelector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/dbSelector.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/generateTasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/hideSidebar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/submitTask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/frontend/const/
--rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/const/dbCaseConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/const/dbPrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/const/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/frontend/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/pages/quries_per_dollar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/pages/run_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/frontend/vdb_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/log_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/ElasticCloud/
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/ElasticCloud/result_20230727_standard_elasticcloud.json
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/ElasticCloud/result_20230808_standard_elasticcloud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/Milvus/
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/Milvus/result_20230727_standard_milvus.json
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/Milvus/result_20230808_standard_milvus.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/PgVector/
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/PgVector/result_20230727_standard_pgvector.json
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/PgVector/result_20230808_standard_pgvector.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/Pinecone/
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/Pinecone/result_20230727_standard_pinecone.json
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/Pinecone/result_20230808_standard_pinecone.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/QdrantCloud/
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/QdrantCloud/result_20230727_standard_qdrantcloud.json
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/QdrantCloud/result_20230808_standard_qdrantcloud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.950230 vectordb-bench-0.0.7/vectordb_bench/results/WeaviateCloud/
--rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/WeaviateCloud/result_20230727_standard_weaviatecloud.json
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/WeaviateCloud/result_20230808_standard_weaviatecloud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.954230 vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/
--rw-r--r--   0 runner    (1001) docker     (127)    17398 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20230727_standard_zillizcloud.json
--rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20230808_standard_zillizcloud.json
--rw-r--r--   0 runner    (1001) docker     (127)    30990 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20240105_beta_202401_zillizcloud.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/dbPrices.json
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/getLeaderboardData.py
--rw-r--r--   0 runner    (1001) docker     (127)    55388 2024-03-13 09:55:35.000000 vectordb-bench-0.0.7/vectordb_bench/results/leaderboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 09:55:39.954230 vectordb-bench-0.0.7/vectordb_bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 09:55:39.000000 vectordb-bench-0.0.7/vectordb_bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.797742 vectordb_bench-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.773742 vectordb_bench-0.0.8/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.769741 vectordb_bench-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.773742 vectordb_bench-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.github/workflows/publish_package_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/OWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-04-23 06:25:46.797742 vectordb_bench-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20178 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.773742 vectordb_bench-0.0.8/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/install/requirements_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:25:46.797742 vectordb_bench-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.777742 vectordb_bench-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_bench_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_elasticsearch_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/tests/ut_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.777742 vectordb_bench-0.0.8/vectordb_bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/chroma/
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/chroma/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/chroma/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/elastic_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/elastic_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/milvus/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/milvus/milvus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvecto_rs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvecto_rs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvecto_rs/pgvecto_rs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvector/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvector/pgvector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pinecone/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pinecone/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/pinecone/pinecone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/qdrant_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/qdrant_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.781741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/redis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/weaviate_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/weaviate_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/backend/clients/zilliz_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/zilliz_cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/result_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/backend/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/runner/mp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/runner/serial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/backend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.769741 vectordb_bench-0.0.8/vectordb_bench/frontend/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/expanderStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/headerIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/priceTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/stPageConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.785741 vectordb_bench-0.0.8/vectordb_bench/frontend/components/get_results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/get_results/saveAsImage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/autoRefresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/caseSelector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/dbConfigSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/dbSelector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/generateTasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/hideSidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/submitTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/frontend/const/
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/const/dbCaseConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/const/dbPrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/const/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/frontend/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/pages/quries_per_dollar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/pages/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/frontend/vdb_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/log_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/ElasticCloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/ElasticCloud/result_20230727_standard_elasticcloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/ElasticCloud/result_20230808_standard_elasticcloud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/Milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)    15916 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/Milvus/result_20230727_standard_milvus.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/Milvus/result_20230808_standard_milvus.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/PgVector/
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/PgVector/result_20230727_standard_pgvector.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/PgVector/result_20230808_standard_pgvector.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/Pinecone/
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/Pinecone/result_20230727_standard_pinecone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/Pinecone/result_20230808_standard_pinecone.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.789742 vectordb_bench-0.0.8/vectordb_bench/results/QdrantCloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/QdrantCloud/result_20230727_standard_qdrantcloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/QdrantCloud/result_20230808_standard_qdrantcloud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.793742 vectordb_bench-0.0.8/vectordb_bench/results/WeaviateCloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/WeaviateCloud/result_20230727_standard_weaviatecloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/WeaviateCloud/result_20230808_standard_weaviatecloud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.793742 vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    17398 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20230727_standard_zillizcloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14969 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20230808_standard_zillizcloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41007 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20240105_standard_202401_zillizcloud.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/dbPrices.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/getLeaderboardData.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66580 2024-04-23 06:25:40.000000 vectordb_bench-0.0.8/vectordb_bench/results/leaderboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:25:46.793742 vectordb_bench-0.0.8/vectordb_bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 06:25:46.000000 vectordb_bench-0.0.8/vectordb_bench.egg-info/top_level.txt
```

### Comparing `vectordb-bench-0.0.7/.devcontainer/devcontainer.json` & `vectordb_bench-0.0.8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/.github/workflows/publish_package_on_release.yml` & `vectordb_bench-0.0.8/.github/workflows/publish_package_on_release.yml`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/.github/workflows/pull_request.yml` & `vectordb_bench-0.0.8/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/.ruff.toml` & `vectordb_bench-0.0.8/.ruff.toml`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/Dockerfile` & `vectordb_bench-0.0.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/LICENSE` & `vectordb_bench-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/PKG-INFO` & `vectordb_bench-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb-bench
-Version: 0.0.7
+Version: 0.0.8
 Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 Author-email: XuanYang-cn <xuan.yang@zilliz.com>
 Project-URL: repository, https://github.com/zilliztech/VectorDBBench
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -45,15 +45,15 @@
 Requires-Dist: pinecone-client; extra == "pinecone"
 Provides-Extra: weaviate
 Requires-Dist: weaviate-client; extra == "weaviate"
 Provides-Extra: elastic
 Requires-Dist: elasticsearch; extra == "elastic"
 Provides-Extra: pgvector
 Requires-Dist: pgvector; extra == "pgvector"
-Requires-Dist: sqlalchemy; extra == "pgvector"
+Requires-Dist: psycopg2; extra == "pgvector"
 Provides-Extra: pgvecto-rs
 Requires-Dist: psycopg2; extra == "pgvecto-rs"
 Provides-Extra: redis
 Requires-Dist: redis; extra == "redis"
 Provides-Extra: chromadb
 Requires-Dist: chromadb; extra == "chromadb"
```

### Comparing `vectordb-bench-0.0.7/README.md` & `vectordb_bench-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/install.py` & `vectordb_bench-0.0.8/install.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/pyproject.toml` & `vectordb_bench-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "psycopg2",
 ]
 
 qdrant = [ "qdrant-client" ]
 pinecone = [ "pinecone-client" ]
 weaviate = [ "weaviate-client" ]
 elastic = [ "elasticsearch" ]
-pgvector = [ "pgvector", "sqlalchemy" ]
+pgvector = [ "pgvector", "psycopg2" ]
 pgvecto_rs = [ "psycopg2" ]
 redis = [ "redis" ]
 chromadb = [ "chromadb" ]
 
 [project.urls]
 "repository" = "https://github.com/zilliztech/VectorDBBench"
```

### Comparing `vectordb-bench-0.0.7/tests/test_bench_runner.py` & `vectordb_bench-0.0.8/tests/test_bench_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_chroma.py` & `vectordb_bench-0.0.8/tests/test_chroma.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_data_source.py` & `vectordb_bench-0.0.8/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_dataset.py` & `vectordb_bench-0.0.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_elasticsearch_cloud.py` & `vectordb_bench-0.0.8/tests/test_elasticsearch_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_models.py` & `vectordb_bench-0.0.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_redis.py` & `vectordb_bench-0.0.8/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/test_utils.py` & `vectordb_bench-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/tests/ut_cases.py` & `vectordb_bench-0.0.8/tests/ut_cases.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/__init__.py` & `vectordb_bench-0.0.8/vectordb_bench/__init__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/__main__.py` & `vectordb_bench-0.0.8/vectordb_bench/__main__.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/assembler.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/assembler.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/cases.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/cases.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/__init__.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             return Pinecone
 
         if self == DB.ElasticCloud:
             from .elastic_cloud.elastic_cloud import ElasticCloud
             return ElasticCloud
 
         if self == DB.QdrantCloud:
-            from .qdrant_cloud.qdrant_cloud import QdrantClient
-            return QdrantClient
+            from .qdrant_cloud.qdrant_cloud import QdrantCloud
+            return QdrantCloud
 
         if self == DB.WeaviateCloud:
             from .weaviate_cloud.weaviate_cloud import WeaviateCloud
             return WeaviateCloud
 
         if self == DB.PgVector:
             from .pgvector.pgvector import PgVector
@@ -138,16 +138,16 @@
             return QdrantIndexConfig
 
         if self == DB.WeaviateCloud:
             from .weaviate_cloud.config import WeaviateIndexConfig
             return WeaviateIndexConfig
 
         if self == DB.PgVector:
-            from .pgvector.config import PgVectorIndexConfig
-            return PgVectorIndexConfig
+            from .pgvector.config import _pgvector_case_config
+            return _pgvector_case_config.get(index_type)
 
         if self == DB.PgVectoRS:
             from .pgvecto_rs.config import _pgvecto_rs_case_config
             return _pgvecto_rs_case_config.get(index_type)
 
         # DB.Pinecone, DB.Chroma, DB.Redis
         return EmptyDBCaseConfig
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/api.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/api.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/chroma/chroma.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/elastic_cloud/config.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/elastic_cloud/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/elastic_cloud/elastic_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/milvus/config.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/milvus/config.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/milvus/milvus.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/milvus/milvus.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvecto_rs/config.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvecto_rs/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,112 +4,124 @@
 
 POSTGRE_URL_PLACEHOLDER = "postgresql://%s:%s@%s/%s"
 
 
 class PgVectoRSConfig(DBConfig):
     user_name: SecretStr = "postgres"
     password: SecretStr
-    url: SecretStr
+    host: str = "localhost"
+    port: int = 5432
     db_name: str
 
     def to_dict(self) -> dict:
         user_str = self.user_name.get_secret_value()
         pwd_str = self.password.get_secret_value()
-        url_str = self.url.get_secret_value()
-        host, port = url_str.split(":")
         return {
-            "host": host,
-            "port": port,
+            "host": self.host,
+            "port": self.port,
             "dbname": self.db_name,
             "user": user_str,
-            "password": pwd_str,
+            "password": pwd_str
         }
 
-
 class PgVectoRSIndexConfig(BaseModel, DBCaseConfig):
     metric_type: MetricType | None = None
-    quantizationType: Literal["trivial", "scalar", "product"]
-    quantizationRatio: None | Literal["x4", "x8", "x16", "x32", "x64"]
-
-    def parse_quantization(self) -> str:
-        if self.quantizationType == "trivial":
-            return "quantization = { trivial = { } }"
-        elif self.quantizationType == "scalar":
-            return "quantization = { scalar = { } }"
-        else:
-            return f'quantization = {{ product = {{ ratio = "{self.quantizationRatio}" }} }}'
 
     def parse_metric(self) -> str:
         if self.metric_type == MetricType.L2:
-            return "l2_ops"
+            return "vector_l2_ops"
         elif self.metric_type == MetricType.IP:
-            return "dot_ops"
-        return "cosine_ops"
+            return "vector_dot_ops"
+        return "vector_cos_ops"
 
     def parse_metric_fun_op(self) -> str:
         if self.metric_type == MetricType.L2:
             return "<->"
         elif self.metric_type == MetricType.IP:
             return "<#>"
         return "<=>"
 
+class PgVectoRSQuantConfig(PgVectoRSIndexConfig):
+    quantizationType: Literal["trivial", "scalar", "product"]
+    quantizationRatio: None | Literal["x4", "x8", "x16", "x32", "x64"]
 
-class HNSWConfig(PgVectoRSIndexConfig):
+    def parse_quantization(self) -> str:
+        if self.quantizationType == "trivial":
+            return "quantization = { trivial = { } }"
+        elif self.quantizationType == "scalar":
+            return "quantization = { scalar = { } }"
+        else:
+            return f'quantization = {{ product = {{ ratio = "{self.quantizationRatio}" }} }}'
+
+
+class HNSWConfig(PgVectoRSQuantConfig):
     M: int
     efConstruction: int
     index: IndexType = IndexType.HNSW
 
     def index_param(self) -> dict:
         options = f"""
-capacity = 1048576
-[algorithm.hnsw]
+[indexing.hnsw]
 m = {self.M}
 ef_construction = {self.efConstruction}
 {self.parse_quantization()}
 """
         return {"options": options, "metric": self.parse_metric()}
 
     def search_param(self) -> dict:
         return {"metrics_op": self.parse_metric_fun_op()}
 
 
-class IVFFlatConfig(PgVectoRSIndexConfig):
+class IVFFlatConfig(PgVectoRSQuantConfig):
     nlist: int
     nprobe: int | None = None
     index: IndexType = IndexType.IVFFlat
 
     def index_param(self) -> dict:
         options = f"""
-capacity = 1048576
-[algorithm.ivf]
+[indexing.ivf]
 nlist = {self.nlist}
-nprob = {self.nprobe if self.nprobe else 10}
+nsample = {self.nprobe if self.nprobe else 10}
 {self.parse_quantization()}
 """
         return {"options": options, "metric": self.parse_metric()}
 
     def search_param(self) -> dict:
         return {"metrics_op": self.parse_metric_fun_op()}
 
+class IVFFlatSQ8Config(PgVectoRSIndexConfig):
+    nlist: int
+    nprobe: int | None = None
+    index: IndexType = IndexType.IVFSQ8
+
+    def index_param(self) -> dict:
+        options = f"""
+[indexing.ivf]
+nlist = {self.nlist}
+nsample = {self.nprobe if self.nprobe else 10}
+quantization = {{ scalar = {{ }} }}
+"""
+        return {"options": options, "metric": self.parse_metric()}
+
+    def search_param(self) -> dict:
+        return {"metrics_op": self.parse_metric_fun_op()}
 
-class FLATConfig(PgVectoRSIndexConfig):
+class FLATConfig(PgVectoRSQuantConfig):
     index: IndexType = IndexType.Flat
 
     def index_param(self) -> dict:
         options = f"""
-capacity = 1048576
-[algorithm.flat]
+[indexing.flat]
 {self.parse_quantization()}
 """
         return {"options": options, "metric": self.parse_metric()}
 
     def search_param(self) -> dict:
         return {"metrics_op": self.parse_metric_fun_op()}
 
 
 _pgvecto_rs_case_config = {
-    IndexType.AUTOINDEX: HNSWConfig,
     IndexType.HNSW: HNSWConfig,
-    IndexType.DISKANN: HNSWConfig,
     IndexType.IVFFlat: IVFFlatConfig,
+    IndexType.IVFSQ8: IVFFlatSQ8Config,
     IndexType.Flat: FLATConfig,
 }
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvecto_rs/pgvecto_rs.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/pgvecto_rs/pgvecto_rs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Wrapper around the Pgvector vector database over VectorDB"""
+"""Wrapper around the Pgvecto.rs vector database over VectorDB"""
 
 import io
 import logging
 from contextlib import contextmanager
 from typing import Any
 import pandas as pd
-
 import psycopg2
+import psycopg2.extras
 
 from ..api import VectorDB, DBCaseConfig
 
 log = logging.getLogger(__name__)
 
-
 class PgVectoRS(VectorDB):
     """Use SQLAlchemy instructions"""
 
     def __init__(
         self,
         dim: int,
         db_config: dict,
@@ -62,14 +61,16 @@
             >>> with self.init():
             >>>     self.insert_embeddings()
             >>>     self.search_embedding()
         """
         self.conn = psycopg2.connect(**self.db_config)
         self.conn.autocommit = False
         self.cursor = self.conn.cursor()
+        self.cursor.execute('SET search_path = "$user", public, vectors')
+        self.conn.commit()
 
         try:
             yield
         finally:
             self.cursor.close()
             self.conn.close()
             self.cursor = None
@@ -109,63 +110,62 @@
             self.cursor.execute(
                 f'CREATE INDEX IF NOT EXISTS {self._index_name} ON public."{self.table_name}" \
                     USING vectors (embedding {index_param["metric"]}) WITH (options = $${index_param["options"]}$$);'
             )
             self.conn.commit()
         except Exception as e:
             log.warning(
-                f"Failed to create pgvector table: {self.table_name} error: {e}"
+                f"Failed to create pgvecto.rs table: {self.table_name} error: {e}"
             )
             raise e from None
 
     def _create_table(self, dim: int):
         assert self.conn is not None, "Connection is not initialized"
         assert self.cursor is not None, "Cursor is not initialized"
 
         try:
             # create table
             self.cursor.execute(
                 f'CREATE TABLE IF NOT EXISTS public."{self.table_name}" \
                     (id Integer PRIMARY KEY, embedding vector({dim}));'
             )
-            self.cursor.execute(
-                f'ALTER TABLE public."{self.table_name}" ALTER COLUMN embedding SET STORAGE PLAIN;'
-            )
             self.conn.commit()
         except Exception as e:
             log.warning(
-                f"Failed to create pgvector table: {self.table_name} error: {e}"
+                f"Failed to create pgvecto.rs table: {self.table_name} error: {e}"
             )
             raise e from None
 
     def insert_embeddings(
         self,
         embeddings: list[list[float]],
         metadata: list[int],
         **kwargs: Any,
     ) -> (int, Exception):
         assert self.conn is not None, "Connection is not initialized"
         assert self.cursor is not None, "Cursor is not initialized"
 
+        assert self.conn is not None, "Connection is not initialized"
+        assert self.cursor is not None, "Cursor is not initialized"
+
         try:
-            items = {"id": metadata, "embedding": embeddings}
+            items = {
+                "id": metadata,
+                "embedding": embeddings
+            }
             df = pd.DataFrame(items)
             csv_buffer = io.StringIO()
             df.to_csv(csv_buffer, index=False, header=False)
             csv_buffer.seek(0)
-            self.cursor.copy_expert(
-                f'COPY public."{self.table_name}" FROM STDIN WITH (FORMAT CSV)',
-                csv_buffer,
-            )
+            self.cursor.copy_expert(f"COPY public.\"{self.table_name}\" FROM STDIN WITH (FORMAT CSV)", csv_buffer)
             self.conn.commit()
             return len(metadata), None
         except Exception as e:
-            log.warning(
-                f"Failed to insert data into pgvector table ({self.table_name}), error: {e}"
-            )
+            log.warning(f"Failed to insert data into pgvecto.rs table ({self.table_name}), error: {e}")
+            return 0, e
 
     def search_embedding(
         self,
         query: list[float],
         k: int = 100,
         filters: dict | None = None,
         timeout: int | None = None,
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/pgvector/config.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/weaviate_cloud/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,44 @@
 from pydantic import BaseModel, SecretStr
+
 from ..api import DBConfig, DBCaseConfig, MetricType
 
-POSTGRE_URL_PLACEHOLDER = "postgresql://%s:%s@%s/%s"
 
-class PgVectorConfig(DBConfig):
-    user_name: SecretStr = "postgres"
-    password: SecretStr
-    host: str = "localhost"
-    port: int = 5432
-    db_name: str
+class WeaviateConfig(DBConfig):
+    url: SecretStr
+    api_key: SecretStr
 
     def to_dict(self) -> dict:
-        user_str = self.user_name.get_secret_value()
-        pwd_str = self.password.get_secret_value()
         return {
-            "host" : self.host,
-            "port" : self.port,
-            "dbname" : self.db_name,
-            "user" : user_str,
-            "password" : pwd_str
+            "url": self.url.get_secret_value(),
+            "auth_client_secret": self.api_key.get_secret_value(),
         }
 
-class PgVectorIndexConfig(BaseModel, DBCaseConfig):
+
+class WeaviateIndexConfig(BaseModel, DBCaseConfig):
     metric_type: MetricType | None = None
-    lists: int | None = 1000
-    probes: int | None = 10
+    ef: int | None = -1
+    efConstruction: int | None = None
+    maxConnections: int | None = None
 
-    def parse_metric(self) -> str: 
-        if self.metric_type == MetricType.L2:
-            return "vector_l2_ops"
-        elif self.metric_type == MetricType.IP:
-            return "vector_ip_ops"
-        return "vector_cosine_ops"
-    
-    def parse_metric_fun_op(self) -> str:
-        if self.metric_type == MetricType.L2:
-            return "<->"
-        elif self.metric_type == MetricType.IP:
-            return "<#>"
-        return "<=>"
-    
-    def parse_metric_fun_str(self) -> str: 
+    def parse_metric(self) -> str:
         if self.metric_type == MetricType.L2:
-            return "l2_distance"
+            return "l2-squared"
         elif self.metric_type == MetricType.IP:
-            return "max_inner_product"
-        return "cosine_distance"
+            return "dot"
+        return "cosine"
 
     def index_param(self) -> dict:
-        return {
-            "lists" : self.lists,
-            "metric" : self.parse_metric()
-        }
-    
+        if self.maxConnections is not None and self.efConstruction is not None:
+            params = {
+                "distance": self.parse_metric(),
+                "maxConnections": self.maxConnections,
+                "efConstruction": self.efConstruction,
+            }
+        else:
+            params = {"distance": self.parse_metric()}
+        return params
+
     def search_param(self) -> dict:
         return {
-            "probes" : self.probes,
-            "metric_fun" : self.parse_metric_fun_str(),
-            "metric_fun_op" : self.parse_metric_fun_op(),
-        }
+            "ef": self.ef,
+        }
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/pinecone/pinecone.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/qdrant_cloud/config.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/zilliz_cloud/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from pydantic import BaseModel, SecretStr
+from pydantic import SecretStr
 
-from ..api import DBConfig, DBCaseConfig, MetricType
+from ..api import DBCaseConfig, DBConfig
+from ..milvus.config import MilvusIndexConfig, IndexType
 
 
-class QdrantConfig(DBConfig):
-    url: SecretStr
-    api_key: SecretStr
+class ZillizCloudConfig(DBConfig):
+    uri: SecretStr
+    user: str
+    password: SecretStr
 
     def to_dict(self) -> dict:
         return {
-            "url": self.url.get_secret_value(),
-            "api_key": self.api_key.get_secret_value(),
-            "prefer_grpc": True,
+            "uri": self.uri.get_secret_value(),
+            "user": self.user,
+            "password": self.password.get_secret_value(),
         }
 
-class QdrantIndexConfig(BaseModel, DBCaseConfig):
-    metric_type: MetricType | None = None
 
-    def parse_metric(self) -> str:
-        if self.metric_type == MetricType.L2:
-            return "Euclid"
-
-        if self.metric_type == MetricType.IP:
-            return "Dot"
-
-        return "Cosine"
+class AutoIndexConfig(MilvusIndexConfig, DBCaseConfig):
+    index: IndexType = IndexType.AUTOINDEX
+    level: int = 1
 
     def index_param(self) -> dict:
-        params = {"distance": self.parse_metric()}
-        return params
+        return {
+            "metric_type": self.parse_metric(),
+            "index_type": self.index.value,
+            "params": {},
+        }
 
     def search_param(self) -> dict:
-        return {}
+        return {
+            "metric_type": self.parse_metric(),
+            "params": {
+                "level": self.level,
+            }
+        }
+
+
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/qdrant_cloud/qdrant_cloud.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         self._primary_field = "pk"
         self._vector_field = "vector"
 
         tmp_client = QdrantClient(**self.db_config)
         if drop_old:
             log.info(f"QdrantCloud client drop_old collection: {self.collection_name}")
             tmp_client.delete_collection(self.collection_name)
-
-        self._create_collection(dim, tmp_client)
+            self._create_collection(dim, tmp_client)
         tmp_client = None
 
     @contextmanager
     def init(self) -> None:
         """
         Examples:
             >>> with self.init():
@@ -106,21 +105,26 @@
         self,
         embeddings: list[list[float]],
         metadata: list[int],
         **kwargs,
     ) -> (int, Exception):
         """Insert embeddings into Milvus. should call self.init() first"""
         assert self.qdrant_client is not None
+        QDRANT_BATCH_SIZE = 500
         try:
             # TODO: counts
-            _ = self.qdrant_client.upsert(
-                collection_name=self.collection_name,
-                wait=True,
-                points=Batch(ids=metadata, payloads=[{self._primary_field: v} for v in metadata], vectors=embeddings)
-            )
+            for offset in range(0, len(embeddings), QDRANT_BATCH_SIZE):
+                vectors = embeddings[offset: offset + QDRANT_BATCH_SIZE]
+                ids = metadata[offset: offset + QDRANT_BATCH_SIZE]
+                payloads=[{self._primary_field: v} for v in ids]
+                _ = self.qdrant_client.upsert(
+                    collection_name=self.collection_name,
+                    wait=True,
+                    points=Batch(ids=ids, payloads=payloads, vectors=vectors),
+                )
         except Exception as e:
             log.info(f"Failed to insert data, {e}")
             return 0, e
         else:
             return len(metadata), None
 
     def search_embedding(
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/redis/redis.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/redis/redis.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/weaviate_cloud/weaviate_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/clients/zilliz_cloud/zilliz_cloud.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/data_source.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/data_source.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/dataset.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/dataset.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/result_collector.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/result_collector.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/runner/mp_runner.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/runner/mp_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/runner/serial_runner.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/runner/serial_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/task_runner.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/task_runner.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/backend/utils.py` & `vectordb_bench-0.0.8/vectordb_bench/backend/utils.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/charts.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/charts.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/data.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/data.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/expanderStyle.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/expanderStyle.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/filters.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/filters.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/nav.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/nav.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/check_results/priceTable.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/check_results/priceTable.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/get_results/saveAsImage.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/get_results/saveAsImage.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/caseSelector.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/caseSelector.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/dbConfigSetting.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/dbConfigSetting.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/dbSelector.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/dbSelector.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/generateTasks.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/generateTasks.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/components/run_test/submitTask.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/components/run_test/submitTask.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/const/dbCaseConfigs.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/const/dbCaseConfigs.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,24 +393,33 @@
 
 CaseConfigParamInput_QuantizationType_PgVectoRS = CaseConfigInput(
     label=CaseConfigParamType.quantizationType,
     inputType=InputType.Option,
     inputConfig={
         "options": ["trivial", "scalar", "product"],
     },
+    isDisplayed=lambda config: config.get(CaseConfigParamType.IndexType, None)
+    in [
+        IndexType.HNSW.value,
+        IndexType.IVFFlat.value,
+    ],
 )
 
 CaseConfigParamInput_QuantizationRatio_PgVectoRS = CaseConfigInput(
     label=CaseConfigParamType.quantizationRatio,
     inputType=InputType.Option,
     inputConfig={
         "options": ["x4", "x8", "x16", "x32", "x64"],
     },
     isDisplayed=lambda config: config.get(CaseConfigParamType.quantizationType, None)
-    == "product",
+    == "product" and config.get(CaseConfigParamType.IndexType, None)
+    in [
+        IndexType.HNSW.value,
+        IndexType.IVFFlat.value,
+    ],
 )
 
 CaseConfigParamInput_ZillizLevel = CaseConfigInput(
     label=CaseConfigParamType.level,
     inputType=InputType.Number,
     inputConfig={
         "min": 1,
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/const/styles.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/const/styles.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/pages/quries_per_dollar.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/pages/quries_per_dollar.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/pages/run_test.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/pages/run_test.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/frontend/vdb_benchmark.py` & `vectordb_bench-0.0.8/vectordb_bench/frontend/vdb_benchmark.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/interface.py` & `vectordb_bench-0.0.8/vectordb_bench/interface.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/log_util.py` & `vectordb_bench-0.0.8/vectordb_bench/log_util.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/metric.py` & `vectordb_bench-0.0.8/vectordb_bench/metric.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/models.py` & `vectordb_bench-0.0.8/vectordb_bench/models.py`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/ElasticCloud/result_20230727_standard_elasticcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/ElasticCloud/result_20230727_standard_elasticcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/ElasticCloud/result_20230808_standard_elasticcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/ElasticCloud/result_20230808_standard_elasticcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/Milvus/result_20230727_standard_milvus.json` & `vectordb_bench-0.0.8/vectordb_bench/results/Milvus/result_20230727_standard_milvus.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/Milvus/result_20230808_standard_milvus.json` & `vectordb_bench-0.0.8/vectordb_bench/results/Milvus/result_20230808_standard_milvus.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/PgVector/result_20230727_standard_pgvector.json` & `vectordb_bench-0.0.8/vectordb_bench/results/PgVector/result_20230727_standard_pgvector.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993489583333334%*

 * *Differences: {"'results'": "{0: {'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}, 1: {'task_config': "*

 * *              "{'db_case_config': {'index': 'IVF_FLAT'}}}, 2: {'task_config': {'db_case_config': "*

 * *              "{'index': 'IVF_FLAT'}}}, 3: {'task_config': {'db_case_config': {'index': "*

 * *              "'IVF_FLAT'}}}, 4: {'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}, 5: "*

 * *              "{'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}, 6: {'task_config': "*

 * *              "{'db_case_conf […]*

```diff
@@ -13,14 +13,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 1,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -42,14 +43,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 2,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -71,14 +73,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -100,14 +103,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 7,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -129,14 +133,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 9,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -158,14 +163,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 4,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -187,14 +193,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 6,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -216,14 +223,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 8,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "COSINE",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/PgVector/result_20230808_standard_pgvector.json` & `vectordb_bench-0.0.8/vectordb_bench/results/PgVector/result_20230808_standard_pgvector.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993489583333333%*

 * *Differences: {"'results'": "{0: {'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}, 1: {'task_config': "*

 * *              "{'db_case_config': {'index': 'IVF_FLAT'}}}, 2: {'task_config': {'db_case_config': "*

 * *              "{'index': 'IVF_FLAT'}}}, 3: {'task_config': {'db_case_config': {'index': "*

 * *              "'IVF_FLAT'}}}, 4: {'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}, 5: "*

 * *              "{'task_config': {'db_case_config': {'index': 'IVF_FLAT'}}}}"}*

```diff
@@ -13,14 +13,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 10,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -42,14 +43,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 11,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -71,14 +73,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 12,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -100,14 +103,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 13,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -129,14 +133,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 14,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
@@ -158,14 +163,15 @@
             "task_config": {
                 "case_config": {
                     "case_id": 15,
                     "custom_case": {}
                 },
                 "db": "PgVector",
                 "db_case_config": {
+                    "index": "IVF_FLAT",
                     "lists": 10,
                     "metric_type": "L2",
                     "probes": 2
                 },
                 "db_config": {
                     "db_label": "2c8g",
                     "db_name": "**********",
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/Pinecone/result_20230727_standard_pinecone.json` & `vectordb_bench-0.0.8/vectordb_bench/results/Pinecone/result_20230727_standard_pinecone.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/Pinecone/result_20230808_standard_pinecone.json` & `vectordb_bench-0.0.8/vectordb_bench/results/Pinecone/result_20230808_standard_pinecone.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/QdrantCloud/result_20230727_standard_qdrantcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/QdrantCloud/result_20230727_standard_qdrantcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/QdrantCloud/result_20230808_standard_qdrantcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/QdrantCloud/result_20230808_standard_qdrantcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/WeaviateCloud/result_20230727_standard_weaviatecloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/WeaviateCloud/result_20230727_standard_weaviatecloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/WeaviateCloud/result_20230808_standard_weaviatecloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/WeaviateCloud/result_20230808_standard_weaviatecloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20230727_standard_zillizcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20230727_standard_zillizcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20230808_standard_zillizcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20230808_standard_zillizcloud.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/ZillizCloud/result_20240105_beta_202401_zillizcloud.json` & `vectordb_bench-0.0.8/vectordb_bench/results/ZillizCloud/result_20240105_standard_202401_zillizcloud.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8433322482638889%*

 * *Differences: {"'results'": "{0: {'task_config': {'db_config': {'db_label': '8cu-perf-(Jan-2024)'}}}, 1: "*

 * *              "{'task_config': {'db_config': {'db_label': '8cu-perf-(Jan-2024)'}}}, 2: "*

 * *              "{'task_config': {'db_config': {'db_label': '8cu-perf-(Jan-2024)'}}}, 3: "*

 * *              "{'task_config': {'db_config': {'db_label': '8cu-perf-(Jan-2024)'}}}, 4: "*

 * *              "{'task_config': {'db_config': {'db_label': '8cu-perf-(Jan-2024)'}}}, 5: "*

 * *              "{'task_config': {'db_config': {'db_label': '8cu- […]*

```diff
@@ -17,15 +17,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -44,15 +44,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -71,15 +71,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -98,15 +98,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -125,15 +125,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -152,15 +152,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -179,15 +179,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -206,15 +206,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -233,15 +233,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -260,15 +260,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -287,15 +287,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -314,15 +314,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "8cu-perf-beta-202401",
+                    "db_label": "8cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -341,15 +341,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -368,15 +368,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -395,15 +395,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -422,15 +422,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -449,15 +449,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -476,15 +476,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-cap-beta-202401",
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -503,15 +503,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -530,15 +530,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -557,15 +557,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -584,15 +584,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -611,15 +611,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -638,15 +638,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -665,15 +665,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -692,15 +692,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -719,15 +719,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -746,15 +746,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -773,15 +773,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -800,15 +800,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "2cu-cap-beta-202401",
+                    "db_label": "2cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -827,15 +827,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -854,15 +854,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -881,42 +881,42 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
             "label": ":)",
             "metrics": {
-                "load_duration": 960.7296,
+                "load_duration": 963.5924,
                 "max_load_count": 0,
-                "qps": 871.5513,
-                "recall": 0.9471,
-                "serial_latency_p99": 0.0213
+                "qps": 873.3712,
+                "recall": 0.9477,
+                "serial_latency_p99": 0.0067
             },
             "task_config": {
                 "case_config": {
                     "case_id": 5,
                     "custom_case": {}
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -935,15 +935,15 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         },
         {
@@ -962,18 +962,342 @@
                 },
                 "db": "ZillizCloud",
                 "db_case_config": {
                     "index": "AUTOINDEX",
                     "metric_type": "COSINE"
                 },
                 "db_config": {
-                    "db_label": "1cu-perf-beta-202401",
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 11,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 13,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 15,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-perf-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 4,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 6,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 8,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 11,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 13,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
+                    "password": "**********",
+                    "uri": "**********",
+                    "user": "db_admin"
+                }
+            }
+        },
+        {
+            "label": "x",
+            "metrics": {
+                "load_duration": 0.0,
+                "max_load_count": 0,
+                "qps": 0.0,
+                "recall": 0.0,
+                "serial_latency_p99": 0.0
+            },
+            "task_config": {
+                "case_config": {
+                    "case_id": 15,
+                    "custom_case": {}
+                },
+                "db": "ZillizCloud",
+                "db_case_config": {
+                    "index": "AUTOINDEX",
+                    "metric_type": "COSINE"
+                },
+                "db_config": {
+                    "db_label": "1cu-cap-(Jan-2024)",
                     "password": "**********",
                     "uri": "**********",
                     "user": "db_admin"
                 }
             }
         }
     ],
     "run_id": "0ae10e14e34c4c3c9a7116e7a9591d01",
-    "task_label": "zilliz-beta-202401"
+    "task_label": "standard_202401"
 }
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/dbPrices.json` & `vectordb_bench-0.0.8/vectordb_bench/results/dbPrices.json`

 * *Files identical despite different names*

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/getLeaderboardData.py` & `vectordb_bench-0.0.8/vectordb_bench/results/getLeaderboardData.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 }
 
 
 def main():
     allResults: list[TestResult] = benchMarkRunner.get_results()
     results: list[CaseResult] = []
     for result in allResults:
-        if result.task_label == "standard":
+        if "standard" in result.task_label:
             results += result.results
 
     if allResults is not None:
         data = [
             {
                 "db": d.task_config.db.value,
                 "db_label": d.task_config.db_config.db_label,
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench/results/leaderboard.json` & `vectordb_bench-0.0.8/vectordb_bench/results/leaderboard.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5953878406708591%*

 * *Differences: {'10': "{'db': 'ElasticCloud', 'db_label': 'upTo2.5c8g', 'db_name': 'ElasticCloud-upTo2.5c8g', "*

 * *       "'qps': 26.26, 'latency': 556.1, 'recall': 0.9999, 'qp$': 197237.6382224077}",*

 * * '108': "{'db': 'Pinecone', 'db_label': 'p2.x1', 'db_name': 'Pinecone-p2.x1', 'case': 'Search "*

 * *        "Performance Test (500K Dataset, 1536 Dim)', 'qps': 228.4, 'latency': 22.2, 'recall': "*

 * *        "0.9348, 'qp$': 5631780.821917809}",*

 * * '109': "{'db': 'Pinecone', 'db_label': 'p2.x1', 'db_name': 'Pinecone-p2.x1', 'case': 'Searc […]*

```diff
@@ -1,135 +1,69 @@
 [
     {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": 1,
-        "latency": 2523.0,
-        "qp$": 0.0,
-        "qps": 0.8836,
-        "recall": 0.8528
-    },
-    {
-        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -2,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": 1,
-        "latency": 3720.2000000000003,
-        "qp$": 0.0,
-        "qps": 0.8937,
-        "recall": 0.8525
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -2,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": 1,
-        "latency": 3622.3999999999996,
-        "qp$": 0.0,
-        "qps": 1.2145,
-        "recall": 0.7487
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -2,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
         "label": 1,
-        "latency": 730.7,
-        "qp$": 0.0,
-        "qps": 10.6271,
-        "recall": 0.8898
+        "latency": 861.8,
+        "qp$": 114368.53745044857,
+        "qps": 15.2269,
+        "recall": 0.9888
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
         "label": 1,
-        "latency": 733.1999999999999,
-        "qp$": 0.0,
-        "qps": 10.8507,
-        "recall": 0.8897
+        "latency": 774.3,
+        "qp$": 113977.96786981013,
+        "qps": 15.1749,
+        "recall": 0.989
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
         "label": 1,
-        "latency": 121.2,
-        "qp$": 0.0,
-        "qps": 75.7055,
+        "latency": 305.5,
+        "qp$": 207438.26413519715,
+        "qps": 27.6181,
         "recall": 0.9999
     },
     {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -1,
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -1,
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "PgVector",
-        "db_label": "2c8g",
-        "db_name": "PgVector-2c8g",
-        "label": -1,
+        "db": "ElasticCloud",
+        "db_label": "upTo2.5c8g",
+        "db_name": "ElasticCloud-upTo2.5c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
@@ -195,469 +129,667 @@
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 861.8,
-        "qp$": 114368.53745044857,
-        "qps": 15.2269,
-        "recall": 0.9888
+        "latency": 21.1,
+        "qp$": 0.0,
+        "qps": 100.6667,
+        "recall": 0.9909
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 774.3,
-        "qp$": 113977.96786981013,
-        "qps": 15.1749,
-        "recall": 0.989
+        "latency": 19.7,
+        "qp$": 0.0,
+        "qps": 101.1399,
+        "recall": 0.9907
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 305.5,
-        "qp$": 207438.26413519715,
-        "qps": 27.6181,
-        "recall": 0.9999
+        "latency": 18.3,
+        "qp$": 0.0,
+        "qps": 52.2606,
+        "recall": 1.0
     },
     {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
-        "label": -2,
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
+        "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
-        "label": -2,
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
+        "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "ElasticCloud",
-        "db_label": "upTo2.5c8g",
-        "db_name": "ElasticCloud-upTo2.5c8g",
-        "label": -2,
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
+        "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
         "label": 1,
-        "latency": 22.2,
-        "qp$": 5631780.821917809,
-        "qps": 228.4,
-        "recall": 0.9348
+        "latency": 49.8,
+        "qp$": 0.0,
+        "qps": 61.0661,
+        "recall": 0.9911
     },
     {
-        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
-        "label": -1,
-        "latency": 0.0,
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 44.6,
         "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
+        "qps": 58.9326,
+        "recall": 0.9911
     },
     {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
         "label": 1,
-        "latency": 26.1,
-        "qp$": 4475342.465753425,
-        "qps": 181.5,
-        "recall": 0.9345
+        "latency": 54.9,
+        "qp$": 0.0,
+        "qps": 42.5977,
+        "recall": 1.0
     },
     {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 8.200000000000001,
+        "qp$": 0.0,
+        "qps": 536.0726,
+        "recall": 0.9728
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 7.0,
+        "qp$": 0.0,
+        "qps": 467.179,
+        "recall": 0.9697
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 8.3,
+        "qp$": 0.0,
+        "qps": 431.7512,
+        "recall": 1.0
+    },
+    {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
+        "label": 1,
+        "latency": 4.8999999999999995,
+        "qp$": 0.0,
+        "qps": 274.5407,
+        "recall": 0.9807
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
+        "label": 1,
+        "latency": 10.3,
+        "qp$": 0.0,
+        "qps": 236.5672,
+        "recall": 0.981
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
+        "label": 1,
+        "latency": 4.3,
+        "qp$": 0.0,
+        "qps": 309.4833,
+        "recall": 1.0
+    },
+    {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
-        "label": 1,
-        "latency": 24.2,
-        "qp$": 5072054.794520548,
-        "qps": 205.7,
-        "recall": 0.9586
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1",
-        "db_name": "Pinecone-p2.x1",
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 13.700000000000001,
+        "qp$": 0.0,
+        "qps": 178.6585,
+        "recall": 0.9843
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 15.0,
+        "qp$": 0.0,
+        "qps": 178.3732,
+        "recall": 0.9844
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 12.5,
+        "qp$": 0.0,
+        "qps": 229.3526,
+        "recall": 1.0
+    },
+    {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 4.8999999999999995,
+        "qp$": 0.0,
+        "qps": 1258.7043,
+        "recall": 0.9799
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 5.3,
+        "qp$": 0.0,
+        "qps": 1075.8776,
+        "recall": 0.98
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
+        "label": 1,
+        "latency": 4.7,
+        "qp$": 0.0,
+        "qps": 1494.8493,
+        "recall": 1.0
+    },
+    {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 36.0,
-        "qp$": 2502240.4933196297,
-        "qps": 67.63,
-        "recall": 0.8064
+        "latency": 75.0,
+        "qp$": 0.0,
+        "qps": 37.432,
+        "recall": 0.9975
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 38.4,
-        "qp$": 2343884.892086331,
-        "qps": 63.35,
-        "recall": 0.8065
+        "latency": 73.5,
+        "qp$": 0.0,
+        "qps": 37.0696,
+        "recall": 0.9976
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": 1,
-        "latency": 27.599999999999998,
-        "qp$": 6537718.396711202,
-        "qps": 176.7,
+        "latency": 53.0,
+        "qp$": 0.0,
+        "qps": 81.1915,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1",
-        "db_name": "Pinecone-p1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-disk",
+        "db_name": "Milvus-2c8g-disk",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
         "label": 1,
-        "latency": 84.9,
-        "qp$": 567194.2446043165,
-        "qps": 15.33,
-        "recall": 0.8064
+        "latency": 13.4,
+        "qp$": 0.0,
+        "qps": 321.6048,
+        "recall": 0.989
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 86.8,
+        "qp$": 0.0,
+        "qps": 22.1467,
+        "recall": 0.9972
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 10.9,
+        "qp$": 0.0,
+        "qps": 303.2551,
+        "recall": 0.9876
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 81.69999999999999,
+        "qp$": 0.0,
+        "qps": 21.5388,
+        "recall": 0.997
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 8.3,
+        "qp$": 0.0,
+        "qps": 394.5418,
+        "recall": 1.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "Milvus",
+        "db_label": "4c16g-disk",
+        "db_name": "Milvus-4c16g-disk",
+        "label": 1,
+        "latency": 45.0,
+        "qp$": 0.0,
+        "qps": 37.878,
+        "recall": 1.0
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
+        "label": 1,
+        "latency": 6.0,
+        "qp$": 0.0,
+        "qps": 180.2757,
+        "recall": 0.9942
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": 1,
-        "latency": 86.7,
-        "qp$": 559794.4501541625,
-        "qps": 15.13,
-        "recall": 0.8065
+        "latency": 6.4,
+        "qp$": 0.0,
+        "qps": 179.0033,
+        "recall": 0.9943
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": 1,
-        "latency": 74.30000000000001,
-        "qp$": 644152.1068859198,
-        "qps": 17.41,
+        "latency": 3.6,
+        "qp$": 0.0,
+        "qps": 526.8846,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1",
-        "db_name": "Pinecone-s1.x1",
+        "db": "Milvus",
+        "db_label": "2c8g-hnsw",
+        "db_name": "Milvus-2c8g-hnsw",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 88.7,
-        "qp$": 301661.53846153844,
-        "qps": 16.34,
-        "recall": 0.879
+        "latency": 6.2,
+        "qp$": 0.0,
+        "qps": 626.5243,
+        "recall": 0.9954
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 126.8,
-        "qp$": 192923.0769230769,
-        "qps": 10.45,
-        "recall": 0.8208
+        "latency": 25.3,
+        "qp$": 0.0,
+        "qps": 78.4227,
+        "recall": 0.9982
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 87.5,
-        "qp$": 298707.69230769225,
-        "qps": 16.18,
-        "recall": 0.8793
+        "latency": 6.6,
+        "qp$": 0.0,
+        "qps": 599.4213,
+        "recall": 0.9955
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 130.89999999999998,
-        "qp$": 180923.0769230769,
-        "qps": 9.8,
-        "recall": 0.8212
+        "latency": 26.3,
+        "qp$": 0.0,
+        "qps": 78.5351,
+        "recall": 0.9982
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 55.1,
-        "qp$": 666646.1538461539,
-        "qps": 36.11,
+        "latency": 3.4,
+        "qp$": 0.0,
+        "qps": 2098.2113,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "s1.x1-2node",
-        "db_name": "Pinecone-s1.x1-2node",
-        "label": 1,
-        "latency": 92.7,
-        "qp$": 273969.23076923075,
-        "qps": 14.84,
-        "recall": 0.96
-    },
-    {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
+        "db": "Milvus",
+        "db_label": "16c64g-hnsw",
+        "db_name": "Milvus-16c64g-hnsw",
         "label": 1,
-        "latency": 26.4,
-        "qp$": 994623.287671233,
-        "qps": 322.7,
-        "recall": 0.9478
+        "latency": 10.0,
+        "qp$": 0.0,
+        "qps": 275.6292,
+        "recall": 1.0
     },
     {
-        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": 1,
-        "latency": 26.9,
-        "qp$": 818321.9178082192,
-        "qps": 265.5,
-        "recall": 0.9332
+        "latency": 730.7,
+        "qp$": 0.0,
+        "qps": 10.6271,
+        "recall": 0.8898
     },
     {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": 1,
-        "latency": 27.3,
-        "qp$": 936369.8630136987,
-        "qps": 303.8,
-        "recall": 0.9478
+        "latency": 733.1999999999999,
+        "qp$": 0.0,
+        "qps": 10.8507,
+        "recall": 0.8897
     },
     {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": 1,
-        "latency": 28.2,
-        "qp$": 555410.9589041097,
-        "qps": 180.2,
-        "recall": 0.9335
+        "latency": 121.2,
+        "qp$": 0.0,
+        "qps": 75.7055,
+        "recall": 0.9999
     },
     {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
-        "label": 1,
-        "latency": 24.6,
-        "qp$": 2252157.5342465756,
-        "qps": 730.7,
-        "recall": 0.9586
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p2.x1-8node",
-        "db_name": "Pinecone-p2.x1-8node",
-        "label": 1,
-        "latency": 31.7,
-        "qp$": 321472.602739726,
-        "qps": 104.3,
-        "recall": 0.9563
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": 1,
+        "latency": 2523.0,
+        "qp$": 0.0,
+        "qps": 0.8836,
+        "recall": 0.8528
+    },
+    {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
-        "label": -1,
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": 1,
-        "latency": 35.3,
-        "qp$": 682567.3940949935,
-        "qps": 147.7,
-        "recall": 0.9707
+        "latency": 3720.2000000000003,
+        "qp$": 0.0,
+        "qps": 0.8937,
+        "recall": 0.8525
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
-        "label": -1,
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
         "label": 1,
-        "latency": 25.9,
-        "qp$": 3616174.5827984596,
-        "qps": 782.5,
-        "recall": 1.0
+        "latency": 3622.3999999999996,
+        "qp$": 0.0,
+        "qps": 1.2145,
+        "recall": 0.7487
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Pinecone",
-        "db_label": "p1.x1-8node",
-        "db_name": "Pinecone-p1.x1-8node",
-        "label": -1,
+        "db": "PgVector",
+        "db_label": "2c8g",
+        "db_name": "PgVector-2c8g",
+        "label": -2,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
@@ -1052,540 +1184,408 @@
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
-        "label": 1,
-        "latency": 9.0,
-        "qp$": 7472024.150943397,
-        "qps": 330.0144,
-        "recall": 0.9507
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
-        "label": 1,
-        "latency": 10.1,
-        "qp$": 6150758.490566038,
-        "qps": 271.6585,
-        "recall": 0.9678
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
         "label": 1,
-        "latency": 12.9,
-        "qp$": 4902398.490566038,
-        "qps": 216.5226,
-        "recall": 1.0
+        "latency": 22.2,
+        "qp$": 5631780.821917809,
+        "qps": 228.4,
+        "recall": 0.9348
     },
     {
-        "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
+        "label": 1,
+        "latency": 26.1,
+        "qp$": 4475342.465753425,
+        "qps": 181.5,
+        "recall": 0.9345
     },
     {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 23.0,
-        "qp$": 1403267.5471698113,
-        "qps": 123.9553,
-        "recall": 0.971
-    },
-    {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 44.5,
-        "qp$": 669598.8679245282,
-        "qps": 59.1479,
-        "recall": 0.9906
-    },
-    {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 55.300000000000004,
-        "qp$": 464139.62264150946,
-        "qps": 40.999,
-        "recall": 1.0
-    },
-    {
-        "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 9.4,
-        "qp$": 6565376.603773585,
-        "qps": 579.9416,
-        "recall": 0.9213
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 11.299999999999999,
-        "qp$": 4814183.773584905,
-        "qps": 425.2529,
-        "recall": 0.9686
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 13.799999999999999,
-        "qp$": 4494949.811320755,
-        "qps": 397.0539,
-        "recall": 1.0
-    },
-    {
-        "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
-        "label": 1,
-        "latency": 7.0,
-        "qp$": 11689132.075471697,
-        "qps": 516.27,
-        "recall": 0.9463
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
-        "label": 1,
-        "latency": 10.0,
-        "qp$": 8034149.433962264,
-        "qps": 354.8416,
-        "recall": 0.9802
-    },
-    {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
         "label": 1,
-        "latency": 8.7,
-        "qp$": 9679763.773584906,
-        "qps": 427.5229,
-        "recall": 1.0
+        "latency": 24.2,
+        "qp$": 5072054.794520548,
+        "qps": 205.7,
+        "recall": 0.9586
     },
     {
-        "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "Pinecone",
+        "db_label": "p2.x1",
+        "db_name": "Pinecone-p2.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
+        "label": 1,
+        "latency": 36.0,
+        "qp$": 2502240.4933196297,
+        "qps": 67.63,
+        "recall": 0.8064
     },
     {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
         "label": 1,
-        "latency": 5.3,
-        "qp$": 8164214.150943396,
-        "qps": 2884.689,
-        "recall": 0.8801
+        "latency": 38.4,
+        "qp$": 2343884.892086331,
+        "qps": 63.35,
+        "recall": 0.8065
     },
     {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
-        "label": 1,
-        "latency": 6.6,
-        "qp$": 4781829.905660377,
-        "qps": 1689.5799,
-        "recall": 0.9493
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
-        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
         "label": 1,
-        "latency": 10.0,
-        "qp$": 4295318.4905660385,
-        "qps": 1517.6792,
+        "latency": 27.599999999999998,
+        "qp$": 6537718.396711202,
+        "qps": 176.7,
         "recall": 1.0
     },
     {
-        "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
-        "label": 1,
-        "latency": 5.6,
-        "qp$": 2327920.1886792453,
-        "qps": 822.5318,
-        "recall": 0.9294
-    },
-    {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
-        "label": 1,
-        "latency": 10.3,
-        "qp$": 1072399.8113207547,
-        "qps": 378.9146,
-        "recall": 0.9758
-    },
-    {
-        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
-        "label": 1,
-        "latency": 16.2,
-        "qp$": 618920.9433962263,
-        "qps": 218.6854,
-        "recall": 1.0
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "Pinecone",
+        "db_label": "p1.x1",
+        "db_name": "Pinecone-p1.x1",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": 1,
-        "latency": 7.2,
-        "qp$": 6735849.0566037735,
-        "qps": 297.5,
-        "recall": 0.974
+        "latency": 84.9,
+        "qp$": 567194.2446043165,
+        "qps": 15.33,
+        "recall": 0.8064
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": 1,
-        "latency": 10.6,
-        "qp$": 5169056.603773585,
-        "qps": 228.3,
-        "recall": 0.994
+        "latency": 86.7,
+        "qp$": 559794.4501541625,
+        "qps": 15.13,
+        "recall": 0.8065
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": 1,
-        "latency": 4.6,
-        "qp$": 13222641.509433962,
-        "qps": 584.0,
+        "latency": 74.30000000000001,
+        "qp$": 644152.1068859198,
+        "qps": 17.41,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-perf",
-        "db_name": "ZillizCloud-1cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1",
+        "db_name": "Pinecone-s1.x1",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 7.0,
-        "qp$": 5295283.018867925,
-        "qps": 1871.0,
-        "recall": 0.9602
+        "latency": 88.7,
+        "qp$": 301661.53846153844,
+        "qps": 16.34,
+        "recall": 0.879
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 6.7,
-        "qp$": 1575566.0377358492,
-        "qps": 556.7,
-        "recall": 0.9723
+        "latency": 126.8,
+        "qp$": 192923.0769230769,
+        "qps": 10.45,
+        "recall": 0.8208
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 6.8,
-        "qp$": 4480188.679245283,
-        "qps": 1583.0,
-        "recall": 0.9836
+        "latency": 87.5,
+        "qp$": 298707.69230769225,
+        "qps": 16.18,
+        "recall": 0.8793
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 10.9,
-        "qp$": 832924.5283018869,
-        "qps": 294.3,
-        "recall": 0.9939
+        "latency": 130.89999999999998,
+        "qp$": 180923.0769230769,
+        "qps": 9.8,
+        "recall": 0.8212
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 8.9,
-        "qp$": 6636792.452830189,
-        "qps": 2345.0,
+        "latency": 55.1,
+        "qp$": 666646.1538461539,
+        "qps": 36.11,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "8cu-perf",
-        "db_name": "ZillizCloud-8cu-perf",
+        "db": "Pinecone",
+        "db_label": "s1.x1-2node",
+        "db_name": "Pinecone-s1.x1-2node",
         "label": 1,
-        "latency": 12.3,
-        "qp$": 836603.7735849057,
-        "qps": 295.6,
-        "recall": 1.0
+        "latency": 92.7,
+        "qp$": 273969.23076923075,
+        "qps": 14.84,
+        "recall": 0.96
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
         "label": 1,
-        "latency": 33.5,
-        "qp$": 3237735.8490566034,
-        "qps": 143.0,
-        "recall": 0.9818
+        "latency": 26.4,
+        "qp$": 994623.287671233,
+        "qps": 322.7,
+        "recall": 0.9478
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
+        "label": 1,
+        "latency": 26.9,
+        "qp$": 818321.9178082192,
+        "qps": 265.5,
+        "recall": 0.9332
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
         "label": 1,
-        "latency": 20.7,
-        "qp$": 2400000.0,
-        "qps": 106.0,
-        "recall": 0.9887
+        "latency": 27.3,
+        "qp$": 936369.8630136987,
+        "qps": 303.8,
+        "recall": 0.9478
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
+        "label": 1,
+        "latency": 28.2,
+        "qp$": 555410.9589041097,
+        "qps": 180.2,
+        "recall": 0.9335
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
         "label": 1,
-        "latency": 11.6,
-        "qp$": 4279245.2830188675,
-        "qps": 189.0,
-        "recall": 1.0
+        "latency": 24.6,
+        "qp$": 2252157.5342465756,
+        "qps": 730.7,
+        "recall": 0.9586
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "1cu-cap",
-        "db_name": "ZillizCloud-1cu-cap",
+        "db": "Pinecone",
+        "db_label": "p2.x1-8node",
+        "db_name": "Pinecone-p2.x1-8node",
+        "label": 1,
+        "latency": 31.7,
+        "qp$": 321472.602739726,
+        "qps": 104.3,
+        "recall": 0.9563
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 12.4,
-        "qp$": 4301570.9433962265,
-        "qps": 379.9721,
-        "recall": 0.982
-    },
-    {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 50.8,
-        "qp$": 812150.9433962264,
-        "qps": 71.74,
-        "recall": 0.9883
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
         "label": 1,
-        "latency": 14.9,
-        "qp$": 3249056.603773585,
-        "qps": 287.0,
-        "recall": 0.9865
+        "latency": 35.3,
+        "qp$": 682567.3940949935,
+        "qps": 147.7,
+        "recall": 0.9707
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 64.69999999999999,
-        "qp$": 392438.4905660377,
-        "qps": 34.6654,
-        "recall": 0.9961
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
         "label": 1,
-        "latency": 10.3,
-        "qp$": 4664150.9433962265,
-        "qps": 412.0,
+        "latency": 25.9,
+        "qp$": 3616174.5827984596,
+        "qps": 782.5,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "ZillizCloud",
-        "db_label": "2cu-cap",
-        "db_name": "ZillizCloud-2cu-cap",
-        "label": 1,
-        "latency": 46.800000000000004,
-        "qp$": 477384.9056603773,
-        "qps": 42.169,
-        "recall": 1.0
+        "db": "Pinecone",
+        "db_label": "p1.x1-8node",
+        "db_name": "Pinecone-p1.x1-8node",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
         "db": "QdrantCloud",
         "db_label": "2c8g-1node",
         "db_name": "QdrantCloud-2c8g-1node",
         "label": -1,
@@ -1976,146 +1976,14 @@
         "label": 1,
         "latency": 19.599999999999998,
         "qp$": 420905.1332398317,
         "qps": 166.7252,
         "recall": 0.9988
     },
     {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": 1,
-        "latency": 123.0,
-        "qp$": 16703.358415841583,
-        "qps": 46.8622,
-        "recall": 0.9957
-    },
-    {
-        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": 1,
-        "latency": 1063.5,
-        "qp$": 655.4138613861386,
-        "qps": 1.8388,
-        "recall": 0.9957
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": 1,
-        "latency": 109.2,
-        "qp$": 16063.342574257427,
-        "qps": 45.0666,
-        "recall": 1.0
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "WeaviateCloud",
-        "db_label": "standard",
-        "db_name": "WeaviateCloud-standard",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": 1,
-        "latency": 228.7,
-        "qp$": 4803.8687116564415,
-        "qps": 43.5017,
-        "recall": 0.9957
-    },
-    {
-        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": 1,
-        "latency": 1114.4,
-        "qp$": 173.02085889570552,
-        "qps": 1.5668,
-        "recall": 0.9957
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
-        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": 1,
-        "latency": 159.0,
-        "qp$": 4587.714110429448,
-        "qps": 41.5443,
-        "recall": 1.0
-    },
-    {
-        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "WeaviateCloud",
-        "db_label": "bus_crit",
-        "db_name": "WeaviateCloud-bus_crit",
-        "label": -1,
-        "latency": 0.0,
-        "qp$": 0.0,
-        "qps": 0.0,
-        "recall": 0.0
-    },
-    {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
         "db": "WeaviateCloud",
         "db_label": "bus_crit",
         "db_name": "WeaviateCloud-bus_crit",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
@@ -2307,534 +2175,1194 @@
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": 1,
-        "latency": 75.0,
-        "qp$": 0.0,
-        "qps": 37.432,
-        "recall": 0.9975
+        "latency": 123.0,
+        "qp$": 16703.358415841583,
+        "qps": 46.8622,
+        "recall": 0.9957
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": 1,
-        "latency": 73.5,
-        "qp$": 0.0,
-        "qps": 37.0696,
-        "recall": 0.9976
+        "latency": 1063.5,
+        "qp$": 655.4138613861386,
+        "qps": 1.8388,
+        "recall": 0.9957
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": 1,
-        "latency": 53.0,
-        "qp$": 0.0,
-        "qps": 81.1915,
+        "latency": 109.2,
+        "qp$": 16063.342574257427,
+        "qps": 45.0666,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "standard",
+        "db_name": "WeaviateCloud-standard",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
         "label": 1,
-        "latency": 13.4,
-        "qp$": 0.0,
-        "qps": 321.6048,
-        "recall": 0.989
+        "latency": 228.7,
+        "qp$": 4803.8687116564415,
+        "qps": 43.5017,
+        "recall": 0.9957
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
-        "label": 1,
-        "latency": 86.8,
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
+        "label": -1,
+        "latency": 0.0,
         "qp$": 0.0,
-        "qps": 22.1467,
-        "recall": 0.9972
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
         "label": 1,
-        "latency": 10.9,
-        "qp$": 0.0,
-        "qps": 303.2551,
-        "recall": 0.9876
+        "latency": 1114.4,
+        "qp$": 173.02085889570552,
+        "qps": 1.5668,
+        "recall": 0.9957
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
         "label": 1,
-        "latency": 81.69999999999999,
+        "latency": 159.0,
+        "qp$": 4587.714110429448,
+        "qps": 41.5443,
+        "recall": 1.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "WeaviateCloud",
+        "db_label": "bus_crit",
+        "db_name": "WeaviateCloud-bus_crit",
+        "label": -1,
+        "latency": 0.0,
         "qp$": 0.0,
-        "qps": 21.5388,
-        "recall": 0.997
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
+        "label": 1,
+        "latency": 7.2,
+        "qp$": 6735849.0566037735,
+        "qps": 297.5,
+        "recall": 0.974
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
+        "label": 1,
+        "latency": 10.6,
+        "qp$": 5169056.603773585,
+        "qps": 228.3,
+        "recall": 0.994
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": 1,
-        "latency": 8.3,
+        "latency": 4.6,
+        "qp$": 13222641.509433962,
+        "qps": 584.0,
+        "recall": 1.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
+        "label": -1,
+        "latency": 0.0,
         "qp$": 0.0,
-        "qps": 394.5418,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 7.0,
+        "qp$": 5295283.018867925,
+        "qps": 1871.0,
+        "recall": 0.9602
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 6.7,
+        "qp$": 1575566.0377358492,
+        "qps": 556.7,
+        "recall": 0.9723
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 6.8,
+        "qp$": 4480188.679245283,
+        "qps": 1583.0,
+        "recall": 0.9836
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 10.9,
+        "qp$": 832924.5283018869,
+        "qps": 294.3,
+        "recall": 0.9939
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 8.9,
+        "qp$": 6636792.452830189,
+        "qps": 2345.0,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
         "label": 1,
-        "latency": 45.0,
-        "qp$": 0.0,
-        "qps": 37.878,
+        "latency": 12.3,
+        "qp$": 836603.7735849057,
+        "qps": 295.6,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 6.0,
-        "qp$": 0.0,
-        "qps": 180.2757,
-        "recall": 0.9942
+        "latency": 33.5,
+        "qp$": 3237735.8490566034,
+        "qps": 143.0,
+        "recall": 0.9818
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 6.4,
-        "qp$": 0.0,
-        "qps": 179.0033,
-        "recall": 0.9943
+        "latency": 20.7,
+        "qp$": 2400000.0,
+        "qps": 106.0,
+        "recall": 0.9887
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 3.6,
-        "qp$": 0.0,
-        "qps": 526.8846,
+        "latency": 11.6,
+        "qp$": 4279245.2830188675,
+        "qps": 189.0,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (500K Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 6.2,
-        "qp$": 0.0,
-        "qps": 626.5243,
-        "recall": 0.9954
+        "latency": 12.4,
+        "qp$": 4301570.9433962265,
+        "qps": 379.9721,
+        "recall": 0.982
     },
     {
         "case": "Search Performance Test (5M Dataset, 1536 Dim)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 25.3,
-        "qp$": 0.0,
-        "qps": 78.4227,
-        "recall": 0.9982
+        "latency": 50.8,
+        "qp$": 812150.9433962264,
+        "qps": 71.74,
+        "recall": 0.9883
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 6.6,
-        "qp$": 0.0,
-        "qps": 599.4213,
-        "recall": 0.9955
+        "latency": 14.9,
+        "qp$": 3249056.603773585,
+        "qps": 287.0,
+        "recall": 0.9865
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 26.3,
-        "qp$": 0.0,
-        "qps": 78.5351,
-        "recall": 0.9982
+        "latency": 64.69999999999999,
+        "qp$": 392438.4905660377,
+        "qps": 34.6654,
+        "recall": 0.9961
     },
     {
         "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 3.4,
-        "qp$": 0.0,
-        "qps": 2098.2113,
+        "latency": 10.3,
+        "qp$": 4664150.9433962265,
+        "qps": 412.0,
         "recall": 1.0
     },
     {
         "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 10.0,
-        "qp$": 0.0,
-        "qps": 275.6292,
+        "latency": 46.800000000000004,
+        "qp$": 477384.9056603773,
+        "qps": 42.169,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 21.1,
-        "qp$": 0.0,
-        "qps": 100.6667,
-        "recall": 0.9909
+        "latency": 9.0,
+        "qp$": 7472024.150943397,
+        "qps": 330.0144,
+        "recall": 0.9507
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 19.7,
-        "qp$": 0.0,
-        "qps": 101.1399,
-        "recall": 0.9907
+        "latency": 10.1,
+        "qp$": 6150758.490566038,
+        "qps": 271.6585,
+        "recall": 0.9678
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": 1,
-        "latency": 18.3,
-        "qp$": 0.0,
-        "qps": 52.2606,
+        "latency": 12.9,
+        "qp$": 4902398.490566038,
+        "qps": 216.5226,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-disk",
-        "db_name": "Milvus-2c8g-disk",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap",
+        "db_name": "ZillizCloud-1cu-cap",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 49.8,
-        "qp$": 0.0,
-        "qps": 61.0661,
-        "recall": 0.9911
+        "latency": 23.0,
+        "qp$": 1403267.5471698113,
+        "qps": 123.9553,
+        "recall": 0.971
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 44.6,
-        "qp$": 0.0,
-        "qps": 58.9326,
-        "recall": 0.9911
+        "latency": 44.5,
+        "qp$": 669598.8679245282,
+        "qps": 59.1479,
+        "recall": 0.9906
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 54.9,
-        "qp$": 0.0,
-        "qps": 42.5977,
+        "latency": 55.300000000000004,
+        "qp$": 464139.62264150946,
+        "qps": 40.999,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 8.200000000000001,
-        "qp$": 0.0,
-        "qps": 536.0726,
-        "recall": 0.9728
+        "latency": 9.4,
+        "qp$": 6565376.603773585,
+        "qps": 579.9416,
+        "recall": 0.9213
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 7.0,
-        "qp$": 0.0,
-        "qps": 467.179,
-        "recall": 0.9697
+        "latency": 11.299999999999999,
+        "qp$": 4814183.773584905,
+        "qps": 425.2529,
+        "recall": 0.9686
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "4c16g-disk",
-        "db_name": "Milvus-4c16g-disk",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap",
+        "db_name": "ZillizCloud-2cu-cap",
         "label": 1,
-        "latency": 8.3,
-        "qp$": 0.0,
-        "qps": 431.7512,
+        "latency": 13.799999999999999,
+        "qp$": 4494949.811320755,
+        "qps": 397.0539,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": 1,
-        "latency": 4.8999999999999995,
-        "qp$": 0.0,
-        "qps": 274.5407,
-        "recall": 0.9807
+        "latency": 7.0,
+        "qp$": 11689132.075471697,
+        "qps": 516.27,
+        "recall": 0.9463
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": 1,
-        "latency": 10.3,
-        "qp$": 0.0,
-        "qps": 236.5672,
-        "recall": 0.981
+        "latency": 10.0,
+        "qp$": 8034149.433962264,
+        "qps": 354.8416,
+        "recall": 0.9802
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": 1,
-        "latency": 4.3,
-        "qp$": 0.0,
-        "qps": 309.4833,
+        "latency": 8.7,
+        "qp$": 9679763.773584906,
+        "qps": 427.5229,
         "recall": 1.0
     },
     {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "2c8g-hnsw",
-        "db_name": "Milvus-2c8g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf",
+        "db_name": "ZillizCloud-1cu-perf",
         "label": -1,
         "latency": 0.0,
         "qp$": 0.0,
         "qps": 0.0,
         "recall": 0.0
     },
     {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 5.3,
+        "qp$": 8164214.150943396,
+        "qps": 2884.689,
+        "recall": 0.8801
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 6.6,
+        "qp$": 4781829.905660377,
+        "qps": 1689.5799,
+        "recall": 0.9493
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 10.0,
+        "qp$": 4295318.4905660385,
+        "qps": 1517.6792,
+        "recall": 1.0
+    },
+    {
         "case": "Search Performance Test (10M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
         "label": 1,
-        "latency": 13.700000000000001,
+        "latency": 5.6,
+        "qp$": 2327920.1886792453,
+        "qps": 822.5318,
+        "recall": 0.9294
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 10.3,
+        "qp$": 1072399.8113207547,
+        "qps": 378.9146,
+        "recall": 0.9758
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf",
+        "db_name": "ZillizCloud-8cu-perf",
+        "label": 1,
+        "latency": 16.2,
+        "qp$": 618920.9433962263,
+        "qps": 218.6854,
+        "recall": 1.0
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.7,
         "qp$": 0.0,
-        "qps": 178.6585,
-        "recall": 0.9843
+        "qps": 5115.5303,
+        "recall": 0.9469
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 9.1,
+        "qp$": 0.0,
+        "qps": 3685.0767,
+        "recall": 0.9736
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 9.1,
+        "qp$": 0.0,
+        "qps": 4742.1617,
+        "recall": 0.9936
+    },
+    {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.1,
+        "qp$": 0.0,
+        "qps": 6054.4428,
+        "recall": 0.9155
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 10.6,
+        "qp$": 0.0,
+        "qps": 4104.2598,
+        "recall": 0.9506
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 9.2,
+        "qp$": 0.0,
+        "qps": 4252.1267,
+        "recall": 0.9964
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 13.299999999999999,
+        "qp$": 0.0,
+        "qps": 1685.3091,
+        "recall": 0.9718
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 10.7,
+        "qp$": 0.0,
+        "qps": 769.8991,
+        "recall": 0.9884
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 10.9,
+        "qp$": 0.0,
+        "qps": 945.4061,
+        "recall": 0.9941
+    },
+    {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.4,
+        "qp$": 0.0,
+        "qps": 2214.9028,
+        "recall": 0.9249
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
         "label": 1,
-        "latency": 15.0,
+        "latency": 12.0,
         "qp$": 0.0,
-        "qps": 178.3732,
-        "recall": 0.9844
+        "qps": 827.975,
+        "recall": 0.9692
     },
     {
         "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "8cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-8cu-perf-(Jan-2024)",
         "label": 1,
-        "latency": 12.5,
+        "latency": 11.4,
         "qp$": 0.0,
-        "qps": 229.3526,
-        "recall": 1.0
+        "qps": 776.9454,
+        "recall": 0.9966
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 9.799999999999999,
+        "qp$": 0.0,
+        "qps": 269.5464,
+        "recall": 0.9776
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 10.6,
+        "qp$": 0.0,
+        "qps": 240.0363,
+        "recall": 0.9822
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 11.4,
+        "qp$": 0.0,
+        "qps": 218.0627,
+        "recall": 0.9936
     },
     {
         "case": "Search Performance Test (1M Dataset, 768 Dim)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
         "label": 1,
-        "latency": 4.8999999999999995,
+        "latency": 6.8999999999999995,
         "qp$": 0.0,
-        "qps": 1258.7043,
-        "recall": 0.9799
+        "qps": 392.8825,
+        "recall": 0.9581
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
         "label": 1,
-        "latency": 5.3,
+        "latency": 8.4,
         "qp$": 0.0,
-        "qps": 1075.8776,
-        "recall": 0.98
+        "qps": 343.8204,
+        "recall": 0.968
     },
     {
         "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
-        "db": "Milvus",
-        "db_label": "16c64g-hnsw",
-        "db_name": "Milvus-16c64g-hnsw",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
         "label": 1,
-        "latency": 4.7,
+        "latency": 10.1,
         "qp$": 0.0,
-        "qps": 1494.8493,
-        "recall": 1.0
+        "qps": 216.6773,
+        "recall": 0.9968
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 9.0,
+        "qp$": 0.0,
+        "qps": 503.2284,
+        "recall": 0.9677
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 9.6,
+        "qp$": 0.0,
+        "qps": 413.3232,
+        "recall": 0.981
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 10.200000000000001,
+        "qp$": 0.0,
+        "qps": 425.5492,
+        "recall": 0.9936
+    },
+    {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 5.6,
+        "qp$": 0.0,
+        "qps": 789.1229,
+        "recall": 0.9396
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 7.7,
+        "qp$": 0.0,
+        "qps": 571.4257,
+        "recall": 0.9668
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 9.1,
+        "qp$": 0.0,
+        "qps": 411.7653,
+        "recall": 0.9968
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 16.1,
+        "qp$": 0.0,
+        "qps": 98.0448,
+        "recall": 0.9803
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 28.0,
+        "qp$": 0.0,
+        "qps": 58.3152,
+        "recall": 0.9891
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 28.6,
+        "qp$": 0.0,
+        "qps": 46.8304,
+        "recall": 0.9941
+    },
+    {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 8.9,
+        "qp$": 0.0,
+        "qps": 170.5693,
+        "recall": 0.9605
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 19.599999999999998,
+        "qp$": 0.0,
+        "qps": 94.7766,
+        "recall": 0.9843
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "2cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-2cu-cap-(Jan-2024)",
+        "label": 1,
+        "latency": 30.900000000000002,
+        "qp$": 0.0,
+        "qps": 44.8695,
+        "recall": 0.9966
+    },
+    {
+        "case": "Search Performance Test (500K Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 7.7,
+        "qp$": 0.0,
+        "qps": 722.0315,
+        "recall": 0.976
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.8,
+        "qp$": 0.0,
+        "qps": 467.5795,
+        "recall": 0.9898
+    },
+    {
+        "case": "Filtering Search Performance Test (500K Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.200000000000001,
+        "qp$": 0.0,
+        "qps": 975.2503,
+        "recall": 0.9936
+    },
+    {
+        "case": "Search Performance Test (1M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 6.7,
+        "qp$": 0.0,
+        "qps": 873.3712,
+        "recall": 0.9477
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 8.4,
+        "qp$": 0.0,
+        "qps": 544.6203,
+        "recall": 0.977
+    },
+    {
+        "case": "Filtering Search Performance Test (1M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": 1,
+        "latency": 9.6,
+        "qp$": 0.0,
+        "qps": 930.9164,
+        "recall": 0.9968
+    },
+    {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-perf-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-perf-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Search Performance Test (10M Dataset, 768 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (10M Dataset, 768 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Search Performance Test (5M Dataset, 1536 Dim)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 1%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
+    },
+    {
+        "case": "Filtering Search Performance Test (5M Dataset, 1536 Dim, Filter 99%)",
+        "db": "ZillizCloud",
+        "db_label": "1cu-cap-(Jan-2024)",
+        "db_name": "ZillizCloud-1cu-cap-(Jan-2024)",
+        "label": -1,
+        "latency": 0.0,
+        "qp$": 0.0,
+        "qps": 0.0,
+        "recall": 0.0
     }
 ]
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench.egg-info/PKG-INFO` & `vectordb_bench-0.0.8/vectordb_bench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectordb-bench
-Version: 0.0.7
+Version: 0.0.8
 Summary: VectorDBBench is not just an offering of benchmark results for mainstream vector databases and cloud services, it's your go-to tool for the ultimate performance and cost-effectiveness comparison. Designed with ease-of-use in mind, VectorDBBench is devised to help users, even non-professionals, reproduce results or test new systems, making the hunt for the optimal choice amongst a plethora of cloud services and open-source vector databases a breeze.
 Author-email: XuanYang-cn <xuan.yang@zilliz.com>
 Project-URL: repository, https://github.com/zilliztech/VectorDBBench
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -45,15 +45,15 @@
 Requires-Dist: pinecone-client; extra == "pinecone"
 Provides-Extra: weaviate
 Requires-Dist: weaviate-client; extra == "weaviate"
 Provides-Extra: elastic
 Requires-Dist: elasticsearch; extra == "elastic"
 Provides-Extra: pgvector
 Requires-Dist: pgvector; extra == "pgvector"
-Requires-Dist: sqlalchemy; extra == "pgvector"
+Requires-Dist: psycopg2; extra == "pgvector"
 Provides-Extra: pgvecto-rs
 Requires-Dist: psycopg2; extra == "pgvecto-rs"
 Provides-Extra: redis
 Requires-Dist: redis; extra == "redis"
 Provides-Extra: chromadb
 Requires-Dist: chromadb; extra == "chromadb"
```

### Comparing `vectordb-bench-0.0.7/vectordb_bench.egg-info/SOURCES.txt` & `vectordb_bench-0.0.8/vectordb_bench.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -107,8 +107,8 @@
 vectordb_bench/results/Pinecone/result_20230808_standard_pinecone.json
 vectordb_bench/results/QdrantCloud/result_20230727_standard_qdrantcloud.json
 vectordb_bench/results/QdrantCloud/result_20230808_standard_qdrantcloud.json
 vectordb_bench/results/WeaviateCloud/result_20230727_standard_weaviatecloud.json
 vectordb_bench/results/WeaviateCloud/result_20230808_standard_weaviatecloud.json
 vectordb_bench/results/ZillizCloud/result_20230727_standard_zillizcloud.json
 vectordb_bench/results/ZillizCloud/result_20230808_standard_zillizcloud.json
-vectordb_bench/results/ZillizCloud/result_20240105_beta_202401_zillizcloud.json
+vectordb_bench/results/ZillizCloud/result_20240105_standard_202401_zillizcloud.json
```

