# Comparing `tmp/rockai_cli_app-0.2.1.tar.gz` & `tmp/rockai_cli_app-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.1.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.2.tar", max compression
```

## Comparing `rockai_cli_app-0.2.1.tar` & `rockai_cli_app-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      128 2024-05-06 14:26:16.307703 rockai_cli_app-0.2.1/README.md
--rw-r--r--   0        0        0      601 2024-05-11 15:41:21.522167 rockai_cli_app-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309243 rockai_cli_app-0.2.1/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.1/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.1/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.1/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.1/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.1/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.1/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.1/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.1/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.1/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.1/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.1/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.1/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.1/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.1/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.1/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.1/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.1/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.1/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      703 2024-05-06 14:26:16.311710 rockai_cli_app-0.2.1/rockai_cli_app/test.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      128 2024-05-06 14:26:16.307703 rockai_cli_app-0.2.2/README.md
+-rw-r--r--   0        0        0      714 2024-05-16 07:23:30.863623 rockai_cli_app-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7636 2024-05-16 07:23:20.518516 rockai_cli_app-0.2.2/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-16 02:40:27.277757 rockai_cli_app-0.2.2/rockai_cli_app/constant.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.2/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.2/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.2/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.2/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.2/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.2/rockai_cli_app/main.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.2/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.2/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.2/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.2/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.2/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.2/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.2/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.2/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.2/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.2/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.2/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.2/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      703 2024-05-06 14:26:16.311710 rockai_cli_app-0.2.2/rockai_cli_app/test.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.2/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.1/pyproject.toml` & `rockai_cli_app-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.1"
+version = "0.2.2"
 description = "For inference and training"
 authors = ["Rocky <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {extras = ["all"], version = "^0.9.0"}
 fastapi = "^0.109.2"
 uvicorn = {extras = ["standard"], version = "^0.27.0.post1"}
 requests = "^2.31.0"
+sseclient = "^0.0.27"
+httpx = "^0.27.0"
+httpx-sse = "0.1.0"
+aiosseclient = "^0.1.3"
+aiohttp-sse-client = "0.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.2/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.2/rockai_cli_app/docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.2.2/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.2/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/main.py` & `rockai_cli_app-0.2.2/rockai_cli_app/main.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.2/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.2/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.2/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.2/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.2/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/rockai_cli_app/test.py` & `rockai_cli_app-0.2.2/rockai_cli_app/test.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.1/PKG-INFO` & `rockai_cli_app-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.2.1
+Version: 0.2.2
 Summary: For inference and training
 Author: Rocky
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp-sse-client (==0.2.1)
+Requires-Dist: aiosseclient (>=0.1.3,<0.2.0)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: httpx-sse (==0.1.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sseclient (>=0.0.27,<0.0.28)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn[standard] (>=0.27.0.post1,<0.28.0)
 Description-Content-Type: text/markdown
 
 # setup
 python 3.11.5, use this version when developing
 ```
```

