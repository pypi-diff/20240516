# Comparing `tmp/graphlit_client-1.0.20240509002.tar.gz` & `tmp/graphlit_client-1.0.20240515001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240509002.tar", last modified: Fri May 10 05:57:55 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240515001.tar", last modified: Thu May 16 04:23:12 2024, max compression
```

## Comparing `graphlit_client-1.0.20240509002.tar` & `graphlit_client-1.0.20240515001.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 05:57:55.281996 graphlit_client-1.0.20240509002/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-10 05:57:55.281996 graphlit_client-1.0.20240509002/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 05:57:55.253994 graphlit_client-1.0.20240509002/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 05:57:55.277996 graphlit_client-1.0.20240509002/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    84570 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/count_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17117 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7153 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_share_point_consent_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5193 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7962 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    79384 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68105 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3382 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/publish_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_categories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10533 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11920 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_contents_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_contents_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_events.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7957 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_labels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_microsoft_teams_channels.py
--rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_microsoft_teams_teams.py
--rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_one_drive_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_organizations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_persons.py
--rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_places.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_products.py
--rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_repos.py
--rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_share_point_folders.py
--rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_share_point_libraries.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_softwares.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5666 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1502 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8940 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_category.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_event.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_label.py
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_observation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_organization.py
--rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_person.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_place.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_product.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_repo.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_software.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8528 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/graphlit_api/update_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 05:57:55.277996 graphlit_client-1.0.20240509002/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-10 05:57:55.000000 graphlit_client-1.0.20240509002/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-10 05:57:55.000000 graphlit_client-1.0.20240509002/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-10 05:57:55.000000 graphlit_client-1.0.20240509002/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-10 05:57:55.000000 graphlit_client-1.0.20240509002/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-10 05:57:55.000000 graphlit_client-1.0.20240509002/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-10 05:57:55.281996 graphlit_client-1.0.20240509002/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-10 05:57:38.000000 graphlit_client-1.0.20240509002/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 04:23:12.107588 graphlit_client-1.0.20240515001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-16 04:23:12.107588 graphlit_client-1.0.20240515001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 04:23:12.075586 graphlit_client-1.0.20240515001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1878 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 04:23:12.103588 graphlit_client-1.0.20240515001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    86024 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    99668 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      416 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      362 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      392 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      354 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      440 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      400 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/count_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      477 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      450 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      506 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17547 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      408 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9869 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4286 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1383 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7153 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      387 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1164 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1119 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      763 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1045 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      438 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_share_point_consent_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5777 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8029 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      804 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      790 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    80762 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1711 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68874 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2390 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1024 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1094 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      954 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/publish_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_categories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10738 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12137 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_contents_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_contents_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4895 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1004 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1576 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_events.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7957 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      553 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_labels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      834 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_microsoft_teams_channels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      782 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_microsoft_teams_teams.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      718 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_one_drive_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1399 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_organizations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1318 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_persons.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      956 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_places.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1250 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_products.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      592 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_repos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      807 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_share_point_folders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_share_point_libraries.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_softwares.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1645 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9007 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_category.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_event.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_label.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_observation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_organization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      366 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_person.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_place.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_product.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_repo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_software.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8595 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/graphlit_api/update_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-16 04:23:12.107588 graphlit_client-1.0.20240515001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-05-16 04:23:12.000000 graphlit_client-1.0.20240515001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5861 2024-05-16 04:23:12.000000 graphlit_client-1.0.20240515001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-16 04:23:12.000000 graphlit_client-1.0.20240515001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-05-16 04:23:12.000000 graphlit_client-1.0.20240515001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-05-16 04:23:12.000000 graphlit_client-1.0.20240515001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-16 04:23:12.107588 graphlit_client-1.0.20240515001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-05-16 04:22:53.000000 graphlit_client-1.0.20240515001/setup.py
```

### Comparing `graphlit_client-1.0.20240509002/LICENSE` & `graphlit_client-1.0.20240515001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/PKG-INFO` & `graphlit_client-1.0.20240515001/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240509002
+Version: 1.0.20240515001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240509002/README.md` & `graphlit_client-1.0.20240515001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit/graphlit.py` & `graphlit_client-1.0.20240515001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/__init__.py` & `graphlit_client-1.0.20240515001/graphlit_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
     FacetValueTypes,
     FeedConnectorTypes,
     FeedListingTypes,
     FeedServiceTypes,
     FeedTypes,
     FilePreparationServiceTypes,
     FileTypes,
+    GraphStrategyTypes,
     GroqModels,
     H3ResolutionTypes,
     ImageProjectionTypes,
     IntegrationServiceTypes,
     LabelFacetTypes,
     LinkTypes,
     MailImportance,
@@ -230,14 +231,15 @@
     MistralModels,
     ModelServiceTypes,
     NotionTypes,
     ObservableTypes,
     OccurrenceTypes,
     OpenAIModels,
     OpenAIVisionDetailLevels,
+    OperationTypes,
     OrderByTypes,
     OrderDirectionTypes,
     OrganizationFacetTypes,
     OrientationTypes,
     PersonFacetTypes,
     PlaceFacetTypes,
     PolicyTimeTypes,
@@ -245,14 +247,15 @@
     PromptStrategyTypes,
     RenditionTypes,
     ReplicateModels,
     RepoFacetTypes,
     RerankingModelServiceTypes,
     ResourceConnectorTypes,
     RetrievalStrategyTypes,
+    RevisionStrategyTypes,
     SearchQueryTypes,
     SearchTypes,
     SharePointAuthenticationTypes,
     SiteTypes,
     SoftwareFacetTypes,
     SpecificationTypes,
     SummarizationTypes,
@@ -321,14 +324,15 @@
     GetContentContentIssue,
     GetContentContentLinks,
     GetContentContentLocation,
     GetContentContentObservations,
     GetContentContentObservationsObservable,
     GetContentContentObservationsOccurrences,
     GetContentContentObservationsOccurrencesBoundingBox,
+    GetContentContentObservationsRelated,
     GetContentContentOwner,
     GetContentContentPackage,
     GetContentContentPages,
     GetContentContentPagesChunks,
     GetContentContentParent,
     GetContentContentSegments,
     GetContentContentVideo,
