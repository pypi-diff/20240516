# Comparing `tmp/dwave_sona_core-1.2.9.tar.gz` & `tmp/dwave_sona_core-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave_sona_core-1.2.9.tar", max compression
+gzip compressed data, was "dwave_sona_core-1.3.0.tar", max compression
```

## Comparing `dwave_sona_core-1.2.9.tar` & `dwave_sona_core-1.3.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1085 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.9/LICENSE
--rw-r--r--   0        0        0     2382 2024-01-08 09:33:15.595928 dwave_sona_core-1.2.9/README.md
--rw-r--r--   0        0        0      814 2024-01-24 02:37:23.203903 dwave_sona_core-1.2.9/pyproject.toml
--rw-r--r--   0        0        0      308 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/__init__.py
--rw-r--r--   0        0        0       59 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/__main__.py
--rw-r--r--   0        0        0     1157 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/commands.py
--rw-r--r--   0        0        0       98 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/exceptions.py
--rw-r--r--   0        0        0     4124 2024-01-08 09:52:51.856623 dwave_sona_core-1.2.9/sona/core/inferencer.py
--rw-r--r--   0        0        0      155 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/__init__.py
--rw-r--r--   0        0        0      349 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/base.py
--rw-r--r--   0        0        0     1880 2024-01-08 09:50:36.655781 dwave_sona_core-1.2.9/sona/core/messages/context.py
--rw-r--r--   0        0        0     1269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/file.py
--rw-r--r--   0        0        0     1422 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/job.py
--rw-r--r--   0        0        0      353 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/result.py
--rw-r--r--   0        0        0      797 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/messages/state.py
--rw-r--r--   0        0        0      265 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/__init__.py
--rw-r--r--   0        0        0      601 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/base.py
--rw-r--r--   0        0        0     2269 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/supervisors.py
--rw-r--r--   0        0        0     2410 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/middlewares/tracer.py
--rw-r--r--   0        0        0      242 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/__init__.py
--rw-r--r--   0        0        0      888 2024-01-10 03:09:17.675435 dwave_sona_core-1.2.9/sona/core/storages/azureblob.py
--rw-r--r--   0        0        0     2751 2024-01-08 09:59:34.870210 dwave_sona_core-1.2.9/sona/core/storages/base.py
--rw-r--r--   0        0        0      578 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/filters/audio.py
--rw-r--r--   0        0        0      629 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/local.py
--rw-r--r--   0        0        0      865 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/s3.py
--rw-r--r--   0        0        0      187 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/__init__.py
--rw-r--r--   0        0        0     1146 2024-01-10 03:09:03.015604 dwave_sona_core-1.2.9/sona/core/storages/sources/azureblob.py
--rw-r--r--   0        0        0      294 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/base.py
--rw-r--r--   0        0        0     1246 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/gdrive.py
--rw-r--r--   0        0        0      796 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/http.py
--rw-r--r--   0        0        0      682 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/local.py
--rw-r--r--   0        0        0     1168 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/s3.py
--rw-r--r--   0        0        0      848 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/storages/sources/youtube.py
--rw-r--r--   0        0        0     2190 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/inferencer.py
--rw-r--r--   0        0        0       61 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/__init__.py
--rw-r--r--   0        0        0      304 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/context.py
--rw-r--r--   0        0        0     1205 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/messages/streamdata.py
--rw-r--r--   0        0        0     1029 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/core/stream/parsers/audio.py
--rw-r--r--   0        0        0     1882 2024-01-10 03:08:43.279837 dwave_sona_core-1.2.9/sona/settings.py
--rw-r--r--   0        0        0     1777 2024-01-24 02:34:26.628913 dwave_sona_core-1.2.9/sona/utils/common.py
--rw-r--r--   0        0        0      215 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/commands.py
--rw-r--r--   0        0        0       74 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/__init__.py
--rw-r--r--   0        0        0      117 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/requests.py
--rw-r--r--   0        0        0      172 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/messages/responses.py
--rw-r--r--   0        0        0     2962 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/rpc/handlers.py
--rw-r--r--   0        0        0      995 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/rpc/tracks.py
--rw-r--r--   0        0        0     4581 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/server.py
--rw-r--r--   0        0        0     8884 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/static/client.js
--rw-r--r--   0        0        0     3470 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/web/static/webrtc.html
--rw-r--r--   0        0        0        0 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/__init__.py
--rw-r--r--   0        0        0      948 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/commands.py
--rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/__init__.py
--rw-r--r--   0        0        0      223 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/base.py
--rw-r--r--   0        0        0     1112 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/kafka.py
--rw-r--r--   0        0        0     1299 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/redis.py
--rw-r--r--   0        0        0     1021 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/consumers/sqs.py
--rw-r--r--   0        0        0      560 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/__init__.py
--rw-r--r--   0        0        0      131 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/base.py
--rw-r--r--   0        0        0      651 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/kafka.py
--rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/redis.py
--rw-r--r--   0        0        0      387 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/producers/sqs.py
--rw-r--r--   0        0        0     2780 2024-01-08 09:33:15.599928 dwave_sona_core-1.2.9/sona/worker/workers.py
--rw-r--r--   0        0        0     3659 1970-01-01 00:00:00.000000 dwave_sona_core-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-29 09:40:42.005779 dwave_sona_core-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2382 2024-04-29 09:40:42.017779 dwave_sona_core-1.3.0/README.md
+-rw-r--r--   0        0        0      965 2024-05-16 03:55:05.791865 dwave_sona_core-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/__main__.py
+-rw-r--r--   0        0        0     1157 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/commands.py
+-rw-r--r--   0        0        0       98 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/exceptions.py
+-rw-r--r--   0        0        0     4100 2024-05-07 11:17:04.856934 dwave_sona_core-1.3.0/sona/core/inferencer.py
+-rw-r--r--   0        0        0      155 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/messages/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-06 09:59:41.001325 dwave_sona_core-1.3.0/sona/core/messages/base.py
+-rw-r--r--   0        0        0     1892 2024-05-06 10:18:17.921108 dwave_sona_core-1.3.0/sona/core/messages/context.py
+-rw-r--r--   0        0        0     1283 2024-05-08 02:52:18.180538 dwave_sona_core-1.3.0/sona/core/messages/file.py
+-rw-r--r--   0        0        0     1422 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/messages/job.py
+-rw-r--r--   0        0        0      353 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/messages/result.py
+-rw-r--r--   0        0        0      797 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/messages/state.py
+-rw-r--r--   0        0        0      265 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/middlewares/__init__.py
+-rw-r--r--   0        0        0     1213 2024-05-07 08:30:52.602643 dwave_sona_core-1.3.0/sona/core/middlewares/base.py
+-rw-r--r--   0        0        0     6720 2024-05-14 09:50:06.983760 dwave_sona_core-1.3.0/sona/core/middlewares/supervisors.py
+-rw-r--r--   0        0        0     2410 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/middlewares/tracer.py
+-rw-r--r--   0        0        0      242 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/storages/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/storages/azureblob.py
+-rw-r--r--   0        0        0     2751 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/storages/base.py
+-rw-r--r--   0        0        0      578 2024-04-30 02:20:50.000477 dwave_sona_core-1.3.0/sona/core/storages/filters/audio.py
+-rw-r--r--   0        0        0      629 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/local.py
+-rw-r--r--   0        0        0      865 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/s3.py
+-rw-r--r--   0        0        0      187 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/azureblob.py
+-rw-r--r--   0        0        0      294 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/base.py
+-rw-r--r--   0        0        0     1246 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/gdrive.py
+-rw-r--r--   0        0        0      796 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/http.py
+-rw-r--r--   0        0        0      682 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/local.py
+-rw-r--r--   0        0        0     1168 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/storages/sources/s3.py
+-rw-r--r--   0        0        0      996 2024-04-30 02:20:52.580444 dwave_sona_core-1.3.0/sona/core/storages/sources/youtube.py
+-rw-r--r--   0        0        0     2127 2024-05-07 06:54:34.802357 dwave_sona_core-1.3.0/sona/core/stream/inferencer.py
+-rw-r--r--   0        0        0       61 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/stream/messages/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-07 06:57:28.323905 dwave_sona_core-1.3.0/sona/core/stream/messages/context.py
+-rw-r--r--   0        0        0     1205 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/stream/messages/streamdata.py
+-rw-r--r--   0        0        0     1029 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/core/stream/parsers/audio.py
+-rw-r--r--   0        0        0     2168 2024-05-16 03:54:31.891648 dwave_sona_core-1.3.0/sona/settings.py
+-rw-r--r--   0        0        0     2042 2024-05-08 02:50:46.586961 dwave_sona_core-1.3.0/sona/utils/common.py
+-rw-r--r--   0        0        0      215 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/web/commands.py
+-rw-r--r--   0        0        0       74 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/web/messages/__init__.py
+-rw-r--r--   0        0        0      117 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/web/messages/requests.py
+-rw-r--r--   0        0        0      172 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/web/messages/responses.py
+-rw-r--r--   0        0        0     3059 2024-05-07 08:44:44.758714 dwave_sona_core-1.3.0/sona/web/rpc/handlers.py
+-rw-r--r--   0        0        0      995 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/web/rpc/tracks.py
+-rw-r--r--   0        0        0     5083 2024-05-16 03:54:08.023494 dwave_sona_core-1.3.0/sona/web/server.py
+-rw-r--r--   0        0        0     9838 2024-05-07 08:23:11.503489 dwave_sona_core-1.3.0/sona/web/static/client.js
+-rw-r--r--   0        0        0     3714 2024-05-07 08:22:34.671622 dwave_sona_core-1.3.0/sona/web/static/webrtc.html
+-rw-r--r--   0        0        0        0 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/__init__.py
+-rw-r--r--   0        0        0      948 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/commands.py
+-rw-r--r--   0        0        0      560 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/consumers/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/consumers/base.py
+-rw-r--r--   0        0        0     1112 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/consumers/kafka.py
+-rw-r--r--   0        0        0     1299 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/consumers/redis.py
+-rw-r--r--   0        0        0     1021 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/consumers/sqs.py
+-rw-r--r--   0        0        0      560 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/producers/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/producers/base.py
+-rw-r--r--   0        0        0      651 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/producers/kafka.py
+-rw-r--r--   0        0        0      387 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/producers/redis.py
+-rw-r--r--   0        0        0      387 2024-04-30 02:20:50.004477 dwave_sona_core-1.3.0/sona/worker/producers/sqs.py
+-rw-r--r--   0        0        0     2834 2024-04-30 02:20:52.580444 dwave_sona_core-1.3.0/sona/worker/workers.py
+-rw-r--r--   0        0        0     3668 1970-01-01 00:00:00.000000 dwave_sona_core-1.3.0/PKG-INFO
```

### Comparing `dwave_sona_core-1.2.9/LICENSE` & `dwave_sona_core-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/README.md` & `dwave_sona_core-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/commands.py` & `dwave_sona_core-1.3.0/sona/core/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/inferencer.py` & `dwave_sona_core-1.3.0/sona/core/inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,16 @@
 class InferencerBase:
     name: str = "base"
     description: str = ""
     input_params_schema: BaseModel = None
     input_files_schema: BaseModel = DefaultInputFilesSchema
 
     def setup(self):
