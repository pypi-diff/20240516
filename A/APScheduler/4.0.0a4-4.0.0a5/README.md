# Comparing `tmp/APScheduler-4.0.0a4.tar.gz` & `tmp/apscheduler-4.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APScheduler-4.0.0a4.tar", last modified: Mon Nov 13 00:47:30 2023, max compression
+gzip compressed data, was "apscheduler-4.0.0a5.tar", last modified: Wed May 15 23:14:57 2024, max compression
```

## Comparing `APScheduler-4.0.0a4.tar` & `apscheduler-4.0.0a5.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.717669 APScheduler-4.0.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.693668 APScheduler-4.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.693668 APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.693668 APScheduler-4.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2023-11-13 00:47:30.717669 APScheduler-4.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/integrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23799 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/docs/versionhistory.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/examples/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/gui/qt_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/examples/separate_worker/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/separate_worker/async_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/separate_worker/async_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/separate_worker/example_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/separate_worker/sync_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/separate_worker/sync_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/examples/standalone/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/standalone/async_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/standalone/async_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/standalone/async_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/standalone/sync_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/examples/web/
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/web/asgi_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/web/asgi_noframework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/web/asgi_starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/web/wsgi_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/examples/web/wsgi_noframework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 00:47:30.717669 APScheduler-4.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.693668 APScheduler-4.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.697668 APScheduler-4.0.0a4/src/APScheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2023-11-13 00:47:30.000000 APScheduler-4.0.0a4/src/APScheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-11-13 00:47:30.000000 APScheduler-4.0.0a4/src/APScheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 00:47:30.000000 APScheduler-4.0.0a4/src/APScheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-11-13 00:47:30.000000 APScheduler-4.0.0a4/src/APScheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-13 00:47:30.000000 APScheduler-4.0.0a4/src/APScheduler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/_schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38620 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_schedulers/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)    11099 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_schedulers/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/datastores/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/datastores/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/datastores/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)    38857 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/datastores/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/eventbrokers/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/executors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/executors/async_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/executors/qt.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/executors/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/executors/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/serializers/cbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/serializers/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.701669 APScheduler-4.0.0a4/src/apscheduler/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/calendarinterval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/combining.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.705669 APScheduler-4.0.0a4/src/apscheduler/triggers/cron/
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/cron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/cron/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/cron/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/src/apscheduler/triggers/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.705669 APScheduler-4.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9896 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18756 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_eventbrokers.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.705669 APScheduler-4.0.0a4/tests/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/triggers/test_calendarinterval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/triggers/test_combining.py
--rw-r--r--   0 runner    (1001) docker     (127)    17910 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/triggers/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/triggers/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tests/triggers/test_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 00:47:30.705669 APScheduler-4.0.0a4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)  8528260 2023-11-13 00:47:19.000000 APScheduler-4.0.0a4/tools/dockerize
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.556443 apscheduler-4.0.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.524443 apscheduler-4.0.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.524443 apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/features_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.524443 apscheduler-4.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-15 23:14:57.556443 apscheduler-4.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/integrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26892 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/docs/versionhistory.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/examples/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/gui/qt_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/examples/separate_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/separate_worker/async_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/separate_worker/async_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/separate_worker/example_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/separate_worker/sync_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/separate_worker/sync_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/examples/standalone/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/standalone/async_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/standalone/async_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/standalone/async_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/standalone/sync_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.528443 apscheduler-4.0.0a5/examples/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/web/asgi_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/web/asgi_noframework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/web/asgi_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/web/wsgi_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/examples/web/wsgi_noframework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:14:57.556443 apscheduler-4.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.524443 apscheduler-4.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.552443 apscheduler-4.0.0a5/src/APScheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-15 23:14:57.000000 apscheduler-4.0.0a5/src/APScheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-15 23:14:57.000000 apscheduler-4.0.0a5/src/APScheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:14:57.000000 apscheduler-4.0.0a5/src/APScheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-15 23:14:57.000000 apscheduler-4.0.0a5/src/APScheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 23:14:57.000000 apscheduler-4.0.0a5/src/APScheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.532443 apscheduler-4.0.0a5/src/apscheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.532443 apscheduler-4.0.0a5/src/apscheduler/_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42608 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_schedulers/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_schedulers/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.536443 apscheduler-4.0.0a5/src/apscheduler/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/datastores/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/datastores/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28438 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/datastores/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41232 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/datastores/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.536443 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/eventbrokers/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.536443 apscheduler-4.0.0a5/src/apscheduler/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/executors/async_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/executors/qt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/executors/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/executors/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.536443 apscheduler-4.0.0a5/src/apscheduler/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/serializers/cbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/serializers/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.540443 apscheduler-4.0.0a5/src/apscheduler/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/calendarinterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/combining.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.540443 apscheduler-4.0.0a5/src/apscheduler/triggers/cron/
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/cron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8250 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/cron/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/cron/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/src/apscheduler/triggers/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.540443 apscheduler-4.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19688 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/test_eventbrokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/test_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43636 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/test_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.540443 apscheduler-4.0.0a5/tests/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/triggers/test_calendarinterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/triggers/test_combining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/triggers/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/triggers/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tests/triggers/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:14:57.540443 apscheduler-4.0.0a5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)  8528260 2024-05-15 23:14:52.000000 apscheduler-4.0.0a5/tools/dockerize
```

### Comparing `APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/bug_report.yaml` & `apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/.github/ISSUE_TEMPLATE/features_request.yaml` & `apscheduler-4.0.0a5/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/.github/workflows/publish.yml` & `apscheduler-4.0.0a5/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
       with:
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create packages
       run: python -m build
     - name: Archive packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: dist
         path: dist
 
   publish:
     name: Publish build artifacts to the PyPI
     needs: build
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
     steps:
     - name: Retrieve packages
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
     - name: Upload packages
       uses: pypa/gh-action-pypi-publish@release/v1
 
   release:
     name: Create a GitHub release
     needs: build
     runs-on: ubuntu-latest
```

### Comparing `APScheduler-4.0.0a4/.github/workflows/test.yml` & `apscheduler-4.0.0a5/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,40 @@
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.11", "3.12"]
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Start external services
       run: docker compose up -d
     - name: Install the project and its dependencies
       run: pip install -e .[test]
     - name: Test with pytest
-      run: |
-        coverage run -m pytest -v
-        coverage xml
+      run: coverage run -m pytest -v
+    - name: Generate coverage report
+      run: coverage xml
     - name: Upload Coverage
       uses: coverallsapp/github-action@v2
       with:
         parallel: true
         file: coverage.xml
 
   test-pypy:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: pypy-3.10
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Start external services
       run: docker compose up -d
     - name: Install the project and its dependencies
@@ -58,26 +58,26 @@
       matrix:
         os: [macos-latest, windows-latest]
         python-version: ["3.8", "3.12"]
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
         allow-prereleases: true
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Install the project and its dependencies
       run: pip install -e .[test]
     - name: Test with pytest
-      run: |
-        coverage run -m pytest -v -m "not external_service"
-        coverage xml
+      run: coverage run -m pytest -v -m "not external_service"
+    - name: Generate coverage report
+      run: coverage xml
     - name: Upload Coverage
       uses: coverallsapp/github-action@v2
       with:
         parallel: true
         file: coverage.xml
 
   coveralls:
```

### Comparing `APScheduler-4.0.0a4/.pre-commit-config.yaml` & `apscheduler-4.0.0a5/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.4
+    rev: v0.4.4
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
-
-  - repo: https://github.com/psf/black
-    rev: 23.10.1
-    hooks:
-      - id: black
+      - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.6.1
+    rev: v1.10.0
     hooks:
       - id: mypy
         additional_dependencies:
           - attrs == 23.1.0
+          - pymongo == 4.6.0
           - redis == 5.0.1
           - sqlalchemy == 2.0.23
           - tzlocal == 5.2
         exclude: docs/conf.py
         stages: [manual]
 
   - repo: https://github.com/codespell-project/codespell
```

### Comparing `APScheduler-4.0.0a4/LICENSE.txt` & `apscheduler-4.0.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/PKG-INFO` & `apscheduler-4.0.0a5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: APScheduler
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: In-process task scheduler with Cron-like capabilities
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://apscheduler.readthedocs.io/en/master/
 Project-URL: Changelog, https://apscheduler.readthedocs.io/en/master/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/apscheduler
 Project-URL: Issue tracker, https://github.com/agronholm/apscheduler/issues
 Keywords: scheduling,cron
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -30,36 +31,34 @@
 Provides-Extra: asyncpg
 Requires-Dist: asyncpg>=0.20; extra == "asyncpg"
 Provides-Extra: cbor
 Requires-Dist: cbor2>=5.0; extra == "cbor"
 Provides-Extra: mongodb
 Requires-Dist: pymongo>=4; extra == "mongodb"
 Provides-Extra: mqtt
-Requires-Dist: paho-mqtt>=1.5; extra == "mqtt"
+Requires-Dist: paho-mqtt>=2.0; extra == "mqtt"
 Provides-Extra: redis
-Requires-Dist: redis>=4.4.0; extra == "redis"
+Requires-Dist: redis>=5.0.1; extra == "redis"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy>=2.0.19; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy[asyncio]>=2.0.19; extra == "sqlalchemy"
 Provides-Extra: test
 Requires-Dist: APScheduler[cbor,mongodb,mqtt,redis,sqlalchemy]; extra == "test"
 Requires-Dist: asyncpg>=0.20; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: aiosqlite>=0.19; extra == "test"
 Requires-Dist: anyio[trio]; extra == "test"
 Requires-Dist: asyncmy>=0.2.5; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: coverage>=7; extra == "test"
-Requires-Dist: freezegun; extra == "test"
-Requires-Dist: paho-mqtt>=1.5; extra == "test"
 Requires-Dist: psycopg; extra == "test"
 Requires-Dist: pymongo>=4; extra == "test"
 Requires-Dist: pymysql[rsa]; extra == "test"
 Requires-Dist: PySide6>=6.6; platform_python_implementation == "CPython" and extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: pytest-freezer; extra == "test"
-Requires-Dist: pytest-lazy-fixture; extra == "test"
+Requires-Dist: pytest>=7.4; extra == "test"
+Requires-Dist: pytest-lazy-fixtures; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: time-machine>=2.13.0; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: uwsgi; (platform_python_implementation == "CPython" and platform_system == "Linux") and extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "doc"
 Requires-Dist: sphinx-tabs>=3.3.1; extra == "doc"
```

### Comparing `APScheduler-4.0.0a4/README.rst` & `apscheduler-4.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/api.rst` & `apscheduler-4.0.0a5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/conf.py` & `apscheduler-4.0.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/contributing.rst` & `apscheduler-4.0.0a5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/extending.rst` & `apscheduler-4.0.0a5/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/faq.rst` & `apscheduler-4.0.0a5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/integrations.rst` & `apscheduler-4.0.0a5/docs/integrations.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/migration.rst` & `apscheduler-4.0.0a5/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/docs/userguide.rst` & `apscheduler-4.0.0a5/docs/userguide.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
 The core concept of APScheduler is to give the user the ability to queue Python code to
 be executed, either as soon as possible, later at a given time, or on a recurring
 schedule.
 
 The *scheduler* is the user-facing interface of the system. When it's running, it does
 two things concurrently. The first is processing *schedules*. From its *data store*,
-it fetches `schedules <schedule>`_ due to be run. For each such schedule, it then uses
+it fetches :ref:`schedules <schedule>` due to be run. For each such schedule, it then uses
 the schedule's trigger_ to calculate run times up to the present. The scheduler then
 creates one or more jobs (controllable by configuration) based on these run times and
 adds them to the data store.
 
-The second role of the scheduler is running `jobs <job>`_ The scheduler asks the
+The second role of the scheduler is running :ref:`jobs <job>`. The scheduler asks the
 `data store`_ for jobs, and then starts running those jobs. If the data store signals
 that it has new jobs, the scheduler will try to acquire those jobs if it is capable of
 accommodating more. When a scheduler completes a job, it will then also ask the data
 store for as many more jobs as it can handle.
 
 By default, schedulers operate in both of these roles, but can be configured to only
 process schedules or run jobs if deemed necessary. It may even be desirable to use the
@@ -86,69 +86,70 @@
 
 A *job* is request for a task_ to be run. It can be created automatically from a
 schedule when a scheduler processes it, or it can be directly created by the user if
 they directly request a task_ to be run.
 
 .. _data store:
 
-A *data store* is used to store `schedules <schedule>`_ and `jobs <job>`_, and to keep
-track of `tasks <task>`_.
+A *data store* is used to store :ref:`schedules <schedule>` and :ref:`jobs <job>`, and to keep
+track of :ref:`tasks <task>`.
 
 .. _job executor:
 
 A *job executor* runs the job_, by calling the function associated with the job's task.
 An executor could directly call the callable_, or do it in another thread, subprocess or
 even some external service.
 
 .. _event broker:
 
 An *event broker* delivers published events to all interested parties. It facilitates
 the cooperation between schedulers by notifying them of new or updated
-`schedules <schedule>`_ and `jobs <job>`_.
+:ref:`schedules <schedule>` and :ref:`jobs <job>`.
 
 .. _scheduler:
 
 A *scheduler* is the main interface of this library. It houses both a `data store`_ and
-an `event broker`_, plus one or more `job executors <job executor>`_. It contains
+an `event broker`_, plus one or more :ref:`job executors <job executor>`. It contains
 methods users can use to work with tasks, schedules and jobs. Behind the scenes, it also
 processes due schedules, spawning jobs and updating the next run times. It also
-processes available jobs, making the appropriate `job executors <job executor>`_ to run
+processes available jobs, making the appropriate :ref:`job executors <job executor>` to run
 them, and then sending back the results to the `data store`_.
 
 Running the scheduler
 =====================
 
 The scheduler_ comes in two flavors: synchronous and asynchronous. The synchronous
 scheduler actually runs an asynchronous scheduler behind the scenes in a dedicated
-thread, so if your app runs on :mod:`asyncio` or Trio_, you should prefer the
-asynchronous scheduler.
+thread, so if your app runs on :mod:`asyncio` or Trio_, you should prefer the asynchronous
+scheduler.
 
 The scheduler can run either in the foreground, blocking on a call to
 :meth:`~Scheduler.run_until_stopped`, or in the background where it does its work while
 letting the rest of the program run.
 
 If the only intent of your program is to run scheduled tasks, then you should start the
 scheduler with :meth:`~Scheduler.run_until_stopped`. But if you need to do other things
 too, then you should call :meth:`~Scheduler.start_in_background` before running the rest
 of the program.
 
 In almost all cases, the scheduler should be used as a context manager. This initializes
 the underlying `data store`_ and `event broker`_, allowing you to use the scheduler for
-manipulating `tasks <task>`_, `schedules <schedule>`_ and jobs prior to starting the
+manipulating :ref:`tasks <task>`, :ref:`schedules <schedule>` and jobs prior to starting the
 processing of schedules and jobs. Exiting the context manager will shut down the
 scheduler and its underlying services. This mode of operation is mandatory for the
 asynchronous scheduler when running it in the background, but it is preferred for the
 synchronous scheduler too.
 
 As a special consideration (for use with WSGI_ based web frameworks), the synchronous
 scheduler can be run in the background without being used as a context manager. In this
 scenario, the scheduler adds an :mod:`atexit` hook that will perform an orderly shutdown
 of the scheduler before the process terminates.
 
 .. _WSGI: https://wsgi.readthedocs.io/en/latest/what.html
+.. _Trio: https://trio.readthedocs.io/en/stable/
 
 .. warning:: If you start the scheduler in the background and let the script finish
    execution, the scheduler will automatically shut down as well.
 
 .. tabs::
 
    .. code-tab:: python Synchronous (run in foreground)
@@ -202,15 +203,15 @@
      asyncio.run(main())
 
 .. _configuring-tasks:
 
 Configuring tasks
 =================
 
-In order to add `schedules <schedule>`_ or `jobs <job>`_ to the `data store`_, you need
+In order to add :ref:`schedules <schedule>` or :ref:`jobs <job>` to the `data store`_, you need
 to have a task_ that defines which callable_ will be called when each job_ is run.
 
 In most cases, you don't need to go through this step, and instead have a task_
 implicitly created for you by the methods that add `schedules or jobs.
 
 Explicitly configuring a task is generally only necessary in the following cases:
 
@@ -309,44 +310,71 @@
 
 In some cases, you want to run tasks directly, without involving schedules:
 
 * You're only interested in using the scheduler system as a job queue
 * You're interested in the job's return value
 
 To queue a job and wait for its completion and get the result, the easiest way is to
-use :meth:`~Scheduler.run_job`. If you prefer to just launch
-a job and not wait for its result, use
-:meth:`~Scheduler.add_job` instead. If you want to get the
-results later, you can then call
-:meth:`~Scheduler.get_job_result` with the job ID you got
-from :meth:`~Scheduler.add_job`.
+use :meth:`~Scheduler.run_job`. If you prefer to just launch a job and not wait for its
+result, use :meth:`~Scheduler.add_job` instead. If you want to get the results later, you
+need to pass an appropriate ``result_expiration_time`` parameter to
+:meth:`~Scheduler.add_job` so that the result is saved. Then, you can call
+:meth:`~Scheduler.get_job_result` with the job ID you got from
+:meth:`~Scheduler.add_job` to retrieve the result.
 
 Removing schedules
 ------------------
 
 To remove a previously added schedule, call
 :meth:`~Scheduler.remove_schedule`. Pass the identifier of
 the schedule you want to remove as an argument. This is the ID you got from
 :meth:`~Scheduler.add_schedule`.
 
 Note that removing a schedule does not cancel any jobs derived from it, but does prevent
 further jobs from being created from that schedule.
 
+Pausing schedules
+-----------------
+
+To pause a schedule, call :meth:`~Scheduler.pause_schedule`. Pass the identifier of the
+schedule you want to pause as an argument. This is the ID you got from
+:meth:`~Scheduler.add_schedule`.
+
+Pausing a schedule prevents any new jobs from being created from it, but does not cancel
+any jobs that have already been created from that schedule.
+
+The schedule can be unpaused by calling :meth:`~Scheduler.unpause_schedule` with the
+identifier of the schedule you want to unpause.
+
+By default the schedule will retain the next fire time it had when it was paused, which
+may result in the schedule being considered to have misfired when it is unpaused,
+resulting in whatever misfire behavior it has configured
+(see :ref:`controlling-how-much-a-job-can-be-started-late` for more details).
+
+The ``resume_from`` parameter can be used to specify the time from which the schedule
+should be resumed. This can be used to avoid the misfire behavior mentioned above. It
+can be either a datetime object, or the string ``"now"`` as a convenient shorthand for
+the current datetime. If this parameter is provided, the schedules trigger will be
+repeatedly advanced to determine a next fire time that is at or after the specified time
+to resume from.
+
 Limiting the number of concurrently executing instances of a job
 ----------------------------------------------------------------
 
 It is possible to control the maximum number of concurrently running jobs for a
 particular task. By default, only one job is allowed to be run for every task.
 This means that if the job is about to be run but there is another job for the same task
 still running, the later job is terminated with the outcome of
 :attr:`~JobOutcome.missed_start_deadline`.
 
 To allow more jobs to be concurrently running for a task, pass the desired maximum
 number as the ``max_running_jobs`` keyword argument to :meth:`~Scheduler.add_schedule`.
 
+.. _controlling-how-much-a-job-can-be-started-late:
+
 Controlling how much a job can be started late
 ----------------------------------------------
 
 Some tasks are time sensitive, and should not be run at all if they fail to be started
 on time (like, for example, if the scheduler(s) were down while they were supposed to be
 running the scheduled jobs). You can control this time limit with the
 ``misfire_grace_time`` option passed to :meth:`~Scheduler.add_schedule`. A scheduler
@@ -437,24 +465,32 @@
 
         async def listener(event: Event) -> None:
             print(f"Received {event.__class__.__name__}")
 
         scheduler.subscribe(listener, {JobAcquired, JobReleased})
 
 This example subscribes to the :class:`~JobAcquired` and
-:class:`~JobAcquired` event types. The callback will receive an event of
+:class:`~JobReleased` event types. The callback will receive an event of
 either type, and prints the name of the class of the received event.
 
 Asynchronous schedulers and workers support both synchronous and asynchronous callbacks,
 but their synchronous counterparts only support synchronous callbacks.
 
 When **distributed** event brokers (that is, other than the default one) are being used,
 events other than the ones relating to the life cycles of schedulers and workers, will
 be sent to all schedulers and workers connected to that event broker.
 
+Clean-up of expired jobs and schedules
+======================================
+
+Expired job results and finished schedules are, by default, automatically cleaned up by
+each running scheduler on 15 minute intervals (counting from the scheduler's start
+time). This can be adjusted (or disabled entirely) through the ``cleanup_interval``
+configuration option.
+
 Deployment
 ==========
 
 Using persistent data stores
 ----------------------------
 
 The default data store, :class:`~datastores.memory.MemoryDataStore`, stores
@@ -533,14 +569,41 @@
 You can then run one or more schedulers against the same data store and event broker
 elsewhere where they don't disturb the web application. These schedulers will do all the
 heavy lifting like processing schedules and running jobs.
 
 .. seealso:: A practical example of this separation of concerns can be found in the
     :file:`examples/separate_worker` directory.
 
+Explicitly assigning an identity to the scheduler
+-------------------------------------------------
+
+If you're running one or more schedulers against a persistent data store in a production
+setting, it'd be wise to assign each scheduler a custom identity. The reason for this is
+twofold:
+
+#. It helps you figure out which jobs are being run where
+#. It allows crashed jobs to cleared out quicker, as other schedulers aren't allowed to
+   clean them up until the jobs' timeouts expire
+
+The best choice would be something that the environment guarantees to be unique among
+all the scheduler instances but stays the same when the scheduler instance is restarted.
+For example, on Kubernetes, this would be the name of the pod where the scheduler is
+running, assuming of course that there is only one scheduler running in each pod against
+the same data store.
+
+Of course, if you're only ever running one scheduler against a persistent data store,
+you can just use a static scheduler ID.
+
+If no ID is explicitly given, the scheduler generates an ID by concatenating the
+following:
+
+* the current host name
+* the current process ID
+* the ID of the scheduler instance
+
 .. _troubleshooting:
 
 Troubleshooting
 ===============
 
 If something isn't working as expected, it will be helpful to increase the logging level
 of the ``apscheduler`` logger to the ``DEBUG`` level.
```

### Comparing `APScheduler-4.0.0a4/docs/versionhistory.rst` & `apscheduler-4.0.0a5/docs/versionhistory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,48 @@
 Version history
 ===============
 
 To find out how to migrate your application from a previous version of
 APScheduler, see the :doc:`migration section <migration>`.
 
-**v4.0.0a4**
+**4.0.0a5**
+
+- **BREAKING** Added the ``cleanup()`` scheduler method and a configuration option
+  (``cleanup_interval``). A corresponding abstract method was added to the ``DataStore``
+  class. This method purges expired job results and schedules that have exhausted their
+  triggers and have no more associated jobs running. Previously, schedules were
+  automatically deleted instantly once their triggers could no longer produce any fire
+  times.
+- **BREAKING** Made publishing ``JobReleased`` events the responsibility of the
+  ``DataStore`` implementation, rather than the scheduler, for consistency with the
+  ``acquire_jobs()`` method
+- **BREAKING** The ``started_at`` field was moved from ``Job`` to ``JobResult``
+- **BREAKING** Removed the ``from_url()`` class methods of ``SQLAlchemyDataStore``,
+  ``MongoDBDataStore`` and ``RedisEventBroker`` in favor of the ability to pass a
+  connection url to the initializer
+- Added the ability to pause and unpause schedules (PR by @WillDaSilva)
+- Added the ``scheduled_start`` field to the ``JobAcquired`` event
+- Added the ``scheduled_start`` and ``started_at`` fields to the ``JobReleased`` event
+- Fixed large parts of ``MongoDBDataStore`` still calling blocking functions in the
+  event loop thread
+- Fixed JSON serialization of triggers that had been used at least once
+- Fixed dialect name checks in the SQLAlchemy job store
+- Fixed JSON and CBOR serializers unable to serialize enums
+- Fixed infinite loop in CalendarIntervalTrigger with UTC timezone (PR by unights)
+- Fixed scheduler not resuming job processing when ``max_concurrent_jobs`` had been
+  reached and then a job was completed, thus making job processing possible again
+  (PR by MohammadAmin Vahedinia)
+- Fixed the shutdown procedure of the Redis event broker
+- Fixed ``SQLAlchemyDataStore`` not respecting custom schema name when creating enums
+- Fixed skipped intervals with overlapping schedules in ``AndTrigger``
+  (#911 <https://github.com/agronholm/apscheduler/issues/911>_; PR by Bennett Meares)
+- Fixed implicitly created client instances in data stores and event brokers not being
+  closed along with the store/broker
+
+**4.0.0a4**
 
 - **BREAKING** Renamed any leftover fields named ``executor`` to ``job_executor``
   (this breaks data store compatibility)
 - **BREAKING** Switched to using the timezone aware timestamp column type on Oracle
 - **BREAKING** Fixed precision issue with interval columns on MySQL
 - **BREAKING** Fixed datetime comparison issues on SQLite and MySQL
 - **BREAKING** Worked around datetime microsecond precision issue on MongoDB
```

### Comparing `APScheduler-4.0.0a4/examples/README.rst` & `apscheduler-4.0.0a5/examples/README.rst`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/gui/qt_executor.py` & `apscheduler-4.0.0a5/examples/gui/qt_executor.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/separate_worker/async_scheduler.py` & `apscheduler-4.0.0a5/examples/separate_worker/async_scheduler.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/separate_worker/async_worker.py` & `apscheduler-4.0.0a5/examples/separate_worker/async_worker.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/separate_worker/sync_scheduler.py` & `apscheduler-4.0.0a5/examples/separate_worker/sync_scheduler.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/separate_worker/sync_worker.py` & `apscheduler-4.0.0a5/examples/separate_worker/sync_worker.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/standalone/async_memory.py` & `apscheduler-4.0.0a5/examples/standalone/async_memory.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/standalone/async_mysql.py` & `apscheduler-4.0.0a5/examples/standalone/async_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Example demonstrating use of the asynchronous scheduler with persistence via MySQL or
 MariaDB in a simple asyncio app.
 
 Requires the "mysql" service to be running.
 To install prerequisites: pip install sqlalchemy asyncmy
-To run: python async_postgres.py
+To run: python async_mysql.py
 
 It should print a line on the console on a one-second interval.
 """
 
 from __future__ import annotations
 
 from asyncio import run
```

### Comparing `APScheduler-4.0.0a4/examples/standalone/async_postgres.py` & `apscheduler-4.0.0a5/examples/standalone/async_postgres.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/web/asgi_fastapi.py` & `apscheduler-4.0.0a5/examples/web/asgi_fastapi.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/web/asgi_noframework.py` & `apscheduler-4.0.0a5/examples/web/asgi_noframework.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/web/asgi_starlette.py` & `apscheduler-4.0.0a5/examples/web/asgi_starlette.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/examples/web/wsgi_flask.py` & `apscheduler-4.0.0a5/examples/web/wsgi_flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
 @app.route("/")
 def hello_world():
     return "<p>Hello, World!</p>"
 
 
 engine = create_engine("postgresql+psycopg://postgres:secret@localhost/testdb")
 data_store = SQLAlchemyDataStore(engine)
-event_broker = RedisEventBroker.from_url("redis://localhost")
+event_broker = RedisEventBroker("redis://localhost")
 scheduler = Scheduler(data_store, event_broker)
 scheduler.add_schedule(tick, IntervalTrigger(seconds=1), id="tick")
 scheduler.start_in_background()
```

### Comparing `APScheduler-4.0.0a4/examples/web/wsgi_noframework.py` & `apscheduler-4.0.0a5/examples/web/wsgi_noframework.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         ("Content-Type", "text/plain"),
         ("Content-Length", str(len(response_body))),
     ]
     start_response("200 OK", response_headers)
     return [response_body]
 
 
