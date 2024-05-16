# Comparing `tmp/dwave_sona_core-1.2.8.tar.gz` & `tmp/dwave_sona_core-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave_sona_core-1.2.8.tar", max compression
+gzip compressed data, was "dwave_sona_core-1.2.9.tar", max compression
```

## Comparing `dwave_sona_core-1.2.8.tar` & `dwave_sona_core-1.2.9.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0     1085 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.8/LICENSE
--rw-r--r--   0        0        0     2382 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.8/README.md
--rw-r--r--   0        0        0      755 2024-01-08 10:00:28.384751 dwave_sona_core-1.2.8/pyproject.toml
--rw-r--r--   0        0        0      308 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/__init__.py
--rw-r--r--   0        0        0       59 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/__main__.py
--rw-r--r--   0        0        0     1157 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/commands.py
--rw-r--r--   0        0        0       98 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/exceptions.py
--rw-r--r--   0        0        0     4124 2024-01-08 09:52:51.856623 dwave_sona_core-1.2.8/sona/core/inferencer.py
--rw-r--r--   0        0        0      155 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/__init__.py
--rw-r--r--   0        0        0      349 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/base.py
--rw-r--r--   0        0        0     1880 2024-01-08 09:50:36.655781 dwave_sona_core-1.2.8/sona/core/messages/context.py
--rw-r--r--   0        0        0     1269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/file.py
--rw-r--r--   0        0        0     1422 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/job.py
--rw-r--r--   0        0        0      353 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/result.py
--rw-r--r--   0        0        0      797 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/messages/state.py
--rw-r--r--   0        0        0      265 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/middlewares/__init__.py
--rw-r--r--   0        0        0      601 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/middlewares/base.py
--rw-r--r--   0        0        0     2269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/middlewares/supervisors.py
--rw-r--r--   0        0        0     2410 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/middlewares/tracer.py
--rw-r--r--   0        0        0      242 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/__init__.py
--rw-r--r--   0        0        0     2751 2024-01-08 09:59:34.870210 dwave_sona_core-1.2.8/sona/core/storages/base.py
--rw-r--r--   0        0        0      578 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/filters/audio.py
--rw-r--r--   0        0        0      629 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/local.py
--rw-r--r--   0        0        0      865 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/s3.py
--rw-r--r--   0        0        0      187 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/__init__.py
--rw-r--r--   0        0        0      294 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/base.py
--rw-r--r--   0        0        0     1246 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/gdrive.py
--rw-r--r--   0        0        0      796 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/http.py
--rw-r--r--   0        0        0      682 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/local.py
--rw-r--r--   0        0        0     1168 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/s3.py
--rw-r--r--   0        0        0      848 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/storages/sources/youtube.py
--rw-r--r--   0        0        0     2190 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/stream/inferencer.py
--rw-r--r--   0        0        0       61 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/stream/messages/__init__.py
--rw-r--r--   0        0        0      304 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/stream/messages/context.py
--rw-r--r--   0        0        0     1205 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/stream/messages/streamdata.py
--rw-r--r--   0        0        0     1029 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/core/stream/parsers/audio.py
--rw-r--r--   0        0        0     1778 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/settings.py
--rw-r--r--   0        0        0     1531 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/utils/common.py
--rw-r--r--   0        0        0      215 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/commands.py
--rw-r--r--   0        0        0       74 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/messages/__init__.py
--rw-r--r--   0        0        0      117 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/messages/requests.py
--rw-r--r--   0        0        0      172 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/messages/responses.py
--rw-r--r--   0        0        0     2962 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/rpc/handlers.py
--rw-r--r--   0        0        0      995 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/rpc/tracks.py
--rw-r--r--   0        0        0     4581 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/server.py
--rw-r--r--   0        0        0     8884 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/static/client.js
--rw-r--r--   0        0        0     3470 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/web/static/webrtc.html
--rw-r--r--   0        0        0        0 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/__init__.py
--rw-r--r--   0        0        0      948 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/commands.py
--rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/consumers/__init__.py
--rw-r--r--   0        0        0      223 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/consumers/base.py
--rw-r--r--   0        0        0     1112 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/consumers/kafka.py
--rw-r--r--   0        0        0     1299 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/consumers/redis.py
--rw-r--r--   0        0        0     1021 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/consumers/sqs.py
--rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/producers/__init__.py
--rw-r--r--   0        0        0      131 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/producers/base.py
--rw-r--r--   0        0        0      651 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/producers/kafka.py
--rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/producers/redis.py
--rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/producers/sqs.py
--rw-r--r--   0        0        0     2780 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.8/sona/worker/workers.py
--rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 dwave_sona_core-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.9/LICENSE
+-rw-r--r--   0        0        0     2382 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.9/README.md
+-rw-r--r--   0        0        0      814 2024-01-24 02:37:23.203903 dwave_sona_core-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/__init__.py
+-rw-r--r--   0        0        0       59 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/__main__.py
+-rw-r--r--   0        0        0     1157 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/commands.py
+-rw-r--r--   0        0        0       98 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/exceptions.py
+-rw-r--r--   0        0        0     4124 2024-01-08 09:52:51.856623 dwave_sona_core-1.2.9/sona/core/inferencer.py
+-rw-r--r--   0        0        0      155 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/__init__.py
+-rw-r--r--   0        0        0      349 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/base.py
+-rw-r--r--   0        0        0     1880 2024-01-08 09:50:36.655781 dwave_sona_core-1.2.9/sona/core/messages/context.py
+-rw-r--r--   0        0        0     1269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/file.py
+-rw-r--r--   0        0        0     1422 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/job.py
+-rw-r--r--   0        0        0      353 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/result.py
+-rw-r--r--   0        0        0      797 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/state.py
+-rw-r--r--   0        0        0      265 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/__init__.py
+-rw-r--r--   0        0        0      601 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/base.py
+-rw-r--r--   0        0        0     2269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/supervisors.py
+-rw-r--r--   0        0        0     2410 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/tracer.py
+-rw-r--r--   0        0        0      242 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/__init__.py
+-rw-r--r--   0        0        0      888 2024-01-10 03:09:17.675435 dwave_sona_core-1.2.9/sona/core/storages/azureblob.py
+-rw-r--r--   0        0        0     2751 2024-01-08 09:59:34.870210 dwave_sona_core-1.2.9/sona/core/storages/base.py
+-rw-r--r--   0        0        0      578 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/filters/audio.py
+-rw-r--r--   0        0        0      629 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/local.py
+-rw-r--r--   0        0        0      865 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/s3.py
+-rw-r--r--   0        0        0      187 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/__init__.py
+-rw-r--r--   0        0        0     1146 2024-01-10 03:09:03.015604 dwave_sona_core-1.2.9/sona/core/storages/sources/azureblob.py
+-rw-r--r--   0        0        0      294 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/base.py
+-rw-r--r--   0        0        0     1246 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/gdrive.py
+-rw-r--r--   0        0        0      796 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/http.py
+-rw-r--r--   0        0        0      682 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/local.py
+-rw-r--r--   0        0        0     1168 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/s3.py
+-rw-r--r--   0        0        0      848 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/youtube.py
+-rw-r--r--   0        0        0     2190 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/inferencer.py
+-rw-r--r--   0        0        0       61 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/__init__.py
+-rw-r--r--   0        0        0      304 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/context.py
+-rw-r--r--   0        0        0     1205 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/streamdata.py
+-rw-r--r--   0        0        0     1029 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/parsers/audio.py
+-rw-r--r--   0        0        0     1882 2024-01-10 03:08:43.279837 dwave_sona_core-1.2.9/sona/settings.py
+-rw-r--r--   0        0        0     1777 2024-01-24 02:34:26.628913 dwave_sona_core-1.2.9/sona/utils/common.py
+-rw-r--r--   0        0        0      215 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/commands.py
+-rw-r--r--   0        0        0       74 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/__init__.py
+-rw-r--r--   0        0        0      117 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/requests.py
+-rw-r--r--   0        0        0      172 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/responses.py
+-rw-r--r--   0        0        0     2962 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/rpc/handlers.py
+-rw-r--r--   0        0        0      995 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/rpc/tracks.py
+-rw-r--r--   0        0        0     4581 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/server.py
+-rw-r--r--   0        0        0     8884 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/static/client.js
+-rw-r--r--   0        0        0     3470 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/static/webrtc.html
+-rw-r--r--   0        0        0        0 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/__init__.py
+-rw-r--r--   0        0        0      948 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/commands.py
+-rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/__init__.py
+-rw-r--r--   0        0        0      223 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/base.py
+-rw-r--r--   0        0        0     1112 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/kafka.py
+-rw-r--r--   0        0        0     1299 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/redis.py
+-rw-r--r--   0        0        0     1021 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/sqs.py
+-rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/__init__.py
+-rw-r--r--   0        0        0      131 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/base.py
+-rw-r--r--   0        0        0      651 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/kafka.py
+-rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/redis.py
+-rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/sqs.py
+-rw-r--r--   0        0        0     2780 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/workers.py
+-rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 dwave_sona_core-1.2.9/PKG-INFO
```

### Comparing `dwave_sona_core-1.2.8/LICENSE` & `dwave_sona_core-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/README.md` & `dwave_sona_core-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/pyproject.toml` & `dwave_sona_core-1.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dwave-sona-core"
-version = "1.2.8"
+version = "1.2.9"
 description = ""
 authors = ["dwave-dev"]
 license = ""
 readme = "README.md"
 packages = [{include = "sona"}]
 
 [tool.poetry.dependencies]
