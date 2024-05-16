# Comparing `tmp/mmisp_lib-0.1.4.tar.gz` & `tmp/mmisp_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmisp_lib-0.1.4.tar", last modified: Mon May  6 10:41:05 2024, max compression
+gzip compressed data, was "mmisp_lib-0.1.5.tar", last modified: Thu May 16 15:46:31 2024, max compression
```

## Comparing `mmisp_lib-0.1.4.tar` & `mmisp_lib-0.1.5.tar`

### file list

```diff
@@ -1,194 +1,196 @@
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.364229 mmisp_lib-0.1.4/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-06 10:41:05.364229 mmisp_lib-0.1.4/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.4/README.md
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      947 2024-05-06 10:35:43.000000 mmisp_lib-0.1.4/pyproject.toml
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-06 10:41:05.364229 mmisp_lib-0.1.4/setup.cfg
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.344229 mmisp_lib-0.1.4/src/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.344229 mmisp_lib-0.1.4/src/mmisp/
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.344229 mmisp_lib-0.1.4/src/mmisp/api_schemas/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/__init__.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.348229 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1092 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/add_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      764 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/add_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/delete_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/edit_attribute_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/edit_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_attribute_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1486 2024-05-02 19:26:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      813 2024-05-02 19:26:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_describe_types_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3225 2024-05-02 19:26:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/search_attributes_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1119 2024-05-02 19:26:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/search_attributes_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.348229 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      564 2024-05-03 14:59:12.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.348229 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/password_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/start_login_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/start_login_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/authentication/token_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.348229 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_edit_get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/delete_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/edit_event_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/get_all_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/get_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/index_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/index_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/publish_event_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/search_events_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/search_events_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/events/unpublish_event_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/cache_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/create_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/get_feed_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/toggle_feed_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/update_feed_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/galaxy_schema.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/noticelists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/noticelists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      747 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      578 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/create_object_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1505 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/get_object_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/search_objects_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/organisations/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/organisations/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/organisations/organisation.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/roles/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/roles/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/roles/role.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.352229 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/create_sighting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/get_sighting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/standard_status_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/create_tag_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/delete_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/get_tag_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/search_tags_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/update_tag_body.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/users/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/users/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/users/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/users/users_view_me_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7189 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/warninglist_response.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.356229 mmisp_lib-0.1.4/src/mmisp/db/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/src/mmisp/db/config.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1099 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/src/mmisp/db/database.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.360229 mmisp_lib-0.1.4/src/mmisp/db/models/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3685 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/src/mmisp/db/models/attribute.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/auth_key.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2707 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/event.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1498 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/feed.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      858 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/galaxy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2456 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/galaxy_cluster.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      846 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/identity_provider.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      888 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/noticelist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1819 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/object.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      940 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/organisation.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1249 2024-05-05 20:35:54.000000 mmisp_lib-0.1.4/src/mmisp/db/models/role.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1495 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/server.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1727 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/sharing_group.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      829 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/sighting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      752 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/tag.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1434 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/taxonomy.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2068 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/user.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      997 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/user_setting.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1185 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/models/warninglist.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.4/src/mmisp/db/print_changes.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.360229 mmisp_lib-0.1.4/src/mmisp/lib/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/src/mmisp/lib/__init__.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53293 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/src/mmisp/lib/attributes.py
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2639 2024-05-05 20:35:54.000000 mmisp_lib-0.1.4/src/mmisp/lib/permissions.py
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.360229 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3076 2024-05-06 10:41:05.000000 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/PKG-INFO
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8689 2024-05-06 10:41:05.000000 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-06 10:41:05.000000 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-06 10:41:05.000000 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/requires.txt
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-06 10:41:05.000000 mmisp_lib-0.1.4/src/mmisp_lib.egg-info/top_level.txt
-drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-06 10:41:05.360229 mmisp_lib-0.1.4/tests/
--rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.4/tests/test_dummy.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.157064 mmisp_lib-0.1.5/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1076 2024-05-14 11:01:09.000000 mmisp_lib-0.1.5/LICENSE
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-16 15:46:31.157064 mmisp_lib-0.1.5/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2050 2024-04-18 07:49:23.000000 mmisp_lib-0.1.5/README.md
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      947 2024-05-16 15:42:06.000000 mmisp_lib-0.1.5/pyproject.toml
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       38 2024-05-16 15:46:31.157064 mmisp_lib-0.1.5/setup.cfg
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.141064 mmisp_lib-0.1.5/src/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.141064 mmisp_lib-0.1.5/src/mmisp/
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.141064 mmisp_lib-0.1.5/src/mmisp/api_schemas/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/__init__.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.141064 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1147 2024-05-14 16:15:10.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/add_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      755 2024-05-16 13:33:55.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/add_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      256 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/add_remove_tag_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      135 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/delete_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      226 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/delete_selected_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      216 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/delete_selected_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      675 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/edit_attribute_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      838 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/edit_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1163 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_all_attributes_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      901 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_attribute_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1486 2024-05-02 19:26:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      813 2024-05-02 19:26:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_describe_types_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      469 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/restore_attribute_reponse.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3225 2024-05-02 19:26:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/search_attributes_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1119 2024-05-02 19:26:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/search_attributes_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.145064 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      268 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/add_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      431 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/add_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      207 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/edit_auth_key_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      460 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/edit_auth_key_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      564 2024-05-03 14:59:12.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      603 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      567 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.145064 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       97 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/exchange_token_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      102 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/password_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       81 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/start_login_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      364 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/start_login_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       80 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/authentication/token_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.145064 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      310 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/FreeTextImportWorkerBody.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      273 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      277 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_attribute_via_free_text_import_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     5438 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_edit_get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      808 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      236 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_remove_tag_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      248 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/delete_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/edit_event_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2143 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/get_all_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      158 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/get_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      926 2024-05-02 10:34:56.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/index_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      881 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/index_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      247 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/publish_event_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1347 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/search_events_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/search_events_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      249 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/events/unpublish_event_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.145064 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      190 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/cache_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      924 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/create_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      164 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/enable_disable_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      128 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/fetch_feeds_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1234 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/get_feed_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      126 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/toggle_feed_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      893 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/update_feed_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.145064 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      229 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      179 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/attach_galaxy_cluster_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      238 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/delete_force_update_import_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      323 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/export_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1139 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/export_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      289 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/galaxy_schema.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      421 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/get_all_search_galaxies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      866 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/get_galaxy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      298 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/import_galaxies_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      514 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/search_galaxies_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/noticelists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/noticelists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      237 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/noticelists/get_all_noticelist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      747 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/noticelists/get_noticelist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      535 2024-05-14 12:28:31.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/create_object_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1526 2024-05-14 16:15:10.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/get_object_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1539 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/search_objects_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/organisations/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/organisations/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      583 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/organisations/organisation.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/roles/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/roles/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2980 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/roles/role.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      131 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      113 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/add_org_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      130 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      118 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/add_server_to_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      428 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/create_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      862 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      524 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      140 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/delete_sharing_group_legacy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1443 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1120 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      340 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      138 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/sharing_group_org.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      146 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/sharing_group_server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      357 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/update_sharing_group_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1062 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1084 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1487 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/create_sighting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      589 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/get_sighting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      230 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/standard_status_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      392 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/create_tag_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      156 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/delete_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      645 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/get_tag_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      690 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/search_tags_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      369 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/update_tag_body.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.149064 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      566 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      632 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      367 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/get_taxonomy_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      676 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      301 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/get_uid_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      232 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/get_user_settings_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      161 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/search_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      209 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/search_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       93 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/set_user_setting_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/set_user_setting_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/user_settings/view_user_setting_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/api_schemas/users/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/users/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      910 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/users/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      267 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/users/users_view_me_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      136 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/check_value_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      225 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/check_value_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     7189 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/create_warninglist_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      210 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/delete_warninglist_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      341 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/get_selected_all_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      183 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      191 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      204 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      952 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/warninglist_response.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/db/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      270 2024-04-30 12:43:28.000000 mmisp_lib-0.1.5/src/mmisp/db/config.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1099 2024-04-30 12:43:28.000000 mmisp_lib-0.1.5/src/mmisp/db/database.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      495 2024-05-14 23:46:30.000000 mmisp_lib-0.1.5/src/mmisp/db/mixins.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/db/models/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3699 2024-05-16 14:00:39.000000 mmisp_lib-0.1.5/src/mmisp/db/models/attribute.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      861 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/auth_key.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2707 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/event.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1498 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/feed.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      858 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/galaxy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2456 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/galaxy_cluster.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      846 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/identity_provider.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      888 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/noticelist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1819 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/object.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      989 2024-05-14 23:46:30.000000 mmisp_lib-0.1.5/src/mmisp/db/models/organisation.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1249 2024-05-14 11:01:09.000000 mmisp_lib-0.1.5/src/mmisp/db/models/role.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1495 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/server.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1798 2024-05-14 23:46:30.000000 mmisp_lib-0.1.5/src/mmisp/db/models/sharing_group.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      829 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/sighting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      752 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/tag.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1434 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/taxonomy.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2068 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/user.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      997 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/user_setting.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1185 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/models/warninglist.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     1181 2024-04-18 07:49:24.000000 mmisp_lib-0.1.5/src/mmisp/db/print_changes.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.153064 mmisp_lib-0.1.5/src/mmisp/lib/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        0 2024-04-30 12:43:28.000000 mmisp_lib-0.1.5/src/mmisp/lib/__init__.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)    53425 2024-05-16 13:28:29.000000 mmisp_lib-0.1.5/src/mmisp/lib/attributes.py
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     2639 2024-05-14 11:01:09.000000 mmisp_lib-0.1.5/src/mmisp/lib/permissions.py
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.157064 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     3098 2024-05-16 15:46:31.000000 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)     8720 2024-05-16 15:46:31.000000 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        1 2024-05-16 15:46:31.000000 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)      420 2024-05-16 15:46:31.000000 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/requires.txt
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)        6 2024-05-16 15:46:31.000000 mmisp_lib-0.1.5/src/mmisp_lib.egg-info/top_level.txt
+drwxr-xr-x   0 konstantin  (1000) konstantin  (1000)        0 2024-05-16 15:46:31.157064 mmisp_lib-0.1.5/tests/
+-rw-r--r--   0 konstantin  (1000) konstantin  (1000)       42 2024-04-30 12:43:28.000000 mmisp_lib-0.1.5/tests/test_dummy.py
```

### Comparing `mmisp_lib-0.1.4/PKG-INFO` & `mmisp_lib-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.4
+Version: 0.1.5
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: SQLAlchemy[asyncio]==1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: alembic==1.8.1
 Requires-Dist: aiomysql==0.2.0
