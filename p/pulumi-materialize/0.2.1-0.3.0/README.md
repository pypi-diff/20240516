# Comparing `tmp/pulumi_materialize-0.2.1.tar.gz` & `tmp/pulumi_materialize-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_materialize-0.2.1.tar", last modified: Wed May  1 15:55:28 2024, max compression
+gzip compressed data, was "pulumi_materialize-0.3.0.tar", last modified: Thu May 16 19:15:49 2024, max compression
```

## Comparing `pulumi_materialize-0.2.1.tar` & `pulumi_materialize-0.3.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.728999 pulumi_materialize-0.2.1/pulumi_materialize/
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   215981 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/app_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cloud_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    31143 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26832 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/cluster_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/pulumi_materialize/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    38914 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    27823 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    46164 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_confluent_schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    54296 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    47009 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    48996 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    28427 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/connection_ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_cluster_replicas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_current_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_egress_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_materialized_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_scim_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_system_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/get_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_connection_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_database_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_schema_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_secret_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_system_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_table_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_type_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/grant_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    24868 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)   247075 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/role_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    21129 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    44072 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sink_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    68769 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    41564 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_loadgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    36112 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/source_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/sso_role_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/system_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22074 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    27564 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/pulumi_materialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:55:28.732998 pulumi_materialize-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-01 15:55:28.000000 pulumi_materialize-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:15:49.843861 pulumi_materialize-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-16 19:15:49.843861 pulumi_materialize-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:15:49.839861 pulumi_materialize-0.3.0/pulumi_materialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211667 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/app_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/cloud_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31143 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26832 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/cluster_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:15:49.843861 pulumi_materialize-0.3.0/pulumi_materialize/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38914 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27823 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46164 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_confluent_schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54296 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47009 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48996 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28427 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/connection_ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_cluster_replicas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_current_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_egress_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_materialized_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_scim_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_system_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_cluster_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_connection_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15687 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_database_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_schema_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_secret_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17336 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_system_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17548 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20733 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_table_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_type_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/grant_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24868 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)   242606 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/role_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/scim2_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/scim2_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/scim2_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/scim2_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21129 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44072 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/sink_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67456 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/source_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40237 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/source_loadgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36251 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/source_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35899 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/source_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36214 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/source_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/sso_default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/sso_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/sso_role_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/system_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22074 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27564 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:15:49.843861 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/pulumi_materialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:15:49.843861 pulumi_materialize-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-16 19:15:49.000000 pulumi_materialize-0.3.0/setup.py
```

### Comparing `pulumi_materialize-0.2.1/PKG-INFO` & `pulumi_materialize-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_materialize
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.2.1/README.md` & `pulumi_materialize-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/__init__.py` & `pulumi_materialize-0.3.0/pulumi_materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/_inputs.py` & `pulumi_materialize-0.3.0/pulumi_materialize/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,41 +84,37 @@
     'SourceKafkaKafkaConnectionArgs',
     'SourceKafkaKeyFormatArgs',
     'SourceKafkaKeyFormatAvroArgs',
     'SourceKafkaKeyFormatAvroSchemaRegistryConnectionArgs',
     'SourceKafkaKeyFormatCsvArgs',
     'SourceKafkaKeyFormatProtobufArgs',
     'SourceKafkaKeyFormatProtobufSchemaRegistryConnectionArgs',
-    'SourceKafkaSubsourceArgs',
     'SourceKafkaValueFormatArgs',
     'SourceKafkaValueFormatAvroArgs',
     'SourceKafkaValueFormatAvroSchemaRegistryConnectionArgs',
     'SourceKafkaValueFormatCsvArgs',
     'SourceKafkaValueFormatProtobufArgs',
     'SourceKafkaValueFormatProtobufSchemaRegistryConnectionArgs',
     'SourceLoadgenAuctionOptionsArgs',
     'SourceLoadgenCounterOptionsArgs',
     'SourceLoadgenExposeProgressArgs',
     'SourceLoadgenKeyValueOptionsArgs',
     'SourceLoadgenMarketingOptionsArgs',
-    'SourceLoadgenSubsourceArgs',
     'SourceLoadgenTpchOptionsArgs',
+    'SourceMysqlExposeProgressArgs',
     'SourceMysqlMysqlConnectionArgs',
-    'SourceMysqlSubsourceArgs',
     'SourceMysqlTableArgs',
     'SourcePostgresExposeProgressArgs',
     'SourcePostgresPostgresConnectionArgs',
-    'SourcePostgresSubsourceArgs',
     'SourcePostgresTableArgs',
     'SourceWebhookCheckOptionArgs',
     'SourceWebhookCheckOptionFieldArgs',
     'SourceWebhookCheckOptionFieldSecretArgs',
     'SourceWebhookIncludeHeaderArgs',
     'SourceWebhookIncludeHeadersArgs',
-    'SourceWebhookSubsourceArgs',
     'TableColumnArgs',
     'TypeListPropertiesArgs',
     'TypeMapPropertiesArgs',
     'TypeRowPropertyArgs',
 ]
 
 @pulumi.input_type
@@ -4035,68 +4031,14 @@
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
 
 @pulumi.input_type
-class SourceKafkaSubsourceArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 database_name: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The identifier for the source.
-        :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @database_name.setter
-    def database_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "database_name", value)
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-    @schema_name.setter
-    def schema_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema_name", value)
-
-
-@pulumi.input_type
 class SourceKafkaValueFormatArgs:
     def __init__(__self__, *,
                  avro: Optional[pulumi.Input['SourceKafkaValueFormatAvroArgs']] = None,
                  bytes: Optional[pulumi.Input[bool]] = None,
                  csvs: Optional[pulumi.Input[Sequence[pulumi.Input['SourceKafkaValueFormatCsvArgs']]]] = None,
                  json: Optional[pulumi.Input[bool]] = None,
                  protobuf: Optional[pulumi.Input['SourceKafkaValueFormatProtobufArgs']] = None,
@@ -4747,68 +4689,14 @@
 
     @tick_interval.setter
     def tick_interval(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tick_interval", value)
 
 
 @pulumi.input_type
-class SourceLoadgenSubsourceArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 database_name: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The identifier for the source.
-        :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @database_name.setter
-    def database_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "database_name", value)
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-    @schema_name.setter
-    def schema_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema_name", value)
-
-
-@pulumi.input_type
 class SourceLoadgenTpchOptionsArgs:
     def __init__(__self__, *,
                  scale_factor: Optional[pulumi.Input[float]] = None,
                  tick_interval: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[float] scale_factor: The scale factor for the generator. Defaults to 0.01 (~ 10MB).
         :param pulumi.Input[str] tick_interval: The interval at which the next datum should be emitted. Defaults to one second.
@@ -4840,157 +4728,205 @@
 
     @tick_interval.setter
     def tick_interval(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tick_interval", value)
 
 
 @pulumi.input_type
-class SourceMysqlMysqlConnectionArgs:
+class SourceMysqlExposeProgressArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  database_name: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] name: The mysql_connection name.
-        :param pulumi.Input[str] database_name: The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The mysql_connection schema name. Defaults to `public`.
+        :param pulumi.Input[str] name: The expose_progress name.
+        :param pulumi.Input[str] database_name: The expose_progress database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input[str] schema_name: The expose_progress schema name. Defaults to `public`.
         """
         pulumi.set(__self__, "name", name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The mysql_connection name.
+        The expose_progress name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The expose_progress database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         """
         return pulumi.get(self, "database_name")
 
     @database_name.setter
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The mysql_connection schema name. Defaults to `public`.
+        The expose_progress schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
 
 @pulumi.input_type
-class SourceMysqlSubsourceArgs:
+class SourceMysqlMysqlConnectionArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  database_name: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] name: The identifier for the source.
-        :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
+        :param pulumi.Input[str] name: The mysql_connection name.
+        :param pulumi.Input[str] database_name: The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input[str] schema_name: The mysql_connection schema name. Defaults to `public`.
         """
         pulumi.set(__self__, "name", name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
-        The identifier for the source.
+        The mysql_connection name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         """
         return pulumi.get(self, "database_name")
 
     @database_name.setter
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the source schema in Materialize. Defaults to `public`.
+        The mysql_connection schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
 
 @pulumi.input_type
 class SourceMysqlTableArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 alias: Optional[pulumi.Input[str]] = None):
+                 upstream_name: pulumi.Input[str],
+                 database_name: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 schema_name: Optional[pulumi.Input[str]] = None,
+                 upstream_schema_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] name: The name of the table.
-        :param pulumi.Input[str] alias: An alias for the table, used in Materialize.
+        :param pulumi.Input[str] upstream_name: The name of the table in the upstream MySQL database.
+        :param pulumi.Input[str] database_name: The database of the table in Materialize.
+        :param pulumi.Input[str] name: The name for the table, used in Materialize.
+        :param pulumi.Input[str] schema_name: The schema of the table in Materialize.
+        :param pulumi.Input[str] upstream_schema_name: The schema of the table in the upstream MySQL database.
         """
-        pulumi.set(__self__, "name", name)
-        if alias is not None:
-            pulumi.set(__self__, "alias", alias)
+        pulumi.set(__self__, "upstream_name", upstream_name)
+        if database_name is not None:
+            pulumi.set(__self__, "database_name", database_name)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if schema_name is not None:
+            pulumi.set(__self__, "schema_name", schema_name)
+        if upstream_schema_name is not None:
+            pulumi.set(__self__, "upstream_schema_name", upstream_schema_name)
+
+    @property
+    @pulumi.getter(name="upstreamName")
+    def upstream_name(self) -> pulumi.Input[str]:
+        """
+        The name of the table in the upstream MySQL database.
+        """
+        return pulumi.get(self, "upstream_name")
+
+    @upstream_name.setter
+    def upstream_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "upstream_name", value)
+
+    @property
+    @pulumi.getter(name="databaseName")
+    def database_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The database of the table in Materialize.
+        """
+        return pulumi.get(self, "database_name")
+
+    @database_name.setter
+    def database_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the table.
+        The name for the table, used in Materialize.
         """
         return pulumi.get(self, "name")
 
     @name.setter
-    def name(self, value: pulumi.Input[str]):
+    def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def alias(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="schemaName")
+    def schema_name(self) -> Optional[pulumi.Input[str]]:
         """