@@ -22,14 +22,16 @@
 redis = "^5.0.1"
 aiortc = "^1.6.0"
 fastapi = "^0.108.0"
 uvicorn = "^0.25.0"
 opentelemetry-api = "^1.22.0"
 opentelemetry-sdk = "^1.21.0"
 opentelemetry-exporter-jaeger-thrift = "^1.21.0"
+azure-storage-blob = "^12.19.0"
+azure-identity = "^1.15.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.11.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dwave_sona_core-1.2.8/sona/core/commands.py` & `dwave_sona_core-1.2.9/sona/core/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/inferencer.py` & `dwave_sona_core-1.2.9/sona/core/inferencer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/messages/context.py` & `dwave_sona_core-1.2.9/sona/core/messages/context.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/messages/file.py` & `dwave_sona_core-1.2.9/sona/core/messages/file.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/messages/job.py` & `dwave_sona_core-1.2.9/sona/core/messages/job.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/messages/state.py` & `dwave_sona_core-1.2.9/sona/core/messages/state.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/middlewares/base.py` & `dwave_sona_core-1.2.9/sona/core/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/middlewares/supervisors.py` & `dwave_sona_core-1.2.9/sona/core/middlewares/supervisors.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/middlewares/tracer.py` & `dwave_sona_core-1.2.9/sona/core/middlewares/tracer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/base.py` & `dwave_sona_core-1.2.9/sona/core/storages/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/filters/audio.py` & `dwave_sona_core-1.2.9/sona/core/storages/filters/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/local.py` & `dwave_sona_core-1.2.9/sona/core/storages/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/s3.py` & `dwave_sona_core-1.2.9/sona/core/storages/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/sources/gdrive.py` & `dwave_sona_core-1.2.9/sona/core/storages/sources/gdrive.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/sources/http.py` & `dwave_sona_core-1.2.9/sona/core/storages/sources/http.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/sources/local.py` & `dwave_sona_core-1.2.9/sona/core/storages/sources/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/sources/s3.py` & `dwave_sona_core-1.2.9/sona/core/storages/sources/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/storages/sources/youtube.py` & `dwave_sona_core-1.2.9/sona/core/storages/sources/youtube.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/stream/inferencer.py` & `dwave_sona_core-1.2.9/sona/core/stream/inferencer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/stream/messages/streamdata.py` & `dwave_sona_core-1.2.9/sona/core/stream/messages/streamdata.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/core/stream/parsers/audio.py` & `dwave_sona_core-1.2.9/sona/core/stream/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/settings.py` & `dwave_sona_core-1.2.9/sona/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
     # Core Storage settings
     SONA_STORAGE_LOCAL_PATH: str = os.getcwd()
     SONA_STORAGE_S3_SETTING: Dict = dict()
     SONA_STORAGE_S3_BUCKET: str = "sona"
     SONA_SOURCE_GOOGLE_SERVICE_ACCOUNT_INFO: Optional[Dict] = None
 