-        func = self.on_context
         for middleware in reversed(middlewares):
-            func = middleware(func)
-        self.on_context = func
+            middleware.setup(self)
 
     def on_context(self, ctx: Context) -> Context:
         storage = create_storage()
         try:
             logger.info(f"[{self.name}] recv: {ctx.to_message()}")
 
             # Prepare process data
@@ -107,14 +105,17 @@
             raise Exception(f"Unknown inferencer class: {import_str}")
         return _cls
 
     # Callbacks
     def on_load(self) -> None:
         return
 
+    def on_stop(self):
+        return
+
     @abc.abstractmethod
     def inference(self, params: Dict, files: List[File]) -> Result:
         return NotImplemented
 
     def context_example(self) -> Context:
         return None
```

### Comparing `dwave_sona_core-1.2.9/sona/core/messages/context.py` & `dwave_sona_core-1.3.0/sona/core/messages/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import time
 import uuid
 from typing import Dict, List
 
-from pydantic import Field, validator
+from pydantic import Field, field_validator
 
 from .base import MessageBase
 from .job import Job
 from .result import Result
 from .state import State
 
 
@@ -20,15 +20,15 @@
     supervisors: List[str] = []
     fallbacks: List[str] = []
     headers: Dict = {}
     jobs: List[Job]
     results: Dict[str, Result] = {}
     states: List[State] = []
 