-        An alias for the table, used in Materialize.
+        The schema of the table in Materialize.
         """
-        return pulumi.get(self, "alias")
+        return pulumi.get(self, "schema_name")
 
-    @alias.setter
-    def alias(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "alias", value)
+    @schema_name.setter
+    def schema_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "schema_name", value)
+
+    @property
+    @pulumi.getter(name="upstreamSchemaName")
+    def upstream_schema_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The schema of the table in the upstream MySQL database.
+        """
+        return pulumi.get(self, "upstream_schema_name")
+
+    @upstream_schema_name.setter
+    def upstream_schema_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "upstream_schema_name", value)
 
 
 @pulumi.input_type
 class SourcePostgresExposeProgressArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  database_name: Optional[pulumi.Input[str]] = None,
@@ -5094,103 +5030,97 @@
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
 
 @pulumi.input_type
-class SourcePostgresSubsourceArgs:
+class SourcePostgresTableArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
+                 upstream_name: pulumi.Input[str],
                  database_name: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
+                 name: Optional[pulumi.Input[str]] = None,
+                 schema_name: Optional[pulumi.Input[str]] = None,
+                 upstream_schema_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] name: The identifier for the source.
-        :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
+        :param pulumi.Input[str] upstream_name: The name of the table in the upstream Postgres database.
+        :param pulumi.Input[str] database_name: The database of the table in Materialize.
+        :param pulumi.Input[str] name: The name of the table in Materialize.
+        :param pulumi.Input[str] schema_name: The schema of the table in Materialize.
+        :param pulumi.Input[str] upstream_schema_name: The schema of the table in the upstream Postgres database.
         """
-        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "upstream_name", upstream_name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
+        if upstream_schema_name is not None:
+            pulumi.set(__self__, "upstream_schema_name", upstream_schema_name)
 
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="upstreamName")
+    def upstream_name(self) -> pulumi.Input[str]:
         """
-        The identifier for the source.
+        The name of the table in the upstream Postgres database.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "upstream_name")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @upstream_name.setter
+    def upstream_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "upstream_name", value)
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The database of the table in Materialize.
         """
         return pulumi.get(self, "database_name")
 
     @database_name.setter
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the table in Materialize.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The identifier for the source schema in Materialize. Defaults to `public`.
+        The schema of the table in Materialize.
         """
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
-
-@pulumi.input_type
-class SourcePostgresTableArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 alias: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The name of the table.
-        :param pulumi.Input[str] alias: The alias of the table.
-        """
-        pulumi.set(__self__, "name", name)
-        if alias is not None:
-            pulumi.set(__self__, "alias", alias)
-
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The name of the table.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def alias(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="upstreamSchemaName")
+    def upstream_schema_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The alias of the table.
+        The schema of the table in the upstream Postgres database.
         """
-        return pulumi.get(self, "alias")
+        return pulumi.get(self, "upstream_schema_name")
 
-    @alias.setter
-    def alias(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "alias", value)
+    @upstream_schema_name.setter
+    def upstream_schema_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "upstream_schema_name", value)
 
 
 @pulumi.input_type
 class SourceWebhookCheckOptionArgs:
     def __init__(__self__, *,
                  field: pulumi.Input['SourceWebhookCheckOptionFieldArgs'],
                  alias: Optional[pulumi.Input[str]] = None,
@@ -5444,68 +5374,14 @@
 
     @onlies.setter
     def onlies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "onlies", value)
 
 
 @pulumi.input_type
-class SourceWebhookSubsourceArgs:
-    def __init__(__self__, *,
-                 name: pulumi.Input[str],
-                 database_name: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] name: The identifier for the source.
-        :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @database_name.setter
-    def database_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "database_name", value)
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-    @schema_name.setter
-    def schema_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "schema_name", value)
-
-
-@pulumi.input_type
 class TableColumnArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  type: pulumi.Input[str],
                  comment: Optional[pulumi.Input[str]] = None,
                  default: Optional[pulumi.Input[str]] = None,
                  nullable: Optional[pulumi.Input[bool]] = None):
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/_utilities.py` & `pulumi_materialize-0.3.0/pulumi_materialize/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/app_password.py` & `pulumi_materialize-0.3.0/pulumi_materialize/app_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/cloud_region.py` & `pulumi_materialize-0.3.0/pulumi_materialize/cloud_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/cluster.py` & `pulumi_materialize-0.3.0/pulumi_materialize/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/cluster_replica.py` & `pulumi_materialize-0.3.0/pulumi_materialize/cluster_replica.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/config/vars.py` & `pulumi_materialize-0.3.0/pulumi_materialize/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_aws.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_aws_privatelink.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_confluent_schema_registry.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_confluent_schema_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_kafka.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_mysql.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_postgres.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_postgres.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/connection_ssh_tunnel.py` & `pulumi_materialize-0.3.0/pulumi_materialize/connection_ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/database.py` & `pulumi_materialize-0.3.0/pulumi_materialize/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_cluster_replicas.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_cluster_replicas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_clusters.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_connections.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_current_cluster.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_current_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_current_database.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_current_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_databases.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_egress_ips.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_egress_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_indexes.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_materialized_views.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_materialized_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_roles.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_schemas.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_scim_configs.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_scim_configs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_scim_groups.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_scim_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_secrets.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_sinks.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_sinks.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_sources.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_sources.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_sso_config.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_system_parameters.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_system_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_tables.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_types.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/get_views.py` & `pulumi_materialize-0.3.0/pulumi_materialize/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_cluster_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_cluster_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_connection.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_connection_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_connection_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_database.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_database_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_database_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_materialized_view.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_role.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_schema.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_schema_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_schema_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_secret.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_secret_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_secret_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_source.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_system_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_system_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_table.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_table_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_table_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_type.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_type_default_privilege.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_type_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/grant_view.py` & `pulumi_materialize-0.3.0/pulumi_materialize/grant_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/index.py` & `pulumi_materialize-0.3.0/pulumi_materialize/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/materialized_view.py` & `pulumi_materialize-0.3.0/pulumi_materialize/materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/outputs.py` & `pulumi_materialize-0.3.0/pulumi_materialize/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,41 +108,37 @@
     'SourceKafkaKafkaConnection',
     'SourceKafkaKeyFormat',
     'SourceKafkaKeyFormatAvro',
     'SourceKafkaKeyFormatAvroSchemaRegistryConnection',
     'SourceKafkaKeyFormatCsv',
     'SourceKafkaKeyFormatProtobuf',
     'SourceKafkaKeyFormatProtobufSchemaRegistryConnection',
-    'SourceKafkaSubsource',
     'SourceKafkaValueFormat',
     'SourceKafkaValueFormatAvro',
     'SourceKafkaValueFormatAvroSchemaRegistryConnection',
     'SourceKafkaValueFormatCsv',
     'SourceKafkaValueFormatProtobuf',
     'SourceKafkaValueFormatProtobufSchemaRegistryConnection',
     'SourceLoadgenAuctionOptions',
     'SourceLoadgenCounterOptions',
     'SourceLoadgenExposeProgress',
     'SourceLoadgenKeyValueOptions',
     'SourceLoadgenMarketingOptions',
-    'SourceLoadgenSubsource',
     'SourceLoadgenTpchOptions',
+    'SourceMysqlExposeProgress',
     'SourceMysqlMysqlConnection',
-    'SourceMysqlSubsource',
     'SourceMysqlTable',
     'SourcePostgresExposeProgress',
     'SourcePostgresPostgresConnection',
-    'SourcePostgresSubsource',
     'SourcePostgresTable',
     'SourceWebhookCheckOption',
     'SourceWebhookCheckOptionField',
     'SourceWebhookCheckOptionFieldSecret',
     'SourceWebhookIncludeHeader',
     'SourceWebhookIncludeHeaders',
-    'SourceWebhookSubsource',
     'TableColumn',
     'TypeListProperties',
     'TypeMapProperties',
     'TypeRowProperty',
 ]
 
 @pulumi.output_type
