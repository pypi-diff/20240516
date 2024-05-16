# Comparing `tmp/astronomer_cosmos-1.4.0rc1.tar.gz` & `tmp/astronomer_cosmos-1.4.1rc1.tar.gz`

## Comparing `astronomer_cosmos-1.4.0rc1.tar` & `astronomer_cosmos-1.4.1rc1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/__init__.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/cache.py
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/config.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/constants.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/converter.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/exceptions.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/log.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    18527 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/project.py
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    32840 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/local.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/__init__.py
--rwxr-xr-x   0        0        0    11351 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/README.rst
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/__init__.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/config.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/constants.py
+-rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/converter.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/log.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    33776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11466 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/README.rst
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/PKG-INFO
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/__init__.py` & `astronomer_cosmos-1.4.1rc1/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.4.0rc1"
+__version__ = "1.4.1rc1"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/cache.py` & `astronomer_cosmos-1.4.1rc1/cosmos/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import msgpack
 from airflow.models.dag import DAG
 from airflow.utils.task_group import TaskGroup
 
 from cosmos import settings
 from cosmos.constants import DBT_MANIFEST_FILE_NAME, DBT_TARGET_DIR_NAME
 from cosmos.dbt.project import get_partial_parse_path
+from cosmos.log import get_logger
+
+logger = get_logger()
 
 
 # It was considered to create a cache identifier based on the dbt project path, as opposed
 # to where it is used in Airflow. However, we could have concurrency issues if the same
 # dbt cached directory was being used by different dbt task groups or DAGs within the same
 # node. For this reason, as a starting point, the cache is identified by where it is used.
 # This can be reviewed in the future.
@@ -104,14 +107,55 @@
     manifest_path = get_partial_parse_path(cache_dir).parent / DBT_MANIFEST_FILE_NAME
     latest_manifest_filepath = latest_partial_parse_filepath.parent / DBT_MANIFEST_FILE_NAME
 
     shutil.copy(str(latest_partial_parse_filepath), str(cache_path))
     shutil.copy(str(latest_manifest_filepath), str(manifest_path))
 
 
+def patch_partial_parse_content(partial_parse_filepath: Path, project_path: Path) -> bool:
+    """
+    Update, if needed, the root_path references in partial_parse.msgpack to an existing project directory.
+    This is necessary because an issue is observed where on specific earlier versions of dbt-core like 1.5.4 and 1.6.5,
+    the commands fail to locate project files as they are pointed to a stale directory by the root_path in the partial
+    parse file.
+
+    This issue was not observed on recent versions of dbt-core 1.5.8, 1.6.6, 1.7.0 and 1.8.0 as tested on.
+    It is suspected that PR dbt-labs/dbt-core#8762 is likely the fix and the fix appears to be backported to later
+    version releases of 1.5.x and 1.6.x. However, the below modification is applied to ensure that the root_path is
+    correctly set to the needed project directory and the feature is compatible across all dbt-core versions.
+
+    :param partial_parse_filepath: Path to the most up-to-date partial parse file
+    :param project_path: Path to the target dbt project directory
+    """
+    should_patch_partial_parse_content = False
+
+    try:
+        with partial_parse_filepath.open("rb") as f:
+            # Issue reported: https://github.com/astronomer/astronomer-cosmos/issues/971
+            # it may be due a race condition of multiple processes trying to read/write this file
+            data = msgpack.unpack(f)
+    except ValueError as e:
+        logger.info("Unable to patch the partial_parse.msgpack file due to %s" % repr(e))
+    else:
+        for node in data["nodes"].values():
+            expected_filepath = node.get("root_path")
+            if expected_filepath is None:
+                continue
+            elif expected_filepath and not Path(expected_filepath).exists():
+                node["root_path"] = str(project_path)
+                should_patch_partial_parse_content = True
+            else:
+                break
+        if should_patch_partial_parse_content:
+            with partial_parse_filepath.open("wb") as f:
+                packed = msgpack.packb(data)
+                f.write(packed)
+    return should_patch_partial_parse_content
+
+
 def _copy_partial_parse_to_project(partial_parse_filepath: Path, project_path: Path) -> None:
     """
     Update target dbt project directory to have the latest partial parse file contents.
 
     :param partial_parse_filepath: Path to the most up-to-date partial parse file
     :param project_path: Path to the target dbt project directory
     """
