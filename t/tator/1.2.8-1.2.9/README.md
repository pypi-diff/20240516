# Comparing `tmp/tator-1.2.8.tar.gz` & `tmp/tator-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tator-1.2.8.tar", last modified: Tue May  7 16:51:31 2024, max compression
+gzip compressed data, was "tator-1.2.9.tar", last modified: Mon May 13 02:29:36 2024, max compression
```

## Comparing `tator-1.2.8.tar` & `tator-1.2.9.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.627840 tator-1.2.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2024-05-07 16:42:39.000000 tator-1.2.8/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-07 16:51:31.627840 tator-1.2.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2024-05-07 16:42:39.000000 tator-1.2.8/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2024-05-07 16:42:39.000000 tator-1.2.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-07 16:51:31.627840 tator-1.2.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3752 2024-05-07 16:42:39.000000 tator-1.2.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.583840 tator-1.2.8/tator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2024-05-07 16:42:39.000000 tator-1.2.8/tator/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.587840 tator-1.2.8/tator/extractor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:42:39.000000 tator-1.2.8/tator/extractor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2024-05-07 16:42:39.000000 tator-1.2.8/tator/extractor/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2024-05-07 16:42:39.000000 tator-1.2.8/tator/extractor/env_launcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12298 2024-05-07 16:42:39.000000 tator-1.2.8/tator/extractor/extractor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.587840 tator-1.2.8/tator/openapi/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2024-05-07 16:42:39.000000 tator-1.2.8/tator/openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.587840 tator-1.2.8/tator/openapi/tator_openapi/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12670 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.587840 tator-1.2.8/tator/openapi/tator_openapi/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  2015800 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/api/tator_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.611840 tator-1.2.8/tator/openapi/tator_openapi/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12080 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8289 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/affiliation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/affiliation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/affiliation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/algorithm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_manifest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_parameter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/announcement.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/applet.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/applet_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/archive_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10923 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_filter_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12585 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_operation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14330 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15184 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/audio_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6819 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/autocomplete_service.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bad_request_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bookmark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bookmark_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bookmark_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2024-05-07 16:51:27.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_gcp_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_oci_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_s3_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/bucket_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/change_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/change_log_description_of_change.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/clone_media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/color_map.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/concat_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/create_list_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/create_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/credentials.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/download_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/download_info_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/email_attachment_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/email_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/encode_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/favorite.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/favorite_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/favorite_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/feed_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/file_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/fill.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/float_array_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/generic_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/generic_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/get_cloned_media_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/image_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/invitation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/invitation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/invitation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job_cluster.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job_cluster_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job_node.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_suggestion.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/leaf_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/live_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/live_update_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10180 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/localization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18930 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_files.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_next.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_prev.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15998 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_stats.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/media_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/membership_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/membership_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/message_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/multi_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/not_found_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/notify_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/organization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/organization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/organization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/password_reset_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/project.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/project_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/project_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/resolution_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/s3_storage_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8248 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/section.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7300 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/section_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/section_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11740 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_merge_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_trim_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/state_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/temporary_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/temporary_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/transcode.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10987 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/transcode_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/upload_completion_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/upload_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/upload_part.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/user_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9465 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/user_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/version_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/version_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/video_clip.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10920 2024-05-07 16:51:28.000000 tator-1.2.8/tator/openapi/tator_openapi/models/video_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13483 2024-05-07 16:51:30.000000 tator-1.2.8/tator/openapi/tator_openapi/rest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.611840 tator-1.2.8/tator/transcode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7730 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/black.mp4
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/create_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/delete_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9452 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/determine_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/make_fragment_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5922 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/make_thumbnails.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/prepare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19361 2024-05-07 16:42:39.000000 tator-1.2.8/tator/transcode/transcode.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.619840 tator-1.2.8/tator/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2061 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/_download_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7264 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/_upload_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2119 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/chunked_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/chunked_file_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4482 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_leaf_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7453 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_localization_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11130 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_media_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6572 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_state_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/concat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/download_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/download_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/find_single_change.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/full_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/get_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/get_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3224 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/get_paginator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1371 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/get_parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1732 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/live_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/md5sum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17899 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8461 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/multi_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/register_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/register_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3512 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/tator-symbol.gif
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/tator-symbol.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/to_dataframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/update_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/upload_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2008 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/upload_generic_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/upload_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2024-05-07 16:42:39.000000 tator-1.2.8/tator/util/upload_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2024-05-07 16:42:39.000000 tator-1.2.8/tator/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.587840 tator-1.2.8/tator.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-07 16:51:31.000000 tator-1.2.8/tator.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11849 2024-05-07 16:51:31.000000 tator-1.2.8/tator.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-07 16:51:31.000000 tator-1.2.8/tator.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      144 2024-05-07 16:51:31.000000 tator-1.2.8/tator.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2024-05-07 16:51:31.000000 tator-1.2.8/tator.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-07 16:51:31.627840 tator-1.2.8/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4892 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_a_float_array.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_algorithm_launch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_archive_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6437 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_attribute_type_addition.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_attribute_type_deletion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_attribute_type_mutation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_attributes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23752 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_change_log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4174 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_chunked_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7222 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_collection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13655 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_file_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_get_clip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_getframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_job_cancel.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_job_cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_leaf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3031 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_local_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9223 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_localization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_localization_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10371 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4902 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_poly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_project_thumbnail.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9537 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_stategraphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_tracks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5369 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_util_media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_util_media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2024-05-07 16:42:39.000000 tator-1.2.8/test/test_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:36.017160 tator-1.2.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2024-05-13 02:19:40.000000 tator-1.2.9/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-13 02:29:36.013160 tator-1.2.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2024-05-13 02:19:40.000000 tator-1.2.9/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2024-05-13 02:19:40.000000 tator-1.2.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-13 02:29:36.017160 tator-1.2.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3752 2024-05-13 02:19:40.000000 tator-1.2.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.973159 tator-1.2.9/tator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2024-05-13 02:19:40.000000 tator-1.2.9/tator/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.977159 tator-1.2.9/tator/extractor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:19:40.000000 tator-1.2.9/tator/extractor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2024-05-13 02:19:40.000000 tator-1.2.9/tator/extractor/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2024-05-13 02:19:40.000000 tator-1.2.9/tator/extractor/env_launcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12298 2024-05-13 02:19:40.000000 tator-1.2.9/tator/extractor/extractor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.977159 tator-1.2.9/tator/openapi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2024-05-13 02:19:40.000000 tator-1.2.9/tator/openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.977159 tator-1.2.9/tator/openapi/tator_openapi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12670 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.977159 tator-1.2.9/tator/openapi/tator_openapi/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  2015800 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/api/tator_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:36.001160 tator-1.2.9/tator/openapi/tator_openapi/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12080 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8289 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/affiliation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/affiliation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/affiliation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/algorithm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_manifest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_parameter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/announcement.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/applet.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/applet_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/archive_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10923 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_filter_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12585 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_operation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14330 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15184 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/audio_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6819 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/autocomplete_service.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bad_request_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bookmark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bookmark_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bookmark_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_gcp_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_oci_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_s3_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/bucket_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/change_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/change_log_description_of_change.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/clone_media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/color_map.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/concat_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/create_list_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/create_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/download_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/download_info_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/email_attachment_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/encode_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/favorite.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/favorite_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/favorite_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/feed_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/file_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/fill.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/float_array_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/generic_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/generic_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/get_cloned_media_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/image_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/invitation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/invitation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/invitation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job_cluster.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job_cluster_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job_node.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_suggestion.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/leaf_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/live_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/live_update_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10180 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/localization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18930 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_files.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_next.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_prev.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15998 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_stats.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/media_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/membership_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/membership_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/message_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/multi_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/not_found_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/notify_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2024-05-13 02:29:32.000000 tator-1.2.9/tator/openapi/tator_openapi/models/organization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/organization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/organization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/password_reset_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/project.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/project_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/project_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/resolution_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/s3_storage_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8248 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/section.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7300 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/section_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/section_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11740 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_merge_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_trim_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/state_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/temporary_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/temporary_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/transcode.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10987 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/transcode_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/upload_completion_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/upload_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/upload_part.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/user_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9465 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/user_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/version_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/version_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/video_clip.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10920 2024-05-13 02:29:33.000000 tator-1.2.9/tator/openapi/tator_openapi/models/video_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13483 2024-05-13 02:29:34.000000 tator-1.2.9/tator/openapi/tator_openapi/rest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:36.001160 tator-1.2.9/tator/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7730 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/black.mp4
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/create_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/delete_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9452 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/determine_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/make_fragment_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5922 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/make_thumbnails.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/prepare.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19361 2024-05-13 02:19:40.000000 tator-1.2.9/tator/transcode/transcode.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:36.009160 tator-1.2.9/tator/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2061 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/_download_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7264 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/_upload_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2119 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/chunked_file_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4482 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_leaf_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7453 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_localization_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11130 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_media_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6572 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_state_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/concat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/download_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/download_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/find_single_change.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/full_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1405 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/get_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/get_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3224 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/get_paginator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1371 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/get_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1732 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/live_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/md5sum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17899 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8461 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/multi_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/register_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/register_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3512 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/tator-symbol.gif
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/tator-symbol.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/to_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/update_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/upload_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2008 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/upload_generic_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/upload_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2024-05-13 02:19:40.000000 tator-1.2.9/tator/util/upload_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2024-05-13 02:19:40.000000 tator-1.2.9/tator/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:35.977159 tator-1.2.9/tator.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2024-05-13 02:29:35.000000 tator-1.2.9/tator.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11849 2024-05-13 02:29:35.000000 tator-1.2.9/tator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-13 02:29:35.000000 tator-1.2.9/tator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      144 2024-05-13 02:29:35.000000 tator-1.2.9/tator.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2024-05-13 02:29:35.000000 tator-1.2.9/tator.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-13 02:29:36.013160 tator-1.2.9/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4892 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_a_float_array.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_algorithm_launch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_archive_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6437 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_attribute_type_addition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_attribute_type_deletion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_attribute_type_mutation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_attributes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23752 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_change_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4174 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7222 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_collection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13655 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_file_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_get_clip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_getframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_job_cancel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_job_cluster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_leaf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3031 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_local_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9223 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_localization_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10371 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1524 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4902 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_poly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_project_thumbnail.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9537 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_stategraphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_tracks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5369 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_util_media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_util_media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2024-05-13 02:19:40.000000 tator-1.2.9/test/test_version.py
```

### Comparing `tator-1.2.8/README.md` & `tator-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/setup.py` & `tator-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/__init__.py` & `tator-1.2.9/tator/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/extractor/__main__.py` & `tator-1.2.9/tator/extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/extractor/env_launcher.py` & `tator-1.2.9/tator/extractor/env_launcher.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/extractor/extractor.py` & `tator-1.2.9/tator/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/__init__.py` & `tator-1.2.9/tator/openapi/tator_openapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 # import apis into sdk package
 from tator.openapi.tator_openapi.api.tator_api import TatorApi
 
 # import ApiClient
 from tator.openapi.tator_openapi.api_client import ApiClient
 from tator.openapi.tator_openapi.configuration import Configuration
