# Comparing `tmp/honcho_ai-0.0.8.tar.gz` & `tmp/honcho_ai-0.0.8a1.tar.gz`

## Comparing `honcho_ai-0.0.8.tar` & `honcho_ai-0.0.8a1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/__init__.py
--rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_base_client.py
--rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_version.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/lib/.keep
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/__init__.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/__init__.py
--rw-r--r--   0        0        0    19418 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/apps.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/__init__.py
--rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/users.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/__init__.py
--rw-r--r--   0        0        0    32165 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/collections.py
--rw-r--r--   0        0        0    23953 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/documents.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/__init__.py
--rw-r--r--   0        0        0    21471 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/messages.py
--rw-r--r--   0        0        0    24422 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/metamessages.py
--rw-r--r--   0        0        0    36225 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/sessions.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/app.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/app_create_params.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/app_update_params.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/page_user.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/user.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/user_create_params.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/user_list_params.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/user_update_params.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/agent_chat.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection_create_params.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection_list_params.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection_query_params.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection_query_response.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collection_update_params.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/page_collection.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/page_session.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session_chat_params.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session_create_params.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session_list_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session_stream_params.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/session_update_params.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/document.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/document_create_params.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/document_list_params.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/document_update_params.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/collections/page_document.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/message.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/message_create_params.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/message_list_params.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/message_update_params.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage_create_params.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage_get_params.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage_list_params.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage_update_params.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/page_message.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/page_metamessage.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 honcho_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/__init__.py
+-rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_base_client.py
+-rw-r--r--   0        0        0    17622 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_version.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/lib/.keep
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/__init__.py
+-rw-r--r--   0        0        0    19418 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/apps.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/__init__.py
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/users.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/__init__.py
+-rw-r--r--   0        0        0    32165 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/collections.py
+-rw-r--r--   0        0        0    23953 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/documents.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/__init__.py
+-rw-r--r--   0        0        0    21471 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/messages.py
+-rw-r--r--   0        0        0    24422 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/metamessages.py
+-rw-r--r--   0        0        0    36225 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/sessions.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app_create_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app_update_params.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/page_user.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_create_params.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_list_params.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_update_params.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/agent_chat.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_create_params.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_list_params.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_query_params.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_query_response.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_update_params.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/page_collection.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/page_session.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_chat_params.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_create_params.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_list_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_stream_params.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_update_params.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_create_params.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_list_params.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_update_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/page_document.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_create_params.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_list_params.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_update_params.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_create_params.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_get_params.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_list_params.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_update_params.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/page_message.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/page_metamessage.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/LICENSE
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/pyproject.toml
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/PKG-INFO
```

### Comparing `honcho_ai-0.0.8/src/honcho/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_base_client.py` & `honcho_ai-0.0.8a1/src/honcho/_base_client.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_client.py` & `honcho_ai-0.0.8a1/src/honcho/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 from ._utils import (
     is_given,
     get_async_library,
 )
 from ._version import __version__
 from ._streaming import Stream as Stream, AsyncStream as AsyncStream
-from ._exceptions import APIStatusError
+from ._exceptions import HonchoError, APIStatusError
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
@@ -53,15 +53,15 @@
 
 class Honcho(SyncAPIClient):
     apps: resources.AppsResource
     with_raw_response: HonchoWithRawResponse
     with_streaming_response: HonchoWithStreamedResponse
 
     # client options
-    api_key: str | None
+    api_key: str
 
     _environment: Literal["local", "demo"] | NotGiven
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
@@ -87,14 +87,18 @@
     ) -> None:
         """Construct a new synchronous honcho client instance.
 
         This automatically infers the `api_key` argument from the `HONCHO_AUTH_TOKEN` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("HONCHO_AUTH_TOKEN")
+        if api_key is None:
+            raise HonchoError(
+                "The api_key client option must be set either by passing api_key to the client or by setting the HONCHO_AUTH_TOKEN environment variable"
+            )
         self.api_key = api_key
 
         self._environment = environment
 
         base_url_env = os.environ.get("HONCHO_BASE_URL")
         if is_given(base_url) and base_url is not None:
             # cast required because mypy doesn't understand the type narrowing
@@ -139,16 +143,14 @@
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
     def auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
-        if api_key is None:
-            return {}
         return {"Authorization": f"Bearer {api_key}"}
 
     @property
     @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
@@ -245,15 +247,15 @@
 
 class AsyncHoncho(AsyncAPIClient):
     apps: resources.AsyncAppsResource
     with_raw_response: AsyncHonchoWithRawResponse
     with_streaming_response: AsyncHonchoWithStreamedResponse
 
     # client options
-    api_key: str | None
+    api_key: str
 
     _environment: Literal["local", "demo"] | NotGiven
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
@@ -279,14 +281,18 @@
     ) -> None:
         """Construct a new async honcho client instance.
 
         This automatically infers the `api_key` argument from the `HONCHO_AUTH_TOKEN` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("HONCHO_AUTH_TOKEN")
