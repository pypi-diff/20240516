# Comparing `tmp/azure-eventhub-5.9.0b2.zip` & `tmp/azure-eventhub-5.9.0b3.zip`

## zipinfo {}

```diff
@@ -1,161 +1,177 @@
-Zip file size: 260980 bytes, number of entries: 159
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/doc/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/
--rw-rw-r--  2.0 unx     2436 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/setup.py
--rw-rw-r--  2.0 unx    19924 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/migration_guide.md
--rw-rw-r--  2.0 unx    29636 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx     1073 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/LICENSE
--rw-rw-r--  2.0 unx      175 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/MANIFEST.in
--rw-rw-r--  2.0 unx    25509 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/README.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/setup.cfg
--rw-rw-r--  2.0 unx    64026 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     5963 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       46 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/requires.txt
--rw-rw-r--  2.0 unx    64026 b- defN 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure_eventhub.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx      164 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/doc/azure.rst
--rw-rw-r--  2.0 unx      577 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/doc/azure.eventhub.amqp.rst
--rw-rw-r--  2.0 unx     1390 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/doc/azure.eventhub.rst
--rw-rw-r--  2.0 unx     1020 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/doc/azure.eventhub.exceptions.rst
--rw-rw-r--  2.0 unx      706 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/doc/azure.eventhub.aio.rst
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/perfstress_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/unittest/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/livetest/
--rw-rw-r--  2.0 unx    15029 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/eventhub_preparer.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/
--rw-rw-r--  2.0 unx     1501 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event.py
--rw-rw-r--  2.0 unx      345 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     4131 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/_test_base.py
--rw-rw-r--  2.0 unx     1694 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event_batch.py
--rw-rw-r--  2.0 unx     1609 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/send_event_batch.py
--rw-rw-r--  2.0 unx      866 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event.py
--rw-rw-r--  2.0 unx      345 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/__init__.py
--rw-rw-r--  2.0 unx     4976 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/_test_base.py
--rw-rw-r--  2.0 unx     1038 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py
--rw-rw-r--  2.0 unx     1002 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/unittest/asynctests/
--rw-rw-r--  2.0 unx     5685 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/test_client_creation.py
--rw-rw-r--  2.0 unx     2117 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/test_dict_mixin.py
--rw-rw-r--  2.0 unx     5955 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/test_event_data.py
--rw-rw-r--  2.0 unx     7586 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/test_connection_string_parser.py
--rw-rw-r--  2.0 unx     4849 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_in_memory_checkpointstore.py
--rw-rw-r--  2.0 unx     4252 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_client_creation_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/livetest/synctests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/tests/livetest/asynctests/
--rw-rw-r--  2.0 unx     8287 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_consumer_client.py
--rw-rw-r--  2.0 unx    25110 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_eventprocessor.py
--rw-rw-r--  2.0 unx     4087 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_negative.py
--rw-rw-r--  2.0 unx    14932 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_send.py
--rw-rw-r--  2.0 unx     6407 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_auth.py
--rw-rw-r--  2.0 unx     7615 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_receive.py
--rw-rw-r--  2.0 unx     4935 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_reconnect.py
--rw-rw-r--  2.0 unx     3596 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/synctests/test_properties.py
--rw-rw-r--  2.0 unx     7698 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_consumer_client_async.py
--rw-rw-r--  2.0 unx    14936 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_send_async.py
--rw-rw-r--  2.0 unx     3746 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_properties_async.py
--rw-rw-r--  2.0 unx    27955 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_eventprocessor_async.py
--rw-rw-r--  2.0 unx     7856 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_receive_async.py
--rw-rw-r--  2.0 unx     5049 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_reconnect_async.py
--rw-rw-r--  2.0 unx     5962 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_negative_async.py
--rw-rw-r--  2.0 unx     6543 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_auth_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/samples/async_samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/samples/sync_samples/
--rw-rw-r--  2.0 unx     1719 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_track_last_enqueued_event_prop_async.py
--rw-rw-r--  2.0 unx     3409 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_with_custom_starting_position_async.py
--rw-rw-r--  2.0 unx     2286 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_async.py
--rw-rw-r--  2.0 unx     4236 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/client_creation_async.py
--rw-rw-r--  2.0 unx     2290 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/receive_batch_with_checkpoint_async.py
--rw-rw-r--  2.0 unx     1614 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_named_key_credential_async.py
--rw-rw-r--  2.0 unx     5378 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/iot_hub_connection_string_receive_async.py
--rw-rw-r--  2.0 unx     3026 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/connection_to_custom_endpoint_address_async.py
--rw-rw-r--  2.0 unx     4121 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
--rw-rw-r--  2.0 unx     1585 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/send_stream_async.py
--rw-rw-r--  2.0 unx     4176 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/send_async.py
--rw-rw-r--  2.0 unx     2890 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_event_count_async.py
--rw-rw-r--  2.0 unx     2954 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py
--rw-rw-r--  2.0 unx     2662 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_sas_credential_async.py
--rw-rw-r--  2.0 unx     9021 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/sample_code_eventhub_async.py
--rw-rw-r--  2.0 unx     2593 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_for_period_async.py
--rw-rw-r--  2.0 unx     2952 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/client_identity_authentication_async.py
--rw-rw-r--  2.0 unx     2509 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_store_async.py
--rw-rw-r--  2.0 unx     1010 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/connection_string_authentication_async.py
--rw-rw-r--  2.0 unx     2209 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/proxy_async.py
--rw-rw-r--  2.0 unx     3149 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_sas_token_async.py
--rw-rw-r--  2.0 unx     2951 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_sas_token.py
--rw-rw-r--  2.0 unx     2432 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_sas_credential.py
--rw-rw-r--  2.0 unx     2577 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_store.py
--rw-rw-r--  2.0 unx     3304 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_custom_starting_position.py
--rw-rw-r--  2.0 unx     1411 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_named_key_credential.py
--rw-rw-r--  2.0 unx     3023 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_time_interval.py
--rw-rw-r--  2.0 unx     4083 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/client_creation.py
--rw-rw-r--  2.0 unx     1960 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/proxy.py
--rw-rw-r--  2.0 unx     2901 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/connection_to_custom_endpoint_address.py
--rw-rw-r--  2.0 unx     3901 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/send.py
--rw-rw-r--  2.0 unx     1708 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_track_last_enqueued_event_prop.py
--rw-rw-r--  2.0 unx     2960 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_event_count.py
--rw-rw-r--  2.0 unx     1385 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/send_stream.py
--rw-rw-r--  2.0 unx     3835 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/send_and_receive_amqp_annotated_message.py
--rw-rw-r--  2.0 unx      885 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/connection_string_authentication.py
--rw-rw-r--  2.0 unx     3601 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/client_identity_authentication.py
--rw-rw-r--  2.0 unx     2065 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/receive_batch_with_checkpoint.py
--rw-rw-r--  2.0 unx     2644 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv_for_period.py
--rw-rw-r--  2.0 unx     8704 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/sample_code_eventhub.py
--rw-rw-r--  2.0 unx     2261 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/samples/sync_samples/recv.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/
--rw-rw-r--  2.0 unx      426 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/extensions/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/amqp/
--rw-rw-r--  2.0 unx     2099 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_constants.py
--rw-rw-r--  2.0 unx     3112 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_configuration.py
--rw-rw-r--  2.0 unx    37032 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_consumer_client.py
--rw-rw-r--  2.0 unx     1408 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_connection_manager.py
--rw-rw-r--  2.0 unx    24219 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_client_base.py
--rw-rw-r--  2.0 unx    23483 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_common.py
--rw-rw-r--  2.0 unx     3083 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_connection_string_parser.py
--rw-rw-r--  2.0 unx    11625 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_producer.py
--rw-rw-r--  2.0 unx      172 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_version.py
--rw-rw-r--  2.0 unx    11215 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_consumer.py
--rw-rw-r--  2.0 unx    22717 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_producer_client.py
--rw-rw-r--  2.0 unx     1321 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/__init__.py
--rw-rw-r--  2.0 unx     2240 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_mixin.py
--rw-rw-r--  2.0 unx    11594 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_utils.py
--rw-rw-r--  2.0 unx     8191 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/exceptions.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 22-Mar-09 19:15 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/
--rw-rw-r--  2.0 unx    11473 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_producer_async.py
--rw-rw-r--  2.0 unx     3056 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_error_async.py
--rw-rw-r--  2.0 unx    20215 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_client_base_async.py
--rw-rw-r--  2.0 unx      575 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_async_utils.py
--rw-rw-r--  2.0 unx    23756 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_producer_client_async.py
--rw-rw-r--  2.0 unx    42344 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_client_async.py
--rw-rw-r--  2.0 unx      806 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/__init__.py
--rw-rw-r--  2.0 unx     1382 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_connection_manager_async.py
--rw-rw-r--  2.0 unx    10630 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_async.py
--rw-rw-r--  2.0 unx      336 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/__init__.py
--rw-rw-r--  2.0 unx     4280 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/partition_context.py
--rw-rw-r--  2.0 unx     1664 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py
--rw-rw-r--  2.0 unx    18174 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/event_processor.py
--rw-rw-r--  2.0 unx      715 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/utils.py
--rw-rw-r--  2.0 unx     6992 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/checkpoint_store.py
--rw-rw-r--  2.0 unx    10204 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/_ownership_manager.py
--rw-rw-r--  2.0 unx     4299 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py
--rw-rw-r--  2.0 unx      847 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/common.py
--rw-rw-r--  2.0 unx    10165 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/ownership_manager.py
--rw-rw-r--  2.0 unx      345 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/__init__.py
--rw-rw-r--  2.0 unx     4337 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/partition_context.py
--rw-rw-r--  2.0 unx     5412 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py
--rw-rw-r--  2.0 unx    17225 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/event_processor.py
--rw-rw-r--  2.0 unx     7001 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/checkpoint_store.py
--rw-rw-r--  2.0 unx      426 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/extensions/__init__.py
--rw-rw-r--  2.0 unx      688 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/amqp/_constants.py
--rw-rw-r--  2.0 unx      567 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/amqp/__init__.py
--rw-rw-r--  2.0 unx    23863 b- defN 22-Mar-09 19:14 azure-eventhub-5.9.0b2/azure/eventhub/amqp/_amqp_message.py
-159 files, 954505 bytes uncompressed, 229058 bytes compressed:  76.0%
+Zip file size: 292774 bytes, number of entries: 175
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/doc/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/
+-rw-rw-r--  2.0 unx    25509 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/README.md
+-rw-rw-r--  2.0 unx    19924 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/migration_guide.md
+-rw-rw-r--  2.0 unx     2472 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/setup.py
+-rw-rw-r--  2.0 unx    31293 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/LICENSE
+-rw-rw-r--  2.0 unx    65795 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/setup.cfg
+-rw-rw-r--  2.0 unx      175 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/samples/sync_samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/samples/async_samples/
+-rw-rw-r--  2.0 unx     1385 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/send_stream.py
+-rw-rw-r--  2.0 unx     4083 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/client_creation.py
+-rw-rw-r--  2.0 unx     2065 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/receive_batch_with_checkpoint.py
+-rw-rw-r--  2.0 unx     3835 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/send_and_receive_amqp_annotated_message.py
+-rw-rw-r--  2.0 unx     2261 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv.py
+-rw-rw-r--  2.0 unx     2644 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_for_period.py
+-rw-rw-r--  2.0 unx     1411 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_named_key_credential.py
+-rw-rw-r--  2.0 unx     1960 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/proxy.py
+-rw-rw-r--  2.0 unx     3023 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_time_interval.py
+-rw-rw-r--  2.0 unx     8704 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/sample_code_eventhub.py
+-rw-rw-r--  2.0 unx     3304 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_custom_starting_position.py
+-rw-rw-r--  2.0 unx     2901 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/connection_to_custom_endpoint_address.py
+-rw-rw-r--  2.0 unx     1706 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/send_buffered_mode.py
+-rw-rw-r--  2.0 unx     2432 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_sas_credential.py
+-rw-rw-r--  2.0 unx     2577 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_store.py
+-rw-rw-r--  2.0 unx      885 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/connection_string_authentication.py
+-rw-rw-r--  2.0 unx     1708 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_track_last_enqueued_event_prop.py
+-rw-rw-r--  2.0 unx     2960 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_event_count.py
+-rw-rw-r--  2.0 unx     2951 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_sas_token.py
+-rw-rw-r--  2.0 unx     3601 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/client_identity_authentication.py
+-rw-rw-r--  2.0 unx     3901 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/sync_samples/send.py
+-rw-rw-r--  2.0 unx     1585 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/send_stream_async.py
+-rw-rw-r--  2.0 unx     2954 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py
+-rw-rw-r--  2.0 unx     2890 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_event_count_async.py
+-rw-rw-r--  2.0 unx     1010 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/connection_string_authentication_async.py
+-rw-rw-r--  2.0 unx     1614 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_named_key_credential_async.py
+-rw-rw-r--  2.0 unx     9021 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/sample_code_eventhub_async.py
+-rw-rw-r--  2.0 unx     4121 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
+-rw-rw-r--  2.0 unx     1719 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_track_last_enqueued_event_prop_async.py
+-rw-rw-r--  2.0 unx     3409 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_with_custom_starting_position_async.py
+-rw-rw-r--  2.0 unx     5378 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/iot_hub_connection_string_receive_async.py
+-rw-rw-r--  2.0 unx     1925 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/send_buffered_mode_async.py
+-rw-rw-r--  2.0 unx     3149 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_sas_token_async.py
+-rw-rw-r--  2.0 unx     2209 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/proxy_async.py
+-rw-rw-r--  2.0 unx     2286 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_async.py
+-rw-rw-r--  2.0 unx     3026 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/connection_to_custom_endpoint_address_async.py
+-rw-rw-r--  2.0 unx     4236 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/client_creation_async.py
+-rw-rw-r--  2.0 unx     2662 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_sas_credential_async.py
+-rw-rw-r--  2.0 unx     2509 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_store_async.py
+-rw-rw-r--  2.0 unx     2593 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/recv_for_period_async.py
+-rw-rw-r--  2.0 unx     2290 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/receive_batch_with_checkpoint_async.py
+-rw-rw-r--  2.0 unx     2952 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/client_identity_authentication_async.py
+-rw-rw-r--  2.0 unx     4176 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/samples/async_samples/send_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/livetest/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/perfstress_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/unittest/
+-rw-rw-r--  2.0 unx    15029 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/eventhub_preparer.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/livetest/synctests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/livetest/asynctests/
+-rw-rw-r--  2.0 unx     7615 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_receive.py
+-rw-rw-r--  2.0 unx     8287 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_consumer_client.py
+-rw-rw-r--  2.0 unx     6407 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_auth.py
+-rw-rw-r--  2.0 unx    25110 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_eventprocessor.py
+-rw-rw-r--  2.0 unx    20471 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_send.py
+-rw-rw-r--  2.0 unx     3596 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_properties.py
+-rw-rw-r--  2.0 unx     4935 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_reconnect.py
+-rw-rw-r--  2.0 unx    23327 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_buffered_producer.py
+-rw-rw-r--  2.0 unx     4768 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/synctests/test_negative.py
+-rw-rw-r--  2.0 unx    24146 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_buffered_producer_async.py
+-rw-rw-r--  2.0 unx     6673 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_negative_async.py
+-rw-rw-r--  2.0 unx     7698 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_consumer_client_async.py
+-rw-rw-r--  2.0 unx    27955 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_eventprocessor_async.py
+-rw-rw-r--  2.0 unx     5049 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_reconnect_async.py
+-rw-rw-r--  2.0 unx     3746 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_properties_async.py
+-rw-rw-r--  2.0 unx    20013 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_send_async.py
+-rw-rw-r--  2.0 unx     7856 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_receive_async.py
+-rw-rw-r--  2.0 unx     6543 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_auth_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/
+-rw-rw-r--  2.0 unx     1501 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event.py
+-rw-rw-r--  2.0 unx      345 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     4131 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/_test_base.py
+-rw-rw-r--  2.0 unx     1609 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/send_event_batch.py
+-rw-rw-r--  2.0 unx     1694 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event_batch.py
+-rw-rw-r--  2.0 unx      345 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/__init__.py
+-rw-rw-r--  2.0 unx     4976 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/_test_base.py
+-rw-rw-r--  2.0 unx     1002 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py
+-rw-rw-r--  2.0 unx      866 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event.py
+-rw-rw-r--  2.0 unx     1038 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/tests/unittest/asynctests/
+-rw-rw-r--  2.0 unx     5685 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/test_client_creation.py
+-rw-rw-r--  2.0 unx     2297 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/test_partition_resolver.py
+-rw-rw-r--  2.0 unx     7586 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/test_connection_string_parser.py
+-rw-rw-r--  2.0 unx     2117 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/test_dict_mixin.py
+-rw-rw-r--  2.0 unx     5955 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/test_event_data.py
+-rw-rw-r--  2.0 unx     4252 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_client_creation_async.py
+-rw-rw-r--  2.0 unx     4849 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_in_memory_checkpointstore.py
+-rw-rw-r--  2.0 unx     1464 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_partition_resolver_async.py
+-rw-rw-r--  2.0 unx     6752 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       71 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    65795 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure_eventhub.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx      577 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/doc/azure.eventhub.amqp.rst
+-rw-rw-r--  2.0 unx      164 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/doc/azure.rst
+-rw-rw-r--  2.0 unx     1390 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/doc/azure.eventhub.rst
+-rw-rw-r--  2.0 unx     1020 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/doc/azure.eventhub.exceptions.rst
+-rw-rw-r--  2.0 unx      706 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/doc/azure.eventhub.aio.rst
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/
+-rw-rw-r--  2.0 unx      426 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/amqp/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/extensions/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/aio/
+-rw-rw-r--  2.0 unx     3083 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_connection_string_parser.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/py.typed
+-rw-rw-r--  2.0 unx     1408 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_connection_manager.py
+-rw-rw-r--  2.0 unx     2240 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_mixin.py
+-rw-rw-r--  2.0 unx    23800 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_common.py
+-rw-rw-r--  2.0 unx    43504 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_producer_client.py
+-rw-rw-r--  2.0 unx     1321 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/__init__.py
+-rw-rw-r--  2.0 unx    12279 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_utils.py
+-rw-rw-r--  2.0 unx     8191 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/exceptions.py
+-rw-rw-r--  2.0 unx    24326 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_client_base.py
+-rw-rw-r--  2.0 unx     3112 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_configuration.py
+-rw-rw-r--  2.0 unx      172 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_version.py
+-rw-rw-r--  2.0 unx    11877 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_producer.py
+-rw-rw-r--  2.0 unx     2099 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_constants.py
+-rw-rw-r--  2.0 unx    11215 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_consumer.py
+-rw-rw-r--  2.0 unx    36948 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_consumer_client.py
+-rw-rw-r--  2.0 unx      847 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/common.py
+-rw-rw-r--  2.0 unx     4299 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py
+-rw-rw-r--  2.0 unx     5412 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py
+-rw-rw-r--  2.0 unx      345 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/__init__.py
+-rw-rw-r--  2.0 unx    10165 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/ownership_manager.py
+-rw-rw-r--  2.0 unx     4337 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/partition_context.py
+-rw-rw-r--  2.0 unx    17225 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/event_processor.py
+-rw-rw-r--  2.0 unx     7001 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/checkpoint_store.py
+-rw-rw-r--  2.0 unx    23863 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/amqp/_amqp_message.py
+-rw-rw-r--  2.0 unx      567 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/amqp/__init__.py
+-rw-rw-r--  2.0 unx      770 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/amqp/_constants.py
+-rw-rw-r--  2.0 unx      426 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/extensions/__init__.py
+-rw-rw-r--  2.0 unx     6209 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_partition_resolver.py
+-rw-rw-r--  2.0 unx     6437 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_buffered_producer_dispatcher.py
+-rw-rw-r--  2.0 unx      613 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/__init__.py
+-rw-rw-r--  2.0 unx    10135 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_buffered_producer.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-21 02:09 azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/
+-rw-rw-r--  2.0 unx    44390 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_producer_client_async.py
+-rw-rw-r--  2.0 unx    10630 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_async.py
+-rw-rw-r--  2.0 unx      806 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/__init__.py
+-rw-rw-r--  2.0 unx    11581 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_producer_async.py
+-rw-rw-r--  2.0 unx    42247 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_client_async.py
+-rw-rw-r--  2.0 unx    20282 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_client_base_async.py
+-rw-rw-r--  2.0 unx      839 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_async_utils.py
+-rw-rw-r--  2.0 unx     3056 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_error_async.py
+-rw-rw-r--  2.0 unx     1382 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_connection_manager_async.py
+-rw-rw-r--  2.0 unx     1664 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py
+-rw-rw-r--  2.0 unx      715 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/utils.py
+-rw-rw-r--  2.0 unx      336 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/__init__.py
+-rw-rw-r--  2.0 unx    10204 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/_ownership_manager.py
+-rw-rw-r--  2.0 unx     4280 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/partition_context.py
+-rw-rw-r--  2.0 unx    18174 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/event_processor.py
+-rw-rw-r--  2.0 unx     6992 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/checkpoint_store.py
+-rw-rw-r--  2.0 unx    10199 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_buffered_producer_async.py
+-rw-rw-r--  2.0 unx      630 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/__init__.py
+-rw-rw-r--  2.0 unx     6133 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_buffered_producer_dispatcher_async.py
+-rw-rw-r--  2.0 unx     1195 b- defN 22-Apr-21 02:08 azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_partition_resolver_async.py
+175 files, 1112096 bytes uncompressed, 257206 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,478 +1,526 @@
-Filename: azure-eventhub-5.9.0b2/
+Filename: azure-eventhub-5.9.0b3/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/
+Filename: azure-eventhub-5.9.0b3/samples/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/
+Filename: azure-eventhub-5.9.0b3/tests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/
+Filename: azure-eventhub-5.9.0b3/doc/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/
+Filename: azure-eventhub-5.9.0b3/azure/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/setup.py
+Filename: azure-eventhub-5.9.0b3/README.md
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/migration_guide.md
+Filename: azure-eventhub-5.9.0b3/migration_guide.md
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/CHANGELOG.md
+Filename: azure-eventhub-5.9.0b3/setup.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/LICENSE
+Filename: azure-eventhub-5.9.0b3/CHANGELOG.md
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/MANIFEST.in
+Filename: azure-eventhub-5.9.0b3/LICENSE
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/README.md
+Filename: azure-eventhub-5.9.0b3/PKG-INFO
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/setup.cfg
+Filename: azure-eventhub-5.9.0b3/setup.cfg
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/PKG-INFO
+Filename: azure-eventhub-5.9.0b3/MANIFEST.in
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/top_level.txt
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/not-zip-safe
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/dependency_links.txt
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/send_stream.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/SOURCES.txt
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/client_creation.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/requires.txt
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/receive_batch_with_checkpoint.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure_eventhub.egg-info/PKG-INFO
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/send_and_receive_amqp_annotated_message.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/azure.rst
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/azure.eventhub.amqp.rst
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_for_period.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/azure.eventhub.rst
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_named_key_credential.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/azure.eventhub.exceptions.rst
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/proxy.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/doc/azure.eventhub.aio.rst
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_time_interval.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/sample_code_eventhub.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_custom_starting_position.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/connection_to_custom_endpoint_address.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/eventhub_preparer.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/send_buffered_mode.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_sas_credential.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_store.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/__init__.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/connection_string_authentication.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/_test_base.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_track_last_enqueued_event_prop.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event_batch.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_event_count.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/send_event_batch.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_sas_token.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/client_identity_authentication.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/__init__.py
+Filename: azure-eventhub-5.9.0b3/samples/sync_samples/send.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/_test_base.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/send_stream_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_event_count_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/asynctests/
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/connection_string_authentication_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/test_client_creation.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_named_key_credential_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/test_dict_mixin.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/sample_code_eventhub_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/test_event_data.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/test_connection_string_parser.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_track_last_enqueued_event_prop_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_in_memory_checkpointstore.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_with_custom_starting_position_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_client_creation_async.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/iot_hub_connection_string_receive_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/send_buffered_mode_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_sas_token_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_consumer_client.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/proxy_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_eventprocessor.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_negative.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/connection_to_custom_endpoint_address_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_send.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/client_creation_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_auth.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_sas_credential_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_receive.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_store_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_reconnect.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/recv_for_period_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/synctests/test_properties.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/receive_batch_with_checkpoint_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_consumer_client_async.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/client_identity_authentication_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_send_async.py
+Filename: azure-eventhub-5.9.0b3/samples/async_samples/send_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_properties_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_eventprocessor_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_receive_async.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_reconnect_async.py
+Filename: azure-eventhub-5.9.0b3/tests/eventhub_preparer.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_negative_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_auth_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_receive.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_consumer_client.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_track_last_enqueued_event_prop_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_auth.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_with_custom_starting_position_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_eventprocessor.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_send.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/client_creation_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_properties.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/receive_batch_with_checkpoint_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_reconnect.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_named_key_credential_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_buffered_producer.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/iot_hub_connection_string_receive_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/synctests/test_negative.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/connection_to_custom_endpoint_address_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_buffered_producer_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/send_and_receive_amqp_annotated_message_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_negative_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/send_stream_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_consumer_client_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/send_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_eventprocessor_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_event_count_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_reconnect_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_properties_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_sas_credential_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_send_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/sample_code_eventhub_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_receive_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_for_period_async.py
+Filename: azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_auth_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/client_identity_authentication_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_store_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/connection_string_authentication_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/proxy_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/_test_base.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_sas_token_async.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/send_event_batch.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_sas_token.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event_batch.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_sas_credential.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_store.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/_test_base.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_custom_starting_position.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_named_key_credential.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_time_interval.py
+Filename: azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/client_creation.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/asynctests/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/proxy.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/test_client_creation.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/connection_to_custom_endpoint_address.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/test_partition_resolver.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/send.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/test_connection_string_parser.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_track_last_enqueued_event_prop.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/test_dict_mixin.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_event_count.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/test_event_data.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/send_stream.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_client_creation_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/send_and_receive_amqp_annotated_message.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_in_memory_checkpointstore.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/connection_string_authentication.py
+Filename: azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_partition_resolver_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/client_identity_authentication.py
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/receive_batch_with_checkpoint.py
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/requires.txt
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv_for_period.py
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/sample_code_eventhub.py
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/samples/sync_samples/recv.py
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/
+Filename: azure-eventhub-5.9.0b3/azure_eventhub.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/__init__.py
+Filename: azure-eventhub-5.9.0b3/doc/azure.eventhub.amqp.rst
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/
+Filename: azure-eventhub-5.9.0b3/doc/azure.rst
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/
+Filename: azure-eventhub-5.9.0b3/doc/azure.eventhub.rst
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/extensions/
+Filename: azure-eventhub-5.9.0b3/doc/azure.eventhub.exceptions.rst
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/amqp/
+Filename: azure-eventhub-5.9.0b3/doc/azure.eventhub.aio.rst
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_constants.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_configuration.py
+Filename: azure-eventhub-5.9.0b3/azure/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_consumer_client.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_connection_manager.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/amqp/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_client_base.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/extensions/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_common.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_connection_string_parser.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_producer.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_connection_string_parser.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_version.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/py.typed
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_consumer.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_connection_manager.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_producer_client.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_mixin.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_common.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_mixin.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_producer_client.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_utils.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/exceptions.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_utils.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/py.typed
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/exceptions.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_client_base.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_producer_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_configuration.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_error_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_version.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_client_base_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_producer.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_async_utils.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_constants.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_producer_client_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_consumer.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_client_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_consumer_client.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/common.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_connection_manager_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_async.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/partition_context.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/ownership_manager.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/partition_context.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/event_processor.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/event_processor.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/utils.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/checkpoint_store.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/checkpoint_store.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/amqp/_amqp_message.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/_ownership_manager.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/amqp/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/amqp/_constants.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/common.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/extensions/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/ownership_manager.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_partition_resolver.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_buffered_producer_dispatcher.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/partition_context.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/_buffered_producer/_buffered_producer.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/event_processor.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/checkpoint_store.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/extensions/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_producer_client_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/amqp/_constants.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_async.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/amqp/__init__.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/__init__.py
 Comment: 
 
-Filename: azure-eventhub-5.9.0b2/azure/eventhub/amqp/_amqp_message.py
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_producer_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_client_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_client_base_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_async_utils.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_error_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_connection_manager_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/utils.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/__init__.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/_ownership_manager.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/partition_context.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/event_processor.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/checkpoint_store.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_buffered_producer_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/__init__.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_buffered_producer_dispatcher_async.py
+Comment: 
+
+Filename: azure-eventhub-5.9.0b3/azure/eventhub/aio/_buffered_producer/_partition_resolver_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-eventhub-5.9.0b2/setup.py` & `azure-eventhub-5.9.0b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,9 +67,10 @@
     ],
     python_requires=">=3.6",
     zip_safe=False,
     packages=find_packages(exclude=exclude_packages),
     install_requires=[
         "azure-core<2.0.0,>=1.14.0",
         "uamqp>=1.5.1,<2.0.0",
+        "typing-extensions>=4.0.1",
     ]
 )
```

