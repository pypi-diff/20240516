# Comparing `tmp/fcw_service-0.8.1.tar.gz` & `tmp/fcw_service-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_service-0.8.1.tar", max compression
+gzip compressed data, was "fcw_service-0.9.1.tar", max compression
```

## Comparing `fcw_service-0.8.1.tar` & `fcw_service-0.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      236 2023-07-19 16:34:58.000000 fcw_service-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_service-0.8.1/fcw_service/__init__.py
--rw-r--r--   0        0        0     8284 2023-11-28 14:19:35.000000 fcw_service-0.8.1/fcw_service/collision_worker.py
--rw-r--r--   0        0        0     8833 2023-12-11 16:53:02.000000 fcw_service-0.8.1/fcw_service/interface.py
--rw-r--r--   0        0        0     8508 2023-10-23 10:37:40.000000 fcw_service-0.8.1/fcw_service/visualization.py
--rw-r--r--   0        0        0      797 2023-12-11 18:50:57.000000 fcw_service-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 fcw_service-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      236 2023-07-19 16:34:58.000000 fcw_service-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_service-0.9.1/fcw_service/__init__.py
+-rw-r--r--   0        0        0     8284 2023-11-28 14:19:35.000000 fcw_service-0.9.1/fcw_service/collision_worker.py
+-rw-r--r--   0        0        0     8759 2023-12-18 10:07:52.000000 fcw_service-0.9.1/fcw_service/interface.py
+-rw-r--r--   0        0        0     8508 2023-10-23 10:37:40.000000 fcw_service-0.9.1/fcw_service/visualization.py
+-rw-r--r--   0        0        0      797 2023-12-18 10:29:27.000000 fcw_service-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 fcw_service-0.9.1/PKG-INFO
```

### Comparing `fcw_service-0.8.1/fcw_service/collision_worker.py` & `fcw_service-0.9.1/fcw_service/collision_worker.py`

 * *Files identical despite different names*

### Comparing `fcw_service-0.8.1/fcw_service/interface.py` & `fcw_service-0.9.1/fcw_service/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 import os
+import signal
 import sys
-import threading
 import time
 import traceback
 from dataclasses import dataclass
 from queue import Queue
 from typing import Dict, Tuple, Any
 
 import numpy as np
 
-import era_5g_interface.interface_helpers
 from era_5g_interface.channels import CallbackInfoServer, ChannelType, DATA_NAMESPACE, DATA_ERROR_EVENT
 from era_5g_interface.dataclasses.control_command import ControlCommand, ControlCmdType
-from era_5g_interface.interface_helpers import HeartBeatSender
+from era_5g_interface.interface_helpers import HeartBeatSender, MIDDLEWARE_REPORT_INTERVAL, RepeatedTimer
 from era_5g_interface.task_handler_internal_q import TaskHandlerInternalQ
 from era_5g_server.server import NetworkApplicationServer
 from fcw_core.yolo_detector import YOLODetector
 from fcw_service.collision_worker import CollisionWorker
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
 logger = logging.getLogger("FCW interface")