@@ -119,24 +163,11 @@
     tmp_target_dir = project_path / DBT_TARGET_DIR_NAME
     tmp_target_dir.mkdir(exist_ok=True)
 
     source_manifest_filepath = partial_parse_filepath.parent / DBT_MANIFEST_FILE_NAME
     target_manifest_filepath = target_partial_parse_file.parent / DBT_MANIFEST_FILE_NAME
     shutil.copy(str(partial_parse_filepath), str(target_partial_parse_file))
 
-    # Update root_path in partial parse file to point to the needed project directory. This is necessary because
-    # an issue is observed where on specific earlier versions of dbt-core like 1.5.4 and 1.6.5, the commands fail to
-    # locate project files as they are pointed to a stale directory by the root_path in the partial parse file.
-    # This issue was not observed on recent versions of dbt-core 1.5.8, 1.6.6, 1.7.0 and 1.8.0 as tested on.
-    # It is suspected that PR dbt-labs/dbt-core#8762 is likely the fix and the fix appears to be backported to later
-    # version releases of 1.5.x and 1.6.x. However, the below modification is applied to ensure that the root_path is
-    # correctly set to the needed project directory and the feature is compatible across all dbt-core versions.
-    with target_partial_parse_file.open("rb") as f:
-        data = msgpack.unpack(f)
-    for node in data["nodes"].values():
-        if node.get("root_path"):
-            node["root_path"] = str(project_path)
-    with target_partial_parse_file.open("wb") as f:
-        packed = msgpack.packb(data)
-        f.write(packed)
+    patch_partial_parse_content(target_partial_parse_file, project_path)
 
-    shutil.copy(str(source_manifest_filepath), str(target_manifest_filepath))
+    if source_manifest_filepath.exists():
+        shutil.copy(str(source_manifest_filepath), str(target_manifest_filepath))
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/config.py` & `astronomer_cosmos-1.4.1rc1/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/constants.py` & `astronomer_cosmos-1.4.1rc1/cosmos/constants.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/converter.py` & `astronomer_cosmos-1.4.1rc1/cosmos/converter.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/log.py` & `astronomer_cosmos-1.4.1rc1/cosmos/log.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/airflow/dag.py` & `astronomer_cosmos-1.4.1rc1/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/airflow/graph.py` & `astronomer_cosmos-1.4.1rc1/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.4.1rc1/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/core/airflow.py` & `astronomer_cosmos-1.4.1rc1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.4.1rc1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/dbt/graph.py` & `astronomer_cosmos-1.4.1rc1/cosmos/dbt/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,12 +436,13 @@
     def update_node_dependency(self) -> None:
         """
         This will update the property `has_test` if node has `dbt` test
 
         Updates in-place:
         * self.filtered_nodes
         """
-        for _, node in self.filtered_nodes.items():
+        for _, node in list(self.nodes.items()):
             if node.resource_type == DbtResourceType.TEST:
                 for node_id in node.depends_on:
                     if node_id in self.filtered_nodes:
                         self.filtered_nodes[node_id].has_test = True
+                        self.filtered_nodes[node.unique_id] = node
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/dbt/project.py` & `astronomer_cosmos-1.4.1rc1/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/dbt/selector.py` & `astronomer_cosmos-1.4.1rc1/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.4.1rc1/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/__init__.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/azure_container_instance.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/base.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     :param warn_error: dbt optional argument to convert dbt warnings into errors
     :param db_name: override the target db instead of the one supplied in the airflow connection
     :param schema: override the target schema instead of the one supplied in the airflow connection
     :param env: If env is not None, it must be a dict that defines the
         environment variables for the new process; these are used instead
         of inheriting the current process environment, which is the default
         behavior. (templated)