@@ -406,20 +410,22 @@
 from .get_software import GetSoftware, GetSoftwareSoftware
 from .get_specification import (
     GetSpecification,
     GetSpecificationSpecification,
     GetSpecificationSpecificationAnthropic,
     GetSpecificationSpecificationAzureOpenAi,
     GetSpecificationSpecificationCohere,
+    GetSpecificationSpecificationGraphStrategy,
     GetSpecificationSpecificationOpenAi,
     GetSpecificationSpecificationOwner,
     GetSpecificationSpecificationPromptStrategy,
     GetSpecificationSpecificationReplicate,
     GetSpecificationSpecificationRerankingStrategy,
     GetSpecificationSpecificationRetrievalStrategy,
+    GetSpecificationSpecificationRevisionStrategy,
     GetSpecificationSpecificationStrategy,
     GetSpecificationSpecificationTools,
 )
 from .get_workflow import (
     GetWorkflow,
     GetWorkflowWorkflow,
     GetWorkflowWorkflowActions,
@@ -543,14 +549,16 @@
     GitHubIssuesFeedPropertiesUpdateInput,
     GoogleDriveFeedPropertiesInput,
     GoogleDriveFeedPropertiesUpdateInput,
     GoogleEmailFeedPropertiesInput,
     GoogleEmailFeedPropertiesUpdateInput,
     GoogleFeedPropertiesInput,
     GoogleFeedPropertiesUpdateInput,
+    GraphStrategyInput,
+    GraphStrategyUpdateInput,
     GroqModelPropertiesInput,
     GroqModelPropertiesUpdateInput,
     H3Filter,
     H3IndexFilter,
     ImageMetadataInput,
     IngestionContentFilterInput,
     IngestionWorkflowStageInput,
@@ -629,14 +637,16 @@
     RepoFilter,
     RepoInput,
     RepoUpdateInput,
     RerankingStrategyInput,
     RerankingStrategyUpdateInput,
     RetrievalStrategyInput,
     RetrievalStrategyUpdateInput,
+    RevisionStrategyInput,
+    RevisionStrategyUpdateInput,
     RSSFeedPropertiesInput,
     RSSFeedPropertiesUpdateInput,
     ShapeMetadataInput,
     SharePointFeedPropertiesInput,
     SharePointFeedPropertiesUpdateInput,
     SharePointFoldersInput,
     SharePointLibrariesInput,
@@ -840,14 +850,17 @@
     PromptConversation,
     PromptConversationPromptConversation,
     PromptConversationPromptConversationConversation,
     PromptConversationPromptConversationFacets,
     PromptConversationPromptConversationFacetsObservable,
     PromptConversationPromptConversationFacetsObservableObservable,
     PromptConversationPromptConversationFacetsRange,
+    PromptConversationPromptConversationGraph,
+    PromptConversationPromptConversationGraphEdges,
+    PromptConversationPromptConversationGraphNodes,
     PromptConversationPromptConversationMessage,
     PromptConversationPromptConversationMessageCitations,
     PromptConversationPromptConversationMessageCitationsContent,
 )
 from .prompt_specifications import (
     PromptSpecifications,
     PromptSpecificationsPromptSpecifications,
@@ -923,14 +936,15 @@
     QueryContentsContentsResultsIssue,
     QueryContentsContentsResultsLinks,
     QueryContentsContentsResultsLocation,
     QueryContentsContentsResultsObservations,
     QueryContentsContentsResultsObservationsObservable,
     QueryContentsContentsResultsObservationsOccurrences,
     QueryContentsContentsResultsObservationsOccurrencesBoundingBox,
+    QueryContentsContentsResultsObservationsRelated,
     QueryContentsContentsResultsOwner,
     QueryContentsContentsResultsPackage,
     QueryContentsContentsResultsPages,
     QueryContentsContentsResultsPagesChunks,
     QueryContentsContentsResultsParent,
     QueryContentsContentsResultsSegments,
     QueryContentsContentsResultsVideo,
@@ -959,14 +973,15 @@
     QueryContentsFacetsContentsResultsIssue,
     QueryContentsFacetsContentsResultsLinks,
     QueryContentsFacetsContentsResultsLocation,
     QueryContentsFacetsContentsResultsObservations,
     QueryContentsFacetsContentsResultsObservationsObservable,
     QueryContentsFacetsContentsResultsObservationsOccurrences,
     QueryContentsFacetsContentsResultsObservationsOccurrencesBoundingBox,
+    QueryContentsFacetsContentsResultsObservationsRelated,
     QueryContentsFacetsContentsResultsOwner,
     QueryContentsFacetsContentsResultsPackage,
     QueryContentsFacetsContentsResultsPages,
     QueryContentsFacetsContentsResultsPagesChunks,
     QueryContentsFacetsContentsResultsParent,
     QueryContentsFacetsContentsResultsSegments,
     QueryContentsFacetsContentsResultsVideo,
@@ -1094,20 +1109,22 @@
 from .query_specifications import (
     QuerySpecifications,
     QuerySpecificationsSpecifications,
     QuerySpecificationsSpecificationsResults,
     QuerySpecificationsSpecificationsResultsAnthropic,
     QuerySpecificationsSpecificationsResultsAzureOpenAi,
     QuerySpecificationsSpecificationsResultsCohere,
+    QuerySpecificationsSpecificationsResultsGraphStrategy,
     QuerySpecificationsSpecificationsResultsOpenAi,
     QuerySpecificationsSpecificationsResultsOwner,
     QuerySpecificationsSpecificationsResultsPromptStrategy,
     QuerySpecificationsSpecificationsResultsReplicate,
     QuerySpecificationsSpecificationsResultsRerankingStrategy,
     QuerySpecificationsSpecificationsResultsRetrievalStrategy,
+    QuerySpecificationsSpecificationsResultsRevisionStrategy,
     QuerySpecificationsSpecificationsResultsStrategy,
     QuerySpecificationsSpecificationsResultsTools,
 )
 from .query_usage import QueryUsage, QueryUsageUsage
 from .query_workflows import (
     QueryWorkflows,
     QueryWorkflowsWorkflows,
@@ -1689,14 +1706,15 @@
     "GetContentContentIssue",
     "GetContentContentLinks",
     "GetContentContentLocation",
     "GetContentContentObservations",
     "GetContentContentObservationsObservable",
     "GetContentContentObservationsOccurrences",
     "GetContentContentObservationsOccurrencesBoundingBox",
+    "GetContentContentObservationsRelated",
     "GetContentContentOwner",
     "GetContentContentPackage",
     "GetContentContentPages",
     "GetContentContentPagesChunks",
     "GetContentContentParent",
     "GetContentContentSegments",
     "GetContentContentVideo",
@@ -1773,20 +1791,22 @@
     "GetSoftware",
     "GetSoftwareSoftware",
     "GetSpecification",
     "GetSpecificationSpecification",
     "GetSpecificationSpecificationAnthropic",
     "GetSpecificationSpecificationAzureOpenAi",
     "GetSpecificationSpecificationCohere",
+    "GetSpecificationSpecificationGraphStrategy",
     "GetSpecificationSpecificationOpenAi",
     "GetSpecificationSpecificationOwner",
     "GetSpecificationSpecificationPromptStrategy",
     "GetSpecificationSpecificationReplicate",
     "GetSpecificationSpecificationRerankingStrategy",
     "GetSpecificationSpecificationRetrievalStrategy",
+    "GetSpecificationSpecificationRevisionStrategy",
     "GetSpecificationSpecificationStrategy",
     "GetSpecificationSpecificationTools",
     "GetWorkflow",
     "GetWorkflowWorkflow",
     "GetWorkflowWorkflowActions",
     "GetWorkflowWorkflowActionsConnector",
     "GetWorkflowWorkflowActionsConnectorSlack",
@@ -1824,14 +1844,17 @@
     "GoogleFeedPropertiesInput",
     "GoogleFeedPropertiesUpdateInput",
     "GraphQLClientError",
     "GraphQLClientGraphQLError",
     "GraphQLClientGraphQLMultiError",
     "GraphQLClientHttpError",
     "GraphQLClientInvalidResponseError",
+    "GraphStrategyInput",
+    "GraphStrategyTypes",
+    "GraphStrategyUpdateInput",
     "GroqModelPropertiesInput",
     "GroqModelPropertiesUpdateInput",
     "GroqModels",
     "H3Filter",
     "H3IndexFilter",
     "H3ResolutionTypes",
     "INGEST_ENCODED_FILE_GQL",
@@ -1911,14 +1934,15 @@
     "OneDriveFeedPropertiesUpdateInput",
     "OneDriveFoldersInput",
     "OpenAIImageExtractionPropertiesInput",
     "OpenAIModelPropertiesInput",
     "OpenAIModelPropertiesUpdateInput",
     "OpenAIModels",
     "OpenAIVisionDetailLevels",
+    "OperationTypes",
     "OrderByTypes",
     "OrderDirectionTypes",
     "OrganizationFacetInput",
     "OrganizationFacetTypes",
     "OrganizationFilter",
     "OrganizationInput",
     "OrganizationUpdateInput",
@@ -1957,14 +1981,17 @@
     "PromptConversation",
     "PromptConversationPromptConversation",
     "PromptConversationPromptConversationConversation",
     "PromptConversationPromptConversationFacets",
     "PromptConversationPromptConversationFacetsObservable",
     "PromptConversationPromptConversationFacetsObservableObservable",
     "PromptConversationPromptConversationFacetsRange",
+    "PromptConversationPromptConversationGraph",
+    "PromptConversationPromptConversationGraphEdges",
+    "PromptConversationPromptConversationGraphNodes",
     "PromptConversationPromptConversationMessage",
     "PromptConversationPromptConversationMessageCitations",
     "PromptConversationPromptConversationMessageCitationsContent",
     "PromptSpecifications",
     "PromptSpecificationsPromptSpecifications",
     "PromptSpecificationsPromptSpecificationsMessages",
     "PromptSpecificationsPromptSpecificationsMessagesCitations",
@@ -2052,14 +2079,15 @@
     "QueryContentsContentsResultsIssue",
     "QueryContentsContentsResultsLinks",
     "QueryContentsContentsResultsLocation",
     "QueryContentsContentsResultsObservations",
     "QueryContentsContentsResultsObservationsObservable",
     "QueryContentsContentsResultsObservationsOccurrences",
     "QueryContentsContentsResultsObservationsOccurrencesBoundingBox",
+    "QueryContentsContentsResultsObservationsRelated",
     "QueryContentsContentsResultsOwner",
     "QueryContentsContentsResultsPackage",
     "QueryContentsContentsResultsPages",
     "QueryContentsContentsResultsPagesChunks",
     "QueryContentsContentsResultsParent",
     "QueryContentsContentsResultsSegments",
     "QueryContentsContentsResultsVideo",
@@ -2086,14 +2114,15 @@
     "QueryContentsFacetsContentsResultsIssue",
     "QueryContentsFacetsContentsResultsLinks",
     "QueryContentsFacetsContentsResultsLocation",
     "QueryContentsFacetsContentsResultsObservations",
     "QueryContentsFacetsContentsResultsObservationsObservable",
     "QueryContentsFacetsContentsResultsObservationsOccurrences",
     "QueryContentsFacetsContentsResultsObservationsOccurrencesBoundingBox",
+    "QueryContentsFacetsContentsResultsObservationsRelated",
     "QueryContentsFacetsContentsResultsOwner",
     "QueryContentsFacetsContentsResultsPackage",
     "QueryContentsFacetsContentsResultsPages",
     "QueryContentsFacetsContentsResultsPagesChunks",
     "QueryContentsFacetsContentsResultsParent",
     "QueryContentsFacetsContentsResultsSegments",
     "QueryContentsFacetsContentsResultsVideo",
@@ -2196,20 +2225,22 @@
     "QuerySoftwaresSoftwaresResults",
     "QuerySpecifications",
     "QuerySpecificationsSpecifications",
     "QuerySpecificationsSpecificationsResults",
     "QuerySpecificationsSpecificationsResultsAnthropic",
     "QuerySpecificationsSpecificationsResultsAzureOpenAi",
     "QuerySpecificationsSpecificationsResultsCohere",
+    "QuerySpecificationsSpecificationsResultsGraphStrategy",
     "QuerySpecificationsSpecificationsResultsOpenAi",
     "QuerySpecificationsSpecificationsResultsOwner",
     "QuerySpecificationsSpecificationsResultsPromptStrategy",
     "QuerySpecificationsSpecificationsResultsReplicate",
     "QuerySpecificationsSpecificationsResultsRerankingStrategy",
     "QuerySpecificationsSpecificationsResultsRetrievalStrategy",
+    "QuerySpecificationsSpecificationsResultsRevisionStrategy",
     "QuerySpecificationsSpecificationsResultsStrategy",
     "QuerySpecificationsSpecificationsResultsTools",
     "QueryUsage",
     "QueryUsageUsage",
     "QueryWorkflows",
     "QueryWorkflowsWorkflows",
     "QueryWorkflowsWorkflowsResults",
@@ -2261,14 +2292,17 @@
     "RerankingModelServiceTypes",
     "RerankingStrategyInput",
     "RerankingStrategyUpdateInput",
     "ResourceConnectorTypes",
     "RetrievalStrategyInput",
     "RetrievalStrategyTypes",
     "RetrievalStrategyUpdateInput",
+    "RevisionStrategyInput",
+    "RevisionStrategyTypes",
+    "RevisionStrategyUpdateInput",
     "SUGGEST_CONVERSATION_GQL",
     "SUMMARIZE_CONTENTS_GQL",
     "SearchQueryTypes",
     "SearchTypes",
     "ShapeMetadataInput",
     "SharePointAuthenticationTypes",
     "SharePointFeedPropertiesInput",
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240515001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240515001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/base_model.py` & `graphlit_client-1.0.20240515001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/client.py` & `graphlit_client-1.0.20240515001/graphlit_api/client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240515001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240515001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240515001/graphlit_api/create_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
 
 class CreateWorkflowCreateWorkflowExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
+    extracted_count: Optional[int] = Field(alias="extractedCount")
     azure_text: Optional[
         "CreateWorkflowCreateWorkflowExtractionJobsConnectorAzureText"
     ] = Field(alias="azureText")
     azure_image: Optional[
         "CreateWorkflowCreateWorkflowExtractionJobsConnectorAzureImage"
     ] = Field(alias="azureImage")
     open_ai_image: Optional[
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240515001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/delete_all_organizations.py` & `graphlit_client-1.0.20240515001/graphlit_api/delete_all_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/delete_all_specifications.py` & `graphlit_client-1.0.20240515001/graphlit_api/delete_all_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/enums.py` & `graphlit_client-1.0.20240515001/graphlit_api/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,14 +478,26 @@
 
 class RerankingModelServiceTypes(str, Enum):
     COHERE = "COHERE"
     JINA = "JINA"
     PONGO = "PONGO"
 
 
+class GraphStrategyTypes(str, Enum):
+    EXTRACT_ENTITIES_FILTER = "EXTRACT_ENTITIES_FILTER"
+    EXTRACT_ENTITIES_GRAPH = "EXTRACT_ENTITIES_GRAPH"
+    NONE = "NONE"
+
+
+class RevisionStrategyTypes(str, Enum):
+    REVISE = "REVISE"
+    CUSTOM = "CUSTOM"
+    NONE = "NONE"
+
+
 class OpenAIModels(str, Enum):
     GPT35_TURBO = "GPT35_TURBO"
     GPT35_TURBO_0613 = "GPT35_TURBO_0613"
     GPT35_TURBO_16K = "GPT35_TURBO_16K"
     GPT35_TURBO_16K_0613 = "GPT35_TURBO_16K_0613"
     GPT35_TURBO_16K_1106 = "GPT35_TURBO_16K_1106"
     GPT35_TURBO_16K_0125 = "GPT35_TURBO_16K_0125"
@@ -495,14 +507,16 @@
     GPT4_TURBO_128K_1106 = "GPT4_TURBO_128K_1106"
     GPT4_TURBO_128K_0125 = "GPT4_TURBO_128K_0125"
     GPT4_TURBO_128K_20240409 = "GPT4_TURBO_128K_20240409"
     GPT4_TURBO_VISION_128K = "GPT4_TURBO_VISION_128K"
     GPT4_TURBO_VISION_128K_1106 = "GPT4_TURBO_VISION_128K_1106"
     GPT4_32K = "GPT4_32K"
     GPT4_32K_0613 = "GPT4_32K_0613"
+    GPT4O_128K_20240513 = "GPT4O_128K_20240513"
+    GPT4O_128K = "GPT4O_128K"
     CUSTOM = "CUSTOM"
 
 
 class AzureOpenAIModels(str, Enum):
     GPT35_TURBO_16K = "GPT35_TURBO_16K"
     GPT4 = "GPT4"
     GPT4_TURBO_128K = "GPT4_TURBO_128K"
@@ -727,13 +741,18 @@
     REPO = "REPO"
     SITE = "SITE"
     SOFTWARE = "SOFTWARE"
     SPECIFICATION = "SPECIFICATION"
     WORKFLOW = "WORKFLOW"
 
 
+class OperationTypes(str, Enum):
+    QUERY = "QUERY"
+    MUTATION = "MUTATION"
+
+
 class RepoFacetTypes(str, Enum):
     CREATION_DATE = "CREATION_DATE"
 
 
 class SoftwareFacetTypes(str, Enum):
     CREATION_DATE = "CREATION_DATE"
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240515001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240515001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_content.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,23 +242,30 @@
     link_type: Optional[LinkTypes] = Field(alias="linkType")
 
 
 class GetContentContentObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "GetContentContentObservationsObservable"
+    related: Optional["GetContentContentObservationsRelated"]
+    relation: Optional[str]
     occurrences: Optional[List[Optional["GetContentContentObservationsOccurrences"]]]
     state: EntityState
 
 
 class GetContentContentObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
+class GetContentContentObservationsRelated(BaseModel):
+    id: str
+    name: Optional[str]
+
+
 class GetContentContentObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
     page_index: Optional[int] = Field(alias="pageIndex")
     bounding_box: Optional["GetContentContentObservationsOccurrencesBoundingBox"] = (
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_event.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_event.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_organization.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_organization.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_person.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_person.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_place.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_place.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_product.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_product.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_project.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_software.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_software.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_specification.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from .enums import (
     AnthropicModels,
     AzureOpenAIModels,
     CohereModels,
     ConversationSearchTypes,
     ConversationStrategyTypes,
     EntityState,
+    GraphStrategyTypes,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
     RerankingModelServiceTypes,
     RetrievalStrategyTypes,
+    RevisionStrategyTypes,
     SpecificationTypes,
 )
 
 
 class GetSpecification(BaseModel):
     specification: Optional["GetSpecificationSpecification"]
 
@@ -46,14 +48,20 @@
     )
     retrieval_strategy: Optional["GetSpecificationSpecificationRetrievalStrategy"] = (
         Field(alias="retrievalStrategy")
     )
     reranking_strategy: Optional["GetSpecificationSpecificationRerankingStrategy"] = (
         Field(alias="rerankingStrategy")
     )
+    graph_strategy: Optional["GetSpecificationSpecificationGraphStrategy"] = Field(
+        alias="graphStrategy"
+    )
+    revision_strategy: Optional["GetSpecificationSpecificationRevisionStrategy"] = (
+        Field(alias="revisionStrategy")
+    )
     open_ai: Optional["GetSpecificationSpecificationOpenAi"] = Field(alias="openAI")
     azure_open_ai: Optional["GetSpecificationSpecificationAzureOpenAi"] = Field(
         alias="azureOpenAI"
     )
     cohere: Optional["GetSpecificationSpecificationCohere"]
     anthropic: Optional["GetSpecificationSpecificationAnthropic"]
     replicate: Optional["GetSpecificationSpecificationReplicate"]
@@ -82,14 +90,24 @@
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
 class GetSpecificationSpecificationRerankingStrategy(BaseModel):
     service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
+class GetSpecificationSpecificationGraphStrategy(BaseModel):
+    type: GraphStrategyTypes
+
+
+class GetSpecificationSpecificationRevisionStrategy(BaseModel):
+    type: RevisionStrategyTypes
+    custom_revision: Optional[str] = Field(alias="customRevision")
+    count: Optional[int]
+
+
 class GetSpecificationSpecificationOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240515001/graphlit_api/get_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
 
 class GetWorkflowWorkflowExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
+    extracted_count: Optional[int] = Field(alias="extractedCount")
     azure_text: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureText"] = Field(
         alias="azureText"
     )
     azure_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorAzureImage"] = (
         Field(alias="azureImage")
     )
     open_ai_image: Optional["GetWorkflowWorkflowExtractionJobsConnectorOpenAiImage"] = (
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240515001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240515001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240515001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/input_types.py` & `graphlit_client-1.0.20240515001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     EnvironmentTypes,
     EventFacetTypes,
     FeedListingTypes,
     FeedServiceTypes,
     FeedTypes,
     FilePreparationServiceTypes,
     FileTypes,
+    GraphStrategyTypes,
     GroqModels,
     H3ResolutionTypes,
     ImageProjectionTypes,
     IntegrationServiceTypes,
     LabelFacetTypes,
     LinkTypes,
     MailImportance,
@@ -61,14 +62,15 @@
     ProductFacetTypes,
     PromptStrategyTypes,
     ReplicateModels,
     RepoFacetTypes,
     RerankingModelServiceTypes,
     ResourceConnectorTypes,
     RetrievalStrategyTypes,
+    RevisionStrategyTypes,
     SearchQueryTypes,
     SearchTypes,
     SharePointAuthenticationTypes,
     SoftwareFacetTypes,
     SpecificationTypes,
     SummarizationTypes,
     TimedPolicyRecurrenceTypes,
@@ -545,14 +547,16 @@
     content: Optional["EntityReferenceInput"] = None
 
 
 class ObservationInput(BaseModel):
     content: "EntityReferenceInput"
     type: ObservableTypes
     observable: "NamedEntityReferenceInput"
+    related: Optional["NamedEntityReferenceInput"] = None
+    relation: Optional[str] = None
     occurrences: List["ObservationOccurrenceInput"]
 
 
 class OrganizationInput(BaseModel):
     name: str
     uri: Optional[Any] = None
     identifier: Optional[str] = None
@@ -656,14 +660,20 @@
     )
     retrieval_strategy: Optional["RetrievalStrategyInput"] = Field(
         alias="retrievalStrategy", default=None
     )
     reranking_strategy: Optional["RerankingStrategyInput"] = Field(
         alias="rerankingStrategy", default=None
     )
+    graph_strategy: Optional["GraphStrategyInput"] = Field(
+        alias="graphStrategy", default=None
+    )
+    revision_strategy: Optional["RevisionStrategyInput"] = Field(
+        alias="revisionStrategy", default=None
+    )
     tools: Optional[List["ToolDefinitionInput"]] = None
     open_ai: Optional["OpenAIModelPropertiesInput"] = Field(
         alias="openAI", default=None
     )
     azure_open_ai: Optional["AzureOpenAIModelPropertiesInput"] = Field(
         alias="azureOpenAI", default=None
     )
@@ -788,14 +798,16 @@
     content: Optional["EntityReferenceInput"] = None
 
 
 class ObservationUpdateInput(BaseModel):
     id: str
     type: Optional[ObservableTypes] = None
     observable: Optional["NamedEntityReferenceInput"] = None
+    related: Optional["NamedEntityReferenceInput"] = None
+    relation: Optional[str] = None
     occurrences: Optional[List["ObservationOccurrenceInput"]] = None
 
 
 class OrganizationUpdateInput(BaseModel):
     id: str
     name: Optional[str] = None
     uri: Optional[Any] = None
@@ -902,14 +914,20 @@
     )
     retrieval_strategy: Optional["RetrievalStrategyUpdateInput"] = Field(
         alias="retrievalStrategy", default=None
     )
     reranking_strategy: Optional["RerankingStrategyUpdateInput"] = Field(
         alias="rerankingStrategy", default=None
     )
