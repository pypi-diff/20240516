# Comparing `tmp/pyatlan-2.1.9.tar.gz` & `tmp/pyatlan-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-2.1.9.tar", last modified: Tue May 14 15:10:41 2024, max compression
+gzip compressed data, was "pyatlan-2.2.0.tar", last modified: Wed May 15 12:40:29 2024, max compression
```

## Comparing `pyatlan-2.1.9.tar` & `pyatlan-2.2.0.tar`

### file list

```diff
@@ -1,492 +1,492 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-14 15:10:35.000000 pyatlan-2.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 15:10:35.000000 pyatlan-2.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-14 15:10:41.929864 pyatlan-2.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 15:10:35.000000 pyatlan-2.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.841863 pyatlan-2.1.9/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.845864 pyatlan-2.1.9/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/events/atlan_lambda_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/create_typedefs_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.849864 pyatlan-2.1.9/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/enums.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/globals.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/properties.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/referenceable_attributes.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/referenceable_methods.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/generator/templates/structs.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.857864 pyatlan-2.1.9/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/api_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.905864 pyatlan-2.1.9/pyatlan/model/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_p_i_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/a_w_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/auth_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/b_i_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/calculation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite3_d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cognite_time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/cube_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/data_studio_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_model_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/domo_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/dynamo_dbtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/event_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/g_c_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_look.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/looker_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/m_c_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/m_c_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/materialised_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/matillion_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metabase_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_dossier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mode_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/multi_dimensional_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/no_s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/power_b_i_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/preset_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/process_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/qlik_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/quick_sight_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/readme_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/redash_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s3_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/saa_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/salesforce_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/schema_registry_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sigma_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/sisense_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/snowflake_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/soda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/soda_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/spark_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/table_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_calculated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tableau_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/tag_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_dashlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/assets/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    76441 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.905864 pyatlan-2.1.9/pyatlan/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fields/atlan_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fluent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/fluent_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/model/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/model/packages/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/base/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/big_query_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/confluent_kafka_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/dbt_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/dynamo_d_b_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/glue_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/postgres_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/powerbi_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/s_q_l_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/sigma_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/snowflake_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/snowflake_miner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/sql_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/packages/tableau_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/model/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/multipart_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.909864 pyatlan-2.1.9/pyatlan/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/create_package_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.913864 pyatlan-2.1.9/pyatlan/pkg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/default_configmap.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/default_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/templates/package_config.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/pkg/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 15:10:35.000000 pyatlan-2.1.9/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 15:10:41.000000 pyatlan-2.1.9/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 15:10:35.000000 pyatlan-2.1.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:10:35.000000 pyatlan-2.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:10:41.929864 pyatlan-2.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-14 15:10:35.000000 pyatlan-2.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.913864 pyatlan-2.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.917864 pyatlan-2.1.9/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/adls_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/airflow_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/api_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/custom_package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/data_mesh_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/gcs_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/owner_propagator_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/preset_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/requests_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_sql_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/test_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.921864 pyatlan-2.1.9/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_account_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_d_l_s_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_p_i_path_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/a_p_i_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/column_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_product_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/database_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/fields/atlan_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/gcs_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/gcs_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_chart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_dashboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/preset_workspace_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/model/view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:41.929864 pyatlan-2.1.9/tests/unit/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/pkg/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    68514 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_credential_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_file_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_query_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_sso_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-14 15:10:35.000000 pyatlan-2.1.9/tests/unit/test_workflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.429369 pyatlan-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 12:40:23.000000 pyatlan-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 12:40:23.000000 pyatlan-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 12:40:29.429369 pyatlan-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-15 12:40:23.000000 pyatlan-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.353369 pyatlan-2.2.0/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77429 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59409 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33221 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.357369 pyatlan-2.2.0/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/events/atlan_lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.361369 pyatlan-2.2.0/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32321 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/create_typedefs_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.361369 pyatlan-2.2.0/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/enums.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/globals.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/properties.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/referenceable_attributes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/referenceable_methods.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/generator/templates/structs.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.365369 pyatlan-2.2.0/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/api_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.405369 pyatlan-2.2.0/pyatlan/model/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    23409 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_p_i_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/a_w_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)   124326 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/auth_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/b_i_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/calculation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite3_d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cognite_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45012 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21623 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/cube_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/data_studio_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_model_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/domo_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/dynamo_dbtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/event_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/g_c_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_look.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/looker_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/m_c_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/m_c_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/materialised_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/matillion_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metabase_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_dossier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mode_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/multi_dimensional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/no_s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/power_b_i_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/preset_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/process_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/qlik_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/quick_sight_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/readme_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/redash_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s3_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/saa_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/salesforce_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/schema_registry_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sigma_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/sisense_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/snowflake_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/soda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/soda_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/spark_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/table_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_calculated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tableau_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/tag_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_dashlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/assets/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76441 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.405369 pyatlan-2.2.0/pyatlan/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fields/atlan_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fluent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/fluent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/model/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/model/packages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/big_query_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/confluent_kafka_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/dbt_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/dynamo_d_b_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/postgres_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/powerbi_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/s_q_l_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/sigma_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/snowflake_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/snowflake_miner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/sql_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/packages/tableau_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/model/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/multipart_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.409369 pyatlan-2.2.0/pyatlan/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/create_package_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.413369 pyatlan-2.2.0/pyatlan/pkg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/default_configmap.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/default_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/templates/package_config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/pkg/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 12:40:23.000000 pyatlan-2.2.0/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.429369 pyatlan-2.2.0/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 12:40:29.000000 pyatlan-2.2.0/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-15 12:40:23.000000 pyatlan-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 12:40:23.000000 pyatlan-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:40:29.429369 pyatlan-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-15 12:40:23.000000 pyatlan-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.413369 pyatlan-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.417369 pyatlan-2.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/adls_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/airflow_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/api_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/custom_package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/data_mesh_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/gcs_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26912 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/owner_propagator_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/preset_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/requests_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_sql_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/test_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.421369 pyatlan-2.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_account_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_d_l_s_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_p_i_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/a_p_i_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/column_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/fields/atlan_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/gcs_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/gcs_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_chart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_dashboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/preset_workspace_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/model/view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:29.425369 pyatlan-2.2.0/tests/unit/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/pkg/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68514 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_credential_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_file_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_query_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_sso_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15955 2024-05-15 12:40:23.000000 pyatlan-2.2.0/tests/unit/test_workflow_client.py
```

### Comparing `pyatlan-2.1.9/LICENSE` & `pyatlan-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/PKG-INFO` & `pyatlan-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.9
+Version: 2.2.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.9/README.md` & `pyatlan-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-2.2.0/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-2.2.0/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/enum_cache.py` & `pyatlan-2.2.0/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/group_cache.py` & `pyatlan-2.2.0/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/role_cache.py` & `pyatlan-2.2.0/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/cache/user_cache.py` & `pyatlan-2.2.0/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/admin.py` & `pyatlan-2.2.0/pyatlan/client/admin.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/asset.py` & `pyatlan-2.2.0/pyatlan/client/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/atlan.py` & `pyatlan-2.2.0/pyatlan/client/atlan.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/audit.py` & `pyatlan-2.2.0/pyatlan/client/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/common.py` & `pyatlan-2.2.0/pyatlan/client/common.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/constants.py` & `pyatlan-2.2.0/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/credential.py` & `pyatlan-2.2.0/pyatlan/client/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/file.py` & `pyatlan-2.2.0/pyatlan/client/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/group.py` & `pyatlan-2.2.0/pyatlan/client/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/impersonate.py` & `pyatlan-2.2.0/pyatlan/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/query.py` & `pyatlan-2.2.0/pyatlan/client/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/role.py` & `pyatlan-2.2.0/pyatlan/client/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/search_log.py` & `pyatlan-2.2.0/pyatlan/client/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/sso.py` & `pyatlan-2.2.0/pyatlan/client/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/task.py` & `pyatlan-2.2.0/pyatlan/client/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/token.py` & `pyatlan-2.2.0/pyatlan/client/token.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/typedef.py` & `pyatlan-2.2.0/pyatlan/client/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/user.py` & `pyatlan-2.2.0/pyatlan/client/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/client/workflow.py` & `pyatlan-2.2.0/pyatlan/client/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/errors.py` & `pyatlan-2.2.0/pyatlan/errors.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/events/atlan_event_handler.py` & `pyatlan-2.2.0/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-2.2.0/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/class_generator.py` & `pyatlan-2.2.0/pyatlan/generator/class_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/create_typedefs_file.py` & `pyatlan-2.2.0/pyatlan/generator/create_typedefs_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/globals.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/globals.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/imports.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/imports.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/macros.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/module.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/module.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/properties.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/properties.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/referenceable_attributes.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/referenceable_attributes.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/referenceable_methods.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/referenceable_methods.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/generator/templates/structs.jinja2` & `pyatlan-2.2.0/pyatlan/generator/templates/structs.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/logging.conf` & `pyatlan-2.2.0/pyatlan/logging.conf`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/aggregation.py` & `pyatlan-2.2.0/pyatlan/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/api_tokens.py` & `pyatlan-2.2.0/pyatlan/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/__init__.py` & `pyatlan-2.2.0/pyatlan/model/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_account.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_account.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_container.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_container.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_d_l_s_object.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_d_l_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_p_i.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_p_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_p_i_path.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_p_i_path.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_p_i_spec.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_p_i_spec.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/a_w_s.py` & `pyatlan-2.2.0/pyatlan/model/assets/a_w_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/access_control.py` & `pyatlan-2.2.0/pyatlan/model/assets/access_control.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/airflow.py` & `pyatlan-2.2.0/pyatlan/model/assets/airflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/airflow_dag.py` & `pyatlan-2.2.0/pyatlan/model/assets/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/airflow_task.py` & `pyatlan-2.2.0/pyatlan/model/assets/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/asset.py` & `pyatlan-2.2.0/pyatlan/model/assets/asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary.py` & `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_category.py` & `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_category.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/atlas_glossary_term.py` & `pyatlan-2.2.0/pyatlan/model/assets/atlas_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/auth_policy.py` & `pyatlan-2.2.0/pyatlan/model/assets/auth_policy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/auth_service.py` & `pyatlan-2.2.0/pyatlan/model/assets/auth_service.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure_event_hub_consumer_group.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure_event_hub_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_namespace.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/azure_service_bus_topic.py` & `pyatlan-2.2.0/pyatlan/model/assets/azure_service_bus_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/b_i.py` & `pyatlan-2.2.0/pyatlan/model/assets/b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/b_i_process.py` & `pyatlan-2.2.0/pyatlan/model/assets/b_i_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/badge.py` & `pyatlan-2.2.0/pyatlan/model/assets/badge.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/calculation_view.py` & `pyatlan-2.2.0/pyatlan/model/assets/calculation_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/catalog.py` & `pyatlan-2.2.0/pyatlan/model/assets/catalog.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cloud.py` & `pyatlan-2.2.0/pyatlan/model/assets/cloud.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite3_d_model.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite3_d_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite_asset.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite_event.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite_event.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite_file.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite_sequence.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite_sequence.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cognite_time_series.py` & `pyatlan-2.2.0/pyatlan/model/assets/cognite_time_series.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/collection.py` & `pyatlan-2.2.0/pyatlan/model/assets/collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/column.py` & `pyatlan-2.2.0/pyatlan/model/assets/column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/column_process.py` & `pyatlan-2.2.0/pyatlan/model/assets/column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/connection.py` & `pyatlan-2.2.0/pyatlan/model/assets/connection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b.py` & `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_collection.py` & `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cosmos_mongo_d_b_database.py` & `pyatlan-2.2.0/pyatlan/model/assets/cosmos_mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cube.py` & `pyatlan-2.2.0/pyatlan/model/assets/cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cube_dimension.py` & `pyatlan-2.2.0/pyatlan/model/assets/cube_dimension.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cube_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/cube_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/cube_hierarchy.py` & `pyatlan-2.2.0/pyatlan/model/assets/cube_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_contract.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_contract.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_domain.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_domain.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_mesh.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_product.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_product.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_quality.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_quality.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_set.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_set.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_studio.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_studio.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/data_studio_asset.py` & `pyatlan-2.2.0/pyatlan/model/assets/data_studio_asset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/database.py` & `pyatlan-2.2.0/pyatlan/model/assets/database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_column_process.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_column_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_metric.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_model.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_model_column.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_model_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_process.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_source.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_source.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_tag.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dbt_test.py` & `pyatlan-2.2.0/pyatlan/model/assets/dbt_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/domo.py` & `pyatlan-2.2.0/pyatlan/model/assets/domo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/domo_card.py` & `pyatlan-2.2.0/pyatlan/model/assets/domo_card.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/domo_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/domo_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/domo_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/domo_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/domo_dataset_column.py` & `pyatlan-2.2.0/pyatlan/model/assets/domo_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b.py` & `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py` & `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py` & `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dynamo_d_b_secondary_index.py` & `pyatlan-2.2.0/pyatlan/model/assets/dynamo_d_b_secondary_index.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/dynamo_dbtable.py` & `pyatlan-2.2.0/pyatlan/model/assets/dynamo_dbtable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/event_store.py` & `pyatlan-2.2.0/pyatlan/model/assets/event_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/file.py` & `pyatlan-2.2.0/pyatlan/model/assets/file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/folder.py` & `pyatlan-2.2.0/pyatlan/model/assets/folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/function.py` & `pyatlan-2.2.0/pyatlan/model/assets/function.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/g_c_s.py` & `pyatlan-2.2.0/pyatlan/model/assets/g_c_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/g_c_s_bucket.py` & `pyatlan-2.2.0/pyatlan/model/assets/g_c_s_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/g_c_s_object.py` & `pyatlan-2.2.0/pyatlan/model/assets/g_c_s_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/google.py` & `pyatlan-2.2.0/pyatlan/model/assets/google.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/infrastructure.py` & `pyatlan-2.2.0/pyatlan/model/assets/infrastructure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/insight.py` & `pyatlan-2.2.0/pyatlan/model/assets/insight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/kafka.py` & `pyatlan-2.2.0/pyatlan/model/assets/kafka.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/kafka_consumer_group.py` & `pyatlan-2.2.0/pyatlan/model/assets/kafka_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/kafka_topic.py` & `pyatlan-2.2.0/pyatlan/model/assets/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/link.py` & `pyatlan-2.2.0/pyatlan/model/assets/link.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_explore.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_explore.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_folder.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_look.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_look.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_model.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_project.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_query.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_tile.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/looker_view.py` & `pyatlan-2.2.0/pyatlan/model/assets/looker_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/m_c_incident.py` & `pyatlan-2.2.0/pyatlan/model/assets/m_c_incident.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/m_c_monitor.py` & `pyatlan-2.2.0/pyatlan/model/assets/m_c_monitor.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/materialised_view.py` & `pyatlan-2.2.0/pyatlan/model/assets/materialised_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/matillion.py` & `pyatlan-2.2.0/pyatlan/model/assets/matillion.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/matillion_component.py` & `pyatlan-2.2.0/pyatlan/model/assets/matillion_component.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/matillion_group.py` & `pyatlan-2.2.0/pyatlan/model/assets/matillion_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/matillion_job.py` & `pyatlan-2.2.0/pyatlan/model/assets/matillion_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/matillion_project.py` & `pyatlan-2.2.0/pyatlan/model/assets/matillion_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/metabase.py` & `pyatlan-2.2.0/pyatlan/model/assets/metabase.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/metabase_collection.py` & `pyatlan-2.2.0/pyatlan/model/assets/metabase_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/metabase_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/metabase_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/metabase_question.py` & `pyatlan-2.2.0/pyatlan/model/assets/metabase_question.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/metric.py` & `pyatlan-2.2.0/pyatlan/model/assets/metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_attribute.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_attribute.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_cube.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_cube.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_document.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_document.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_dossier.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_dossier.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_fact.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_fact.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_metric.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_project.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_report.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/micro_strategy_visualization.py` & `pyatlan-2.2.0/pyatlan/model/assets/micro_strategy_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode_chart.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode_collection.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode_query.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode_report.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mode_workspace.py` & `pyatlan-2.2.0/pyatlan/model/assets/mode_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b.py` & `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_collection.py` & `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_collection.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/mongo_d_b_database.py` & `pyatlan-2.2.0/pyatlan/model/assets/mongo_d_b_database.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/monte_carlo.py` & `pyatlan-2.2.0/pyatlan/model/assets/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/multi_dimensional_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/multi_dimensional_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/namespace.py` & `pyatlan-2.2.0/pyatlan/model/assets/namespace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/no_s_q_l.py` & `pyatlan-2.2.0/pyatlan/model/assets/no_s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/object_store.py` & `pyatlan-2.2.0/pyatlan/model/assets/object_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/persona.py` & `pyatlan-2.2.0/pyatlan/model/assets/persona.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_column.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataflow.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_datasource.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_measure.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_measure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_page.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_report.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_table.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_tile.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_tile.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/power_b_i_workspace.py` & `pyatlan-2.2.0/pyatlan/model/assets/power_b_i_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/preset.py` & `pyatlan-2.2.0/pyatlan/model/assets/preset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/preset_chart.py` & `pyatlan-2.2.0/pyatlan/model/assets/preset_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/preset_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/preset_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/preset_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/preset_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/preset_workspace.py` & `pyatlan-2.2.0/pyatlan/model/assets/preset_workspace.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/procedure.py` & `pyatlan-2.2.0/pyatlan/model/assets/procedure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/process.py` & `pyatlan-2.2.0/pyatlan/model/assets/process.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/process_execution.py` & `pyatlan-2.2.0/pyatlan/model/assets/process_execution.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/purpose.py` & `pyatlan-2.2.0/pyatlan/model/assets/purpose.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_app.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_app.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_chart.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_chart.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_sheet.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_sheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_space.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_space.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/qlik_stream.py` & `pyatlan-2.2.0/pyatlan/model/assets/qlik_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/query.py` & `pyatlan-2.2.0/pyatlan/model/assets/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_analysis_visual.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_analysis_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dashboard_visual.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dashboard_visual.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_dataset_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_dataset_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/quick_sight_folder.py` & `pyatlan-2.2.0/pyatlan/model/assets/quick_sight_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/readme.py` & `pyatlan-2.2.0/pyatlan/model/assets/readme.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/readme_template.py` & `pyatlan-2.2.0/pyatlan/model/assets/readme_template.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/redash.py` & `pyatlan-2.2.0/pyatlan/model/assets/redash.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/redash_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/redash_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/redash_query.py` & `pyatlan-2.2.0/pyatlan/model/assets/redash_query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/redash_visualization.py` & `pyatlan-2.2.0/pyatlan/model/assets/redash_visualization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/referenceable.py` & `pyatlan-2.2.0/pyatlan/model/assets/referenceable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/resource.py` & `pyatlan-2.2.0/pyatlan/model/assets/resource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/s3.py` & `pyatlan-2.2.0/pyatlan/model/assets/s3.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/s3_bucket.py` & `pyatlan-2.2.0/pyatlan/model/assets/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/s3_object.py` & `pyatlan-2.2.0/pyatlan/model/assets/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/s_q_l.py` & `pyatlan-2.2.0/pyatlan/model/assets/s_q_l.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/saa_s.py` & `pyatlan-2.2.0/pyatlan/model/assets/saa_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce_object.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce_object.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce_organization.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce_organization.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/salesforce_report.py` & `pyatlan-2.2.0/pyatlan/model/assets/salesforce_report.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/schema.py` & `pyatlan-2.2.0/pyatlan/model/assets/schema.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/schema_registry.py` & `pyatlan-2.2.0/pyatlan/model/assets/schema_registry.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/schema_registry_subject.py` & `pyatlan-2.2.0/pyatlan/model/assets/schema_registry_subject.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_data_element_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_data_element_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_dataset_column.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_dataset_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_page.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_page.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sigma_workbook.py` & `pyatlan-2.2.0/pyatlan/model/assets/sigma_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense_datamodel_table.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense_datamodel_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense_folder.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense_folder.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/sisense_widget.py` & `pyatlan-2.2.0/pyatlan/model/assets/sisense_widget.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/snowflake_dynamic_table.py` & `pyatlan-2.2.0/pyatlan/model/assets/snowflake_dynamic_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/snowflake_pipe.py` & `pyatlan-2.2.0/pyatlan/model/assets/snowflake_pipe.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/snowflake_stream.py` & `pyatlan-2.2.0/pyatlan/model/assets/snowflake_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/snowflake_tag.py` & `pyatlan-2.2.0/pyatlan/model/assets/snowflake_tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/soda.py` & `pyatlan-2.2.0/pyatlan/model/assets/soda.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/soda_check.py` & `pyatlan-2.2.0/pyatlan/model/assets/soda_check.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/spark.py` & `pyatlan-2.2.0/pyatlan/model/assets/spark.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/spark_job.py` & `pyatlan-2.2.0/pyatlan/model/assets/spark_job.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/table.py` & `pyatlan-2.2.0/pyatlan/model/assets/table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/table_partition.py` & `pyatlan-2.2.0/pyatlan/model/assets/table_partition.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_calculated_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_calculated_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_dashboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_datasource_field.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_datasource_field.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_flow.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_flow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_metric.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_metric.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_project.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_project.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_site.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_site.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_workbook.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_workbook.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tableau_worksheet.py` & `pyatlan-2.2.0/pyatlan/model/assets/tableau_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tag.py` & `pyatlan-2.2.0/pyatlan/model/assets/tag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/tag_attachment.py` & `pyatlan-2.2.0/pyatlan/model/assets/tag_attachment.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_answer.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_answer.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_column.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_column.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_dashlet.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_dashlet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_liveboard.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_liveboard.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_table.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_table.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_view.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/thoughtspot_worksheet.py` & `pyatlan-2.2.0/pyatlan/model/assets/thoughtspot_worksheet.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/assets/view.py` & `pyatlan-2.2.0/pyatlan/model/assets/view.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/atlan_image.py` & `pyatlan-2.2.0/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/audit.py` & `pyatlan-2.2.0/pyatlan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/core.py` & `pyatlan-2.2.0/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/credential.py` & `pyatlan-2.2.0/pyatlan/model/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/custom_metadata.py` & `pyatlan-2.2.0/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/data_mesh.py` & `pyatlan-2.2.0/pyatlan/model/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/enums.py` & `pyatlan-2.2.0/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/events.py` & `pyatlan-2.2.0/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/fields/atlan_fields.py` & `pyatlan-2.2.0/pyatlan/model/fields/atlan_fields.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/fluent_search.py` & `pyatlan-2.2.0/pyatlan/model/fluent_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/fluent_tasks.py` & `pyatlan-2.2.0/pyatlan/model/fluent_tasks.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/group.py` & `pyatlan-2.2.0/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/keycloak_events.py` & `pyatlan-2.2.0/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/lineage.py` & `pyatlan-2.2.0/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/__init__.py` & `pyatlan-2.2.0/pyatlan/model/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/base/crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/base/crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/base/miner.py` & `pyatlan-2.2.0/pyatlan/model/packages/base/miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/base/package.py` & `pyatlan-2.2.0/pyatlan/model/packages/base/package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/big_query_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/big_query_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/confluent_kafka_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/confluent_kafka_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/dbt_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/dbt_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/dynamo_d_b_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/dynamo_d_b_crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             "auth_type": "iam",
             "username": access_key,
             "password": secret_key,
         }
         self._credentials_body.update(local_creds)
         return self
 
-    def iam_user_role_auth(self, arn: str, external_id: str) -> DynamoDBCrawler:
+    def iam_role_auth(self, arn: str, external_id: str) -> DynamoDBCrawler:
         """
         Set up the crawler to use IAM role-based authentication.
 
         :param arn: ARN of the AWS role
         :param external_id: AWS external ID
         :returns: crawler, set up to use IAM user role-based authentication
         """
```

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/glue_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/postgres_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/postgres_crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,36 +117,36 @@
 
     def iam_user_auth(
         self, username: str, access_key: str, secret_key: str
     ) -> PostgresCrawler:
         """
         Set up the crawler to use IAM user-based authentication.
 
-        :param username: username for the IAM user
+        :param username: database username to extract from
         :param access_key: through which to access PostgreSQL
         :param secret_key: through which to access PostgreSQL
         :returns: crawler, set up to use IAM user-based authentication
         """
         local_creds = {
             "auth_type": "iam_user",
             "connector_type": "jdbc",
             "username": access_key,
             "password": secret_key,
         }
         self._credentials_body["extra"].update({"username": username})
         self._credentials_body.update(local_creds)
         return self
 