## Comparing `azure-eventhub-5.9.0b2/migration_guide.md` & `azure-eventhub-5.9.0b3/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/CHANGELOG.md` & `azure-eventhub-5.9.0b3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Release History
 
+## 5.9.0b3 (2022-04-20)
+
+### Features Added
+
+- Introduced new method `send_event` to `EventHubProducerClient` which allows sending single `EventData` or `AmqpAnnotatedMessage`.
+- Introduced buffered mode sending to `EventHubProducerClient` which is intended to allow for efficient publishing of events
+ without having to explicitly manage batches in the application.
+  - The constructor of `EventHubProducerClient` and `from_connection_string` method now takes the following new keyword arguments
+   for configuration:
+    - `buffered_mode`: The flag to enable/disable buffered mode sending.
+    - `on_success`: The callback to be called once events have been successfully published.
+    - `on_error`: The callback to be called once events have failed to be published.
+    - `max_buffer_length`: The total number of events per partition that can be buffered before a flush will be triggered.
+    - `max_wait_time`: The amount of time to wait for a batch to be built with events in the buffer before publishing.
+  - Introduced new method `EventHubProducerClient.flush` which flushes events in the buffer to be sent immediately.
+  - Introduced new method `EventHubProducerClient.get_buffered_event_count` which returns the number of events that are buffered and waiting to be published for a given partition.
+  - Introduced new property `EventHubProducerClient.total_buffered_event_count` which returns the total number of events that are currently buffered and waiting to be published, across all partitions.
+  - Introduced new boolean keyword argument `flush` to `EventHubProducerClient.close` which indicates whether to flush the buffer or not while closing.
+
+### Other Changes
+
+- Updated `EventData` internals for interoperability with the Schema Registry Avro Encoder library.
+
 ## 5.9.0b2 (2022-03-09)
 
 ### Breaking Changes
 
 - `from_message_data` on `EventData` has been renamed `from_message_content` for interoperability with the Schema Registry Avro Encoder library. The `data` parameter has been renamed to `content`.
 
 ## 5.9.0b1 (2022-02-09)
