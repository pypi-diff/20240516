# Comparing `tmp/buz-2.6.6rc1.tar.gz` & `tmp/buz-2.6.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buz-2.6.6rc1.tar", max compression
+gzip compressed data, was "buz-2.6.7rc1.tar", max compression
```

## Comparing `buz-2.6.6rc1.tar` & `buz-2.6.7rc1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     1062 2024-05-03 10:39:43.856093 buz-2.6.6rc1/LICENSE
--rw-r--r--   0        0        0      104 2024-05-03 10:39:43.856093 buz-2.6.6rc1/README.md
--rw-r--r--   0        0        0     1432 2024-05-03 10:39:43.856093 buz-2.6.6rc1/pyproject.toml
--rw-r--r--   0        0        0      109 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/__init__.py
--rw-r--r--   0        0        0      223 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/__init__.py
--rw-r--r--   0        0        0      271 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/__init__.py
--rw-r--r--   0        0        0      709 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/base_command_handler.py
--rw-r--r--   0        0        0      181 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/command_bus.py
--rw-r--r--   0        0        0      330 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/command_handler.py
--rw-r--r--   0        0        0      409 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/middleware/__init__.py
--rw-r--r--   0        0        0      788 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      449 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1147 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      134 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py
--rw-r--r--   0        0        0      193 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/command.py
--rw-r--r--   0        0        0      554 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/more_than_one_command_handler_related_exception.py
--rw-r--r--   0        0        0      268 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/__init__.py
--rw-r--r--   0        0        0      708 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/base_command_handler.py
--rw-r--r--   0        0        0      175 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/command_bus.py
--rw-r--r--   0        0        0      316 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/command_handler.py
--rw-r--r--   0        0        0      406 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/middleware/__init__.py
--rw-r--r--   0        0        0      774 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      420 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1133 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      133 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py
--rw-r--r--   0        0        0      133 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/synced_async/__init__.py
--rw-r--r--   0        0        0      459 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/command/synchronous/synced_async/synced_async_command_bus.py
--rw-r--r--   0        0        0      256 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/__init__.py
--rw-r--r--   0        0        0      645 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/base_subscriber.py
--rw-r--r--   0        0        0      189 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/event.py
--rw-r--r--   0        0        0      293 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/event_bus.py
--rw-r--r--   0        0        0      656 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/__init__.py
--rw-r--r--   0        0        0      263 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/consume_strategy/__init__.py
--rw-r--r--   0        0        0      179 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
--rw-r--r--   0        0        0      756 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
--rw-r--r--   0        0        0      215 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/event_not_published_exception.py
--rw-r--r--   0        0        0      302 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/event_restore_exception.py
--rw-r--r--   0        0        0      258 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/execution_strategy/__init__.py
--rw-r--r--   0        0        0      192 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
--rw-r--r--   0        0        0      429 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
--rw-r--r--   0        0        0     6031 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/kombu_consumer.py
--rw-r--r--   0        0        0     3251 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/kombu_event_bus.py
--rw-r--r--   0        0        0      285 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/publish_strategy/__init__.py
--rw-r--r--   0        0        0      382 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
--rw-r--r--   0        0        0      309 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
--rw-r--r--   0        0        0      894 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/__init__.py
--rw-r--r--   0        0        0      361 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/consume_retrier.py
--rw-r--r--   0        0        0      229 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/consumed_event_retry.py
--rw-r--r--   0        0        0      449 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
--rw-r--r--   0        0        0     1332 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
--rw-r--r--   0        0        0      230 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
--rw-r--r--   0        0        0      993 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/publish_retry_policy.py
--rw-r--r--   0        0        0      241 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/reject_callback.py
--rw-r--r--   0        0        0     1236 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
--rw-r--r--   0        0        0       75 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/serializer_enum.py
--rw-r--r--   0        0        0      695 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/subscribers_not_found_exception.py
--rw-r--r--   0        0        0      265 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/term_signal_interruption_exception.py
--rw-r--r--   0        0        0      742 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/kombu/worker.py
--rw-r--r--   0        0        0      773 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/__init__.py
--rw-r--r--   0        0        0      651 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/base_consume_middleware.py
--rw-r--r--   0        0        0      531 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/base_publish_middleware.py
--rw-r--r--   0        0        0      363 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/consume_middleware.py
--rw-r--r--   0        0        0     1021 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
--rw-r--r--   0        0        0        0 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0      296 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/exceptions/event_already_in_progress_exception.py
--rw-r--r--   0        0        0      315 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/publish_middleware.py
--rw-r--r--   0        0        0      949 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
--rw-r--r--   0        0        0      303 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/subscriber.py
--rw-r--r--   0        0        0       91 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/sync/__init__.py
--rw-r--r--   0        0        0     1413 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/sync/sync_event_bus.py
--rw-r--r--   0        0        0     1381 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/__init__.py
--rw-r--r--   0        0        0      534 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
--rw-r--r--   0        0        0      779 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
--rw-r--r--   0        0        0      594 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/__init__.py
--rw-r--r--   0        0        0      347 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/deliverable_records_outbox_criteria_factory.py
--rw-r--r--   0        0        0      622 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria.py
--rw-r--r--   0        0        0      220 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria_factory.py
--rw-r--r--   0        0        0       89 2024-05-03 10:39:43.856093 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_sorting_criteria.py
--rw-r--r--   0        0        0     1157 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record.py
--rw-r--r--   0        0        0      344 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_finder/__init__.py
--rw-r--r--   0        0        0      239 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_finder/outbox_record_stream_finder.py
--rw-r--r--   0        0        0     1078 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_finder/polling_outbox_record_stream_finder.py
--rw-r--r--   0        0        0      708 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
--rw-r--r--   0        0        0        0 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/__init__.py
--rw-r--r--   0        0        0      610 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/abstract_outbox_record_validator.py
--rw-r--r--   0        0        0      749 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_size_not_allowed_exception.py
--rw-r--r--   0        0        0      134 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_validation_exception.py
--rw-r--r--   0        0        0      328 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_validator.py
--rw-r--r--   0        0        0     2443 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/size_outbox_record_validator.py
--rw-r--r--   0        0        0      509 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_repository.py
--rw-r--r--   0        0        0     1436 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
--rw-r--r--   0        0        0     2186 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
--rw-r--r--   0        0        0      272 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/handler.py
--rw-r--r--   0        0        0      293 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/__init__.py
--rw-r--r--   0        0        0      206 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/handler_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/locator.py
--rw-r--r--   0        0        0      206 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/message_fqn_not_found_exception.py
--rw-r--r--   0        0        0      365 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/pypendency/__init__.py
--rw-r--r--   0        0        0     4393 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/pypendency/container_locator.py
--rw-r--r--   0        0        0      426 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/pypendency/container_locator_resolution_configuration.py
--rw-r--r--   0        0        0      240 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/pypendency/handler_not_found_exception.py
--rw-r--r--   0        0        0      235 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
--rw-r--r--   0        0        0      370 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/sync/__init__.py
--rw-r--r--   0        0        0      245 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/sync/handler_already_registered_exception.py
--rw-r--r--   0        0        0      234 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/sync/handler_not_registered_exception.py
--rw-r--r--   0        0        0     2082 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/locator/sync/instance_locator.py
--rw-r--r--   0        0        0     2391 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/message.py
--rw-r--r--   0        0        0      176 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/middleware/__init__.py
--rw-r--r--   0        0        0       54 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/middleware/middleware.py
--rw-r--r--   0        0        0     1002 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/middleware/middleware_chain_builder.py
--rw-r--r--   0        0        0        0 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/py.typed
--rw-r--r--   0        0        0      274 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/__init__.py
--rw-r--r--   0        0        0      247 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/__init__.py
--rw-r--r--   0        0        0      675 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/base_query_handler.py
--rw-r--r--   0        0        0      404 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/middleware/__init__.py
--rw-r--r--   0        0        0      874 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      462 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1148 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      195 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/query_bus.py
--rw-r--r--   0        0        0      334 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/query_handler.py
--rw-r--r--   0        0        0      126 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1223 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py
--rw-r--r--   0        0        0      516 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/more_than_one_query_handler_related_exception.py
--rw-r--r--   0        0        0      189 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/query.py
--rw-r--r--   0        0        0      153 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/query_response.py
--rw-r--r--   0        0        0      244 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/__init__.py
--rw-r--r--   0        0        0      674 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/base_query_handler.py
--rw-r--r--   0        0        0      400 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/middleware/__init__.py
--rw-r--r--   0        0        0      846 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      433 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1095 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      189 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/query_bus.py
--rw-r--r--   0        0        0      328 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/query_handler.py
--rw-r--r--   0        0        0      125 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/self_process/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py
--rw-r--r--   0        0        0      125 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/synced_async/__init__.py
--rw-r--r--   0        0        0      470 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/query/synchronous/synced_async/synced_async_query_bus.py
--rw-r--r--   0        0        0       77 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/wrapper/__init__.py
--rw-r--r--   0        0        0      698 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/wrapper/async_to_sync.py
--rw-r--r--   0        0        0      266 2024-05-03 10:39:43.860092 buz-2.6.6rc1/src/buz/wrapper/event_loop.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 buz-2.6.6rc1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-16 09:00:11.994729 buz-2.6.7rc1/LICENSE
+-rw-r--r--   0        0        0      104 2024-05-16 09:00:11.994729 buz-2.6.7rc1/README.md
+-rw-r--r--   0        0        0     1432 2024-05-16 09:00:11.994729 buz-2.6.7rc1/pyproject.toml
+-rw-r--r--   0        0        0      109 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/__init__.py
+-rw-r--r--   0        0        0      271 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/__init__.py
+-rw-r--r--   0        0        0      709 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/base_command_handler.py
+-rw-r--r--   0        0        0      181 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/command_bus.py
+-rw-r--r--   0        0        0      330 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/command_handler.py
+-rw-r--r--   0        0        0      409 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      449 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1147 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      134 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      193 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/command.py
+-rw-r--r--   0        0        0      554 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/more_than_one_command_handler_related_exception.py
+-rw-r--r--   0        0        0      268 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/__init__.py
+-rw-r--r--   0        0        0      708 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/base_command_handler.py
+-rw-r--r--   0        0        0      175 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/command_bus.py
+-rw-r--r--   0        0        0      316 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/command_handler.py
+-rw-r--r--   0        0        0      406 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      420 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1133 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      133 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      133 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      459 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/command/synchronous/synced_async/synced_async_command_bus.py
+-rw-r--r--   0        0        0      256 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/base_subscriber.py
+-rw-r--r--   0        0        0      189 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/event.py
+-rw-r--r--   0        0        0      293 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/event_bus.py
+-rw-r--r--   0        0        0      656 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/consume_strategy/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
+-rw-r--r--   0        0        0      756 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
+-rw-r--r--   0        0        0      215 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/event_not_published_exception.py
+-rw-r--r--   0        0        0      302 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/event_restore_exception.py
+-rw-r--r--   0        0        0      258 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/execution_strategy/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
+-rw-r--r--   0        0        0      429 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
+-rw-r--r--   0        0        0     6031 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/kombu_consumer.py
+-rw-r--r--   0        0        0     3251 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/kombu_event_bus.py
+-rw-r--r--   0        0        0      285 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/publish_strategy/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
+-rw-r--r--   0        0        0      309 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
+-rw-r--r--   0        0        0      894 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/consume_retrier.py
+-rw-r--r--   0        0        0      229 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/consumed_event_retry.py
+-rw-r--r--   0        0        0      449 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
+-rw-r--r--   0        0        0     1332 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
+-rw-r--r--   0        0        0      230 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
+-rw-r--r--   0        0        0      993 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/publish_retry_policy.py
+-rw-r--r--   0        0        0      241 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/reject_callback.py
+-rw-r--r--   0        0        0     1236 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
+-rw-r--r--   0        0        0       75 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/serializer_enum.py
+-rw-r--r--   0        0        0      695 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/subscribers_not_found_exception.py
+-rw-r--r--   0        0        0      265 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/term_signal_interruption_exception.py
+-rw-r--r--   0        0        0      742 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/kombu/worker.py
+-rw-r--r--   0        0        0      773 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/base_consume_middleware.py
+-rw-r--r--   0        0        0      531 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/base_publish_middleware.py
+-rw-r--r--   0        0        0      363 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/consume_middleware.py
+-rw-r--r--   0        0        0     1021 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/exceptions/event_already_in_progress_exception.py
+-rw-r--r--   0        0        0      315 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/publish_middleware.py
+-rw-r--r--   0        0        0      949 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      303 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/subscriber.py
+-rw-r--r--   0        0        0       91 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/sync/__init__.py
+-rw-r--r--   0        0        0     1413 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/sync/sync_event_bus.py
+-rw-r--r--   0        0        0     1381 2024-05-16 09:00:11.994729 buz-2.6.7rc1/src/buz/event/transactional_outbox/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
+-rw-r--r--   0        0        0      779 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
+-rw-r--r--   0        0        0      594 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/__init__.py
+-rw-r--r--   0        0        0      347 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/deliverable_records_outbox_criteria_factory.py
+-rw-r--r--   0        0        0      649 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria.py
+-rw-r--r--   0        0        0      220 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria_factory.py
+-rw-r--r--   0        0        0       89 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_sorting_criteria.py
+-rw-r--r--   0        0        0     1157 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record.py
+-rw-r--r--   0        0        0      344 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_finder/__init__.py
+-rw-r--r--   0        0        0      239 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_finder/outbox_record_stream_finder.py
+-rw-r--r--   0        0        0     1078 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_finder/polling_outbox_record_stream_finder.py
+-rw-r--r--   0        0        0      708 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/__init__.py
+-rw-r--r--   0        0        0      610 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/abstract_outbox_record_validator.py
+-rw-r--r--   0        0        0      749 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_size_not_allowed_exception.py
+-rw-r--r--   0        0        0      134 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_validation_exception.py
+-rw-r--r--   0        0        0      328 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_validator.py
+-rw-r--r--   0        0        0     2443 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/size_outbox_record_validator.py
+-rw-r--r--   0        0        0      509 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_repository.py
+-rw-r--r--   0        0        0     1436 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
+-rw-r--r--   0        0        0     2186 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
+-rw-r--r--   0        0        0      272 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/handler.py
+-rw-r--r--   0        0        0      293 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/handler_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/locator.py
+-rw-r--r--   0        0        0      206 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/message_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      365 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/pypendency/__init__.py
+-rw-r--r--   0        0        0     4393 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/pypendency/container_locator.py
+-rw-r--r--   0        0        0      426 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/pypendency/container_locator_resolution_configuration.py
+-rw-r--r--   0        0        0      240 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/pypendency/handler_not_found_exception.py
+-rw-r--r--   0        0        0      235 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
+-rw-r--r--   0        0        0      370 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/sync/__init__.py
+-rw-r--r--   0        0        0      245 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/sync/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      234 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/sync/handler_not_registered_exception.py
+-rw-r--r--   0        0        0     2082 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/locator/sync/instance_locator.py
+-rw-r--r--   0        0        0     2391 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/message.py
+-rw-r--r--   0        0        0      176 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/middleware/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/middleware/middleware.py
+-rw-r--r--   0        0        0     1002 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/middleware/middleware_chain_builder.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/py.typed
+-rw-r--r--   0        0        0      274 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/__init__.py
+-rw-r--r--   0        0        0      675 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/base_query_handler.py
+-rw-r--r--   0        0        0      404 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      462 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1148 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      195 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/query_bus.py
+-rw-r--r--   0        0        0      334 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/query_handler.py
+-rw-r--r--   0        0        0      126 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1223 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      516 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/more_than_one_query_handler_related_exception.py
+-rw-r--r--   0        0        0      189 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/query.py
+-rw-r--r--   0        0        0      153 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/query_response.py
+-rw-r--r--   0        0        0      244 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/__init__.py
+-rw-r--r--   0        0        0      674 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/base_query_handler.py
+-rw-r--r--   0        0        0      400 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      846 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      433 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1095 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      189 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/query_bus.py
+-rw-r--r--   0        0        0      328 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/query_handler.py
+-rw-r--r--   0        0        0      125 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      125 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/query/synchronous/synced_async/synced_async_query_bus.py
+-rw-r--r--   0        0        0       77 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/wrapper/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/wrapper/async_to_sync.py
+-rw-r--r--   0        0        0      266 2024-05-16 09:00:11.998729 buz-2.6.7rc1/src/buz/wrapper/event_loop.py
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 buz-2.6.7rc1/PKG-INFO
```

### Comparing `buz-2.6.6rc1/LICENSE` & `buz-2.6.7rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/pyproject.toml` & `buz-2.6.7rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "buz"
-version = "2.6.6rc1"
+version = "2.6.7rc1"
 description = "Buz is a set of light, simple and extensible implementations of event, command and query buses."
 readme = "README.md"
 authors = ["Luis Pintado Lozano <luis.pintado.lozano@gmail.com>", "Gerardo Parra <gprauxiliar@gmail.com>"]
 maintainers = ["Fever - Platform Squad <platform@feverup.com>"]
 license = "MIT License"
 classifiers=[
     "Intended Audience :: Developers",
```

### Comparing `buz-2.6.6rc1/src/buz/command/asynchronous/base_command_handler.py` & `buz-2.6.7rc1/src/buz/command/asynchronous/base_command_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py` & `buz-2.6.7rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py` & `buz-2.6.7rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/more_than_one_command_handler_related_exception.py` & `buz-2.6.7rc1/src/buz/command/more_than_one_command_handler_related_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/synchronous/base_command_handler.py` & `buz-2.6.7rc1/src/buz/command/synchronous/base_command_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py` & `buz-2.6.7rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py` & `buz-2.6.7rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/base_subscriber.py` & `buz-2.6.7rc1/src/buz/event/base_subscriber.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/__init__.py` & `buz-2.6.7rc1/src/buz/event/kombu/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py` & `buz-2.6.7rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/kombu_consumer.py` & `buz-2.6.7rc1/src/buz/event/kombu/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/kombu_event_bus.py` & `buz-2.6.7rc1/src/buz/event/kombu/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/retry/__init__.py` & `buz-2.6.7rc1/src/buz/event/kombu/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py` & `buz-2.6.7rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/retry/publish_retry_policy.py` & `buz-2.6.7rc1/src/buz/event/kombu/retry/publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py` & `buz-2.6.7rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/subscribers_not_found_exception.py` & `buz-2.6.7rc1/src/buz/event/kombu/subscribers_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/kombu/worker.py` & `buz-2.6.7rc1/src/buz/event/kombu/worker.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/middleware/__init__.py` & `buz-2.6.7rc1/src/buz/event/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/middleware/base_consume_middleware.py` & `buz-2.6.7rc1/src/buz/event/middleware/base_consume_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/middleware/base_publish_middleware.py` & `buz-2.6.7rc1/src/buz/event/middleware/base_publish_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/sync/sync_event_bus.py` & `buz-2.6.7rc1/src/buz/event/sync/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/__init__.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/__init__.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_criteria/outbox_criteria.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from datetime import datetime, timedelta
-from typing import ClassVar, Union
+from typing import ClassVar, Union, Tuple
 
 from buz.event.transactional_outbox.outbox_criteria import OutboxSortingCriteria
 
 
 @dataclass(frozen=True)
 class OutboxCriteria:
     UNSET_VALUE: ClassVar[object] = object()
 
     delivered_at: Union[datetime, None, object] = UNSET_VALUE
     delivered_at_previous_to: Union[datetime, object] = UNSET_VALUE
     delivery_paused: Union[bool, object] = UNSET_VALUE
     order_by: Union[OutboxSortingCriteria, None, object] = UNSET_VALUE
-    created_since_more_than_x_timedelta: Union[timedelta, object] = UNSET_VALUE
+    created_within_timerange: Union[Tuple[Union[timedelta, None], timedelta], object] = UNSET_VALUE
```

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_finder/polling_outbox_record_stream_finder.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_finder/polling_outbox_record_stream_finder.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/abstract_outbox_record_validator.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/abstract_outbox_record_validator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_size_not_allowed_exception.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/outbox_record_size_not_allowed_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/outbox_record_validation/size_outbox_record_validator.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/outbox_record_validation/size_outbox_record_validator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py` & `buz-2.6.7rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/locator/locator.py` & `buz-2.6.7rc1/src/buz/locator/locator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/locator/pypendency/container_locator.py` & `buz-2.6.7rc1/src/buz/locator/pypendency/container_locator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/locator/sync/instance_locator.py` & `buz-2.6.7rc1/src/buz/locator/sync/instance_locator.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/message.py` & `buz-2.6.7rc1/src/buz/message.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/middleware/middleware_chain_builder.py` & `buz-2.6.7rc1/src/buz/middleware/middleware_chain_builder.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/asynchronous/base_query_handler.py` & `buz-2.6.7rc1/src/buz/query/asynchronous/base_query_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py` & `buz-2.6.7rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py` & `buz-2.6.7rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/more_than_one_query_handler_related_exception.py` & `buz-2.6.7rc1/src/buz/query/more_than_one_query_handler_related_exception.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/synchronous/base_query_handler.py` & `buz-2.6.7rc1/src/buz/query/synchronous/base_query_handler.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py` & `buz-2.6.7rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py` & `buz-2.6.7rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py` & `buz-2.6.7rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/src/buz/wrapper/async_to_sync.py` & `buz-2.6.7rc1/src/buz/wrapper/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `buz-2.6.6rc1/PKG-INFO` & `buz-2.6.7rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buz
-Version: 2.6.6rc1
+Version: 2.6.7rc1
 Summary: Buz is a set of light, simple and extensible implementations of event, command and query buses.
 License: MIT
 Author: Luis Pintado Lozano
 Author-email: luis.pintado.lozano@gmail.com
 Maintainer: Fever - Platform Squad
 Maintainer-email: platform@feverup.com
 Requires-Python: >=3.8.0,<4.0.0
```