-    @validator("jobs")
+    @field_validator("jobs")
     def uuique_jobs(cls, v: List[Job]):
         job_names = set()
         for job in v:
             assert (
                 job.name not in job_names
             ), f"job name must be uniuqe in list, {job.name}"
             job_names.add(job.name)
```

### Comparing `dwave_sona_core-1.2.9/sona/core/messages/file.py` & `dwave_sona_core-1.3.0/sona/core/messages/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     path: str
     metadata: Dict = {}
 
     def to_wav(self, *args, **kwargs):
         file_path = Path(self.path)
         if file_path.suffix == ".wav":
             return self
-        file_path = convert_audio(file_path, "wav")
+        file_path = convert_audio(file_path, "wav", format="s16")
         metadata = {}
         with wave.open(file_path, "rb") as w:
             metadata["OrigFilename"] = Path(self.path).name
             metadata["Channel"] = "stereo" if w.getnchannels() == 2 else "mono"
             metadata["Duration"] = float(w.getnframes()) / float(w.getframerate())
             metadata["Samplerate"] = w.getframerate()
         Path(self.path).unlink(missing_ok=True)
```

### Comparing `dwave_sona_core-1.2.9/sona/core/messages/job.py` & `dwave_sona_core-1.3.0/sona/core/messages/job.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/messages/state.py` & `dwave_sona_core-1.3.0/sona/core/messages/state.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/middlewares/tracer.py` & `dwave_sona_core-1.3.0/sona/core/middlewares/tracer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/azureblob.py` & `dwave_sona_core-1.3.0/sona/core/storages/azureblob.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/base.py` & `dwave_sona_core-1.3.0/sona/core/storages/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/filters/audio.py` & `dwave_sona_core-1.3.0/sona/core/storages/filters/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/local.py` & `dwave_sona_core-1.3.0/sona/core/storages/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/s3.py` & `dwave_sona_core-1.3.0/sona/core/storages/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/sources/azureblob.py` & `dwave_sona_core-1.3.0/sona/core/storages/sources/azureblob.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/sources/gdrive.py` & `dwave_sona_core-1.3.0/sona/core/storages/sources/gdrive.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/sources/http.py` & `dwave_sona_core-1.3.0/sona/core/storages/sources/http.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/sources/local.py` & `dwave_sona_core-1.3.0/sona/core/storages/sources/local.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/storages/sources/s3.py` & `dwave_sona_core-1.3.0/sona/core/storages/sources/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/stream/inferencer.py` & `dwave_sona_core-1.3.0/sona/core/stream/inferencer.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 
     def set_audio_input_spec(
         self, samples=3200, sample_rate=16000, layout="mono", format="s16"
     ):
         self.audio_parser = AudioStreamParser(samples, sample_rate, layout, format)
 
     def setup(self):
-        func = self.on_context
-        for middleware in reversed(middlewares):
-            func = middleware(func)
-        self.on_context = func
         self.audio_parser = AudioStreamParser()
+        for middleware in reversed(middlewares):
+            middleware.setup(self)
 
     def reply(self, streamdata: StreamData, header: Dict = None):
         header = header or dict()
         ctx = StreamContext(
             event_type=streamdata._type, header=header, payload=streamdata.payload
         )
         self.on_reply(ctx)
```

### Comparing `dwave_sona_core-1.2.9/sona/core/stream/messages/streamdata.py` & `dwave_sona_core-1.3.0/sona/core/stream/messages/streamdata.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/core/stream/parsers/audio.py` & `dwave_sona_core-1.3.0/sona/core/stream/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/settings.py` & `dwave_sona_core-1.3.0/sona/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import os
 from typing import Dict, List, Optional
 
 from pydantic import RedisDsn