@@ -514,17 +537,8 @@
 
 ## 0.2.0b1 (2018-04-20)
 
 - Updated uAMQP to latest version.
 - Further testing and minor bug fixes.
 
 
-## 0.2.0a2 (2018-04-02)
-
-- Updated uAQMP dependency.
-
-
-## 0.2.0a1 (unreleased)
-
-- Swapped out Proton dependency for uAMQP.
-
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/eventhub/azure-eventhub/HISTORY.png)
```

## Comparing `azure-eventhub-5.9.0b2/LICENSE` & `azure-eventhub-5.9.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/README.md` & `azure-eventhub-5.9.0b3/README.md`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/PKG-INFO` & `azure-eventhub-5.9.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-eventhub
-Version: 5.9.0b2
+Version: 5.9.0b3
 Summary: Microsoft Azure Event Hubs Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventhub/azure-eventhub
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Azure Event Hubs client library for Python
         
@@ -478,14 +478,37 @@
         [schemaregistry_avroencoder_repo]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/schemaregistry/azure-schemaregistry-avroencoder
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/eventhub/azure-eventhub/README.png)
         
         
         # Release History
         
+        ## 5.9.0b3 (2022-04-20)
+        
+        ### Features Added
+        
+        - Introduced new method `send_event` to `EventHubProducerClient` which allows sending single `EventData` or `AmqpAnnotatedMessage`.
+        - Introduced buffered mode sending to `EventHubProducerClient` which is intended to allow for efficient publishing of events
+         without having to explicitly manage batches in the application.
+          - The constructor of `EventHubProducerClient` and `from_connection_string` method now takes the following new keyword arguments
+           for configuration:
+            - `buffered_mode`: The flag to enable/disable buffered mode sending.
+            - `on_success`: The callback to be called once events have been successfully published.
+            - `on_error`: The callback to be called once events have failed to be published.
+            - `max_buffer_length`: The total number of events per partition that can be buffered before a flush will be triggered.
+            - `max_wait_time`: The amount of time to wait for a batch to be built with events in the buffer before publishing.
+          - Introduced new method `EventHubProducerClient.flush` which flushes events in the buffer to be sent immediately.
+          - Introduced new method `EventHubProducerClient.get_buffered_event_count` which returns the number of events that are buffered and waiting to be published for a given partition.
+          - Introduced new property `EventHubProducerClient.total_buffered_event_count` which returns the total number of events that are currently buffered and waiting to be published, across all partitions.
+          - Introduced new boolean keyword argument `flush` to `EventHubProducerClient.close` which indicates whether to flush the buffer or not while closing.
+        
+        ### Other Changes
+        
+        - Updated `EventData` internals for interoperability with the Schema Registry Avro Encoder library.
+        
         ## 5.9.0b2 (2022-03-09)
         
         ### Breaking Changes
         
         - `from_message_data` on `EventData` has been renamed `from_message_content` for interoperability with the Schema Registry Avro Encoder library. The `data` parameter has been renamed to `content`.
         
         ## 5.9.0b1 (2022-02-09)
@@ -996,23 +1019,14 @@
         
         ## 0.2.0b1 (2018-04-20)
         
         - Updated uAMQP to latest version.
         - Further testing and minor bug fixes.
         
         
-        ## 0.2.0a2 (2018-04-02)
-        
-        - Updated uAQMP dependency.
-        
-        
-        ## 0.2.0a1 (unreleased)
-        
-        - Swapped out Proton dependency for uAMQP.
-        
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/eventhub/azure-eventhub/HISTORY.png)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `azure-eventhub-5.9.0b2/azure_eventhub.egg-info/SOURCES.txt` & `azure-eventhub-5.9.0b3/azure_eventhub.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 azure/eventhub/_mixin.py
 azure/eventhub/_producer.py
 azure/eventhub/_producer_client.py
 azure/eventhub/_utils.py
 azure/eventhub/_version.py
 azure/eventhub/exceptions.py
 azure/eventhub/py.typed
+azure/eventhub/_buffered_producer/__init__.py
+azure/eventhub/_buffered_producer/_buffered_producer.py
+azure/eventhub/_buffered_producer/_buffered_producer_dispatcher.py
+azure/eventhub/_buffered_producer/_partition_resolver.py
 azure/eventhub/_eventprocessor/__init__.py
 azure/eventhub/_eventprocessor/_eventprocessor_mixin.py
 azure/eventhub/_eventprocessor/checkpoint_store.py
 azure/eventhub/_eventprocessor/common.py
 azure/eventhub/_eventprocessor/event_processor.py
 azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py
 azure/eventhub/_eventprocessor/ownership_manager.py
@@ -34,14 +38,18 @@
 azure/eventhub/aio/_client_base_async.py
 azure/eventhub/aio/_connection_manager_async.py
 azure/eventhub/aio/_consumer_async.py
 azure/eventhub/aio/_consumer_client_async.py
 azure/eventhub/aio/_error_async.py
 azure/eventhub/aio/_producer_async.py
 azure/eventhub/aio/_producer_client_async.py
+azure/eventhub/aio/_buffered_producer/__init__.py
+azure/eventhub/aio/_buffered_producer/_buffered_producer_async.py
+azure/eventhub/aio/_buffered_producer/_buffered_producer_dispatcher_async.py
+azure/eventhub/aio/_buffered_producer/_partition_resolver_async.py
 azure/eventhub/aio/_eventprocessor/__init__.py
 azure/eventhub/aio/_eventprocessor/_ownership_manager.py
 azure/eventhub/aio/_eventprocessor/checkpoint_store.py
 azure/eventhub/aio/_eventprocessor/event_processor.py
 azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py
 azure/eventhub/aio/_eventprocessor/partition_context.py
 azure/eventhub/aio/_eventprocessor/utils.py
