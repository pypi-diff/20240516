# Comparing `tmp/openclip_client-0.1.0.tar.gz` & `tmp/openclip_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openclip_client-0.1.0.tar", max compression
+gzip compressed data, was "openclip_client-0.1.1.tar", max compression
```

## Comparing `openclip_client-0.1.0.tar` & `openclip_client-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0      167 2024-03-27 10:59:04.000000 openclip_client-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 openclip_client-0.1.0/examples/openclip_client_python/__init__.py
--rw-r--r--   0        0        0      182 2024-05-09 12:57:46.792764 openclip_client-0.1.0/examples/openclip_client_python/client-channels-input-20240509_145746_797.csv
--rw-r--r--   0        0        0    23856 2024-05-09 12:58:55.339372 openclip_client-0.1.0/examples/openclip_client_python/client-channels-input-20240509_145836_900.csv
--rw-r--r--   0        0        0      286 2024-05-09 12:57:46.792764 openclip_client-0.1.0/examples/openclip_client_python/client-channels-output-20240509_145746_797.csv
--rw-r--r--   0        0        0    45304 2024-05-09 12:58:55.311373 openclip_client-0.1.0/examples/openclip_client_python/client-channels-output-20240509_145836_900.csv
--rw-r--r--   0        0        0      138 2024-05-09 12:57:46.792764 openclip_client-0.1.0/examples/openclip_client_python/client-final-20240509_145746_795.csv
--rw-r--r--   0        0        0    27536 2024-05-09 12:58:55.339372 openclip_client-0.1.0/examples/openclip_client_python/client-final-20240509_145836_898.csv
--rw-r--r--   0        0        0     6425 2024-05-09 12:22:25.000000 openclip_client-0.1.0/examples/openclip_client_python/client_python.py
--rw-r--r--   0        0        0     7378 2024-05-09 12:22:35.000000 openclip_client-0.1.0/examples/openclip_client_python/client_python_middleware.py
--rw-r--r--   0        0        0    13389 2024-05-09 12:46:09.000000 openclip_client-0.1.0/openclip_client/client_common.py
--rw-r--r--   0        0        0      972 2024-04-04 09:20:27.000000 openclip_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 openclip_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      167 2024-03-27 10:59:04.000000 openclip_client-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 openclip_client-0.1.1/examples/openclip_client_python/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-15 08:49:48.720677 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_104948_726.csv
+-rw-r--r--   0        0        0      138 2024-05-15 08:50:37.211666 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_105037_216.csv
+-rw-r--r--   0        0        0      138 2024-05-15 08:54:26.378891 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_105426_381.csv
+-rw-r--r--   0        0        0      138 2024-05-15 08:59:01.533156 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_105901_535.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:04:17.018967 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_110417_021.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:08:12.374584 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_110812_375.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:08:37.630103 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_110837_633.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:10:29.679952 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_111029_685.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:12:33.777538 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_111233_781.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:42:53.145468 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_114253_148.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:50:55.936044 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_115055_941.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:51:30.411363 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_115130_418.csv
+-rw-r--r--   0        0        0      138 2024-05-15 09:54:53.291344 openclip_client-0.1.1/examples/openclip_client_python/client-final-20240515_115453_298.csv
+-rw-r--r--   0        0        0     6290 2024-05-15 10:12:21.000000 openclip_client-0.1.1/examples/openclip_client_python/client_python.py
+-rw-r--r--   0        0        0     7290 2024-05-16 15:46:21.000000 openclip_client-0.1.1/examples/openclip_client_python/client_python_middleware.py
+-rw-r--r--   0        0        0    13445 2024-05-15 15:33:21.000000 openclip_client-0.1.1/openclip_client/client_common.py
+-rw-r--r--   0        0        0      886 2024-05-16 15:55:15.000000 openclip_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 openclip_client-0.1.1/PKG-INFO
```

### Comparing `openclip_client-0.1.0/examples/openclip_client_python/client_python.py` & `openclip_client-0.1.1/examples/openclip_client_python/client_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,14 @@
 
     # Parse arguments.
     parser = ArgumentParser()
     parser.add_argument(
         "-s", "--stream_type", type=int, help="StreamType: 1 = JPEG, 2 = H.264, 3 = HEVC", default=StreamType.H264
     )
     parser.add_argument("-c", "--config", type=Path, help="Collision warning config", default=CONFIG_FILE)
-    parser.add_argument(
-        "-p", "--out_prefix", type=str, help="Prefix of output csv file with measurements", default=None
-    )
     parser.add_argument("-t", "--play_time", type=int, help="Video play time in seconds", default=5000)
     parser.add_argument("source_video", type=str, help="Video stream (file or url)", nargs="?", default=TEST_VIDEO_FILE)
     parser.add_argument("-m", "--measuring", type=bool, help="Enable extended measuring logs", default=True)
     parser.add_argument("--stats", type=bool, help="Store output data sizes", default=True)
     args = parser.parse_args()
 
     global clip_client