-    :param append_env: . If True (default), inherits the environment variables
-        from current passes and then environment variable passed by the user will either update the existing
+    :param append_env: If True, inherits the environment variables
+        from current process and then environment variable passed by the user will either update the existing
         inherited environment variables or the new variables gets appended to it.
-        If False, only uses the environment variables passed in env params
+        If False (default), only uses the environment variables passed in env params
         and does not inherit the current process environment.
     :param output_encoding: Output encoding of bash command
     :param skip_exit_code: If task exits with this exit code, leave the task
         in ``skipped`` state (default: 99). If set to ``None``, any non-zero
         exit code will be treated as a failure.
     :param partial_parse: If True (default), then the operator will use the
         ``partial_parse.msgpack`` during execution if it exists. If False, then
@@ -100,15 +100,15 @@
         no_version_check: bool = False,
         fail_fast: bool = False,
         quiet: bool = False,
         warn_error: bool = False,
         db_name: str | None = None,
         schema: str | None = None,
         env: dict[str, Any] | None = None,
-        append_env: bool = True,
+        append_env: bool = False,
         output_encoding: str = "utf-8",
         skip_exit_code: int = 99,
         partial_parse: bool = True,
         cancel_query_on_kill: bool = True,
         dbt_executable_path: str = get_system_dbt(),
         dbt_cmd_flags: list[str] | None = None,
         dbt_cmd_global_flags: list[str] | None = None,
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/docker.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/local.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,28 +109,34 @@
     :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
         in your project's dbt_project.yml, "cosmos_profile" is used.
     :param install_deps: If true, install dependencies before running the command
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
     :param target_name: A name to use for the dbt target. If not provided, and no target is found
         in your project's dbt_project.yml, "cosmos_target" is used.
     :param should_store_compiled_sql: If true, store the compiled SQL in the compiled_sql rendered template.