@@ -76,14 +84,15 @@
 samples/async_samples/recv_with_checkpoint_by_event_count_async.py
 samples/async_samples/recv_with_checkpoint_by_time_interval_async.py
 samples/async_samples/recv_with_checkpoint_store_async.py
 samples/async_samples/recv_with_custom_starting_position_async.py
 samples/async_samples/sample_code_eventhub_async.py
 samples/async_samples/send_and_receive_amqp_annotated_message_async.py
 samples/async_samples/send_async.py
+samples/async_samples/send_buffered_mode_async.py
 samples/async_samples/send_stream_async.py
 samples/sync_samples/authenticate_with_azure_named_key_credential.py
 samples/sync_samples/authenticate_with_azure_sas_credential.py
 samples/sync_samples/authenticate_with_sas_token.py
 samples/sync_samples/client_creation.py
 samples/sync_samples/client_identity_authentication.py
 samples/sync_samples/connection_string_authentication.py
@@ -96,25 +105,28 @@
 samples/sync_samples/recv_with_checkpoint_by_event_count.py
 samples/sync_samples/recv_with_checkpoint_by_time_interval.py
 samples/sync_samples/recv_with_checkpoint_store.py
 samples/sync_samples/recv_with_custom_starting_position.py
 samples/sync_samples/sample_code_eventhub.py
 samples/sync_samples/send.py
 samples/sync_samples/send_and_receive_amqp_annotated_message.py
+samples/sync_samples/send_buffered_mode.py
 samples/sync_samples/send_stream.py
 tests/eventhub_preparer.py
 tests/livetest/asynctests/test_auth_async.py
+tests/livetest/asynctests/test_buffered_producer_async.py
 tests/livetest/asynctests/test_consumer_client_async.py
 tests/livetest/asynctests/test_eventprocessor_async.py
 tests/livetest/asynctests/test_negative_async.py
 tests/livetest/asynctests/test_properties_async.py
 tests/livetest/asynctests/test_receive_async.py
 tests/livetest/asynctests/test_reconnect_async.py
 tests/livetest/asynctests/test_send_async.py
 tests/livetest/synctests/test_auth.py
+tests/livetest/synctests/test_buffered_producer.py
 tests/livetest/synctests/test_consumer_client.py
 tests/livetest/synctests/test_eventprocessor.py
 tests/livetest/synctests/test_negative.py
 tests/livetest/synctests/test_properties.py
 tests/livetest/synctests/test_receive.py
 tests/livetest/synctests/test_reconnect.py
 tests/livetest/synctests/test_send.py
@@ -128,9 +140,11 @@
 tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py
 tests/perfstress_tests/T1_legacy_tests/send_event.py
 tests/perfstress_tests/T1_legacy_tests/send_event_batch.py
 tests/unittest/test_client_creation.py
 tests/unittest/test_connection_string_parser.py
 tests/unittest/test_dict_mixin.py
 tests/unittest/test_event_data.py
+tests/unittest/test_partition_resolver.py
 tests/unittest/asynctests/test_client_creation_async.py
-tests/unittest/asynctests/test_in_memory_checkpointstore.py
+tests/unittest/asynctests/test_in_memory_checkpointstore.py
+tests/unittest/asynctests/test_partition_resolver_async.py
```

## Comparing `azure-eventhub-5.9.0b2/azure_eventhub.egg-info/PKG-INFO` & `azure-eventhub-5.9.0b3/azure_eventhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-eventhub
-Version: 5.9.0b2
+Version: 5.9.0b3
 Summary: Microsoft Azure Event Hubs Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventhub/azure-eventhub
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Azure Event Hubs client library for Python
         
@@ -478,14 +478,37 @@
         [schemaregistry_avroencoder_repo]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/schemaregistry/azure-schemaregistry-avroencoder
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/eventhub/azure-eventhub/README.png)
         
         
         # Release History
         
+        ## 5.9.0b3 (2022-04-20)
+        
+        ### Features Added
+        
+        - Introduced new method `send_event` to `EventHubProducerClient` which allows sending single `EventData` or `AmqpAnnotatedMessage`.
+        - Introduced buffered mode sending to `EventHubProducerClient` which is intended to allow for efficient publishing of events
+         without having to explicitly manage batches in the application.
+          - The constructor of `EventHubProducerClient` and `from_connection_string` method now takes the following new keyword arguments
+           for configuration:
+            - `buffered_mode`: The flag to enable/disable buffered mode sending.
+            - `on_success`: The callback to be called once events have been successfully published.
+            - `on_error`: The callback to be called once events have failed to be published.
+            - `max_buffer_length`: The total number of events per partition that can be buffered before a flush will be triggered.
+            - `max_wait_time`: The amount of time to wait for a batch to be built with events in the buffer before publishing.
+          - Introduced new method `EventHubProducerClient.flush` which flushes events in the buffer to be sent immediately.
+          - Introduced new method `EventHubProducerClient.get_buffered_event_count` which returns the number of events that are buffered and waiting to be published for a given partition.
+          - Introduced new property `EventHubProducerClient.total_buffered_event_count` which returns the total number of events that are currently buffered and waiting to be published, across all partitions.
+          - Introduced new boolean keyword argument `flush` to `EventHubProducerClient.close` which indicates whether to flush the buffer or not while closing.
+        
+        ### Other Changes
+        
+        - Updated `EventData` internals for interoperability with the Schema Registry Avro Encoder library.
+        
         ## 5.9.0b2 (2022-03-09)
         
         ### Breaking Changes
         
         - `from_message_data` on `EventData` has been renamed `from_message_content` for interoperability with the Schema Registry Avro Encoder library. The `data` parameter has been renamed to `content`.
         
         ## 5.9.0b1 (2022-02-09)
@@ -996,23 +1019,14 @@
         
         ## 0.2.0b1 (2018-04-20)
         
         - Updated uAMQP to latest version.
         - Further testing and minor bug fixes.
         
         
-        ## 0.2.0a2 (2018-04-02)
-        
-        - Updated uAQMP dependency.
-        
-        
-        ## 0.2.0a1 (unreleased)
-        
-        - Swapped out Proton dependency for uAMQP.
-        
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/eventhub/azure-eventhub/HISTORY.png)
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `azure-eventhub-5.9.0b2/doc/azure.eventhub.amqp.rst` & `azure-eventhub-5.9.0b3/doc/azure.eventhub.amqp.rst`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/doc/azure.eventhub.rst` & `azure-eventhub-5.9.0b3/doc/azure.eventhub.rst`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/doc/azure.eventhub.exceptions.rst` & `azure-eventhub-5.9.0b3/doc/azure.eventhub.exceptions.rst`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/doc/azure.eventhub.aio.rst` & `azure-eventhub-5.9.0b3/doc/azure.eventhub.aio.rst`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/eventhub_preparer.py` & `azure-eventhub-5.9.0b3/tests/eventhub_preparer.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/_test_base.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/_test_base.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/receive_event_batch.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/receive_event_batch.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/send_event_batch.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/send_event_batch.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/_test_base.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/_test_base.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/receive_event_batch.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py` & `azure-eventhub-5.9.0b3/tests/perfstress_tests/T1_legacy_tests/send_event_batch.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/test_client_creation.py` & `azure-eventhub-5.9.0b3/tests/unittest/test_client_creation.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/test_dict_mixin.py` & `azure-eventhub-5.9.0b3/tests/unittest/test_dict_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/test_event_data.py` & `azure-eventhub-5.9.0b3/tests/unittest/test_event_data.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/test_connection_string_parser.py` & `azure-eventhub-5.9.0b3/tests/unittest/test_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_in_memory_checkpointstore.py` & `azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_in_memory_checkpointstore.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/unittest/asynctests/test_client_creation_async.py` & `azure-eventhub-5.9.0b3/tests/unittest/asynctests/test_client_creation_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_consumer_client.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_consumer_client.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_eventprocessor.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_eventprocessor.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_negative.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_negative.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,34 @@
     client = EventHubProducerClient.from_connection_string(invalid_hostname)
     with client:
         with pytest.raises(ConnectError):
             batch = EventDataBatch()
             batch.add(EventData("test data"))
             client.send_batch(batch)
 
+    # test setting callback
+    def on_error(events, pid, err):
+        assert len(events) == 1
+        assert not pid
+        on_error.err = err
+
+    on_error.err = None
+    client = EventHubProducerClient.from_connection_string(invalid_hostname, on_error=on_error)
+    with client:
+        batch = EventDataBatch()
+        batch.add(EventData("test data"))
+        client.send_batch(batch)
+    assert isinstance(on_error.err, ConnectError)
+
+    on_error.err = None
+    client = EventHubProducerClient.from_connection_string(invalid_hostname, on_error=on_error)
+    with client:
+        client.send_event(EventData("test data"))
+    assert isinstance(on_error.err, ConnectError)
+
 
 @pytest.mark.liveTest
 def test_receive_with_invalid_hostname_sync(invalid_hostname):
     def on_event(partition_context, event):
         pass
 
     client = EventHubConsumerClient.from_connection_string(invalid_hostname, consumer_group='$default')
```

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_send.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_send.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,70 +7,136 @@
 
 import pytest
 import threading
 import time
 import json
 import sys
 
+import uamqp
 from azure.eventhub import EventData, TransportType, EventDataBatch
 from azure.eventhub import EventHubProducerClient, EventHubConsumerClient
-from azure.eventhub.exceptions import EventDataSendError
+from azure.eventhub.exceptions import EventDataSendError, OperationTimeoutError
 from azure.eventhub.amqp import (
     AmqpMessageHeader,
     AmqpMessageBodyType,
     AmqpAnnotatedMessage,
     AmqpMessageProperties,
 )
 
+
 @pytest.mark.liveTest
-def test_send_with_partition_key(connstr_receivers):
+def test_send_with_partition_key(connstr_receivers, live_eventhub):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
         data_val = 0
         for partition in [b"a", b"b", b"c", b"d", b"e", b"f"]:
             partition_key = b"test_partition_" + partition
-            for i in range(50):
+            for i in range(10):
                 batch = client.create_batch(partition_key=partition_key)
                 batch.add(EventData(str(data_val)))
                 data_val += 1
                 client.send_batch(batch)
 
         client.send_batch(client.create_batch())
 
+        for partition in [b"a", b"b", b"c", b"d", b"e", b"f"]:
+            partition_key = b"test_partition_" + partition
+            for i in range(10):
+                event_data = EventData(str(data_val))
+                event_data.properties = {'is_single': True}
+                data_val += 1
+                client.send_event(event_data, partition_key=partition_key)
+
+    batch_cnt = 0
+    single_cnt = 0
     found_partition_keys = {}
+    reconnect_receivers = []
     for index, partition in enumerate(receivers):
-        received = partition.receive_message_batch(timeout=5000)
-        for message in received:
+        retry_total = 0
+        while retry_total < 3:
+            timeout = 5000 + retry_total * 1000
             try:
-                event_data = EventData._from_message(message)
-                existing = found_partition_keys[event_data.partition_key]
-                assert existing == index
-            except KeyError:
-                found_partition_keys[event_data.partition_key] = index
+                received = partition.receive_message_batch(timeout=timeout)
+                for message in received:
+                    try:
+                        event_data = EventData._from_message(message)
+                        if event_data.properties and event_data.properties[b'is_single']:
+                            single_cnt += 1
+                        else:
+                            batch_cnt += 1
+                        existing = found_partition_keys[event_data.partition_key]
+                        assert existing == index
+                    except KeyError:
+                        found_partition_keys[event_data.partition_key] = index
+                if received:
+                    break
+                retry_total += 1
+            except uamqp.errors.ConnectionClose:
+                for r in reconnect_receivers:
+                    r.close()
+                uri = "sb://{}/{}".format(live_eventhub['hostname'], live_eventhub['event_hub'])
+                sas_auth = uamqp.authentication.SASTokenAuth.from_shared_access_key(
+                    uri, live_eventhub['key_name'], live_eventhub['access_key'])
+
+                source = "amqps://{}/{}/ConsumerGroups/{}/Partitions/{}".format(
+                    live_eventhub['hostname'],
+                    live_eventhub['event_hub'],
+                    live_eventhub['consumer_group'],
+                    index)
+                partition = uamqp.ReceiveClient(source, auth=sas_auth, debug=True, timeout=0, prefetch=500)
+                reconnect_receivers.append(partition)
+                retry_total += 1
+        if retry_total == 3:
+            raise OperationTimeoutError(f"Exhausted retries for receiving from {live_eventhub['hostname']}.")
+
+    for r in reconnect_receivers:
+        r.close()
+
+    assert single_cnt == 60
+    assert batch_cnt == 60
+    assert len(found_partition_keys) == 6
 
 
 @pytest.mark.liveTest
 def test_send_and_receive_large_body_size(connstr_receivers):
     if sys.platform.startswith('darwin'):
         pytest.skip("Skipping on OSX - open issue regarding message size")
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
         payload = 250 * 1024
         batch = client.create_batch()
         batch.add(EventData("A" * payload))
         client.send_batch(batch)
