# Comparing `tmp/pytest_aws_apigateway-0.5.0.tar.gz` & `tmp/pytest_aws_apigateway-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.5.0.tar", last modified: Wed May 15 17:55:14 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.5.1.tar", last modified: Thu May 16 16:02:26 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.5.0.tar` & `pytest_aws_apigateway-0.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.475822 pytest_aws_apigateway-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.475822 pytest_aws_apigateway-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_powertools.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.633358 pytest_aws_apigateway-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.625358 pytest_aws_apigateway-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.629358 pytest_aws_apigateway-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-16 16:02:26.633358 pytest_aws_apigateway-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.629358 pytest_aws_apigateway-0.5.1/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:02:26.633358 pytest_aws_apigateway-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.625358 pytest_aws_apigateway-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.629358 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.633358 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 16:02:26.000000 pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.629358 pytest_aws_apigateway-0.5.1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:26.633358 pytest_aws_apigateway-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/test_powertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 16:02:14.000000 pytest_aws_apigateway-0.5.1/tox.ini
```

### Comparing `pytest_aws_apigateway-0.5.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.5.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/CHANGELOG.md` & `pytest_aws_apigateway-0.5.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# pytest-aws-apigateway 0.5.1 (2024-05-16)
+
+No significant changes.
+
+
 # pytest-aws-apigateway 0.5.0 (2024-05-15)
 
 ### Features
 
 - `add_integration` now accepts "ANY" as a http method as a catch-all
 - `add_integration` now returns an `Integration` object with attributes for `resource`, `method` and `endpoint`
```

### Comparing `pytest_aws_apigateway-0.5.0/LICENSE` & `pytest_aws_apigateway-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/PKG-INFO` & `pytest_aws_apigateway-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.5.0
+Version: 0.5.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -37,36 +37,40 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 
 -----
 
 ## Rationale
 
-`pytest_aws_apigateway` is a pytest plugin to make testing AWS lambda integrations with API Gateway easier.
+`pytest_aws_apigateway` is a pytest plugin to make testing AWS Lambda integrations with AWS ApiGateway easier.
+It registers AWS Lambda function handlers as callbacks to requests made using `httpx` so you can test your
+REST API using HTTP requests.
 
+## Usage
 
-## Installation
-
-```console
-pip install pytest-aws-apigateway
-```
+### Add integrations
 
-## Usage
+`pytest-aws-apigateway` lets you register AWS Lambda function handlers to act just like AWS ApiGateway proxy
+integrations.
 
 ```python
-def test_root_resource(apigateway_mock: ApiGatewayMock):
-    def handler(event, context):
-        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
+import httpx
+from pytest_aws_apigateway import ApiGatewayMock
+
+
+def handler(event, context):
+    return {"statusCode": 200, "body": json.dumps({"message": "Hello World!"})}
 
+def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
-        assert resp.json() == {"body": "hello"}
+        assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.5.0/README.md` & `pytest_aws_apigateway-0.5.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 
 -----
 
 ## Rationale
 
-`pytest_aws_apigateway` is a pytest plugin to make testing AWS lambda integrations with API Gateway easier.
+`pytest_aws_apigateway` is a pytest plugin to make testing AWS Lambda integrations with AWS ApiGateway easier.
+It registers AWS Lambda function handlers as callbacks to requests made using `httpx` so you can test your
+REST API using HTTP requests.
 
+## Usage
 
-## Installation
-
-```console
-pip install pytest-aws-apigateway
-```
+### Add integrations
 
-## Usage
+`pytest-aws-apigateway` lets you register AWS Lambda function handlers to act just like AWS ApiGateway proxy
+integrations.
 
 ```python
-def test_root_resource(apigateway_mock: ApiGatewayMock):
-    def handler(event, context):
-        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
+import httpx
+from pytest_aws_apigateway import ApiGatewayMock
+
+
+def handler(event, context):
+    return {"statusCode": 200, "body": json.dumps({"message": "Hello World!"})}
 
+def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
-        assert resp.json() == {"body": "hello"}
+        assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.5.0/pyproject.toml` & `pytest_aws_apigateway-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/apigateway.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/context.py` & `pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/context.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/integration.py` & `pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.5.0
+Version: 0.5.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -37,36 +37,40 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-aws-apigateway.svg)](https://pypi.org/project/pytest-aws-apigateway)
 
 -----
 
 ## Rationale
 
-`pytest_aws_apigateway` is a pytest plugin to make testing AWS lambda integrations with API Gateway easier.
+`pytest_aws_apigateway` is a pytest plugin to make testing AWS Lambda integrations with AWS ApiGateway easier.
+It registers AWS Lambda function handlers as callbacks to requests made using `httpx` so you can test your
+REST API using HTTP requests.
 
+## Usage
 
-## Installation
-
-```console
-pip install pytest-aws-apigateway
-```
+### Add integrations
 
-## Usage
+`pytest-aws-apigateway` lets you register AWS Lambda function handlers to act just like AWS ApiGateway proxy
+integrations.
 
 ```python
-def test_root_resource(apigateway_mock: ApiGatewayMock):
-    def handler(event, context):
-        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
+import httpx
+from pytest_aws_apigateway import ApiGatewayMock
+
+
+def handler(event, context):
+    return {"statusCode": 200, "body": json.dumps({"message": "Hello World!"})}
 
+def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
-        assert resp.json() == {"body": "hello"}
+        assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.5.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/tasks/release.py` & `pytest_aws_apigateway-0.5.1/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/tests/test_apigateway.py` & `pytest_aws_apigateway-0.5.1/tests/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/tests/test_plugin.py` & `pytest_aws_apigateway-0.5.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.5.0/tests/test_powertools.py` & `pytest_aws_apigateway-0.5.1/tests/test_powertools.py`

 * *Files identical despite different names*

