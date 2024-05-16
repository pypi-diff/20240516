# Comparing `tmp/faststream-0.5.5.tar.gz` & `tmp/faststream-0.5.6.tar.gz`

## Comparing `faststream-0.5.5.tar` & `faststream-0.5.6.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.5/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.5/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.5/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.5/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.5/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/security.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/types.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/security.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18973 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/parser.py
--rw-r--r--   0        0        0    22297 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/security.py
--rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29045 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/message.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/security.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/message.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/security.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.5/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.5/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.5/README.md
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.5/pyproject.toml
--rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.6/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.6/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.6/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.6/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.6/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/security.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18973 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    22297 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/security.py
+-rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29045 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/message.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/security.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27057 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    21801 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/message.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/security.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.6/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.6/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.6/README.md
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.6/PKG-INFO
```

### Comparing `faststream-0.5.5/.pre-commit-config.yaml` & `faststream-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.secrets.baseline` & `faststream-0.5.6/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/CITATION.cff` & `faststream-0.5.6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/CODE_OF_CONDUCT.md` & `faststream-0.5.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/CONTRIBUTING.md` & `faststream-0.5.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/SECURITY.md` & `faststream-0.5.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/dependabot.yml` & `faststream-0.5.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.6/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/codeql.yml` & `faststream-0.5.6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/dependency-review.yaml` & `faststream-0.5.6/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/deploy-docs.yaml` & `faststream-0.5.6/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/publish_coverage.yml` & `faststream-0.5.6/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/publish_pypi.yml` & `faststream-0.5.6/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/test.yaml` & `faststream-0.5.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/.github/workflows/update_release_notes.yaml` & `faststream-0.5.6/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e02_1_basic_publisher.py` & `faststream-0.5.6/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e02_2_basic_publisher.py` & `faststream-0.5.6/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e02_3_basic_publisher.py` & `faststream-0.5.6/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e03_miltiple_pubsub.py` & `faststream-0.5.6/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e04_msg_filter.py` & `faststream-0.5.6/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e07_ack_immediately.py` & `faststream-0.5.6/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e09_testing_mocks.py` & `faststream-0.5.6/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e10_middlewares.py` & `faststream-0.5.6/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/e11_settings.py` & `faststream-0.5.6/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/fastapi_integration/testing.py` & `faststream-0.5.6/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/howto/structlogs.py` & `faststream-0.5.6/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/kafka/testing.py` & `faststream-0.5.6/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/nats/e03_publisher.py` & `faststream-0.5.6/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/nats/e04_js_basic.py` & `faststream-0.5.6/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/nats/e05_basic_and_js.py` & `faststream-0.5.6/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/nats/e06_key_value.py` & `faststream-0.5.6/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/nats/e07_object_storage.py` & `faststream-0.5.6/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/rabbit/direct.py` & `faststream-0.5.6/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/rabbit/fanout.py` & `faststream-0.5.6/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/rabbit/header.py` & `faststream-0.5.6/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/rabbit/topic.py` & `faststream-0.5.6/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/redis/channel_sub_pattern.py` & `faststream-0.5.6/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/redis/rpc.py` & `faststream-0.5.6/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/router/basic_publish.py` & `faststream-0.5.6/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/serialization/avro/avro.py` & `faststream-0.5.6/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/serialization/msgpack/pack.py` & `faststream-0.5.6/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.6/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/__init__.py` & `faststream-0.5.6/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/_compat.py` & `faststream-0.5.6/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/app.py` & `faststream-0.5.6/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/exceptions.py` & `faststream-0.5.6/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/security.py` & `faststream-0.5.6/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/types.py` & `faststream-0.5.6/faststream/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,30 +59,24 @@
 SendableTable: TypeAlias = Dict[str, "BaseSendableMessage"]
 
 
 class StandardDataclass(Protocol):
     """Protocol to check type is dataclass."""
 
     __dataclass_fields__: ClassVar[Dict[str, Any]]
