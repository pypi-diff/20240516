# Comparing `tmp/sapx-0.2.8.tar.gz` & `tmp/sapx-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapx-0.2.8.tar", last modified: Wed May  8 09:22:52 2024, max compression
+gzip compressed data, was "sapx-0.2.9.tar", last modified: Wed May  8 13:31:31 2024, max compression
```

## Comparing `sapx-0.2.8.tar` & `sapx-0.2.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 09:22:52.033253 sapx-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 09:22:45.000000 sapx-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-08 09:22:45.000000 sapx-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/beanie/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/document.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/beanie/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.025253 sapx-0.2.8/sap/chart/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/chart/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/fastapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/pydantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/rest/rest_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/crons.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/typing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.029253 sapx-0.2.8/sap/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/amqp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/crons_airtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/lambdas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 09:22:45.000000 sapx-0.2.8/sap/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/sapx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 09:22:52.000000 sapx-0.2.8/sapx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:22:52.033253 sapx-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 09:22:45.000000 sapx-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:22:52.033253 sapx-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-08 09:22:45.000000 sapx-0.2.8/tests/test_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.514579 sapx-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 13:31:31.514579 sapx-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 13:31:23.000000 sapx-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-08 13:31:23.000000 sapx-0.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.506579 sapx-0.2.9/sap/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.506579 sapx-0.2.9/sap/beanie/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/beanie/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.506579 sapx-0.2.9/sap/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/chart/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.510579 sapx-0.2.9/sap/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/fastapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.510579 sapx-0.2.9/sap/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/pydantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.510579 sapx-0.2.9/sap/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/rest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/rest/rest_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.510579 sapx-0.2.9/sap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/tests/crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/tests/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.510579 sapx-0.2.9/sap/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/typing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.514579 sapx-0.2.9/sap/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/amqp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/crons_airtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/lambdas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-08 13:31:23.000000 sapx-0.2.9/sap/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.514579 sapx-0.2.9/sapx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-08 13:31:31.000000 sapx-0.2.9/sapx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 13:31:31.000000 sapx-0.2.9/sapx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:31:31.000000 sapx-0.2.9/sapx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 13:31:31.000000 sapx-0.2.9/sapx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 13:31:31.000000 sapx-0.2.9/sapx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:31:31.514579 sapx-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 13:31:23.000000 sapx-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:31:31.514579 sapx-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-08 13:31:23.000000 sapx-0.2.9/tests/test_rest_client.py
```

### Comparing `sapx-0.2.8/PKG-INFO` & `sapx-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.2.8/pyproject.toml` & `sapx-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/client.py` & `sapx-0.2.9/sap/beanie/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/document.py` & `sapx-0.2.9/sap/beanie/document.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/link.py` & `sapx-0.2.9/sap/beanie/link.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/mixins.py` & `sapx-0.2.9/sap/beanie/mixins.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/patch.py` & `sapx-0.2.9/sap/beanie/patch.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/beanie/query.py` & `sapx-0.2.9/sap/beanie/query.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/chart/serializers.py` & `sapx-0.2.9/sap/chart/serializers.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/__init__.py` & `sapx-0.2.9/sap/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/auth.py` & `sapx-0.2.9/sap/fastapi/auth.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/exceptions.py` & `sapx-0.2.9/sap/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/forms.py` & `sapx-0.2.9/sap/fastapi/forms.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/middleware.py` & `sapx-0.2.9/sap/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/pagination.py` & `sapx-0.2.9/sap/fastapi/pagination.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/serializers.py` & `sapx-0.2.9/sap/fastapi/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
             # A: An explicit method was declared to retrieve the value
             if hasattr(cls, f"get_{field_name}"):
                 return getattr(cls, f"get_{field_name}")(instance=instance)
 
             related_object = getattr(instance, field_name, None)
 
-            origin = get_origin(field_info.annotation)
+            origin = get_origin(field_info.annotation) or field_info.annotation
             args = get_args(field_info.annotation)
 
             # B. The field is an embedded serializer
             if inspect.isclass(origin) and issubclass(origin, ObjectSerializer):
                 return origin.read(related_object, exclude=exclude) if related_object else None
 
             # C. The field is a list of embedded serializer or optional
```

### Comparing `sapx-0.2.8/sap/fastapi/user.py` & `sapx-0.2.9/sap/fastapi/user.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/fastapi/utils.py` & `sapx-0.2.9/sap/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/rest/client.py` & `sapx-0.2.9/sap/rest/client.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/rest/rest_exceptions.py` & `sapx-0.2.9/sap/rest/rest_exceptions.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/settings.py` & `sapx-0.2.9/sap/settings.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/tests/crons.py` & `sapx-0.2.9/sap/tests/crons.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/tests/rest.py` & `sapx-0.2.9/sap/tests/rest.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/tests/utils.py` & `sapx-0.2.9/sap/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/__init__.py` & `sapx-0.2.9/sap/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/amqp.py` & `sapx-0.2.9/sap/worker/amqp.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/config.py` & `sapx-0.2.9/sap/worker/config.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/crons.py` & `sapx-0.2.9/sap/worker/crons.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/crons_airtable.py` & `sapx-0.2.9/sap/worker/crons_airtable.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/debug.py` & `sapx-0.2.9/sap/worker/debug.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/lambdas.py` & `sapx-0.2.9/sap/worker/lambdas.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/packet.py` & `sapx-0.2.9/sap/worker/packet.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sap/worker/utils.py` & `sapx-0.2.9/sap/worker/utils.py`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/sapx.egg-info/PKG-INFO` & `sapx-0.2.9/sapx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library of re-usable utilities for python web apps.
 Home-page: https://github.com/trellixio/sap
 Author: Trellix Dev
 Author-email: contact@trellix.io
 License: COPYRIGHT @ Trellix
 Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI
```

### Comparing `sapx-0.2.8/sapx.egg-info/SOURCES.txt` & `sapx-0.2.9/sapx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sapx-0.2.8/setup.py` & `sapx-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 setup(
     name="sapx",
     version=VERSION,
     packages=find_packages(include=("sap.*", "sap")),
     package_data={"sap": ["py.typed"]},
     include_package_data=True,
```

### Comparing `sapx-0.2.8/tests/test_rest_client.py` & `sapx-0.2.9/tests/test_rest_client.py`

 * *Files identical despite different names*