+    SONA_STORAGE_AZURE_BLOB_SETTING: Dict = dict()
+    SONA_STORAGE_AZURE_BLOB_CONTAINER: str = "sona"
+
     # Worker base settings
     SONA_WORKER_CLASS: str = "sona.worker.workers.InferencerWorker"
     SONA_WORKER_TOPIC_PREFIX: str = "sona.inferencer."
 
     # Worker consumer settings
     SONA_WORKER_CONSUMER_SQS_SETTING: Optional[Dict] = None
     SONA_WORKER_CONSUMER_KAFKA_SETTING: Optional[Dict] = None
```

### Comparing `dwave_sona_core-1.2.8/sona/utils/common.py` & `dwave_sona_core-1.2.9/sona/utils/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import os
 import sys
 import traceback
 from pathlib import Path
 
 import av
+from loguru import logger
 
 
 def import_class(import_str):
     mod_str, _sep, class_str = import_str.rpartition(".")
     __import__(mod_str)
     try:
         return getattr(sys.modules[mod_str], class_str)
@@ -23,17 +24,22 @@
     in_path = str(filepath)
     out_path = str(filepath.parent / f"{filepath.stem}.{ext}")
 
     codec = "pcm_s16le" if ext == "wav" else ext
     with av.open(in_path, "r") as in_av:
         with av.open(out_path, "w") as out_av:
             out_stream = out_av.add_stream(codec)