-    __dataclass_params__: ClassVar[Any]
-    __post_init__: ClassVar[Callable[..., None]]
-
-    def __init__(self, *args: object, **kwargs: object) -> None:
-        """Interface method."""
-        ...
 
 
 BaseSendableMessage: TypeAlias = Union[
     JsonDecodable,
     Decimal,
     datetime,
-    None,
     StandardDataclass,
     SendableTable,
     SendableArray,
+    None,
 ]
 
 try:
     from faststream._compat import BaseModel
 
     SendableMessage: TypeAlias = Union[
         BaseModel,
```

### Comparing `faststream-0.5.5/faststream/asyncapi/abc.py` & `faststream-0.5.6/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/generate.py` & `faststream-0.5.6/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/message.py` & `faststream-0.5.6/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/proto.py` & `faststream-0.5.6/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/site.py` & `faststream-0.5.6/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/utils.py` & `faststream-0.5.6/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.6/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/channels.py` & `faststream-0.5.6/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/info.py` & `faststream-0.5.6/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/main.py` & `faststream-0.5.6/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/message.py` & `faststream-0.5.6/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/operations.py` & `faststream-0.5.6/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/security.py` & `faststream-0.5.6/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/servers.py` & `faststream-0.5.6/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/utils.py` & `faststream-0.5.6/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.6/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.6/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/message.py` & `faststream-0.5.6/faststream/broker/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from contextlib import suppress
 from dataclasses import dataclass, field
 from inspect import Parameter
 from typing import (
     TYPE_CHECKING,
     Any,
     Generic,
+    List,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
@@ -34,14 +35,15 @@
 class StreamMessage(Generic[MsgType]):
     """Generic class to represent a stream message."""
 
     raw_message: "MsgType"
 
     body: Union[bytes, Any]
     headers: "AnyDict" = field(default_factory=dict)
+    batch_headers: List["AnyDict"] = field(default_factory=list)
     path: "AnyDict" = field(default_factory=dict)
 
     content_type: Optional[str] = None
     reply_to: str = ""
     message_id: str = field(default_factory=gen_cor_id)  # pragma: no cover
     correlation_id: str = field(
         default_factory=gen_cor_id  # pragma: no cover
```

### Comparing `faststream-0.5.5/faststream/broker/router.py` & `faststream-0.5.6/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/schemas.py` & `faststream-0.5.6/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/types.py` & `faststream-0.5.6/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/utils.py` & `faststream-0.5.6/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/core/abc.py` & `faststream-0.5.6/faststream/broker/core/abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,27 @@
         self._publishers = {}
 
         self._dependencies = dependencies
         self._middlewares = middlewares
         self._parser = parser
         self._decoder = decoder
 
+    def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None:
+        """Append BrokerMiddleware to the end of middlewares list.
+
+        Current middleware will be used as a most inner of already existed ones.
+        """
+        self._middlewares = (*self._middlewares, middleware)
+
+        for sub in self._subscribers.values():
+            sub.add_middleware(middleware)
+
+        for pub in self._publishers.values():
+            pub.add_middleware(middleware)
+
     @abstractmethod
     def subscriber(
         self,
         subscriber: "SubscriberProto[MsgType]",
     ) -> "SubscriberProto[MsgType]":
         subscriber.add_prefix(self.prefix)
         key = hash(subscriber)
```

### Comparing `faststream-0.5.5/faststream/broker/core/logging.py` & `faststream-0.5.6/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/core/usecase.py` & `faststream-0.5.6/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/fastapi/context.py` & `faststream-0.5.6/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.6/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/fastapi/route.py` & `faststream-0.5.6/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/fastapi/router.py` & `faststream-0.5.6/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/middlewares/base.py` & `faststream-0.5.6/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/middlewares/logging.py` & `faststream-0.5.6/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/publisher/fake.py` & `faststream-0.5.6/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/publisher/proto.py` & `faststream-0.5.6/faststream/broker/publisher/proto.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 ):
     schema_: Any
 
     _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
     _middlewares: Iterable["PublisherMiddleware"]
     _producer: Optional["ProducerProto"]
 
+    @abstractmethod
+    def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None: ...
+
     @staticmethod
     @abstractmethod
     def create() -> "PublisherProto[MsgType]":
         """Abstract factory to create a real Publisher."""
         ...
 
     @override
```

### Comparing `faststream-0.5.5/faststream/broker/publisher/usecase.py` & `faststream-0.5.6/faststream/broker/publisher/usecase.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 from fast_depends.core import CallModel, build_call_model
 from typing_extensions import Annotated, Doc, override
 
 from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import get_response_schema
 from faststream.asyncapi.utils import to_camelcase
 from faststream.broker.publisher.proto import PublisherProto
-from faststream.broker.types import MsgType, P_HandlerParams, T_HandlerReturn
+from faststream.broker.types import (
+    BrokerMiddleware,
+    MsgType,
+    P_HandlerParams,
+    T_HandlerReturn,
+)
 from faststream.broker.wrapper.call import HandlerCallWrapper
 
 if TYPE_CHECKING:
     from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         BrokerMiddleware,
         PublisherMiddleware,
@@ -83,14 +88,17 @@
 
         # AsyncAPI
         self.title_ = title_
         self.description_ = description_
         self.include_in_schema = include_in_schema
         self.schema_ = schema_
 
+    def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None:
+        self._broker_middlewares = (*self._broker_middlewares, middleware)
+
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         producer: Optional["ProducerProto"],
     ) -> None:
         self._producer = producer
```

### Comparing `faststream-0.5.5/faststream/broker/subscriber/call_item.py` & `faststream-0.5.6/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/subscriber/proto.py` & `faststream-0.5.6/faststream/broker/subscriber/proto.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     calls: List["HandlerItem[MsgType]"]
     running: bool
 
     _broker_dependecies: Iterable["Depends"]
     _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
     _producer: Optional["ProducerProto"]
 
+    @abstractmethod
+    def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None: ...
+
     @staticmethod
     @abstractmethod
     def create() -> "SubscriberProto[MsgType]":
         """Abstract factory to create a real Subscriber."""
         ...
 
     @abstractmethod
```

### Comparing `faststream-0.5.5/faststream/broker/subscriber/usecase.py` & `faststream-0.5.6/faststream/broker/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         self.extra_watcher_options = {}
 
         # AsyncAPI
         self.title_ = title_
         self.description_ = description_
         self.include_in_schema = include_in_schema
 
+    def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None:
+        self._broker_middlewares = (*self._broker_middlewares, middleware)
+
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         logger: Optional["LoggerProto"],
         producer: Optional[ProducerProto],
         graceful_timeout: Optional[float],
```

### Comparing `faststream-0.5.5/faststream/broker/wrapper/call.py` & `faststream-0.5.6/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/broker/wrapper/proto.py` & `faststream-0.5.6/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/main.py` & `faststream-0.5.6/faststream/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,29 +90,35 @@
         ".",
         "--app-dir",
         help=(
             "Look for APP in the specified directory, by adding this to the PYTHONPATH."
             " Defaults to the current working directory."
         ),
     ),
+    is_factory: bool = typer.Option(
+        False,
+        "--factory",
+        is_flag=True,
+        help="Treat APP as an application factory",
+    ),
 ) -> None:
     """Run [MODULE:APP] FastStream application."""
     if watch_extensions and not reload:
         typer.echo(
             "Extra reload extensions has no effect without `--reload` flag."
             "\nProbably, you forgot it?"
         )
 
     app, extra = parse_cli_args(app, *ctx.args)
     casted_log_level = get_log_level(log_level)
 
     if app_dir:  # pragma: no branch
         sys.path.insert(0, app_dir)
 