```

### Comparing `mmisp_lib-0.1.4/README.md` & `mmisp_lib-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/pyproject.toml` & `mmisp_lib-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmisp-lib"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = []
 readme = "README.md"
 requires-python = ">=3.11.0"
 
 
 dependencies = [
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/add_attribute_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/create_feed_body.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-from typing import Any, Optional
+from pydantic import BaseModel, Field
 
-from pydantic import BaseModel, root_validator
 
-
-class AddAttributeBody(BaseModel):
-    type: str
-    value: Optional[str]
-    value1: Optional[str]
-    value2: str | None = None
-    event_id: str | None = None
-    object_id: str | None = None
-    object_relation: str | None = None
-    category: str | None = None
-    to_ids: bool | None = None
-    uuid: str | None = None
-    timestamp: str | None = None
+class FeedCreateBody(BaseModel):
+    name: str = Field(min_length=1)
+    provider: str = Field(min_length=1)
+    url: str = Field(min_length=1)
+    rules: str | None = None
+    enabled: bool | None = None
     distribution: str | None = None
     sharing_group_id: str | None = None
-    comment: str | None = None
-    deleted: bool | None = None
-    disable_correlation: bool | None = None
-    first_seen: str | None = None
-    last_seen: str | None = None
-
-    @root_validator
-    def ensure_value_or_value1_is_set(cls, data: dict[str, Any]) -> Optional[dict[str, Any]]:  # noqa: ANN101
-        required_values: list[str] = [str(data.get("value")), str(data.get("value1"))]
-        if all(item is None for item in required_values):
-            raise ValueError("value or value1 has to be set")
-        return data
+    tag_id: str | None = None
+    default: bool | None = None
+    source_format: str | None = None
+    fixed_event: bool | None = None
+    delta_merge: bool | None = None
+    event_id: str | None = None
+    publish: bool | None = None
+    override_ids: bool | None = None
+    settings: str | None = None
+    input_source: str | None = None
+    delete_local_file: bool | None = None
+    lookup_visible: bool | None = None
+    headers: str | None = None
+    caching_enabled: bool | None = None
+    force_to_ids: bool | None = None
+    orgc_id: str | None = None
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/add_attribute_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_attribute_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
-class AddAttributeAttributes(BaseModel):
+class GetAttributeTag(BaseModel):
+    id: str
+    name: str
+    colour: str
+    numerical_value: int | None = None
+    is_galaxy: bool
+    local: bool
+
+
+class GetAttributeAttributes(BaseModel):
     id: str
     event_id: str
     object_id: str
     object_relation: Optional[str] = Field(..., nullable=True)
     category: str
     type: str
     value: str
-    value1: str
-    value2: str
     to_ids: bool
     uuid: str
     timestamp: str
     distribution: str
     sharing_group_id: str
-    comment: str
+    comment: str | None = None
     deleted: bool
     disable_correlation: bool
     first_seen: Optional[str] = Field(..., nullable=True)
     last_seen: Optional[str] = Field(..., nullable=True)
-    attribute_tag: list[str] = Field([], alias="AttributeTag")
+    event_uuid: str
+    tag: list[GetAttributeTag] | None = None
 
 
-class AddAttributeResponse(BaseModel):
-    Attribute: AddAttributeAttributes
+class GetAttributeResponse(BaseModel):
+    Attribute: GetAttributeAttributes
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/edit_attribute_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/edit_attribute_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/edit_attributes_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/edit_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_all_attributes_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_all_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_attribute_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/export_galaxies_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-from typing import Optional
+from pydantic import BaseModel
 
-from pydantic import BaseModel, Field
+from mmisp.api_schemas.events.add_edit_get_event_response import AddEditGetEventGalaxyClusterRelation
+from mmisp.api_schemas.events.get_all_events_response import GetAllEventsGalaxyClusterGalaxy
+from mmisp.api_schemas.organisations.organisation import Organisation
 
 
-class GetAttributeTag(BaseModel):
-    id: str
-    name: str
-    colour: str
-    numerical_value: int | None = None
-    is_galaxy: bool
-    local: bool
+class ExportGalaxyGalaxyElement(BaseModel):
+    id: str | None = None
+    galaxy_cluster_id: str | None = None
+    key: str
+    value: str
 
 
-class GetAttributeAttributes(BaseModel):
+class ExportGalaxyClusterResponse(BaseModel):
     id: str
-    event_id: str
-    object_id: str
-    object_relation: Optional[str] = Field(..., nullable=True)
-    category: str
+    uuid: str
+    collection_uuid: str
     type: str
     value: str
-    to_ids: bool
-    uuid: str
-    timestamp: str
+    tag_name: str
+    description: str
+    galaxy_id: str
+    source: str
+    authors: list[str]
+    version: str
     distribution: str
     sharing_group_id: str
-    comment: str | None = None
+    org_id: str
+    orgc_id: str
+    default: bool
+    locked: bool
+    extends_uuid: str
+    extends_version: str
+    published: bool
     deleted: bool
-    disable_correlation: bool
-    first_seen: Optional[str] = Field(..., nullable=True)
-    last_seen: Optional[str] = Field(..., nullable=True)
-    event_uuid: str
-    tag: list[GetAttributeTag] | None = None
-
-
-class GetAttributeResponse(BaseModel):
-    Attribute: GetAttributeAttributes
+    GalaxyElement: list[ExportGalaxyGalaxyElement]
+    Galaxy: GetAllEventsGalaxyClusterGalaxy
+    GalaxyClusterRelation: list[AddEditGetEventGalaxyClusterRelation] = []
+    Org: Organisation
+    Orgc: Organisation
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_attribute_statistics_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/get_describe_types_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/get_describe_types_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/search_attributes_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/search_attributes_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/attributes/search_attributes_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/attributes/search_attributes_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/search_auth_keys_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/search_get_all_auth_keys_users_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/auth_keys/view_auth_key_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_edit_get_event_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_edit_get_event_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/add_event_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/add_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/edit_event_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/edit_event_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/get_all_events_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/get_all_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/index_events_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/index_events_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/index_events_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/index_events_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/events/search_events_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/events/search_events_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/create_feed_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/search_objects_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,49 @@
-from pydantic import BaseModel, Field
+from typing import Any
 
+from pydantic import BaseModel, validator
 
-class FeedCreateBody(BaseModel):
-    name: str = Field(min_length=1)
-    provider: str = Field(min_length=1)
-    url: str = Field(min_length=1)
-    rules: str | None = None
-    enabled: bool | None = None
-    distribution: str | None = None
-    sharing_group_id: str | None = None
-    tag_id: str | None = None
-    default: bool | None = None
-    source_format: str | None = None
-    fixed_event: bool | None = None
-    delta_merge: bool | None = None
+
+class ObjectSearchBody(BaseModel):
+    object_name: str | None = None
+    object_template_uuid: str | None = None
+    object_template_version: str | None = None
     event_id: str | None = None
-    publish: bool | None = None
-    override_ids: bool | None = None
-    settings: str | None = None
-    input_source: str | None = None
-    delete_local_file: bool | None = None
-    lookup_visible: bool | None = None
-    headers: str | None = None
-    caching_enabled: bool | None = None
-    force_to_ids: bool | None = None
-    orgc_id: str | None = None
+    category: str | None = None
+    comment: str | None = None
+    first_seen: str | None = None
+    last_seen: str | None = None
+    quick_filter: str | None = None
+    timestamp: str | None = None
+    event_info: str | None = None
+    from_: str | None = None  # 'from' is a reserved word in Python, so an underscore is added
+    to: str | None = None
+    date: str | None = None
+    last: str | None = None
+    event_timestamp: str | None = None
+    org_id: str | None = None
+    uuid: str | None = None
+    value1: str | None = None
+    value2: str | None = None
+    type: str | None = None
+    object_relation: str | None = None
+    attribute_timestamp: str | None = None
+    to_ids: bool | None = None
+    published: bool | None = None
+    deleted: bool | None = None
+    return_format: str | None = "json"
+    limit: str | None = "25"
+
+    @validator("limit")
+    def check_limit(cls, value: Any) -> str:  # noqa: ANN101
+        if value:
+            try:
+                limit_int = int(value)
+            except ValueError:
+                raise ValueError("'limit' must be a valid integer")
+
+            if not 1 <= limit_int <= 500:
+                raise ValueError("'limit' must be between 1 and 500")
+        return value
 
     class Config:
         orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/get_feed_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/get_feed_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/feeds/update_feed_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/feeds/update_feed_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/get_galaxy_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/get_galaxy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/galaxies/search_galaxies_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/galaxies/search_galaxies_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/noticelists/get_noticelist_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/noticelists/get_noticelist_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/create_object_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/create_object_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,10 +10,7 @@
     distribution: str | None = None
     sharing_group_id: str = Field(min_length=1)
     comment: str = Field(min_length=1)
     deleted: bool | None = None
     first_seen: str | None = None
     last_seen: str | None = None
     Attribute: list[AddAttributeBody] | None = None
-
-    class Config:
-        orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/objects/get_object_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/objects/get_object_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
 from mmisp.api_schemas.attributes.get_all_attributes_response import GetAllAttributesResponse
 from mmisp.api_schemas.events.get_event_response import ObjectEventResponse
 
 
 class ObjectWithAttributesResponse(BaseModel):
     id: str
@@ -18,33 +18,30 @@
     timestamp: str | None = None
     distribution: str | None = None
     sharing_group_id: str | None = None
     comment: str | None = None
     deleted: bool | None = None
     first_seen: str | None = None
     last_seen: str | None = None
-    Attribute: list[GetAllAttributesResponse] | None = None
+    attributes: list[GetAllAttributesResponse] | None = Field(alias="Attribute", default=None)
     Event: ObjectEventResponse | None = None
 
     @validator("sharing_group_id", always=True)
     def check_sharing_group_id(cls, value: Any, values: Dict[str, Any]) -> Optional[int]:  # noqa: ANN101
         """
         If distribution equals 4, sharing_group_id will be shown.
         """
         distribution = values.get("distribution", None)
         if distribution == "4" and value is not None:
             return value
         return None
 
+    class Config:
+        allow_population_by_field_name = True
+
 
 class ObjectResponse(BaseModel):
     Object: ObjectWithAttributesResponse
 
-    class Config:
-        orm_mode = True
-
 
 class ObjectSearchResponse(BaseModel):
     response: list[ObjectResponse]
-
-    class Config:
-        orm_mode = True
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/organisations/organisation.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/organisations/organisation.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/roles/role.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/roles/role.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/create_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/get_all_sharing_groups_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/get_sharing_group_info_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/update_sharing_group_legacy_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sharing_groups/view_update_sharing_group_legacy_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/create_sighting_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/create_sighting_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/sightings/get_sighting_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/sightings/get_sighting_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/get_tag_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/get_tag_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/tags/search_tags_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/tags/search_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/export_taxonomies_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/get_taxonomy_by_id_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/taxonomies/get_taxonomy_tags_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/users/user.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/users/user.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/create_warninglist_body.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/create_warninglist_body.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/api_schemas/warninglists/warninglist_response.py` & `mmisp_lib-0.1.5/src/mmisp/api_schemas/warninglists/warninglist_response.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/database.py` & `mmisp_lib-0.1.5/src/mmisp/db/database.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/attribute.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/attribute.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 from typing import Self, Type
 
-from sqlalchemy import BigInteger, Boolean, Column, ForeignKey, Integer, String, Text, inspect
+from sqlalchemy import BigInteger, Boolean, Column, ForeignKey, Integer, String, Text
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.decl_api import DeclarativeMeta
 
+from mmisp.db.mixins import DictMixin
 from mmisp.lib.attributes import categories, default_category, mapper_safe_clsname_val, to_ids
 from mmisp.util.uuid import uuid
 
 from ..database import Base
 from .event import Event
 from .tag import Tag
 
 
-class DictMixin:
-    def asdict(self: Self) -> dict:
-        d = {}
-        for key in self.__mapper__.c.keys():
-            if not key.startswith("_"):
-                d[key] = getattr(self, key)
-
-        for key, prop in inspect(self.__class__).all_orm_descriptors.items():
-            if isinstance(prop, hybrid_property):
-                d[key] = getattr(self, key)
-        return d
-
-
 class Attribute(Base, DictMixin):
     __tablename__ = "attributes"
 
     id = Column(Integer, primary_key=True, nullable=False)
     uuid = Column(String(40), unique=True, default=uuid, index=True)
     event_id = Column(Integer, ForeignKey("events.id", ondelete="CASCADE"), nullable=False, index=True)
     object_id = Column(Integer, nullable=False, default=0, index=True)
@@ -46,14 +34,25 @@
     deleted = Column(Boolean, nullable=False, default=False)
     disable_correlation = Column(Boolean, nullable=False, default=False)
     first_seen = Column(BigInteger, index=True)
     last_seen = Column(BigInteger, index=True)
 
     event = relationship("Event", back_populates="attributes", lazy="joined")
 
+    __mapper_args__ = {"polymorphic_on": "type"}
+
+    def __init__(self: Self, *arg, **kwargs) -> None:
+        if kwargs["value1"] is None:
+            split_val = kwargs["value"].split("|", 1)
+            kwargs["value1"] = split_val[0]
+            if len(split_val) == 2:
+                kwargs["value2"] = split_val[1]
+
+        super().__init__(*arg, **kwargs)
+
     @property
     def event_uuid(self: "Attribute") -> str:
         return self.event.uuid
 
     @hybrid_property
     def value(self: Self) -> str:
         if self.value2 == "":
@@ -79,14 +78,14 @@
 
 
 class AttributeMeta(DeclarativeMeta):
     def __new__(cls: Type[type], clsname: str, bases: tuple, dct: dict) -> "AttributeMeta":
         key = clsname[len("Attribute") :]
         dct["default_category"] = default_category[mapper_safe_clsname_val[key]]
         dct["categories"] = categories[mapper_safe_clsname_val[key]]
-        dct["to_ids"] = to_ids[mapper_safe_clsname_val[key]]
+        dct["default_to_ids"] = to_ids[mapper_safe_clsname_val[key]]
         dct["__mapper_args__"] = {"polymorphic_identity": mapper_safe_clsname_val[key]}
         return super().__new__(cls, clsname, bases, dct)
 
 
 for k, _ in mapper_safe_clsname_val.items():
     vars()["Attribute" + k] = AttributeMeta("Attribute" + k, (Attribute,), dict())
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/auth_key.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/auth_key.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/event.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/event.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/feed.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/feed.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/galaxy.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/galaxy.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/galaxy_cluster.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/galaxy_cluster.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/identity_provider.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/identity_provider.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/noticelist.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/noticelist.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/object.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/object.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/organisation.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/organisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 
 from sqlalchemy import Boolean, Column, DateTime, Integer, String, Text
 
+from mmisp.db.mixins import DictMixin
 from mmisp.util.uuid import uuid
 
 from ..database import Base
 
 
-class Organisation(Base):
+class Organisation(Base, DictMixin):
     __tablename__ = "organisations"
 
     id = Column(Integer, primary_key=True, nullable=False)
     name = Column(String(255), nullable=False, unique=True)
     date_created = Column(DateTime, default=datetime.utcnow, nullable=False)
     date_modified = Column(DateTime, default=datetime.utcnow, onupdate=datetime.utcnow, nullable=False)
     description = Column(Text)
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/role.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/role.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/server.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/server.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/sharing_group.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/sharing_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from datetime import datetime
 
 from sqlalchemy import Boolean, Column, DateTime, Integer, String, Text
 
+from mmisp.db.mixins import DictMixin
 from mmisp.util.uuid import uuid
 
 from ..database import Base
 
 
-class SharingGroup(Base):
+class SharingGroup(Base, DictMixin):
     __tablename__ = "sharing_groups"
 
     id = Column(Integer, primary_key=True, nullable=False)
     name = Column(String(255), nullable=False, unique=True)
     releasability = Column(Text, nullable=False)
     description = Column(Text, nullable=False, default="")
     uuid = Column(String(40), unique=True, default=uuid, nullable=False)
@@ -21,23 +22,23 @@
     active = Column(Boolean, nullable=False, default=False)
     created = Column(DateTime, default=datetime.utcnow, nullable=False)
     modified = Column(DateTime, default=datetime.utcnow, onupdate=datetime.utcnow, nullable=False)
     local = Column(Boolean, nullable=False, default=True)
     roaming = Column(Boolean, default=False, nullable=False)
 
 
-class SharingGroupOrg(Base):
+class SharingGroupOrg(Base, DictMixin):
     __tablename__ = "sharing_group_orgs"
 
     id = Column(Integer, primary_key=True, nullable=False)
     sharing_group_id = Column(Integer, index=True, nullable=False)
     org_id = Column(Integer, index=True, nullable=False)
     extend = Column(Boolean, default=False, nullable=False)
 
 
-class SharingGroupServer(Base):
+class SharingGroupServer(Base, DictMixin):
     __tablename__ = "sharing_group_servers"
 
     id = Column(Integer, primary_key=True, nullable=False)
     sharing_group_id = Column(Integer, index=True, nullable=False)
     server_id = Column(Integer, index=True, nullable=False)
     all_orgs = Column(Boolean, index=True, nullable=False, default=False)
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/sighting.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/sighting.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/tag.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/tag.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/taxonomy.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/taxonomy.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/user.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/user.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/user_setting.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/user_setting.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/models/warninglist.py` & `mmisp_lib-0.1.5/src/mmisp/db/models/warninglist.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/db/print_changes.py` & `mmisp_lib-0.1.5/src/mmisp/db/print_changes.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp/lib/attributes.py` & `mmisp_lib-0.1.5/src/mmisp/lib/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
-from enum import Enum
+from enum import StrEnum
+from typing import Literal, Union
 
 
-class AttributeCategories(Enum):
+class AttributeCategories(StrEnum):
     PAYLOAD_DELIVERY = "Payload delivery"
     ARTIFACTS_DROPPED = "Artifacts dropped"
     PAYLOAD_INSTALLATION = "Payload installation"
     EXTERNAL_ANALYSIS = "External analysis"
     PERSISTENCE_MECHANISM = "Persistence mechanism"
     NETWORK_ACTIVITY = "Network activity"
     ATTRIBUTION = "Attribution"
@@ -209,15 +210,15 @@
     "x509-fingerprint-sha1": "X509FingerprintSha1",
     "x509-fingerprint-sha256": "X509FingerprintSha256",
     "xmr": "Xmr",
     "yara": "Yara",
 }
 
 mapper_safe_clsname_val = dict((v, k) for k, v in mapper_val_safe_clsname.items())