-engine = create_engine("postgresql+psycopg://postgres:secret@localhost/testdb")
+engine = create_engine("mysql+pymysql://root:secret@localhost/testdb")
 data_store = SQLAlchemyDataStore(engine)
-event_broker = RedisEventBroker.from_url("redis://localhost")
+event_broker = RedisEventBroker("redis://localhost")
 scheduler = Scheduler(data_store, event_broker)
 scheduler.add_schedule(tick, IntervalTrigger(seconds=1), id="tick")
 scheduler.start_in_background()
```

### Comparing `APScheduler-4.0.0a4/pyproject.toml` & `apscheduler-4.0.0a5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 description = "In-process task scheduler with Cron-like capabilities"
 readme = "README.rst"
 authors = [{name = "Alex Grönholm", email = "alex.gronholm@nextday.fi"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
+    "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -40,34 +41,32 @@
 "Source code" = "https://github.com/agronholm/apscheduler"
 "Issue tracker" = "https://github.com/agronholm/apscheduler/issues"
 
 [project.optional-dependencies]
 asyncpg = ["asyncpg >= 0.20"]
 cbor = ["cbor2 >= 5.0"]
 mongodb = ["pymongo >= 4"]
-mqtt = ["paho-mqtt >= 1.5"]
-redis = ["redis >= 4.4.0"]
-sqlalchemy = ["sqlalchemy >= 2.0.19"]
+mqtt = ["paho-mqtt >= 2.0"]
+redis = ["redis >= 5.0.1"]
+sqlalchemy = ["sqlalchemy[asyncio] >= 2.0.19"]
 test = [
     "APScheduler[cbor,mongodb,mqtt,redis,sqlalchemy]",
     "asyncpg >= 0.20; python_implementation == 'CPython'",
     "aiosqlite >= 0.19",
     "anyio[trio]",
     "asyncmy >= 0.2.5; python_implementation == 'CPython'",
     "coverage >= 7",
-    "freezegun",
-    "paho-mqtt >= 1.5",
     "psycopg",
     "pymongo >= 4",
     "pymysql[rsa]",
     "PySide6 >= 6.6; python_implementation == 'CPython'",
-    "pytest >= 7.4.0",
-    "pytest-freezer",
-    "pytest-lazy-fixture",
+    "pytest >= 7.4",
+    "pytest-lazy-fixtures",
     "pytest-mock",
+    "time-machine >= 2.13.0; python_implementation == 'CPython'",
     "uwsgi; python_implementation == 'CPython' and platform_system == 'Linux'",
 ]
 doc = [
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-rtd-theme >= 1.3.0",
     "sphinx-tabs >= 3.3.1",
@@ -87,29 +86,34 @@
 
 [tool.coverage.run]
 source = ["apscheduler"]
 
 [tool.coverage.report]
 show_missing = true
 
-[tool.ruff]
-select = [
+[tool.ruff.lint]
+extend-select = [
     "ASYNC",        # flake8-async
-    "E", "F", "W",  # default Flake8
     "G",            # flake8-logging-format
     "I",            # isort
     "ISC",          # flake8-implicit-str-concat
     "PGH",          # pygrep-hooks
-    "RUF100",       # unused noqa (yesqa)
+    "RUF",          # ruff specific rules
+    "TRIO",         # trio/anyio rules
     "UP",           # pyupgrade
+    "W",            # pycodestyle warnings
+]
+ignore = [
+    "RUF001",
+    "RUF002",
 ]
-src = ["src"]
 
-[tool.ruff.isort]
-"required-imports" = ["from __future__ import annotations"]
+[tool.ruff.lint.isort]
+known-first-party = ["apscheduler"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.mypy]
 python_version = "3.10"
 ignore_missing_imports = true
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `APScheduler-4.0.0a4/src/APScheduler.egg-info/PKG-INFO` & `apscheduler-4.0.0a5/src/APScheduler.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: APScheduler
-Version: 4.0.0a4
+Version: 4.0.0a5
 Summary: In-process task scheduler with Cron-like capabilities
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://apscheduler.readthedocs.io/en/master/
 Project-URL: Changelog, https://apscheduler.readthedocs.io/en/master/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/apscheduler
 Project-URL: Issue tracker, https://github.com/agronholm/apscheduler/issues
 Keywords: scheduling,cron
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -30,36 +31,34 @@
 Provides-Extra: asyncpg
 Requires-Dist: asyncpg>=0.20; extra == "asyncpg"
 Provides-Extra: cbor
 Requires-Dist: cbor2>=5.0; extra == "cbor"
 Provides-Extra: mongodb
 Requires-Dist: pymongo>=4; extra == "mongodb"
 Provides-Extra: mqtt
-Requires-Dist: paho-mqtt>=1.5; extra == "mqtt"
+Requires-Dist: paho-mqtt>=2.0; extra == "mqtt"
 Provides-Extra: redis
-Requires-Dist: redis>=4.4.0; extra == "redis"
+Requires-Dist: redis>=5.0.1; extra == "redis"
 Provides-Extra: sqlalchemy
-Requires-Dist: sqlalchemy>=2.0.19; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy[asyncio]>=2.0.19; extra == "sqlalchemy"
 Provides-Extra: test
 Requires-Dist: APScheduler[cbor,mongodb,mqtt,redis,sqlalchemy]; extra == "test"
 Requires-Dist: asyncpg>=0.20; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: aiosqlite>=0.19; extra == "test"
 Requires-Dist: anyio[trio]; extra == "test"
 Requires-Dist: asyncmy>=0.2.5; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: coverage>=7; extra == "test"
-Requires-Dist: freezegun; extra == "test"
-Requires-Dist: paho-mqtt>=1.5; extra == "test"
 Requires-Dist: psycopg; extra == "test"
 Requires-Dist: pymongo>=4; extra == "test"
 Requires-Dist: pymysql[rsa]; extra == "test"
 Requires-Dist: PySide6>=6.6; platform_python_implementation == "CPython" and extra == "test"
-Requires-Dist: pytest>=7.4.0; extra == "test"
-Requires-Dist: pytest-freezer; extra == "test"
-Requires-Dist: pytest-lazy-fixture; extra == "test"
+Requires-Dist: pytest>=7.4; extra == "test"
+Requires-Dist: pytest-lazy-fixtures; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: time-machine>=2.13.0; platform_python_implementation == "CPython" and extra == "test"
 Requires-Dist: uwsgi; (platform_python_implementation == "CPython" and platform_system == "Linux") and extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "doc"
 Requires-Dist: sphinx-tabs>=3.3.1; extra == "doc"
```

### Comparing `APScheduler-4.0.0a4/src/APScheduler.egg-info/SOURCES.txt` & `apscheduler-4.0.0a5/src/APScheduler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .mailmap
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE.txt
 README.rst
 docker-compose.yml
 pyproject.toml
+.github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.yaml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/features_request.yaml
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/api.rst
 docs/conf.py
@@ -85,15 +86,14 @@
 src/apscheduler/triggers/interval.py
 src/apscheduler/triggers/cron/__init__.py
 src/apscheduler/triggers/cron/expressions.py
 src/apscheduler/triggers/cron/fields.py
 tests/conftest.py
 tests/test_datastores.py
 tests/test_eventbrokers.py
-tests/test_events.py
 tests/test_marshalling.py
 tests/test_schedulers.py
 tests/test_serializers.py
 tests/triggers/test_calendarinterval.py
 tests/triggers/test_combining.py
 tests/triggers/test_cron.py
 tests/triggers/test_date.py
```

### Comparing `APScheduler-4.0.0a4/src/APScheduler.egg-info/requires.txt` & `apscheduler-4.0.0a5/src/APScheduler.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,37 +18,35 @@
 sphinx-rtd-theme>=1.3.0
 sphinx-tabs>=3.3.1
 
 [mongodb]
 pymongo>=4
 
 [mqtt]
-paho-mqtt>=1.5
+paho-mqtt>=2.0
 
 [redis]
-redis>=4.4.0
+redis>=5.0.1
 
 [sqlalchemy]
-sqlalchemy>=2.0.19
+sqlalchemy[asyncio]>=2.0.19
 
 [test]
 APScheduler[cbor,mongodb,mqtt,redis,sqlalchemy]
 aiosqlite>=0.19
 anyio[trio]
 coverage>=7
-freezegun
-paho-mqtt>=1.5
 psycopg
 pymongo>=4
 pymysql[rsa]
-pytest>=7.4.0
-pytest-freezer
-pytest-lazy-fixture
+pytest>=7.4
+pytest-lazy-fixtures
 pytest-mock
 
 [test:platform_python_implementation == "CPython"]
 asyncpg>=0.20
 asyncmy>=0.2.5
 PySide6>=6.6
+time-machine>=2.13.0
 
 [test:platform_python_implementation == "CPython" and platform_system == "Linux"]
 uwsgi
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/__init__.py` & `apscheduler-4.0.0a5/src/apscheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_context.py` & `apscheduler-4.0.0a5/src/apscheduler/_context.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_enums.py` & `apscheduler-4.0.0a5/src/apscheduler/_enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     scheduler = auto()
     worker = auto()
     both = auto()
 
 
 class RunState(Enum):
     """
-    Used to track the running state of schedulers and workers.
+    Used to track the running state of schedulers.
 
     .. attribute:: starting
 
         not running yet, but in the process of starting
 
     .. attribute:: started
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_events.py` & `apscheduler-4.0.0a5/src/apscheduler/_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from __future__ import annotations
 
 from datetime import datetime, timezone
 from functools import partial
 from traceback import format_tb
-from typing import Any
+from typing import Any, TypeVar
 from uuid import UUID
 
 import attrs
 from attrs.converters import optional
 
-from . import abc
 from ._converters import as_aware_datetime, as_enum, as_uuid
 from ._enums import JobOutcome
-from ._structures import JobResult
+from ._structures import Job, JobResult
 from ._utils import qualified_name
 
-
-def serialize(inst, field, value):
-    if isinstance(value, frozenset):
-        return list(value)
-    elif isinstance(value, JobOutcome):
-        return value.name
-
-    return value
+T_Event = TypeVar("T_Event", bound="Event")
 
 
 @attrs.define(kw_only=True, frozen=True)
 class Event:
     """
     Base class for all events.
 
-    :ivar timestamp: the time when the event occurrent
+    :ivar timestamp: the time when the event occurred
     """
 
     timestamp: datetime = attrs.field(
         factory=partial(datetime.now, timezone.utc), converter=as_aware_datetime
     )
 
-    def marshal(self, serializer: abc.Serializer) -> dict[str, Any]:
-        return attrs.asdict(self, value_serializer=serialize)
+    def marshal(self) -> dict[str, Any]:
+        return attrs.asdict(self)
 
     @classmethod
-    def unmarshal(cls, serializer: abc.Serializer, marshalled: dict[str, Any]) -> Event:
+    def unmarshal(cls, marshalled: dict[str, Any]) -> Event:
         return cls(**marshalled)
 
 
 #
 # Data store events
 #
 
@@ -214,63 +206,110 @@
 
     exception: BaseException | None = None
 
 
 @attrs.define(kw_only=True, frozen=True)
 class JobAcquired(SchedulerEvent):
     """
-    Signals that a worker has acquired a job for processing.
+    Signals that a scheduler has acquired a job for processing.
 
     :param job_id: the ID of the job that was acquired
     :param scheduler_id: the ID of the scheduler that acquired the job
+    :param task_id: ID of the task the job belongs to
+    :param schedule_id: ID of the schedule that
+    :param scheduled_start: the time the job was scheduled to start via a schedule (if
+        any)
     """
 
     job_id: UUID = attrs.field(converter=as_uuid)
     scheduler_id: str
+    task_id: str
+    schedule_id: str | None = None
+    scheduled_start: datetime | None = attrs.field(converter=as_aware_datetime)
+
+    @classmethod
+    def from_job(cls, job: Job, scheduler_id: str) -> JobAcquired:
+        """
+        Create a new job-acquired event from a job and a scheduler ID.
+
+        :param job: the job that was acquired
+        :param scheduler_id: the ID of the scheduler that acquired the job
+        :return: a new job-acquired event
+
+        """
+        return cls(
+            job_id=job.id,
+            scheduler_id=scheduler_id,
+            task_id=job.task_id,
+            schedule_id=job.schedule_id,
+            scheduled_start=job.scheduled_fire_time,
+        )
 
 
 @attrs.define(kw_only=True, frozen=True)
 class JobReleased(SchedulerEvent):
     """
-    Signals that a worker has finished processing of a job.
+    Signals that a scheduler has finished processing of a job.
 
     :param uuid.UUID job_id: the ID of the job that was released
-    :param scheduler_id: the ID of the worker that released the job
+    :param scheduler_id: the ID of the scheduler that released the job
+    :param scheduled_start: the time the job was scheduled to start via a schedule (if
+        any)
+    :param started_at: the time the executor actually started running the job (``None``
+        if the job was skipped due to missing its start deadline)
     :param outcome: the outcome of the job
     :param exception_type: the fully qualified name of the exception if ``outcome`` is
         :attr:`JobOutcome.error`
     :param exception_message: the result of ``str(exception)`` if ``outcome`` is
         :attr:`JobOutcome.error`
     :param exception_traceback: the traceback lines from the exception if ``outcome`` is
         :attr:`JobOutcome.error`
     """
 
     job_id: UUID = attrs.field(converter=as_uuid)
     scheduler_id: str
+    task_id: str
+    schedule_id: str | None = None
+    scheduled_start: datetime | None = attrs.field(converter=as_aware_datetime)
+    started_at: datetime | None = attrs.field(converter=as_aware_datetime)
     outcome: JobOutcome = attrs.field(converter=as_enum(JobOutcome))
     exception_type: str | None = None
     exception_message: str | None = None
     exception_traceback: list[str] | None = None
 
     @classmethod
-    def from_result(cls, result: JobResult, worker_id: str) -> JobReleased:
+    def from_result(cls, job: Job, result: JobResult, scheduler_id: str) -> JobReleased:
+        """
+        Create a new job-released event from a job, the job result and a scheduler ID.
+
+        :param job: the job that was acquired
+        :param result: the result of the job
+        :param scheduler_id: the ID of the scheduler that acquired the job
+        :return: a new job-released event
+
+        """
         if result.exception is not None:
             exception_type: str | None = qualified_name(result.exception.__class__)
             exception_message: str | None = str(result.exception)
             exception_traceback: list[str] | None = format_tb(
                 result.exception.__traceback__
             )
         else:
             exception_type = exception_message = exception_traceback = None
 
         return cls(
+            timestamp=result.finished_at,
             job_id=result.job_id,
-            scheduler_id=worker_id,
+            scheduler_id=scheduler_id,
+            task_id=job.task_id,
+            schedule_id=job.schedule_id,
             outcome=result.outcome,
+            scheduled_start=job.scheduled_fire_time,
+            started_at=result.started_at,
             exception_type=exception_type,
             exception_message=exception_message,
             exception_traceback=exception_traceback,
         )
 
-    def marshal(self, serializer: abc.Serializer) -> dict[str, Any]:
-        marshalled = super().marshal(serializer)
+    def marshal(self) -> dict[str, Any]:
+        marshalled = super().marshal()
         return marshalled
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_exceptions.py` & `apscheduler-4.0.0a5/src/apscheduler/_exceptions.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_marshalling.py` & `apscheduler-4.0.0a5/src/apscheduler/_marshalling.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_retry.py` & `apscheduler-4.0.0a5/src/apscheduler/_retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         Tuple of exception classes which indicate that the operation should be retried.
 
         """
         return ()
 
     def _retry(self) -> AsyncRetrying:
-        def after_attempt(self, retry_state: RetryCallState) -> None:
+        def after_attempt(retry_state: RetryCallState) -> None:
             self._logger.warning(
                 "Temporary data store error (attempt %d): %s",
                 retry_state.attempt_number,
                 retry_state.outcome.exception(),
             )
 
         return AsyncRetrying(
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_schedulers/async_.py` & `apscheduler-4.0.0a5/src/apscheduler/_schedulers/async_.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,42 @@
 from collections.abc import MutableMapping, Sequence
 from contextlib import AsyncExitStack
 from datetime import datetime, timedelta, timezone
 from functools import partial
 from inspect import isbuiltin, isclass, ismethod, ismodule
 from logging import Logger, getLogger
 from types import TracebackType
-from typing import Any, Callable, Iterable, Mapping, cast
+from typing import Any, Callable, Iterable, Literal, Mapping, cast, overload
 from uuid import UUID, uuid4
 
 import anyio
 import attrs
 from anyio import (
     TASK_STATUS_IGNORED,
     CancelScope,
     create_task_group,
     get_cancelled_exc_class,
     move_on_after,
+    sleep,
 )
 from anyio.abc import TaskGroup, TaskStatus
-from attr.validators import instance_of
+from attr.validators import instance_of, optional
 
 from .. import JobAdded, SerializationError, TaskLookupError
 from .._context import current_async_scheduler, current_job
+from .._converters import as_enum, as_timedelta
 from .._enums import CoalescePolicy, ConflictPolicy, JobOutcome, RunState, SchedulerRole
 from .._events import (
     Event,
     JobReleased,
     ScheduleAdded,
     SchedulerStarted,
     SchedulerStopped,
     ScheduleUpdated,
+    T_Event,
 )
 from .._exceptions import (
     CallableLookupError,
     DeserializationError,
     JobCancelled,
     JobDeadlineMissed,
     JobLookupError,
@@ -73,35 +76,61 @@
 
 
 @attrs.define(eq=False)
 class AsyncScheduler:
     """
     An asynchronous (AnyIO based) scheduler implementation.
 
+    Requires either :mod:`asyncio` or Trio_ to work.
+
+    .. note:: If running on Trio, ensure that the data store and event broker are
+        compatible with Trio.
+
+    .. _AnyIO: https://pypi.org/project/anyio/
+    .. _Trio: https://pypi.org/project/trio/
+
     :param data_store: the data store for tasks, schedules and jobs
     :param event_broker: the event broker to use for publishing an subscribing events
-    :param max_concurrent_jobs: Maximum number of jobs the worker will run at once
-    :param role: specifies what the scheduler should be doing when running
+    :param identity: the unique identifier of the scheduler
+    :param role: specifies what the scheduler should be doing when running (scheduling
+        only, job running only, or both)
+    :param max_concurrent_jobs: Maximum number of jobs the scheduler will run at once
+    :param job_executors: a mutable mapping of executor names to executor instances
+    :param default_job_executor: name of the default job executor
+    :param cleanup_interval: interval (as seconds or timedelta) between automatic
+        calls to :meth:`cleanup` – ``None`` to disable automatic clean-up
+    :param logger: the logger instance used to log events from the scheduler, data store
+        and event broker
     """
 
     data_store: DataStore = attrs.field(
         validator=instance_of(DataStore), factory=MemoryDataStore
     )
     event_broker: EventBroker = attrs.field(
         validator=instance_of(EventBroker), factory=LocalEventBroker
     )
-    identity: str = attrs.field(kw_only=True, default=None)
-    role: SchedulerRole = attrs.field(kw_only=True, default=SchedulerRole.both)
+    identity: str = attrs.field(kw_only=True, validator=instance_of(str), default="")
+    role: SchedulerRole = attrs.field(
+        kw_only=True, converter=as_enum(SchedulerRole), default=SchedulerRole.both
+    )
     max_concurrent_jobs: int = attrs.field(
         kw_only=True, validator=non_negative_number, default=100
     )
     job_executors: MutableMapping[str, JobExecutor] = attrs.field(
-        kw_only=True, factory=dict
+        kw_only=True, validator=instance_of(MutableMapping), factory=dict
+    )
+    default_job_executor: str | None = attrs.field(
+        kw_only=True, validator=optional(instance_of(str)), default=None
+    )
+    cleanup_interval: timedelta | None = attrs.field(
+        kw_only=True,
+        converter=as_timedelta,
+        validator=optional(instance_of(timedelta)),
+        default=timedelta(minutes=15),
     )
-    default_job_executor: str | None = attrs.field(kw_only=True, default=None)
     logger: Logger = attrs.field(kw_only=True, default=getLogger(__name__))
 
     _state: RunState = attrs.field(init=False, default=RunState.stopped)
     _services_task_group: TaskGroup | None = attrs.field(init=False, default=None)
     _exit_stack: AsyncExitStack = attrs.field(init=False)
     _services_initialized: bool = attrs.field(init=False, default=False)
     _scheduler_cancel_scope: CancelScope | None = attrs.field(init=False, default=None)
@@ -137,17 +166,17 @@
             exit_stack.callback(setattr, self, "_services_task_group", None)
             self._exit_stack = exit_stack.pop_all()
 
         return self
 
     async def __aexit__(
         self,
-        exc_type: type[BaseException],
-        exc_val: BaseException,
-        exc_tb: TracebackType,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         await self.stop()
         await self._exit_stack.__aexit__(exc_type, exc_val, exc_tb)
 
     async def _ensure_services_initialized(self, exit_stack: AsyncExitStack) -> None:
         """
         Initialize the data store and event broker if this hasn't already been done.
@@ -165,23 +194,55 @@
         if not self._services_initialized:
             raise RuntimeError(
                 "The scheduler has not been initialized yet. Use the scheduler as an "
                 "async context manager (async with ...) in order to call methods other "
                 "than run_until_stopped()."
             )
 
+    async def _cleanup_loop(self) -> None:
+        delay = self.cleanup_interval.total_seconds()
+        assert delay > 0
+        while self._state in (RunState.starting, RunState.started):
+            await self.cleanup()
+            await sleep(delay)
+
     @property
     def state(self) -> RunState:
         """The current running state of the scheduler."""
         return self._state
 
+    async def cleanup(self) -> None:
+        """Clean up expired job results and finished schedules."""
+        await self.data_store.cleanup()
+        self.logger.info("Cleaned up expired job results and finished schedules")
+
+    @overload
+    def subscribe(
+        self,
+        callback: Callable[[T_Event], Any],
+        event_types: type[T_Event],
+        *,
+        one_shot: bool = ...,
+        is_async: bool = ...,
+    ) -> Subscription: ...
+
+    @overload
     def subscribe(
         self,
         callback: Callable[[Event], Any],
-        event_types: type[Event] | Iterable[type[Event]] | None = None,
+        event_types: Iterable[type[Event]] | None = None,
+        *,
+        one_shot: bool = False,
+        is_async: bool = True,
+    ) -> Subscription: ...
+
+    def subscribe(
+        self,
+        callback: Callable[[T_Event], Any],
+        event_types: type[T_Event] | Iterable[type[T_Event]] | None = None,
         *,
         one_shot: bool = False,
         is_async: bool = True,
     ) -> Subscription:
         """
         Subscribe to events.
 
@@ -345,14 +406,15 @@
         self,
         func_or_task_id: TaskType,
         trigger: Trigger,
         *,
         id: str | None = None,
         args: Iterable | None = None,
         kwargs: Mapping[str, Any] | None = None,
+        paused: bool = False,
         job_executor: str | UnsetValue = unset,
         coalesce: CoalescePolicy = CoalescePolicy.latest,
         misfire_grace_time: float | timedelta | None | UnsetValue = unset,
         max_jitter: float | timedelta | None = None,
         max_running_jobs: int | None | UnsetValue = unset,
         conflict_policy: ConflictPolicy = ConflictPolicy.do_nothing,
     ) -> str:
@@ -362,14 +424,15 @@
         :param func_or_task_id: either a callable or an ID of an existing task
             definition
         :param trigger: determines the times when the task should be run
         :param id: an explicit identifier for the schedule (if omitted, a random, UUID
             based ID will be assigned)
         :param args: positional arguments to be passed to the task function
         :param kwargs: keyword arguments to be passed to the task function
+        :param paused: whether the schedule is paused
         :param job_executor: name of the job executor to run the task with
         :param coalesce: determines what to do when processing the schedule if multiple
             fire times have become due for this schedule since the last processing
         :param misfire_grace_time: maximum number of seconds the scheduled job's actual
             run time is allowed to be late, compared to the scheduled run time
         :param max_jitter: maximum number of seconds to randomly add to the scheduled
             time for each job created from this schedule
@@ -391,47 +454,48 @@
             args = func_or_task_id.args + args
             kwargs.update(func_or_task_id.keywords)
             func_or_task_id = func_or_task_id.func
 
         # For instance methods, use the unbound function as the function, and  the
         # "self" argument as the first positional argument
         if ismethod(func_or_task_id):
-            args = (func_or_task_id.__self__,) + args
+            args = (func_or_task_id.__self__, *args)
             func_or_task_id = func_or_task_id.__func__
         elif (
             isbuiltin(func_or_task_id)
             and func_or_task_id.__self__ is not None
             and not ismodule(func_or_task_id.__self__)
         ):
-            args = (func_or_task_id.__self__,) + args
+            args = (func_or_task_id.__self__, *args)
             method_class = type(func_or_task_id.__self__)
             func_or_task_id = getattr(method_class, func_or_task_id.__name__)
 
         task = await self.configure_task(
             func_or_task_id,
             job_executor=job_executor,
             max_running_jobs=max_running_jobs,
         )
         schedule = Schedule(
             id=schedule_id,
             task_id=task.id,
             trigger=trigger,
             args=args,
             kwargs=kwargs,
+            paused=paused,
             coalesce=coalesce,
             misfire_grace_time=task.misfire_grace_time
             if misfire_grace_time is unset
             else misfire_grace_time,
             max_jitter=max_jitter,
         )
         schedule.next_fire_time = trigger.next()
         await self.data_store.add_schedule(schedule, conflict_policy)
         self.logger.info(
             "Added new schedule (task=%r, trigger=%r); next run time at %s",
-            task,
+            task.id,
             trigger,
             schedule.next_fire_time,
         )
         return schedule.id
 
     async def get_schedule(self, id: str) -> Schedule:
         """
@@ -464,14 +528,66 @@
 
         :param id: the unique identifier of the schedule
 
         """
         self._check_initialized()
         await self.data_store.remove_schedules({id})
 
+    async def pause_schedule(self, id: str) -> None:
+        """Pause the specified schedule."""
+        self._check_initialized()
+        await self.data_store.add_schedule(
+            schedule=attrs.evolve(await self.get_schedule(id), paused=True),
+            conflict_policy=ConflictPolicy.replace,
+        )
+
+    async def unpause_schedule(
+        self,
+        id: str,
+        *,
+        resume_from: datetime | Literal["now"] | None = None,
+    ) -> None:
+        """
+        Unpause the specified schedule.
+
+
+        :param resume_from: the time to resume the schedules from, or ``'now'`` as a
+            shorthand for ``datetime.now(tz=UTC)`` or ``None`` to resume from where the
+            schedule left off which may cause it to misfire
+
+        """
+        self._check_initialized()
+        schedule = await self.get_schedule(id)
+
+        if resume_from == "now":
+            resume_from = datetime.now(tz=timezone.utc)
+
+        if resume_from is None:
+            next_fire_time = schedule.next_fire_time
+        elif (
+            schedule.next_fire_time is not None
+            and schedule.next_fire_time >= resume_from
+        ):
+            next_fire_time = schedule.next_fire_time
+        else:
+            # Advance `next_fire_time` until its at or past `resume_from`, or until it's
+            # exhausted
+            while next_fire_time := schedule.trigger.next():
+                if next_fire_time is None or next_fire_time >= resume_from:
+                    break
+
+        await self.data_store.add_schedule(
+            schedule=attrs.evolve(
+                schedule,
+                paused=False,
+                next_fire_time=next_fire_time,
+            ),
+            conflict_policy=ConflictPolicy.replace,
+        )
+
     async def add_job(
         self,
         func_or_task_id: TaskType,
         *,
         args: Iterable | None = None,
         kwargs: Mapping[str, Any] | None = None,
         job_executor: str | None | UnsetValue = unset,
@@ -480,18 +596,17 @@
         """
         Add a job to the data store.
 
         :param func_or_task_id:
             Either the ID of a pre-existing task, or a function/method. If a function is
             given, a task will be created with the fully qualified name of the function
             as the task ID (unless that task already exists of course).
-        :param job_executor: name of the job executor to run the job with
         :param args: positional arguments to call the target callable with
         :param kwargs: keyword arguments to call the target callable with
-        :param job_executor: name of the job executor to run the task with
+        :param job_executor: name of the job executor to run the job with
         :param result_expiration_time: the minimum time (as seconds, or timedelta) to
             keep the result of the job available for fetching (the result won't be
             saved at all if that time is 0)
         :return: the ID of the newly created job
 
         """
         self._check_initialized()
@@ -503,22 +618,22 @@
             args = func_or_task_id.args + args
             kwargs.update(func_or_task_id.keywords)
             func_or_task_id = func_or_task_id.func
 
         # For instance methods, use the unbound function as the function, and  the
         # "self" argument as the first positional argument
         if ismethod(func_or_task_id):
-            args = (func_or_task_id.__self__,) + args
+            args = (func_or_task_id.__self__, *args)
             func_or_task_id = func_or_task_id.__func__
         elif (
             isbuiltin(func_or_task_id)
             and func_or_task_id.__self__ is not None
             and not ismodule(func_or_task_id.__self__)
         ):
-            args = (func_or_task_id.__self__,) + args
+            args = (func_or_task_id.__self__, *args)
             method_class = type(func_or_task_id.__self__)
             func_or_task_id = getattr(method_class, func_or_task_id.__name__)
 
         task = await self.configure_task(func_or_task_id, job_executor=job_executor)
         job = Job(
             task_id=task.id,
             args=args or (),
@@ -536,33 +651,35 @@
     async def get_job_result(self, job_id: UUID, *, wait: bool = True) -> JobResult:
         """
         Retrieve the result of a job.
 
         :param job_id: the ID of the job
         :param wait: if ``True``, wait until the job has ended (one way or another),
             ``False`` to raise an exception if the result is not yet available
-        :raises JobLookupError: if ``wait=False`` and the job result does not exist in
-            the data store
+        :raises JobLookupError: if neither the job or its result exist in the data
+            store, or the job exists but the result is not ready yet and ``wait=False``
+            is set
 
         """
         self._check_initialized()
         wait_event = anyio.Event()
 
         def listener(event: JobReleased) -> None:
             if event.job_id == job_id:
                 wait_event.set()
 
         with self.event_broker.subscribe(listener, {JobReleased}):
-            result = await self.data_store.get_job_result(job_id)
-            if result:
+            job_exists = bool(await self.data_store.get_jobs([job_id]))
+            if result := await self.data_store.get_job_result(job_id):
                 return result
-            elif not wait:
-                raise JobLookupError(job_id)
 
-            await wait_event.wait()
+            if job_exists and wait:
+                await wait_event.wait()
+            else:
+                raise JobLookupError(job_id)
 
         return await self.data_store.get_job_result(job_id)
 
     async def run_job(
         self,
         func_or_task_id: str | Callable,
         *,
@@ -664,14 +781,22 @@
 
             exception: BaseException | None = None
             try:
                 async with create_task_group() as task_group:
                     self._scheduler_cancel_scope = task_group.cancel_scope
                     exit_stack.callback(setattr, self, "_scheduler_cancel_scope", None)
 
+                    # Start periodic cleanups
+                    if self.cleanup_interval:
+                        task_group.start_soon(self._cleanup_loop)
+                        self.logger.debug(
+                            "Started internal cleanup loop with interval: %s",
+                            self.cleanup_interval,
+                        )
+
                     # Start processing due schedules, if configured to do so
                     if self.role in (SchedulerRole.scheduler, SchedulerRole.both):
                         await task_group.start(self._process_schedules)
 
                     # Start processing due jobs, if configured to do so
                     if self.role in (SchedulerRole.worker, SchedulerRole.both):
                         await task_group.start(self._process_jobs)
@@ -852,27 +977,31 @@
                 f"scheduler.configure_task({task.id!r}, func=...) to define the local "
                 f"callable."
             )
 
     async def _process_jobs(self, *, task_status: TaskStatus) -> None:
         wakeup_event = anyio.Event()
 
-        async def job_added(event: Event) -> None:
+        async def check_queue_capacity(event: Event) -> None:
             if len(self._running_jobs) < self.max_concurrent_jobs:
                 wakeup_event.set()
 
         async with AsyncExitStack() as exit_stack:
             # Start the job executors
             for job_executor in self.job_executors.values():
                 await job_executor.start(exit_stack)
 
             task_group = await exit_stack.enter_async_context(create_task_group())
 
             # Fetch new jobs every time
-            exit_stack.enter_context(self.event_broker.subscribe(job_added, {JobAdded}))
+            exit_stack.enter_context(
+                self.event_broker.subscribe(
+                    check_queue_capacity, {JobAdded, JobReleased}
+                )
+            )
 
             # Signal that we are ready, and wait for the scheduler start event
             task_status.started()
             await self.get_next_event(SchedulerStarted)
 
             while self._state is RunState.started:
                 limit = self.max_concurrent_jobs - len(self._running_jobs)
@@ -891,76 +1020,57 @@
 
     async def _run_job(self, job: Job, func: Callable, executor: str) -> None:
         try:
             # Check if the job started before the deadline
             start_time = datetime.now(timezone.utc)
             if job.start_deadline is not None and start_time > job.start_deadline:
                 result = JobResult.from_job(
-                    job,
-                    outcome=JobOutcome.missed_start_deadline,
-                    finished_at=start_time,
-                )
-                await self.data_store.release_job(self.identity, job.task_id, result)
-                await self.event_broker.publish(
-                    JobReleased.from_result(result, self.identity)
+                    job, JobOutcome.missed_start_deadline, finished_at=start_time
                 )
+                await self.data_store.release_job(self.identity, job, result)
                 return
 
             try:
                 job_executor = self.job_executors[executor]
             except KeyError:
                 return
 
             token = current_job.set(job)
             try:
                 retval = await job_executor.run_job(func, job)
             except get_cancelled_exc_class():
                 self.logger.info("Job %s was cancelled", job.id)
                 with CancelScope(shield=True):
                     result = JobResult.from_job(
-                        job,
-                        outcome=JobOutcome.cancelled,
-                    )
-                    await self.data_store.release_job(
-                        self.identity, job.task_id, result
-                    )
-                    await self.event_broker.publish(
-                        JobReleased.from_result(result, self.identity)
+                        job, JobOutcome.cancelled, started_at=start_time
                     )
+                    await self.data_store.release_job(self.identity, job, result)
             except BaseException as exc:
                 if isinstance(exc, Exception):
                     self.logger.exception("Job %s raised an exception", job.id)
                 else:
                     self.logger.error(
                         "Job %s was aborted due to %s", job.id, exc.__class__.__name__
                     )
 
                 result = JobResult.from_job(
                     job,
                     JobOutcome.error,
+                    started_at=start_time,
                     exception=exc,
                 )
-                await self.data_store.release_job(
-                    self.identity,
-                    job.task_id,
-                    result,
-                )
-                await self.event_broker.publish(
-                    JobReleased.from_result(result, self.identity)
-                )
+                await self.data_store.release_job(self.identity, job, result)
                 if not isinstance(exc, Exception):
                     raise
             else:
                 self.logger.info("Job %s completed successfully", job.id)
                 result = JobResult.from_job(
                     job,
                     JobOutcome.success,
+                    started_at=start_time,
                     return_value=retval,
                 )
-                await self.data_store.release_job(self.identity, job.task_id, result)
-                await self.event_broker.publish(
-                    JobReleased.from_result(result, self.identity)
-                )
+                await self.data_store.release_job(self.identity, job, result)
             finally:
                 current_job.reset(token)
         finally:
             self._running_jobs.remove(job.id)
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_schedulers/sync.py` & `apscheduler-4.0.0a5/src/apscheduler/_schedulers/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,63 +2,78 @@
 
 import atexit
 import logging
 import sys
 import threading
 from collections.abc import MutableMapping, Sequence
 from contextlib import ExitStack
-from datetime import timedelta
+from datetime import datetime, timedelta
 from functools import partial
 from logging import Logger
 from types import TracebackType
-from typing import Any, Callable, Iterable, Mapping
+from typing import Any, Callable, Iterable, Literal, Mapping, overload
 from uuid import UUID
 
 from anyio.from_thread import BlockingPortal, start_blocking_portal
 
-from .. import Event, current_scheduler
+from .. import current_scheduler
 from .._enums import CoalescePolicy, ConflictPolicy, RunState, SchedulerRole
+from .._events import Event, T_Event
 from .._structures import Job, JobResult, Schedule, Task
 from .._utils import UnsetValue, unset
 from ..abc import DataStore, EventBroker, JobExecutor, Subscription, Trigger
 from .async_ import AsyncScheduler, TaskType
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 
 class Scheduler:
-    """A synchronous scheduler implementation."""
+    """
+    A synchronous wrapper for :class:`AsyncScheduler`.
+
+    When started, this wrapper launches an asynchronous event loop in a separate thread
+    and runs the asynchronous scheduler there. This thread is shut down along with the
+    scheduler.
+
+    See the documentation of the :class:`AsyncScheduler` class for the documentation of
+    the configuration options.
+    """
 
     def __init__(
         self,
         data_store: DataStore | None = None,
         event_broker: EventBroker | None = None,
         *,
-        identity: str | None = None,
+        identity: str = "",
         role: SchedulerRole = SchedulerRole.both,
+        max_concurrent_jobs: int = 100,
+        cleanup_interval: float | timedelta | None = None,
         job_executors: MutableMapping[str, JobExecutor] | None = None,
         default_job_executor: str | None = None,
         logger: Logger | None = None,
     ):
         kwargs: dict[str, Any] = {}
         if data_store is not None:
             kwargs["data_store"] = data_store
+
         if event_broker is not None:
             kwargs["event_broker"] = event_broker
 
         if not default_job_executor and not job_executors:
             default_job_executor = "threadpool"
 
         self._async_scheduler = AsyncScheduler(
             identity=identity,
             role=role,
-            job_executors=job_executors,
+            max_concurrent_jobs=max_concurrent_jobs,
+            job_executors=job_executors or {},
+            cleanup_interval=cleanup_interval,
             default_job_executor=default_job_executor,
             logger=logger or logging.getLogger(__name__),
             **kwargs,
         )
         self._exit_stack = ExitStack()
         self._portal: BlockingPortal | None = None
         self._lock = threading.RLock()
@@ -76,14 +91,22 @@
         return self._async_scheduler.identity
 
     @property
     def role(self) -> SchedulerRole:
         return self._async_scheduler.role
 
     @property
+    def max_concurrent_jobs(self) -> int:
+        return self._async_scheduler.max_concurrent_jobs
+
+    @property
+    def cleanup_interval(self) -> timedelta:
+        return self._async_scheduler.cleanup_interval
+
+    @property
     def job_executors(self) -> MutableMapping[str, JobExecutor]:
         return self._async_scheduler.job_executors
 
     @property
     def default_job_executor(self) -> str:
         return self._async_scheduler.default_job_executor
 
@@ -98,17 +121,17 @@
 
     def __enter__(self: Self) -> Self:
         self._ensure_services_ready(self._exit_stack)
         return self
 
     def __exit__(
         self,
-        exc_type: type[BaseException],
-        exc_val: BaseException,
-        exc_tb: TracebackType,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         if self._exit_stack:
             self._exit_stack.__exit__(exc_type, exc_val, exc_tb)
 
     def _ensure_services_ready(self, exit_stack: ExitStack | None = None) -> None:
         """Ensure that the underlying asynchronous scheduler has been initialized."""
         with self._lock:
@@ -125,20 +148,42 @@
 
                 self._portal = exit_stack.enter_context(start_blocking_portal())
                 exit_stack.callback(setattr, self, "_portal", None)
                 exit_stack.enter_context(
                     self._portal.wrap_async_context_manager(self._async_scheduler)
                 )
 
+    def cleanup(self) -> None:
+        self._ensure_services_ready()
+        return self._portal.call(self._async_scheduler.cleanup)
+
+    @overload
+    def subscribe(
+        self,
+        callback: Callable[[T_Event], Any],
+        event_types: type[T_Event],
+        *,
+        one_shot: bool = ...,
+    ) -> Subscription: ...
+
+    @overload
     def subscribe(
         self,
         callback: Callable[[Event], Any],
         event_types: Iterable[type[Event]] | None = None,
         *,
         one_shot: bool = False,
+    ) -> Subscription: ...
+
+    def subscribe(
+        self,
+        callback: Callable[[T_Event], Any],
+        event_types: type[T_Event] | Iterable[type[T_Event]] | None = None,
+        *,
+        one_shot: bool = False,
     ) -> Subscription:
         """
         Subscribe to events.
 
         To unsubscribe, call the :meth:`~abc.Subscription.unsubscribe` method on the
         returned object.
 
@@ -189,14 +234,15 @@
         self,
         func_or_task_id: TaskType,
         trigger: Trigger,
         *,
         id: str | None = None,
         args: Iterable | None = None,
         kwargs: Mapping[str, Any] | None = None,
+        paused: bool = False,
         job_executor: str | UnsetValue = unset,
         coalesce: CoalescePolicy = CoalescePolicy.latest,
         misfire_grace_time: float | timedelta | None | UnsetValue = unset,
         max_jitter: float | timedelta | None = None,
         max_running_jobs: int | None | UnsetValue = unset,
         conflict_policy: ConflictPolicy = ConflictPolicy.do_nothing,
     ) -> str:
@@ -205,14 +251,15 @@
             partial(
                 self._async_scheduler.add_schedule,
                 func_or_task_id,
                 trigger,
                 id=id,
                 args=args,
                 kwargs=kwargs,
+                paused=paused,
                 job_executor=job_executor,
                 coalesce=coalesce,
                 misfire_grace_time=misfire_grace_time,
                 max_jitter=max_jitter,
                 max_running_jobs=max_running_jobs,
                 conflict_policy=conflict_policy,
             )
@@ -226,14 +273,33 @@
         self._ensure_services_ready()
         return self._portal.call(self._async_scheduler.get_schedules)
 
     def remove_schedule(self, id: str) -> None:
         self._ensure_services_ready()
         self._portal.call(self._async_scheduler.remove_schedule, id)
 
+    def pause_schedule(self, id: str) -> None:
+        self._ensure_services_ready()
+        self._portal.call(self._async_scheduler.pause_schedule, id)
+
+    def unpause_schedule(
+        self,
+        id: str,
+        *,
+        resume_from: datetime | Literal["now"] | None = None,
+    ) -> None:
+        self._ensure_services_ready()
+        self._portal.call(
+            partial(
+                self._async_scheduler.unpause_schedule,
+                id,
+                resume_from=resume_from,
+            )
+        )
+
     def add_job(
         self,
         func_or_task_id: TaskType,
         *,
         args: Iterable | None = None,
         kwargs: Mapping[str, Any] | None = None,
         job_executor: str | UnsetValue = unset,
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/_structures.py` & `apscheduler-4.0.0a5/src/apscheduler/_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     """
     Represents a schedule on which a task will be run.
 
     :var str id: the unique identifier of this schedule
     :var str task_id: unique identifier of the task to be run on this schedule
     :var tuple args: positional arguments to pass to the task callable
     :var dict[str, Any] kwargs: keyword arguments to pass to the task callable
+    :var bool paused: whether the schedule is paused
     :var CoalescePolicy coalesce: determines what to do when processing the schedule if
         multiple fire times have become due for this schedule since the last processing
     :var ~datetime.timedelta | None misfire_grace_time: maximum number of seconds the
         scheduled job's actual run time is allowed to be late, compared to the scheduled
         run time
     :var ~datetime.timedelta | None max_jitter: maximum number of seconds to randomly
         add to the scheduled time for each job created from this schedule
@@ -101,14 +102,15 @@
         order=False,
         validator=instance_of(Trigger),  # type: ignore[type-abstract]
     )
     args: tuple = attrs.field(eq=False, order=False, converter=tuple, default=())
     kwargs: dict[str, Any] = attrs.field(
         eq=False, order=False, converter=dict, default=()
     )
+    paused: bool = attrs.field(eq=False, order=False, default=False)
     coalesce: CoalescePolicy = attrs.field(
         eq=False,
         order=False,
         default=CoalescePolicy.latest,
         converter=as_enum(CoalescePolicy),
         validator=instance_of(CoalescePolicy),
     )
@@ -167,24 +169,24 @@
     :var dict[str, Any] kwargs: keyword arguments to pass to the task callable
     :var str schedule_id: unique identifier of the associated schedule
         (if the job was derived from a schedule)
     :var ~datetime.datetime | None scheduled_fire_time: the time the job was scheduled
         to run at (if the job was derived from a schedule; includes jitter)
     :var ~datetime.timedelta | None jitter: the time that was randomly added to the
         calculated scheduled run time (if the job was derived from a schedule)
-    :var ~datetime.datetime | None start_deadline: if the job is started in the worker
-        after this time, it is considered to be misfired and will be aborted
+    :var ~datetime.datetime | None start_deadline: if the job is started in the
+        scheduler after this time, it is considered to be misfired and will be aborted
     :var ~datetime.timedelta result_expiration_time: minimum amount of time to keep the
         result available for fetching in the data store
     :var ~datetime.datetime created_at: the time at which the job was created
     :var ~datetime.datetime | None started_at: the time at which the execution of the
         job was started
-    :var str | None acquired_by: the unique identifier of the worker that has acquired
-        the job for execution
-    :var str | None acquired_until: the time after which other workers are free to
+    :var str | None acquired_by: the unique identifier of the scheduler that has
+        acquired the job for execution
+    :var str | None acquired_until: the time after which other schedulers are free to
         acquire the job for processing even if it is still marked as acquired
     """
 
     id: UUID = attrs.field(factory=uuid4)
     task_id: str = attrs.field(eq=False, order=False)
     args: tuple = attrs.field(eq=False, order=False, converter=tuple, default=())
     kwargs: dict[str, Any] = attrs.field(
@@ -205,17 +207,14 @@
     )
     created_at: datetime = attrs.field(
         eq=False,
         order=False,
         converter=as_aware_datetime,
         factory=partial(datetime.now, timezone.utc),
     )
-    started_at: datetime | None = attrs.field(
-        eq=False, order=False, converter=as_aware_datetime, default=None
-    )
     acquired_by: str | None = attrs.field(eq=False, order=False, default=None)
     acquired_until: datetime | None = attrs.field(
         eq=False, order=False, converter=as_aware_datetime, default=None
     )
 
     @property
     def original_scheduled_time(self) -> datetime | None:
@@ -245,52 +244,61 @@
 @attrs.define(kw_only=True, frozen=True)
 class JobResult:
     """
     Represents the result of running a job.
 
     :var ~uuid.UUID job_id: the unique identifier of the job
     :var JobOutcome outcome: indicates how the job ended
-    :var ~datetime.datetime finished_at: the time when the job ended
+    :var ~datetime.datetime started_at: the time when the job was submitted to the
+        executor (``None`` if the job never started in the first place)
+    :var ~datetime.datetime finished_at: the time when the job ended (``None`` if the
+        job never started in the first place)
     :var BaseException | None exception: the exception object if the job ended due to an
         exception being raised
     :var return_value: the return value from the task function (if the job ran to
         completion successfully)
     """
 
     job_id: UUID
     outcome: JobOutcome = attrs.field(
         eq=False, order=False, converter=as_enum(JobOutcome)
     )
+    started_at: datetime | None = attrs.field(
+        eq=False,
+        order=False,
+        converter=as_aware_datetime,
+    )
     finished_at: datetime = attrs.field(
         eq=False,
         order=False,
         converter=as_aware_datetime,
-        factory=partial(datetime.now, timezone.utc),
     )
     expires_at: datetime = attrs.field(
         eq=False, converter=as_aware_datetime, order=False
     )
     exception: BaseException | None = attrs.field(eq=False, order=False, default=None)
     return_value: Any = attrs.field(eq=False, order=False, default=None)
 
     @classmethod
     def from_job(
         cls,
         job: Job,
         outcome: JobOutcome,
         *,
         finished_at: datetime | None = None,
+        started_at: datetime | None = None,
         exception: BaseException | None = None,
         return_value: Any = None,
     ) -> JobResult:
         real_finished_at = finished_at or datetime.now(timezone.utc)
         expires_at = real_finished_at + job.result_expiration_time
         return cls(
             job_id=job.id,
             outcome=outcome,
+            started_at=started_at,
             finished_at=real_finished_at,
             expires_at=expires_at,
             exception=exception,
             return_value=return_value,
         )
 
     def marshal(self, serializer: Serializer) -> dict[str, Any]:
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/abc.py` & `apscheduler-4.0.0a5/src/apscheduler/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
 if TYPE_CHECKING:
     from ._enums import ConflictPolicy
-    from ._events import Event
+    from ._events import Event, T_Event
     from ._structures import Job, JobResult, Schedule, Task
 
 
 class Trigger(Iterator[datetime], metaclass=ABCMeta):
     """
     Abstract base class that defines the interface that every trigger must implement.
     """
@@ -131,16 +131,16 @@
     @abstractmethod
     async def publish_local(self, event: Event) -> None:
         """Publish an event, but only to local subscribers."""
 
     @abstractmethod
     def subscribe(
         self,
-        callback: Callable[[Event], Any],
-        event_types: Iterable[type[Event]] | None = None,
+        callback: Callable[[T_Event], Any],
+        event_types: Iterable[type[T_Event]] | None = None,
         *,
         is_async: bool = True,
         one_shot: bool = False,
     ) -> Subscription:
         """
         Subscribe to events from this event broker.
 
@@ -306,36 +306,41 @@
 
         :param scheduler_id: unique identifier of the scheduler
         :param limit: maximum number of jobs to claim and return
         :return: the list of claimed jobs
         """
 
     @abstractmethod
-    async def release_job(
-        self, scheduler_id: str, task_id: str, result: JobResult
-    ) -> None:
+    async def release_job(self, scheduler_id: str, job: Job, result: JobResult) -> None:
         """
         Release the claim on the given job and record the result.
 
         :param scheduler_id: unique identifier of the scheduler
-        :param task_id: the job's task ID
+        :param job: the job to be released
         :param result: the result of the job
         """
 
     @abstractmethod
     async def get_job_result(self, job_id: UUID) -> JobResult | None:
         """
         Retrieve the result of a job.
 
         The result is removed from the store after retrieval.
 
         :param job_id: the identifier of the job
         :return: the result, or ``None`` if the result was not found
         """
 
+    @abstractmethod
+    async def cleanup(self) -> None:
+        """
+        Purge expired job results and finished schedules that have no running jobs
+        associated with them.
+        """
+
 
 class JobExecutor(metaclass=ABCMeta):
     async def start(self, exit_stack: AsyncExitStack) -> None:
         """
         Start the job executor.
 
         :param exit_stack: an asynchronous exit stack which will be processed when the
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/datastores/base.py` & `apscheduler-4.0.0a5/src/apscheduler/datastores/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @attrs.define(kw_only=True)
 class BaseDataStore(DataStore):
     """
     Base class for data stores.
 
     :param lock_expiration_delay: maximum amount of time (in seconds) that a scheduler
-        or worker can keep a lock on a schedule or task
+        can keep a lock on a schedule or task
     """
 
     lock_expiration_delay: float = 30
     _event_broker: EventBroker = attrs.field(init=False)
     _logger: Logger = attrs.field(init=False)
 
     async def start(
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/datastores/memory.py` & `apscheduler-4.0.0a5/src/apscheduler/datastores/memory.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import attrs
 
 from .._enums import ConflictPolicy
 from .._events import (
     JobAcquired,
     JobAdded,
+    JobReleased,
     ScheduleAdded,
     ScheduleRemoved,
     ScheduleUpdated,
     TaskAdded,
     TaskRemoved,
     TaskUpdated,
 )
@@ -100,14 +101,17 @@
         partial(defaultdict, set)
     )
     _jobs: list[JobState] = attrs.Factory(list)
     _jobs_by_id: dict[UUID, JobState] = attrs.Factory(dict)
     _jobs_by_task_id: dict[str, set[JobState]] = attrs.Factory(
         partial(defaultdict, set)
     )
+    _jobs_by_schedule_id: dict[str, set[JobState]] = attrs.Factory(
+        partial(defaultdict, set)
+    )
     _job_results: dict[UUID, JobResult] = attrs.Factory(dict)
 
     def _find_schedule_index(self, state: ScheduleState) -> int | None:
         left_index = bisect_left(self._schedules, state)
         right_index = bisect_right(self._schedules, state)
         return self._schedules.index(state, left_index, right_index + 1)
 
@@ -199,16 +203,20 @@
                 await self._event_broker.publish(event)
 
     async def acquire_schedules(self, scheduler_id: str, limit: int) -> list[Schedule]:
         now = datetime.now(timezone.utc)
         schedules: list[Schedule] = []
         for state in self._schedules:
             if state.next_fire_time is None or state.next_fire_time > now:
-                # The schedule is either paused or not yet due
+                # The schedule is either exhausted or not yet due. There will be no
+                # schedules that are due after this one, so we can stop here.
                 break
+            elif state.schedule.paused:
+                # The schedule is paused
+                continue
             elif state.acquired_by is not None:
                 if state.acquired_by != scheduler_id and now <= state.acquired_until:
                     # The schedule has been acquired by another scheduler and the
                     # timeout has not expired yet
                     continue
 
             schedules.append(state.schedule)
@@ -218,61 +226,58 @@
                 break
 
         return schedules
 
     async def release_schedules(
         self, scheduler_id: str, schedules: list[Schedule]
     ) -> None:
-        # Send update events for schedules that have a next time
-        finished_schedule_ids: list[str] = []
+        # Send update events for schedules
         for s in schedules:
-            if s.next_fire_time is not None:
-                # Remove the schedule
-                schedule_state = self._schedules_by_id.get(s.id)
-                index = self._find_schedule_index(schedule_state)
-                del self._schedules[index]
-
-                # Re-add the schedule to its new position
-                schedule_state.next_fire_time = s.next_fire_time
-                schedule_state.acquired_by = None
-                schedule_state.acquired_until = None
-                insort_right(self._schedules, schedule_state)
-                event = ScheduleUpdated(
-                    schedule_id=s.id, task_id=s.task_id, next_fire_time=s.next_fire_time
-                )
-                await self._event_broker.publish(event)
-            else:
-                finished_schedule_ids.append(s.id)
+            # Remove the schedule
+            schedule_state = self._schedules_by_id.get(s.id)
+            index = self._find_schedule_index(schedule_state)
+            del self._schedules[index]
 
-        # Remove schedules that didn't get a new next fire time
-        await self.remove_schedules(finished_schedule_ids, finished=True)
+            # Re-add the schedule to its new position
+            schedule_state.next_fire_time = s.next_fire_time
+            schedule_state.acquired_by = None
+            schedule_state.acquired_until = None
+            insort_right(self._schedules, schedule_state)
+            event = ScheduleUpdated(
+                schedule_id=s.id, task_id=s.task_id, next_fire_time=s.next_fire_time
+            )
+            await self._event_broker.publish(event)
 
     async def get_next_schedule_run_time(self) -> datetime | None:
         return self._schedules[0].next_fire_time if self._schedules else None
 
     async def add_job(self, job: Job) -> None:
         state = JobState(job)
         self._jobs.append(state)
         self._jobs_by_id[job.id] = state
         self._jobs_by_task_id[job.task_id].add(state)
+        if job.schedule_id is not None:
+            self._jobs_by_schedule_id[job.schedule_id].add(state)
 
         event = JobAdded(
             job_id=job.id,
             task_id=job.task_id,
             schedule_id=job.schedule_id,
         )
         await self._event_broker.publish(event)
 
     async def get_jobs(self, ids: Iterable[UUID] | None = None) -> list[Job]:
         if ids is not None:
             ids = frozenset(ids)
 
         return [state.job for state in self._jobs if ids is None or state.job.id in ids]
 
-    async def acquire_jobs(self, worker_id: str, limit: int | None = None) -> list[Job]:
+    async def acquire_jobs(
+        self, scheduler_id: str, limit: int | None = None
+    ) -> list[Job]:
         now = datetime.now(timezone.utc)
         jobs: list[Job] = []
         for _index, job_state in enumerate(self._jobs):
             task_state = self._tasks[job_state.job.task_id]
 
             # Skip already acquired jobs (unless the acquisition lock has expired)
             if job_state.acquired_by is not None:
@@ -286,47 +291,84 @@
                 task_state.task.max_running_jobs is not None
                 and task_state.running_jobs >= task_state.task.max_running_jobs
             ):
                 continue
 
             # Mark the job as acquired by this worker
             jobs.append(job_state.job)
-            job_state.acquired_by = worker_id
+            job_state.acquired_by = scheduler_id
             job_state.acquired_until = now + timedelta(
                 seconds=self.lock_expiration_delay
             )
 
             # Increment the number of running jobs for this task
             task_state.running_jobs += 1
 
             # Exit the loop if enough jobs have been acquired
             if len(jobs) == limit:
                 break
 
         # Publish the appropriate events
         for job in jobs:
             await self._event_broker.publish(
-                JobAcquired(job_id=job.id, scheduler_id=worker_id)
+                JobAcquired.from_job(job, scheduler_id=scheduler_id)
             )
 
         return jobs
 
-    async def release_job(
-        self, worker_id: str, task_id: str, result: JobResult
-    ) -> None:
+    async def release_job(self, scheduler_id: str, job: Job, result: JobResult) -> None:
         # Record the job result
         if result.expires_at > result.finished_at:
             self._job_results[result.job_id] = result
 
         # Decrement the number of running jobs for this task
-        task_state = self._tasks.get(task_id)
+        task_state = self._tasks.get(job.task_id)
         if task_state is not None:
             task_state.running_jobs -= 1
 
         # Delete the job
         job_state = self._jobs_by_id.pop(result.job_id)
-        self._jobs_by_task_id[task_id].remove(job_state)
+
+        # Remove the job from the jobs belonging to its task
+        task_jobs = self._jobs_by_task_id[job.task_id]
+        task_jobs.remove(job_state)
+        if not task_jobs:
+            del self._jobs_by_task_id[job.task_id]
+
+        # If this was a scheduled job, remove the job from the set of jobs belonging to
+        # this schedule
+        if job.schedule_id:
+            schedule_jobs = self._jobs_by_schedule_id[job.schedule_id]
+            schedule_jobs.remove(job_state)
+            if not schedule_jobs:
+                del self._jobs_by_schedule_id[job.schedule_id]
+
         index = self._find_job_index(job_state)
         del self._jobs[index]
 
+        # Notify other schedulers
+        await self._event_broker.publish(
+            JobReleased.from_result(job, result, scheduler_id)
+        )
+
     async def get_job_result(self, job_id: UUID) -> JobResult | None:
         return self._job_results.pop(job_id, None)
+
+    async def cleanup(self) -> None:
+        # Clean up expired job results
+        now = datetime.now(timezone.utc)
+        expired_job_ids = [
+            result.job_id
+            for result in self._job_results.values()
+            if result.expires_at <= now
+        ]
+        for job_id in expired_job_ids:
+            del self._job_results[job_id]
+
+        # Clean up finished schedules that have no running jobs
+        finished_schedule_ids = [
+            schedule_id
+            for schedule_id, state in self._schedules_by_id.items()
+            if state.next_fire_time is None
+            and schedule_id not in self._jobs_by_schedule_id
+        ]
+        await self.remove_schedules(finished_schedule_ids, finished=True)
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/datastores/mongodb.py` & `apscheduler-4.0.0a5/src/apscheduler/datastores/mongodb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
 
 import operator
+import sys
 from collections import defaultdict
-from collections.abc import Mapping
+from collections.abc import AsyncIterator
 from contextlib import AsyncExitStack
 from datetime import datetime, timedelta, timezone
 from logging import Logger
-from typing import Any, Callable, ClassVar, Iterable
+from typing import Any, Callable, ClassVar, Generic, Iterable, Mapping, TypeVar
 from uuid import UUID
 
 import attrs
 import pymongo
 from anyio import to_thread
 from attrs.validators import instance_of
 from bson import CodecOptions, UuidRepresentation
 from bson.codec_options import TypeEncoder, TypeRegistry
 from pymongo import ASCENDING, DeleteOne, MongoClient, UpdateOne
 from pymongo.collection import Collection
+from pymongo.cursor import Cursor
 from pymongo.errors import ConnectionFailure, DuplicateKeyError
 
 from .._enums import CoalescePolicy, ConflictPolicy, JobOutcome
 from .._events import (
     DataStoreEvent,
     JobAcquired,
     JobAdded,
+    JobReleased,
     ScheduleAdded,
     ScheduleRemoved,
     ScheduleUpdated,
     TaskAdded,
     TaskRemoved,
     TaskUpdated,
 )
@@ -37,29 +40,39 @@
     SerializationError,
     TaskLookupError,
 )
 from .._structures import Job, JobResult, Schedule, Task
 from ..abc import EventBroker
 from .base import BaseExternalDataStore
 
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+T = TypeVar("T", bound=Mapping[str, Any])
+
 
 class CustomEncoder(TypeEncoder):
     def __init__(self, python_type: type, encoder: Callable):
         self._python_type = python_type
         self._encoder = encoder
 
     @property
     def python_type(self) -> type:
         return self._python_type
 
     def transform_python(self, value: Any) -> Any:
         return self._encoder(value)
 
 
-def marshal_timestamp(timestamp: datetime, key: str) -> Mapping[str, Any]:
+def marshal_timestamp(timestamp: datetime | None, key: str) -> Mapping[str, Any]:
+    if timestamp is None:
+        return {key: None, key + "_utcoffset": None}
+
     return {
         key: timestamp.timestamp(),
         key + "_utcoffset": timestamp.utcoffset().total_seconds() // 60,
     }
 
 
 def marshal_document(document: dict[str, Any]) -> None:
@@ -69,43 +82,87 @@
     for key, value in list(document.items()):
         if isinstance(value, datetime):
             document.update(marshal_timestamp(document[key], key))
 
 
 def unmarshal_timestamps(document: dict[str, Any]) -> None:
     for key in list(document):
-        if key.endswith("_utcoffset"):
-            offset = timedelta(seconds=document.pop(key) * 60)
+        if key.endswith("_utcoffset") and (value := document.pop(key)) is not None:
+            offset = timedelta(seconds=value * 60)
             tzinfo = timezone(offset)
             time_micro = document[key[:-10]]
             document[key[:-10]] = datetime.fromtimestamp(time_micro, tzinfo)
 
 
+class AsyncCursor(Generic[T]):
+    sentinel: ClassVar[object] = object()
+
+    def __init__(self, cursor: Cursor[T]):
+        self._cursor = cursor
+
+    def __aiter__(self) -> AsyncIterator[T]:
+        return self
+
+    async def __aenter__(self) -> Self:
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+        await to_thread.run_sync(self._cursor.close)
+
+    def _get_next(self) -> T:
+        try:
+            return next(self._cursor)
+        except StopIteration:
+            return self.sentinel
+
+    async def __anext__(self) -> T:
+        obj = await to_thread.run_sync(self._get_next)
+        if obj is self.sentinel:
+            raise StopAsyncIteration
+
+        return obj
+
+    @classmethod
+    async def create(cls, func: Callable[..., Cursor[T]]) -> AsyncCursor[T]:
+        cursor = await to_thread.run_sync(func)
+        return AsyncCursor(cursor)
+
+
 @attrs.define(eq=False)
 class MongoDBDataStore(BaseExternalDataStore):
     """
     Uses a MongoDB server to store data.
 
     When started, this data store creates the appropriate indexes on the given database
     if they're not already present.
 
     Operations are retried (in accordance to ``retry_settings``) when an operation
     raises :exc:`pymongo.errors.ConnectionFailure`.
 
-    :param client: a PyMongo client
+    :param client_or_uri: a PyMongo client or a MongoDB connection URI
     :param database: name of the database to use
 
+    .. note:: The data store will not manage the life cycle of any client instance
+        passed to it, so you need to close the client afterwards when you're done with
+        it.
+
     .. note:: Datetimes are stored as integers along with their UTC offsets instead of
         BSON datetimes due to the BSON datetimes only being accurate to the millisecond
         while Python datetimes are accurate to the microsecond.
     """
 
-    client: MongoClient = attrs.field(validator=instance_of(MongoClient))
-    database: str = attrs.field(default="apscheduler", kw_only=True)
+    client_or_uri: MongoClient | str = attrs.field(
+        validator=instance_of((MongoClient, str))
+    )
+    database: str = attrs.field(
+        default="apscheduler", kw_only=True, validator=instance_of(str)
+    )
 
+    _client: MongoClient = attrs.field(init=False)
+    _close_on_exit: bool = attrs.field(init=False, default=False)
     _task_attrs: ClassVar[list[str]] = [field.name for field in attrs.fields(Task)]
     _schedule_attrs: ClassVar[list[str]] = [
         field.name for field in attrs.fields(Schedule)
     ]
     _job_attrs: ClassVar[list[str]] = [field.name for field in attrs.fields(Job)]
     _tasks: Collection = attrs.field(init=False)
     _schedules: Collection = attrs.field(init=False)
@@ -113,56 +170,61 @@
     _jobs_results: Collection = attrs.field(init=False)
 
     @property
     def _temporary_failure_exceptions(self) -> tuple[type[Exception], ...]:
         return (ConnectionFailure,)
 
     def __attrs_post_init__(self) -> None:
+        if isinstance(self.client_or_uri, str):
+            self._client = MongoClient(self.client_or_uri)
+            self._close_on_exit = True
+        else:
+            self._client = self.client_or_uri
+
         type_registry = TypeRegistry(
             [
                 CustomEncoder(timedelta, timedelta.total_seconds),
                 CustomEncoder(ConflictPolicy, operator.attrgetter("name")),
                 CustomEncoder(CoalescePolicy, operator.attrgetter("name")),
                 CustomEncoder(JobOutcome, operator.attrgetter("name")),
             ]
         )
         codec_options = CodecOptions(
             type_registry=type_registry,
             uuid_representation=UuidRepresentation.STANDARD,
         )
-        database = self.client.get_database(self.database, codec_options=codec_options)
+        database = self._client.get_database(self.database, codec_options=codec_options)
         self._tasks = database["tasks"]
         self._schedules = database["schedules"]
         self._jobs = database["jobs"]
         self._jobs_results = database["job_results"]
 
-    @classmethod
-    def from_url(cls, uri: str, **options) -> MongoDBDataStore:
-        client = MongoClient(uri)
-        return cls(client, **options)
-
     def _initialize(self) -> None:
-        with self.client.start_session() as session:
+        with self._client.start_session() as session:
             if self.start_from_scratch:
                 self._tasks.delete_many({}, session=session)
                 self._schedules.delete_many({}, session=session)
                 self._jobs.delete_many({}, session=session)
                 self._jobs_results.delete_many({}, session=session)
 
             self._schedules.create_index("next_fire_time", session=session)
             self._jobs.create_index("task_id", session=session)
+            self._jobs.create_index("schedule_id", session=session)
             self._jobs.create_index("created_at", session=session)
             self._jobs_results.create_index("finished_at", session=session)
             self._jobs_results.create_index("expires_at", session=session)
 
     async def start(
         self, exit_stack: AsyncExitStack, event_broker: EventBroker, logger: Logger
     ) -> None:
+        if self._close_on_exit:
+            exit_stack.push_async_callback(to_thread.run_sync, self._client.close)
+
         await super().start(exit_stack, event_broker, logger)
-        server_info = await to_thread.run_sync(self.client.server_info)
+        server_info = await to_thread.run_sync(self._client.server_info)
         if server_info["versionArray"] < [4, 0]:
             raise RuntimeError(
                 f"MongoDB server must be at least v4.0; current version = "
                 f"{server_info['version']}"
             )
 
         async for attempt in self._retry():
@@ -214,61 +276,69 @@
         task = Task.unmarshal(self.serializer, document)
         return task
 
     async def get_tasks(self) -> list[Task]:
         async for attempt in self._retry():
             with attempt:
                 tasks: list[Task] = []
-                for document in self._tasks.find(
-                    projection=self._task_attrs, sort=[("_id", pymongo.ASCENDING)]
-                ):
-                    document["id"] = document.pop("_id")
-                    tasks.append(Task.unmarshal(self.serializer, document))
+                async with await AsyncCursor.create(
+                    lambda: self._tasks.find(
+                        projection=self._task_attrs, sort=[("_id", pymongo.ASCENDING)]
+                    )
+                ) as cursor:
+                    async for document in cursor:
+                        document["id"] = document.pop("_id")
+                        tasks.append(Task.unmarshal(self.serializer, document))
 
         return tasks
 
     async def get_schedules(self, ids: set[str] | None = None) -> list[Schedule]:
         filters = {"_id": {"$in": list(ids)}} if ids is not None else {}
         async for attempt in self._retry():
             with attempt:
                 schedules: list[Schedule] = []
-                cursor = self._schedules.find(filters).sort("_id")
-                for document in cursor:
-                    document["id"] = document.pop("_id")
-                    unmarshal_timestamps(document)
-                    try:
-                        schedule = Schedule.unmarshal(self.serializer, document)
-                    except DeserializationError:
-                        self._logger.warning(
-                            "Failed to deserialize schedule %r", document["_id"]
-                        )
-                        continue
+                async with await AsyncCursor.create(
+                    lambda: self._schedules.find(filters).sort("_id")
+                ) as cursor:
+                    async for document in cursor:
+                        document["id"] = document.pop("_id")
+                        unmarshal_timestamps(document)
+                        try:
+                            schedule = Schedule.unmarshal(self.serializer, document)
+                        except DeserializationError:
+                            self._logger.warning(
+                                "Failed to deserialize schedule %r", document["_id"]
+                            )
+                            continue
 
-                    schedules.append(schedule)
+                        schedules.append(schedule)
 
         return schedules
 
     async def add_schedule(
         self, schedule: Schedule, conflict_policy: ConflictPolicy
     ) -> None:
         event: DataStoreEvent
         document = schedule.marshal(self.serializer)
         marshal_document(document)
         try:
             async for attempt in self._retry():
                 with attempt:
-                    self._schedules.insert_one(document)
+                    await to_thread.run_sync(self._schedules.insert_one, document)
         except DuplicateKeyError:
             if conflict_policy is ConflictPolicy.exception:
                 raise ConflictingIdError(schedule.id) from None
             elif conflict_policy is ConflictPolicy.replace:
                 async for attempt in self._retry():
                     with attempt:
-                        self._schedules.replace_one(
-                            {"_id": schedule.id}, document, True
+                        await to_thread.run_sync(
+                            self._schedules.replace_one,
+                            {"_id": schedule.id},
+                            document,
+                            True,
                         )
 
                 event = ScheduleUpdated(
                     schedule_id=schedule.id,
                     task_id=schedule.task_id,
                     next_fire_time=schedule.next_fire_time,
                 )
@@ -280,53 +350,65 @@
                 next_fire_time=schedule.next_fire_time,
             )
             await self._event_broker.publish(event)
 
     async def remove_schedules(self, ids: Iterable[str]) -> None:
         filters = {"_id": {"$in": list(ids)}} if ids is not None else {}
         async for attempt in self._retry():
-            with attempt, self.client.start_session() as session:
-                cursor = self._schedules.find(
-                    filters, projection=["_id", "task_id"], session=session
-                )
-                ids = [(doc["_id"], doc["task_id"]) for doc in cursor]
-                if ids:
-                    self._schedules.delete_many(filters, session=session)
+            with attempt, self._client.start_session() as session:
+                async with await AsyncCursor.create(
+                    lambda: self._schedules.find(
+                        filters, projection=["_id", "task_id"], session=session
+                    )
+                ) as cursor:
+                    ids = [(doc["_id"], doc["task_id"]) async for doc in cursor]
+                    if ids:
+                        self._schedules.delete_many(filters, session=session)
 
         for schedule_id, task_id in ids:
             await self._event_broker.publish(
                 ScheduleRemoved(
                     schedule_id=schedule_id, task_id=task_id, finished=False
                 )
             )
 
     async def acquire_schedules(self, scheduler_id: str, limit: int) -> list[Schedule]:
         async for attempt in self._retry():
-            with attempt, self.client.start_session() as session:
+            with attempt, self._client.start_session() as session:
                 schedules: list[Schedule] = []
                 now = datetime.now(timezone.utc).timestamp()
-                cursor = (
-                    self._schedules.find(
+                async with await AsyncCursor.create(
+                    lambda: self._schedules.find(
                         {
                             "next_fire_time": {"$lte": now},
-                            "$or": [
-                                {"acquired_until": {"$exists": False}},
-                                {"acquired_until": {"$lt": now}},
+                            "$and": [
+                                {
+                                    "$or": [
+                                        {"paused": {"$exists": False}},
+                                        {"paused": False},
+                                    ]
+                                },
+                                {
+                                    "$or": [
+                                        {"acquired_until": {"$exists": False}},
+                                        {"acquired_until": {"$lt": now}},
+                                    ]
+                                },
                             ],
                         },
                         session=session,
                     )
                     .sort("next_fire_time")
                     .limit(limit)
-                )
-                for document in cursor:
-                    document["id"] = document.pop("_id")
-                    unmarshal_timestamps(document)
-                    schedule = Schedule.unmarshal(self.serializer, document)
-                    schedules.append(schedule)
+                ) as cursor:
+                    async for document in cursor:
+                        document["id"] = document.pop("_id")
+                        unmarshal_timestamps(document)
+                        schedule = Schedule.unmarshal(self.serializer, document)
+                        schedules.append(schedule)
 
                 if schedules:
                     now = datetime.now(timezone.utc)
                     acquired_until = now + timedelta(seconds=self.lock_expiration_delay)
                     filters = {"_id": {"$in": [schedule.id for schedule in schedules]}}
                     update = {
                         "$set": {
@@ -341,53 +423,50 @@
     async def release_schedules(
         self, scheduler_id: str, schedules: list[Schedule]
     ) -> None:
         updated_schedules: list[tuple[str, datetime]] = []
         finished_schedule_ids: list[str] = []
         task_ids = {schedule.id: schedule.task_id for schedule in schedules}
 
-        # Update schedules that have a next fire time
         requests = []
         for schedule in schedules:
             filters = {"_id": schedule.id, "acquired_by": scheduler_id}
-            if schedule.next_fire_time is not None:
-                try:
-                    serialized_trigger = self.serializer.serialize(schedule.trigger)
-                except SerializationError:
-                    self._logger.exception(
-                        "Error serializing schedule %r – removing from data store",
-                        schedule.id,
-                    )
-                    requests.append(DeleteOne(filters))
-                    finished_schedule_ids.append(schedule.id)
-                    continue
-
-                update = {
-                    "$unset": {
-                        "acquired_by": True,
-                        "acquired_until": True,
-                        "acquired_until_utcoffset": True,
-                    },
-                    "$set": {
-                        "trigger": serialized_trigger,
-                        **marshal_timestamp(schedule.next_fire_time, "next_fire_time"),
-                    },
-                }
-                requests.append(UpdateOne(filters, update))
-                updated_schedules.append((schedule.id, schedule.next_fire_time))
-            else:
+            try:
+                serialized_trigger = self.serializer.serialize(schedule.trigger)
+            except SerializationError:
+                self._logger.exception(
+                    "Error serializing schedule %r – removing from data store",
+                    schedule.id,
+                )
                 requests.append(DeleteOne(filters))
                 finished_schedule_ids.append(schedule.id)
+                continue
 
-            if requests:
-                async for attempt in self._retry():
-                    with attempt, self.client.start_session() as session:
-                        self._schedules.bulk_write(
+            update = {
+                "$unset": {
+                    "acquired_by": True,
+                    "acquired_until": True,
+                    "acquired_until_utcoffset": True,
+                },
+                "$set": {
+                    "trigger": serialized_trigger,
+                    **marshal_timestamp(schedule.next_fire_time, "next_fire_time"),
+                },
+            }
+            requests.append(UpdateOne(filters, update))
+            updated_schedules.append((schedule.id, schedule.next_fire_time))
+
+        if requests:
+            async for attempt in self._retry():
+                with attempt, self._client.start_session() as session:
+                    await to_thread.run_sync(
+                        lambda: self._schedules.bulk_write(
                             requests, ordered=False, session=session
                         )
+                    )
 
         for schedule_id, next_fire_time in updated_schedules:
             event = ScheduleUpdated(
                 schedule_id=schedule_id,
                 task_id=task_ids[schedule_id],
                 next_fire_time=next_fire_time,
             )
@@ -401,84 +480,97 @@
                     finished=True,
                 )
             )
 
     async def get_next_schedule_run_time(self) -> datetime | None:
         async for attempt in self._retry():
             with attempt:
-                document = self._schedules.find_one(
-                    {"next_fire_time": {"$ne": None}},
-                    projection=["next_fire_time", "next_fire_time_utcoffset"],
-                    sort=[("next_fire_time", ASCENDING)],
+                document = await to_thread.run_sync(
+                    lambda: self._schedules.find_one(
+                        {"next_fire_time": {"$ne": None}},
+                        projection=["next_fire_time", "next_fire_time_utcoffset"],
+                        sort=[("next_fire_time", ASCENDING)],
+                    )
                 )
 
         if document:
             unmarshal_timestamps(document)
             return document["next_fire_time"]
         else:
             return None
 
     async def add_job(self, job: Job) -> None:
         document = job.marshal(self.serializer)
         marshal_document(document)
         async for attempt in self._retry():
             with attempt:
-                self._jobs.insert_one(document)
+                await to_thread.run_sync(self._jobs.insert_one, document)
 
         event = JobAdded(
             job_id=job.id,
             task_id=job.task_id,
             schedule_id=job.schedule_id,
         )
         await self._event_broker.publish(event)
 
     async def get_jobs(self, ids: Iterable[UUID] | None = None) -> list[Job]:
         filters = {"_id": {"$in": list(ids)}} if ids is not None else {}
         async for attempt in self._retry():
             with attempt:
                 jobs: list[Job] = []
-                cursor = self._jobs.find(filters).sort("_id")
-                for document in cursor:
-                    document["id"] = document.pop("_id")
-                    unmarshal_timestamps(document)
-                    try:
-                        job = Job.unmarshal(self.serializer, document)
-                    except DeserializationError:
-                        self._logger.warning(
-                            "Failed to deserialize job %r", document["id"]
-                        )
-                        continue
+                async with await AsyncCursor.create(
+                    lambda: self._jobs.find(filters).sort("_id")
+                ) as cursor:
+                    async for document in cursor:
+                        document["id"] = document.pop("_id")
+                        unmarshal_timestamps(document)
+                        try:
+                            job = Job.unmarshal(self.serializer, document)
+                        except DeserializationError:
+                            self._logger.warning(
+                                "Failed to deserialize job %r", document["id"]
+                            )
+                            continue
 
-                    jobs.append(job)
+                        jobs.append(job)
 
         return jobs
 
-    async def acquire_jobs(self, worker_id: str, limit: int | None = None) -> list[Job]:
+    async def acquire_jobs(
+        self, scheduler_id: str, limit: int | None = None
+    ) -> list[Job]:
         async for attempt in self._retry():
-            with attempt, self.client.start_session() as session:
+            with attempt, self._client.start_session() as session:
                 now = datetime.now(timezone.utc)
-                cursor = self._jobs.find(
-                    {
-                        "$or": [
-                            {"acquired_until": {"$exists": False}},
-                            {"acquired_until": {"$lt": now.timestamp()}},
-                        ]
-                    },
-                    sort=[("created_at", ASCENDING)],
-                    limit=limit,
-                    session=session,
-                )
-                documents = list(cursor)
+                async with await AsyncCursor.create(
+                    lambda: self._jobs.find(
+                        {
+                            "$or": [
+                                {"acquired_until": {"$exists": False}},
+                                {"acquired_until": {"$lt": now.timestamp()}},
+                            ]
+                        },
+                        sort=[("created_at", ASCENDING)],
+                        limit=limit,
+                        session=session,
+                    )
+                ) as cursor:
+                    documents = [doc async for doc in cursor]
 
                 # Retrieve the limits
                 task_ids: set[str] = {document["task_id"] for document in documents}
-                task_limits = self._tasks.find(
-                    {"_id": {"$in": list(task_ids)}, "max_running_jobs": {"$ne": None}},
-                    projection=["max_running_jobs", "running_jobs"],
-                    session=session,
+                task_limits = await to_thread.run_sync(
+                    lambda: self._tasks.find(
+                        {
+                            "_id": {"$in": list(task_ids)},
+                            "max_running_jobs": {"$ne": None},
+                        },
+                        projection=["max_running_jobs", "running_jobs"],
+                        session=session,
+                    )
                 )
                 job_slots_left = {
                     doc["_id"]: doc["max_running_jobs"] - doc["running_jobs"]
                     for doc in task_limits
                 }
 
                 # Filter out jobs that don't have free slots
@@ -503,60 +595,130 @@
                     now = datetime.now(timezone.utc)
                     acquired_until = datetime.fromtimestamp(
                         now.timestamp() + self.lock_expiration_delay, timezone.utc
                     )
                     filters = {"_id": {"$in": [job.id for job in acquired_jobs]}}
                     update = {
                         "$set": {
-                            "acquired_by": worker_id,
+                            "acquired_by": scheduler_id,
                             **marshal_timestamp(acquired_until, "acquired_until"),
                         }
                     }
-                    self._jobs.update_many(filters, update, session=session)
+                    await to_thread.run_sync(
+                        lambda: self._jobs.update_many(filters, update, session=session)
+                    )
 
                     # Increment the running job counters on each task
                     for task_id, increment in increments.items():
-                        self._tasks.find_one_and_update(
-                            {"_id": task_id},
-                            {"$inc": {"running_jobs": increment}},
-                            session=session,
+                        await to_thread.run_sync(
+                            lambda: self._tasks.find_one_and_update(
+                                {"_id": task_id},
+                                {"$inc": {"running_jobs": increment}},
+                                session=session,
+                            )
                         )
 
         # Publish the appropriate events
         for job in acquired_jobs:
             await self._event_broker.publish(
-                JobAcquired(job_id=job.id, scheduler_id=worker_id)
+                JobAcquired.from_job(job, scheduler_id=scheduler_id)
             )
 
         return acquired_jobs
 
-    async def release_job(
-        self, worker_id: str, task_id: str, result: JobResult
-    ) -> None:
+    async def release_job(self, scheduler_id: str, job: Job, result: JobResult) -> None:
         async for attempt in self._retry():
-            with attempt, self.client.start_session() as session:
+            with attempt, self._client.start_session() as session:
                 # Record the job result
                 if result.expires_at > result.finished_at:
                     document = result.marshal(self.serializer)
                     document["_id"] = document.pop("job_id")
                     marshal_document(document)
                     self._jobs_results.insert_one(document, session=session)
 
                 # Decrement the running jobs counter
-                self._tasks.find_one_and_update(
-                    {"_id": task_id}, {"$inc": {"running_jobs": -1}}, session=session
+                await to_thread.run_sync(
+                    lambda: self._tasks.find_one_and_update(
+                        {"_id": job.task_id},
+                        {"$inc": {"running_jobs": -1}},
+                        session=session,
+                    )
                 )
 
                 # Delete the job
-                self._jobs.delete_one({"_id": result.job_id}, session=session)
+                await to_thread.run_sync(
+                    lambda: self._jobs.delete_one(
+                        {"_id": result.job_id}, session=session
+                    )
+                )
+
+        # Notify other schedulers
+        await self._event_broker.publish(
+            JobReleased.from_result(job, result, scheduler_id)
+        )
 
     async def get_job_result(self, job_id: UUID) -> JobResult | None:
         async for attempt in self._retry():
             with attempt:
-                document = self._jobs_results.find_one_and_delete({"_id": job_id})
+                document = await to_thread.run_sync(
+                    lambda: self._jobs_results.find_one_and_delete({"_id": job_id})
+                )
 
         if document:
             document["job_id"] = document.pop("_id")
             unmarshal_timestamps(document)
             return JobResult.unmarshal(self.serializer, document)
         else:
             return None
+
+    async def cleanup(self) -> None:
+        # Clean up expired job results
+        async for attempt in self._retry():
+            with attempt, self._client.start_session() as session:
+                # Purge expired job results
+                now = datetime.now(timezone.utc).timestamp()
+
+                await to_thread.run_sync(
+                    lambda: self._jobs_results.delete_many(
+                        {"expires_at": {"$lte": now}}, session=session
+                    )
+                )
+
+                # Find finished schedules
+                async with await AsyncCursor.create(
+                    lambda: self._schedules.find(
+                        {"next_fire_time": None},
+                        projection=["_id", "task_id"],
+                        session=session,
+                    )
+                ) as cursor:
+                    if finished_schedules := {
+                        item["_id"]: item["task_id"] async for item in cursor
+                    }:
+                        # Find distinct schedule IDs of jobs associated with these
+                        # schedules
+                        for schedule_id in await to_thread.run_sync(
+                            lambda: self._jobs.distinct(
+                                "schedule_id",
+                                {"schedule_id": {"$in": list(finished_schedules)}},
+                                session=session,
+                            )
+                        ):
+                            finished_schedules.pop(schedule_id)
+
+                # Delete finished schedules that not having any associated jobs
+                if finished_schedules:
+                    await to_thread.run_sync(
+                        lambda: self._schedules.delete_many(
+                            {"_id": {"$in": list(finished_schedules)}},
+                            session=session,
+                        )
+                    )
+
+                for schedule_id, task_id in finished_schedules.items():
+                    await self._event_broker.publish(
+                        ScheduleRemoved(
+                            schedule_id=schedule_id,
+                            task_id=task_id,
+                            finished=True,
+                        )
+                    )
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/datastores/sqlalchemy.py` & `apscheduler-4.0.0a5/src/apscheduler/datastores/sqlalchemy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 from __future__ import annotations
 
-import sys
 from collections import defaultdict
 from collections.abc import AsyncGenerator, Mapping, Sequence
 from contextlib import AsyncExitStack, asynccontextmanager
 from datetime import datetime, timedelta, timezone
 from functools import partial
 from logging import Logger
 from typing import Any, Iterable
 from uuid import UUID
 
 import anyio
 import attrs
 import sniffio
 import tenacity
 from anyio import CancelScope, to_thread
+from attr.validators import instance_of
 from sqlalchemy import (
     BigInteger,
+    Boolean,
     Column,
     DateTime,
     Enum,
     Integer,
     Interval,
     LargeBinary,
     MetaData,
     SmallInteger,
     Table,
     TypeDecorator,
     Unicode,
     Uuid,
     and_,
     bindparam,
+    create_engine,
+    false,
     or_,
     select,
 )
 from sqlalchemy.engine import URL, Dialect, Result
 from sqlalchemy.exc import (
     CompileError,
     IntegrityError,
     InterfaceError,
+    InvalidRequestError,
     ProgrammingError,
 )
 from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, create_async_engine
 from sqlalchemy.future import Connection, Engine
 from sqlalchemy.sql import Executable
 from sqlalchemy.sql.ddl import DropTable
 from sqlalchemy.sql.elements import BindParameter, literal
@@ -50,32 +54,28 @@
 
 from .._enums import CoalescePolicy, ConflictPolicy, JobOutcome
 from .._events import (
     DataStoreEvent,
     JobAcquired,
     JobAdded,
     JobDeserializationFailed,
+    JobReleased,
     ScheduleAdded,
     ScheduleDeserializationFailed,
     ScheduleRemoved,
     ScheduleUpdated,
     TaskAdded,
     TaskRemoved,
     TaskUpdated,
 )
 from .._exceptions import ConflictingIdError, SerializationError, TaskLookupError
 from .._structures import Job, JobResult, Schedule, Task
 from ..abc import EventBroker
 from .base import BaseExternalDataStore
 
-if sys.version_info >= (3, 11):
-    from typing import Self
-else:
-    from typing_extensions import Self
-
 
 class EmulatedTimestampTZ(TypeDecorator[datetime]):
     impl = Unicode(32)
     cache_ok = True
 
     def process_bind_param(
         self, value: datetime | None, dialect: Dialect
@@ -116,62 +116,65 @@
 
     This store has been tested to work with:
 
      * PostgreSQL (asyncpg and psycopg drivers)
      * MySQL (asyncmy driver)
      * aiosqlite
 
-    :param engine: an asynchronous SQLAlchemy engine
+    :param engine_or_url: a SQLAlchemy URL or engine (preferably asynchronous, but can
+        be synchronous)
     :param schema: a database schema name to use, if not the default
+
+    .. note:: The data store will not manage the life cycle of any engine instance
+        passed to it, so you need to close the engine afterwards when you're done with
+        it.
     """
 
-    engine: Engine | AsyncEngine
-    schema: str | None = attrs.field(default=None)
-    max_poll_time: float | None = attrs.field(default=1)
-    max_idle_time: float = attrs.field(default=60)
+    engine_or_url: str | URL | Engine | AsyncEngine = attrs.field(
+        validator=instance_of((str, URL, Engine, AsyncEngine))
+    )
+    schema: str | None = attrs.field(kw_only=True, default=None)
 
+    _engine: Engine | AsyncEngine = attrs.field(init=False)
+    _close_on_exit: bool = attrs.field(init=False, default=False)
     _supports_update_returning: bool = attrs.field(init=False, default=False)
     _supports_tzaware_timestamps: bool = attrs.field(init=False, default=False)
     _supports_native_interval: bool = attrs.field(init=False, default=False)
     _metadata: MetaData = attrs.field(init=False)
     _t_metadata: Table = attrs.field(init=False)
     _t_tasks: Table = attrs.field(init=False)
     _t_schedules: Table = attrs.field(init=False)
     _t_jobs: Table = attrs.field(init=False)
     _t_job_results: Table = attrs.field(init=False)
 
     def __attrs_post_init__(self) -> None:
+        if isinstance(self.engine_or_url, (str, URL)):
+            try:
+                self._engine = create_async_engine(self.engine_or_url)
+            except InvalidRequestError:
+                self._engine = create_engine(self.engine_or_url)
+
+            self._close_on_exit = True
+        else:
+            self._engine = self.engine_or_url
+
         # Generate the table definitions
         prefix = f"{self.schema}." if self.schema else ""
-        self._supports_tzaware_timestamps = self.engine.dialect in (
+        self._supports_tzaware_timestamps = self._engine.dialect.name in (
             "postgresql",
             "oracle",
         )
-        self._supports_native_interval = self.engine.dialect == "postgresql"
+        self._supports_native_interval = self._engine.dialect.name == "postgresql"
         self._metadata = self.get_table_definitions()
         self._t_metadata = self._metadata.tables[prefix + "metadata"]
         self._t_tasks = self._metadata.tables[prefix + "tasks"]
         self._t_schedules = self._metadata.tables[prefix + "schedules"]
         self._t_jobs = self._metadata.tables[prefix + "jobs"]
         self._t_job_results = self._metadata.tables[prefix + "job_results"]
 
-    @classmethod
-    def from_url(cls: type[Self], url: str | URL, **options) -> Self:
-        """
-        Create a new asynchronous SQLAlchemy data store.
-
-        :param url: an SQLAlchemy URL to pass to :func:`~sqlalchemy.create_engine`
-            (must use an async dialect like ``asyncpg`` or ``asyncmy``)
-        :param options: keyword arguments to pass to the initializer of this class
-        :return: the newly created data store
-
-        """
-        engine = create_async_engine(url, future=True)
-        return cls(engine, **options)
-
     def _retry(self) -> tenacity.AsyncRetrying:
         def after_attempt(retry_state: tenacity.RetryCallState) -> None:
             self._logger.warning(
                 "Temporary data store error (attempt %d): %s",
                 retry_state.attempt_number,
                 retry_state.outcome.exception(),
             )
@@ -189,21 +192,21 @@
     @asynccontextmanager
     async def _begin_transaction(
         self,
     ) -> AsyncGenerator[Connection | AsyncConnection, None]:
         # A shielded cancel scope is injected to the exit stack to allow finalization
         # to occur even when the surrounding cancel scope is cancelled
         async with AsyncExitStack() as exit_stack:
-            if isinstance(self.engine, AsyncEngine):
-                async_cm = self.engine.begin()
+            if isinstance(self._engine, AsyncEngine):
+                async_cm = self._engine.begin()
                 conn = await async_cm.__aenter__()
                 exit_stack.enter_context(CancelScope(shield=True))
                 exit_stack.push_async_exit(async_cm.__aexit__)
             else:
-                cm = self.engine.begin()
+                cm = self._engine.begin()
                 conn = await to_thread.run_sync(cm.__enter__)
                 exit_stack.enter_context(CancelScope(shield=True))
                 exit_stack.push_async_exit(partial(to_thread.run_sync, cm.__exit__))
 
             yield conn
 
     async def _create_metadata(self, conn: Connection | AsyncConnection) -> None:
@@ -222,15 +225,15 @@
             return await conn.execute(statement, parameters)
         else:
             return await to_thread.run_sync(conn.execute, statement, parameters)
 
     @property
     def _temporary_failure_exceptions(self) -> tuple[type[Exception], ...]:
         # SQlite does not use the network, so it doesn't have "temporary" failures
-        if self.engine.dialect == "sqlite":
+        if self._engine.dialect.name == "sqlite":
             return ()
 
         return InterfaceError, OSError
 
     def _convert_incoming_next_fire_time(self, data: dict[str, Any]) -> dict[str, Any]:
         if not self._supports_tzaware_timestamps:
             utcoffset_minutes = data.pop("next_fire_time_utcoffset", None)
@@ -288,61 +291,66 @@
             "schedules",
             metadata,
             Column("id", Unicode(500), primary_key=True),
             Column("task_id", Unicode(500), nullable=False, index=True),
             Column("trigger", LargeBinary),
             Column("args", LargeBinary),
             Column("kwargs", LargeBinary),
-            Column("coalesce", Enum(CoalescePolicy), nullable=False),
+            Column("paused", Boolean, nullable=False, server_default=literal(False)),
+            Column("coalesce", Enum(CoalescePolicy, metadata=metadata), nullable=False),
             Column("misfire_grace_time", interval_type),
             Column("max_jitter", interval_type),
             *next_fire_time_tzoffset_columns,
             Column("last_fire_time", timestamp_type),
             Column("acquired_by", Unicode(500)),
             Column("acquired_until", timestamp_type),
         )
         Table(
             "jobs",
             metadata,
             Column("id", Uuid, primary_key=True),
             Column("task_id", Unicode(500), nullable=False, index=True),
             Column("args", LargeBinary, nullable=False),
             Column("kwargs", LargeBinary, nullable=False),
-            Column("schedule_id", Unicode(500)),
+            Column("schedule_id", Unicode(500), index=True),
             Column("scheduled_fire_time", timestamp_type),
             Column("jitter", interval_type),
             Column("start_deadline", timestamp_type),
             Column("result_expiration_time", interval_type),
             Column("created_at", timestamp_type, nullable=False),
-            Column("started_at", timestamp_type),
             Column("acquired_by", Unicode(500)),
             Column("acquired_until", timestamp_type),
         )
         Table(
             "job_results",
             metadata,
             Column("job_id", Uuid, primary_key=True),
-            Column("outcome", Enum(JobOutcome), nullable=False),
-            Column("finished_at", timestamp_type, index=True),
+            Column("outcome", Enum(JobOutcome, metadata=metadata), nullable=False),
+            Column("started_at", timestamp_type, index=True),
+            Column("finished_at", timestamp_type, nullable=False, index=True),
             Column("expires_at", timestamp_type, nullable=False, index=True),
             Column("exception", LargeBinary),
             Column("return_value", LargeBinary),
         )
         return metadata
 
     async def start(
         self, exit_stack: AsyncExitStack, event_broker: EventBroker, logger: Logger
     ) -> None:
-        await super().start(exit_stack, event_broker, logger)
         asynclib = sniffio.current_async_library() or "(unknown)"
         if asynclib != "asyncio":
             raise RuntimeError(
                 f"This data store requires asyncio; currently running: {asynclib}"
             )
 
+        if self._close_on_exit:
+            exit_stack.push_async_callback(self._engine.dispose)
+
+        await super().start(exit_stack, event_broker, logger)
+
         # Verify that the schema is in place
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     if self.start_from_scratch:
                         for table in self._metadata.sorted_tables:
                             await self._execute(conn, DropTable(table, if_exists=True))
@@ -595,14 +603,15 @@
 
                     schedules_cte = (
                         select(self._t_schedules.c.id)
                         .where(
                             and_(
                                 self._t_schedules.c.next_fire_time.isnot(None),
                                 comparison,
+                                self._t_schedules.c.paused == false(),
                                 or_(
                                     self._t_schedules.c.acquired_until.is_(None),
                                     self._t_schedules.c.acquired_until < now,
                                 ),
                             )
                         )
                         .order_by(self._t_schedules.c.next_fire_time)
@@ -640,55 +649,57 @@
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     update_events: list[ScheduleUpdated] = []
                     finished_schedule_ids: list[str] = []
                     update_args: list[dict[str, Any]] = []
                     for schedule in schedules:
-                        if schedule.next_fire_time is not None:
-                            try:
-                                serialized_trigger = self.serializer.serialize(
-                                    schedule.trigger
-                                )
-                            except SerializationError:
-                                self._logger.exception(
-                                    "Error serializing trigger for schedule %r – "
-                                    "removing from data store",
-                                    schedule.id,
-                                )
-                                finished_schedule_ids.append(schedule.id)
-                                continue
+                        try:
+                            serialized_trigger = self.serializer.serialize(
+                                schedule.trigger
+                            )
+                        except SerializationError:
+                            self._logger.exception(
+                                "Error serializing trigger for schedule %r – "
+                                "removing from data store",
+                                schedule.id,
+                            )
+                            finished_schedule_ids.append(schedule.id)
+                            continue
 
-                            if self._supports_tzaware_timestamps:
-                                update_args.append(
-                                    {
-                                        "p_id": schedule.id,
-                                        "p_trigger": serialized_trigger,
-                                        "p_next_fire_time": schedule.next_fire_time,
-                                    }
+                        if self._supports_tzaware_timestamps:
+                            update_args.append(
+                                {
+                                    "p_id": schedule.id,
+                                    "p_trigger": serialized_trigger,
+                                    "p_next_fire_time": schedule.next_fire_time,
+                                }
+                            )
+                        else:
+                            if schedule.next_fire_time is not None:
+                                timestamp = int(
+                                    schedule.next_fire_time.timestamp() * 1000_000
                                 )
-                            else:
-                                update_args.append(
-                                    {
-                                        "p_id": schedule.id,
-                                        "p_trigger": serialized_trigger,
-                                        "p_next_fire_time": int(
-                                            schedule.next_fire_time.timestamp()
-                                            * 1000_000
-                                        ),
-                                        "p_next_fire_time_utcoffset": (
-                                            schedule.next_fire_time.utcoffset().total_seconds()
-                                            // 60
-                                        ),
-                                    }
+                                utcoffset = (
+                                    schedule.next_fire_time.utcoffset().total_seconds()
+                                    // 60
                                 )
-                        else:
-                            finished_schedule_ids.append(schedule.id)
+                            else:
+                                timestamp = utcoffset = None
+
+                            update_args.append(
+                                {
+                                    "p_id": schedule.id,
+                                    "p_trigger": serialized_trigger,
+                                    "p_next_fire_time": timestamp,
+                                    "p_next_fire_time_utcoffset": utcoffset,
+                                }
+                            )
 
-                    # Update schedules that have a next fire time
+                    # Update schedules
                     if update_args:
                         extra_values = {}
                         p_id: BindParameter = bindparam("p_id")
                         p_trigger: BindParameter = bindparam("p_trigger")
                         p_next_fire_time: BindParameter = bindparam("p_next_fire_time")
                         if not self._supports_tzaware_timestamps:
                             extra_values["next_fire_time_utcoffset"] = bindparam(
@@ -719,16 +730,15 @@
                             event = ScheduleUpdated(
                                 schedule_id=schedule_id,
                                 task_id=task_ids[schedule_id],
                                 next_fire_time=next_fire_times[schedule_id],
                             )
                             update_events.append(event)
 
-                    # Remove schedules that have no next fire time or failed to
-                    # serialize
+                    # Remove schedules that failed to serialize
                     if finished_schedule_ids:
                         delete = self._t_schedules.delete().where(
                             self._t_schedules.c.id.in_(finished_schedule_ids)
                         )
                         await self._execute(conn, delete)
 
         for event in update_events:
@@ -746,15 +756,18 @@
     async def get_next_schedule_run_time(self) -> datetime | None:
         columns = [self._t_schedules.c.next_fire_time]
         if not self._supports_tzaware_timestamps:
             columns.append(self._t_schedules.c.next_fire_time_utcoffset)
 
         statenent = (
             select(*columns)
-            .where(self._t_schedules.c.next_fire_time.isnot(None))
+            .where(
+                self._t_schedules.c.next_fire_time.isnot(None),
+                self._t_schedules.c.paused == false(),
+            )
             .order_by(self._t_schedules.c.next_fire_time)
             .limit(1)
         )
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     result = await self._execute(conn, statenent)
@@ -792,15 +805,17 @@
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     result = await self._execute(conn, query)
 
         return await self._deserialize_jobs(result)
 
-    async def acquire_jobs(self, worker_id: str, limit: int | None = None) -> list[Job]:
+    async def acquire_jobs(
+        self, scheduler_id: str, limit: int | None = None
+    ) -> list[Job]:
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     now = datetime.now(timezone.utc)
                     acquired_until = now + timedelta(seconds=self.lock_expiration_delay)
                     query = (
                         self._t_jobs.select()
@@ -853,15 +868,15 @@
 
                     if acquired_jobs:
                         # Mark the acquired jobs as acquired by this worker
                         acquired_job_ids = [job.id for job in acquired_jobs]
                         update = (
                             self._t_jobs.update()
                             .values(
-                                acquired_by=worker_id, acquired_until=acquired_until
+                                acquired_by=scheduler_id, acquired_until=acquired_until
                             )
                             .where(self._t_jobs.c.id.in_(acquired_job_ids))
                         )
                         await self._execute(conn, update)
 
                         # Increment the running job counters on each task
                         p_id: BindParameter = bindparam("p_id")
@@ -878,45 +893,48 @@
                             .where(self._t_tasks.c.id == p_id)
                         )
                         await self._execute(conn, update, params)
 
         # Publish the appropriate events
         for job in acquired_jobs:
             await self._event_broker.publish(
-                JobAcquired(job_id=job.id, scheduler_id=worker_id)
+                JobAcquired.from_job(job, scheduler_id=scheduler_id)
             )
 
         return acquired_jobs
 
-    async def release_job(
-        self, worker_id: str, task_id: str, result: JobResult
-    ) -> None:
+    async def release_job(self, scheduler_id: str, job: Job, result: JobResult) -> None:
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     # Record the job result
                     if result.expires_at > result.finished_at:
                         marshalled = result.marshal(self.serializer)
                         insert = self._t_job_results.insert().values(**marshalled)
                         await self._execute(conn, insert)
 
                     # Decrement the number of running jobs for this task
                     update = (
                         self._t_tasks.update()
                         .values(running_jobs=self._t_tasks.c.running_jobs - 1)
-                        .where(self._t_tasks.c.id == task_id)
+                        .where(self._t_tasks.c.id == job.task_id)
                     )
                     await self._execute(conn, update)
 
                     # Delete the job
                     delete = self._t_jobs.delete().where(
                         self._t_jobs.c.id == result.job_id
                     )
                     await self._execute(conn, delete)
 
+        # Notify other schedulers
+        await self._event_broker.publish(
+            JobReleased.from_result(job, result, scheduler_id)
+        )
+
     async def get_job_result(self, job_id: UUID) -> JobResult | None:
         async for attempt in self._retry():
             with attempt:
                 async with self._begin_transaction() as conn:
                     # Retrieve the result
                     query = self._t_job_results.select().where(
                         self._t_job_results.c.job_id == job_id
@@ -926,7 +944,45 @@
                     # Delete the result
                     delete = self._t_job_results.delete().where(
                         self._t_job_results.c.job_id == job_id
                     )
                     await self._execute(conn, delete)
 
         return JobResult.unmarshal(self.serializer, row._asdict()) if row else None
+
+    async def cleanup(self) -> None:
+        async for attempt in self._retry():
+            with attempt:
+                async with self._begin_transaction() as conn:
+                    # Purge expired job results
+                    delete = self._t_job_results.delete().where(
+                        self._t_job_results.c.expires_at <= datetime.now(timezone.utc)
+                    )
+                    await self._execute(conn, delete)
+
+                    # Clean up finished schedules that have no running jobs
+                    query = (
+                        select(self._t_schedules.c.id, self._t_schedules.c.task_id)
+                        .outerjoin(
+                            self._t_jobs,
+                            self._t_jobs.c.schedule_id == self._t_schedules.c.id,
+                        )
+                        .where(
+                            self._t_schedules.c.next_fire_time.is_(None),
+                            self._t_jobs.c.id.is_(None),
+                        )
+                    )
+                    results = await self._execute(conn, query)
+                    if finished_schedule_ids := dict(results.all()):
+                        delete = self._t_schedules.delete().where(
+                            self._t_schedules.c.id.in_(finished_schedule_ids)
+                        )
+                        await self._execute(conn, delete)
+
+                for schedule_id, task_id in finished_schedule_ids.items():
+                    await self._event_broker.publish(
+                        ScheduleRemoved(
+                            schedule_id=schedule_id,
+                            task_id=task_id,
+                            finished=True,
+                        )
+                    )
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/eventbrokers/asyncpg.py` & `apscheduler-4.0.0a5/src/apscheduler/eventbrokers/asyncpg.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/eventbrokers/base.py` & `apscheduler-4.0.0a5/src/apscheduler/eventbrokers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,19 +104,19 @@
 
     :param serializer: the serializer used to (de)serialize events for transport
     """
 
     serializer: Serializer = attrs.field(factory=JSONSerializer)
 
     def generate_notification(self, event: Event) -> bytes:
-        serialized = self.serializer.serialize(event.marshal(self.serializer))
+        serialized = self.serializer.serialize(event.marshal())
         return event.__class__.__name__.encode("ascii") + b" " + serialized
 
     def generate_notification_str(self, event: Event) -> str:
-        serialized = self.serializer.serialize(event.marshal(self.serializer))
+        serialized = self.serializer.serialize(event.marshal())
         return event.__class__.__name__ + " " + b64encode(serialized).decode("ascii")
 
     def _reconstitute_event(self, event_type: str, serialized: bytes) -> Event | None:
         try:
             kwargs = self.serializer.deserialize(serialized)
         except DeserializationError:
             self._logger.exception(
@@ -133,15 +133,15 @@
                 "Receive notification for a nonexistent event type: %s",
                 event_type,
                 extra={"serialized": serialized},
             )
             return None
 
         try:
-            return event_class.unmarshal(self.serializer, kwargs)
+            return event_class.unmarshal(kwargs)
         except Exception:
             self._logger.exception("Error reconstituting event of type %s", event_type)
             return None
 
     def reconstitute_event(self, payload: bytes) -> Event | None:
         try:
             event_type_bytes, serialized = payload.split(b" ", 1)
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/eventbrokers/mqtt.py` & `apscheduler-4.0.0a5/src/apscheduler/eventbrokers/mqtt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,133 @@
 from __future__ import annotations
 
 import sys
 from concurrent.futures import Future
 from contextlib import AsyncExitStack
 from logging import Logger
+from ssl import SSLContext
 from typing import Any
 
 import attrs
 from anyio import to_thread
 from anyio.from_thread import BlockingPortal
+from attr.validators import in_, instance_of, optional
 from paho.mqtt.client import Client, MQTTMessage
-from paho.mqtt.properties import Properties
-from paho.mqtt.reasoncodes import ReasonCodes
+from paho.mqtt.enums import CallbackAPIVersion
 
 from .._events import Event
 from .base import BaseExternalEventBroker
 
+ALLOWED_TRANSPORTS = ("mqtt", "mqtts", "ws", "wss", "unix")
+
 
 @attrs.define(eq=False)
 class MQTTEventBroker(BaseExternalEventBroker):
     """
     An event broker that uses an MQTT (v3.1 or v5) broker to broadcast events.
 
-    Requires the paho-mqtt_ library to be installed.
+    Requires the paho-mqtt_ library (v2.0 or later) to be installed.
 
     .. _paho-mqtt: https://pypi.org/project/paho-mqtt/
 
-    :param client: a paho-mqtt client
-    :param host: host name or IP address to connect to
-    :param port: TCP port number to connect to
+    :param host: MQTT broker host (or UNIX socket path)
+    :param port: MQTT broker port (for ``tcp`` or ``websocket`` transports)
+    :param transport: one of ``tcp``, ``websocket`` or ``unix`` (default: ``tcp``)
+    :param client_id: MQTT client ID (needed to resume an MQTT session if a connection
+        is broken)
+    :param ssl: either ``True`` or a custom SSL context to enable SSL/TLS, ``False`` to
+        disable
     :param topic: topic on which to send the messages
     :param subscribe_qos: MQTT QoS to use for subscribing messages
     :param publish_qos: MQTT QoS to use for publishing messages
     """
 
-    client: Client = attrs.field(factory=Client)
-    host: str = attrs.field(kw_only=True, default="localhost")
-    port: int = attrs.field(kw_only=True, default=1883)
-    topic: str = attrs.field(kw_only=True, default="apscheduler")
-    subscribe_qos: int = attrs.field(kw_only=True, default=0)
-    publish_qos: int = attrs.field(kw_only=True, default=0)
+    host: str = attrs.field(default="localhost", validator=instance_of(str))
+    port: int | None = attrs.field(default=None, validator=optional(instance_of(int)))
+    transport: str = attrs.field(
+        default="tcp", validator=in_(["tcp", "websocket", "unix"])
+    )
+    client_id: str | None = attrs.field(
+        default=None, validator=optional(instance_of(str))
+    )
+    ssl: bool | SSLContext = attrs.field(
+        default=False, validator=instance_of((bool, SSLContext))
+    )
+    topic: str = attrs.field(
+        kw_only=True, default="apscheduler", validator=instance_of(str)
+    )
+    subscribe_qos: int = attrs.field(kw_only=True, default=0, validator=in_([0, 1, 2]))
+    publish_qos: int = attrs.field(kw_only=True, default=0, validator=in_([0, 1, 2]))
+
+    _use_tls: bool = attrs.field(init=False, default=False)
+    _client: Client = attrs.field(init=False)
     _portal: BlockingPortal = attrs.field(init=False)
     _ready_future: Future[None] = attrs.field(init=False)
 
+    def __attrs_post_init__(self) -> None:
+        if self.port is None:
+            if self.transport == "tcp":
+                self.port = 8883 if self.ssl else 1883
+            elif self.transport == "websocket":
+                self.port = 443 if self.ssl else 80
+
+        self._client = Client(
+            callback_api_version=CallbackAPIVersion.VERSION2,
+            client_id=self.client_id,
+            transport=self.transport,
+        )
+        if isinstance(self.ssl, SSLContext):
+            self._client.tls_set_context(self.ssl)
+        elif self.ssl:
+            self._client.tls_set()
+
     async def start(self, exit_stack: AsyncExitStack, logger: Logger) -> None:
         await super().start(exit_stack, logger)
         self._portal = await exit_stack.enter_async_context(BlockingPortal())
         self._ready_future = Future()
-        self.client.on_connect = self._on_connect
-        self.client.on_connect_fail = self._on_connect_fail
-        self.client.on_disconnect = self._on_disconnect
-        self.client.on_message = self._on_message
-        self.client.on_subscribe = self._on_subscribe
-        self.client.connect(self.host, self.port)
-        self.client.loop_start()
-        exit_stack.push_async_callback(to_thread.run_sync, self.client.loop_stop)
+        self._client.on_connect = self._on_connect
+        self._client.on_connect_fail = self._on_connect_fail
+        self._client.on_disconnect = self._on_disconnect
+        self._client.on_message = self._on_message
+        self._client.on_subscribe = self._on_subscribe
+        self._client.connect_async(self.host, self.port)
+        self._client.loop_start()
+        exit_stack.push_async_callback(to_thread.run_sync, self._client.loop_stop)
+
+        # Wait for the connection attempt to be done
         await to_thread.run_sync(self._ready_future.result, 10)
-        exit_stack.push_async_callback(to_thread.run_sync, self.client.disconnect)
 
-    def _on_connect(
-        self,
-        client: Client,
-        userdata: Any,
-        flags: dict[str, Any],
-        rc: ReasonCodes | int,
-        properties: Properties | None = None,
-    ) -> None:
+        # Schedule a disconnection for when the exit stack is exited
+        exit_stack.callback(self._client.disconnect)
+
+    def _on_connect(self, client: Client, *_: Any) -> None:
         self._logger.info("%s: Connected", self.__class__.__name__)
         try:
             client.subscribe(self.topic, qos=self.subscribe_qos)
         except Exception as exc:
             self._ready_future.set_exception(exc)
             raise
 
-    def _on_connect_fail(self, client: Client, userdata: Any) -> None:
+    def _on_connect_fail(self, *_: Any) -> None:
         exc = sys.exc_info()[1]
         self._logger.error("%s: Connection failed (%s)", self.__class__.__name__, exc)
 
-    def _on_disconnect(
-        self,
-        client: Client,
-        userdata: Any,
-        rc: ReasonCodes | int,
-        properties: Properties | None = None,
-    ) -> None:
-        self._logger.error("%s: Disconnected (code: %s)", self.__class__.__name__, rc)
-
-    def _on_subscribe(
-        self, client: Client, userdata: Any, mid: int, granted_qos: list[int]
-    ) -> None:
+    def _on_disconnect(self, *args: Any) -> None:
+        reason_code = args[3] if len(args) == 5 else args[2]
+        self._logger.error(
+            "%s: Disconnected (code: %s)", self.__class__.__name__, reason_code
+        )
+
+    def _on_subscribe(self, *_: Any) -> None:
         self._logger.info("%s: Subscribed", self.__class__.__name__)
         self._ready_future.set_result(None)
 
-    def _on_message(self, client: Client, userdata: Any, msg: MQTTMessage) -> None:
+    def _on_message(self, _: Any, __: Any, msg: MQTTMessage) -> None:
         event = self.reconstitute_event(msg.payload)
         if event is not None:
             self._portal.call(self.publish_local, event)
 
     async def publish(self, event: Event) -> None:
         notification = self.generate_notification(event)
         await to_thread.run_sync(
-            lambda: self.client.publish(self.topic, notification, qos=self.publish_qos)
+            lambda: self._client.publish(self.topic, notification, qos=self.publish_qos)
         )
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/eventbrokers/redis.py` & `apscheduler-4.0.0a5/src/apscheduler/eventbrokers/redis.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from asyncio import CancelledError
 from contextlib import AsyncExitStack
 from logging import Logger
 
 import anyio
 import attrs
 import tenacity
+from anyio import move_on_after
+from attr.validators import instance_of
 from redis import ConnectionError
 from redis.asyncio import Redis
 from redis.asyncio.client import PubSub
 from redis.asyncio.connection import ConnectionPool
 
 from .._events import Event
 from .base import BaseExternalEventBroker
@@ -21,39 +23,41 @@
     """
     An event broker that uses a Redis server to broadcast events.
 
     Requires the redis_ library to be installed.
 
     .. _redis: https://pypi.org/project/redis/
 
-    :param client: an asynchronous Redis client
+    :param client_or_url: an asynchronous Redis client or a Redis URL
+        (```redis://...```)
     :param channel: channel on which to send the messages
     :param stop_check_interval: interval (in seconds) on which the channel listener
         should check if it should stop (higher values mean slower reaction time but less
         CPU use)
+
+    .. note:: The event broker will not manage the life cycle of any client instance
+        passed to it, so you need to close the client afterwards when you're done with
+        it.
     """
 
-    client: Redis
+    client_or_url: Redis | str = attrs.field(validator=instance_of((Redis, str)))
     channel: str = attrs.field(kw_only=True, default="apscheduler")
     stop_check_interval: float = attrs.field(kw_only=True, default=1)
+
+    _client: Redis = attrs.field(init=False)
+    _close_on_exit: bool = attrs.field(init=False, default=False)
     _stopped: bool = attrs.field(init=False, default=True)
 
-    @classmethod
-    def from_url(cls, url: str, **kwargs) -> RedisEventBroker:
-        """
-        Create a new event broker from a URL.
-
-        :param url: a Redis URL (```redis://...```)
-        :param kwargs: keyword arguments to pass to the initializer of this class
-        :return: the newly created event broker
-
-        """
-        pool = ConnectionPool.from_url(url)
-        client = Redis(connection_pool=pool)
-        return cls(client, **kwargs)
+    def __attrs_post_init__(self) -> None:
+        if isinstance(self.client_or_url, str):
+            pool = ConnectionPool.from_url(self.client_or_url)
+            self._client = Redis(connection_pool=pool)
+            self._close_on_exit = True
+        else:
+            self._client = self.client_or_url
 
     def _retry(self) -> tenacity.AsyncRetrying:
         def after_attempt(retry_state: tenacity.RetryCallState) -> None:
             self._logger.warning(
                 "%s: connection failure (attempt %d): %s",
                 self.__class__.__name__,
                 retry_state.attempt_number,
@@ -65,18 +69,27 @@
             wait=self.retry_settings.wait,
             retry=tenacity.retry_if_exception_type(ConnectionError),
             after=after_attempt,
             sleep=anyio.sleep,
             reraise=True,
         )
 
+    async def _close_client(self) -> None:
+        with move_on_after(5, shield=True):
+            await self._client.aclose(close_connection_pool=True)
+
     async def start(self, exit_stack: AsyncExitStack, logger: Logger) -> None:
-        await super().start(exit_stack, logger)
-        pubsub = self.client.pubsub()
+        # Close the client and its connection pool if this broker was created using
+        # .from_url()
+        if self._close_on_exit:
+            exit_stack.push_async_callback(self._close_client)
+
+        pubsub = await exit_stack.enter_async_context(self._client.pubsub())
         await pubsub.subscribe(self.channel)
+        await super().start(exit_stack, logger)
 
         self._stopped = False
         exit_stack.callback(setattr, self, "_stopped", True)
         self._task_group.start_soon(
             self._listen_messages, pubsub, name="Redis subscriber"
         )
 
@@ -97,15 +110,15 @@
             except Exception as exc:
                 # CancelledError is a subclass of Exception in Python 3.7
                 if not isinstance(exc, CancelledError):
                     self._logger.exception(
                         "%s listener crashed", self.__class__.__name__
                     )
 
-                await pubsub.close()
+                await pubsub.aclose()
                 raise
 
     async def publish(self, event: Event) -> None:
         notification = self.generate_notification(event)
         async for attempt in self._retry():
             with attempt:
-                await self.client.publish(self.channel, notification)
+                await self._client.publish(self.channel, notification)
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/executors/async_.py` & `apscheduler-4.0.0a5/src/apscheduler/executors/async_.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/executors/qt.py` & `apscheduler-4.0.0a5/src/apscheduler/executors/qt.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/executors/subprocess.py` & `apscheduler-4.0.0a5/src/apscheduler/executors/subprocess.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/executors/thread.py` & `apscheduler-4.0.0a5/src/apscheduler/executors/thread.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/serializers/cbor.py` & `apscheduler-4.0.0a5/src/apscheduler/serializers/cbor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from datetime import date, timedelta, tzinfo
+from enum import Enum
 from typing import Any
 
 import attrs
 from cbor2 import CBORDecoder, CBOREncoder, CBOREncodeTypeError, CBORTag, dumps, loads
 
 from .._marshalling import marshal_object, marshal_timezone, unmarshal_object
 from ..abc import Serializer
@@ -34,14 +35,16 @@
     def _default_hook(self, encoder: CBOREncoder, value: object) -> None:
         if isinstance(value, date):
             encoder.encode(value.isoformat())
         elif isinstance(value, timedelta):
             encoder.encode(value.total_seconds())
         elif isinstance(value, tzinfo):
             encoder.encode(marshal_timezone(value))
+        elif isinstance(value, Enum):
+            encoder.encode(value.name)
         elif hasattr(value, "__getstate__"):
             marshalled = marshal_object(value)
             encoder.encode(CBORTag(self.type_tag, marshalled))
         else:
             raise CBOREncodeTypeError(
                 f"cannot serialize type {value.__class__.__name__}"
             )
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/serializers/json.py` & `apscheduler-4.0.0a5/src/apscheduler/serializers/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from datetime import date, timedelta, tzinfo
+from enum import Enum
 from json import dumps, loads
 from typing import Any
 from uuid import UUID
 
 import attrs
 
 from .._marshalling import (
@@ -43,14 +44,16 @@
             return obj.isoformat()
         elif isinstance(obj, timedelta):
             return obj.total_seconds()
         elif isinstance(obj, tzinfo):
             return marshal_timezone(obj)
         elif isinstance(obj, UUID):
             return str(obj)
+        elif isinstance(obj, Enum):
+            return obj.name
         elif hasattr(obj, "__getstate__"):
             cls_ref, state = marshal_object(obj)
             return {self.magic_key: [cls_ref, state]}
 
         raise TypeError(
             f"Object of type {obj.__class__.__name__!r} is not JSON serializable"
         )
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/serializers/pickle.py` & `apscheduler-4.0.0a5/src/apscheduler/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/calendarinterval.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/calendarinterval.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from datetime import date, datetime, time, timedelta, tzinfo
 from typing import Any
 
 import attrs
+from attr.validators import instance_of, optional
 
-from .._utils import timezone_repr
-from .._validators import as_date, as_timezone, require_state_version
+from .._converters import as_aware_datetime, as_date, as_timezone
+from .._utils import require_state_version, timezone_repr
 from ..abc import Trigger
 
 
 @attrs.define(kw_only=True)
 class CalendarIntervalTrigger(Trigger):
     """
     Runs the task on specified calendar-based intervals always at the same exact time of
@@ -62,19 +63,27 @@
     years: int = 0
     months: int = 0
     weeks: int = 0
     days: int = 0
     hour: int = 0
     minute: int = 0
     second: int = 0
-    start_date: date = attrs.field(converter=as_date, factory=date.today)
-    end_date: date | None = attrs.field(converter=as_date, default=None)
-    timezone: tzinfo = attrs.field(converter=as_timezone, default="local")
+    start_date: date = attrs.field(
+        converter=as_date, validator=instance_of(date), factory=date.today
+    )
+    end_date: date | None = attrs.field(
+        converter=as_date, validator=optional(instance_of(date)), default=None
+    )
+    timezone: tzinfo = attrs.field(
+        converter=as_timezone, validator=instance_of(tzinfo), default="local"
+    )
     _time: time = attrs.field(init=False, eq=False)
-    _last_fire_date: date | None = attrs.field(init=False, eq=False, default=None)
+    _last_fire_date: date | None = attrs.field(
+        init=False, eq=False, converter=as_aware_datetime, default=None
+    )
 
     def __attrs_post_init__(self) -> None:
         self._time = time(self.hour, self.minute, self.second, tzinfo=self.timezone)
 
         if self.years == self.months == self.weeks == self.days == 0:
             raise ValueError("interval must be at least 1 day long")
 
@@ -105,15 +114,15 @@
                 return None
 
             # Combine the date with the designated time and normalize the result
             timestamp = datetime.combine(next_date, self._time).timestamp()
             next_time = datetime.fromtimestamp(timestamp, self.timezone)
 
             # Check if the time is off due to normalization and a forward DST shift
-            if next_time.time() != self._time:
+            if next_time.timetz() != self._time:
                 previous_date = next_time.date()
             else:
                 self._last_fire_date = next_date
                 return next_time
 
     def __getstate__(self) -> dict[str, Any]:
         return {
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/combining.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/combining.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from typing import Any
 
 import attrs
 
+from .._converters import as_aware_datetime, as_timedelta, list_converter
 from .._exceptions import MaxIterationsReached
 from .._marshalling import marshal_object, unmarshal_object
-from .._validators import as_timedelta, require_state_version
+from .._utils import require_state_version
 from ..abc import Trigger
 
 
 @attrs.define
 class BaseCombiningTrigger(Trigger):
     triggers: list[Trigger]
     _next_fire_times: list[datetime | None] = attrs.field(
-        init=False, eq=False, factory=list
+        init=False, eq=False, converter=list_converter(as_aware_datetime), factory=list
     )
 
     def __getstate__(self) -> dict[str, Any]:
         return {
             "version": 1,
             "triggers": [marshal_object(trigger) for trigger in self.triggers],
             "next_fire_times": self._next_fire_times,
@@ -82,15 +83,14 @@
             # Replace all the fire times that were within the threshold
             for i, _trigger in enumerate(self.triggers):
                 if self._next_fire_times[i] - earliest_fire_time <= self.threshold:
                     self._next_fire_times[i] = self.triggers[i].next()
 
             # If all the fire times were within the threshold, return the earliest one
             if latest_fire_time - earliest_fire_time <= self.threshold:
-                self._next_fire_times = [t.next() for t in self.triggers]
                 return earliest_fire_time
         else:
             raise MaxIterationsReached
 
     def __getstate__(self) -> dict[str, Any]:
         state = super().__getstate__()
         state["threshold"] = self.threshold
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/cron/__init__.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/cron/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta, tzinfo
 from typing import Any, ClassVar, Sequence
 
 import attrs
+from attr.validators import instance_of, optional
 from tzlocal import get_localzone
 
-from ..._utils import timezone_repr
-from ..._validators import as_aware_datetime, as_timezone, require_state_version
+from ..._converters import as_aware_datetime, as_timezone
+from ..._utils import require_state_version, timezone_repr
 from ...abc import Trigger
 from .fields import (
     DEFAULT_VALUES,
     BaseField,
     DayOfMonthField,
     DayOfWeekField,
     MonthField,
@@ -59,20 +60,30 @@
     day: int | str | None = None
     week: int | str | None = None
     day_of_week: int | str | None = None
     hour: int | str | None = None
     minute: int | str | None = None
     second: int | str | None = None
     start_time: datetime = attrs.field(
-        converter=as_aware_datetime, factory=datetime.now
+        converter=as_aware_datetime,
+        validator=instance_of(datetime),
+        factory=datetime.now,
+    )
+    end_time: datetime | None = attrs.field(
+        converter=as_aware_datetime,
+        validator=optional(instance_of(datetime)),
+        default=None,
+    )
+    timezone: tzinfo = attrs.field(
+        converter=as_timezone, validator=instance_of(tzinfo), factory=get_localzone
     )
-    end_time: datetime | None = attrs.field(converter=as_aware_datetime, default=None)
-    timezone: tzinfo = attrs.field(converter=as_timezone, factory=get_localzone)
     _fields: list[BaseField] = attrs.field(init=False, eq=False, factory=list)
-    _last_fire_time: datetime | None = attrs.field(init=False, eq=False, default=None)
+    _last_fire_time: datetime | None = attrs.field(
+        converter=as_aware_datetime, init=False, eq=False, default=None
+    )
 
     def __attrs_post_init__(self) -> None:
         self._set_fields(
             [
                 self.year,
                 self.month,
                 self.day,
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/cron/expressions.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/cron/expressions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """This module contains the expressions applicable for CronTrigger's fields."""
+
 from __future__ import annotations
 
 import re
 from calendar import monthrange
 from datetime import datetime
+from typing import TYPE_CHECKING, ClassVar, Pattern
+
+import attrs
+from attr.validators import instance_of, optional
+
+from ..._converters import as_int
+from ..._validators import non_negative_number, positive_number
 
-from ..._validators import as_int
+if TYPE_CHECKING:
+    from .fields import BaseField
 
 WEEKDAYS = ["mon", "tue", "wed", "thu", "fri", "sat", "sun"]
 MONTHS = [
     "jan",
     "feb",
     "mar",
     "apr",
@@ -27,67 +36,69 @@
 def get_weekday_index(weekday: str) -> int:
     try:
         return WEEKDAYS.index(weekday.lower())
     except ValueError:
         raise ValueError(f"Invalid weekday name {weekday!r}") from None
 
 
+@attrs.define(slots=True)
 class AllExpression:
-    __slots__ = "step"
+    value_re: ClassVar[Pattern] = re.compile(r"\*(?:/(?P<step>\d+))?$")
 
-    value_re = re.compile(r"\*(?:/(?P<step>\d+))?$")
-
-    def __init__(self, step: str | int | None = None):
-        self.step = as_int(step)
-        if self.step == 0:
-            raise ValueError("Step must be higher than 0")
+    step: int | None = attrs.field(
+        converter=as_int,
+        validator=optional([instance_of(int), positive_number]),
+        default=None,
+    )
 
     def validate_range(self, field_name: str, min_value: int, max_value: int) -> None:
         value_range = max_value - min_value
         if self.step and self.step > value_range:
             raise ValueError(
                 f"the step value ({self.step}) is higher than the total range of the "
                 f"expression ({value_range})"
             )
 
-    def get_next_value(self, dateval: datetime, field) -> int | None:
+    def get_next_value(self, dateval: datetime, field: BaseField) -> int | None:
         start = field.get_value(dateval)
         minval = field.get_min(dateval)
         maxval = field.get_max(dateval)
         start = max(start, minval)
 
         if not self.step:
             nextval = start
         else:
             distance_to_next = (self.step - (start - minval)) % self.step
             nextval = start + distance_to_next
 
         return nextval if nextval <= maxval else None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"*/{self.step}" if self.step else "*"
 
 
+@attrs.define(kw_only=True, slots=True)
 class RangeExpression(AllExpression):
-    __slots__ = "first", "last"
-
-    value_re = re.compile(r"(?P<first>\d+)(?:-(?P<last>\d+))?(?:/(?P<step>\d+))?$")
+    value_re: ClassVar[Pattern] = re.compile(
+        r"(?P<first>\d+)(?:-(?P<last>\d+))?(?:/(?P<step>\d+))?$"
+    )
 
-    def __init__(
-        self,
-        first: str | int,
-        last: str | int | None = None,
-        step: str | int | None = None,
-    ):
-        super().__init__(step)
-        self.first = as_int(first)
-        self.last = as_int(last)
+    first: int = attrs.field(
+        converter=as_int, validator=[instance_of(int), non_negative_number]
+    )
+    last: int = attrs.field(
+        converter=as_int,
+        validator=optional([instance_of(int), non_negative_number]),
+        default=None,
+    )
 
+    def __attrs_post_init__(self) -> None:
         if self.last is None and self.step is None:
             self.last = self.first
+
         if self.last is not None and self.first > self.last:
             raise ValueError(
                 "The minimum value in a range must not be higher than the maximum"
             )
 
     def validate_range(self, field_name: str, min_value: int, max_value: int) -> None:
         super().validate_range(field_name, min_value, max_value)
@@ -104,106 +115,111 @@
         value_range = (self.last or max_value) - self.first
         if self.step and self.step > value_range:
             raise ValueError(
                 f"the step value ({self.step}) is higher than the total range of the "
                 f"expression ({value_range})"
             )
 
-    def get_next_value(self, date, field):
-        startval = field.get_value(date)
-        minval = field.get_min(date)
-        maxval = field.get_max(date)
+    def get_next_value(self, dateval: datetime, field: BaseField) -> int | None:
+        startval = field.get_value(dateval)
+        minval = field.get_min(dateval)
+        maxval = field.get_max(dateval)
 
         # Apply range limits
         minval = max(minval, self.first)
         maxval = min(maxval, self.last) if self.last is not None else maxval
         nextval = max(minval, startval)
 
         # Apply the step if defined
         if self.step:
             distance_to_next = (self.step - (nextval - minval)) % self.step
             nextval += distance_to_next
 
         return nextval if nextval <= maxval else None
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
             rangeval = f"{self.first}-{self.last}"
         else:
             rangeval = str(self.first)
 
         if self.step:
             return f"{rangeval}/{self.step}"
 
         return rangeval
 
 
+# @attrs.define(kw_only=True, slots=True)
 class MonthRangeExpression(RangeExpression):
-    __slots__ = ()
-
-    value_re = re.compile(r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE)
+    value_re: ClassVar[Pattern] = re.compile(
+        r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE
+    )
 
-    def __init__(self, first, last=None):
+    def __init__(self, first: str, last: str | None = None):
         try:
             first_num = MONTHS.index(first.lower()) + 1
         except ValueError:
             raise ValueError(f"Invalid month name {first!r}") from None
 
         if last:
             try:
                 last_num = MONTHS.index(last.lower()) + 1
             except ValueError:
                 raise ValueError(f"Invalid month name {last!r}") from None
         else:
             last_num = None
 
-        super().__init__(first_num, last_num)
+        super().__init__(first=first_num, last=last_num)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
             return f"{MONTHS[self.first - 1]}-{MONTHS[self.last - 1]}"
 
         return MONTHS[self.first - 1]
 
 
+@attrs.define(kw_only=True, slots=True)
 class WeekdayRangeExpression(RangeExpression):
-    __slots__ = ()
-
-    value_re = re.compile(r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE)
+    value_re: ClassVar[Pattern] = re.compile(
+        r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE
+    )
 
     def __init__(self, first: str, last: str | None = None):
         first_num = get_weekday_index(first)
         last_num = get_weekday_index(last) if last else None
-        super().__init__(first_num, last_num)
+        self.__attrs_init__(first=first_num, last=last_num)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
             return f"{WEEKDAYS[self.first]}-{WEEKDAYS[self.last]}"
 
         return WEEKDAYS[self.first]
 
 
+@attrs.define(kw_only=True, slots=True)
 class WeekdayPositionExpression(AllExpression):
-    __slots__ = "option_num", "weekday"
-
-    options = ["1st", "2nd", "3rd", "4th", "5th", "last"]
-    value_re = re.compile(
-        r"(?P<option_name>%s) +(?P<weekday_name>(?:\d+|\w+))" % "|".join(options),
+    options: ClassVar[tuple[str, ...]] = ("1st", "2nd", "3rd", "4th", "5th", "last")
+    value_re: ClassVar[Pattern] = re.compile(
+        f"(?P<option_name>{'|'.join(options)}) +(?P<weekday_name>(?:\\d+|\\w+))",
         re.IGNORECASE,
     )
 
-    def __init__(self, option_name: str, weekday_name: str):
-        super().__init__(None)
-        self.option_num = self.options.index(option_name.lower())
+    option_num: int
+    weekday: int
+
+    def __init__(self, *, option_name: str, weekday_name: str):
+        option_num = self.options.index(option_name.lower())
         try:
-            self.weekday = WEEKDAYS.index(weekday_name.lower())
+            weekday = WEEKDAYS.index(weekday_name.lower())
         except ValueError:
             raise ValueError(f"Invalid weekday name {weekday_name!r}") from None
 
-    def get_next_value(self, dateval: datetime, field) -> int | None:
+        self.__attrs_init__(option_num=option_num, weekday=weekday)
+
+    def get_next_value(self, dateval: datetime, field: BaseField) -> int | None:
         # Figure out the weekday of the month's first day and the number of days in that
         # month
         first_day_wday, last_day = monthrange(dateval.year, dateval.month)
 
         # Calculate which day of the month is the first of the target weekdays
         first_hit_day = self.weekday - first_day_wday + 1
         if first_hit_day <= 0:
@@ -216,24 +232,22 @@
             target_day = first_hit_day + ((last_day - first_hit_day) // 7) * 7
 
         if last_day >= target_day >= dateval.day:
             return target_day
         else:
             return None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.options[self.option_num]} {WEEKDAYS[self.weekday]}"
 
 
 class LastDayOfMonthExpression(AllExpression):
-    __slots__ = ()
-
-    value_re = re.compile(r"last", re.IGNORECASE)
+    value_re: ClassVar[Pattern] = re.compile(r"last", re.IGNORECASE)
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(None)
 
-    def get_next_value(self, dateval: datetime, field):
+    def get_next_value(self, dateval: datetime, field: BaseField) -> int | None:
         return monthrange(dateval.year, dateval.month)[1]
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "last"
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/cron/fields.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/cron/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     ) from exc
 
                 self.expressions.append(compiled_expr)
                 return
 
         raise ValueError(f"Unrecognized expression {expr!r} for field {self.name!r}")
 
-    def __str__(self):
+    def __str__(self) -> str:
         expr_strings = (str(e) for e in self.expressions)
         return ",".join(expr_strings)
 
 
 class WeekField(BaseField, real=False):
     __slots__ = ()
```

### Comparing `APScheduler-4.0.0a4/src/apscheduler/triggers/interval.py` & `apscheduler-4.0.0a5/src/apscheduler/triggers/interval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from typing import Any
 
 import attrs
+from attr.validators import instance_of, optional
 
-from .._validators import as_aware_datetime, require_state_version
+from .._converters import as_aware_datetime
+from .._utils import require_state_version
 from ..abc import Trigger
 
 
 @attrs.define(kw_only=True)
 class IntervalTrigger(Trigger):
     """
     Triggers on specified intervals.
@@ -34,19 +36,27 @@
     weeks: float = 0
     days: float = 0
     hours: float = 0
     minutes: float = 0
     seconds: float = 0
     microseconds: float = 0
     start_time: datetime = attrs.field(
-        converter=as_aware_datetime, factory=datetime.now
+        converter=as_aware_datetime,
+        factory=datetime.now,
+        validator=instance_of(datetime),
+    )
+    end_time: datetime | None = attrs.field(
+        converter=as_aware_datetime,
+        validator=optional(instance_of(datetime)),
+        default=None,
     )
-    end_time: datetime | None = attrs.field(converter=as_aware_datetime, default=None)
     _interval: timedelta = attrs.field(init=False, eq=False, repr=False)
-    _last_fire_time: datetime | None = attrs.field(init=False, eq=False, default=None)
+    _last_fire_time: datetime | None = attrs.field(
+        init=False, eq=False, converter=as_aware_datetime, default=None
+    )
 
     def __attrs_post_init__(self) -> None:
         self._interval = timedelta(
             weeks=self.weeks,
             days=self.days,
             hours=self.hours,
             minutes=self.minutes,
```

### Comparing `APScheduler-4.0.0a4/tests/conftest.py` & `apscheduler-4.0.0a5/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import logging
 import sys
 from collections.abc import Generator
 from contextlib import AsyncExitStack
 from logging import Logger
-from tempfile import TemporaryDirectory
+from pathlib import Path
 from typing import Any, AsyncGenerator, cast
 
 import pytest
 from _pytest.fixtures import SubRequest
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 
 from apscheduler.abc import DataStore, EventBroker, Serializer
 from apscheduler.datastores.memory import MemoryDataStore
 from apscheduler.serializers.cbor import CBORSerializer
 from apscheduler.serializers.json import JSONSerializer
 from apscheduler.serializers.pickle import PickleSerializer
 
@@ -25,14 +25,19 @@
 
 
 @pytest.fixture(scope="session")
 def timezone() -> ZoneInfo:
     return ZoneInfo("Europe/Berlin")
 
 
+@pytest.fixture(scope="session")
+def utc_timezone() -> ZoneInfo:
+    return ZoneInfo("UTC")
+
+
 @pytest.fixture(
     params=[
         pytest.param(PickleSerializer, id="pickle"),
         pytest.param(CBORSerializer, id="cbor"),
         pytest.param(JSONSerializer, id="json"),
     ]
 )
@@ -50,33 +55,28 @@
     from apscheduler.eventbrokers.local import LocalEventBroker
 
     return LocalEventBroker()
 
 
 @pytest.fixture
 async def redis_broker(serializer: Serializer) -> EventBroker:
-    from redis.asyncio import Redis
-
     from apscheduler.eventbrokers.redis import RedisEventBroker
 
-    broker = RedisEventBroker.from_url(
+    broker = RedisEventBroker(
         "redis://localhost:6379", serializer=serializer, stop_check_interval=0.05
     )
-    assert isinstance(broker.client, Redis)
-    await broker.client.flushdb()
+    await broker._client.flushdb()
     return broker
 
 
 @pytest.fixture
 def mqtt_broker(serializer: Serializer) -> EventBroker:
-    from paho.mqtt.client import Client
-
     from apscheduler.eventbrokers.mqtt import MQTTEventBroker
 
-    return MQTTEventBroker(Client(), serializer=serializer)
+    return MQTTEventBroker(serializer=serializer)
 
 
 @pytest.fixture
 async def asyncpg_broker(serializer: Serializer) -> EventBroker:
     pytest.importorskip("asyncpg", reason="asyncpg is not installed")
     from apscheduler.eventbrokers.asyncpg import AsyncpgEventBroker
 
@@ -84,27 +84,27 @@
         "postgres://postgres:secret@localhost:5432/testdb", serializer=serializer
     )
     return broker
 
 
 @pytest.fixture(
     params=[
-        pytest.param(lazy_fixture("local_broker"), id="local"),
+        pytest.param(lf("local_broker"), id="local"),
         pytest.param(
-            lazy_fixture("asyncpg_broker"),
+            lf("asyncpg_broker"),
             id="asyncpg",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("redis_broker"),
+            lf("redis_broker"),
             id="redis",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("mqtt_broker"), id="mqtt", marks=[pytest.mark.external_service]
+            lf("mqtt_broker"), id="mqtt", marks=[pytest.mark.external_service]
         ),
     ]
 )
 async def raw_event_broker(request: SubRequest) -> EventBroker:
     return cast(EventBroker, request.param)
 
 
@@ -129,29 +129,14 @@
     from apscheduler.datastores.mongodb import MongoDBDataStore
 
     with MongoClient(tz_aware=True, serverSelectionTimeoutMS=1000) as client:
         yield MongoDBDataStore(client, start_from_scratch=True)
 
 
 @pytest.fixture
-def sqlite_store() -> Generator[DataStore, None, None]:
-    from sqlalchemy import create_engine
-
-    from apscheduler.datastores.sqlalchemy import SQLAlchemyDataStore
-
-    with TemporaryDirectory("sqlite_") as tempdir:
-        engine = create_engine(f"sqlite:///{tempdir}/test.db")
-        try:
-            yield SQLAlchemyDataStore(engine)
-            assert "Current Checked out connections: 0" in engine.pool.status()
-        finally:
-            engine.dispose()
-
-
-@pytest.fixture
 async def psycopg_async_store() -> AsyncGenerator[DataStore, None]:
     from sqlalchemy import text
     from sqlalchemy.ext.asyncio import create_async_engine
 
     from apscheduler.datastores.sqlalchemy import SQLAlchemyDataStore
 
     engine = create_async_engine(
@@ -199,25 +184,24 @@
         yield SQLAlchemyDataStore(engine, start_from_scratch=True)
         assert "Current Checked out connections: 0" in engine.pool.status()
     finally:
         engine.dispose()
 
 
 @pytest.fixture
-async def aiosqlite_store() -> AsyncGenerator[DataStore, None]:
+async def aiosqlite_store(tmp_path: Path) -> AsyncGenerator[DataStore, None]:
     from sqlalchemy.ext.asyncio import create_async_engine
 
     from apscheduler.datastores.sqlalchemy import SQLAlchemyDataStore
 
-    with TemporaryDirectory("sqlite_") as tempdir:
-        engine = create_async_engine(f"sqlite+aiosqlite:///{tempdir}/test.db")
-        try:
-            yield SQLAlchemyDataStore(engine)
-        finally:
-            await engine.dispose()
+    engine = create_async_engine(f"sqlite+aiosqlite:///{tmp_path}/test.db")
+    try:
+        yield SQLAlchemyDataStore(engine)
+    finally:
+        await engine.dispose()
 
 
 @pytest.fixture
 async def asyncpg_store() -> AsyncGenerator[DataStore, None]:
     pytest.importorskip("asyncpg", reason="asyncpg is not installed")
     from asyncpg import compat
     from sqlalchemy.ext.asyncio import create_async_engine
@@ -267,48 +251,48 @@
     finally:
         await engine.dispose()
 
 
 @pytest.fixture(
     params=[
         pytest.param(
-            lazy_fixture("memory_store"),
+            lf("memory_store"),
             id="memory",
         ),
         pytest.param(
-            lazy_fixture("aiosqlite_store"),
+            lf("aiosqlite_store"),
             id="aiosqlite",
         ),
         pytest.param(
-            lazy_fixture("asyncpg_store"),
+            lf("asyncpg_store"),
             id="asyncpg",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("asyncmy_store"),
+            lf("asyncmy_store"),
             id="asyncmy",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("psycopg_async_store"),
+            lf("psycopg_async_store"),
             id="psycopg_async",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("psycopg_sync_store"),
+            lf("psycopg_sync_store"),
             id="psycopg_sync",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("pymysql_store"),
+            lf("pymysql_store"),
             id="pymysql",
             marks=[pytest.mark.external_service],
         ),
         pytest.param(
-            lazy_fixture("mongodb_store"),
+            lf("mongodb_store"),
             id="mongodb",
             marks=[pytest.mark.external_service],
         ),
     ]
 )
 async def raw_datastore(request: SubRequest) -> DataStore:
     return cast(DataStore, request.param)
```

### Comparing `APScheduler-4.0.0a4/tests/test_datastores.py` & `apscheduler-4.0.0a5/tests/test_datastores.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
+import platform
 from contextlib import AsyncExitStack, asynccontextmanager
 from datetime import datetime, timedelta, timezone
 from logging import Logger
-from typing import AsyncGenerator
+from typing import TYPE_CHECKING, AsyncGenerator
 
 import anyio
 import pytest
 from anyio import CancelScope
-from freezegun.api import FrozenDateTimeFactory
 
 from apscheduler import (
     CoalescePolicy,
     ConflictPolicy,
     Event,
     Job,
     JobOutcome,
@@ -25,14 +25,17 @@
     TaskAdded,
     TaskLookupError,
     TaskUpdated,
 )
 from apscheduler.abc import DataStore, EventBroker
 from apscheduler.triggers.date import DateTrigger
 
+if TYPE_CHECKING:
+    from time_machine import TimeMachineFixture
+
 pytestmark = pytest.mark.anyio
 
 
 @pytest.fixture
 def schedules() -> list[Schedule]:
     trigger = DateTrigger(datetime(2020, 9, 13, tzinfo=timezone.utc))
     schedule1 = Schedule(id="s1", task_id="task1", trigger=trigger)
@@ -173,18 +176,23 @@
 
     received_event = events.pop(0)
     assert received_event.schedule_id == "s2"
 
     assert not events
 
 
-@pytest.mark.freeze_time(datetime(2020, 9, 14, tzinfo=timezone.utc))
+@pytest.mark.skipif(
+    platform.python_implementation() != "CPython",
+    reason="time-machine is not available",
+)
 async def test_acquire_release_schedules(
-    datastore: DataStore, schedules: list[Schedule]
+    datastore: DataStore, schedules: list[Schedule], time_machine: TimeMachineFixture
 ) -> None:
+    time_machine.move_to(datetime(2020, 9, 14, tzinfo=timezone.utc))
+
     event_types = {ScheduleRemoved, ScheduleUpdated}
     async with capture_events(datastore, 2, event_types) as events:
         for schedule in schedules:
             await datastore.add_schedule(schedule, ConflictPolicy.exception)
 
         # The first scheduler gets the first due schedule
         schedules1 = await datastore.acquire_schedules("dummy-id1", 1)
@@ -205,25 +213,28 @@
         schedules1[0].next_fire_time = None
         schedules2[0].next_fire_time = datetime(2020, 9, 15, tzinfo=timezone.utc)
 
         # Release all the schedules
         await datastore.release_schedules("dummy-id1", schedules1)
         await datastore.release_schedules("dummy-id2", schedules2)
 
-        # Check that the first schedule is gone
+        # Check that the first schedule has its next fire time nullified
         schedules = await datastore.get_schedules()
-        assert len(schedules) == 2
-        assert schedules[0].id == "s2"
-        assert schedules[1].id == "s3"
+        assert len(schedules) == 3
+        schedules.sort(key=lambda s: s.id)
+        assert schedules[0].id == "s1"
+        assert schedules[0].next_fire_time is None
+        assert schedules[1].id == "s2"
+        assert schedules[2].id == "s3"
 
     # Check for the appropriate update and delete events
     received_event = events.pop(0)
-    assert isinstance(received_event, ScheduleRemoved)
+    assert isinstance(received_event, ScheduleUpdated)
     assert received_event.schedule_id == "s1"
-    assert received_event.finished
+    assert received_event.next_fire_time is None
 
     received_event = events.pop(0)
     assert isinstance(received_event, ScheduleUpdated)
     assert received_event.schedule_id == "s2"
     assert received_event.next_fire_time == datetime(2020, 9, 15, tzinfo=timezone.utc)
 
     assert not events
@@ -238,16 +249,20 @@
         await datastore.add_schedule(schedule, ConflictPolicy.exception)
 
     schedules = await datastore.acquire_schedules("foo", 3)
     schedules[0].next_fire_time = None
     await datastore.release_schedules("foo", schedules)
 
     remaining = await datastore.get_schedules({s.id for s in schedules})
-    assert len(remaining) == 1
-    assert remaining[0].id == schedules[1].id
+    assert len(remaining) == 2
+    remaining.sort(key=lambda s: s.id)
+    assert remaining[0].id == schedules[0].id
+    assert remaining[0].next_fire_time is None
+    assert remaining[1].id == schedules[1].id
+    assert remaining[1].next_fire_time
 
 
 async def test_release_two_schedules_at_once(datastore: DataStore) -> None:
     """Regression test for #621."""
     for i in range(2):
         trigger = DateTrigger(datetime(2020, 9, 13, tzinfo=timezone.utc))
         schedule = Schedule(id=f"s{i}", task_id="task1", trigger=trigger)
@@ -257,37 +272,44 @@
     schedules = await datastore.acquire_schedules("foo", 3)
     await datastore.release_schedules("foo", schedules)
 
     remaining = await datastore.get_schedules({s.id for s in schedules})
     assert len(remaining) == 2
 
 
+@pytest.mark.skipif(
+    platform.python_implementation() != "CPython",
+    reason="time-machine is not available",
+)
 async def test_acquire_schedules_lock_timeout(
-    datastore: DataStore, schedules: list[Schedule], freezer
+    datastore: DataStore,
+    schedules: list[Schedule],
+    time_machine: TimeMachineFixture,
 ) -> None:
     """
     Test that a scheduler can acquire schedules that were acquired by another
     scheduler but not released within the lock timeout period.
 
     """
+    time_machine.move_to(datetime.now(timezone.utc), tick=False)
     await datastore.add_schedule(schedules[0], ConflictPolicy.exception)
 
     # First, one scheduler acquires the first available schedule
     acquired1 = await datastore.acquire_schedules("dummy-id1", 1)
     assert len(acquired1) == 1
     assert acquired1[0].id == "s1"
 
     # Try to acquire the schedule just at the threshold (now == acquired_until).
     # This should not yield any schedules.
-    freezer.tick(30)
+    time_machine.shift(30)
     acquired2 = await datastore.acquire_schedules("dummy-id2", 1)
     assert not acquired2
 
     # Right after that, the schedule should be available
-    freezer.tick(1)
+    time_machine.shift(1)
     acquired3 = await datastore.acquire_schedules("dummy-id2", 1)
     assert len(acquired3) == 1
     assert acquired3[0].id == "s1"
 
 
 async def test_acquire_multiple_workers(datastore: DataStore) -> None:
     await datastore.add_task(
@@ -321,15 +343,15 @@
 
     acquired = await datastore.acquire_jobs("worker_id", 2)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
     await datastore.release_job(
         "worker_id",
-        acquired[0].task_id,
+        acquired[0],
         JobResult.from_job(
             acquired[0],
             JobOutcome.success,
             return_value="foo",
         ),
     )
     result = await datastore.get_job_result(acquired[0].id)
@@ -351,15 +373,15 @@
 
     acquired = await datastore.acquire_jobs("worker_id", 2)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
     await datastore.release_job(
         "worker_id",
-        acquired[0].task_id,
+        acquired[0],
         JobResult.from_job(
             acquired[0],
             JobOutcome.error,
             exception=ValueError("foo"),
         ),
     )
     result = await datastore.get_job_result(acquired[0].id)
@@ -382,15 +404,15 @@
 
     acquired = await datastore.acquire_jobs("worker_id", 2)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
     await datastore.release_job(
         "worker_id",
-        acquired[0].task_id,
+        acquired[0],
         JobResult.from_job(
             acquired[0],
             JobOutcome.missed_start_deadline,
         ),
     )
     result = await datastore.get_job_result(acquired[0].id)
     assert result.outcome is JobOutcome.missed_start_deadline
@@ -411,53 +433,58 @@
 
     acquired = await datastore.acquire_jobs("worker1", 2)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
     await datastore.release_job(
         "worker1",
-        acquired[0].task_id,
+        acquired[0],
         JobResult.from_job(acquired[0], JobOutcome.cancelled),
     )
     result = await datastore.get_job_result(acquired[0].id)
     assert result.outcome is JobOutcome.cancelled
     assert result.exception is None
     assert result.return_value is None
 
     # Check that the job and its result are gone
     assert not await datastore.get_jobs({acquired[0].id})
     assert not await datastore.get_job_result(acquired[0].id)
 
 
+@pytest.mark.skipif(
+    platform.python_implementation() != "CPython",
+    reason="time-machine is not available",
+)
 async def test_acquire_jobs_lock_timeout(
-    datastore: DataStore, freezer: FrozenDateTimeFactory
+    datastore: DataStore, time_machine: TimeMachineFixture
 ) -> None:
     """
     Test that a worker can acquire jobs that were acquired by another scheduler but
     not released within the lock timeout period.
 
     """
     await datastore.add_task(
         Task(id="task1", func="contextlib:asynccontextmanager", job_executor="async")
     )
     job = Job(task_id="task1", result_expiration_time=timedelta(minutes=1))
     await datastore.add_job(job)
 
     # First, one worker acquires the first available job
+    time_machine.move_to(datetime.now(timezone.utc), tick=False)
     acquired = await datastore.acquire_jobs("worker1", 1)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
     # Try to acquire the job just at the threshold (now == acquired_until).
     # This should not yield any jobs.
-    freezer.tick(30)
+    time_machine.shift(30)
     assert not await datastore.acquire_jobs("worker2", 1)
 
     # Right after that, the job should be available
-    freezer.tick(1)
+    time_machine.shift(1)
     acquired = await datastore.acquire_jobs("worker2", 1)
     assert len(acquired) == 1
     assert acquired[0].id == job.id
 
 
 async def test_acquire_jobs_max_number_exceeded(datastore: DataStore) -> None:
     await datastore.add_task(
@@ -476,15 +503,15 @@
     # wqas 3
     acquired_jobs = await datastore.acquire_jobs("worker1", 3)
     assert [job.id for job in acquired_jobs] == [job.id for job in jobs[:2]]
 
     # Release one job, and the worker should be able to acquire the third job
     await datastore.release_job(
         "worker1",
-        acquired_jobs[0].task_id,
+        acquired_jobs[0],
         JobResult.from_job(
             acquired_jobs[0],
             JobOutcome.success,
             return_value=None,
         ),
     )
     acquired_jobs = await datastore.acquire_jobs("worker1", 3)
```

### Comparing `APScheduler-4.0.0a4/tests/test_eventbrokers.py` & `apscheduler-4.0.0a5/tests/test_eventbrokers.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/tests/test_marshalling.py` & `apscheduler-4.0.0a5/tests/test_marshalling.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/tests/test_schedulers.py` & `apscheduler-4.0.0a5/tests/test_schedulers.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 from functools import partial
 from pathlib import Path
 from queue import Queue
 from types import ModuleType
 
 import anyio
 import pytest
-from anyio import WouldBlock, create_memory_object_stream, fail_after
+from anyio import (
+    Lock,
+    WouldBlock,
+    create_memory_object_stream,
+    fail_after,
+    sleep,
+)
 from pytest import MonkeyPatch
 from pytest_mock import MockerFixture, MockFixture
 
 from apscheduler import (
     AsyncScheduler,
     CoalescePolicy,
     Event,
@@ -27,14 +33,15 @@
     JobAcquired,
     JobAdded,
     JobLookupError,
     JobOutcome,
     JobReleased,
     RunState,
     ScheduleAdded,
+    ScheduleLookupError,
     Scheduler,
     ScheduleRemoved,
     SchedulerRole,
     SchedulerStarted,
     SchedulerStopped,
     ScheduleUpdated,
     TaskAdded,
@@ -187,32 +194,42 @@
             assert isinstance(event, TaskAdded)
             assert event.task_id == "mytask"
 
             event = await receive.receive()
             assert isinstance(event, TaskUpdated)
             assert event.task_id == "mytask"
 
-    async def test_add_remove_schedule(
+    async def test_add_pause_unpause_remove_schedule(
         self, raw_datastore: DataStore, timezone: ZoneInfo
     ) -> None:
-        send, receive = create_memory_object_stream[Event](3)
+        send, receive = create_memory_object_stream[Event](5)
         async with AsyncScheduler(data_store=raw_datastore) as scheduler:
             scheduler.subscribe(send.send)
             now = datetime.now(timezone)
             trigger = DateTrigger(now)
             schedule_id = await scheduler.add_schedule(
                 dummy_async_job, trigger, id="foo"
             )
             assert schedule_id == "foo"
 
             schedules = await scheduler.get_schedules()
             assert len(schedules) == 1
             assert schedules[0].id == "foo"
             assert schedules[0].task_id == f"{__name__}:dummy_async_job"
 
+            await scheduler.pause_schedule("foo")
+            schedule = await scheduler.get_schedule("foo")
+            assert schedule.paused
+            assert schedule.next_fire_time == now
+
+            await scheduler.unpause_schedule("foo")
+            schedule = await scheduler.get_schedule("foo")
+            assert not schedule.paused
+            assert schedule.next_fire_time == now
+
             await scheduler.remove_schedule(schedule_id)
             assert not await scheduler.get_schedules()
 
         with fail_after(3):
             event = await receive.receive()
             assert isinstance(event, TaskAdded)
             assert event.task_id == f"{__name__}:dummy_async_job"
@@ -220,14 +237,26 @@
             event = await receive.receive()
             assert isinstance(event, ScheduleAdded)
             assert event.schedule_id == "foo"
             assert event.task_id == f"{__name__}:dummy_async_job"
             assert event.next_fire_time == now
 
             event = await receive.receive()
+            assert isinstance(event, ScheduleUpdated)
+            assert event.schedule_id == "foo"
+            assert event.task_id == f"{__name__}:dummy_async_job"
+            assert event.next_fire_time == now
+
+            event = await receive.receive()
+            assert isinstance(event, ScheduleUpdated)
+            assert event.schedule_id == "foo"
+            assert event.task_id == f"{__name__}:dummy_async_job"
+            assert event.next_fire_time == now
+
+            event = await receive.receive()
             assert isinstance(event, ScheduleRemoved)
             assert event.schedule_id == "foo"
             assert event.task_id == f"{__name__}:dummy_async_job"
             assert not event.finished
 
     async def test_add_job_wait_result(self, raw_datastore: DataStore) -> None:
         send, receive = create_memory_object_stream[Event](2)
@@ -259,18 +288,26 @@
             with fail_after(3):
                 event = await receive.receive()
                 assert isinstance(event, SchedulerStarted)
 
                 event = await receive.receive()
                 assert isinstance(event, JobAcquired)
                 assert event.job_id == job_id
+                assert event.task_id == f"{__name__}:dummy_async_job"
+                assert event.schedule_id is None
+                assert event.scheduled_start is None
+                acquired_at = event.timestamp
 
                 event = await receive.receive()
                 assert isinstance(event, JobReleased)
                 assert event.job_id == job_id
+                assert event.task_id == f"{__name__}:dummy_async_job"
+                assert event.schedule_id is None
+                assert event.scheduled_start is None
+                assert event.started_at >= acquired_at
                 assert event.outcome is JobOutcome.success
 
                 result = await scheduler.get_job_result(job_id)
                 assert result.outcome is JobOutcome.success
                 assert result.return_value == "returnvalue"
 
     @pytest.mark.parametrize("success", [True, False])
@@ -302,20 +339,28 @@
                 job_id = event.job_id
                 assert event.task_id == f"{__name__}:dummy_async_job"
 
                 # The scheduler acquired the job
                 event = await receive.receive()
                 assert isinstance(event, JobAcquired)
                 assert event.job_id == job_id
+                assert event.task_id == f"{__name__}:dummy_async_job"
+                assert event.schedule_id is None
+                assert event.scheduled_start is None
                 assert event.scheduler_id == scheduler.identity
+                acquired_at = event.timestamp
 
                 # The scheduler released the job
                 event = await receive.receive()
                 assert isinstance(event, JobReleased)
                 assert event.job_id == job_id
+                assert event.task_id == f"{__name__}:dummy_async_job"
+                assert event.schedule_id is None
+                assert event.scheduled_start is None
+                assert event.started_at >= acquired_at
                 assert event.scheduler_id == scheduler.identity
 
         # The scheduler was stopped
         event = await receive.receive()
         assert isinstance(event, SchedulerStopped)
 
         # There should be no more events on the list
@@ -383,16 +428,16 @@
                 assert result.outcome is JobOutcome.success
                 assert result.return_value == expected_result
 
     async def test_scheduled_job_missed_deadline(
         self, raw_datastore: DataStore, timezone: ZoneInfo
     ) -> None:
         send, receive = create_memory_object_stream[Event](4)
-        now = datetime.now(timezone)
-        trigger = DateTrigger(now)
+        one_second_in_past = datetime.now(timezone) - timedelta(seconds=1)
+        trigger = DateTrigger(one_second_in_past)
         async with AsyncScheduler(data_store=raw_datastore) as scheduler:
             await scheduler.add_schedule(
                 dummy_async_job, trigger, misfire_grace_time=0, id="foo"
             )
             scheduler.subscribe(send.send)
             await scheduler.start_in_background()
 
@@ -403,31 +448,35 @@
 
                 # The schedule was processed and a job was added for it
                 event = await receive.receive()
                 assert isinstance(event, JobAdded)
                 assert event.schedule_id == "foo"
                 assert event.task_id == "test_schedulers:dummy_async_job"
 
-                # The schedule was removed since the trigger had been exhausted
+                # The schedule was updated with a null next fire time
                 event = await receive.receive()
-                assert isinstance(event, ScheduleRemoved)
+                assert isinstance(event, ScheduleUpdated)
                 assert event.schedule_id == "foo"
-                assert event.finished
+                assert event.next_fire_time is None
 
                 # The new job was acquired
                 event = await receive.receive()
                 assert isinstance(event, JobAcquired)
                 job_id = event.job_id
-                # assert event.schedule_id == "foo"
-                # assert event.task_id == "test_schedulers:dummy_async_job"
+                assert event.task_id == "test_schedulers:dummy_async_job"
+                assert event.schedule_id == "foo"
 
                 # The new job was released
                 event = await receive.receive()
                 assert isinstance(event, JobReleased)
                 assert event.job_id == job_id
+                assert event.task_id == "test_schedulers:dummy_async_job"
+                assert event.schedule_id == "foo"
+                assert event.scheduled_start == one_second_in_past
+                assert event.started_at is None
                 assert event.outcome is JobOutcome.missed_start_deadline
 
         # The scheduler was stopped
         event = await receive.receive()
         assert isinstance(event, SchedulerStopped)
 
         # There should be no more events on the list
@@ -458,15 +507,17 @@
         timezone: ZoneInfo,
     ) -> None:
         send, receive = create_memory_object_stream[Event](4)
         now = datetime.now(timezone)
         first_start_time = now - timedelta(minutes=3, seconds=5)
         trigger = IntervalTrigger(minutes=1, start_time=first_start_time)
         async with AsyncScheduler(
-            data_store=raw_datastore, role=SchedulerRole.scheduler
+            data_store=raw_datastore,
+            role=SchedulerRole.scheduler,
+            cleanup_interval=None,
         ) as scheduler:
             await scheduler.add_schedule(
                 dummy_async_job, trigger, id="foo", coalesce=coalesce
             )
             scheduler.subscribe(send.send)
             await scheduler.start_in_background()
 
@@ -516,15 +567,16 @@
     ) -> None:
         send, receive = create_memory_object_stream[Event](4)
         jitter = 1.569374
         now = datetime.now(timezone)
         fake_uniform = mocker.patch("random.uniform")
         fake_uniform.configure_mock(side_effect=lambda a, b: jitter)
         async with AsyncScheduler(
-            data_store=raw_datastore, role=SchedulerRole.scheduler
+            data_store=raw_datastore,
+            role=SchedulerRole.scheduler,
         ) as scheduler:
             scheduler.subscribe(send.send)
             trigger = DateTrigger(now)
             schedule_id = await scheduler.add_schedule(
                 dummy_async_job, trigger, id="foo", max_jitter=max_jitter
             )
             schedule = await scheduler.get_schedule(schedule_id)
@@ -590,18 +642,22 @@
                 event = await receive.receive()
                 assert isinstance(event, JobAdded)
                 assert event.job_id == job_id
 
                 event = await receive.receive()
                 assert isinstance(event, JobAcquired)
                 assert event.job_id == job_id
+                assert event.task_id == "test_schedulers:dummy_async_job"
+                assert event.schedule_id is None
 
                 event = await receive.receive()
                 assert isinstance(event, JobReleased)
                 assert event.job_id == job_id
+                assert event.task_id == "test_schedulers:dummy_async_job"
+                assert event.schedule_id is None
 
             with pytest.raises(JobLookupError):
                 await scheduler.get_job_result(job_id, wait=False)
 
     async def test_add_job_get_result_error(self) -> None:
         async with AsyncScheduler() as scheduler:
             job_id = await scheduler.add_job(
@@ -666,24 +722,165 @@
             await scheduler.start_in_background()
 
             with fail_after(3):
                 event = await receive.receive()
 
             assert event.outcome is JobOutcome.success
 
+    async def test_explicit_cleanup(self, raw_datastore: DataStore) -> None:
+        send, receive = create_memory_object_stream[Event](1)
+        async with AsyncScheduler(raw_datastore, cleanup_interval=None) as scheduler:
+            scheduler.subscribe(send.send, {ScheduleRemoved})
+            event = anyio.Event()
+            scheduler.subscribe(lambda _: event.set(), {JobReleased}, one_shot=True)
+            await scheduler.start_in_background()
+
+            # Add a job whose result expires after 1 ms
+            job_id = await scheduler.add_job(
+                dummy_async_job, result_expiration_time=0.001
+            )
+            with fail_after(3):
+                await event.wait()
+
+            # After the sleeping past the expiration time and performing a cleanup, the
+            # result should not be there anymore
+            await sleep(0.001)
+            await scheduler.cleanup()
+            with pytest.raises(JobLookupError):
+                await scheduler.get_job_result(job_id)
+
+            # Add a schedule to immediately set the event
+            event = anyio.Event()
+            scheduler.subscribe(lambda _: event.set(), {JobReleased}, one_shot=True)
+            await scheduler.add_schedule(
+                dummy_async_job, DateTrigger(datetime.now(timezone.utc)), id="event_set"
+            )
+            with fail_after(3):
+                await event.wait()
+
+            # The schedule should still be around, but with a null next_fire_time
+            schedule = await scheduler.get_schedule("event_set")
+            assert schedule.next_fire_time is None
+
+            # After the cleanup, the schedule should be gone
+            await scheduler.cleanup()
+            with pytest.raises(ScheduleLookupError):
+                await scheduler.get_schedule("event_set")
+
+            # Check that the corresponding event was received
+            with fail_after(3):
+                event = await receive.receive()
+                assert isinstance(event, ScheduleRemoved)
+                assert event.schedule_id == schedule.id
+                assert event.finished
+
+    async def test_explicit_cleanup_avoid_schedules_still_having_jobs(
+        self, raw_datastore: DataStore
+    ) -> None:
+        send, receive = create_memory_object_stream[Event](4)
+        async with AsyncScheduler(raw_datastore, cleanup_interval=None) as scheduler:
+            scheduler.subscribe(send.send, {ScheduleUpdated, JobAdded, JobReleased})
+            await scheduler.start_in_background()
+
+            # Add a schedule to immediately set the event
+            dummy_event = anyio.Event()
+            await scheduler.configure_task("event_set", func=dummy_event.wait)
+            schedule_id = await scheduler.add_schedule(
+                "event_set", DateTrigger(datetime.now(timezone.utc)), id="event_set"
+            )
+
+            # Wait for the job to be submitted
+            event = await receive.receive()
+            assert isinstance(event, JobAdded)
+            assert event.schedule_id == schedule_id
+
+            # Wait for the schedule to be updated
+            event = await receive.receive()
+            assert isinstance(event, ScheduleUpdated)
+            assert event.schedule_id == schedule_id
+            assert event.next_fire_time is None
+
+            # Check that there is a job for the schedule
+            jobs = await scheduler.get_jobs()
+            assert len(jobs) == 1
+            assert jobs[0].schedule_id == schedule_id
+
+            # After the cleanup, the schedule should still be around, with a
+            # null next_fire_time
+            await scheduler.cleanup()
+            schedule = await scheduler.get_schedule("event_set")
+            assert schedule.next_fire_time is None
+
+            # Wait for the job to finish
+            dummy_event.set()
+            event = await receive.receive()
+            assert isinstance(event, JobReleased)
+
+    async def test_implicit_cleanup(self, mocker: MockerFixture) -> None:
+        """
+        Test that the scheduler's cleanup() method is called when the scheduler is
+        started.
+
+        """
+        async with AsyncScheduler() as scheduler:
+            event = anyio.Event()
+            mocker.patch.object(scheduler.data_store, "cleanup", side_effect=event.set)
+            await scheduler.start_in_background()
+            with fail_after(3):
+                await event.wait()
+
     async def test_wait_until_stopped(self) -> None:
         async with AsyncScheduler() as scheduler:
             await scheduler.add_job(scheduler.stop)
             await scheduler.wait_until_stopped()
 
         # This should be a no-op
         await scheduler.wait_until_stopped()
 
+    async def test_max_concurrent_jobs(self) -> None:
+        lock = Lock()
+        scheduler = AsyncScheduler(max_concurrent_jobs=1)
+        tasks_done = 0
+
+        async def acquire_release() -> None:
+            nonlocal tasks_done
+            lock.acquire_nowait()
+            await sleep(0.1)
+            tasks_done += 1
+            if tasks_done == 2:
+                await scheduler.stop()
+
+            lock.release()
+
+        with fail_after(3):
+            async with scheduler:
+                await scheduler.configure_task("dummyjob", func=acquire_release)
+                await scheduler.add_job("dummyjob")
+                await scheduler.add_job("dummyjob")
+                await scheduler.run_until_stopped()
+
 
 class TestSyncScheduler:
+    def test_configure(self) -> None:
+        executor = ThreadPoolJobExecutor()
+        scheduler = Scheduler(
+            identity="identity",
+            role=SchedulerRole.scheduler,
+            max_concurrent_jobs=150,
+            cleanup_interval=5,
+            job_executors={"executor1": executor},
+            default_job_executor="executor1",
+        )
+        assert scheduler.identity == "identity"
+        assert scheduler.role is SchedulerRole.scheduler
+        assert scheduler.max_concurrent_jobs == 150
+        assert scheduler.cleanup_interval == timedelta(seconds=5)
+        assert scheduler.job_executors == {"executor1": executor}
+        assert scheduler.default_job_executor == "executor1"
+
     @pytest.mark.parametrize("as_default", [False, True])
     def test_threadpool_executor(self, as_default: bool) -> None:
         with Scheduler() as scheduler:
             scheduler.start_in_background()
             if as_default:
                 thread_id = scheduler.run_job(threading.get_ident)
             else:
@@ -808,18 +1005,22 @@
 
             event = queue.get(timeout=1)
             assert isinstance(event, SchedulerStarted)
 
             event = queue.get(timeout=1)
             assert isinstance(event, JobAcquired)
             assert event.job_id == job_id
+            assert event.task_id == f"{__name__}:dummy_sync_job"
+            assert event.schedule_id is None
 
             event = queue.get(timeout=1)
             assert isinstance(event, JobReleased)
             assert event.job_id == job_id
+            assert event.task_id == f"{__name__}:dummy_sync_job"
+            assert event.schedule_id is None
             assert event.outcome is JobOutcome.success
 
             result = scheduler.get_job_result(job_id)
             assert result.outcome is JobOutcome.success
             assert result.return_value == "returnvalue"
 
     def test_wait_until_stopped(self) -> None:
@@ -839,14 +1040,32 @@
 
         event = queue.get(timeout=1)
         assert isinstance(event, JobReleased)
 
         event = queue.get(timeout=1)
         assert isinstance(event, SchedulerStopped)
 
+    def test_explicit_cleanup(self) -> None:
+        with Scheduler(cleanup_interval=None) as scheduler:
+            event = threading.Event()
+            scheduler.add_schedule(
+                event.set, DateTrigger(datetime.now(timezone.utc)), id="event_set"
+            )
+            scheduler.start_in_background()
+            assert event.wait(3)
+
+            # The schedule should still be around, but with a null next_fire_time
+            schedule = scheduler.get_schedule("event_set")
+            assert schedule.next_fire_time is None
+
+            # After the cleanup, the schedule should be gone
+            scheduler.cleanup()
+            with pytest.raises(ScheduleLookupError):
+                scheduler.get_schedule("event_set")
+
     def test_run_until_stopped(self) -> None:
         queue = Queue()
         with Scheduler() as scheduler:
             scheduler.configure_task("stop", func=scheduler.stop)
             scheduler.add_job("stop")
             scheduler.subscribe(queue.put_nowait)
             scheduler.run_until_stopped()
```

### Comparing `APScheduler-4.0.0a4/tests/triggers/test_calendarinterval.py` & `apscheduler-4.0.0a5/tests/triggers/test_calendarinterval.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,18 +68,19 @@
 
 
 def test_nonexistent_days(timezone, serializer):
     """Test that invalid dates are skipped."""
     trigger = CalendarIntervalTrigger(
         months=1, start_date=date(2016, 3, 31), timezone=timezone
     )
+    assert trigger.next() == datetime(2016, 3, 31, tzinfo=timezone)
+
     if serializer:
         trigger = serializer.deserialize(serializer.serialize(trigger))
 
-    assert trigger.next() == datetime(2016, 3, 31, tzinfo=timezone)
     assert trigger.next() == datetime(2016, 5, 31, tzinfo=timezone)
 
 
 def test_repr(timezone, serializer):
     trigger = CalendarIntervalTrigger(
         years=1,
         months=5,
@@ -95,7 +96,14 @@
         trigger = serializer.deserialize(serializer.serialize(trigger))
 
     assert repr(trigger) == (
         "CalendarIntervalTrigger(years=1, months=5, weeks=6, days=8, "
         "time='03:00:08', start_date='2016-03-05', end_date='2020-12-25', "
         "timezone='Europe/Berlin')"
     )
+
+
+def test_utc_timezone(utc_timezone):
+    trigger = CalendarIntervalTrigger(
+        days=1, hour=1, start_date=date(2016, 3, 31), timezone=utc_timezone
+    )
+    assert trigger.next() == datetime(2016, 3, 31, 1, tzinfo=utc_timezone)
```

### Comparing `APScheduler-4.0.0a4/tests/triggers/test_cron.py` & `apscheduler-4.0.0a5/tests/triggers/test_cron.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def test_invalid_expression():
     exc = pytest.raises(ValueError, CronTrigger, year="2009-fault")
     exc.match("Unrecognized expression '2009-fault' for field 'year'")
 
 
 def test_invalid_step():
     exc = pytest.raises(ValueError, CronTrigger, year="2009/0")
-    exc.match("Step must be higher than 0")
+    exc.match("step must be positive, got: 0")
 
 
 def test_invalid_range():
     exc = pytest.raises(ValueError, CronTrigger, year="2009-2008")
     exc.match("The minimum value in a range must not be higher than the maximum")
 
 
@@ -85,18 +85,22 @@
     trigger = CronTrigger(
         year="2009/2",
         month="1-4/3",
         day="5-6",
         start_time=start_time,
         timezone=timezone,
     )
+
+    # since `next` is modifying the trigger, we call it before serializing
+    # to make sure the serialization works correctly also for modified triggers
+    assert trigger.next() == datetime(2009, 1, 5, tzinfo=timezone)
+
     if serializer:
         trigger = serializer.deserialize(serializer.serialize(trigger))
 
-    assert trigger.next() == datetime(2009, 1, 5, tzinfo=timezone)
     assert trigger.next() == datetime(2009, 1, 6, tzinfo=timezone)
     assert trigger.next() == datetime(2009, 4, 5, tzinfo=timezone)
     assert trigger.next() == datetime(2009, 4, 6, tzinfo=timezone)
     assert trigger.next() == datetime(2011, 1, 5, tzinfo=timezone)
     assert repr(trigger) == (
         "CronTrigger(year='2009/2', month='1-4/3', day='5-6', week='*', "
         "day_of_week='*', hour='0', minute='0', second='0', "
```

### Comparing `APScheduler-4.0.0a4/tests/triggers/test_date.py` & `apscheduler-4.0.0a5/tests/triggers/test_date.py`

 * *Files identical despite different names*

### Comparing `APScheduler-4.0.0a4/tests/triggers/test_interval.py` & `apscheduler-4.0.0a5/tests/triggers/test_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 def test_end_time(timezone, serializer):
     start_time = datetime(2020, 5, 16, 19, 32, 44, 649521, tzinfo=timezone)
     end_time = datetime(2020, 5, 16, 22, 33, 1, tzinfo=timezone)
     interval = timedelta(hours=1, seconds=6)
     trigger = IntervalTrigger(
         start_time=start_time, end_time=end_time, hours=1, seconds=6
     )
+    assert trigger.next() == start_time
+
     if serializer:
         trigger = serializer.deserialize(serializer.serialize(trigger))
 
-    assert trigger.next() == start_time
     assert trigger.next() == start_time + interval
     assert trigger.next() == start_time + interval * 2
     assert trigger.next() is None
 
 
 def test_repr(timezone, serializer):
     start_time = datetime(2020, 5, 15, 12, 55, 32, 954032, tzinfo=timezone)
```

### Comparing `APScheduler-4.0.0a4/tools/dockerize` & `apscheduler-4.0.0a5/tools/dockerize`

 * *Files identical despite different names*