-    args = (app, extra, casted_log_level)
+    args = (app, extra, is_factory, casted_log_level)
 
     if reload and workers > 1:
         raise SetupError("You can't use reload option with multiprocessing")
 
     if reload:
         try:
             from faststream.cli.supervisors.watchfiles import WatchReloader
@@ -147,19 +153,22 @@
         _run(*args)
 
 
 def _run(
     # NOTE: we should pass `str` due FastStream is not picklable
     app: str,
     extra_options: Dict[str, "SettingField"],
+    is_factory: bool,
     log_level: int = logging.INFO,
     app_level: int = logging.INFO,
 ) -> None:
     """Runs the specified application."""
     _, app_obj = import_from_string(app)
+    if is_factory and callable(app_obj):
+        app_obj = app_obj()
 
     if not isinstance(app_obj, FastStream):
         raise typer.BadParameter(
             f'Imported object "{app_obj}" must be "FastStream" type.',
         )
 
     set_log_level(log_level, app_obj)
@@ -196,14 +205,20 @@
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
 )
 def publish(
     ctx: typer.Context,
     app: str = typer.Argument(..., help="FastStream app instance, e.g., main:app"),
     message: str = typer.Argument(..., help="Message to be published"),
     rpc: bool = typer.Option(False, help="Enable RPC mode and system output"),
+    is_factory: bool = typer.Option(
+        False,
+        "--factory",
+        is_flag=True,
+        help="Treat APP as an application factory",
+    ),
 ) -> None:
     """Publish a message using the specified broker in a FastStream application.
 
     This command publishes a message to a broker configured in a FastStream app instance.
     It supports various brokers and can handle extra arguments specific to each broker type.
     These are parsed and passed to the broker's publish method.
     """
@@ -214,14 +229,17 @@
     try:
         if not app:
             raise ValueError("App parameter is required.")
         if not message:
             raise ValueError("Message parameter is required.")
 
         _, app_obj = import_from_string(app)
+        if callable(app_obj) and is_factory:
+            app_obj = app_obj()
+
         if not app_obj.broker:
             raise ValueError("Broker instance not found in the app.")
 
         result = anyio.run(publish_message, app_obj.broker, extra)
 
         if rpc:
             typer.echo(result)
```

### Comparing `faststream-0.5.5/faststream/cli/docs/app.py` & `faststream-0.5.6/faststream/cli/docs/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,17 @@
         ".",
         "--app-dir",
         help=(
             "Look for APP in the specified directory, by adding this to the PYTHONPATH."
             " Defaults to the current working directory."
         ),
     ),
+    is_factory: bool = typer.Option(
+        False, "--factory", help="Treat APP as an application factory"
+    ),
 ) -> None:
     """Serve project AsyncAPI schema."""
     if ":" in app:
         if app_dir:  # pragma: no branch
             sys.path.insert(0, app_dir)
 
         module, _ = import_from_string(app)
@@ -62,26 +65,26 @@
 
     if reload:
         try:
             from faststream.cli.supervisors.watchfiles import WatchReloader
 
         except ImportError:
             warnings.warn(INSTALL_WATCHFILES, category=ImportWarning, stacklevel=1)
-            _parse_and_serve(app, host, port)
+            _parse_and_serve(app, host, port, is_factory)
 
         else:
             WatchReloader(
                 target=_parse_and_serve,
-                args=(app, host, port),
+                args=(app, host, port, is_factory),
                 reload_dirs=(str(module_parent),),
                 extra_extensions=extra_extensions,
             ).run()
 
     else:
-        _parse_and_serve(app, host, port)
+        _parse_and_serve(app, host, port, is_factory)
 
 
 @docs_app.command(name="gen")
 def gen(
     app: str = typer.Argument(
         ...,
         help="[python_module:FastStream] - path to your application",
@@ -100,20 +103,27 @@
         ".",
         "--app-dir",
         help=(
             "Look for APP in the specified directory, by adding this to the PYTHONPATH."
             " Defaults to the current working directory."
         ),
     ),
+    is_factory: bool = typer.Option(
+        False,
+        "--factory",
+        help="Treat APP as an application factory",
+    ),
 ) -> None:
     """Generate project AsyncAPI schema."""
     if app_dir:  # pragma: no branch
         sys.path.insert(0, app_dir)
 
     _, app_obj = import_from_string(app)
+    if callable(app_obj) and is_factory:
+        app_obj = app_obj()
     raw_schema = get_app_schema(app_obj)
 
     if yaml:
         try:
             schema = raw_schema.to_yaml()
         except ImportError as e:  # pragma: no cover
             typer.echo(INSTALL_YAML, err=True)
@@ -134,17 +144,20 @@
     typer.echo(f"Your project AsyncAPI scheme was placed to `{name}`")
 
 
 def _parse_and_serve(
     app: str,
     host: str = "localhost",
     port: int = 8000,
+    is_factory: bool = False,
 ) -> None:
     if ":" in app:
         _, app_obj = import_from_string(app)
+        if callable(app_obj) and is_factory:
+            app_obj = app_obj()
         raw_schema = get_app_schema(app_obj)
 
     else:
         schema_filepath = Path.cwd() / app
 
         if schema_filepath.suffix == ".json":
             data = schema_filepath.read_bytes()
```

### Comparing `faststream-0.5.5/faststream/cli/supervisors/basereload.py` & `faststream-0.5.6/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.6/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/supervisors/utils.py` & `faststream-0.5.6/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.6/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/utils/imports.py` & `faststream-0.5.6/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/utils/logs.py` & `faststream-0.5.6/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/cli/utils/parser.py` & `faststream-0.5.6/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/annotations.py` & `faststream-0.5.6/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/client.py` & `faststream-0.5.6/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/message.py` & `faststream-0.5.6/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/parser.py` & `faststream-0.5.6/faststream/confluent/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from faststream.broker.message import decode_message, gen_cor_id
 from faststream.confluent.message import FAKE_CONSUMER, KafkaMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
     from confluent_kafka import Message
