# Comparing `tmp/pytest_aws_apigateway-0.4.1.tar.gz` & `tmp/pytest_aws_apigateway-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.4.1.tar", last modified: Tue May 14 20:26:02 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.5.0.tar", last modified: Wed May 15 17:55:14 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.4.1.tar` & `pytest_aws_apigateway-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.982100 pytest_aws_apigateway-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.974100 pytest_aws_apigateway-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:26:02.982100 pytest_aws_apigateway-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.974100 pytest_aws_apigateway-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 20:26:02.000000 pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:26:02.978100 pytest_aws_apigateway-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 20:25:56.000000 pytest_aws_apigateway-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.475822 pytest_aws_apigateway-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.475822 pytest_aws_apigateway-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 17:55:14.000000 pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.479822 pytest_aws_apigateway-0.5.0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:14.483821 pytest_aws_apigateway-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_powertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-15 17:55:05.000000 pytest_aws_apigateway-0.5.0/tox.ini
```

### Comparing `pytest_aws_apigateway-0.4.1/.github/workflows/main.yml` & `pytest_aws_apigateway-0.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/LICENSE` & `pytest_aws_apigateway-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/PKG-INFO` & `pytest_aws_apigateway-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.4.1
+Version: 0.5.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.4.1/README.md` & `pytest_aws_apigateway-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/pyproject.toml` & `pytest_aws_apigateway-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/apigateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Union
 
 import httpx
 import pytest_httpx
 
 from pytest_aws_apigateway.context import LambdaContext
 from pytest_aws_apigateway.context import create_context
-from pytest_aws_apigateway.integration import IntegrationResponse
+from pytest_aws_apigateway.integration import Integration, IntegrationResponse
 from pytest_aws_apigateway.integration import ResponseFormatError
 from pytest_aws_apigateway.integration import build_integration_request
 from pytest_aws_apigateway.integration import transform_integration_response
 
 __all__ = ["ApiGatewayMock"]
 
 
@@ -26,21 +26,21 @@
 
     def add_integration(
         self,
         resource: str,
         method: str,
         endpoint: str,
         handler: Callable[[dict[str, Any], LambdaContext], IntegrationResponse],
-    ):
+    ) -> Integration:
         """
         Register an AWS Lambda function handler that will be called if a request matches.
 
         Args:
             resource: Resource path where to mount the integration. Will be combined with endpoint to match request URLs
-            method: HTTP method for which the integration should be called
+            method: HTTP method for which the integration should be called. Can be 'ANY' as a catch-all.
             endpoint: API endpoint for the API gateway. Example: 'http://localhost'
             handler: AWS Lambda handler function that will be called when a request matches
         """
         resource = self._normalize_resource(resource)
         endpoint = self._normalize_endpoint(endpoint)
 
         url = self._url_expression(endpoint, resource)
@@ -53,15 +53,21 @@
                 return transform_integration_response(resp)
             except ResponseFormatError:
                 return httpx.Response(
                     status_code=500,
                     json=json.dumps({"message": "Internal server error"}),
                 )
 
-        self.httpx_mock.add_callback(callback=integration, url=url, method=method)
+        method_to_match = method.upper()
+        if method_to_match == "ANY":
+            method_to_match = None
+        self.httpx_mock.add_callback(
+            callback=integration, url=url, method=method_to_match
+        )
+        return Integration(resource, method.upper(), endpoint)
 
     def _normalize_resource(self, resource: str) -> str:
         resource = resource.lstrip("/")
         resource = f"/{resource}"
         return resource
 
     def _url_expression(self, endpoint: str, resource: str) -> Union[re.Pattern, str]:
```

### Comparing `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/context.py` & `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/context.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway/integration.py` & `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway/integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     isBase64Encoded: bool
     statusCode: int
     headers: dict[str, str]
     multiValueHeaders: dict[str, list[str]]
     body: str
 
 
+class Integration:
+    def __init__(self, resource: str, method: str, endpoint: str) -> None:
+        self.resource = resource
+        self.method = method
+        self.endpoint = endpoint
+
+
 def build_integration_request(request: httpx.Request, resource: str) -> dict[str, Any]:
     # TODO isBase64Encoded depends on content-type header
 
     path = request.url.path
     path_parameters = _extract_path_parameters(path, resource)
 
     event = {
```

### Comparing `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.4.1
+Version: 0.5.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.4.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.5.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 src/pytest_aws_apigateway.egg-info/top_level.txt
 tasks/release.py
 tests/__init__.py
 tests/conftest.py
 tests/test_apigateway.py
 tests/test_integration.py
 tests/test_plugin.py
+tests/test_powertools.py
 tests/test_response.py
```

### Comparing `pytest_aws_apigateway-0.4.1/tasks/release.py` & `pytest_aws_apigateway-0.5.0/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.4.1/tests/test_apigateway.py` & `pytest_aws_apigateway-0.5.0/tests/test_apigateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,7 +64,20 @@
     apigateway_mock.add_integration(
         "/", handler=handler, method="GET", endpoint="https://some/"
     )
 
     with httpx.Client() as client:
         resp = client.get("https://some/")
         assert resp.status_code == 200
+
+
+def test_match_on_ANY_method(apigateway_mock: ApiGatewayMock):
+    def handler(event, context):
+        return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
+
+    apigateway_mock.add_integration(
+        "/", handler=handler, method="ANY", endpoint="https://some/"
+    )
+
+    with httpx.Client() as client:
+        resp = client.get("https://some/")
+        assert resp.json() == {"body": "hello"}
```

### Comparing `pytest_aws_apigateway-0.4.1/tests/test_plugin.py` & `pytest_aws_apigateway-0.5.0/tests/test_plugin.py`

 * *Files identical despite different names*