-from pydantic_settings import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class Settings(BaseSettings):
+    model_config = SettingsConfigDict(
+        env_file=".env", env_file_encoding="utf-8", extra="ignore"
+    )
+
     SONA_INFERENCER_CLASS: Optional[str] = None
     SONA_STREAM_INFERENCER_CLASS: Optional[str] = None
+    SONA_INFERENCER_PROCESS_LIMIT: int = 10
 
     # Core Storage settings
     SONA_STORAGE_LOCAL_PATH: str = os.getcwd()
     SONA_STORAGE_S3_SETTING: Dict = dict()
     SONA_STORAGE_S3_BUCKET: str = "sona"
     SONA_SOURCE_GOOGLE_SERVICE_ACCOUNT_INFO: Optional[Dict] = None
 
     SONA_STORAGE_AZURE_BLOB_SETTING: Dict = dict()
     SONA_STORAGE_AZURE_BLOB_CONTAINER: str = "sona"
 
     # Worker base settings
     SONA_WORKER_CLASS: str = "sona.worker.workers.InferencerWorker"
     SONA_WORKER_TOPIC_PREFIX: str = "sona.inferencer."
+    SONA_WORKER_TOPIC: Optional[str] = None
 
     # Worker consumer settings
     SONA_WORKER_CONSUMER_SQS_SETTING: Optional[Dict] = None
     SONA_WORKER_CONSUMER_KAFKA_SETTING: Optional[Dict] = None
     SONA_WORKER_CONSUMER_REDIS_URL: Optional[RedisDsn] = None
     SONA_WORKER_CONSUMER_REDIS_GROUP: Optional[str] = "sona.anonymous"
 
@@ -33,23 +39,23 @@
     SONA_WORKER_PRODUCER_KAFKA_SETTING: Optional[Dict] = None
     SONA_WORKER_PRODUCER_REDIS_URL: Optional[RedisDsn] = None
 
     # Middleware settings
     SONA_MIDDLEWARE_CLASSES: List[str] = []
     SONA_MIDDLEWARE_SUPERVISOR_SQS_SETTING: Optional[Dict] = None
     SONA_MIDDLEWARE_SUPERVISOR_KAFKA_SETTING: Optional[Dict] = None
+
+    SONA_MIDDLEWARE_SUPERVISOR_S3_SETTING: Optional[Dict] = None
+    SONA_MIDDLEWARE_SUPERVISOR_S3_BUCKET: str = "sona"
+    SONA_MIDDLEWARE_SUPERVISOR_TOPICS: List = []
+
     SONA_MIDDLEWARE_TRACER_SERVICE_NAME: str = "SONA API"
     SONA_MIDDLEWARE_TRACER_JAEGER_HOST: str = "localhost"
     SONA_MIDDLEWARE_TRACER_JAEGER_PORT: int = 6831
 
     # Streaming Settings
     SONA_STREAM_RTC_TURN_FDQN: str = ""
     SONA_STREAM_RTC_USER: str = ""
     SONA_STREAM_RTC_PASS: str = ""
 
-    class Config:
-        env_file = ".env"
-        env_file_encoding = "utf-8"
-        extra = "ignore"
-
 
 settings = Settings()
```

### Comparing `dwave_sona_core-1.2.9/sona/utils/common.py` & `dwave_sona_core-1.3.0/sona/utils/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,31 @@
         return getattr(sys.modules[mod_str], class_str)
     except AttributeError:
         raise ImportError(
             f"Class {class_str} cannot be found ({traceback.format_exception(*sys.exc_info())})"
         )
 
 
-def convert_audio(filepath, ext):
+def convert_audio(filepath, ext, format=None, sample_rate=None):
     filepath = Path(filepath)
     in_path = str(filepath)
     out_path = str(filepath.parent / f"{filepath.stem}.{ext}")
 
     codec = "pcm_s16le" if ext == "wav" else ext
     with av.open(in_path, "r") as in_av:
         with av.open(out_path, "w") as out_av:
+            in_stream = in_av.streams.audio[0]
+            format = format or in_stream.format
+            sample_rate = sample_rate or in_stream.sample_rate
+
             out_stream = out_av.add_stream(codec)
+            out_stream.format = format
+            out_stream.sample_rate = sample_rate
             try:
-                for frame in in_av.decode(in_av.streams.audio[0]):
+                for frame in in_av.decode(in_stream):
                     for packet in out_stream.encode(frame):
                         out_av.mux(packet)
             except Exception as e:
                 logger.warning(
                     f"Converting incomplete cause: {e}, inferencer may not process all of the audio data"
                 )
             for packet in out_stream.encode(None):
```

### Comparing `dwave_sona_core-1.2.9/sona/web/rpc/handlers.py` & `dwave_sona_core-1.3.0/sona/web/rpc/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         options = options or {}
         inferencer: StreamInferencerBase = self.inferencer_cls(**options)
         inferencer.setup()
         inferencer.on_load()
         inferencer.on_reply = lambda ctx: self.queue.put_nowait((inferencer, ctx))
         inferencer.reply_channel = peer.createDataChannel(f"reply_{track.id}")
         inferencer.audio_track = AudioInferencerTrack()