@@ -16,26 +16,22 @@
     """A class to parse Kafka messages."""
 
     @staticmethod
     async def parse_message(
         message: "Message",
     ) -> "StreamMessage[Message]":
         """Parses a Kafka message."""
-        headers = {}
-        if message.headers() is not None:
-            for i, j in message.headers():  # type: ignore[union-attr]
-                if isinstance(j, str):
-                    headers[i] = j
-                else:
-                    headers[i] = j.decode()
+        headers = _parse_msg_headers(message.headers())
+
         body = message.value()
         offset = message.offset()
         _, timestamp = message.timestamp()
 
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
+
         return KafkaMessage(
             body=body,
             headers=headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=f"{offset}-{timestamp}",
             correlation_id=headers.get("correlation_id", gen_cor_id()),
@@ -45,36 +41,37 @@
         )
 
     @staticmethod
     async def parse_message_batch(
         message: Tuple["Message", ...],
     ) -> "StreamMessage[Tuple[Message, ...]]":
         """Parses a batch of messages from a Kafka consumer."""
+        body: List[Any] = []
+        batch_headers: List[Dict[str, str]] = []
+
         first = message[0]
         last = message[-1]
 
-        headers = {}
-        if first.headers() is not None:
-            for i, j in first.headers():  # type: ignore[union-attr]
-                if isinstance(j, str):
-                    headers[i] = j
-                else:
-                    headers[i] = j.decode()
-        body = [m.value() for m in message]
-        first_offset = first.offset()
-        last_offset = last.offset()
+        for m in message:
+            body.append(m.value)
+            batch_headers.append(_parse_msg_headers(m.headers()))
+
+        headers = next(iter(batch_headers), {})
+
         _, first_timestamp = first.timestamp()
 
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
+
         return KafkaMessage(
             body=body,
             headers=headers,
+            batch_headers=batch_headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
-            message_id=f"{first_offset}-{last_offset}-{first_timestamp}",
+            message_id=f"{first.offset()}-{last.offset()}-{first_timestamp}",
             correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
@@ -87,7 +84,13 @@
     @classmethod
     async def decode_message_batch(
         cls,
         msg: "StreamMessage[Tuple[Message, ...]]",
     ) -> "DecodedMessage":
         """Decode a batch of messages."""
         return [decode_message(await cls.parse_message(m)) for m in msg.raw_message]
+
+
+def _parse_msg_headers(
+    headers: Sequence[Tuple[str, Union[bytes, str]]],
+) -> Dict[str, str]:
+    return {i: j if isinstance(j, str) else j.decode() for i, j in headers}
```

### Comparing `faststream-0.5.5/faststream/confluent/router.py` & `faststream-0.5.6/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/security.py` & `faststream-0.5.6/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/testing.py` & `faststream-0.5.6/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/broker/broker.py` & `faststream-0.5.6/faststream/confluent/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/broker/logging.py` & `faststream-0.5.6/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/broker/registrator.py` & `faststream-0.5.6/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.6/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.6/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.6/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/publisher/producer.py` & `faststream-0.5.6/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/publisher/usecase.py` & `faststream-0.5.6/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/schemas/params.py` & `faststream-0.5.6/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.6/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.6/faststream/confluent/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/annotations.py` & `faststream-0.5.6/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/message.py` & `faststream-0.5.6/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/parser.py` & `faststream-0.5.6/faststream/kafka/parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from faststream.broker.message import decode_message, gen_cor_id
 from faststream.kafka.message import FAKE_CONSUMER, KafkaMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
     from aiokafka import ConsumerRecord
@@ -35,21 +35,32 @@
         )
 
     @staticmethod
     async def parse_message_batch(
         message: Tuple["ConsumerRecord", ...],
     ) -> "StreamMessage[Tuple[ConsumerRecord, ...]]":
         """Parses a batch of messages from a Kafka consumer."""
+        body: List[Any] = []
+        batch_headers: List[Dict[str, str]] = []
+
         first = message[0]
         last = message[-1]