@@ -5359,75 +5355,14 @@
         """
         The identifier for the source schema in Materialize. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
 
 @pulumi.output_type
-class SourceKafkaSubsource(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "databaseName":
-            suggest = "database_name"
-        elif key == "schemaName":
-            suggest = "schema_name"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourceKafkaSubsource. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        SourceKafkaSubsource.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        SourceKafkaSubsource.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 name: str,
-                 database_name: Optional[str] = None,
-                 schema_name: Optional[str] = None):
-        """
-        :param str name: The identifier for the source.
-        :param str database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[str]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[str]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-
-@pulumi.output_type
 class SourceKafkaValueFormat(dict):
     def __init__(__self__, *,
                  avro: Optional['outputs.SourceKafkaValueFormatAvro'] = None,
                  bytes: Optional[bool] = None,
                  csvs: Optional[Sequence['outputs.SourceKafkaValueFormatCsv']] = None,
                  json: Optional[bool] = None,
                  protobuf: Optional['outputs.SourceKafkaValueFormatProtobuf'] = None,
@@ -6113,75 +6048,14 @@
         """
         The interval at which the next datum should be emitted. Defaults to one second.
         """
         return pulumi.get(self, "tick_interval")
 
 
 @pulumi.output_type
-class SourceLoadgenSubsource(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "databaseName":
-            suggest = "database_name"
-        elif key == "schemaName":
-            suggest = "schema_name"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourceLoadgenSubsource. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        SourceLoadgenSubsource.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        SourceLoadgenSubsource.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 name: str,
-                 database_name: Optional[str] = None,
-                 schema_name: Optional[str] = None):
-        """
-        :param str name: The identifier for the source.
-        :param str database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[str]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[str]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-
-@pulumi.output_type
 class SourceLoadgenTpchOptions(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "scaleFactor":
             suggest = "scale_factor"
         elif key == "tickInterval":
@@ -6224,163 +6098,222 @@
         """
         The interval at which the next datum should be emitted. Defaults to one second.
         """
         return pulumi.get(self, "tick_interval")
 
 
 @pulumi.output_type
-class SourceMysqlMysqlConnection(dict):
+class SourceMysqlExposeProgress(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "databaseName":
             suggest = "database_name"
         elif key == "schemaName":
             suggest = "schema_name"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourceMysqlMysqlConnection. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in SourceMysqlExposeProgress. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        SourceMysqlMysqlConnection.__key_warning(key)
+        SourceMysqlExposeProgress.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        SourceMysqlMysqlConnection.__key_warning(key)
+        SourceMysqlExposeProgress.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  database_name: Optional[str] = None,
                  schema_name: Optional[str] = None):
         """
-        :param str name: The mysql_connection name.
-        :param str database_name: The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The mysql_connection schema name. Defaults to `public`.
+        :param str name: The expose_progress name.
+        :param str database_name: The expose_progress database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param str schema_name: The expose_progress schema name. Defaults to `public`.
         """
         pulumi.set(__self__, "name", name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        The mysql_connection name.
+        The expose_progress name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[str]:
         """
-        The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The expose_progress database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[str]:
         """
-        The mysql_connection schema name. Defaults to `public`.
+        The expose_progress schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
 
 @pulumi.output_type
-class SourceMysqlSubsource(dict):
+class SourceMysqlMysqlConnection(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "databaseName":
             suggest = "database_name"
         elif key == "schemaName":
             suggest = "schema_name"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourceMysqlSubsource. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in SourceMysqlMysqlConnection. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        SourceMysqlSubsource.__key_warning(key)
+        SourceMysqlMysqlConnection.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        SourceMysqlSubsource.__key_warning(key)
+        SourceMysqlMysqlConnection.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  database_name: Optional[str] = None,
                  schema_name: Optional[str] = None):
         """
-        :param str name: The identifier for the source.
-        :param str database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
+        :param str name: The mysql_connection name.
+        :param str database_name: The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param str schema_name: The mysql_connection schema name. Defaults to `public`.
         """
         pulumi.set(__self__, "name", name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        The identifier for the source.
+        The mysql_connection name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[str]:
         """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The mysql_connection database name. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter(name="schemaName")
     def schema_name(self) -> Optional[str]:
         """
-        The identifier for the source schema in Materialize. Defaults to `public`.
+        The mysql_connection schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
 
 @pulumi.output_type
 class SourceMysqlTable(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "upstreamName":
+            suggest = "upstream_name"
+        elif key == "databaseName":
+            suggest = "database_name"
+        elif key == "schemaName":
+            suggest = "schema_name"
+        elif key == "upstreamSchemaName":
+            suggest = "upstream_schema_name"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SourceMysqlTable. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SourceMysqlTable.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SourceMysqlTable.__key_warning(key)
+        return super().get(key, default)
+
     def __init__(__self__, *,
-                 name: str,
-                 alias: Optional[str] = None):
+                 upstream_name: str,
+                 database_name: Optional[str] = None,
+                 name: Optional[str] = None,
+                 schema_name: Optional[str] = None,
+                 upstream_schema_name: Optional[str] = None):
         """
-        :param str name: The name of the table.
-        :param str alias: An alias for the table, used in Materialize.
+        :param str upstream_name: The name of the table in the upstream MySQL database.
+        :param str database_name: The database of the table in Materialize.
+        :param str name: The name for the table, used in Materialize.
+        :param str schema_name: The schema of the table in Materialize.
+        :param str upstream_schema_name: The schema of the table in the upstream MySQL database.
         """
-        pulumi.set(__self__, "name", name)
-        if alias is not None:
-            pulumi.set(__self__, "alias", alias)
+        pulumi.set(__self__, "upstream_name", upstream_name)
+        if database_name is not None:
+            pulumi.set(__self__, "database_name", database_name)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if schema_name is not None:
+            pulumi.set(__self__, "schema_name", schema_name)
+        if upstream_schema_name is not None:
+            pulumi.set(__self__, "upstream_schema_name", upstream_schema_name)
+
+    @property
+    @pulumi.getter(name="upstreamName")
+    def upstream_name(self) -> str:
+        """
+        The name of the table in the upstream MySQL database.
+        """
+        return pulumi.get(self, "upstream_name")
+
+    @property
+    @pulumi.getter(name="databaseName")
+    def database_name(self) -> Optional[str]:
+        """
+        The database of the table in Materialize.
+        """
+        return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def name(self) -> Optional[str]:
         """
-        The name of the table.
+        The name for the table, used in Materialize.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def alias(self) -> Optional[str]:
+    @pulumi.getter(name="schemaName")
+    def schema_name(self) -> Optional[str]:
         """
-        An alias for the table, used in Materialize.
+        The schema of the table in Materialize.
         """
-        return pulumi.get(self, "alias")
+        return pulumi.get(self, "schema_name")
+
+    @property
+    @pulumi.getter(name="upstreamSchemaName")
+    def upstream_schema_name(self) -> Optional[str]:
+        """
+        The schema of the table in the upstream MySQL database.
+        """
+        return pulumi.get(self, "upstream_schema_name")
 
 
 @pulumi.output_type
 class SourcePostgresExposeProgress(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -6498,102 +6431,100 @@
         """
         The postgres_connection schema name. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
 
 @pulumi.output_type
-class SourcePostgresSubsource(dict):
+class SourcePostgresTable(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "databaseName":
+        if key == "upstreamName":
+            suggest = "upstream_name"
+        elif key == "databaseName":
             suggest = "database_name"
         elif key == "schemaName":
             suggest = "schema_name"
+        elif key == "upstreamSchemaName":
+            suggest = "upstream_schema_name"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourcePostgresSubsource. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in SourcePostgresTable. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        SourcePostgresSubsource.__key_warning(key)
+        SourcePostgresTable.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        SourcePostgresSubsource.__key_warning(key)
+        SourcePostgresTable.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 name: str,
+                 upstream_name: str,
                  database_name: Optional[str] = None,
-                 schema_name: Optional[str] = None):
+                 name: Optional[str] = None,
+                 schema_name: Optional[str] = None,
+                 upstream_schema_name: Optional[str] = None):
         """
-        :param str name: The identifier for the source.
-        :param str database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
+        :param str upstream_name: The name of the table in the upstream Postgres database.
+        :param str database_name: The database of the table in Materialize.
+        :param str name: The name of the table in Materialize.
+        :param str schema_name: The schema of the table in Materialize.
+        :param str upstream_schema_name: The schema of the table in the upstream Postgres database.
         """
-        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "upstream_name", upstream_name)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
+        if upstream_schema_name is not None:
+            pulumi.set(__self__, "upstream_schema_name", upstream_schema_name)
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
+    @pulumi.getter(name="upstreamName")
+    def upstream_name(self) -> str:
         """
-        The identifier for the source.
+        The name of the table in the upstream Postgres database.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "upstream_name")
 
     @property
     @pulumi.getter(name="databaseName")
     def database_name(self) -> Optional[str]:
         """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        The database of the table in Materialize.
         """
         return pulumi.get(self, "database_name")
 
     @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[str]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-
-@pulumi.output_type
-class SourcePostgresTable(dict):
-    def __init__(__self__, *,
-                 name: str,
-                 alias: Optional[str] = None):
+    @pulumi.getter
+    def name(self) -> Optional[str]:
         """
-        :param str name: The name of the table.
-        :param str alias: The alias of the table.
+        The name of the table in Materialize.
         """
-        pulumi.set(__self__, "name", name)
-        if alias is not None:
-            pulumi.set(__self__, "alias", alias)
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
+    @pulumi.getter(name="schemaName")
+    def schema_name(self) -> Optional[str]:
         """
-        The name of the table.
+        The schema of the table in Materialize.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "schema_name")
 
     @property
-    @pulumi.getter
-    def alias(self) -> Optional[str]:
+    @pulumi.getter(name="upstreamSchemaName")
+    def upstream_schema_name(self) -> Optional[str]:
         """
-        The alias of the table.
+        The schema of the table in the upstream Postgres database.
         """
-        return pulumi.get(self, "alias")
+        return pulumi.get(self, "upstream_schema_name")
 
 
 @pulumi.output_type
 class SourceWebhookCheckOption(dict):
     def __init__(__self__, *,
                  field: 'outputs.SourceWebhookCheckOptionField',
                  alias: Optional[str] = None,
@@ -6806,75 +6737,14 @@
         """
         Headers that should be included.
         """
         return pulumi.get(self, "onlies")
 
 
 @pulumi.output_type
-class SourceWebhookSubsource(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "databaseName":
-            suggest = "database_name"
-        elif key == "schemaName":
-            suggest = "schema_name"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in SourceWebhookSubsource. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        SourceWebhookSubsource.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        SourceWebhookSubsource.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 name: str,
-                 database_name: Optional[str] = None,
-                 schema_name: Optional[str] = None):
-        """
-        :param str name: The identifier for the source.
-        :param str database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param str schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        pulumi.set(__self__, "name", name)
-        if database_name is not None:
-            pulumi.set(__self__, "database_name", database_name)
-        if schema_name is not None:
-            pulumi.set(__self__, "schema_name", schema_name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        """
-        The identifier for the source.
-        """
-        return pulumi.get(self, "name")
-
-    @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> Optional[str]:
-        """
-        The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        """
-        return pulumi.get(self, "database_name")
-
-    @property
-    @pulumi.getter(name="schemaName")
-    def schema_name(self) -> Optional[str]:
-        """
-        The identifier for the source schema in Materialize. Defaults to `public`.
-        """
-        return pulumi.get(self, "schema_name")
-
-
-@pulumi.output_type
 class TableColumn(dict):
     def __init__(__self__, *,
                  name: str,
                  type: str,
                  comment: Optional[str] = None,
                  default: Optional[str] = None,
                  nullable: Optional[bool] = None):
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/provider.py` & `pulumi_materialize-0.3.0/pulumi_materialize/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/region.py` & `pulumi_materialize-0.3.0/pulumi_materialize/region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/role.py` & `pulumi_materialize-0.3.0/pulumi_materialize/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/role_parameter.py` & `pulumi_materialize-0.3.0/pulumi_materialize/role_parameter.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/schema.py` & `pulumi_materialize-0.3.0/pulumi_materialize/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/scim2_configuration.py` & `pulumi_materialize-0.3.0/pulumi_materialize/scim2_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group.py` & `pulumi_materialize-0.3.0/pulumi_materialize/scim2_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_roles.py` & `pulumi_materialize-0.3.0/pulumi_materialize/scim2_group_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/scim2_group_users.py` & `pulumi_materialize-0.3.0/pulumi_materialize/scim2_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/secret.py` & `pulumi_materialize-0.3.0/pulumi_materialize/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/sink_kafka.py` & `pulumi_materialize-0.3.0/pulumi_materialize/sink_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/source_kafka.py` & `pulumi_materialize-0.3.0/pulumi_materialize/source_kafka.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         The set of arguments for constructing a SourceKafka resource.
         :param pulumi.Input['SourceKafkaKafkaConnectionArgs'] kafka_connection: The Kafka connection to use in the source.
         :param pulumi.Input[str] topic: The Kafka topic you want to subscribe to.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input['SourceKafkaEnvelopeArgs'] envelope: How Materialize should interpret records (e.g. append-only, upsert)..
-        :param pulumi.Input['SourceKafkaExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourceKafkaExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input['SourceKafkaFormatArgs'] format: How to decode raw bytes from different formats into data structures Materialize can understand at runtime.
         :param pulumi.Input[bool] include_headers: Include message headers.
         :param pulumi.Input[str] include_headers_alias: Provide an alias for the headers column.
         :param pulumi.Input[bool] include_key: Include a column containing the Kafka message key.
         :param pulumi.Input[str] include_key_alias: Provide an alias for the key column.
         :param pulumi.Input[bool] include_offset: Include an offset column containing the Kafka message offset.
         :param pulumi.Input[str] include_offset_alias: Provide an alias for the offset column.
@@ -194,15 +194,15 @@
     def envelope(self, value: Optional[pulumi.Input['SourceKafkaEnvelopeArgs']]):
         pulumi.set(self, "envelope", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourceKafkaExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceKafkaExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -460,24 +460,23 @@
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  start_offsets: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  start_timestamp: Optional[pulumi.Input[int]] = None,
-                 subsources: Optional[pulumi.Input[Sequence[pulumi.Input['SourceKafkaSubsourceArgs']]]] = None,
                  topic: Optional[pulumi.Input[str]] = None,
                  value_format: Optional[pulumi.Input['SourceKafkaValueFormatArgs']] = None):
         """
         Input properties used for looking up and filtering SourceKafka resources.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input['SourceKafkaEnvelopeArgs'] envelope: How Materialize should interpret records (e.g. append-only, upsert)..
-        :param pulumi.Input['SourceKafkaExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourceKafkaExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input['SourceKafkaFormatArgs'] format: How to decode raw bytes from different formats into data structures Materialize can understand at runtime.
         :param pulumi.Input[bool] include_headers: Include message headers.
         :param pulumi.Input[str] include_headers_alias: Provide an alias for the headers column.
         :param pulumi.Input[bool] include_key: Include a column containing the Kafka message key.
         :param pulumi.Input[str] include_key_alias: Provide an alias for the key column.
         :param pulumi.Input[bool] include_offset: Include an offset column containing the Kafka message offset.
         :param pulumi.Input[str] include_offset_alias: Provide an alias for the offset column.
@@ -491,15 +490,14 @@
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] start_offsets: Read partitions from the specified offset.
         :param pulumi.Input[int] start_timestamp: Use the specified value to set `START OFFSET` based on the Kafka timestamp.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceKafkaSubsourceArgs']]] subsources: Subsources of a source.
         :param pulumi.Input[str] topic: The Kafka topic you want to subscribe to.
         :param pulumi.Input['SourceKafkaValueFormatArgs'] value_format: Set the value format explicitly.
         """
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
@@ -547,16 +545,14 @@
             pulumi.set(__self__, "schema_name", schema_name)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if start_offsets is not None:
             pulumi.set(__self__, "start_offsets", start_offsets)
         if start_timestamp is not None:
             pulumi.set(__self__, "start_timestamp", start_timestamp)
-        if subsources is not None:
-            pulumi.set(__self__, "subsources", subsources)
         if topic is not None:
             pulumi.set(__self__, "topic", topic)
         if value_format is not None:
             pulumi.set(__self__, "value_format", value_format)
 
     @property
     @pulumi.getter(name="clusterName")
@@ -606,15 +602,15 @@
     def envelope(self, value: Optional[pulumi.Input['SourceKafkaEnvelopeArgs']]):
         pulumi.set(self, "envelope", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourceKafkaExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceKafkaExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -868,26 +864,14 @@
 
     @start_timestamp.setter
     def start_timestamp(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_timestamp", value)
 
     @property
     @pulumi.getter
-    def subsources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceKafkaSubsourceArgs']]]]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @subsources.setter
-    def subsources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceKafkaSubsourceArgs']]]]):
-        pulumi.set(self, "subsources", value)
-
-    @property
-    @pulumi.getter
     def topic(self) -> Optional[pulumi.Input[str]]:
         """
         The Kafka topic you want to subscribe to.
         """
         return pulumi.get(self, "topic")
 
     @topic.setter
@@ -982,15 +966,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[pulumi.InputType['SourceKafkaEnvelopeArgs']] envelope: How Materialize should interpret records (e.g. append-only, upsert)..
-        :param pulumi.Input[pulumi.InputType['SourceKafkaExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourceKafkaExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[pulumi.InputType['SourceKafkaFormatArgs']] format: How to decode raw bytes from different formats into data structures Materialize can understand at runtime.
         :param pulumi.Input[bool] include_headers: Include message headers.
         :param pulumi.Input[str] include_headers_alias: Provide an alias for the headers column.
         :param pulumi.Input[bool] include_key: Include a column containing the Kafka message key.
         :param pulumi.Input[str] include_key_alias: Provide an alias for the key column.
         :param pulumi.Input[bool] include_offset: Include an offset column containing the Kafka message offset.
         :param pulumi.Input[str] include_offset_alias: Provide an alias for the offset column.
@@ -1134,15 +1118,14 @@
             __props__.__dict__["start_timestamp"] = start_timestamp
             if topic is None and not opts.urn:
                 raise TypeError("Missing required property 'topic'")
             __props__.__dict__["topic"] = topic
             __props__.__dict__["value_format"] = value_format
             __props__.__dict__["qualified_sql_name"] = None
             __props__.__dict__["size"] = None
-            __props__.__dict__["subsources"] = None
         super(SourceKafka, __self__).__init__(
             'materialize:index/sourceKafka:SourceKafka',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -1171,29 +1154,28 @@
             ownership_role: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
             start_offsets: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             start_timestamp: Optional[pulumi.Input[int]] = None,
-            subsources: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceKafkaSubsourceArgs']]]]] = None,
             topic: Optional[pulumi.Input[str]] = None,
             value_format: Optional[pulumi.Input[pulumi.InputType['SourceKafkaValueFormatArgs']]] = None) -> 'SourceKafka':
         """
         Get an existing SourceKafka resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[pulumi.InputType['SourceKafkaEnvelopeArgs']] envelope: How Materialize should interpret records (e.g. append-only, upsert)..
-        :param pulumi.Input[pulumi.InputType['SourceKafkaExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourceKafkaExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[pulumi.InputType['SourceKafkaFormatArgs']] format: How to decode raw bytes from different formats into data structures Materialize can understand at runtime.
         :param pulumi.Input[bool] include_headers: Include message headers.
         :param pulumi.Input[str] include_headers_alias: Provide an alias for the headers column.
         :param pulumi.Input[bool] include_key: Include a column containing the Kafka message key.
         :param pulumi.Input[str] include_key_alias: Provide an alias for the key column.
         :param pulumi.Input[bool] include_offset: Include an offset column containing the Kafka message offset.
         :param pulumi.Input[str] include_offset_alias: Provide an alias for the offset column.
@@ -1207,15 +1189,14 @@
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] start_offsets: Read partitions from the specified offset.
         :param pulumi.Input[int] start_timestamp: Use the specified value to set `START OFFSET` based on the Kafka timestamp.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceKafkaSubsourceArgs']]]] subsources: Subsources of a source.
         :param pulumi.Input[str] topic: The Kafka topic you want to subscribe to.
         :param pulumi.Input[pulumi.InputType['SourceKafkaValueFormatArgs']] value_format: Set the value format explicitly.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SourceKafkaState.__new__(_SourceKafkaState)
 
@@ -1241,15 +1222,14 @@
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["size"] = size
         __props__.__dict__["start_offsets"] = start_offsets
         __props__.__dict__["start_timestamp"] = start_timestamp
-        __props__.__dict__["subsources"] = subsources
         __props__.__dict__["topic"] = topic
         __props__.__dict__["value_format"] = value_format
         return SourceKafka(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Output[str]:
@@ -1282,15 +1262,15 @@
         """
         return pulumi.get(self, "envelope")
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> pulumi.Output[Optional['outputs.SourceKafkaExposeProgress']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @property
     @pulumi.getter
     def format(self) -> pulumi.Output[Optional['outputs.SourceKafkaFormat']]:
         """
@@ -1456,22 +1436,14 @@
         """
         Use the specified value to set `START OFFSET` based on the Kafka timestamp.
         """
         return pulumi.get(self, "start_timestamp")
 
     @property
     @pulumi.getter
-    def subsources(self) -> pulumi.Output[Sequence['outputs.SourceKafkaSubsource']]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @property
-    @pulumi.getter
     def topic(self) -> pulumi.Output[str]:
         """
         The Kafka topic you want to subscribe to.
         """
         return pulumi.get(self, "topic")
 
     @property
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/source_loadgen.py` & `pulumi_materialize-0.3.0/pulumi_materialize/source_loadgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         The set of arguments for constructing a SourceLoadgen resource.
         :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input['SourceLoadgenAuctionOptionsArgs'] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input['SourceLoadgenCounterOptionsArgs'] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input['SourceLoadgenKeyValueOptionsArgs'] key_value_options: KEY VALUE Load Generator Options.
         :param pulumi.Input['SourceLoadgenMarketingOptionsArgs'] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input['SourceLoadgenTpchOptionsArgs'] tpch_options: TPCH Options.
@@ -147,15 +147,15 @@
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -258,34 +258,32 @@
                  marketing_options: Optional[pulumi.Input['SourceLoadgenMarketingOptionsArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
-                 subsources: Optional[pulumi.Input[Sequence[pulumi.Input['SourceLoadgenSubsourceArgs']]]] = None,
                  tpch_options: Optional[pulumi.Input['SourceLoadgenTpchOptionsArgs']] = None):
         """
         Input properties used for looking up and filtering SourceLoadgen resources.
         :param pulumi.Input['SourceLoadgenAuctionOptionsArgs'] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input['SourceLoadgenCounterOptionsArgs'] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourceLoadgenExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input['SourceLoadgenKeyValueOptionsArgs'] key_value_options: KEY VALUE Load Generator Options.
         :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input['SourceLoadgenMarketingOptionsArgs'] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceLoadgenSubsourceArgs']]] subsources: Subsources of a source.
         :param pulumi.Input['SourceLoadgenTpchOptionsArgs'] tpch_options: TPCH Options.
         """
         if auction_options is not None:
             pulumi.set(__self__, "auction_options", auction_options)
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
@@ -310,16 +308,14 @@
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
         if size is not None:
             pulumi.set(__self__, "size", size)
-        if subsources is not None:
-            pulumi.set(__self__, "subsources", subsources)
         if tpch_options is not None:
             pulumi.set(__self__, "tpch_options", tpch_options)
 
     @property
     @pulumi.getter(name="auctionOptions")
     def auction_options(self) -> Optional[pulumi.Input['SourceLoadgenAuctionOptionsArgs']]:
         """
@@ -379,15 +375,15 @@
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourceLoadgenExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -496,26 +492,14 @@
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size", value)
 
     @property
-    @pulumi.getter
-    def subsources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceLoadgenSubsourceArgs']]]]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @subsources.setter
-    def subsources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceLoadgenSubsourceArgs']]]]):
-        pulumi.set(self, "subsources", value)
-
-    @property
     @pulumi.getter(name="tpchOptions")
     def tpch_options(self) -> Optional[pulumi.Input['SourceLoadgenTpchOptionsArgs']]:
         """
         TPCH Options.
         """
         return pulumi.get(self, "tpch_options")
 
@@ -575,15 +559,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']] key_value_options: KEY VALUE Load Generator Options.
         :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
@@ -675,15 +659,14 @@
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
             __props__.__dict__["tpch_options"] = tpch_options
             __props__.__dict__["qualified_sql_name"] = None
             __props__.__dict__["size"] = None
-            __props__.__dict__["subsources"] = None
         super(SourceLoadgen, __self__).__init__(
             'materialize:index/sourceLoadgen:SourceLoadgen',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -701,39 +684,37 @@
             marketing_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
-            subsources: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceLoadgenSubsourceArgs']]]]] = None,
             tpch_options: Optional[pulumi.Input[pulumi.InputType['SourceLoadgenTpchOptionsArgs']]] = None) -> 'SourceLoadgen':
         """
         Get an existing SourceLoadgen resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenAuctionOptionsArgs']] auction_options: Auction Options.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenCounterOptionsArgs']] counter_options: Counter Options.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourceLoadgenExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenKeyValueOptionsArgs']] key_value_options: KEY VALUE Load Generator Options.
         :param pulumi.Input[str] load_generator_type: The load generator types: [AUCTION MARKETING COUNTER TPCH KEY VALUE].
         :param pulumi.Input[pulumi.InputType['SourceLoadgenMarketingOptionsArgs']] marketing_options: Marketing Options.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceLoadgenSubsourceArgs']]]] subsources: Subsources of a source.
         :param pulumi.Input[pulumi.InputType['SourceLoadgenTpchOptionsArgs']] tpch_options: TPCH Options.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SourceLoadgenState.__new__(_SourceLoadgenState)
 
         __props__.__dict__["auction_options"] = auction_options
@@ -747,15 +728,14 @@
         __props__.__dict__["marketing_options"] = marketing_options
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["size"] = size
-        __props__.__dict__["subsources"] = subsources
         __props__.__dict__["tpch_options"] = tpch_options
         return SourceLoadgen(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="auctionOptions")
     def auction_options(self) -> pulumi.Output[Optional['outputs.SourceLoadgenAuctionOptions']]:
         """
@@ -795,15 +775,15 @@
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> pulumi.Output[Optional['outputs.SourceLoadgenExposeProgress']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @property
     @pulumi.getter(name="keyValueOptions")
     def key_value_options(self) -> pulumi.Output[Optional['outputs.SourceLoadgenKeyValueOptions']]:
         """
@@ -872,22 +852,14 @@
     def size(self) -> pulumi.Output[str]:
         """
         The size of the cluster maintaining this source.
         """
         return pulumi.get(self, "size")
 
     @property
-    @pulumi.getter
-    def subsources(self) -> pulumi.Output[Sequence['outputs.SourceLoadgenSubsource']]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @property
     @pulumi.getter(name="tpchOptions")
     def tpch_options(self) -> pulumi.Output[Optional['outputs.SourceLoadgenTpchOptions']]:
         """
         TPCH Options.
         """
         return pulumi.get(self, "tpch_options")
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/source_mysql.py` & `pulumi_materialize-0.3.0/pulumi_materialize/source_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,42 +16,46 @@
 @pulumi.input_type
 class SourceMysqlArgs:
     def __init__(__self__, *,
                  mysql_connection: pulumi.Input['SourceMysqlMysqlConnectionArgs'],
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 expose_progress: Optional[pulumi.Input['SourceMysqlExposeProgressArgs']] = None,
                  ignore_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SourceMysql resource.
         :param pulumi.Input['SourceMysqlMysqlConnectionArgs'] mysql_connection: The MySQL connection to use in the source.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input['SourceMysqlExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_columns: Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]] tables: Specifies the tables to be included in the source. If not specified, all tables are included.
+        :param pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]] tables: Specify the tables to be included in the source. If not specified, all tables are included.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain MySQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         pulumi.set(__self__, "mysql_connection", mysql_connection)
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
+        if expose_progress is not None:
+            pulumi.set(__self__, "expose_progress", expose_progress)
         if ignore_columns is not None:
             pulumi.set(__self__, "ignore_columns", ignore_columns)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
@@ -108,14 +112,26 @@
         return pulumi.get(self, "database_name")
 
     @database_name.setter
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
+    @pulumi.getter(name="exposeProgress")
+    def expose_progress(self) -> Optional[pulumi.Input['SourceMysqlExposeProgressArgs']]:
+        """
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
+        """
+        return pulumi.get(self, "expose_progress")
+
+    @expose_progress.setter
+    def expose_progress(self, value: Optional[pulumi.Input['SourceMysqlExposeProgressArgs']]):
+        pulumi.set(self, "expose_progress", value)
+
+    @property
     @pulumi.getter(name="ignoreColumns")
     def ignore_columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         return pulumi.get(self, "ignore_columns")
 
@@ -171,15 +187,15 @@
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
     @property
     @pulumi.getter
     def tables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]]:
         """
-        Specifies the tables to be included in the source. If not specified, all tables are included.
+        Specify the tables to be included in the source. If not specified, all tables are included.
         """
         return pulumi.get(self, "tables")
 
     @tables.setter
     def tables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]]):
         pulumi.set(self, "tables", value)
 
@@ -198,48 +214,50 @@
 
 @pulumi.input_type
 class _SourceMysqlState:
     def __init__(__self__, *,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 expose_progress: Optional[pulumi.Input['SourceMysqlExposeProgressArgs']] = None,
                  ignore_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mysql_connection: Optional[pulumi.Input['SourceMysqlMysqlConnectionArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
-                 subsources: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlSubsourceArgs']]]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering SourceMysql resources.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input['SourceMysqlExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_columns: Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         :param pulumi.Input['SourceMysqlMysqlConnectionArgs'] mysql_connection: The MySQL connection to use in the source.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceMysqlSubsourceArgs']]] subsources: Subsources of a source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]] tables: Specifies the tables to be included in the source. If not specified, all tables are included.
+        :param pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]] tables: Specify the tables to be included in the source. If not specified, all tables are included.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain MySQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
+        if expose_progress is not None:
+            pulumi.set(__self__, "expose_progress", expose_progress)
         if ignore_columns is not None:
             pulumi.set(__self__, "ignore_columns", ignore_columns)
         if mysql_connection is not None:
             pulumi.set(__self__, "mysql_connection", mysql_connection)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
@@ -248,16 +266,14 @@
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
         if size is not None:
             pulumi.set(__self__, "size", size)
-        if subsources is not None:
-            pulumi.set(__self__, "subsources", subsources)
         if tables is not None:
             pulumi.set(__self__, "tables", tables)
         if text_columns is not None:
             pulumi.set(__self__, "text_columns", text_columns)
 
     @property
     @pulumi.getter(name="clusterName")
@@ -292,14 +308,26 @@
         return pulumi.get(self, "database_name")
 
     @database_name.setter
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
+    @pulumi.getter(name="exposeProgress")
+    def expose_progress(self) -> Optional[pulumi.Input['SourceMysqlExposeProgressArgs']]:
+        """
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
+        """
+        return pulumi.get(self, "expose_progress")
+
+    @expose_progress.setter
+    def expose_progress(self, value: Optional[pulumi.Input['SourceMysqlExposeProgressArgs']]):
+        pulumi.set(self, "expose_progress", value)
+
+    @property
     @pulumi.getter(name="ignoreColumns")
     def ignore_columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         return pulumi.get(self, "ignore_columns")
 
@@ -389,29 +417,17 @@
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
-    def subsources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlSubsourceArgs']]]]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @subsources.setter
-    def subsources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlSubsourceArgs']]]]):
-        pulumi.set(self, "subsources", value)
-
-    @property
-    @pulumi.getter
     def tables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]]:
         """
-        Specifies the tables to be included in the source. If not specified, all tables are included.
+        Specify the tables to be included in the source. If not specified, all tables are included.
         """
         return pulumi.get(self, "tables")
 
     @tables.setter
     def tables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceMysqlTableArgs']]]]):
         pulumi.set(self, "tables", value)
 
@@ -432,51 +448,27 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceMysqlExposeProgressArgs']]] = None,
                  ignore_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mysql_connection: Optional[pulumi.Input[pulumi.InputType['SourceMysqlMysqlConnectionArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         A MySQL source describes a MySQL instance you want Materialize to read data from.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_materialize as materialize
-
-        test = materialize.SourceMysql("test",
-            schema_name=materialize_schema["test"]["name"],
-            database_name=materialize_database["test"]["name"],
-            cluster_name="quickstart",
-            mysql_connection=materialize.SourceMysqlMysqlConnectionArgs(
-                name=materialize_connection_mysql["test"]["name"],
-            ),
-            tables=[
-                materialize.SourceMysqlTableArgs(
-                    name="shop.mysql_table1",
-                    alias="alias_mysql_table1",
-                ),
-                materialize.SourceMysqlTableArgs(
-                    name="shop.mysql_table2",
-                    alias="alias_mysql_table2",
-                ),
-            ])
-        ```
-
         ## Import
 
         Sources can be imported using the source id
 
         ```sh
          $ pulumi import materialize:index/sourceMysql:SourceMysql example_source_mysql <region>:<source_id>
         ```
@@ -484,57 +476,33 @@
          Source id and information be found in the `mz_catalog.mz_sources` table The region is the region where the database is located (e.g. aws/us-east-1)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input[pulumi.InputType['SourceMysqlExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_columns: Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         :param pulumi.Input[pulumi.InputType['SourceMysqlMysqlConnectionArgs']] mysql_connection: The MySQL connection to use in the source.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]] tables: Specifies the tables to be included in the source. If not specified, all tables are included.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]] tables: Specify the tables to be included in the source. If not specified, all tables are included.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain MySQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SourceMysqlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A MySQL source describes a MySQL instance you want Materialize to read data from.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_materialize as materialize
-
-        test = materialize.SourceMysql("test",
-            schema_name=materialize_schema["test"]["name"],
-            database_name=materialize_database["test"]["name"],
-            cluster_name="quickstart",
-            mysql_connection=materialize.SourceMysqlMysqlConnectionArgs(
-                name=materialize_connection_mysql["test"]["name"],
-            ),
-            tables=[
-                materialize.SourceMysqlTableArgs(
-                    name="shop.mysql_table1",
-                    alias="alias_mysql_table1",
-                ),
-                materialize.SourceMysqlTableArgs(
-                    name="shop.mysql_table2",
-                    alias="alias_mysql_table2",
-                ),
-            ])
-        ```
-
         ## Import
 
         Sources can be imported using the source id
 
         ```sh
          $ pulumi import materialize:index/sourceMysql:SourceMysql example_source_mysql <region>:<source_id>
         ```
@@ -555,14 +523,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
+                 expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceMysqlExposeProgressArgs']]] = None,
                  ignore_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  mysql_connection: Optional[pulumi.Input[pulumi.InputType['SourceMysqlMysqlConnectionArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]]] = None,
@@ -575,89 +544,89 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SourceMysqlArgs.__new__(SourceMysqlArgs)
 
             __props__.__dict__["cluster_name"] = cluster_name
             __props__.__dict__["comment"] = comment
             __props__.__dict__["database_name"] = database_name
+            __props__.__dict__["expose_progress"] = expose_progress
             __props__.__dict__["ignore_columns"] = ignore_columns
             if mysql_connection is None and not opts.urn:
                 raise TypeError("Missing required property 'mysql_connection'")
             __props__.__dict__["mysql_connection"] = mysql_connection
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
             __props__.__dict__["tables"] = tables
             __props__.__dict__["text_columns"] = text_columns
             __props__.__dict__["qualified_sql_name"] = None
             __props__.__dict__["size"] = None
-            __props__.__dict__["subsources"] = None
         super(SourceMysql, __self__).__init__(
             'materialize:index/sourceMysql:SourceMysql',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             cluster_name: Optional[pulumi.Input[str]] = None,
             comment: Optional[pulumi.Input[str]] = None,
             database_name: Optional[pulumi.Input[str]] = None,
+            expose_progress: Optional[pulumi.Input[pulumi.InputType['SourceMysqlExposeProgressArgs']]] = None,
             ignore_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             mysql_connection: Optional[pulumi.Input[pulumi.InputType['SourceMysqlMysqlConnectionArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
-            subsources: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlSubsourceArgs']]]]] = None,
             tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]]] = None,
             text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'SourceMysql':
         """
         Get an existing SourceMysql resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
+        :param pulumi.Input[pulumi.InputType['SourceMysqlExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ignore_columns: Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         :param pulumi.Input[pulumi.InputType['SourceMysqlMysqlConnectionArgs']] mysql_connection: The MySQL connection to use in the source.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlSubsourceArgs']]]] subsources: Subsources of a source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]] tables: Specifies the tables to be included in the source. If not specified, all tables are included.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceMysqlTableArgs']]]] tables: Specify the tables to be included in the source. If not specified, all tables are included.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain MySQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SourceMysqlState.__new__(_SourceMysqlState)
 
         __props__.__dict__["cluster_name"] = cluster_name
         __props__.__dict__["comment"] = comment
         __props__.__dict__["database_name"] = database_name
+        __props__.__dict__["expose_progress"] = expose_progress
         __props__.__dict__["ignore_columns"] = ignore_columns
         __props__.__dict__["mysql_connection"] = mysql_connection
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["size"] = size
-        __props__.__dict__["subsources"] = subsources
         __props__.__dict__["tables"] = tables
         __props__.__dict__["text_columns"] = text_columns
         return SourceMysql(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Output[str]:
@@ -679,14 +648,22 @@
     def database_name(self) -> pulumi.Output[Optional[str]]:
         """
         The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         """
         return pulumi.get(self, "database_name")
 
     @property
+    @pulumi.getter(name="exposeProgress")
+    def expose_progress(self) -> pulumi.Output[Optional['outputs.SourceMysqlExposeProgress']]:
+        """
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
+        """
+        return pulumi.get(self, "expose_progress")
+
+    @property
     @pulumi.getter(name="ignoreColumns")
     def ignore_columns(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         Ignore specific columns when reading data from MySQL. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         return pulumi.get(self, "ignore_columns")
 
@@ -744,25 +721,17 @@
         """
         The size of the cluster maintaining this source.
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def subsources(self) -> pulumi.Output[Sequence['outputs.SourceMysqlSubsource']]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @property
-    @pulumi.getter
     def tables(self) -> pulumi.Output[Optional[Sequence['outputs.SourceMysqlTable']]]:
         """
-        Specifies the tables to be included in the source. If not specified, all tables are included.
+        Specify the tables to be included in the source. If not specified, all tables are included.
         """
         return pulumi.get(self, "tables")
 
     @property
     @pulumi.getter(name="textColumns")
     def text_columns(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/source_postgres.py` & `pulumi_materialize-0.3.0/pulumi_materialize/source_postgres.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,43 +14,42 @@
 __all__ = ['SourcePostgresArgs', 'SourcePostgres']
 
 @pulumi.input_type
 class SourcePostgresArgs:
     def __init__(__self__, *,
                  postgres_connection: pulumi.Input['SourcePostgresPostgresConnectionArgs'],
                  publication: pulumi.Input[str],
+                 tables: pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]],
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  expose_progress: Optional[pulumi.Input['SourcePostgresExposeProgressArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 schemas: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 tables: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a SourcePostgres resource.
         :param pulumi.Input['SourcePostgresPostgresConnectionArgs'] postgres_connection: The PostgreSQL connection to use in the source.
         :param pulumi.Input[str] publication: The PostgreSQL publication (the replication data set containing the tables to be streamed to Materialize).
+        :param pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]] tables: Creates subsources for specific tables in the Postgres connection.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input['SourcePostgresExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourcePostgresExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] schemas: Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
-        :param pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]] tables: Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain PostgreSQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         pulumi.set(__self__, "postgres_connection", postgres_connection)
         pulumi.set(__self__, "publication", publication)
+        pulumi.set(__self__, "tables", tables)
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if expose_progress is not None:
@@ -59,18 +58,14 @@
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
-        if schemas is not None:
-            pulumi.set(__self__, "schemas", schemas)
-        if tables is not None:
-            pulumi.set(__self__, "tables", tables)
         if text_columns is not None:
             pulumi.set(__self__, "text_columns", text_columns)
 
     @property
     @pulumi.getter(name="postgresConnection")
     def postgres_connection(self) -> pulumi.Input['SourcePostgresPostgresConnectionArgs']:
         """
@@ -91,14 +86,26 @@
         return pulumi.get(self, "publication")
 
     @publication.setter
     def publication(self, value: pulumi.Input[str]):
         pulumi.set(self, "publication", value)
 
     @property
+    @pulumi.getter
+    def tables(self) -> pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]:
+        """
+        Creates subsources for specific tables in the Postgres connection.
+        """
+        return pulumi.get(self, "tables")
+
+    @tables.setter
+    def tables(self, value: pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]):
+        pulumi.set(self, "tables", value)
+
+    @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> Optional[pulumi.Input[str]]:
         """
         The cluster to maintain this source.
         """
         return pulumi.get(self, "cluster_name")
 
@@ -130,15 +137,15 @@
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourcePostgresExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourcePostgresExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -187,38 +194,14 @@
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
     @property
-    @pulumi.getter
-    def schemas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
-        """
-        return pulumi.get(self, "schemas")
-
-    @schemas.setter
-    def schemas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "schemas", value)
-
-    @property
-    @pulumi.getter
-    def tables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]]:
-        """
-        Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
-        """
-        return pulumi.get(self, "tables")
-
-    @tables.setter
-    def tables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]]):
-        pulumi.set(self, "tables", value)
-
-    @property
     @pulumi.getter(name="textColumns")
     def text_columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Decode data as text for specific columns that contain PostgreSQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         return pulumi.get(self, "text_columns")
 
@@ -237,36 +220,32 @@
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  postgres_connection: Optional[pulumi.Input['SourcePostgresPostgresConnectionArgs']] = None,
                  publication: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 schemas: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  size: Optional[pulumi.Input[str]] = None,
-                 subsources: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresSubsourceArgs']]]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering SourcePostgres resources.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input['SourcePostgresExposeProgressArgs'] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input['SourcePostgresExposeProgressArgs'] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input['SourcePostgresPostgresConnectionArgs'] postgres_connection: The PostgreSQL connection to use in the source.
         :param pulumi.Input[str] publication: The PostgreSQL publication (the replication data set containing the tables to be streamed to Materialize).
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] schemas: Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourcePostgresSubsourceArgs']]] subsources: Subsources of a source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]] tables: Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
+        :param pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]] tables: Creates subsources for specific tables in the Postgres connection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain PostgreSQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
@@ -283,20 +262,16 @@
             pulumi.set(__self__, "publication", publication)
         if qualified_sql_name is not None:
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
-        if schemas is not None:
-            pulumi.set(__self__, "schemas", schemas)
         if size is not None:
             pulumi.set(__self__, "size", size)
-        if subsources is not None:
-            pulumi.set(__self__, "subsources", subsources)
         if tables is not None:
             pulumi.set(__self__, "tables", tables)
         if text_columns is not None:
             pulumi.set(__self__, "text_columns", text_columns)
 
     @property
     @pulumi.getter(name="clusterName")
@@ -334,15 +309,15 @@
     def database_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "database_name", value)
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> Optional[pulumi.Input['SourcePostgresExposeProgressArgs']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @expose_progress.setter
     def expose_progress(self, value: Optional[pulumi.Input['SourcePostgresExposeProgressArgs']]):
         pulumi.set(self, "expose_progress", value)
 
@@ -428,53 +403,29 @@
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
     @property
     @pulumi.getter
-    def schemas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
-        """
-        return pulumi.get(self, "schemas")
-
-    @schemas.setter
-    def schemas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "schemas", value)
-
-    @property
-    @pulumi.getter
     def size(self) -> Optional[pulumi.Input[str]]:
         """
         The size of the cluster maintaining this source.
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter
-    def subsources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresSubsourceArgs']]]]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @subsources.setter
-    def subsources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresSubsourceArgs']]]]):
-        pulumi.set(self, "subsources", value)
-
-    @property
-    @pulumi.getter
     def tables(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]]:
         """
-        Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
+        Creates subsources for specific tables in the Postgres connection.
         """
         return pulumi.get(self, "tables")
 
     @tables.setter
     def tables(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourcePostgresTableArgs']]]]):
         pulumi.set(self, "tables", value)
 
@@ -502,46 +453,20 @@
                  expose_progress: Optional[pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  postgres_connection: Optional[pulumi.Input[pulumi.InputType['SourcePostgresPostgresConnectionArgs']]] = None,
                  publication: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 schemas: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         A Postgres source describes a PostgreSQL instance you want Materialize to read data from.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_materialize as materialize
-
-        example_source_postgres = materialize.SourcePostgres("exampleSourcePostgres",
-            cluster_name="quickstart",
-            postgres_connection=materialize.SourcePostgresPostgresConnectionArgs(
-                name="pg_connection",
-            ),
-            publication="mz_source",
-            schema_name="schema",
-            tables=[
-                materialize.SourcePostgresTableArgs(
-                    alias="s1_table_1",
-                    name="schema1.table_1",
-                ),
-                materialize.SourcePostgresTableArgs(
-                    alias="s2_table_1",
-                    name="schema2.table_1",
-                ),
-            ])
-        ```
-
         ## Import
 
         Sources can be imported using the source id
 
         ```sh
          $ pulumi import materialize:index/sourcePostgres:SourcePostgres example_source_postgres <region>:<source_id>
         ```
@@ -549,59 +474,33 @@
          Source id and information be found in the `mz_catalog.mz_sources` table The region is the region where the database is located (e.g. aws/us-east-1)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[pulumi.InputType['SourcePostgresPostgresConnectionArgs']] postgres_connection: The PostgreSQL connection to use in the source.
         :param pulumi.Input[str] publication: The PostgreSQL publication (the replication data set containing the tables to be streamed to Materialize).
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] schemas: Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]] tables: Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]] tables: Creates subsources for specific tables in the Postgres connection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain PostgreSQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: SourcePostgresArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A Postgres source describes a PostgreSQL instance you want Materialize to read data from.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_materialize as materialize
-
-        example_source_postgres = materialize.SourcePostgres("exampleSourcePostgres",
-            cluster_name="quickstart",
-            postgres_connection=materialize.SourcePostgresPostgresConnectionArgs(
-                name="pg_connection",
-            ),
-            publication="mz_source",
-            schema_name="schema",
-            tables=[
-                materialize.SourcePostgresTableArgs(
-                    alias="s1_table_1",
-                    name="schema1.table_1",
-                ),
-                materialize.SourcePostgresTableArgs(
-                    alias="s2_table_1",
-                    name="schema2.table_1",
-                ),
-            ])
-        ```
-
         ## Import
 
         Sources can be imported using the source id
 
         ```sh
          $ pulumi import materialize:index/sourcePostgres:SourcePostgres example_source_postgres <region>:<source_id>
         ```
@@ -629,15 +528,14 @@
                  expose_progress: Optional[pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  postgres_connection: Optional[pulumi.Input[pulumi.InputType['SourcePostgresPostgresConnectionArgs']]] = None,
                  publication: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 schemas: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]]] = None,
                  text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -655,20 +553,20 @@
                 raise TypeError("Missing required property 'postgres_connection'")
             __props__.__dict__["postgres_connection"] = postgres_connection
             if publication is None and not opts.urn:
                 raise TypeError("Missing required property 'publication'")
             __props__.__dict__["publication"] = publication
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
-            __props__.__dict__["schemas"] = schemas
+            if tables is None and not opts.urn:
+                raise TypeError("Missing required property 'tables'")
             __props__.__dict__["tables"] = tables
             __props__.__dict__["text_columns"] = text_columns
             __props__.__dict__["qualified_sql_name"] = None
             __props__.__dict__["size"] = None
-            __props__.__dict__["subsources"] = None
         super(SourcePostgres, __self__).__init__(
             'materialize:index/sourcePostgres:SourcePostgres',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -682,41 +580,37 @@
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             postgres_connection: Optional[pulumi.Input[pulumi.InputType['SourcePostgresPostgresConnectionArgs']]] = None,
             publication: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
-            schemas: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             size: Optional[pulumi.Input[str]] = None,
-            subsources: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresSubsourceArgs']]]]] = None,
             tables: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]]] = None,
             text_columns: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'SourcePostgres':
         """
         Get an existing SourcePostgres resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the source database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
-        :param pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']] expose_progress: The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        :param pulumi.Input[pulumi.InputType['SourcePostgresExposeProgressArgs']] expose_progress: The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[pulumi.InputType['SourcePostgresPostgresConnectionArgs']] postgres_connection: The PostgreSQL connection to use in the source.
         :param pulumi.Input[str] publication: The PostgreSQL publication (the replication data set containing the tables to be streamed to Materialize).
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] schemas: Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresSubsourceArgs']]]] subsources: Subsources of a source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]] tables: Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourcePostgresTableArgs']]]] tables: Creates subsources for specific tables in the Postgres connection.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] text_columns: Decode data as text for specific columns that contain PostgreSQL types that are unsupported in Materialize. Can only be updated in place when also updating a corresponding `table` attribute.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SourcePostgresState.__new__(_SourcePostgresState)
 
         __props__.__dict__["cluster_name"] = cluster_name