+        inferencer.session_param = options
         peer.addTrack(inferencer.audio_track)
 
         self.tracks += [track]
         self.inferencers[track.id] = inferencer
 
     async def start(self):
         self.task = asyncio.create_task(self.on_reply())
@@ -46,32 +47,35 @@
 
     async def run_track(
         self, track: MediaStreamTrack, inferencer: StreamInferencerBase
     ):
         while True:
             try:
                 frame = await track.recv()
-                ctx = StreamContext(event_type=EvtType.AV_AUDIO, payload=frame)
+                ctx = StreamContext(
+                    event_type=EvtType.AV_AUDIO,
+                    payload=frame,
+                    header=inferencer.session_param,
+                )
                 inferencer.on_context(ctx)
             except MediaStreamError:
                 logger.warning("MediaStreamError")
                 return
             except Exception as e:
                 logger.exception(e)
                 raise
 
-    async def stop(self, track):
-        inferencer = self.inferencers[track.id]
+    async def stop(self, track_id):
+        inferencer = self.inferencers[track_id]
         inferencer.on_stop()
         inferencer.task.cancel()
 
-    async def stop_all(self, track=None):
-        for inferencer in self.inferencers.values():
-            inferencer.on_stop()
-            inferencer.task.cancel()
+    async def stop_all(self):
+        for track_id in self.inferencers:
+            self.stop(track_id)
 
     async def on_reply(self):
         while True:
             inferencer, ctx = await self.queue.get()
             _type = ctx.event_type
             if _type == EvtType.AV_AUDIO.value:
                 inferencer.audio_track.reply(ctx.payload)
```

### Comparing `dwave_sona_core-1.2.9/sona/web/rpc/tracks.py` & `dwave_sona_core-1.3.0/sona/web/rpc/tracks.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/web/server.py` & `dwave_sona_core-1.3.0/sona/web/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
+import contextlib
 import os
 
+from fastapi import HTTPException
 from fastapi.staticfiles import StaticFiles
 from loguru import logger
 from sona.core.inferencer import InferencerBase
 from sona.core.messages import Context
 from sona.core.messages.result import Result
 from sona.settings import settings
 
@@ -24,40 +26,44 @@
     from fastapi.responses import JSONResponse
 except ImportError:
     pass
 
 
 INFERENCER_CLASS = settings.SONA_INFERENCER_CLASS
 STREAM_INFERENCER_CLASS = settings.SONA_STREAM_INFERENCER_CLASS
+INFERENCER_PROCESS_LIMIT = settings.SONA_INFERENCER_PROCESS_LIMIT
 STATIC_ROOT = os.path.dirname(__file__)
 
 RTC_TURN_FDQN = settings.SONA_STREAM_RTC_TURN_FDQN
 RTC_USER = settings.SONA_STREAM_RTC_USER
 RTC_PASS = settings.SONA_STREAM_RTC_PASS
 
-app = FastAPI()
+
+@contextlib.asynccontextmanager
+async def lifespan(app):
+    app.peers = set()
+    app.handlers = set()
+    if INFERENCER_CLASS:
+        app.inferencer = InferencerBase.load_class(INFERENCER_CLASS)()
+        app.inferencer.setup()
+        app.inferencer.on_load()
+    yield
+
+
+app = FastAPI(lifespan=lifespan)
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_methods=["*"],
     allow_headers=["*"],
     allow_credentials=True,
 )
 
 
-@app.on_event("startup")
-async def startup():
-    app.peers = set()
-    if INFERENCER_CLASS:
-        app.inferencer = InferencerBase.load_class(INFERENCER_CLASS)()
-        app.inferencer.setup()
-        app.inferencer.on_load()
-
-
 @app.exception_handler(RequestValidationError)
 async def validation_exception_handler(request: Request, err: RequestValidationError):
     logger.warning(f"Client Error: {request}, {err.errors()}")
     resp = SonaResponse(code="400", message=str(err.errors()))
     return JSONResponse(status_code=400, content=resp.model_dump())
 
 
@@ -87,56 +93,60 @@
 
 if STREAM_INFERENCER_CLASS:
     app.mount("/static", StaticFiles(directory=f"{STATIC_ROOT}/static"), name="static")
 
     @app.post("/offer")
     async def offer(req: RPCOfferRequest):
         logger.info(f"Recive offer: {req}")
