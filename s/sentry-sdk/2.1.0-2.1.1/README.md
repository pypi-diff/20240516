# Comparing `tmp/sentry_sdk-2.1.0.tar.gz` & `tmp/sentry_sdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_sdk-2.1.0.tar", last modified: Mon May  6 09:04:51 2024, max compression
+gzip compressed data, was "sentry_sdk-2.1.1.tar", last modified: Mon May  6 11:53:20 2024, max compression
```

## Comparing `sentry_sdk-2.1.0.tar` & `sentry_sdk-2.1.1.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/_werkzeug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/ai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/ai/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.289579 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.301579 sentry_sdk-2.1.0/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/huggingface_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.305579 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.313579 sentry_sdk-2.1.0/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 09:04:51.000000 sentry_sdk-2.1.0/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:04:51.317579 sentry_sdk-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:04:51.313579 sentry_sdk-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_propagationcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-06 09:04:41.000000 sentry_sdk-2.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.446497 sentry_sdk-2.1.1/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_werkzeug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/huggingface_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.466496 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.470496 sentry_sdk-2.1.1/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.466496 sentry_sdk-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_propagationcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_utils.py
```

### Comparing `sentry_sdk-2.1.0/LICENSE` & `sentry_sdk-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/PKG-INFO` & `sentry_sdk-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.1.0/README.md` & `sentry_sdk-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/_compat.py` & `sentry_sdk-2.1.1/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/_lru_cache.py` & `sentry_sdk-2.1.1/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/_queue.py` & `sentry_sdk-2.1.1/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/_types.py` & `sentry_sdk-2.1.1/sentry_sdk/_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/_werkzeug.py` & `sentry_sdk-2.1.1/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/ai/monitoring.py` & `sentry_sdk-2.1.1/sentry_sdk/ai/monitoring.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/ai/utils.py` & `sentry_sdk-2.1.1/sentry_sdk/ai/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/api.py` & `sentry_sdk-2.1.1/sentry_sdk/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/attachments.py` & `sentry_sdk-2.1.1/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/client.py` & `sentry_sdk-2.1.1/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/consts.py` & `sentry_sdk-2.1.1/sentry_sdk/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,8 +429,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.1.0"
+VERSION = "2.1.1"
```

### Comparing `sentry_sdk-2.1.0/sentry_sdk/crons/api.py` & `sentry_sdk-2.1.1/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/crons/decorator.py` & `sentry_sdk-2.1.1/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/django.py` & `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/debug.py` & `sentry_sdk-2.1.1/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/envelope.py` & `sentry_sdk-2.1.1/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/hub.py` & `sentry_sdk-2.1.1/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/_asgi_common.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/_wsgi_common.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/aiohttp.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/anthropic.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/anthropic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/argv.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/ariadne.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/arq.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/asgi.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/asyncio.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/asyncpg.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/atexit.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/aws_lambda.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/beam.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/boto3.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/bottle.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Callable
     from typing import List
     from typing import Optional
     from typing import TypeVar
+    from typing import Union
 
     from sentry_sdk._types import EventProcessor, Event, Hint, ExcInfo
     from sentry_sdk.tracing import Span
 
     F = TypeVar("F", bound=Callable[..., Any])
 
 
@@ -219,14 +220,24 @@
             for key, value in updated_headers.items():
                 if key.startswith("sentry-"):
                     updated_headers["headers"][key] = value
 
     return updated_headers
 
 
+class NoOpMgr:
+    def __enter__(self):
+        # type: () -> None
+        return None
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        # type: (Any, Any, Any) -> None
+        return None
+
+
 def _wrap_apply_async(f):
     # type: (F) -> F
     @wraps(f)
     @ensure_integration_enabled(CeleryIntegration, f)
     def apply_async(*args, **kwargs):
         # type: (*Any, **Any) -> Any
         # Note: kwargs can contain headers=None, so no setdefault!
@@ -238,17 +249,25 @@
         )
 
         if not propagate_traces:
             return f(*args, **kwargs)
 
         task = args[0]
 
-        with sentry_sdk.start_span(
-            op=OP.QUEUE_SUBMIT_CELERY, description=task.name
-        ) as span:
+        task_started_from_beat = (
+            sentry_sdk.Scope.get_isolation_scope()._name == "celery-beat"
+        )
+
+        span_mgr = (
+            sentry_sdk.start_span(op=OP.QUEUE_SUBMIT_CELERY, description=task.name)
+            if not task_started_from_beat
+            else NoOpMgr()
+        )  # type: Union[Span, NoOpMgr]
+
+        with span_mgr as span:
             kwargs["headers"] = _update_celery_task_headers(
                 kwarg_headers, span, integration.monitor_beat_tasks
             )
             return f(*args, **kwargs)
 
     return apply_async  # type: ignore