+        if api_key is None:
+            raise HonchoError(
+                "The api_key client option must be set either by passing api_key to the client or by setting the HONCHO_AUTH_TOKEN environment variable"
+            )
         self.api_key = api_key
 
         self._environment = environment
 
         base_url_env = os.environ.get("HONCHO_BASE_URL")
         if is_given(base_url) and base_url is not None:
             # cast required because mypy doesn't understand the type narrowing
@@ -331,16 +337,14 @@
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
     @override
     def auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
-        if api_key is None:
-            return {}
         return {"Authorization": f"Bearer {api_key}"}
 
     @property
     @override
     def default_headers(self) -> dict[str, str | Omit]:
         return {
             **super().default_headers,
```

### Comparing `honcho_ai-0.0.8/src/honcho/_compat.py` & `honcho_ai-0.0.8a1/src/honcho/_compat.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_exceptions.py` & `honcho_ai-0.0.8a1/src/honcho/_exceptions.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_files.py` & `honcho_ai-0.0.8a1/src/honcho/_files.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_models.py` & `honcho_ai-0.0.8a1/src/honcho/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     get_model_config,
     get_model_fields,
     field_get_default,
 )
 from ._constants import RAW_RESPONSE_HEADER
 
 if TYPE_CHECKING:
-    from pydantic_core.core_schema import ModelField, LiteralSchema, ModelFieldsSchema
+    from pydantic_core.core_schema import ModelField, ModelFieldsSchema
 
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
@@ -247,17 +247,15 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool | Literal["none", "warn", "error"] = True,
-            context: dict[str, Any] | None = None,
-            serialize_as_any: bool = False,
+            warnings: bool = True,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -277,18 +275,14 @@
             """
             if mode != "python":
                 raise ValueError("mode is only supported in Pydantic v2")
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
-            if context is not None:
-                raise ValueError("context is only supported in Pydantic v2")
-            if serialize_as_any != False:
-                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().dict(  # pyright: ignore[reportDeprecated]
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
@@ -302,17 +296,15 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool | Literal["none", "warn", "error"] = True,
-            context: dict[str, Any] | None = None,
-            serialize_as_any: bool = False,
+            warnings: bool = True,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -328,18 +320,14 @@
             Returns:
                 A JSON string representation of the model.
             """
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
-            if context is not None:
-                raise ValueError("context is only supported in Pydantic v2")
-            if serialize_as_any != False:
-                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().json(  # type: ignore[reportDeprecated]
                 indent=indent,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
@@ -558,15 +546,15 @@
 
                 # Note: if one variant defines an alias then they all should
                 discriminator_alias = field.get("serialization_alias")
 
                 field_schema = field["schema"]
 
                 if field_schema["type"] == "literal":
-                    for entry in cast("LiteralSchema", field_schema)["expected"]:
+                    for entry in field_schema["expected"]:
                         if isinstance(entry, str):
                             mapping[entry] = variant
             else:
                 field_info = cast("dict[str, FieldInfo]", variant.__fields__).get(discriminator_field_name)  # pyright: ignore[reportDeprecated, reportUnnecessaryCast]
                 if not field_info:
                     continue
```

### Comparing `honcho_ai-0.0.8/src/honcho/_qs.py` & `honcho_ai-0.0.8a1/src/honcho/_qs.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_resource.py` & `honcho_ai-0.0.8a1/src/honcho/_resource.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_response.py` & `honcho_ai-0.0.8a1/src/honcho/_response.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_streaming.py` & `honcho_ai-0.0.8a1/src/honcho/_streaming.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_types.py` & `honcho_ai-0.0.8a1/src/honcho/_types.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/pagination.py` & `honcho_ai-0.0.8a1/src/honcho/pagination.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_logs.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_proxy.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_sync.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_transform.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_typing.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/_utils/_utils.py` & `honcho_ai-0.0.8a1/src/honcho/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/apps.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/apps.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/users.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/users.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/collections.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/collections.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/collections/documents.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/documents.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/messages.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/messages.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/metamessages.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/metamessages.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/resources/apps/users/sessions/sessions.py` & `honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/sessions.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/types/apps/users/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/types/apps/users/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/__init__.py` & `honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/src/honcho/types/apps/users/sessions/metamessage_list_params.py` & `honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_list_params.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/LICENSE` & `honcho_ai-0.0.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.8/pyproject.toml` & `honcho_ai-0.0.8a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "honcho-ai"
-version = "0.0.8"
+version = "0.0.8-alpha.1"
 description = "The official Python library for the honcho API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Honcho", email = "hello@plasticlabs.ai" },
 ]
 dependencies = [
```

### Comparing `honcho_ai-0.0.8/PKG-INFO` & `honcho_ai-0.0.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: honcho-ai
-Version: 0.0.8
+Version: 0.0.8a1
 Summary: The official Python library for the honcho API
 Project-URL: Homepage, https://github.com/plastic-labs/honcho-python
 Project-URL: Repository, https://github.com/plastic-labs/honcho-python
 Author-email: Honcho <hello@plasticlabs.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