+    :param append_env: If True(default), inherits the environment variables
+        from current process and then environment variable passed by the user will either update the existing
+        inherited environment variables or the new variables gets appended to it.
+        If False, only uses the environment variables passed in env params
+        and does not inherit the current process environment.
     """
 
     template_fields: Sequence[str] = AbstractDbtBaseOperator.template_fields + ("compiled_sql",)  # type: ignore[operator]
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
 
     def __init__(
         self,
         profile_config: ProfileConfig,
         invocation_mode: InvocationMode | None = None,
         install_deps: bool = False,
         callback: Callable[[str], None] | None = None,
         should_store_compiled_sql: bool = True,
+        append_env: bool = True,
         **kwargs: Any,
     ) -> None:
         self.profile_config = profile_config
         self.install_deps = install_deps
         self.callback = callback
         self.compiled_sql = ""
         self.should_store_compiled_sql = should_store_compiled_sql
@@ -140,14 +146,20 @@
         self.handle_exception: Callable[..., None]
         self._dbt_runner: dbtRunner | None = None
         if self.invocation_mode:
             self._set_invocation_methods()
         kwargs.pop("full_refresh", None)  # usage of this param should be implemented in child classes
         super().__init__(**kwargs)
 
+        # For local execution mode, we're consistent with the LoadMode.DBT_LS command in forwarding the environment
+        # variables to the subprocess by default. Although this behavior is designed for ExecuteMode.LOCAL and
+        # ExecuteMode.VIRTUALENV, it is not desired for the other execution modes to forward the environment variables
+        # as it can break existing DAGs.
+        self.append_env = append_env
+
     @cached_property
     def subprocess_hook(self) -> FullOutputSubprocessHook:
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
 
     def _set_invocation_methods(self) -> None:
         """Sets the associated run and exception handling methods based on the invocation mode."""
@@ -222,14 +234,16 @@
         # need to refresh the rendered task field record in the db because Airflow only does this
         # before executing the task, not after
         from airflow.models.renderedtifields import RenderedTaskInstanceFields
 
         ti = context["ti"]
 
         if isinstance(ti, TaskInstance):  # verifies ti is a TaskInstance in order to access and use the "task" field
+            if TYPE_CHECKING:
+                assert ti.task is not None
             ti.task.template_fields = self.template_fields
             rtif = RenderedTaskInstanceFields(ti, render_templates=False)
 
             # delete the old records
             session.query(RenderedTaskInstanceFields).filter(
                 RenderedTaskInstanceFields.dag_id == self.dag_id,
                 RenderedTaskInstanceFields.task_id == self.task_id,
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.4.1rc1/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.4.1rc1/cosmos/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/base.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     log_format: Optional[Literal["text", "json", "default"]] = None
     debug: Optional[bool] = None
     version_check: Optional[bool] = None
 
     def as_dict(self) -> dict[str, Any] | None:
         result = {
             field.name: getattr(self, field.name)
-            for field in self.__dataclass_fields__.values()
+            # Look like the __dataclass_fields__ attribute is not recognized by mypy
+            for field in self.__dataclass_fields__.values()  # type: ignore[attr-defined]
             if getattr(self, field.name) is not None
         }
         if result != {}:
             return result
         return None
```

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/.gitignore` & `astronomer_cosmos-1.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/LICENSE` & `astronomer_cosmos-1.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/README.rst` & `astronomer_cosmos-1.4.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.0rc1/pyproject.toml` & `astronomer_cosmos-1.4.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     "pytest-split",
     "pytest-dotenv",
     "requests-mock",
     "pytest-cov",
     "pytest-describe",
     "sqlalchemy-stubs", # Change when sqlalchemy is upgraded https://docs.sqlalchemy.org/en/14/orm/extensions/mypy.html
     "types-requests",
-    "mypy",
     "sqlalchemy-stubs", # Change when sqlalchemy is upgraded https://docs.sqlalchemy.org/en/14/orm/extensions/mypy.html
+    "pre-commit",
 ]
 docker = [
     "apache-airflow-providers-docker>=3.5.0",
 ]
 kubernetes = [
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
 ]
@@ -148,15 +148,15 @@
 test-integration-dbt-1-5-4 = 'sh scripts/test/integration-dbt-1-5-4.sh'
 test-integration-expensive = 'sh scripts/test/integration-expensive.sh'
 test-integration-setup = 'sh scripts/test/integration-setup.sh'
 test-integration-sqlite = 'sh scripts/test/integration-sqlite.sh'
 test-integration-sqlite-setup = 'sh scripts/test/integration-sqlite-setup.sh'
 test-performance = 'sh scripts/test/performance.sh'
 test-performance-setup = 'sh scripts/test/performance-setup.sh'
-type-check = "mypy cosmos"
+type-check = " pre-commit run mypy --files cosmos/**/*"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 minversion = "6.0"
 markers = ["integration", "sqlite", "perf"]
 
 ######################################
```

### Comparing `astronomer_cosmos-1.4.0rc1/PKG-INFO` & `astronomer_cosmos-1.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.4.0rc1
+Version: 1.4.1rc1
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -85,16 +85,16 @@
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Provides-Extra: kubernetes
 Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: openlineage
 Requires-Dist: openlineage-airflow; extra == 'openlineage'
 Requires-Dist: openlineage-integration-common; extra == 'openlineage'
 Provides-Extra: tests
-Requires-Dist: mypy; extra == 'tests'
 Requires-Dist: packaging; extra == 'tests'
+Requires-Dist: pre-commit; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
 Requires-Dist: pytest>=6.0; extra == 'tests'
 Requires-Dist: requests-mock; extra == 'tests'
 Requires-Dist: sqlalchemy-stubs; extra == 'tests'
```