+    graph_strategy: Optional["GraphStrategyUpdateInput"] = Field(
+        alias="graphStrategy", default=None
+    )
+    revision_strategy: Optional["RevisionStrategyUpdateInput"] = Field(
+        alias="revisionStrategy", default=None
+    )
     tools: Optional[List["ToolDefinitionUpdateInput"]] = None
     open_ai: Optional["OpenAIModelPropertiesUpdateInput"] = Field(
         alias="openAI", default=None
     )
     azure_open_ai: Optional["AzureOpenAIModelPropertiesUpdateInput"] = Field(
         alias="azureOpenAI", default=None
     )
@@ -1175,14 +1193,24 @@
     content_limit: Optional[int] = Field(alias="contentLimit", default=None)
 
 
 class RerankingStrategyInput(BaseModel):
     service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
+class GraphStrategyInput(BaseModel):
+    type: Optional[GraphStrategyTypes] = None
+
+
+class RevisionStrategyInput(BaseModel):
+    type: Optional[RevisionStrategyTypes] = None
+    custom_revision: Optional[str] = Field(alias="customRevision", default=None)
+    count: Optional[int] = None
+
+
 class ToolDefinitionInput(BaseModel):
     name: str
     description: Optional[str] = None
     schema_: str = Field(alias="schema")
     uri: Optional[Any] = None
 
 