+        client.send_event(EventData("A" * payload))
 
     received = []
     for r in receivers:
         received.extend([EventData._from_message(x) for x in r.receive_message_batch(timeout=10000)])
 
-    assert len(received) == 1
+    assert len(received) == 2
+    assert len(list(received[0].body)[0]) == payload
+    assert len(list(received[1].body)[0]) == payload
+
+    client = EventHubProducerClient.from_connection_string(connection_str)
+    with client:
+        payload = 250 * 1024
+        batch = client.create_batch()
+        batch.add(EventData("A" * payload))
+        client.send_batch(batch)
+        client.send_event(EventData("A" * payload))
+
+    received = []
+    for r in receivers:
+        received.extend([EventData._from_message(x) for x in r.receive_message_batch(timeout=10000)])
+
+    assert len(received) == 2
     assert len(list(received[0].body)[0]) == payload
+    assert len(list(received[1].body)[0]) == payload
 
 
 @pytest.mark.liveTest
 def test_send_amqp_annotated_message(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
@@ -120,14 +186,18 @@
         batch = client.create_batch()
         batch.add(data_message)
         batch.add(value_message)
         batch.add(sequence_message)
         batch.add(event_data)
         client.send_batch(batch)
         client.send_batch([data_message, value_message, sequence_message, event_data])
+        client.send_event(data_message)
+        client.send_event(value_message)
+        client.send_event(sequence_message)
+        client.send_event(event_data)
 
     received_count = {}
     received_count["data_msg"] = 0
     received_count["seq_msg"] = 0
     received_count["value_msg"] = 0
     received_count["normal_msg"] = 0
 
@@ -173,91 +243,103 @@
         thread = threading.Thread(target=client.receive, args=(on_event,),
                                   kwargs={"starting_position": "-1"})
         thread.start()
         time.sleep(15)
         for event in on_event.received:
             check_values(event)
 
-    assert len(on_event.received) == 8
-    assert received_count["data_msg"] == 2
-    assert received_count["seq_msg"] == 2
-    assert received_count["value_msg"] == 2
-    assert received_count["normal_msg"] == 2
+    assert len(on_event.received) == 12
+    assert received_count["data_msg"] == 3
+    assert received_count["seq_msg"] == 3
+    assert received_count["value_msg"] == 3
+    assert received_count["normal_msg"] == 3
 
 
 @pytest.mark.parametrize("payload",
                          [b"", b"A single event"])
 @pytest.mark.liveTest
 def test_send_and_receive_small_body(connstr_receivers, payload):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
         batch = client.create_batch()
         batch.add(EventData(payload))
         client.send_batch(batch)
+        client.send_event(EventData(payload))
     received = []
     for r in receivers:
         received.extend([EventData._from_message(x) for x in r.receive_message_batch(timeout=5000)])
 
-    assert len(received) == 1
+    assert len(received) == 2
     assert list(received[0].body)[0] == payload
+    assert list(received[1].body)[0] == payload
 
 
 @pytest.mark.liveTest
 def test_send_partition(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
 
     with client:
         batch = client.create_batch()
         batch.add(EventData(b"Data"))
         client.send_batch(batch)
+        client.send_event(EventData(b"Data"))
 
     with client:
         batch = client.create_batch(partition_id="1")
         batch.add(EventData(b"Data"))
         client.send_batch(batch)
+        client.send_event(EventData(b"Data"), partition_id="1")
 
     partition_0 = receivers[0].receive_message_batch(timeout=5000)
     partition_1 = receivers[1].receive_message_batch(timeout=5000)
-    assert len(partition_0) + len(partition_1) == 2
+    assert len(partition_1) >= 2
+    assert len(partition_0) + len(partition_1) == 4
 
     with client:
         batch = client.create_batch()
         batch.add(EventData(b"Data"))
         client.send_batch(batch)
+        client.send_event(EventData(b"Data"))
 
     with client:
-        batch = client.create_batch(partition_id="1")
+        batch = client.create_batch(partition_id="0")
         batch.add(EventData(b"Data"))
         client.send_batch(batch)
+        client.send_event(EventData(b"Data"), partition_id="0")
 
     partition_0 = receivers[0].receive_message_batch(timeout=5000)
     partition_1 = receivers[1].receive_message_batch(timeout=5000)
-    assert len(partition_0) + len(partition_1) == 2
+    assert len(partition_0) >= 2
+    assert len(partition_0) + len(partition_1) == 4
 
 
 @pytest.mark.liveTest
 def test_send_non_ascii(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
         batch = client.create_batch(partition_id="0")
         batch.add(EventData(u"é,è,à,ù,â,ê,î,ô,û"))
         batch.add(EventData(json.dumps({"foo": u"漢字"})))
         client.send_batch(batch)
+        client.send_event(EventData(u"é,è,à,ù,â,ê,î,ô,û"), partition_id="0")
+        client.send_event(EventData(json.dumps({"foo": u"漢字"})), partition_id="0")
     time.sleep(1)
     # receive_message_batch() returns immediately once it receives any messages before the max_batch_size
     # and timeout reach. Could be 1, 2, or any number between 1 and max_batch_size.
     # So call it twice to ensure the two events are received.
     partition_0 = [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)] + \
                   [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)]
-    assert len(partition_0) == 2
+    assert len(partition_0) == 4
     assert partition_0[0].body_as_str() == u"é,è,à,ù,â,ê,î,ô,û"
     assert partition_0[1].body_as_json() == {"foo": u"漢字"}
+    assert partition_0[2].body_as_str() == u"é,è,à,ù,â,ê,î,ô,û"
+    assert partition_0[3].body_as_json() == {"foo": u"漢字"}
 
 
 @pytest.mark.liveTest
 def test_send_multiple_partitions_with_app_prop(connstr_receivers):
     connection_str, receivers = connstr_receivers
     app_prop_key = "raw_prop"
     app_prop_value = "raw_value"
@@ -265,43 +347,48 @@
     client = EventHubProducerClient.from_connection_string(connection_str)
     with client:
         ed0 = EventData(b"Message 0")
         ed0.properties = app_prop
         batch = client.create_batch(partition_id="0")
         batch.add(ed0)
         client.send_batch(batch)
+        client.send_event(ed0, partition_id="0")
 
         ed1 = EventData(b"Message 1")
         ed1.properties = app_prop
         batch = client.create_batch(partition_id="1")
         batch.add(ed1)
         client.send_batch(batch)
+        client.send_event(ed1, partition_id="1")
 
     partition_0 = [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)]
-    assert len(partition_0) == 1
+    assert len(partition_0) == 2
     assert partition_0[0].properties[b"raw_prop"] == b"raw_value"
+    assert partition_0[1].properties[b"raw_prop"] == b"raw_value"
     partition_1 = [EventData._from_message(x) for x in receivers[1].receive_message_batch(timeout=5000)]
-    assert len(partition_1) == 1
+    assert len(partition_1) == 2
     assert partition_1[0].properties[b"raw_prop"] == b"raw_value"
+    assert partition_1[1].properties[b"raw_prop"] == b"raw_value"
 
 
 @pytest.mark.liveTest
 def test_send_over_websocket_sync(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str, transport_type=TransportType.AmqpOverWebsocket)
 
     with client:
         batch = client.create_batch(partition_id="0")
         batch.add(EventData("Event Data"))
         client.send_batch(batch)
+        client.send_event(EventData("Event Data"), partition_id="0")
 
     time.sleep(1)
     received = []
     received.extend(receivers[0].receive_message_batch(max_batch_size=5, timeout=10000))
-    assert len(received) == 1
+    assert len(received) == 2
 
 
 @pytest.mark.liveTest
 def test_send_with_create_event_batch_with_app_prop_sync(connstr_receivers):
     connection_str, receivers = connstr_receivers
     app_prop_key = "raw_prop"
     app_prop_value = "raw_value"
@@ -367,7 +454,54 @@
 def test_send_batch_pid_pk(invalid_hostname, partition_id, partition_key):
     # Use invalid_hostname because this is not a live test.
     client = EventHubProducerClient.from_connection_string(invalid_hostname)
     batch = EventDataBatch(partition_id=partition_id, partition_key=partition_key)
     with client:
         with pytest.raises(TypeError):
             client.send_batch(batch, partition_id=partition_id, partition_key=partition_key)