-            for frame in in_av.decode(in_av.streams.audio[0]):
-                for packet in out_stream.encode(frame):
-                    out_av.mux(packet)
+            try:
+                for frame in in_av.decode(in_av.streams.audio[0]):
+                    for packet in out_stream.encode(frame):
+                        out_av.mux(packet)
+            except Exception as e:
+                logger.warning(
+                    f"Converting incomplete cause: {e}, inferencer may not process all of the audio data"
+                )
             for packet in out_stream.encode(None):
                 out_av.mux(packet)
     return out_path
 
 
 def zero_copy(in_fd, out_fd):
     ret = 0
```

### Comparing `dwave_sona_core-1.2.8/sona/web/rpc/handlers.py` & `dwave_sona_core-1.2.9/sona/web/rpc/handlers.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/web/rpc/tracks.py` & `dwave_sona_core-1.2.9/sona/web/rpc/tracks.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/web/server.py` & `dwave_sona_core-1.2.9/sona/web/server.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/web/static/client.js` & `dwave_sona_core-1.2.9/sona/web/static/client.js`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/web/static/webrtc.html` & `dwave_sona_core-1.2.9/sona/web/static/webrtc.html`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/commands.py` & `dwave_sona_core-1.2.9/sona/worker/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/consumers/__init__.py` & `dwave_sona_core-1.2.9/sona/worker/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/consumers/kafka.py` & `dwave_sona_core-1.2.9/sona/worker/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/consumers/redis.py` & `dwave_sona_core-1.2.9/sona/worker/consumers/redis.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/consumers/sqs.py` & `dwave_sona_core-1.2.9/sona/worker/consumers/sqs.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/producers/__init__.py` & `dwave_sona_core-1.2.9/sona/worker/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/producers/kafka.py` & `dwave_sona_core-1.2.9/sona/worker/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/sona/worker/workers.py` & `dwave_sona_core-1.2.9/sona/worker/workers.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.8/PKG-INFO` & `dwave_sona_core-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: dwave-sona-core
-Version: 1.2.8
+Version: 1.2.9
 Summary: 
 Author: dwave-dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiortc (>=1.6.0,<2.0.0)
 Requires-Dist: av (>=11.0.0,<12.0.0)
+Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
+Requires-Dist: azure-storage-blob (>=12.19.0,<13.0.0)
 Requires-Dist: boto3 (>=1.34.14,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.3.0,<3.0.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: google-api-python-client (>=2.112.0,<3.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger-thrift (>=1.21.0,<2.0.0)
```