```

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/beat.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/beat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/celery/utils.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/chalice.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/clickhouse_driver.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/cloud_resource_context.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/dedupe.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/asgi.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/caching.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/middleware.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/signals_handlers.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/templates.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/transactions.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/django/views.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/excepthook.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/executing.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/falcon.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/fastapi.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/flask.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/gcp.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/gnu_backtrace.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/gql.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/graphene.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/client.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/aio/server.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/client.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/grpc/server.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/httpx.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/huey.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/huggingface_hub.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/langchain.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/langchain.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/logging.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/loguru.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/modules.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/openai.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/pure_eval.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/pymongo.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/pyramid.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/quart.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/redis/__init__.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/redis/asyncio.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/rq.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/sanic.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/serverless.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/socket.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_driver.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/spark/spark_worker.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/sqlalchemy.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/starlette.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/starlite.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/stdlib.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/strawberry.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/threading.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/tornado.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/trytond.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/integrations/wsgi.py` & `sentry_sdk-2.1.1/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/metrics.py` & `sentry_sdk-2.1.1/sentry_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/monitor.py` & `sentry_sdk-2.1.1/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/profiler.py` & `sentry_sdk-2.1.1/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/scope.py` & `sentry_sdk-2.1.1/sentry_sdk/scope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/scrubber.py` & `sentry_sdk-2.1.1/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/serializer.py` & `sentry_sdk-2.1.1/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/session.py` & `sentry_sdk-2.1.1/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/sessions.py` & `sentry_sdk-2.1.1/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/spotlight.py` & `sentry_sdk-2.1.1/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/tracing.py` & `sentry_sdk-2.1.1/sentry_sdk/tracing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/tracing_utils.py` & `sentry_sdk-2.1.1/sentry_sdk/tracing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,14 +417,24 @@
         """
         for key, value in other_dict.items():
             try:
                 setattr(self, key, value)
             except AttributeError:
                 pass
 
+    def __repr__(self):
+        # type: (...) -> str
+        return "<PropagationContext _trace_id={} _span_id={} parent_span_id={} parent_sampled={} dynamic_sampling_context={}>".format(
+            self._trace_id,
+            self._span_id,
+            self.parent_span_id,
+            self.parent_sampled,
+            self.dynamic_sampling_context,
+        )
+
 
 class Baggage:
     """
     The W3C Baggage header information (see https://www.w3.org/TR/baggage/).
     """
 
     __slots__ = ("sentry_items", "third_party_items", "mutable")
```

### Comparing `sentry_sdk-2.1.0/sentry_sdk/transport.py` & `sentry_sdk-2.1.1/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/types.py` & `sentry_sdk-2.1.1/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/utils.py` & `sentry_sdk-2.1.1/sentry_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk/worker.py` & `sentry_sdk-2.1.1/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk.egg-info/PKG-INFO` & `sentry_sdk-2.1.1/sentry_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.1.0/sentry_sdk.egg-info/SOURCES.txt` & `sentry_sdk-2.1.1/sentry_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/sentry_sdk.egg-info/requires.txt` & `sentry_sdk-2.1.1/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/setup.py` & `sentry_sdk-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.1.0",
+    version="2.1.1",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry_sdk-2.1.0/tests/test_api.py` & `sentry_sdk-2.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_basics.py` & `sentry_sdk-2.1.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_client.py` & `sentry_sdk-2.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_conftest.py` & `sentry_sdk-2.1.1/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_crons.py` & `sentry_sdk-2.1.1/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_envelope.py` & `sentry_sdk-2.1.1/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_exceptiongroup.py` & `sentry_sdk-2.1.1/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_lru_cache.py` & `sentry_sdk-2.1.1/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_metrics.py` & `sentry_sdk-2.1.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_monitor.py` & `sentry_sdk-2.1.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_new_scopes_compat.py` & `sentry_sdk-2.1.1/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_new_scopes_compat_event.py` & `sentry_sdk-2.1.1/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_profiler.py` & `sentry_sdk-2.1.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_propagationcontext.py` & `sentry_sdk-2.1.1/tests/test_propagationcontext.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_scope.py` & `sentry_sdk-2.1.1/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_scrubber.py` & `sentry_sdk-2.1.1/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_serializer.py` & `sentry_sdk-2.1.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_sessions.py` & `sentry_sdk-2.1.1/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_spotlight.py` & `sentry_sdk-2.1.1/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_transport.py` & `sentry_sdk-2.1.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_types.py` & `sentry_sdk-2.1.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.0/tests/test_utils.py` & `sentry_sdk-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