+
+
+def test_send_with_callback(connstr_receivers):
+
+    def on_error(events, pid, err):
+        on_error.err = err
+
+    def on_success(events, pid):
+        sent_events.append((events, pid))
+
+    sent_events = []
+    on_error.err = None
+    connection_str, receivers = connstr_receivers
+    client = EventHubProducerClient.from_connection_string(connection_str, on_success=on_success, on_error=on_error)
+
+    with client:
+        batch = client.create_batch()
+        batch.add(EventData(b"Data"))
+        batch.add(EventData(b"Data"))
+        client.send_batch(batch)
+        assert len(sent_events[-1][0]) == 2
+        assert not sent_events[-1][1]
+        client.send_event(EventData(b"Data"))
+        assert len(sent_events[-1][0]) == 1
+        assert not sent_events[-1][1]
+
+        batch = client.create_batch(partition_key='key')
+        batch.add(EventData(b"Data"))
+        batch.add(EventData(b"Data"))
+        client.send_batch(batch)
+        assert len(sent_events[-1][0]) == 2
+        assert not sent_events[-1][1]
+        client.send_event(EventData(b"Data"), partition_key='key')
+        assert len(sent_events[-1][0]) == 1
+        assert not sent_events[-1][1]
+
+        batch = client.create_batch(partition_id="0")
+        batch.add(EventData(b"Data"))
+        client.send_batch(batch)
+        batch.add(EventData(b"Data"))
+        assert len(sent_events[-1][0]) == 2
+        assert sent_events[-1][1] == "0"
+        client.send_event(EventData(b"Data"), partition_id="0")
+        assert len(sent_events[-1][0]) == 1
+        assert sent_events[-1][1] == "0"
+
+        assert not on_error.err
```

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_auth.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_auth.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_receive.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_receive.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_reconnect.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_reconnect.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/synctests/test_properties.py` & `azure-eventhub-5.9.0b3/tests/livetest/synctests/test_properties.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_consumer_client_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_consumer_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_send_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_send_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 #--------------------------------------------------------------------------
 
 import os
 import asyncio
 import pytest
 import time
 import json
+import uamqp
 
 from azure.eventhub import EventData, TransportType, EventDataBatch
 from azure.eventhub.aio import EventHubProducerClient, EventHubConsumerClient
-from azure.eventhub.exceptions import EventDataSendError
+from azure.eventhub.exceptions import EventDataSendError, OperationTimeoutError
 from azure.eventhub.amqp import (
     AmqpMessageHeader,
     AmqpMessageBodyType,
     AmqpAnnotatedMessage,
     AmqpMessageProperties,
 )
 
@@ -73,14 +74,18 @@
         batch = await client.create_batch()
         batch.add(data_message)
         batch.add(value_message)
         batch.add(sequence_message)
         batch.add(event_data)
         await client.send_batch(batch)
         await client.send_batch([data_message, value_message, sequence_message, event_data])
+        await client.send_event(data_message)
+        await client.send_event(value_message)
+        await client.send_event(sequence_message)
+        await client.send_event(event_data)
 
     received_count = {}
     received_count["data_msg"] = 0
     received_count["seq_msg"] = 0
     received_count["value_msg"] = 0
     received_count["normal_msg"] = 0
 
@@ -126,123 +131,180 @@
         task = asyncio.ensure_future(client.receive(on_event, starting_position="-1"))
         await asyncio.sleep(15)
         for event in on_event.received:
             check_values(event)
 
     await task
 
-    assert len(on_event.received) == 8
-    assert received_count["data_msg"] == 2
-    assert received_count["seq_msg"] == 2
-    assert received_count["value_msg"] == 2
-    assert received_count["normal_msg"] == 2
+    assert len(on_event.received) == 12
+    assert received_count["data_msg"] == 3
+    assert received_count["seq_msg"] == 3
+    assert received_count["value_msg"] == 3
+    assert received_count["normal_msg"] == 3
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
-async def test_send_with_partition_key_async(connstr_receivers):
+async def test_send_with_partition_key_async(connstr_receivers, live_eventhub):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     async with client:
         data_val = 0
         for partition in [b"a", b"b", b"c", b"d", b"e", b"f"]:
             partition_key = b"test_partition_" + partition
-            for i in range(50):
+            for i in range(10):
                 batch = await client.create_batch(partition_key=partition_key)
                 batch.add(EventData(str(data_val)))
                 data_val += 1
                 await client.send_batch(batch)
 
         await client.send_batch(await client.create_batch())
 
+        for partition in [b"a", b"b", b"c", b"d", b"e", b"f"]:
+            partition_key = b"test_partition_" + partition
+            for i in range(10):
+                event_data = EventData(str(data_val))
+                event_data.properties = {'is_single': True}
+                data_val += 1
+                await client.send_event(event_data, partition_key=partition_key)
+
+    batch_cnt = 0
+    single_cnt = 0
     found_partition_keys = {}
+    reconnect_receivers = []
     for index, partition in enumerate(receivers):
-        received = partition.receive_message_batch(timeout=5000)
-        for message in received:
+        retry_total = 0
+        while retry_total < 3:
+            timeout = 5000 + retry_total * 1000
             try:
-                event_data = EventData._from_message(message)
-                existing = found_partition_keys[event_data.partition_key]
-                assert existing == index
-            except KeyError:
-                found_partition_keys[event_data.partition_key] = index
+                received = partition.receive_message_batch(timeout=timeout)
+                for message in received:
+                    try:
+                        event_data = EventData._from_message(message)
+                        if event_data.properties and event_data.properties[b'is_single']:
+                            single_cnt += 1
+                        else:
+                            batch_cnt += 1
+                        existing = found_partition_keys[event_data.partition_key]
+                        assert existing == index
+                    except KeyError:
+                        found_partition_keys[event_data.partition_key] = index
+                if received:
+                    break
+                retry_total += 1
+            except uamqp.errors.ConnectionClose:
+                for r in reconnect_receivers:
+                    r.close()
+                uri = "sb://{}/{}".format(live_eventhub['hostname'], live_eventhub['event_hub'])
+                sas_auth = uamqp.authentication.SASTokenAuth.from_shared_access_key(
+                    uri, live_eventhub['key_name'], live_eventhub['access_key'])
+
+                source = "amqps://{}/{}/ConsumerGroups/{}/Partitions/{}".format(
+                    live_eventhub['hostname'],
+                    live_eventhub['event_hub'],
+                    live_eventhub['consumer_group'],
+                    index)
+                partition = uamqp.ReceiveClient(source, auth=sas_auth, debug=True, timeout=0, prefetch=500)
+                reconnect_receivers.append(partition)
+                retry_total += 1
+        if retry_total == 3:
+            raise OperationTimeoutError(f"Exhausted retries for receiving from {live_eventhub['hostname']}.")
+    for r in reconnect_receivers:
+        r.close()
+
+    assert single_cnt == 60
+    assert batch_cnt == 60
+    assert len(found_partition_keys) == 6
 
 
 @pytest.mark.parametrize("payload", [b"", b"A single event"])
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_and_receive_small_body_async(connstr_receivers, payload):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     async with client:
         batch = await client.create_batch()
         batch.add(EventData(payload))
         await client.send_batch(batch)
+        await client.send_event(EventData(payload))
     received = []
     for r in receivers:
         received.extend([EventData._from_message(x) for x in r.receive_message_batch(timeout=5000)])
 
-    assert len(received) == 1
+    assert len(received) == 2
     assert list(received[0].body)[0] == payload
+    assert list(received[1].body)[0] == payload
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_partition_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
 
     async with client:
         batch = await client.create_batch()
         batch.add(EventData(b"Data"))
         await client.send_batch(batch)
+        await client.send_event(EventData(b"Data"))
 
     async with client:
         batch = await client.create_batch(partition_id="1")
         batch.add(EventData(b"Data"))
         await client.send_batch(batch)
+        await client.send_event(EventData(b"Data"), partition_id="1")
 
     partition_0 = receivers[0].receive_message_batch(timeout=5000)
     partition_1 = receivers[1].receive_message_batch(timeout=5000)
-    assert len(partition_0) + len(partition_1) == 2
+    assert len(partition_1) >= 2
+    assert len(partition_0) + len(partition_1) == 4
 
     async with client:
         batch = await client.create_batch()
         batch.add(EventData(b"Data"))
         await client.send_batch(batch)
+        await client.send_event(EventData(b"Data"))
 
     async with client:
-        batch = await client.create_batch(partition_id="1")
+        batch = await client.create_batch(partition_id="0")
         batch.add(EventData(b"Data"))
         await client.send_batch(batch)
+        await client.send_event(EventData(b"Data"), partition_id="0")
 
     partition_0 = receivers[0].receive_message_batch(timeout=5000)
     partition_1 = receivers[1].receive_message_batch(timeout=5000)
-    assert len(partition_0) + len(partition_1) == 2
+    assert len(partition_0) >= 2
+    assert len(partition_0) + len(partition_1) == 4
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_non_ascii_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     async with client:
         batch = await client.create_batch(partition_id="0")
         batch.add(EventData(u"é,è,à,ù,â,ê,î,ô,û"))
         batch.add(EventData(json.dumps({"foo": u"漢字"})))
         await client.send_batch(batch)
+        await client.send_event(EventData(u"é,è,à,ù,â,ê,î,ô,û"), partition_id="0")
+        await client.send_event(EventData(json.dumps({"foo": u"漢字"})), partition_id="0")
     await asyncio.sleep(1)
     # receive_message_batch() returns immediately once it receives any messages before the max_batch_size
     # and timeout reach. Could be 1, 2, or any number between 1 and max_batch_size.
     # So call it twice to ensure the two events are received.
     partition_0 = [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)] + \
                   [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)]
 
-    assert len(partition_0) == 2
+    assert len(partition_0) == 4
     assert partition_0[0].body_as_str() == u"é,è,à,ù,â,ê,î,ô,û"
     assert partition_0[1].body_as_json() == {"foo": u"漢字"}
+    assert partition_0[2].body_as_str() == u"é,è,à,ù,â,ê,î,ô,û"
+    assert partition_0[3].body_as_json() == {"foo": u"漢字"}
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_multiple_partition_with_app_prop_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     app_prop_key = "raw_prop"
@@ -251,45 +313,50 @@
     client = EventHubProducerClient.from_connection_string(connection_str)
     async with client:
         ed0 = EventData(b"Message 0")
         ed0.properties = app_prop
         batch = await client.create_batch(partition_id="0")
         batch.add(ed0)
         await client.send_batch(batch)
+        await client.send_event(ed0, partition_id="0")
 
         ed1 = EventData(b"Message 1")
         ed1.properties = app_prop
         batch = await client.create_batch(partition_id="1")
         batch.add(ed1)
         await client.send_batch(batch)
+        await client.send_event(ed1, partition_id="1")
 
     partition_0 = [EventData._from_message(x) for x in receivers[0].receive_message_batch(timeout=5000)]
-    assert len(partition_0) == 1
+    assert len(partition_0) == 2
     assert partition_0[0].properties[b"raw_prop"] == b"raw_value"
+    assert partition_0[1].properties[b"raw_prop"] == b"raw_value"
     partition_1 = [EventData._from_message(x) for x in receivers[1].receive_message_batch(timeout=5000)]
-    assert len(partition_1) == 1
+    assert len(partition_1) == 2
     assert partition_1[0].properties[b"raw_prop"] == b"raw_value"
+    assert partition_0[1].properties[b"raw_prop"] == b"raw_value"
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_over_websocket_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str,
                                                            transport_type=TransportType.AmqpOverWebsocket)
 
     async with client:
         batch = await client.create_batch(partition_id="0")
         batch.add(EventData("Event Data"))
         await client.send_batch(batch)
+        await client.send_event(EventData("Event Data"), partition_id="0")
 
     time.sleep(1)
     received = []
     received.extend(receivers[0].receive_message_batch(max_batch_size=5, timeout=10000))
-    assert len(received) == 1
+    assert len(received) == 2
 
 
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_with_create_event_batch_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     app_prop_key = "raw_prop"
@@ -310,15 +377,14 @@
         received = []
         for r in receivers:
             received.extend(r.receive_message_batch(timeout=10000))
         assert len(received) >= 1
         assert EventData._from_message(received[0]).properties[b"raw_prop"] == b"raw_value"
 
 
-
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_send_list_async(connstr_receivers):
     connection_str, receivers = connstr_receivers
     client = EventHubProducerClient.from_connection_string(connection_str)
     payload = "A1"
     async with client:
@@ -363,7 +429,56 @@
 async def test_send_batch_pid_pk_async(invalid_hostname, partition_id, partition_key):
     # Use invalid_hostname because this is not a live test.
     client = EventHubProducerClient.from_connection_string(invalid_hostname)
     batch = EventDataBatch(partition_id=partition_id, partition_key=partition_key)
     async with client:
         with pytest.raises(TypeError):
             await client.send_batch(batch, partition_id=partition_id, partition_key=partition_key)
+
+
+@pytest.mark.liveTest
+@pytest.mark.asyncio
+async def test_send_with_callback_async(connstr_receivers):
+
+    async def on_error(events, pid, err):
+        on_error.err = err
+
+    async def on_success(events, pid):
+        sent_events.append((events, pid))
+
+    sent_events = []
+    on_error.err = None
+    connection_str, receivers = connstr_receivers
+    client = EventHubProducerClient.from_connection_string(connection_str, on_success=on_success, on_error=on_error)
+
+    async with client:
+        batch = await client.create_batch()
+        batch.add(EventData(b"Data"))
+        batch.add(EventData(b"Data"))
+        await client.send_batch(batch)
+        assert len(sent_events[-1][0]) == 2
+        assert not sent_events[-1][1]
+        await client.send_event(EventData(b"Data"))
+        assert len(sent_events[-1][0]) == 1
+        assert not sent_events[-1][1]
+
+        batch = await client.create_batch(partition_key='key')
+        batch.add(EventData(b"Data"))
+        batch.add(EventData(b"Data"))
+        await client.send_batch(batch)
+        assert len(sent_events[-1][0]) == 2
+        assert not sent_events[-1][1]
+        await client.send_event(EventData(b"Data"), partition_key='key')
+        assert len(sent_events[-1][0]) == 1
+        assert not sent_events[-1][1]
+
+        batch = await client.create_batch(partition_id="0")
+        batch.add(EventData(b"Data"))
+        await client.send_batch(batch)
+        batch.add(EventData(b"Data"))
+        assert len(sent_events[-1][0]) == 2
+        assert sent_events[-1][1] == "0"
+        await client.send_event(EventData(b"Data"), partition_id="0")
+        assert len(sent_events[-1][0]) == 1
+        assert sent_events[-1][1] == "0"
+
+        assert not on_error.err
```

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_properties_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_properties_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_eventprocessor_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_eventprocessor_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_receive_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_receive_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_reconnect_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_reconnect_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_negative_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_negative_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,34 @@
     client = EventHubProducerClient.from_connection_string(invalid_hostname)
     async with client:
         with pytest.raises(ConnectError):
             batch = EventDataBatch()
             batch.add(EventData("test data"))
             await client.send_batch(batch)
 
+    # test setting callback
+    async def on_error(events, pid, err):
+        assert len(events) == 1
+        assert not pid
+        on_error.err = err
+
+    on_error.err = None
+    client = EventHubProducerClient.from_connection_string(invalid_hostname, on_error=on_error)
+    async with client:
+        batch = EventDataBatch()
+        batch.add(EventData("test data"))
+        await client.send_batch(batch)
+    assert isinstance(on_error.err, ConnectError)
+
+    on_error.err = None
+    client = EventHubProducerClient.from_connection_string(invalid_hostname, on_error=on_error)
+    async with client:
+        await client.send_event(EventData("test data"))
+    assert isinstance(on_error.err, ConnectError)
+
 
 @pytest.mark.parametrize("invalid_place",
                          ["hostname", "key_name", "access_key", "event_hub", "partition"])
 @pytest.mark.liveTest
 @pytest.mark.asyncio
 async def test_receive_with_invalid_param_async(live_eventhub, invalid_place):
     eventhub_config = live_eventhub.copy()