@@ -1435,14 +1463,24 @@
 
 class RerankingStrategyUpdateInput(BaseModel):
     service_type: Optional[RerankingModelServiceTypes] = Field(
         alias="serviceType", default=None
     )
 
 
+class GraphStrategyUpdateInput(BaseModel):
+    type: Optional[GraphStrategyTypes] = None
+
+
+class RevisionStrategyUpdateInput(BaseModel):
+    type: Optional[RevisionStrategyTypes] = None
+    custom_revision: Optional[str] = Field(alias="customRevision", default=None)
+    count: Optional[int] = None
+
+
 class ToolDefinitionUpdateInput(BaseModel):
     name: Optional[str] = None
     description: Optional[str] = None
     schema_: Optional[str] = Field(alias="schema", default=None)
     uri: Optional[Any] = None
 
 
@@ -1791,14 +1829,15 @@
     content_types: Optional[List[ContentTypes]] = Field(
         alias="contentTypes", default=None
     )
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes", default=None)
     extracted_types: Optional[List[ObservableTypes]] = Field(
         alias="extractedTypes", default=None
     )
+    extracted_count: Optional[int] = Field(alias="extractedCount", default=None)
     azure_text: Optional["AzureTextExtractionPropertiesInput"] = Field(
         alias="azureText", default=None
     )
     azure_image: Optional["AzureImageExtractionPropertiesInput"] = Field(
         alias="azureImage", default=None
     )
     open_ai_image: Optional["OpenAIImageExtractionPropertiesInput"] = Field(
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240515001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240515001/graphlit_api/lookup_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Source: ./documents
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import BillableMetrics, ContentTypes, EntityTypes, FileTypes
+from .enums import BillableMetrics, ContentTypes, EntityTypes, FileTypes, OperationTypes
 
 
 class LookupUsage(BaseModel):
     lookup_usage: Optional[List[Optional["LookupUsageLookupUsage"]]] = Field(
         alias="lookupUsage"
     )
 
 
 class LookupUsageLookupUsage(BaseModel):
+    id: Optional[str]
     correlation_id: Optional[str] = Field(alias="correlationId")
     date: Any
     credits: Optional[Any]
     name: str
     metric: Optional[BillableMetrics]
     workflow: Optional[str]
     entity_type: Optional[EntityTypes] = Field(alias="entityType")
@@ -36,13 +37,15 @@
     processor_name: Optional[str] = Field(alias="processorName")
     prompt: Optional[str]
     prompt_tokens: Optional[int] = Field(alias="promptTokens")
     completion: Optional[str]
     completion_tokens: Optional[int] = Field(alias="completionTokens")
     tokens: Optional[int]
     count: Optional[int]
+    operation: Optional[str]
+    operation_type: Optional[OperationTypes] = Field(alias="operationType")
     request: Optional[str]
     variables: Optional[str]
     response: Optional[str]
 
 
 LookupUsage.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/operations.py` & `graphlit_client-1.0.20240515001/graphlit_api/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -842,14 +842,19 @@
     observations {
       id
       type
       observable {
         id
         name
       }
+      related {
+        id
+        name
+      }
+      relation
       occurrences {
         type
         confidence
         startTime
         endTime
         pageIndex
         boundingBox {
@@ -1216,14 +1221,19 @@
       observations {
         id
         type
         observable {
           id
           name
         }
+        related {
+          id
+          name
+        }
+        relation
         occurrences {
           type
           confidence
           startTime
           endTime
           pageIndex
           boundingBox {
@@ -1441,14 +1451,19 @@
       observations {
         id
         type
         observable {
           id
           name
         }
+        related {
+          id
+          name
+        }
+        relation
         occurrences {
           type
           confidence
           startTime
           endTime
           pageIndex
           boundingBox {
@@ -1768,14 +1783,26 @@
         type
         observable {
           id
           name
         }
       }
     }
+    graph {
+      nodes {
+        id
+        type
+        metadata
+      }
+      edges {
+        from
+        to
+        relation
+      }
+    }
   }
 }
 """
 
 PUBLISH_CONVERSATION_GQL = """
 mutation PublishConversation($id: ID!, $connector: ContentPublishingConnectorInput!, $name: String, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $correlationId: String) {
   publishConversation(
@@ -3054,14 +3081,15 @@
   }
 }
 """
 
 LOOKUP_USAGE_GQL = """
 query LookupUsage($correlationId: String!) {
   lookupUsage(correlationId: $correlationId) {
+    id
     correlationId
     date
     credits
     name
     metric
     workflow
     entityType
@@ -3078,14 +3106,16 @@
     processorName
     prompt
     promptTokens
     completion
     completionTokens
     tokens
     count
+    operation
+    operationType
     request
     variables
     response
   }
 }
 """
 
@@ -3106,14 +3136,15 @@
   }
 }
 """
 
 QUERY_USAGE_GQL = """
 query QueryUsage($startDate: DateTime!, $duration: TimeSpan!) {
   usage(startDate: $startDate, duration: $duration) {
+    id
     correlationId
     date
     credits
     name
     metric
     workflow
     entityType
@@ -3130,14 +3161,16 @@
     processorName
     prompt
     promptTokens
     completion
     completionTokens
     tokens
     count
+    operation
+    operationType
     request
     variables
     response
   }
 }
 """
 
@@ -3398,14 +3431,22 @@
     retrievalStrategy {
       type
       contentLimit
     }
     rerankingStrategy {
       serviceType
     }
+    graphStrategy {
+      type
+    }
+    revisionStrategy {
+      type
+      customRevision
+      count
+    }
     openAI {
       tokenLimit
       completionTokenLimit
       model
       key
       modelName
       temperature
@@ -3530,14 +3571,22 @@
       retrievalStrategy {
         type
         contentLimit
       }
       rerankingStrategy {
         serviceType
       }
+      graphStrategy {
+        type
+      }
+      revisionStrategy {
+        type
+        customRevision
+        count
+      }
       openAI {
         tokenLimit
         completionTokenLimit
         model
         key
         modelName
         temperature
@@ -3661,14 +3710,15 @@
     extraction {
       jobs {
         connector {
           type
           contentTypes
           fileTypes
           extractedTypes
+          extractedCount
           azureText {
             confidenceThreshold
             enablePII
           }
           azureImage {
             confidenceThreshold
           }
@@ -3803,14 +3853,15 @@
     extraction {
       jobs {
         connector {
           type
           contentTypes
           fileTypes
           extractedTypes
+          extractedCount
           azureText {
             confidenceThreshold
             enablePII
           }
           azureImage {
             confidenceThreshold
           }
@@ -3915,14 +3966,15 @@
       extraction {
         jobs {
           connector {
             type
             contentTypes
             fileTypes
             extractedTypes
+            extractedCount
             azureText {
               confidenceThreshold
               enablePII
             }
             azureImage {
               confidenceThreshold
             }
@@ -4023,14 +4075,15 @@
     extraction {
       jobs {
         connector {
           type
           contentTypes
           fileTypes
           extractedTypes
+          extractedCount
           azureText {
             confidenceThreshold
             enablePII
           }
           azureImage {
             confidenceThreshold
           }
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/prompt_conversation.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .base_model import BaseModel
 from .enums import (
     ContentFacetTypes,
     ContentTypes,
     ConversationRoleTypes,
     EntityState,
+    EntityTypes,
     FacetValueTypes,
     FileTypes,
     ModelServiceTypes,
     ObservableTypes,
 )
 
 
@@ -25,14 +26,15 @@
 
 
 class PromptConversationPromptConversation(BaseModel):
     conversation: Optional["PromptConversationPromptConversationConversation"]
     message: Optional["PromptConversationPromptConversationMessage"]
     message_count: Optional[int] = Field(alias="messageCount")
     facets: Optional[List[Optional["PromptConversationPromptConversationFacets"]]]
+    graph: Optional["PromptConversationPromptConversationGraph"]
 
 
 class PromptConversationPromptConversationConversation(BaseModel):
     id: str
 
 
 class PromptConversationPromptConversationMessage(BaseModel):
@@ -93,13 +95,31 @@
 
 
 class PromptConversationPromptConversationFacetsObservableObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
+class PromptConversationPromptConversationGraph(BaseModel):
+    nodes: Optional[List[Optional["PromptConversationPromptConversationGraphNodes"]]]
+    edges: Optional[List[Optional["PromptConversationPromptConversationGraphEdges"]]]
+
+
+class PromptConversationPromptConversationGraphNodes(BaseModel):
+    id: str
+    type: EntityTypes
+    metadata: Optional[str]
+
+
+class PromptConversationPromptConversationGraphEdges(BaseModel):
+    from_: str = Field(alias="from")
+    to: str
+    relation: Optional[str]
+
+
 PromptConversation.model_rebuild()
 PromptConversationPromptConversation.model_rebuild()
 PromptConversationPromptConversationMessage.model_rebuild()
 PromptConversationPromptConversationMessageCitations.model_rebuild()
 PromptConversationPromptConversationFacets.model_rebuild()
 PromptConversationPromptConversationFacetsObservable.model_rebuild()
+PromptConversationPromptConversationGraph.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240515001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240515001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/publish_text.py` & `graphlit_client-1.0.20240515001/graphlit_api/publish_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_categories.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_categories.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_contents.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,25 +248,32 @@
     link_type: Optional[LinkTypes] = Field(alias="linkType")
 
 
 class QueryContentsContentsResultsObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "QueryContentsContentsResultsObservationsObservable"
+    related: Optional["QueryContentsContentsResultsObservationsRelated"]
+    relation: Optional[str]
     occurrences: Optional[
         List[Optional["QueryContentsContentsResultsObservationsOccurrences"]]
     ]
     state: EntityState
 
 
 class QueryContentsContentsResultsObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
+class QueryContentsContentsResultsObservationsRelated(BaseModel):
+    id: str
+    name: Optional[str]
+
+
 class QueryContentsContentsResultsObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
     page_index: Optional[int] = Field(alias="pageIndex")
     bounding_box: Optional[
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_contents_facets.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_contents_facets.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,25 +255,32 @@
     link_type: Optional[LinkTypes] = Field(alias="linkType")
 
 
 class QueryContentsFacetsContentsResultsObservations(BaseModel):
     id: str
     type: ObservableTypes
     observable: "QueryContentsFacetsContentsResultsObservationsObservable"
+    related: Optional["QueryContentsFacetsContentsResultsObservationsRelated"]
+    relation: Optional[str]
     occurrences: Optional[
         List[Optional["QueryContentsFacetsContentsResultsObservationsOccurrences"]]
     ]
     state: EntityState
 
 
 class QueryContentsFacetsContentsResultsObservationsObservable(BaseModel):
     id: str
     name: Optional[str]
 
 
+class QueryContentsFacetsContentsResultsObservationsRelated(BaseModel):
+    id: str
+    name: Optional[str]
+
+
 class QueryContentsFacetsContentsResultsObservationsOccurrences(BaseModel):
     type: Optional[OccurrenceTypes]
     confidence: Optional[float]
     start_time: Optional[Any] = Field(alias="startTime")
     end_time: Optional[Any] = Field(alias="endTime")
     page_index: Optional[int] = Field(alias="pageIndex")
     bounding_box: Optional[
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_contents_graph.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_contents_graph.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_credits.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_events.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_events.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_labels.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_labels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_microsoft_teams_channels.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_microsoft_teams_channels.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_microsoft_teams_teams.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_microsoft_teams_teams.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_one_drive_folders.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_one_drive_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_organizations.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_organizations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_persons.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_persons.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_places.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_places.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_products.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_products.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_repos.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_repos.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_share_point_folders.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_share_point_folders.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_share_point_libraries.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_share_point_libraries.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_softwares.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_softwares.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_specifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from .enums import (
     AnthropicModels,
     AzureOpenAIModels,
     CohereModels,
     ConversationSearchTypes,
     ConversationStrategyTypes,
     EntityState,
+    GraphStrategyTypes,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
     RerankingModelServiceTypes,
     RetrievalStrategyTypes,
+    RevisionStrategyTypes,
     SpecificationTypes,
 )
 
 
 class QuerySpecifications(BaseModel):
     specifications: Optional["QuerySpecificationsSpecifications"]
 
@@ -50,14 +52,20 @@
     ] = Field(alias="promptStrategy")
     retrieval_strategy: Optional[
         "QuerySpecificationsSpecificationsResultsRetrievalStrategy"
     ] = Field(alias="retrievalStrategy")
     reranking_strategy: Optional[
         "QuerySpecificationsSpecificationsResultsRerankingStrategy"
     ] = Field(alias="rerankingStrategy")
+    graph_strategy: Optional[
+        "QuerySpecificationsSpecificationsResultsGraphStrategy"
+    ] = Field(alias="graphStrategy")
+    revision_strategy: Optional[
+        "QuerySpecificationsSpecificationsResultsRevisionStrategy"
+    ] = Field(alias="revisionStrategy")
     open_ai: Optional["QuerySpecificationsSpecificationsResultsOpenAi"] = Field(
         alias="openAI"
     )
     azure_open_ai: Optional["QuerySpecificationsSpecificationsResultsAzureOpenAi"] = (
         Field(alias="azureOpenAI")
     )
     cohere: Optional["QuerySpecificationsSpecificationsResultsCohere"]
@@ -88,14 +96,24 @@
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
 class QuerySpecificationsSpecificationsResultsRerankingStrategy(BaseModel):
     service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
+class QuerySpecificationsSpecificationsResultsGraphStrategy(BaseModel):
+    type: GraphStrategyTypes
+
+
+class QuerySpecificationsSpecificationsResultsRevisionStrategy(BaseModel):
+    type: RevisionStrategyTypes
+    custom_revision: Optional[str] = Field(alias="customRevision")
+    count: Optional[int]
+
+
 class QuerySpecificationsSpecificationsResultsOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
     model_name: Optional[str] = Field(alias="modelName")
     temperature: Optional[float]
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_usage.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # Source: ./documents
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .enums import BillableMetrics, ContentTypes, EntityTypes, FileTypes
+from .enums import BillableMetrics, ContentTypes, EntityTypes, FileTypes, OperationTypes
 
 
 class QueryUsage(BaseModel):
     usage: Optional[List[Optional["QueryUsageUsage"]]]
 
 
 class QueryUsageUsage(BaseModel):
+    id: Optional[str]
     correlation_id: Optional[str] = Field(alias="correlationId")
     date: Any
     credits: Optional[Any]
     name: str
     metric: Optional[BillableMetrics]
     workflow: Optional[str]
     entity_type: Optional[EntityTypes] = Field(alias="entityType")
@@ -34,13 +35,15 @@
     processor_name: Optional[str] = Field(alias="processorName")
     prompt: Optional[str]
     prompt_tokens: Optional[int] = Field(alias="promptTokens")
     completion: Optional[str]
     completion_tokens: Optional[int] = Field(alias="completionTokens")
     tokens: Optional[int]
     count: Optional[int]
+    operation: Optional[str]
+    operation_type: Optional[OperationTypes] = Field(alias="operationType")
     request: Optional[str]
     variables: Optional[str]
     response: Optional[str]
 
 
 QueryUsage.model_rebuild()
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240515001/graphlit_api/query_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 
 
 class QueryWorkflowsWorkflowsResultsExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
+    extracted_count: Optional[int] = Field(alias="extractedCount")
     azure_text: Optional[
         "QueryWorkflowsWorkflowsResultsExtractionJobsConnectorAzureText"
     ] = Field(alias="azureText")
     azure_image: Optional[
         "QueryWorkflowsWorkflowsResultsExtractionJobsConnectorAzureImage"
     ] = Field(alias="azureImage")
     open_ai_image: Optional[
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240515001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240515001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240515001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/update_content.py` & `graphlit_client-1.0.20240515001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240515001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240515001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240515001/graphlit_api/update_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
 
 class UpdateWorkflowUpdateWorkflowExtractionJobsConnector(BaseModel):
     type: EntityExtractionServiceTypes
     content_types: Optional[List[ContentTypes]] = Field(alias="contentTypes")
     file_types: Optional[List[FileTypes]] = Field(alias="fileTypes")
     extracted_types: Optional[List[ObservableTypes]] = Field(alias="extractedTypes")
+    extracted_count: Optional[int] = Field(alias="extractedCount")
     azure_text: Optional[
         "UpdateWorkflowUpdateWorkflowExtractionJobsConnectorAzureText"
     ] = Field(alias="azureText")
     azure_image: Optional[
         "UpdateWorkflowUpdateWorkflowExtractionJobsConnectorAzureImage"
     ] = Field(alias="azureImage")
     open_ai_image: Optional[
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240515001/graphlit_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240509002
+Version: 1.0.20240515001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240509002/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240515001/graphlit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240509002/setup.py` & `graphlit_client-1.0.20240515001/setup.py`

 * *Files identical despite different names*