@@ -726,17 +620,15 @@
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["postgres_connection"] = postgres_connection
         __props__.__dict__["publication"] = publication
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
-        __props__.__dict__["schemas"] = schemas
         __props__.__dict__["size"] = size
-        __props__.__dict__["subsources"] = subsources
         __props__.__dict__["tables"] = tables
         __props__.__dict__["text_columns"] = text_columns
         return SourcePostgres(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Output[str]:
@@ -761,15 +653,15 @@
         """
         return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter(name="exposeProgress")
     def expose_progress(self) -> pulumi.Output[Optional['outputs.SourcePostgresExposeProgress']]:
         """
-        The name of the progress subsource for the source. If this is not specified, the subsource will be named `<src_name>_progress`.
+        The name of the progress collection for the source. If this is not specified, the collection will be named `<src_name>_progress`.
         """
         return pulumi.get(self, "expose_progress")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
@@ -823,41 +715,25 @@
         """
         The identifier for the source schema in Materialize. Defaults to `public`.
         """
         return pulumi.get(self, "schema_name")
 
     @property
     @pulumi.getter
-    def schemas(self) -> pulumi.Output[Optional[Sequence[str]]]:
-        """
-        Creates subsources for specific schemas. If neither table or schema is specified, will default to ALL TABLES
-        """
-        return pulumi.get(self, "schemas")
-
-    @property
-    @pulumi.getter
     def size(self) -> pulumi.Output[str]:
         """
         The size of the cluster maintaining this source.
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter
-    def subsources(self) -> pulumi.Output[Sequence['outputs.SourcePostgresSubsource']]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @property
-    @pulumi.getter
-    def tables(self) -> pulumi.Output[Optional[Sequence['outputs.SourcePostgresTable']]]:
+    def tables(self) -> pulumi.Output[Sequence['outputs.SourcePostgresTable']]:
         """
-        Creates subsources for specific tables. If neither table or schema is specified, will default to ALL TABLES
+        Creates subsources for specific tables in the Postgres connection.
         """
         return pulumi.get(self, "tables")
 
     @property
     @pulumi.getter(name="textColumns")
     def text_columns(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/source_webhook.py` & `pulumi_materialize-0.3.0/pulumi_materialize/source_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,16 +224,15 @@
                  include_header: Optional[pulumi.Input[Sequence[pulumi.Input['SourceWebhookIncludeHeaderArgs']]]] = None,
                  include_headers: Optional[pulumi.Input['SourceWebhookIncludeHeadersArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 size: Optional[pulumi.Input[str]] = None,
-                 subsources: Optional[pulumi.Input[Sequence[pulumi.Input['SourceWebhookSubsourceArgs']]]] = None):
+                 size: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SourceWebhook resources.
         :param pulumi.Input[str] body_format: The body format of the webhook.
         :param pulumi.Input[str] check_expression: The check expression for the webhook.
         :param pulumi.Input[Sequence[pulumi.Input['SourceWebhookCheckOptionArgs']]] check_options: The check options for the webhook.
         :param pulumi.Input[str] cluster_name: The cluster to maintain this source.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
@@ -242,15 +241,14 @@
         :param pulumi.Input['SourceWebhookIncludeHeadersArgs'] include_headers: Include headers in the webhook.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input['SourceWebhookSubsourceArgs']]] subsources: Subsources of a source.
         """
         if body_format is not None:
             pulumi.set(__self__, "body_format", body_format)
         if check_expression is not None:
             pulumi.set(__self__, "check_expression", check_expression)
         if check_options is not None:
             pulumi.set(__self__, "check_options", check_options)
@@ -272,16 +270,14 @@
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
         if size is not None:
             pulumi.set(__self__, "size", size)
-        if subsources is not None:
-            pulumi.set(__self__, "subsources", subsources)
 
     @property
     @pulumi.getter(name="bodyFormat")
     def body_format(self) -> Optional[pulumi.Input[str]]:
         """
         The body format of the webhook.
         """
@@ -443,26 +439,14 @@
         """
         return pulumi.get(self, "size")
 
     @size.setter
     def size(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "size", value)
 
-    @property
-    @pulumi.getter
-    def subsources(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['SourceWebhookSubsourceArgs']]]]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
-    @subsources.setter
-    def subsources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['SourceWebhookSubsourceArgs']]]]):
-        pulumi.set(self, "subsources", value)
-
 
 class SourceWebhook(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  body_format: Optional[pulumi.Input[str]] = None,
@@ -637,15 +621,14 @@
             __props__.__dict__["include_headers"] = include_headers
             __props__.__dict__["name"] = name
             __props__.__dict__["ownership_role"] = ownership_role
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
             __props__.__dict__["qualified_sql_name"] = None
             __props__.__dict__["size"] = None
-            __props__.__dict__["subsources"] = None
         super(SourceWebhook, __self__).__init__(
             'materialize:index/sourceWebhook:SourceWebhook',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -661,16 +644,15 @@
             include_header: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceWebhookIncludeHeaderArgs']]]]] = None,
             include_headers: Optional[pulumi.Input[pulumi.InputType['SourceWebhookIncludeHeadersArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             ownership_role: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
-            size: Optional[pulumi.Input[str]] = None,
-            subsources: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceWebhookSubsourceArgs']]]]] = None) -> 'SourceWebhook':
+            size: Optional[pulumi.Input[str]] = None) -> 'SourceWebhook':
         """
         Get an existing SourceWebhook resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -684,15 +666,14 @@
         :param pulumi.Input[pulumi.InputType['SourceWebhookIncludeHeadersArgs']] include_headers: Include headers in the webhook.
         :param pulumi.Input[str] name: The identifier for the source.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the source.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the source schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] size: The size of the cluster maintaining this source.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['SourceWebhookSubsourceArgs']]]] subsources: Subsources of a source.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SourceWebhookState.__new__(_SourceWebhookState)
 
         __props__.__dict__["body_format"] = body_format
         __props__.__dict__["check_expression"] = check_expression
@@ -704,15 +685,14 @@
         __props__.__dict__["include_headers"] = include_headers
         __props__.__dict__["name"] = name
         __props__.__dict__["ownership_role"] = ownership_role
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["size"] = size
-        __props__.__dict__["subsources"] = subsources
         return SourceWebhook(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="bodyFormat")
     def body_format(self) -> pulumi.Output[str]:
         """
         The body format of the webhook.
@@ -819,15 +799,7 @@
     @pulumi.getter
     def size(self) -> pulumi.Output[str]:
         """
         The size of the cluster maintaining this source.
         """
         return pulumi.get(self, "size")
 
-    @property
-    @pulumi.getter
-    def subsources(self) -> pulumi.Output[Sequence['outputs.SourceWebhookSubsource']]:
-        """
-        Subsources of a source.
-        """
-        return pulumi.get(self, "subsources")
-
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/sso_config.py` & `pulumi_materialize-0.3.0/pulumi_materialize/sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/sso_default_roles.py` & `pulumi_materialize-0.3.0/pulumi_materialize/sso_default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/sso_domain.py` & `pulumi_materialize-0.3.0/pulumi_materialize/sso_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/sso_role_group_mapping.py` & `pulumi_materialize-0.3.0/pulumi_materialize/sso_role_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/system_parameter.py` & `pulumi_materialize-0.3.0/pulumi_materialize/system_parameter.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/table.py` & `pulumi_materialize-0.3.0/pulumi_materialize/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/type.py` & `pulumi_materialize-0.3.0/pulumi_materialize/type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/user.py` & `pulumi_materialize-0.3.0/pulumi_materialize/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize/view.py` & `pulumi_materialize-0.3.0/pulumi_materialize/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize.egg-info/PKG-INFO` & `pulumi_materialize-0.3.0/pulumi_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-materialize
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.2.1/pulumi_materialize.egg-info/SOURCES.txt` & `pulumi_materialize-0.3.0/pulumi_materialize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.2.1/setup.py` & `pulumi_materialize-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.2.1"
+VERSION = "0.3.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "materialize Pulumi Package - Development Version"
```