@@ -51,63 +50,62 @@
         Args:
             *args: NetworkApplicationServer arguments.
             **kwargs: NetworkApplicationServer arguments.
         """
 
         super().__init__(
             callbacks_info={
-                "image": CallbackInfoServer(ChannelType.H264, self.image_callback),  # Due to 0.8.0 compatibility
                 "image_h264": CallbackInfoServer(ChannelType.H264, self.image_callback),
                 "image_jpeg": CallbackInfoServer(ChannelType.JPEG, self.image_callback),
             },
             *args,
             **kwargs,
         )
 
         # List of registered tasks.
         self.tasks: Dict[str, TaskAndWorker] = dict()
 
         self.heart_beat_sender = HeartBeatSender()
-        self.heart_beat_timer()
+        heart_beat_timer = RepeatedTimer(MIDDLEWARE_REPORT_INTERVAL, self.heart_beat)
+        heart_beat_timer.start()
 
-    def heart_beat_timer(self):
-        """Heart beat timer."""
+    def heart_beat(self):
+        """Heart beat generation and sending."""
 
         latencies = []
         for task_and_worker in self.tasks.values():
             latencies.extend(task_and_worker.worker.latency_measurements.get_latencies())
         avg_latency = 0
         if len(latencies) > 0:
             avg_latency = float(np.mean(np.array(latencies)))
 
-        queue_size = 1
-        queue_occupancy = 1
+        queue_size = NETAPP_INPUT_QUEUE
+        queue_occupancy = 1  # TODO: Compute for every worker?
 
         self.heart_beat_sender.send_middleware_heart_beat(
             avg_latency=avg_latency,
             queue_size=queue_size,
             queue_occupancy=queue_occupancy,
             current_robot_count=len(self.tasks),
         )
-        threading.Timer(era_5g_interface.interface_helpers.MIDDLEWARE_REPORT_INTERVAL, self.heart_beat_timer).start()
 
     def image_callback(self, sid: str, data: Dict[str, Any]) -> None:
         """Allows to receive decoded image using the websocket transport.
 
         Args:
             sid (str): Namespace sid.
             data (Dict[str, Any]): Data dict including decoded frame (data["frame"]) and send timestamp
                 (data["timestamp"]).
         """
 
         eio_sid = self._sio.manager.eio_sid_from_sid(sid, DATA_NAMESPACE)
 
         if eio_sid not in self.tasks:
             logger.error(f"Non-registered client {eio_sid} tried to send data")
-            self.send_data({"message": "Non-registered client tried to send data"}, DATA_ERROR_EVENT, sid)
+            self.send_data({"message": "Non-registered client tried to send data"}, DATA_ERROR_EVENT, sid=sid)
             return
 
         task = self.tasks[eio_sid].task
         task.store_data({"timestamp": data["timestamp"], "recv_timestamp": time.perf_counter_ns()}, data["frame"])
 
     def command_callback(self, command: ControlCommand, sid: str) -> Tuple[bool, str]:
         """Process initialization control command - create task, worker and start the worker.
@@ -158,15 +156,15 @@
                     image_queue,
                     lambda results: self.send_data(data=results, event="results", sid=self.get_sid_of_data(eio_sid)),
                     config,
                     camera_config,
                     fps,
                     viz,
                     viz_zmq_port,
-                    name=f"Detector {eio_sid}",
+                    name=f"Collision Worker {eio_sid}",
                     daemon=True,
                 )
             except Exception as ex:
                 logger.error(f"Failed to create CollisionWorker: {repr(ex)}")
                 logger.error(traceback.format_exc())
                 self.send_command_error(f"Failed to create CollisionWorker: {repr(ex)}", sid)
                 return False, f"Failed to create CollisionWorker: {repr(ex)}"
```

### Comparing `fcw_service-0.8.1/fcw_service/visualization.py` & `fcw_service-0.9.1/fcw_service/visualization.py`

 * *Files identical despite different names*

### Comparing `fcw_service-0.8.1/pyproject.toml` & `fcw_service-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "fcw-service"
-version = "0.8.1"
+version = "0.9.1"
 description = "Early collision warning Network Application for Transportation use case - service part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_service"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 opencv-python = ">=4.8"
 pyzmq = ">=25.1.1"
-era-5g-interface = "^0.7.0"
-era-5g-server = "^0.1.0"
-fcw-core-utils = "^0.8.0"
-fcw-core = "^0.8.0"
+era-5g-interface = "^0.8.0"
+era-5g-server = "^0.2.0"
+fcw-core-utils = "^0.9.0"
+fcw-core = "^0.9.0"
 
 [tool.poetry.scripts]
 fcw_service = "fcw_service.interface:main"
 fcw_visualization = "fcw_service.visualization:main"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `fcw_service-0.8.1/PKG-INFO` & `fcw_service-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: fcw-service
-Version: 0.8.1
+Version: 0.9.1
 Summary: Early collision warning Network Application for Transportation use case - service part
 Home-page: https://github.com/5G-ERA/CollisionWarningService
 Author: Petr Kleparnik
 Author-email: pkleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: era-5g-interface (>=0.7.0,<0.8.0)
-Requires-Dist: era-5g-server (>=0.1.0,<0.2.0)
-Requires-Dist: fcw-core (>=0.8.0,<0.9.0)
-Requires-Dist: fcw-core-utils (>=0.8.0,<0.9.0)
+Requires-Dist: era-5g-interface (>=0.8.0,<0.9.0)
+Requires-Dist: era-5g-server (>=0.2.0,<0.3.0)
+Requires-Dist: fcw-core (>=0.9.0,<0.10.0)
+Requires-Dist: fcw-core-utils (>=0.9.0,<0.10.0)
 Requires-Dist: opencv-python (>=4.8)
 Requires-Dist: pyzmq (>=25.1.1)
 Project-URL: Repository, https://github.com/5G-ERA/CollisionWarningService
 Description-Content-Type: text/markdown
 
 # Forward Collision Warning - service part
```