-    def iam_user_role_auth(
+    def iam_role_auth(
         self, username: str, arn: str, external_id: str
     ) -> PostgresCrawler:
         """
-        Set up the crawler to use IAM user role-based authentication.
+        Set up the crawler to use IAM role-based authentication.
 
-        :param username: username for the IAM user
+        :param username: database username to extract from
         :param arn: ARN of the AWS role
         :param external_id: AWS external ID
         :returns: crawler, set up to use IAM user role-based authentication
         """
         local_creds = {
             "auth_type": "iam_role",
             "connector_type": "jdbc",
```

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/powerbi_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/powerbi_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/s_q_l_server_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/s_q_l_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/sigma_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/sigma_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/snowflake_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/snowflake_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/snowflake_miner.py` & `pyatlan-2.2.0/pyatlan/model/packages/snowflake_miner.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/sql_server_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/sql_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/packages/tableau_crawler.py` & `pyatlan-2.2.0/pyatlan/model/packages/tableau_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/query.py` & `pyatlan-2.2.0/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/response.py` & `pyatlan-2.2.0/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/role.py` & `pyatlan-2.2.0/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/search.py` & `pyatlan-2.2.0/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/search_log.py` & `pyatlan-2.2.0/pyatlan/model/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/sso.py` & `pyatlan-2.2.0/pyatlan/model/sso.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/structs.py` & `pyatlan-2.2.0/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/task.py` & `pyatlan-2.2.0/pyatlan/model/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/typedef.py` & `pyatlan-2.2.0/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/user.py` & `pyatlan-2.2.0/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/utils.py` & `pyatlan-2.2.0/pyatlan/model/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/model/workflow.py` & `pyatlan-2.2.0/pyatlan/model/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/multipart_data_generator.py` & `pyatlan-2.2.0/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/create_package_files.py` & `pyatlan-2.2.0/pyatlan/pkg/create_package_files.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/models.py` & `pyatlan-2.2.0/pyatlan/pkg/models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/templates/default_configmap.jinja2` & `pyatlan-2.2.0/pyatlan/pkg/templates/default_configmap.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/templates/default_template.jinja2` & `pyatlan-2.2.0/pyatlan/pkg/templates/default_template.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/templates/package_config.jinja2` & `pyatlan-2.2.0/pyatlan/pkg/templates/package_config.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/ui.py` & `pyatlan-2.2.0/pyatlan/pkg/ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/utils.py` & `pyatlan-2.2.0/pyatlan/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/pkg/widgets.py` & `pyatlan-2.2.0/pyatlan/pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan/utils.py` & `pyatlan-2.2.0/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/pyatlan.egg-info/PKG-INFO` & `pyatlan-2.2.0/pyatlan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.9
+Version: 2.2.0
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.9/pyatlan.egg-info/SOURCES.txt` & `pyatlan-2.2.0/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/setup.py` & `pyatlan-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/adls_asset_test.py` & `pyatlan-2.2.0/tests/integration/adls_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/admin_test.py` & `pyatlan-2.2.0/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/airflow_asset_test.py` & `pyatlan-2.2.0/tests/integration/airflow_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/api_asset_test.py` & `pyatlan-2.2.0/tests/integration/api_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/atlan_tag_test.py` & `pyatlan-2.2.0/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/client.py` & `pyatlan-2.2.0/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/connection_test.py` & `pyatlan-2.2.0/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/custom_metadata_test.py` & `pyatlan-2.2.0/tests/integration/custom_metadata_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/custom_package_test.py` & `pyatlan-2.2.0/tests/integration/custom_package_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/data_mesh_test.py` & `pyatlan-2.2.0/tests/integration/data_mesh_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/data_studio_asset_test.py` & `pyatlan-2.2.0/tests/integration/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/file_test.py` & `pyatlan-2.2.0/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/gcs_asset_test.py` & `pyatlan-2.2.0/tests/integration/gcs_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/glossary_test.py` & `pyatlan-2.2.0/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/lineage_test.py` & `pyatlan-2.2.0/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/owner_propagator_cfg.py` & `pyatlan-2.2.0/tests/integration/owner_propagator_cfg.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/persona_test.py` & `pyatlan-2.2.0/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/preset_asset_test.py` & `pyatlan-2.2.0/tests/integration/preset_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/purpose_test.py` & `pyatlan-2.2.0/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/query_parser_test.py` & `pyatlan-2.2.0/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/requests_test.py` & `pyatlan-2.2.0/tests/integration/requests_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/s3_asset_test.py` & `pyatlan-2.2.0/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_client.py` & `pyatlan-2.2.0/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_file_client.py` & `pyatlan-2.2.0/tests/integration/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_index_search.py` & `pyatlan-2.2.0/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_sql_assets.py` & `pyatlan-2.2.0/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_sso_client.py` & `pyatlan-2.2.0/tests/integration/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_task_client.py` & `pyatlan-2.2.0/tests/integration/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/test_workflow_client.py` & `pyatlan-2.2.0/tests/integration/test_workflow_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/integration/utils.py` & `pyatlan-2.2.0/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/conftest.py` & `pyatlan-2.2.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/constants.py` & `pyatlan-2.2.0/tests/unit/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/a_d_l_s_account_test.py` & `pyatlan-2.2.0/tests/unit/model/a_d_l_s_account_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/a_d_l_s_container_test.py` & `pyatlan-2.2.0/tests/unit/model/a_d_l_s_container_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/a_d_l_s_object_test.py` & `pyatlan-2.2.0/tests/unit/model/a_d_l_s_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/a_p_i_path_test.py` & `pyatlan-2.2.0/tests/unit/model/a_p_i_path_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/a_p_i_spec_test.py` & `pyatlan-2.2.0/tests/unit/model/a_p_i_spec_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/airflow_dag.py` & `pyatlan-2.2.0/tests/unit/model/airflow_dag.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/airflow_task.py` & `pyatlan-2.2.0/tests/unit/model/airflow_task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/badge_condition_test.py` & `pyatlan-2.2.0/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/badge_test.py` & `pyatlan-2.2.0/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/column_process_test.py` & `pyatlan-2.2.0/tests/unit/model/column_process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/column_test.py` & `pyatlan-2.2.0/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/connection_test.py` & `pyatlan-2.2.0/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/constants.py` & `pyatlan-2.2.0/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/data_domain_test.py` & `pyatlan-2.2.0/tests/unit/model/data_domain_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/data_product_test.py` & `pyatlan-2.2.0/tests/unit/model/data_product_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/data_studio_asset_test.py` & `pyatlan-2.2.0/tests/unit/model/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/database_test.py` & `pyatlan-2.2.0/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/fields/atlan_fields_test.py` & `pyatlan-2.2.0/tests/unit/model/fields/atlan_fields_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/file_test.py` & `pyatlan-2.2.0/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/gcs_bucket_test.py` & `pyatlan-2.2.0/tests/unit/model/gcs_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/gcs_object_test.py` & `pyatlan-2.2.0/tests/unit/model/gcs_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/glossary_category_test.py` & `pyatlan-2.2.0/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/glossary_term_test.py` & `pyatlan-2.2.0/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/glossary_test.py` & `pyatlan-2.2.0/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/materialised_view_test.py` & `pyatlan-2.2.0/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/preset_chart_test.py` & `pyatlan-2.2.0/tests/unit/model/preset_chart_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/preset_dashboard_test.py` & `pyatlan-2.2.0/tests/unit/model/preset_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/preset_dataset_test.py` & `pyatlan-2.2.0/tests/unit/model/preset_dataset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/preset_workspace_test.py` & `pyatlan-2.2.0/tests/unit/model/preset_workspace_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/process_test.py` & `pyatlan-2.2.0/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/readme_test.py` & `pyatlan-2.2.0/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/s3_bucket_test.py` & `pyatlan-2.2.0/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/s3object_test.py` & `pyatlan-2.2.0/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/schema_test.py` & `pyatlan-2.2.0/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/table_test.py` & `pyatlan-2.2.0/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/model/view_test.py` & `pyatlan-2.2.0/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/pkg/conftest.py` & `pyatlan-2.2.0/tests/unit/pkg/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/pkg/test_models.py` & `pyatlan-2.2.0/tests/unit/pkg/test_models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/pkg/test_ui.py` & `pyatlan-2.2.0/tests/unit/pkg/test_ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/pkg/test_utils.py` & `pyatlan-2.2.0/tests/unit/pkg/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/pkg/test_widgets.py` & `pyatlan-2.2.0/tests/unit/pkg/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_atlan_tag_name.py` & `pyatlan-2.2.0/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_client.py` & `pyatlan-2.2.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_core.py` & `pyatlan-2.2.0/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_credential_client.py` & `pyatlan-2.2.0/tests/unit/test_credential_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_custom_metadata.py` & `pyatlan-2.2.0/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_deprecated.py` & `pyatlan-2.2.0/tests/unit/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_events.py` & `pyatlan-2.2.0/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_file_client.py` & `pyatlan-2.2.0/tests/unit/test_file_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_glossary_term.py` & `pyatlan-2.2.0/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_lineage.py` & `pyatlan-2.2.0/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_model.py` & `pyatlan-2.2.0/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_packages.py` & `pyatlan-2.2.0/tests/unit/test_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,15 +466,15 @@
     assert request_json == load_json(DYNAMO_DB_IAM_USER)
 
     dynamo_db_direct_iam_user_role = (
         DynamoDBCrawler(
             connection_name="test-dynamodb-conn", admin_roles=["admin-guid-1234"]
         )
         .direct(region="test-region")
-        .iam_user_role_auth(
+        .iam_role_auth(
             arn="arn:aws:iam::123456789012:user/test", external_id="test-ext-id"
         )
         .include_regex(regex=".*_TEST_INCLUDE")
         .exclude_regex(regex=".*_TEST_EXCLUDE")
         .to_workflow()
     )
     request_json = loads(
@@ -531,15 +531,15 @@
 
     postgres_direct_iam_role = (
         PostgresCrawler(
             connection_name="test-sdk-postgresql",
             admin_roles=["admin-guid-1234"],
         )
         .direct(hostname="test.com", database="test-db")
-        .iam_user_role_auth(
+        .iam_role_auth(
             username="test-user",
             arn="arn:aws:iam::123456789012:user/test",
             external_id="test-ext-id",
         )
         .include(assets={"test-include": ["test-asset-1", "test-asset-2"]})
         .exclude(assets=None)
         .exclude_regex(regex=".*_TEST")
```

### Comparing `pyatlan-2.1.9/tests/unit/test_query_client.py` & `pyatlan-2.2.0/tests/unit/test_query_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_search_model.py` & `pyatlan-2.2.0/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_sso_client.py` & `pyatlan-2.2.0/tests/unit/test_sso_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_structs.py` & `pyatlan-2.2.0/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_task_client.py` & `pyatlan-2.2.0/tests/unit/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_typedef_model.py` & `pyatlan-2.2.0/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_utils.py` & `pyatlan-2.2.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.9/tests/unit/test_workflow_client.py` & `pyatlan-2.2.0/tests/unit/test_workflow_client.py`

 * *Files identical despite different names*