-        headers = {i: j.decode() for i, j in first.headers}
+
+        for m in message:
+            body.append(m.value)
+            batch_headers.append({i: j.decode() for i, j in m.headers})
+
+        headers = next(iter(batch_headers), {})
+
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
+
         return KafkaMessage(
-            body=[m.value for m in message],
+            body=body,
             headers=headers,
+            batch_headers=batch_headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=f"{first.offset}-{last.offset}-{first.timestamp}",
             correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
```

### Comparing `faststream-0.5.5/faststream/kafka/router.py` & `faststream-0.5.6/faststream/kafka/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/security.py` & `faststream-0.5.6/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/testing.py` & `faststream-0.5.6/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/broker/broker.py` & `faststream-0.5.6/faststream/kafka/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/broker/logging.py` & `faststream-0.5.6/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/broker/registrator.py` & `faststream-0.5.6/faststream/kafka/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.6/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.6/faststream/kafka/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.6/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/publisher/producer.py` & `faststream-0.5.6/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/publisher/usecase.py` & `faststream-0.5.6/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/schemas/params.py` & `faststream-0.5.6/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.6/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.6/faststream/kafka/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/log/formatter.py` & `faststream-0.5.6/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/log/logging.py` & `faststream-0.5.6/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/__init__.py` & `faststream-0.5.6/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/annotations.py` & `faststream-0.5.6/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/helpers.py` & `faststream-0.5.6/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/message.py` & `faststream-0.5.6/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/parser.py` & `faststream-0.5.6/faststream/nats/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
 from faststream.nats.message import NatsBatchMessage, NatsMessage
 from faststream.nats.schemas.js_stream import compile_nats_wildcard
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
@@ -98,23 +98,35 @@
 class BatchParser(JsParser):
     """A class to parse NATS batch messages."""
 
     async def parse_batch(
         self,
         message: List["Msg"],
     ) -> "StreamMessage[List[Msg]]":
-        if first_msg := next(iter(message), None):
-            path = self.get_path(first_msg.subject)
+        body: List[bytes] = []
+        batch_headers: List[Dict[str, str]] = []
+
+        if message:
+            path = self.get_path(message[0].subject)
+
+            for m in message:
+                batch_headers.append(m.headers or {})
+                body.append(m.data)
+
         else:
             path = None
 
+        headers = next(iter(batch_headers), {})
+
         return NatsBatchMessage(
             raw_message=message,
-            body=[m.data for m in message],
+            body=body,
             path=path or {},
+            headers=headers,
+            batch_headers=batch_headers,
         )
 
     async def decode_batch(
         self,
         msg: "StreamMessage[List[Msg]]",
     ) -> List["DecodedMessage"]:
         data: List["DecodedMessage"] = []
```

### Comparing `faststream-0.5.5/faststream/nats/router.py` & `faststream-0.5.6/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/security.py` & `faststream-0.5.6/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/testing.py` & `faststream-0.5.6/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/broker/broker.py` & `faststream-0.5.6/faststream/nats/broker/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,20 +619,20 @@
                 try:  # pragma: no branch
                     await self.stream.add_stream(
                         config=stream.config,
                         subjects=stream.subjects,
                     )
 
                 except BadRequestError as e:
-                    old_config = (await self.stream.stream_info(stream.name)).config
-
                     if (
                         e.description
                         == "stream name already in use with a different configuration"
                     ):
+                        old_config = (await self.stream.stream_info(stream.name)).config
+
                         self._log(str(e), logging.WARNING, log_context)
                         await self.stream.update_stream(
                             config=stream.config,
                             subjects=tuple(
                                 set(old_config.subjects or ()).union(stream.subjects)
                             ),
                         )
```

### Comparing `faststream-0.5.5/faststream/nats/broker/logging.py` & `faststream-0.5.6/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/broker/registrator.py` & `faststream-0.5.6/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/fastapi/__init__.py` & `faststream-0.5.6/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.6/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.6/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/publisher/producer.py` & `faststream-0.5.6/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/publisher/usecase.py` & `faststream-0.5.6/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/schemas/js_stream.py` & `faststream-0.5.6/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.6/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.6/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/nats/subscriber/usecase.py` & `faststream-0.5.6/faststream/nats/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/__init__.py` & `faststream-0.5.6/faststream/rabbit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,9 +17,10 @@
     "RabbitRouter",
     "RabbitRoute",
     "RabbitPublisher",
     "ExchangeType",
     "ReplyConfig",
     "RabbitExchange",
     "RabbitQueue",
+    # Annotations
     "RabbitMessage",
 )
```

### Comparing `faststream-0.5.5/faststream/rabbit/annotations.py` & `faststream-0.5.6/faststream/redis/annotations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from redis.asyncio.client import Redis as RedisClient
 from typing_extensions import Annotated
 
 from faststream.annotations import ContextRepo, Logger, NoCast
-from faststream.rabbit.broker import RabbitBroker as RB
-from faststream.rabbit.message import RabbitMessage as RM
-from faststream.rabbit.publisher.producer import AioPikaFastProducer
+from faststream.redis.broker.broker import RedisBroker as RB
+from faststream.redis.message import UnifyRedisMessage
 from faststream.utils.context import Context
 
 __all__ = (
     "Logger",
     "ContextRepo",
     "NoCast",
-    "RabbitMessage",
-    "RabbitBroker",
-    "RabbitProducer",
+    "RedisMessage",
+    "RedisBroker",
+    "Redis",
 )
 
-RabbitMessage = Annotated[RM, Context("message")]
-RabbitBroker = Annotated[RB, Context("broker")]
-RabbitProducer = Annotated[AioPikaFastProducer, Context("broker._producer")]
+RedisMessage = Annotated[UnifyRedisMessage, Context("message")]
+RedisBroker = Annotated[RB, Context("broker")]
+Redis = Annotated[RedisClient, Context("broker._connection")]
```

### Comparing `faststream-0.5.5/faststream/rabbit/message.py` & `faststream-0.5.6/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/parser.py` & `faststream-0.5.6/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/router.py` & `faststream-0.5.6/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/security.py` & `faststream-0.5.6/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/testing.py` & `faststream-0.5.6/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/utils.py` & `faststream-0.5.6/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/broker/broker.py` & `faststream-0.5.6/faststream/rabbit/broker/broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,34 @@
             Optional["FieldTable"],
             Doc("Add custom client capability."),
         ] = None,
         timeout: Annotated[
             "TimeoutType",
             Doc("Connection establishement timeout."),
         ] = None,
+        # channel args
+        channel_number: Annotated[
+            Optional[int],
+            Doc("Specify the channel number explicit."),
+        ] = None,
+        publisher_confirms: Annotated[
+            bool,
+            Doc(
+                "if `True` the `publish` method will "
+                "return `bool` type after publish is complete."
+                "Otherwise it will returns `None`."
+            ),
+        ] = True,
+        on_return_raises: Annotated[
+            bool,
+            Doc(
+                "raise an :class:`aio_pika.exceptions.DeliveryError`"
+                "when mandatory message will be returned"
+            ),
+        ] = False,
         # broker args
         max_consumers: Annotated[
             Optional[int],
             Doc(
                 "RabbitMQ channel `qos` option. "
                 "It limits max messages processing in the same time count."
             ),
@@ -216,14 +236,18 @@
         if protocol is None:
             protocol = builded_asyncapi_url.scheme
 
         super().__init__(
             url=str(amqp_url),
             ssl_context=security_args.get("ssl_context"),
             timeout=timeout,
+            # channel args
+            channel_number=channel_number,
+            publisher_confirms=publisher_confirms,
+            on_return_raises=on_return_raises,
             # Basic args
             graceful_timeout=graceful_timeout,
             dependencies=dependencies,
             decoder=decoder,
             parser=parser,
             middlewares=middlewares,
             # AsyncAPI args
@@ -299,21 +323,50 @@
                 "Security options to connect broker and generate AsyncAPI server security information."
             ),
         ] = None,
         timeout: Annotated[
             "TimeoutType",
             Doc("Connection establishement timeout."),
         ] = None,
