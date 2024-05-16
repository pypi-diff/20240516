# Comparing `tmp/zaqar_tempest_plugin-1.8.0.tar.gz` & `tmp/zaqar_tempest_plugin-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaqar_tempest_plugin-1.8.0.tar", last modified: Thu Mar 21 10:13:40 2024, max compression
+gzip compressed data, was "zaqar_tempest_plugin-2.0.0.tar", last modified: Thu May 16 12:47:52 2024, max compression
```

## Comparing `zaqar_tempest_plugin-1.8.0.tar` & `zaqar_tempest_plugin-2.0.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.272129 zaqar_tempest_plugin-1.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2024-03-21 10:13:40.272129 zaqar_tempest_plugin-1.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.260128 zaqar_tempest_plugin-1.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.256127 zaqar_tempest_plugin-1.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/notes/drop-py-2-7-8a4da4bd0e7c36f5.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9275 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-03-21 10:13:40.272129 zaqar_tempest_plugin-1.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5027 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1/queues.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5479 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1_1/queues.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6585 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v2/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19855 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/json/messaging_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9672 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_queues.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.268129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4185 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4828 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2903 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_queues.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.272129 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5711 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20459 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_claims_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4821 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31336 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_messages_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6526 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9656 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_queues_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6594 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17090 2024-03-21 10:13:12.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_subscriptions_negative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:40.264128 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2564 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-03-21 10:13:40.000000 zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2643 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.419020 zaqar_tempest_plugin-2.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.419020 zaqar_tempest_plugin-2.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.419020 zaqar_tempest_plugin-2.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/notes/drop-py-2-7-8a4da4bd0e7c36f5.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9275 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5027 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1/queues.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5479 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1_1/queues.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6585 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v2/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19855 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/json/messaging_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9672 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_queues.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4185 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4828 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2903 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_queues.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.427019 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5711 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20459 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_claims_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4821 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31336 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_messages_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6526 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9656 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_queues_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6594 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17090 2024-05-16 12:47:21.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_subscriptions_negative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 12:47:52.423020 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1815 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2564 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-05-16 12:47:52.000000 zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/top_level.txt
```

### Comparing `zaqar_tempest_plugin-1.8.0/.zuul.yaml` & `zaqar_tempest_plugin-2.0.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/AUTHORS` & `zaqar_tempest_plugin-2.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/CONTRIBUTING.rst` & `zaqar_tempest_plugin-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/ChangeLog` & `zaqar_tempest_plugin-2.0.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 CHANGES
 =======
 
+2.0.0
+-----
+
+
 1.8.0
 -----
 
 * Remove six
 * zuul: Declare queue at top level
+* Update python classifier in setup.cfg
 * Update deprecated zuul syntax
 
 1.7.0
 -----
 
 * Migrate from testr to stestr
```

### Comparing `zaqar_tempest_plugin-1.8.0/LICENSE` & `zaqar_tempest_plugin-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/PKG-INFO` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: zaqar_tempest_plugin
-Version: 1.8.0
+Name: zaqar-tempest-plugin
+Version: 2.0.0
 Summary: Tempest plugin zaqar_tempest_plugin
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Zaqar Tempest Plugin
@@ -35,10 +35,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `zaqar_tempest_plugin-1.8.0/README.rst` & `zaqar_tempest_plugin-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/doc/source/conf.py` & `zaqar_tempest_plugin-2.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/doc/source/index.rst` & `zaqar_tempest_plugin-2.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/releasenotes/source/conf.py` & `zaqar_tempest_plugin-2.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/setup.cfg` & `zaqar_tempest_plugin-2.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	zaqar_tempest_plugin
 
 [entry_points]
 tempest.test_plugins =
```

### Comparing `zaqar_tempest_plugin-1.8.0/setup.py` & `zaqar_tempest_plugin-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/tox.ini` & `zaqar_tempest_plugin-2.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1/queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v1_1/queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v1_1/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/api_schema/response/v2/queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/api_schema/response/v2/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/config.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/plugin.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/services/messaging/json/messaging_client.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/services/messaging/json/messaging_client.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/base.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_claims.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_messages.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1/test_queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_claims.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_messages.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v1_1/test_queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v1_1/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_claims.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_claims_negative.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_claims_negative.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_messages.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_messages_negative.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_messages_negative.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_queues.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_queues_negative.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_queues_negative.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_subscriptions.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin/tests/v2/test_subscriptions_negative.py` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin/tests/v2/test_subscriptions_negative.py`

 * *Files identical despite different names*

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/PKG-INFO` & `zaqar_tempest_plugin-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: zaqar-tempest-plugin
-Version: 1.8.0
+Name: zaqar_tempest_plugin
+Version: 2.0.0
 Summary: Tempest plugin zaqar_tempest_plugin
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ====================
         Zaqar Tempest Plugin
@@ -35,10 +35,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
```

### Comparing `zaqar_tempest_plugin-1.8.0/zaqar_tempest_plugin.egg-info/SOURCES.txt` & `zaqar_tempest_plugin-2.0.0/zaqar_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