```

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/api/tator_api.py` & `tator-1.2.9/tator/openapi/tator_openapi/api/tator_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/api_client.py` & `tator-1.2.9/tator/openapi/tator_openapi/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.2.8/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/configuration.py` & `tator-1.2.9/tator/openapi/tator_openapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.2.8".\
+               "SDK Package Version: 1.2.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/exceptions.py` & `tator-1.2.9/tator/openapi/tator_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/__init__.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/affiliation.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/affiliation.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/affiliation_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/affiliation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/affiliation_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/affiliation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/algorithm.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_manifest.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_manifest.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_parameter.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_parameter.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/algorithm_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/announcement.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/announcement.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/applet.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/applet_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/applet_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/archive_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/archive_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_combinator_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_combinator_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_filter_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_filter_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_operation_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_operation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_delete.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/audio_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/audio_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/autocomplete_service.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/autocomplete_service.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/auxiliary_file_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/auxiliary_file_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bad_request_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bookmark.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bookmark_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bookmark_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bookmark_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bookmark_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_gcp_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_gcp_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_oci_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_oci_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_oci_native_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_oci_native_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_s3_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_s3_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/bucket_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/change_log.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/change_log_description_of_change.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/change_log_description_of_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/clone_media_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/clone_media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/color_map.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/color_map.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/concat_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/concat_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/create_list_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/create_list_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/create_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/create_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/credentials.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/credentials.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/download_info.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/download_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/download_info_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/download_info_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/email_attachment_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/email_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/email_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/encode_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/encode_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/favorite.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/favorite.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/favorite_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/favorite_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/favorite_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/favorite_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/feed_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/feed_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/file_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/file_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/fill.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/fill.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/float_array_query.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/float_array_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/generic_file.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/generic_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/generic_file_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/generic_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/get_cloned_media_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/get_cloned_media_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/image_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/image_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/invitation.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/invitation.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/invitation_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/invitation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/invitation_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/invitation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job_cluster.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job_cluster_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job_node.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job_node.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_bulk_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_id_query.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_suggestion.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_suggestion.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/leaf_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/leaf_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/live_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/live_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/live_update_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/live_update_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_bulk_delete.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_bulk_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_delete.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_id_query.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/localization_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/localization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_bulk_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_files.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_files.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_id_query.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_next.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_next.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_prev.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_prev.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_stats.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_stats.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/media_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/media_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/membership.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/membership_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/membership_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/membership_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/membership_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/message_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/message_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/multi_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/multi_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/not_found_response.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/not_found_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/notify_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/notify_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/organization.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/organization.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/organization_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/organization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/organization_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/password_reset_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/password_reset_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/project.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/project.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/project_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/project_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/project_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/project_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/resolution_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/resolution_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/s3_storage_config.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/s3_storage_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/section.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/section.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/section_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/section_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/section_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/section_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_bulk_delete.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_bulk_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_delete.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_id_query.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_merge_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_merge_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_trim_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_trim_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_type.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_type_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_type_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/state_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/state_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/temporary_file.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/temporary_file_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/temporary_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/token.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/token.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/transcode.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/transcode_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/transcode_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/upload_completion_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/upload_completion_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/upload_info.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/upload_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/upload_part.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/upload_part.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/user.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/user.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/user_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/user_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/user_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/user_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/version.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/version.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/version_spec.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/version_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/version_update.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/version_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/video_clip.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/video_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/models/video_definition.py` & `tator-1.2.9/tator/openapi/tator_openapi/models/video_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/openapi/tator_openapi/rest.py` & `tator-1.2.9/tator/openapi/tator_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/__main__.py` & `tator-1.2.9/tator/transcode/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/black.mp4` & `tator-1.2.9/tator/transcode/black.mp4`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/create_media.py` & `tator-1.2.9/tator/transcode/create_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/delete_media.py` & `tator-1.2.9/tator/transcode/delete_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/determine_transcode.py` & `tator-1.2.9/tator/transcode/determine_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/make_fragment_info.py` & `tator-1.2.9/tator/transcode/make_fragment_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/make_thumbnails.py` & `tator-1.2.9/tator/transcode/make_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/prepare.py` & `tator-1.2.9/tator/transcode/prepare.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/transcode/transcode.py` & `tator-1.2.9/tator/transcode/transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/__init__.py` & `tator-1.2.9/tator/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/_download_file.py` & `tator-1.2.9/tator/util/_download_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/_upload_file.py` & `tator-1.2.9/tator/util/_upload_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/chunked_create.py` & `tator-1.2.9/tator/util/chunked_create.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/chunked_file_list.py` & `tator-1.2.9/tator/util/chunked_file_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_leaf_list.py` & `tator-1.2.9/tator/util/clone_leaf_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_leaf_type.py` & `tator-1.2.9/tator/util/clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_localization_list.py` & `tator-1.2.9/tator/util/clone_localization_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_localization_type.py` & `tator-1.2.9/tator/util/clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_media_list.py` & `tator-1.2.9/tator/util/clone_media_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_media_type.py` & `tator-1.2.9/tator/util/clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_membership.py` & `tator-1.2.9/tator/util/clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_section.py` & `tator-1.2.9/tator/util/clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_state_list.py` & `tator-1.2.9/tator/util/clone_state_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_state_type.py` & `tator-1.2.9/tator/util/clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/clone_version.py` & `tator-1.2.9/tator/util/clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/concat.py` & `tator-1.2.9/tator/util/concat.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/download_attachment.py` & `tator-1.2.9/tator/util/download_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/download_media.py` & `tator-1.2.9/tator/util/download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/download_temporary_file.py` & `tator-1.2.9/tator/util/download_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/find_single_change.py` & `tator-1.2.9/tator/util/find_single_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/full_state_graphic.py` & `tator-1.2.9/tator/util/full_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/get_api.py` & `tator-1.2.9/tator/util/get_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/get_images.py` & `tator-1.2.9/tator/util/get_images.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/get_paginator.py` & `tator-1.2.9/tator/util/get_paginator.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/get_parser.py` & `tator-1.2.9/tator/util/get_parser.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/import_media.py` & `tator-1.2.9/tator/util/import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/live_stream.py` & `tator-1.2.9/tator/util/live_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/md5sum.py` & `tator-1.2.9/tator/util/md5sum.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/media_manipulation.py` & `tator-1.2.9/tator/util/media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/media_util.py` & `tator-1.2.9/tator/util/media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/multi_stream.py` & `tator-1.2.9/tator/util/multi_stream.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/register_algorithm.py` & `tator-1.2.9/tator/util/register_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/register_applet.py` & `tator-1.2.9/tator/util/register_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/tator-symbol.gif` & `tator-1.2.9/tator/util/tator-symbol.gif`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/tator-symbol.png` & `tator-1.2.9/tator/util/tator-symbol.png`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/to_dataframe.py` & `tator-1.2.9/tator/util/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/update_applet.py` & `tator-1.2.9/tator/util/update_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/upload_attachment.py` & `tator-1.2.9/tator/util/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/upload_generic_file.py` & `tator-1.2.9/tator/util/upload_generic_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/upload_media.py` & `tator-1.2.9/tator/util/upload_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator/util/upload_temporary_file.py` & `tator-1.2.9/tator/util/upload_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/tator.egg-info/SOURCES.txt` & `tator-1.2.9/tator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_a_float_array.py` & `tator-1.2.9/test/test_a_float_array.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_algorithm.py` & `tator-1.2.9/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_algorithm_launch.py` & `tator-1.2.9/test/test_algorithm_launch.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_applet.py` & `tator-1.2.9/test/test_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_archive_date.py` & `tator-1.2.9/test/test_archive_date.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_attachment.py` & `tator-1.2.9/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_attribute_type_addition.py` & `tator-1.2.9/test/test_attribute_type_addition.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_attribute_type_deletion.py` & `tator-1.2.9/test/test_attribute_type_deletion.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_attribute_type_mutation.py` & `tator-1.2.9/test/test_attribute_type_mutation.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_attributes.py` & `tator-1.2.9/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_change_log.py` & `tator-1.2.9/test/test_change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_chunked_create.py` & `tator-1.2.9/test/test_chunked_create.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_leaf_type.py` & `tator-1.2.9/test/test_clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_localization_type.py` & `tator-1.2.9/test/test_clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_media.py` & `tator-1.2.9/test/test_clone_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_media_type.py` & `tator-1.2.9/test/test_clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_membership.py` & `tator-1.2.9/test/test_clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_section.py` & `tator-1.2.9/test/test_clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_state_type.py` & `tator-1.2.9/test/test_clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_clone_version.py` & `tator-1.2.9/test/test_clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_collection.py` & `tator-1.2.9/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_download_media.py` & `tator-1.2.9/test/test_download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_extract.py` & `tator-1.2.9/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_file.py` & `tator-1.2.9/test/test_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_file_type.py` & `tator-1.2.9/test/test_file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_get_clip.py` & `tator-1.2.9/test/test_get_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_getframe.py` & `tator-1.2.9/test/test_getframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_import_media.py` & `tator-1.2.9/test/test_import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_job_cancel.py` & `tator-1.2.9/test/test_job_cancel.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_job_cluster.py` & `tator-1.2.9/test/test_job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_leaf.py` & `tator-1.2.9/test/test_leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_leaf_type.py` & `tator-1.2.9/test/test_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_local_transcode.py` & `tator-1.2.9/test/test_local_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_localization.py` & `tator-1.2.9/test/test_localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_localization_graphic.py` & `tator-1.2.9/test/test_localization_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_localization_type.py` & `tator-1.2.9/test/test_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_media.py` & `tator-1.2.9/test/test_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_media_type.py` & `tator-1.2.9/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_multi.py` & `tator-1.2.9/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_pagination.py` & `tator-1.2.9/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_poly.py` & `tator-1.2.9/test/test_poly.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_search.py` & `tator-1.2.9/test/test_search.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_state.py` & `tator-1.2.9/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_state_graphic.py` & `tator-1.2.9/test/test_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_state_type.py` & `tator-1.2.9/test/test_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_stategraphic.py` & `tator-1.2.9/test/test_stategraphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_temporary_file.py` & `tator-1.2.9/test/test_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_tracks.py` & `tator-1.2.9/test/test_tracks.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_transcode.py` & `tator-1.2.9/test/test_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_util_media_manipulation.py` & `tator-1.2.9/test/test_util_media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_util_media_util.py` & `tator-1.2.9/test/test_util_media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.2.8/test/test_version.py` & `tator-1.2.9/test/test_version.py`

 * *Files identical despite different names*