+        # channel args
+        channel_number: Annotated[
+            Union[int, None, object],
+            Doc("Specify the channel number explicit."),
+        ] = Parameter.empty,
+        publisher_confirms: Annotated[
+            Union[bool, object],
+            Doc(
+                "if `True` the `publish` method will "
+                "return `bool` type after publish is complete."
+                "Otherwise it will returns `None`."
+            ),
+        ] = Parameter.empty,
+        on_return_raises: Annotated[
+            Union[bool, object],
+            Doc(
+                "raise an :class:`aio_pika.exceptions.DeliveryError`"
+                "when mandatory message will be returned"
+            ),
+        ] = Parameter.empty,
     ) -> "RobustConnection":
         """Connect broker object to RabbitMQ.
 
         To startup subscribers too you should use `broker.start()` after/instead this method.
         """
         kwargs: AnyDict = {}
 
+        if channel_number is not Parameter.empty:
+            kwargs["channel_number"] = channel_number
+
+        if publisher_confirms is not Parameter.empty:
+            kwargs["publisher_confirms"] = publisher_confirms
+
+        if on_return_raises is not Parameter.empty:
+            kwargs["on_return_raises"] = on_return_raises
+
         if timeout:
             kwargs["timeout"] = timeout
 
         url = None if url is Parameter.empty else cast(Union[str, "URL"], url)
 
         if url or any(
             (host, port, virtualhost, ssl_options, client_properties, security)
@@ -342,29 +395,36 @@
     @override
     async def _connect(  # type: ignore[override]
         self,
         url: str,
         *,
         timeout: "TimeoutType",
         ssl_context: Optional["SSLContext"],
+        channel_number: Optional[int],
+        publisher_confirms: bool,
+        on_return_raises: bool,
     ) -> "RobustConnection":
         connection = cast(
             "RobustConnection",
             await connect_robust(
                 url,
                 timeout=timeout,
                 ssl_context=ssl_context,
             ),
         )
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             channel = self._channel = cast(
                 "RobustChannel",
-                await connection.channel(),
+                await connection.channel(
+                    channel_number=channel_number,
+                    publisher_confirms=publisher_confirms,
+                    on_return_raises=on_return_raises,
+                ),
             )
 
             declarer = self.declarer = RabbitDeclarer(channel)
             await declarer.declare_queue(RABBIT_REPLY)
 
             self._producer = AioPikaFastProducer(
                 channel=channel,
```

### Comparing `faststream-0.5.5/faststream/rabbit/broker/logging.py` & `faststream-0.5.6/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/broker/registrator.py` & `faststream-0.5.6/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.6/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/fastapi/router.py` & `faststream-0.5.6/faststream/rabbit/fastapi/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,34 @@
             Optional["FieldTable"],
             Doc("Add custom client capability."),
         ] = None,
         timeout: Annotated[
             "TimeoutType",
             Doc("Connection establishement timeout."),
         ] = None,
+        # channel args
+        channel_number: Annotated[
+            Optional[int],
+            Doc("Specify the channel number explicit."),
+        ] = None,
+        publisher_confirms: Annotated[
+            bool,
+            Doc(
+                "if `True` the `publish` method will "
+                "return `bool` type after publish is complete."
+                "Otherwise it will returns `None`."
+            ),
+        ] = True,
+        on_return_raises: Annotated[
+            bool,
+            Doc(
+                "raise an :class:`aio_pika.exceptions.DeliveryError`"
+                "when mandatory message will be returned"
+            ),
+        ] = False,
         # broker args
         max_consumers: Annotated[
             Optional[int],
             Doc(
                 "RabbitMQ channel `qos` option. "
                 "It limits max messages processing in the same time count."
             ),
@@ -404,14 +424,17 @@
             client_properties=client_properties,
             timeout=timeout,
             max_consumers=max_consumers,
             app_id=app_id,
             graceful_timeout=graceful_timeout,
             decoder=decoder,
             parser=parser,
+            channel_number=channel_number,
+            publisher_confirms=publisher_confirms,
+            on_return_raises=on_return_raises,
             middlewares=middlewares,
             security=security,
             asyncapi_url=asyncapi_url,
             protocol=protocol,
             protocol_version=protocol_version,
             description=description,
             logger=logger,
```

### Comparing `faststream-0.5.5/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.6/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/publisher/producer.py` & `faststream-0.5.6/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.6/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/schemas/constants.py` & `faststream-0.5.6/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.6/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/schemas/queue.py` & `faststream-0.5.6/faststream/rabbit/schemas/queue.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import Annotated, Doc
 
 from faststream.broker.schemas import NameRequired
 from faststream.utils.path import compile_path
 
@@ -111,7 +112,17 @@
         self.bind_arguments = bind_arguments
         self.routing_key = routing_key
         self.robust = robust
         self.passive = passive
         self.auto_delete = auto_delete
         self.arguments = arguments
         self.timeout = timeout
+
+    def add_prefix(self, prefix: str) -> "RabbitQueue":
+        new_q: RabbitQueue = deepcopy(self)
+
+        new_q.name = "".join((prefix, new_q.name))
+
+        if new_q.routing_key:
+            new_q.routing_key = "".join((prefix, new_q.routing_key))
+
+        return new_q
```

### Comparing `faststream-0.5.5/faststream/rabbit/schemas/reply.py` & `faststream-0.5.6/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.6/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.6/faststream/rabbit/subscriber/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Optional,
@@ -219,10 +218,8 @@
             message=message,
             queue=self.queue,
             exchange=self.exchange,
         )
 
     def add_prefix(self, prefix: str) -> None:
         """Include Subscriber in router."""
-        new_q = deepcopy(self.queue)
-        new_q.name = "".join((prefix, new_q.name))
-        self.queue = new_q
+        self.queue = self.queue.add_prefix(prefix)
```

### Comparing `faststream-0.5.5/faststream/redis/__init__.py` & `faststream-0.5.6/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/message.py` & `faststream-0.5.6/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/parser.py` & `faststream-0.5.6/faststream/redis/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     TYPE_CHECKING,
     Any,
+    List,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -131,30 +132,35 @@
     ) -> None:
         self.pattern = pattern
 
     async def parse_message(
         self,
         message: Mapping[str, Any],
     ) -> "StreamMessage[Mapping[str, Any]]":