@@ -113,15 +110,15 @@
             [
                 "there is a traffic light in front of me",
                 "there is no traffic light in front of me",
                 "there is a traffic sign in front of me",
                 "no sign or traffic light",
             ],
             ["the traffic light is red", "the traffic light is green", "the traffic light is orange"],
-            ["it's cloudy, it's clear, it's raining"],
+            ["it's cloudy", "it's clear", "it's raining"],
         ]
 
         # Rate timer for control the speed of a loop (fps).
         rate_timer = RateTimer(rate=fps, time_function=time.perf_counter, iteration_miss_warning=True)
         # Start time
         start_time = time.perf_counter_ns()
         # Check elapsed time or stopped flag.
```

### Comparing `openclip_client-0.1.0/examples/openclip_client_python/client_python_middleware.py` & `openclip_client-0.1.1/examples/openclip_client_python/client_python_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 # Middleware address.
 MIDDLEWARE_ADDRESS = str(os.getenv("MIDDLEWARE_ADDRESS", "127.0.0.1"))
 # Middleware user ID.
 MIDDLEWARE_USER = str(os.getenv("MIDDLEWARE_USER", "00000000-0000-0000-0000-000000000000"))
 # Middleware password.
 MIDDLEWARE_PASSWORD = str(os.getenv("MIDDLEWARE_PASSWORD", "password"))
 # Middleware Network Application ID (task ID).
-MIDDLEWARE_TASK_ID = str(os.getenv("MIDDLEWARE_TASK_ID", "00000000-0000-0000-0000-000000000000"))
+MIDDLEWARE_TASK_ID = str(
+    os.getenv("CLIP_MIDDLEWARE_TASK_ID", str(os.getenv("MIDDLEWARE_TASK_ID", "00000000-0000-0000-0000-000000000000")))
+)
 # Middleware robot ID (robot ID).
 MIDDLEWARE_ROBOT_ID = str(os.getenv("MIDDLEWARE_ROBOT_ID", "00000000-0000-0000-0000-000000000000"))
 
 
 def signal_handler(sig: int, *_) -> None:
     """Signal handler for SIGTERM and SIGINT."""
 
@@ -68,17 +70,14 @@
 
     # Parse arguments.
     parser = ArgumentParser()
     parser.add_argument(
         "-s", "--stream_type", type=int, help="StreamType: 1 = JPEG, 2 = H.264, 3 = HEVC", default=StreamType.H264
     )
     parser.add_argument("-c", "--config", type=Path, help="Collision warning config", default=CONFIG_FILE)
-    parser.add_argument(
-        "-p", "--out_prefix", type=str, help="Prefix of output csv file with measurements", default=None
-    )
     parser.add_argument("-t", "--play_time", type=int, help="Video play time in seconds", default=5000)
     parser.add_argument("source_video", type=str, help="Video stream (file or url)", nargs="?", default=TEST_VIDEO_FILE)
     parser.add_argument("-m", "--measuring", type=bool, help="Enable extended measuring logs", default=True)
     parser.add_argument("--stats", type=bool, help="Store output data sizes", default=True)
     args = parser.parse_args()
 
     global clip_client, stopped
```

### Comparing `openclip_client-0.1.0/openclip_client/client_common.py` & `openclip_client-0.1.1/openclip_client/client_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,15 @@
 
         # Create CLIP client.
         if isinstance(netapp_info, MiddlewareAllInfo):
             self.client = NetAppClient(
                 {"results": CallbackInfoClient(ChannelType.JSON, self.results_callback)},
                 logging_level=logging.getLogger().level,
                 stats=stats,
+                extended_measuring=extended_measuring,
             )
             logger.info(f"Register with netapp_info: {netapp_info}")
             self.client.connect_to_middleware(netapp_info.middleware_info)
             # Register client.
             try:
                 self.client.run_task(
                     task_id=netapp_info.task_id,
```

### Comparing `openclip_client-0.1.0/pyproject.toml` & `openclip_client-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openclip-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLIP Service Network Application - client part"
 authors = ["Petr Kleparnik <p.kleparnik@cognitechna.cz>", "Roman Juranek <r.juranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CLIPService"
 packages = [{include = "openclip_client"}, {include = "openclip_client_python", from = "examples"}]
 
 [tool.poetry.dependencies]
@@ -13,16 +13,15 @@
 opencv-python = ">=4.8"
 imutils = ">=0.5.4"
 era-5g-client = "^0.11.0"
 era-5g-interface = "^0.10.0"
 
 [tool.poetry.scripts]
 openclip_client_python = "openclip_client_python.client_python:main"
-#openclip_client_python_middleware = "openclip_client_python.client_python_middleware:main"
-#openclip_client_python_simple = "openclip_client_python.client_python_simple:main"
+openclip_client_python_middleware = "openclip_client_python.client_python_middleware:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `openclip_client-0.1.0/PKG-INFO` & `openclip_client-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclip-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLIP Service Network Application - client part
 Home-page: https://github.com/5G-ERA/CLIPService
 Author: Petr Kleparnik
 Author-email: p.kleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