-        offer = RTCSessionDescription(sdp=req.sdp, type=req.type)
-        peer = RTCPeerConnection(
-            configuration=RTCConfiguration(
-                [
-                    RTCIceServer("stun:stun.l.google:19302"),
-                    RTCIceServer(RTC_TURN_FDQN, RTC_USER, RTC_PASS),
-                ]
+        if len(app.handlers) > INFERENCER_PROCESS_LIMIT:
+            raise HTTPException(
+                status_code=429,
+                detail=f"Too many inference sessions (sessions: {len(app.handlers)}, limit: {INFERENCER_PROCESS_LIMIT})",
             )
-        )
+
+        offer = RTCSessionDescription(sdp=req.sdp, type=req.type)
+        servers = [RTCIceServer("stun:stun.l.google:19302")]
+        if RTC_TURN_FDQN:
+            servers += [RTCIceServer(RTC_TURN_FDQN, RTC_USER, RTC_PASS)]
+        peer = RTCPeerConnection(configuration=RTCConfiguration(servers))
         handler = MediaInferencerHandler()
 
         @peer.on("datachannel")
         def on_datachannel(channel):
             @channel.on("message")
             def on_message(message):
                 if isinstance(message, str) and message.startswith("ping"):
                     channel.send("pong" + message[4:])
 
         @peer.on("connectionstatechange")
         async def on_connectionstatechange():
             logger.info(f"Connection state is {peer.connectionState}")
-            if peer.connectionState == "failed":
+            if peer.connectionState in ["failed", "closed"]:
                 await peer.close()
                 app.peers.discard(peer)
 
         @peer.on("track")
         def on_track(track):
             logger.info(f"Track {track.kind} received")
             if track.kind == "audio":
                 handler.addTrack(track, peer, req.options)
             elif track.kind == "video":
                 peer.addTrack(track)
 
             @track.on("ended")
             async def on_ended():
                 logger.info(f"Track {track.kind} ended")
-                await handler.stop(track)
+                await handler.stop(track.id)
+                app.handlers.discard(handler)
 
         await peer.setRemoteDescription(offer)
         answer = await peer.createAnswer()
         await peer.setLocalDescription(answer)
 
+        app.handlers.add(handler)
         app.peers.add(peer)
         await handler.start()
 
         return SonaResponse(
             result=Result(
                 data={
                     "sdp": peer.localDescription.sdp,
```

### Comparing `dwave_sona_core-1.2.9/sona/web/static/client.js` & `dwave_sona_core-1.3.0/sona/web/static/client.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -21,73 +21,85 @@
             urls: ['stun:stun.l.google.com:19302']
         }];
     }
 
     pc = new RTCPeerConnection(config);
 
     // register some listeners to help debugging
-    pc.addEventListener('icegatheringstatechange', function() {
+    pc.addEventListener('icegatheringstatechange', () => {
         iceGatheringLog.textContent += ' -> ' + pc.iceGatheringState;
     }, false);
     iceGatheringLog.textContent = pc.iceGatheringState;
 
-    pc.addEventListener('iceconnectionstatechange', function() {
+    pc.addEventListener('iceconnectionstatechange', () => {
         iceConnectionLog.textContent += ' -> ' + pc.iceConnectionState;
     }, false);
     iceConnectionLog.textContent = pc.iceConnectionState;
 
-    pc.addEventListener('signalingstatechange', function() {
+    pc.addEventListener('signalingstatechange', () => {
         signalingLog.textContent += ' -> ' + pc.signalingState;
     }, false);
     signalingLog.textContent = pc.signalingState;
 
-    pc.addEventListener(
-        "datachannel",
-        (ev) => {
-            receiveChannel = ev.channel;
-            receiveChannel.onmessage = (evt) => {
-                dataChannelLog.textContent += '> ' + evt.data + '\n';
-            };
-            receiveChannel.onopen = () => {};
-            receiveChannel.onclose = () => {};
-            console.log(receiveChannel)
-        },
-        false,
-    );
-
     // connect audio / video
-    pc.addEventListener('track', function(evt) {
+    pc.addEventListener('track', (evt) => {
         if (evt.track.kind == 'video')
             document.getElementById('video').srcObject = evt.streams[0];
         else
             document.getElementById('audio').srcObject = evt.streams[0];
     });
 
     return pc;
 }
 
+function enumerateInputDevices() {
+    const populateSelect = (select, devices) => {
+        let counter = 1;
+        devices.forEach((device) => {
+            const option = document.createElement('option');
+            option.value = device.deviceId;
+            option.text = device.label || ('Device #' + counter);
+            select.appendChild(option);
+            counter += 1;
+        });
+    };
+
+    navigator.mediaDevices.enumerateDevices().then((devices) => {
+        populateSelect(
+            document.getElementById('audio-input'),
+            devices.filter((device) => device.kind == 'audioinput')
+        );
+        populateSelect(
+            document.getElementById('video-input'),
+            devices.filter((device) => device.kind == 'videoinput')
+        );
+    }).catch((e) => {
+        alert(e);
+    });
+}
+
 function negotiate() {
-    return pc.createOffer().then(function(offer) {
+    return pc.createOffer().then((offer) => {
         return pc.setLocalDescription(offer);
-    }).then(function() {
+    }).then(() => {
         // wait for ICE gathering to complete
-        return new Promise(function(resolve) {
+        return new Promise((resolve) => {
             if (pc.iceGatheringState === 'complete') {
                 resolve();
             } else {
                 function checkState() {
                     if (pc.iceGatheringState === 'complete') {
                         pc.removeEventListener('icegatheringstatechange', checkState);
                         resolve();
                     }
                 }
                 pc.addEventListener('icegatheringstatechange', checkState);
             }
         });
-    }).then(function() {
+    }).then(() => {
         var offer = pc.localDescription;
         var codec;
 
         codec = document.getElementById('audio-codec').value;
         if (codec !== 'default') {
             offer.sdp = sdpFilterCodec('audio', codec, offer.sdp);
         }
@@ -105,95 +117,118 @@
                 video_transform: document.getElementById('video-transform').value
             }),
             headers: {
                 'Content-Type': 'application/json'
             },
             method: 'POST'
         });
-    }).then(function(response) {
+    }).then((response) => {
         return response.json();
-    }).then(function(answer) {
-        answer = answer.result.data
+    }).then((answer) => {
         document.getElementById('answer-sdp').textContent = answer.sdp;
         return pc.setRemoteDescription(answer);
-    }).catch(function(e) {
+    }).catch((e) => {
         alert(e);
     });
 }
 
 function start() {
     document.getElementById('start').style.display = 'none';
 
     pc = createPeerConnection();
 
     var time_start = null;
 
-    function current_stamp() {
+    const current_stamp = () => {
         if (time_start === null) {
             time_start = new Date().getTime();
             return 0;
         } else {
             return new Date().getTime() - time_start;
         }
-    }
+    };
 
     if (document.getElementById('use-datachannel').checked) {
         var parameters = JSON.parse(document.getElementById('datachannel-parameters').value);
 
         dc = pc.createDataChannel('chat', parameters);
-        dc.onclose = function() {
+        dc.addEventListener('close', () => {
             clearInterval(dcInterval);
             dataChannelLog.textContent += '- close\n';
-        };
-        dc.onopen = function() {
+        });
+        dc.addEventListener('open', () => {
             dataChannelLog.textContent += '- open\n';
-            dcInterval = setInterval(function() {
+            dcInterval = setInterval(() => {
                 var message = 'ping ' + current_stamp();
-                // dataChannelLog.textContent += '> ' + message + '\n';
+                dataChannelLog.textContent += '> ' + message + '\n';
                 dc.send(message);
             }, 1000);
-        };
-        dc.onmessage = function(evt) {
-            // dataChannelLog.textContent += '< ' + evt.data + '\n';
+        });
+        dc.addEventListener('message', (evt) => {
+            dataChannelLog.textContent += '< ' + evt.data + '\n';
 
             if (evt.data.substring(0, 4) === 'pong') {
                 var elapsed_ms = current_stamp() - parseInt(evt.data.substring(5), 10);
                 dataChannelLog.textContent += ' RTT ' + elapsed_ms + ' ms\n';
             }
-        };
+        });
     }
 
-    var constraints = {
-        audio: document.getElementById('use-audio').checked,
+    // Build media constraints.
+
+    const constraints = {
+        audio: false,
         video: false
     };
 
+    if (document.getElementById('use-audio').checked) {
+        const audioConstraints = {};
+
+        const device = document.getElementById('audio-input').value;
+        if (device) {
+            audioConstraints.deviceId = {
+                exact: device
+            };
+        }
+
+        constraints.audio = Object.keys(audioConstraints).length ? audioConstraints : true;
+    }
+
     if (document.getElementById('use-video').checked) {
-        var resolution = document.getElementById('video-resolution').value;
-        if (resolution) {
-            resolution = resolution.split('x');
-            constraints.video = {
-                width: parseInt(resolution[0], 0),
-                height: parseInt(resolution[1], 0)
+        const videoConstraints = {};
+
+        const device = document.getElementById('video-input').value;
+        if (device) {
+            videoConstraints.deviceId = {
+                exact: device
             };
-        } else {
-            constraints.video = true;
         }
+
+        const resolution = document.getElementById('video-resolution').value;
+        if (resolution) {
+            const dimensions = resolution.split('x');
+            videoConstraints.width = parseInt(dimensions[0], 0);
+            videoConstraints.height = parseInt(dimensions[1], 0);
+        }
+
+        constraints.video = Object.keys(videoConstraints).length ? videoConstraints : true;
     }
 
+    // Acquire media and start negociation.
+
     if (constraints.audio || constraints.video) {
         if (constraints.video) {
             document.getElementById('media').style.display = 'block';
         }
-        navigator.mediaDevices.getUserMedia(constraints).then(function(stream) {
-            stream.getTracks().forEach(function(track) {
+        navigator.mediaDevices.getUserMedia(constraints).then((stream) => {
+            stream.getTracks().forEach((track) => {
                 pc.addTrack(track, stream);
             });
             return negotiate();
-        }, function(err) {
+        }, (err) => {
             alert('Could not acquire media: ' + err);
         });
     } else {
         negotiate();
     }
 
     document.getElementById('stop').style.display = 'inline-block';
@@ -205,28 +240,28 @@
     // close data channel
     if (dc) {
         dc.close();
     }
 
     // close transceivers
     if (pc.getTransceivers) {
-        pc.getTransceivers().forEach(function(transceiver) {
+        pc.getTransceivers().forEach((transceiver) => {
             if (transceiver.stop) {
                 transceiver.stop();
             }
         });
     }
 
     // close local audio / video
-    pc.getSenders().forEach(function(sender) {
+    pc.getSenders().forEach((sender) => {
         sender.track.stop();
     });
 
     // close peer connection
-    setTimeout(function() {
+    setTimeout(() => {
         pc.close();
     }, 500);
 }
 
 function sdpFilterCodec(kind, codec, realSdp) {
     var allowed = []
     var rtxRegex = new RegExp('a=fmtp:(\\d+) apt=(\\d+)\r$');
@@ -282,8 +317,10 @@
     }
 
     return sdp;
 }
 
 function escapeRegExp(string) {
     return string.replace(/[.*+?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
-}
+}
+
+enumerateInputDevices();
```

### Comparing `dwave_sona_core-1.2.9/sona/web/static/webrtc.html` & `dwave_sona_core-1.3.0/sona/web/static/webrtc.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 
 <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>WebRTC demo</title>
     <style>
@@ -39,24 +40,30 @@
             <option value='{"ordered": false, "maxRetransmits": 0}'>Unordered, no retransmissions</option>
             <option value='{"ordered": false, "maxPacketLifetime": 500}'>Unordered, 500ms lifetime</option>
         </select>
     </div>
     <div class="option">
         <input id="use-audio" checked="checked" type="checkbox" />
         <label for="use-audio">Use audio</label>
+        <select id="audio-input">
+            <option value="" selected>Default device</option>
+        </select>
         <select id="audio-codec">
             <option value="default" selected>Default codecs</option>
             <option value="opus/48000/2">Opus</option>
             <option value="PCMU/8000">PCMU</option>
             <option value="PCMA/8000">PCMA</option>
         </select>
     </div>
     <div class="option">
         <input id="use-video" type="checkbox" />
         <label for="use-video">Use video</label>
+        <select id="video-input">
+            <option value="" selected>Default device</option>
+        </select>
         <select id="video-resolution">
             <option value="" selected>Default resolution</option>
             <option value="320x240">320x240</option>
             <option value="640x480">640x480</option>
             <option value="960x540">960x540</option>
             <option value="1280x720">1280x720</option>
         </select>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ********** OOppttiioonnss **********
 Use datachannel[One of: Ordered, reliable/Unordered, no retransmissions/
 Unordered, 500ms lifetime]
-Use audio[One of: Default codecs/Opus/PCMU/PCMA]
-??Use video[One of: Default resolution/320x240/640x480/960x540/1280x720][One of:
-No transform/Edge detection/Cartoon effect/Rotate][One of: Default codecs/VP8/
-H264]
+Use audio[One of: Default device][One of: Default codecs/Opus/PCMU/PCMA]
+??Use video[One of: Default device][One of: Default resolution/320x240/640x480/
+960x540/1280x720][One of: No transform/Edge detection/Cartoon effect/Rotate]
+[One of: Default codecs/VP8/H264]
 ??Use STUN server
 Start Stop
 ********** SSttaattee **********
 ICE gathering state:
 ICE connection state:
 Signaling state:
 ********** MMeeddiiaa **********
```

### Comparing `dwave_sona_core-1.2.9/sona/worker/commands.py` & `dwave_sona_core-1.3.0/sona/worker/commands.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/consumers/__init__.py` & `dwave_sona_core-1.3.0/sona/worker/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/consumers/kafka.py` & `dwave_sona_core-1.3.0/sona/worker/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/consumers/redis.py` & `dwave_sona_core-1.3.0/sona/worker/consumers/redis.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/consumers/sqs.py` & `dwave_sona_core-1.3.0/sona/worker/consumers/sqs.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/producers/__init__.py` & `dwave_sona_core-1.3.0/sona/worker/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/producers/kafka.py` & `dwave_sona_core-1.3.0/sona/worker/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-1.2.9/sona/worker/workers.py` & `dwave_sona_core-1.3.0/sona/worker/workers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 
 from loguru import logger
+
 from sona.core.inferencer import InferencerBase
 from sona.core.messages import Context
 from sona.settings import settings
 from sona.utils.common import import_class
 from sona.worker.consumers import ConsumerBase
 from sona.worker.producers import ProducerBase
 
 TOPIC_PREFIX = settings.SONA_WORKER_TOPIC_PREFIX
+TOPIC = settings.SONA_WORKER_TOPIC
 
 
 class WorkerBase:
     name: str = None
 
     def set_consumer(self, consumer: ConsumerBase):
         self.consumer = consumer
@@ -33,15 +35,15 @@
                 context = Context.model_validate_json(message)
                 await self.on_context(context)
             except Exception as e:
                 logger.exception(f"[{self.topic}] error: {e}, msg: {message}")
 
     @classmethod
     def get_topic(cls) -> str:
-        return f"{TOPIC_PREFIX}{cls.name}"
+        return TOPIC or f"{TOPIC_PREFIX}{cls.name}"
 
     @classmethod
     def load_class(cls, import_str):
         _cls = import_class(import_str)
         if _cls not in cls.__subclasses__():
             raise Exception(f"Unknown worker class: {import_str}")
         return _cls
@@ -80,8 +82,8 @@
             if next_job:
                 self.producer.emit(next_job.topic, next_ctx.to_message())
             else:
                 for topic in next_ctx.reporters:
                     self.producer.emit(topic, next_ctx.to_message())
 
     def get_topic(self):
-        return f"{TOPIC_PREFIX}{self.inferencer.name}"
+        return TOPIC or f"{TOPIC_PREFIX}{self.inferencer.name}"
```

### Comparing `dwave_sona_core-1.2.9/PKG-INFO` & `dwave_sona_core-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: dwave-sona-core
-Version: 1.2.9
+Version: 1.3.0
 Summary: 
 Author: dwave-dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiortc (>=1.6.0,<2.0.0)
-Requires-Dist: av (>=11.0.0,<12.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiortc (>=1.5.0,<2.0.0)
+Requires-Dist: av
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.0,<13.0.0)
 Requires-Dist: boto3 (>=1.34.14,<2.0.0)
 Requires-Dist: confluent-kafka (>=2.3.0,<3.0.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: google-api-python-client (>=2.112.0,<3.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-jaeger-thrift (>=1.21.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.21.0,<2.0.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: redis (>=5.0.1,<6.0.0)
+Requires-Dist: smart-open (>=7.0.4,<8.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.25.0,<0.26.0)
 Requires-Dist: wget (>=3.2,<4.0)
-Requires-Dist: yt-dlp (>=2023.12.30,<2024.0.0)
+Requires-Dist: yt-dlp
 Description-Content-Type: text/markdown
 
 # Dwave SONA Core
 
 迪威智能 SONA 服務專用核心開發套件
 
 ## 安裝與使用
```