-        data, headers = self._parse_data(message)
+        data, headers, batch_headers = self._parse_data(message)
+
         id_ = gen_cor_id()
+
         return self.msg_class(
             raw_message=message,
             body=data,
             path=self.get_path(message),
             headers=headers,
+            batch_headers=batch_headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=headers.get("message_id", id_),
             correlation_id=headers.get("correlation_id", id_),
         )
 
     @staticmethod
-    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
-        return RawMessage.parse(message["data"])
+    def _parse_data(
+        message: Mapping[str, Any],
+    ) -> Tuple[bytes, "AnyDict", List["AnyDict"]]:
+        return (*RawMessage.parse(message["data"]), [])
 
     def get_path(self, message: Mapping[str, Any]) -> "AnyDict":
         if (
             message.get("pattern")
             and (path_re := self.pattern)
             and (match := path_re.match(message["channel"]))
         ):
@@ -178,42 +184,74 @@
     msg_class = RedisListMessage
 
 
 class RedisBatchListParser(SimpleParser):
     msg_class = RedisBatchListMessage
 
     @staticmethod
-    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
+    def _parse_data(
+        message: Mapping[str, Any],
+    ) -> Tuple[bytes, "AnyDict", List["AnyDict"]]:
+        body: List[Any] = []
+        batch_headers: List["AnyDict"] = []
+
+        for x in message["data"]:
+            msg_data, msg_headers = _decode_batch_body_item(x)
+            body.append(msg_data)
+            batch_headers.append(msg_headers)
+
+        first_msg_headers = next(iter(batch_headers), {})
+
         return (
-            dump_json(_decode_batch_body_item(x) for x in message["data"]),
-            {"content-type": ContentTypes.json},
+            dump_json(body),
+            {
+                **first_msg_headers,
+                "content-type": ContentTypes.json.value,
+            },
+            batch_headers,
         )
 
 
 class RedisStreamParser(SimpleParser):
     msg_class = RedisStreamMessage
 
     @classmethod
-    def _parse_data(cls, message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
+    def _parse_data(
+        cls, message: Mapping[str, Any]
+    ) -> Tuple[bytes, "AnyDict", List["AnyDict"]]:
         data = message["data"]
-        return RawMessage.parse(data.get(bDATA_KEY) or dump_json(data))
+        return (*RawMessage.parse(data.get(bDATA_KEY) or dump_json(data)), [])
 
 
 class RedisBatchStreamParser(SimpleParser):
     msg_class = RedisBatchStreamMessage
 
     @staticmethod
-    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
+    def _parse_data(
+        message: Mapping[str, Any],
+    ) -> Tuple[bytes, "AnyDict", List["AnyDict"]]:
+        body: List[Any] = []
+        batch_headers: List["AnyDict"] = []
+
+        for x in message["data"]:
+            msg_data, msg_headers = _decode_batch_body_item(x.get(bDATA_KEY, x))
+            body.append(msg_data)
+            batch_headers.append(msg_headers)
+
+        first_msg_headers = next(iter(batch_headers), {})
+
         return (
-            dump_json(
-                _decode_batch_body_item(x.get(bDATA_KEY, x)) for x in message["data"]
-            ),
-            {"content-type": ContentTypes.json},
+            dump_json(body),
+            {
+                **first_msg_headers,
+                "content-type": ContentTypes.json.value,
+            },
+            batch_headers,
         )
 
 
-def _decode_batch_body_item(msg_content: bytes) -> Any:
-    msg_body, _ = RawMessage.parse(msg_content)
+def _decode_batch_body_item(msg_content: bytes) -> Tuple[Any, "AnyDict"]:
+    msg_body, headers = RawMessage.parse(msg_content)
     try:
-        return json_loads(msg_body)
+        return json_loads(msg_body), headers
     except Exception:
-        return msg_body
+        return msg_body, headers
```

### Comparing `faststream-0.5.5/faststream/redis/router.py` & `faststream-0.5.6/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/security.py` & `faststream-0.5.6/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/testing.py` & `faststream-0.5.6/faststream/redis/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/broker/broker.py` & `faststream-0.5.6/faststream/redis/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/broker/logging.py` & `faststream-0.5.6/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/broker/registrator.py` & `faststream-0.5.6/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/fastapi/__init__.py` & `faststream-0.5.6/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.6/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.6/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/publisher/producer.py` & `faststream-0.5.6/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/publisher/usecase.py` & `faststream-0.5.6/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/schemas/list_sub.py` & `faststream-0.5.6/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/schemas/proto.py` & `faststream-0.5.6/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.6/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.6/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.6/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/redis/subscriber/usecase.py` & `faststream-0.5.6/faststream/redis/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/testing/app.py` & `faststream-0.5.6/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/testing/broker.py` & `faststream-0.5.6/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/ast.py` & `faststream-0.5.6/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/classes.py` & `faststream-0.5.6/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/data.py` & `faststream-0.5.6/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/functions.py` & `faststream-0.5.6/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/no_cast.py` & `faststream-0.5.6/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/path.py` & `faststream-0.5.6/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/context/builders.py` & `faststream-0.5.6/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/context/repository.py` & `faststream-0.5.6/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/faststream/utils/context/types.py` & `faststream-0.5.6/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/scripts/build-docs-pre-commit.sh` & `faststream-0.5.6/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/scripts/lint-pre-commit.sh` & `faststream-0.5.6/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/scripts/set_variables.sh` & `faststream-0.5.6/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/scripts/static-pre-commit.sh` & `faststream-0.5.6/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/LICENSE` & `faststream-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/README.md` & `faststream-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.5/pyproject.toml` & `faststream-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 nats = ["nats-py>=2.3.1,<=3.0.0"]
 
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
     "mkdocs-material==9.5.21",
-    "mkdocs-static-i18n==1.2.2",
+    "mkdocs-static-i18n==1.2.3",
     "mdx-include==1.4.2",
-    "mkdocstrings[python]==0.25.0",
+    "mkdocstrings[python]==0.25.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.5",
     "mike==2.1.1",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
     "mkdocs-glightbox==0.3.7",                          # img zoom
     "pillow",                                           # required for mkdocs-glightbo
@@ -102,22 +102,22 @@
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
 ]
 
 lint = [
     "faststream[types]",
-    "ruff==0.4.3",
+    "ruff==0.4.4",
     "bandit==1.7.8",
     "semgrep==1.70.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
-    "coverage[toml]==7.4.4",
+    "coverage[toml]==7.5.1",
     "pytest==8.2.0",
     "pytest-asyncio==0.23.6",
     "dirty-equals==0.7.1.post0",
 ]
 
 testing = [
     "faststream[test-core]",
@@ -129,15 +129,15 @@
     "email-validator==2.1.1",
 ]
 
 dev = [
     "faststream[rabbit,kafka,confluent,nats,redis,lint,testing,devdocs]",
     "pre-commit==3.5.0; python_version < '3.9'",
     "pre-commit==3.7.0; python_version >= '3.9'",
-    "detect-secrets==1.4.0",
+    "detect-secrets==1.5.0",
 ]
 
 [project.urls]
 Homepage = "https://faststream.airt.ai/latest/"
 Documentation = "https://faststream.airt.ai/latest/getting-started/"
 Tracker = "https://github.com/airtai/FastStream/issues"
 Source = "https://github.com/airtai/FastStream"