-
+literal_valid_attribute_types = Union[*[Literal[k] for k in mapper_val_safe_clsname.keys()]]
 
 default_category = {
     "md5": AttributeCategories.PAYLOAD_DELIVERY,
     "sha1": AttributeCategories.PAYLOAD_DELIVERY,
     "sha256": AttributeCategories.PAYLOAD_DELIVERY,
     "filename": AttributeCategories.PAYLOAD_DELIVERY,
     "pdb": AttributeCategories.ARTIFACTS_DROPPED,
```

### Comparing `mmisp_lib-0.1.4/src/mmisp/lib/permissions.py` & `mmisp_lib-0.1.5/src/mmisp/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `mmisp_lib-0.1.4/src/mmisp_lib.egg-info/PKG-INFO` & `mmisp_lib-0.1.5/src/mmisp_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: mmisp-lib
-Version: 0.1.4
+Version: 0.1.5
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: fastapi==0.104.1
 Requires-Dist: SQLAlchemy[asyncio]==1.4.46
 Requires-Dist: pydantic==1.10.13
 Requires-Dist: uvicorn==0.24.0.post1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: alembic==1.8.1
 Requires-Dist: aiomysql==0.2.0
```

### Comparing `mmisp_lib-0.1.4/src/mmisp_lib.egg-info/SOURCES.txt` & `mmisp_lib-0.1.5/src/mmisp_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 src/mmisp/api_schemas/__init__.py
 src/mmisp/api_schemas/standard_status_response.py
 src/mmisp/api_schemas/attributes/__init__.py
 src/mmisp/api_schemas/attributes/add_attribute_body.py
 src/mmisp/api_schemas/attributes/add_attribute_response.py
@@ -130,14 +131,15 @@
 src/mmisp/api_schemas/warninglists/get_selected_warninglists_body.py
 src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_body.py
 src/mmisp/api_schemas/warninglists/toggle_enable_warninglists_response.py
 src/mmisp/api_schemas/warninglists/warninglist_response.py
 src/mmisp/db/__init__.py
 src/mmisp/db/config.py
 src/mmisp/db/database.py
+src/mmisp/db/mixins.py
 src/mmisp/db/print_changes.py
 src/mmisp/db/models/__init__.py
 src/mmisp/db/models/attribute.py
 src/mmisp/db/models/auth_key.py
 src/mmisp/db/models/event.py
 src/mmisp/db/models/feed.py
 src/mmisp/db/models/galaxy.py
```