```

## Comparing `azure-eventhub-5.9.0b2/tests/livetest/asynctests/test_auth_async.py` & `azure-eventhub-5.9.0b3/tests/livetest/asynctests/test_auth_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_track_last_enqueued_event_prop_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_track_last_enqueued_event_prop_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_with_custom_starting_position_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_with_custom_starting_position_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/client_creation_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/client_creation_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/receive_batch_with_checkpoint_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/receive_batch_with_checkpoint_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_named_key_credential_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_named_key_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/iot_hub_connection_string_receive_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/iot_hub_connection_string_receive_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/connection_to_custom_endpoint_address_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/connection_to_custom_endpoint_address_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/send_and_receive_amqp_annotated_message_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/send_and_receive_amqp_annotated_message_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/send_stream_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/send_stream_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/send_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/send_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_event_count_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_event_count_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_by_time_interval_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_azure_sas_credential_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_azure_sas_credential_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/sample_code_eventhub_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/sample_code_eventhub_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_for_period_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_for_period_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/client_identity_authentication_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/client_identity_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/recv_with_checkpoint_store_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/recv_with_checkpoint_store_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/connection_string_authentication_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/connection_string_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/proxy_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/proxy_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/async_samples/authenticate_with_sas_token_async.py` & `azure-eventhub-5.9.0b3/samples/async_samples/authenticate_with_sas_token_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_sas_token.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_sas_token.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_sas_credential.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_sas_credential.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_store.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_store.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_custom_starting_position.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_custom_starting_position.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/authenticate_with_azure_named_key_credential.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/authenticate_with_azure_named_key_credential.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_time_interval.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_time_interval.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/client_creation.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/client_creation.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/proxy.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/proxy.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/connection_to_custom_endpoint_address.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/connection_to_custom_endpoint_address.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/send.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/send.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_track_last_enqueued_event_prop.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_track_last_enqueued_event_prop.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_with_checkpoint_by_event_count.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_with_checkpoint_by_event_count.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/send_stream.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/send_stream.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/send_and_receive_amqp_annotated_message.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/send_and_receive_amqp_annotated_message.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/connection_string_authentication.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/connection_string_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/client_identity_authentication.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/client_identity_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/receive_batch_with_checkpoint.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/receive_batch_with_checkpoint.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv_for_period.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv_for_period.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/sample_code_eventhub.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/sample_code_eventhub.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/samples/sync_samples/recv.py` & `azure-eventhub-5.9.0b3/samples/sync_samples/recv.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_constants.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_configuration.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_consumer_client.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_consumer_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,35 +11,31 @@
 from ._constants import ALL_PARTITIONS
 from ._eventprocessor.event_processor import EventProcessor
 from ._eventprocessor.common import LoadBalancingStrategy
 
 
 if TYPE_CHECKING:
     import datetime
-    from azure.core.credentials import (
-        TokenCredential,
-        AzureSasCredential,
-        AzureNamedKeyCredential,
-    )
     from typing import (  # pylint: disable=ungrouped-imports
         Any,
         Union,
         Dict,
         Tuple,
         Callable,
         List,
         Optional,
     )
     from ._eventprocessor.partition_context import PartitionContext
     from ._common import EventData
+    from ._client_base import CredentialTypes
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class EventHubConsumerClient(ClientBase):
+class EventHubConsumerClient(ClientBase):   # pylint: disable=client-accepts-api-version-keyword
     """The EventHubConsumerClient class defines a high level interface for
     receiving events from the Azure Event Hubs service.
 
     The main goal of `EventHubConsumerClient` is to receive events from all partitions of an EventHub with
     load-balancing and checkpointing.
 
     When multiple `EventHubConsumerClient` instances are running against the same event hub, consumer group and
@@ -140,15 +136,15 @@
     """
 
     def __init__(
         self,
         fully_qualified_namespace,  # type: str
         eventhub_name,  # type: str
         consumer_group,  # type: str
-        credential,  # type: Union[AzureSasCredential, TokenCredential, AzureNamedKeyCredential]
+        credential,  # type: CredentialTypes
         **kwargs  # type: Any
     ):
         # type: (...) -> None
         self._checkpoint_store = kwargs.pop("checkpoint_store", None)
         self._load_balancing_interval = kwargs.pop("load_balancing_interval", None)
         if self._load_balancing_interval is None:
             self._load_balancing_interval = 10
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_connection_manager.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_connection_manager.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_client_base.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     JWT_TOKEN_SCOPE,
     MGMT_OPERATION,
     MGMT_PARTITION_OPERATION,
     MGMT_STATUS_CODE,
     MGMT_STATUS_DESC,
 )
 
-if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
 
 _LOGGER = logging.getLogger(__name__)
 _Address = collections.namedtuple("_Address", "hostname path")
 
 
 def _parse_conn_str(conn_str, **kwargs):
     # type: (str, Any) -> Tuple[str, Optional[str], Optional[str], str, Optional[str], Optional[int]]
@@ -260,17 +258,27 @@
         """
         This method is automatically called when token is about to expire.
         """
         signature, expiry = parse_sas_credential(self._credential)
         return AccessToken(signature, expiry)
 
 
+if TYPE_CHECKING:
+    from azure.core.credentials import TokenCredential
+    CredentialTypes = Union[
+        AzureSasCredential,
+        AzureNamedKeyCredential,
+        EventHubSharedKeyCredential,
+        TokenCredential
+    ]
+
+
 class ClientBase(object):  # pylint:disable=too-many-instance-attributes
     def __init__(self, fully_qualified_namespace, eventhub_name, credential, **kwargs):
-        # type: (str, str, Union[AzureSasCredential, TokenCredential, AzureNamedKeyCredential], Any) -> None
+        # type: (str, str, CredentialTypes, Any) -> None
         self.eventhub_name = eventhub_name
         if not eventhub_name:
             raise ValueError("The eventhub name can not be None or empty.")
         path = "/" + eventhub_name if eventhub_name else ""
         self._address = _Address(hostname=fully_qualified_namespace, path=path)
         self._container_id = CONTAINER_PREFIX + str(uuid.uuid4())[:8]
         if isinstance(credential, AzureSasCredential):
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_common.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     AnyStr,
     Iterable,
     Optional,
     List,
     TYPE_CHECKING,
     cast,
 )
+from typing_extensions import TypedDict
 
 import six
 
 from uamqp import BatchMessage, Message, constants
 
 from ._utils import (
     set_message_partition_key,
@@ -56,14 +57,15 @@
     AmqpMessageHeader,
     AmqpMessageProperties,
 )
 
 if TYPE_CHECKING:
     import datetime
 
+MessageContent = TypedDict("MessageContent", {"content": bytes, "content_type": str})
 PrimitiveTypes = Optional[Union[
     int,
     float,
     bytes,
     bool,
     str,
     Dict,
@@ -178,24 +180,25 @@
             if self.enqueued_time:
                 event_str += ", enqueued_time={!r}".format(self.enqueued_time)
         except:  # pylint: disable=bare-except
             pass
         event_str += " }"
         return event_str
 
-    def __message_content__(self) -> Dict:
+    def __message_content__(self) -> MessageContent:
         if self.body_type != AmqpMessageBodyType.DATA:
             raise TypeError('`body_type` must be `AmqpMessageBodyType.DATA`.')
         content = bytearray()
         for c in self.body: # type: ignore
             content += c   # type: ignore
-        return {"content": bytes(content), "content_type": self.content_type}
+        content_type = cast(str, self.content_type)
+        return {"content": bytes(content), "content_type": content_type}
 
     @classmethod
-    def from_message_content(cls, content: bytes, content_type: str) -> "EventData":
+    def from_message_content(cls, content: bytes, content_type: str, **kwargs: Any) -> "EventData": # pylint: disable=unused-argument
         """
         Creates an EventData object given content type and a content value to be set as body.
 
         :param bytes content: The content value to be set as the body of the message.
         :param str content_type: The content type to be set on the message.
         :rtype: ~azure.eventhub.EventData
         """
@@ -527,14 +530,15 @@
         self.message = BatchMessage(data=[], multi_messages=False, properties=None)
         self._partition_id = partition_id
         self._partition_key = partition_key
 
         set_message_partition_key(self.message, self._partition_key)
         self._size = self.message.gather()[0].get_message_encoded_size()
         self._count = 0
+        self._internal_events: List[Union[EventData, AmqpAnnotatedMessage]] = []
 
     def __repr__(self):
         # type: () -> str
         batch_repr = "max_size_in_bytes={}, partition_id={}, partition_key={!r}, event_count={}".format(
             self.max_size_in_bytes, self._partition_id, self._partition_key, self._count
         )
         return "EventDataBatch({})".format(batch_repr)
@@ -543,17 +547,16 @@
         return self._count
 
     @classmethod
     def _from_batch(cls, batch_data, partition_key=None):
         # type: (Iterable[EventData], Optional[AnyStr]) -> EventDataBatch
         outgoing_batch_data = [transform_outbound_single_message(m, EventData) for m in batch_data]
         batch_data_instance = cls(partition_key=partition_key)
-        batch_data_instance.message._body_gen = (  # pylint:disable=protected-access
-            outgoing_batch_data
-        )
+        for data in outgoing_batch_data:
+            batch_data_instance.add(data)
         return batch_data_instance
 
     def _load_events(self, events):
         for event_data in events:
             try:
                 self.add(event_data)
             except ValueError:
@@ -614,11 +617,11 @@
 
         if size_after_add > self.max_size_in_bytes:
             raise ValueError(
                 "EventDataBatch has reached its size limit: {}".format(
                     self.max_size_in_bytes
                 )
             )
-
+        self._internal_events.append(event_data)
         self.message._body_gen.append(outgoing_event_data)  # pylint: disable=protected-access
         self._size = size_after_add
         self._count += 1
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_connection_string_parser.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_producer.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_producer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     create_properties,
     set_message_partition_key,
     trace_message,
     send_context_manager,
     transform_outbound_single_message,
 )
 from ._constants import TIMEOUT_SYMBOL
+from .amqp import AmqpAnnotatedMessage
 
 _LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from uamqp.authentication import JWTTokenAuth  # pylint: disable=ungrouped-imports
     from ._producer_client import EventHubProducerClient
 
@@ -180,29 +181,31 @@
 
         """
         self._outcome = outcome
         self._condition = condition
 
     def _wrap_eventdata(
         self,
-        event_data,  # type: Union[EventData, EventDataBatch, Iterable[EventData]]
+        event_data,  # type: Union[EventData, AmqpAnnotatedMessage, EventDataBatch, Iterable[EventData]]
         span,  # type: Optional[AbstractSpan]
         partition_key,  # type: Optional[AnyStr]
     ):
         # type: (...) -> Union[EventData, EventDataBatch]
-        if isinstance(event_data, EventData):
+        if isinstance(event_data, (EventData, AmqpAnnotatedMessage)):
             outgoing_event_data = transform_outbound_single_message(event_data, EventData)
             if partition_key:
                 set_message_partition_key(outgoing_event_data.message, partition_key)
             wrapper_event_data = outgoing_event_data
             trace_message(wrapper_event_data, span)
         else:
             if isinstance(
                 event_data, EventDataBatch
             ):  # The partition_key in the param will be omitted.
+                if not event_data:
+                    return event_data
                 if (
                     partition_key and partition_key != event_data._partition_key  # pylint: disable=protected-access
                 ):
                     raise ValueError(
                         "The partition_key does not match the one of the EventDataBatch"
                     )
                 for event in event_data.message._body_gen: # pylint: disable=protected-access
@@ -214,15 +217,15 @@
                 event_data = _set_trace_message(event_data, span)
                 wrapper_event_data = EventDataBatch._from_batch(event_data, partition_key)  # type: ignore  # pylint: disable=protected-access
         wrapper_event_data.message.on_send_complete = self._on_outcome
         return wrapper_event_data
 
     def send(
         self,
-        event_data,  # type: Union[EventData, EventDataBatch, Iterable[EventData]]
+        event_data,  # type: Union[EventData, AmqpAnnotatedMessage, EventDataBatch, Iterable[EventData]]
         partition_key=None,  # type: Optional[AnyStr]
         timeout=None,  # type: Optional[float]
     ):
         # type:(...) -> None
         """
         Sends an event data and blocks until acknowledgement is
         received or operation times out.
@@ -247,14 +250,18 @@
         :rtype: None
         """
         # Tracing code
         with self._lock:
             with send_context_manager() as child:
                 self._check_closed()
                 wrapper_event_data = self._wrap_eventdata(event_data, child, partition_key)
+
+                if not wrapper_event_data:
+                    return
+
                 self._unsent_events = [wrapper_event_data.message]
 
                 if child:
                     self._client._add_span_request_attributes(  # pylint: disable=protected-access
                         child
                     )
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_consumer.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_consumer.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/__init__.py` & `azure-eventhub-5.9.0b3/azure/eventhub/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_mixin.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_utils.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from uamqp import types
 from uamqp.message import MessageHeader
 
 from azure.core.settings import settings
 from azure.core.tracing import SpanKind, Link
 
-from .amqp import AmqpAnnotatedMessage
+from .amqp import AmqpAnnotatedMessage, AmqpMessageHeader
 from ._version import VERSION
 from ._constants import (
     PROP_PARTITION_KEY_AMQP_SYMBOL,
     MAX_USER_AGENT_LENGTH,
     USER_AGENT_PREFIX,
     PROP_LAST_ENQUEUED_SEQUENCE_NUMBER,
     PROP_LAST_ENQUEUED_TIME_UTC,
@@ -108,14 +108,36 @@
                 MAX_USER_AGENT_LENGTH, final_user_agent, len(final_user_agent)
             )
         )
     properties[types.AMQPSymbol("user-agent")] = final_user_agent
     return properties
 
 
+def set_event_partition_key(event, partition_key):
+    # type: (Union[AmqpAnnotatedMessage, EventData], Optional[Union[bytes, str]]) -> None
+    if not partition_key:
+        return
+
+    try:
+        raw_message = event.raw_amqp_message  # type: ignore
+    except AttributeError:
+        raw_message = event
+
+    annotations = raw_message.annotations
+    if annotations is None:
+        annotations = dict()
+    annotations[
+        PROP_PARTITION_KEY_AMQP_SYMBOL
+    ] = partition_key  # pylint:disable=protected-access
+    if not raw_message.header:
+        raw_message.header = AmqpMessageHeader(header=True)
+    else:
+        raw_message.header.durable = True
+
+
 def set_message_partition_key(message, partition_key):
     # type: (Message, Optional[Union[bytes, str]]) -> None
     """Set the partition key as an annotation on a uamqp message.
 
     :param ~uamqp.Message message: The message to update.
     :param str partition_key: The partition key value.
     :rtype: None
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/exceptions.py` & `azure-eventhub-5.9.0b3/azure/eventhub/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_producer_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_producer_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     create_properties,
     set_message_partition_key,
     trace_message,
     send_context_manager,
     transform_outbound_single_message,
 )
 from .._constants import TIMEOUT_SYMBOL