```

### Comparing `faststream-0.5.5/PKG-INFO` & `faststream-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.5
+Version: 0.5.6
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -48,43 +48,43 @@
 Requires-Dist: aio-pika<10,>=9; extra == 'dev'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'dev'
 Requires-Dist: bandit==1.7.8; extra == 'dev'
 Requires-Dist: cairosvg; extra == 'dev'
 Requires-Dist: codespell==2.2.6; extra == 'dev'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'dev'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'dev'
-Requires-Dist: coverage[toml]==7.4.4; extra == 'dev'
-Requires-Dist: detect-secrets==1.4.0; extra == 'dev'
+Requires-Dist: coverage[toml]==7.5.1; extra == 'dev'
+Requires-Dist: detect-secrets==1.5.0; extra == 'dev'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'dev'
 Requires-Dist: email-validator==2.1.1; extra == 'dev'
 Requires-Dist: fastapi==0.111.0; extra == 'dev'
 Requires-Dist: griffe-typingdoc==0.2.5; extra == 'dev'
 Requires-Dist: httpx==0.27.0; extra == 'dev'
 Requires-Dist: mdx-include==1.4.2; extra == 'dev'
 Requires-Dist: mike==2.1.1; extra == 'dev'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'dev'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'dev'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'dev'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
 Requires-Dist: mkdocs-material==9.5.21; extra == 'dev'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
-Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'dev'
-Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'dev'
+Requires-Dist: mkdocs-static-i18n==1.2.3; extra == 'dev'
+Requires-Dist: mkdocstrings[python]==0.25.1; extra == 'dev'
 Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
 Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
 Requires-Dist: pytest==8.2.0; extra == 'dev'
 Requires-Dist: pyyaml==6.0.1; extra == 'dev'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'dev'
 Requires-Dist: requests; extra == 'dev'
-Requires-Dist: ruff==0.4.3; extra == 'dev'
+Requires-Dist: ruff==0.4.4; extra == 'dev'
 Requires-Dist: semgrep==1.70.0; extra == 'dev'
 Requires-Dist: types-docutils; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Requires-Dist: types-setuptools; extra == 'dev'
 Requires-Dist: types-ujson; extra == 'dev'
@@ -96,51 +96,51 @@
 Requires-Dist: mike==2.1.1; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
 Requires-Dist: mkdocs-material==9.5.21; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
-Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
-Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'devdocs'
+Requires-Dist: mkdocs-static-i18n==1.2.3; extra == 'devdocs'
+Requires-Dist: mkdocstrings[python]==0.25.1; extra == 'devdocs'
 Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
 Requires-Dist: aio-pika<10,>=9; extra == 'lint'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'lint'
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
 Requires-Dist: mypy==1.10.0; extra == 'lint'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
-Requires-Dist: ruff==0.4.3; extra == 'lint'
+Requires-Dist: ruff==0.4.4; extra == 'lint'
 Requires-Dist: semgrep==1.70.0; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'nats'
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
-Requires-Dist: coverage[toml]==7.4.4; extra == 'test-core'
+Requires-Dist: coverage[toml]==7.5.1; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
 Requires-Dist: pytest==8.2.0; extra == 'test-core'
 Provides-Extra: testing
-Requires-Dist: coverage[toml]==7.4.4; extra == 'testing'
+Requires-Dist: coverage[toml]==7.5.1; extra == 'testing'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'testing'
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.111.0; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'testing'
 Requires-Dist: pytest==8.2.0; extra == 'testing'
```