+from ..amqp import AmqpAnnotatedMessage
 from ._client_base_async import ConsumerProducerMixin
 from ._async_utils import get_dict_with_loop_if_needed
 
 if TYPE_CHECKING:
     from uamqp.authentication import JWTTokenAsync  # pylint: disable=ungrouped-imports
     from ._producer_client_async import EventHubProducerClient
 
@@ -169,19 +170,19 @@
 
         """
         self._outcome = outcome
         self._condition = condition
 
     def _wrap_eventdata(
         self,
-        event_data: Union[EventData, EventDataBatch, Iterable[EventData]],
+        event_data: Union[EventData, AmqpAnnotatedMessage, EventDataBatch, Iterable[EventData]],
         span: Optional[AbstractSpan],
         partition_key: Optional[AnyStr],
     ) -> Union[EventData, EventDataBatch]:
-        if isinstance(event_data, EventData):
+        if isinstance(event_data, (EventData, AmqpAnnotatedMessage)):
             outgoing_event_data = transform_outbound_single_message(event_data, EventData)
             if partition_key:
                 set_message_partition_key(outgoing_event_data.message, partition_key)
             wrapper_event_data = outgoing_event_data
             trace_message(wrapper_event_data, span)
         else:
             if isinstance(
@@ -202,15 +203,15 @@
                 event_data = _set_trace_message(event_data, span)
                 wrapper_event_data = EventDataBatch._from_batch(event_data, partition_key)  # type: ignore  # pylint: disable=protected-access
         wrapper_event_data.message.on_send_complete = self._on_outcome
         return wrapper_event_data
 
     async def send(
         self,
-        event_data: Union[EventData, EventDataBatch, Iterable[EventData]],
+        event_data: Union[EventData, AmqpAnnotatedMessage, EventDataBatch, Iterable[EventData]],
         *,
         partition_key: Optional[AnyStr] = None,
         timeout: Optional[float] = None
     ) -> None:
         """
         Sends an event data and blocks until acknowledgement is
         received or operation times out.
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_error_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_error_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_client_base_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_client_base_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,78 @@
 )
 from ._async_utils import get_dict_with_loop_if_needed
 from ._connection_manager_async import get_connection_manager
 from ._error_async import _handle_exception
 
 if TYPE_CHECKING:
     from azure.core.credentials_async import AsyncTokenCredential
+    CredentialTypes = Union[
+        "EventHubSharedKeyCredential",
+        AsyncTokenCredential,
+        AzureSasCredential,
+        AzureNamedKeyCredential,
+    ]
 
     try:
         from typing_extensions import Protocol
     except ImportError:
         Protocol = object  # type: ignore
 
+    class AbstractConsumerProducer(Protocol):
+        @property
+        def _name(self):
+            # type: () -> str
+            """Name of the consumer or producer"""
+
+        @_name.setter
+        def _name(self, value):
+            pass
+
+        @property
+        def _client(self):
+            # type: () -> ClientBaseAsync
+            """The instance of EventHubComsumerClient or EventHubProducerClient"""
+
+        @_client.setter
+        def _client(self, value):
+            pass
+
+        @property
+        def _handler(self):
+            # type: () -> AMQPClientAsync
+            """The instance of SendClientAsync or ReceiveClientAsync"""
+
+        @property
+        def _internal_kwargs(self):
+            # type: () -> dict
+            """The dict with an event loop that users may pass in to wrap sync calls to async API.
+            It's furthur passed to uamqp APIs
+            """
+
+        @_internal_kwargs.setter
+        def _internal_kwargs(self, value):
+            pass
+
+        @property
+        def running(self):
+            # type: () -> bool
+            """Whether the consumer or producer is running"""
+
+        @running.setter
+        def running(self, value):
+            pass
+
+        def _create_handler(self, auth: authentication.JWTTokenAsync) -> None:
+            pass
+
+    _MIXIN_BASE = AbstractConsumerProducer
+else:
+    _MIXIN_BASE = object
+
+
 _LOGGER = logging.getLogger(__name__)
 
 
 class EventHubSharedKeyCredential(object):
     """The shared access key credential used for authentication.
 
     :param str policy: The name of the shared access policy.
@@ -140,17 +198,15 @@
 
 
 class ClientBaseAsync(ClientBase):
     def __init__(
         self,
         fully_qualified_namespace: str,
         eventhub_name: str,
-        credential: Union[
-            "AsyncTokenCredential", AzureSasCredential, AzureNamedKeyCredential
-        ],
+        credential: "CredentialTypes",
         **kwargs: Any
     ) -> None:
         self._internal_kwargs = get_dict_with_loop_if_needed(kwargs.get("loop", None))
         if isinstance(credential, AzureSasCredential):
             self._credential = EventhubAzureSasTokenCredentialAsync(credential)  # type: ignore
         elif isinstance(credential, AzureNamedKeyCredential):
             self._credential = EventhubAzureNamedKeyTokenCredentialAsync(credential)  # type: ignore
@@ -372,68 +428,14 @@
             )
         return output
 
     async def _close_async(self) -> None:
         await self._conn_manager_async.close_connection()
 
 
-if TYPE_CHECKING:
-
-    class AbstractConsumerProducer(Protocol):
-        @property
-        def _name(self):
-            # type: () -> str
-            """Name of the consumer or producer"""
-
-        @_name.setter
-        def _name(self, value):
-            pass
-
-        @property
-        def _client(self):
-            # type: () -> ClientBaseAsync
-            """The instance of EventHubComsumerClient or EventHubProducerClient"""
-
-        @_client.setter
-        def _client(self, value):
-            pass
-
-        @property
-        def _handler(self):
-            # type: () -> AMQPClientAsync
-            """The instance of SendClientAsync or ReceiveClientAsync"""
-
-        @property
-        def _internal_kwargs(self):
-            # type: () -> dict
-            """The dict with an event loop that users may pass in to wrap sync calls to async API.
-            It's furthur passed to uamqp APIs
-            """
-
-        @_internal_kwargs.setter
-        def _internal_kwargs(self, value):
-            pass
-
-        @property
-        def running(self):
-            # type: () -> bool
-            """Whether the consumer or producer is running"""
-
-        @running.setter
-        def running(self, value):
-            pass
-
-        def _create_handler(self, auth: authentication.JWTTokenAsync) -> None:
-            pass
-
-    _MIXIN_BASE = AbstractConsumerProducer
-else:
-    _MIXIN_BASE = object
-
-
 class ConsumerProducerMixin(_MIXIN_BASE):
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close()
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_client_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,33 @@
     Tuple,
     Callable,
     Optional,
     List,
     Awaitable,
 )
 
-from azure.core.credentials import AzureSasCredential, AzureNamedKeyCredential
-
 from ._eventprocessor.event_processor import EventProcessor
 from ._consumer_async import EventHubConsumer
 from ._client_base_async import ClientBaseAsync
 from .._constants import ALL_PARTITIONS
 from .._eventprocessor.common import LoadBalancingStrategy
 
 
 if TYPE_CHECKING:
-    from azure.core.credentials_async import AsyncTokenCredential
+    from ._client_base_async import CredentialTypes
     from uamqp.constants import TransportType
     from ._eventprocessor.partition_context import PartitionContext
     from ._eventprocessor.checkpoint_store import CheckpointStore
     from .._common import EventData
     from .._eventprocessor.common import CloseReason
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class EventHubConsumerClient(ClientBaseAsync):
+class EventHubConsumerClient(ClientBaseAsync):  # pylint: disable=client-accepts-api-version-keyword
     """The EventHubConsumerClient class defines a high level interface for
     receiving events from the Azure Event Hubs service.
 
     The main goal of `EventHubConsumerClient` is to receive events from all partitions of an EventHub with
     load-balancing and checkpointing.
 
     When multiple `EventHubConsumerClient` instances are running against the same event hub, consumer group and
@@ -143,15 +141,15 @@
     """
 
     def __init__(
         self,
         fully_qualified_namespace: str,
         eventhub_name: str,
         consumer_group: str,
-        credential: Union["AsyncTokenCredential", AzureSasCredential, AzureNamedKeyCredential],
+        credential: "CredentialTypes",
         **kwargs
     ) -> None:
         self._checkpoint_store = kwargs.pop("checkpoint_store", None)
         self._load_balancing_interval = kwargs.pop("load_balancing_interval", None)
         if self._load_balancing_interval is None:
             self._load_balancing_interval = 10
         self._partition_ownership_expiration_interval = kwargs.pop(
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/__init__.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_connection_manager_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_connection_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_consumer_async.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_consumer_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/partition_context.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/partition_context.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/in_memory_checkpoint_store.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/event_processor.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/event_processor.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/utils.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/utils.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/checkpoint_store.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/checkpoint_store.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/aio/_eventprocessor/_ownership_manager.py` & `azure-eventhub-5.9.0b3/azure/eventhub/aio/_eventprocessor/_ownership_manager.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/_eventprocessor_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/common.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/common.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/ownership_manager.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/ownership_manager.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/partition_context.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/partition_context.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/in_memory_checkpoint_store.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/event_processor.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/event_processor.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/_eventprocessor/checkpoint_store.py` & `azure-eventhub-5.9.0b3/azure/eventhub/_eventprocessor/checkpoint_store.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/amqp/_constants.py` & `azure-eventhub-5.9.0b3/azure/eventhub/amqp/_constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 from enum import Enum
 
 from uamqp import MessageBodyType
+from azure.core import CaseInsensitiveEnumMeta
 
 
-class AmqpMessageBodyType(str, Enum):
+class AmqpMessageBodyType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     DATA = "data"
     SEQUENCE = "sequence"
     VALUE = "value"
 
 
 AMQP_MESSAGE_BODY_TYPE_MAP = {
     MessageBodyType.Data.value: AmqpMessageBodyType.DATA,
```

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/amqp/__init__.py` & `azure-eventhub-5.9.0b3/azure/eventhub/amqp/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventhub-5.9.0b2/azure/eventhub/amqp/_amqp_message.py` & `azure-eventhub-5.9.0b3/azure/eventhub/amqp/_amqp_message.py`

 * *Files identical despite different names*

