# Comparing `tmp/naneos_devices-1.0.8.tar.gz` & `tmp/naneos_devices-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naneos_devices-1.0.8.tar", max compression
+gzip compressed data, was "naneos_devices-1.0.9.tar", max compression
```

## Comparing `naneos_devices-1.0.8.tar` & `naneos_devices-1.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2023-12-06 07:33:34.895157 naneos_devices-1.0.8/LICENSE.txt
--rw-r--r--   0        0        0     6015 2023-12-06 21:45:10.868041 naneos_devices-1.0.8/README.md
--rw-r--r--   0        0        0     4875 2023-12-15 22:47:01.413684 naneos_devices-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-01 09:24:51.115402 naneos_devices-1.0.8/src/naneos/__init__.py
--rw-r--r--   0        0        0      284 2023-12-01 13:59:38.407434 naneos_devices-1.0.8/src/naneos/iotweb/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 13:23:20.851419 naneos_devices-1.0.8/src/naneos/iotweb/download/__init__.py
--rw-r--r--   0        0        0     3305 2023-12-06 21:25:51.975171 naneos_devices-1.0.8/src/naneos/iotweb/download/downloader.py
--rw-r--r--   0        0        0     4603 2023-12-15 10:24:47.150463 naneos_devices-1.0.8/src/naneos/iotweb/iotweb.py
--rw-r--r--   0        0        0     2591 2023-12-15 12:22:27.070972 naneos_devices-1.0.8/src/naneos/iotweb/partector2_pro_garage_upload.py
--rw-r--r--   0        0        0      427 2023-12-10 21:54:18.129031 naneos_devices-1.0.8/src/naneos/logger/__init__.py
--rw-r--r--   0        0        0     2384 2023-12-15 22:28:51.178917 naneos_devices-1.0.8/src/naneos/logger/custom_logger.py
--rw-r--r--   0        0        0      433 2023-12-01 13:23:20.856832 naneos_devices-1.0.8/src/naneos/partector/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 13:23:20.862471 naneos_devices-1.0.8/src/naneos/partector/blueprints/__init__.py
--rw-r--r--   0        0        0     4461 2023-12-15 08:00:24.264818 naneos_devices-1.0.8/src/naneos/partector/blueprints/_data_structure.py
--rw-r--r--   0        0        0      785 2023-12-15 10:35:55.902362 naneos_devices-1.0.8/src/naneos/partector/blueprints/_partectorCheckerThread.py
--rw-r--r--   0        0        0    15029 2023-12-15 12:30:44.989925 naneos_devices-1.0.8/src/naneos/partector/blueprints/_partector_blueprint.py
--rw-r--r--   0        0        0      301 2023-12-01 13:23:20.866238 naneos_devices-1.0.8/src/naneos/partector/blueprints/_partector_defaults.py
--rw-r--r--   0        0        0      792 2023-12-01 13:23:20.866548 naneos_devices-1.0.8/src/naneos/partector/partector1.py
--rw-r--r--   0        0        0      924 2023-12-14 22:29:22.835776 naneos_devices-1.0.8/src/naneos/partector/partector2.py
--rw-r--r--   0        0        0      809 2023-12-01 13:23:20.867103 naneos_devices-1.0.8/src/naneos/partector/partector2_pro.py
--rw-r--r--   0        0        0     4667 2023-12-15 22:01:06.740558 naneos_devices-1.0.8/src/naneos/partector/partector2_pro_garage.py
--rw-r--r--   0        0        0     1814 2023-12-14 22:45:28.466154 naneos_devices-1.0.8/src/naneos/partector/scan_for_partector.py
--rw-r--r--   0        0        0        0 2023-12-01 13:23:20.868462 naneos_devices-1.0.8/src/naneos/partector_ble/__init__.py
--rw-r--r--   0        0        0     7839 2023-12-14 21:35:04.028465 naneos_devices-1.0.8/src/naneos/partector_ble/partector_ble.py
--rw-r--r--   0        0        0     6941 2023-12-14 21:34:27.381248 naneos_devices-1.0.8/src/naneos/partector_ble/partector_ble_device.py
--rw-r--r--   0        0        0     1141 2023-12-08 11:21:31.362430 naneos_devices-1.0.8/src/naneos/partector_ble/test.py
--rw-r--r--   0        0        0      248 2023-12-15 10:24:47.153200 naneos_devices-1.0.8/src/naneos/protobuf/__init__.py
--rw-r--r--   0        0        0       74 2023-12-01 13:23:20.870639 naneos_devices-1.0.8/src/naneos/protobuf/partector2_ble/__init__.py
--rw-r--r--   0        0        0     5803 2023-12-08 07:28:55.574174 naneos_devices-1.0.8/src/naneos/protobuf/partector2_ble/partector2_ble.py
--rw-r--r--   0        0        0     2545 2023-12-01 13:23:20.872321 naneos_devices-1.0.8/src/naneos/protobuf/protoV1.proto
--rw-r--r--   0        0        0     4915 2023-12-08 07:28:55.546753 naneos_devices-1.0.8/src/naneos/protobuf/protoV1_pb2.py
--rw-r--r--   0        0        0    10588 2023-12-10 20:24:54.999531 naneos_devices-1.0.8/src/naneos/protobuf/protoV1_pb2.pyi
--rw-r--r--   0        0        0     6155 2023-12-15 11:00:13.047046 naneos_devices-1.0.8/src/naneos/protobuf/protobuf.py
--rw-r--r--   0        0        0       95 2023-12-01 09:24:51.115584 naneos_devices-1.0.8/src/naneos/py.typed
--rw-r--r--   0        0        0      104 2023-12-08 08:27:14.516691 naneos_devices-1.0.8/src/naneos/serial_utils/__init__.py
--rw-r--r--   0        0        0     1337 2023-12-15 22:46:52.413440 naneos_devices-1.0.8/src/naneos/serial_utils/list_serial_ports.py
--rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 naneos_devices-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-12-06 07:33:34.895157 naneos_devices-1.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     6015 2023-12-06 21:45:10.868041 naneos_devices-1.0.9/README.md
+-rw-r--r--   0        0        0     4875 2023-12-20 17:12:25.880221 naneos_devices-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-01 09:24:51.115402 naneos_devices-1.0.9/src/naneos/__init__.py
+-rw-r--r--   0        0        0      284 2023-12-01 13:59:38.407434 naneos_devices-1.0.9/src/naneos/iotweb/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 13:23:20.851419 naneos_devices-1.0.9/src/naneos/iotweb/download/__init__.py
+-rw-r--r--   0        0        0     3305 2023-12-06 21:25:51.975171 naneos_devices-1.0.9/src/naneos/iotweb/download/downloader.py
+-rw-r--r--   0        0        0     4603 2023-12-15 10:24:47.150463 naneos_devices-1.0.9/src/naneos/iotweb/iotweb.py
+-rw-r--r--   0        0        0     2591 2023-12-15 12:22:27.070972 naneos_devices-1.0.9/src/naneos/iotweb/partector2_pro_garage_upload.py
+-rw-r--r--   0        0        0      427 2023-12-10 21:54:18.129031 naneos_devices-1.0.9/src/naneos/logger/__init__.py
+-rw-r--r--   0        0        0     2384 2023-12-15 22:28:51.178917 naneos_devices-1.0.9/src/naneos/logger/custom_logger.py
+-rw-r--r--   0        0        0      433 2023-12-01 13:23:20.856832 naneos_devices-1.0.9/src/naneos/partector/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 13:23:20.862471 naneos_devices-1.0.9/src/naneos/partector/blueprints/__init__.py
+-rw-r--r--   0        0        0     4461 2023-12-15 08:00:24.264818 naneos_devices-1.0.9/src/naneos/partector/blueprints/_data_structure.py
+-rw-r--r--   0        0        0     1043 2023-12-20 16:36:08.985730 naneos_devices-1.0.9/src/naneos/partector/blueprints/_partectorCheckerThread.py
+-rw-r--r--   0        0        0    15396 2023-12-20 17:11:00.034547 naneos_devices-1.0.9/src/naneos/partector/blueprints/_partector_blueprint.py
+-rw-r--r--   0        0        0      301 2023-12-01 13:23:20.866238 naneos_devices-1.0.9/src/naneos/partector/blueprints/_partector_defaults.py
+-rw-r--r--   0        0        0      792 2023-12-01 13:23:20.866548 naneos_devices-1.0.9/src/naneos/partector/partector1.py
+-rw-r--r--   0        0        0      924 2023-12-14 22:29:22.835776 naneos_devices-1.0.9/src/naneos/partector/partector2.py
+-rw-r--r--   0        0        0      809 2023-12-01 13:23:20.867103 naneos_devices-1.0.9/src/naneos/partector/partector2_pro.py
+-rw-r--r--   0        0        0     4804 2023-12-20 17:08:25.053595 naneos_devices-1.0.9/src/naneos/partector/partector2_pro_garage.py
+-rw-r--r--   0        0        0     1814 2023-12-14 22:45:28.466154 naneos_devices-1.0.9/src/naneos/partector/scan_for_partector.py
+-rw-r--r--   0        0        0        0 2023-12-01 13:23:20.868462 naneos_devices-1.0.9/src/naneos/partector_ble/__init__.py
+-rw-r--r--   0        0        0     7839 2023-12-14 21:35:04.028465 naneos_devices-1.0.9/src/naneos/partector_ble/partector_ble.py
+-rw-r--r--   0        0        0     6941 2023-12-14 21:34:27.381248 naneos_devices-1.0.9/src/naneos/partector_ble/partector_ble_device.py
+-rw-r--r--   0        0        0     1141 2023-12-08 11:21:31.362430 naneos_devices-1.0.9/src/naneos/partector_ble/test.py
+-rw-r--r--   0        0        0      248 2023-12-15 10:24:47.153200 naneos_devices-1.0.9/src/naneos/protobuf/__init__.py
+-rw-r--r--   0        0        0       74 2023-12-01 13:23:20.870639 naneos_devices-1.0.9/src/naneos/protobuf/partector2_ble/__init__.py
+-rw-r--r--   0        0        0     5803 2023-12-08 07:28:55.574174 naneos_devices-1.0.9/src/naneos/protobuf/partector2_ble/partector2_ble.py
+-rw-r--r--   0        0        0     2545 2023-12-01 13:23:20.872321 naneos_devices-1.0.9/src/naneos/protobuf/protoV1.proto
+-rw-r--r--   0        0        0     4915 2023-12-08 07:28:55.546753 naneos_devices-1.0.9/src/naneos/protobuf/protoV1_pb2.py
+-rw-r--r--   0        0        0    10588 2023-12-10 20:24:54.999531 naneos_devices-1.0.9/src/naneos/protobuf/protoV1_pb2.pyi
+-rw-r--r--   0        0        0     6155 2023-12-15 11:00:13.047046 naneos_devices-1.0.9/src/naneos/protobuf/protobuf.py
+-rw-r--r--   0        0        0       95 2023-12-01 09:24:51.115584 naneos_devices-1.0.9/src/naneos/py.typed
+-rw-r--r--   0        0        0      104 2023-12-08 08:27:14.516691 naneos_devices-1.0.9/src/naneos/serial_utils/__init__.py
+-rw-r--r--   0        0        0     1337 2023-12-15 22:46:52.413440 naneos_devices-1.0.9/src/naneos/serial_utils/list_serial_ports.py
+-rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 naneos_devices-1.0.9/PKG-INFO
```

### Comparing `naneos_devices-1.0.8/LICENSE.txt` & `naneos_devices-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/README.md` & `naneos_devices-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/pyproject.toml` & `naneos_devices-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "naneos-devices"
 packages = [
     { include = "naneos", from = "src" },
 ]
-version = "1.0.8"
+version = "1.0.9"
 description = "Naneos gmbh python backend"
 authors = ["Mario Huegi <mario.huegi@naneos.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/naneos-org/python-naneos-devices"
 documentation = "https://naneos-org.github.io/python-naneos-devices/"
 classifiers = [
```

### Comparing `naneos_devices-1.0.8/src/naneos/iotweb/download/downloader.py` & `naneos_devices-1.0.9/src/naneos/iotweb/download/downloader.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/iotweb/iotweb.py` & `naneos_devices-1.0.9/src/naneos/iotweb/iotweb.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/iotweb/partector2_pro_garage_upload.py` & `naneos_devices-1.0.9/src/naneos/iotweb/partector2_pro_garage_upload.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/logger/custom_logger.py` & `naneos_devices-1.0.9/src/naneos/logger/custom_logger.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector/blueprints/_data_structure.py` & `naneos_devices-1.0.9/src/naneos/partector/blueprints/_data_structure.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector/blueprints/_partectorCheckerThread.py` & `naneos_devices-1.0.9/src/naneos/partector/blueprints/_partectorCheckerThread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 from threading import Event, Thread
+import time
 
 from naneos.logger.custom_logger import get_naneos_logger
 
 logger = get_naneos_logger(__name__)
 
 
 class PartectorCheckerThread(Thread):
     # from naneos.partector.blueprints._partector_blueprint import PartectorBluePrint
 
     def __init__(self, partector) -> None:
         super().__init__()
         self.partector = partector
 
+        self._last_message_received = time.time()
+
         self._stop_event = Event()
         self.start()
 
     def stop(self) -> None:
         self._stop_event.set()
 
     def run(self) -> None:
         # every 2.1 seconds check if device is still connected
-        while not self._stop_event.wait(2.1):
+        while not self._stop_event.wait(0.5):
+            if time.time() - self._last_message_received < 5:
+                continue
+
             try:
                 self.partector._run_check_connection()
             except Exception as e:
                 logger.error(e)
+
+    def notify_message_received(self) -> None:
+        self._last_message_received = time.time()
```

### Comparing `naneos_devices-1.0.8/src/naneos/partector/blueprints/_partector_blueprint.py` & `naneos_devices-1.0.9/src/naneos/partector/blueprints/_partector_blueprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import ABC, abstractmethod
+import collections
 from datetime import datetime, timezone
 from queue import Queue
+import stat
 from threading import Event, Thread
 import time
 from typing import Any, Callable, Optional
 
 import pandas
 import serial
 
@@ -28,27 +30,32 @@
         self._init(serial_number, port, verb_freq)
 
     def _init_variables(self) -> None:
         self._connected = False
         self._serial_number: Optional[int] = None
         self._port: Optional[str] = ""
         self._ser: Optional[serial.Serial] = None
-        self._time_last_connection_check = time.time()
+        self._time_last_message_received = time.time()
 
     def close(self, blocking: bool = False, shutdown: bool = False) -> None:
         """Closes the serial connection and stops the reading thread."""
         self._close(blocking, shutdown)
 
     def _checker_thread(self) -> None:
-        while not self.thread_event.wait(2.1):
-            try:
-                # logger.info("Checking device connection...")
-                self._run_check_connection()
-            except Exception as e:
-                logger.error(e)
+        while not self.thread_event.wait(0.5):
+            if time.time() - self._time_last_message_received > 5:
+                try:
+                    logger.info("Checking device connection...")
+                    self._run_check_connection()
+                    self._time_last_message_received = time.time()
+                except Exception as e:
+                    logger.error(e)
+
+    def _notify_message_received(self) -> None:
+        self._time_last_message_received = time.time()
 
     def run(self) -> None:
         """Thread method. Reads the serial port and puts the data into the queue."""
 
         # run _checker_thread in own thread
         checker_thread = Thread(target=self._checker_thread)
         checker_thread.start()
@@ -185,14 +192,16 @@
 
         if not line or line == "":
             return
 
         unix_timestamp = int(datetime.now(tz=timezone.utc).timestamp())
         data = [unix_timestamp] + line.split("\t")
 
+        self._notify_message_received()
+
         if len(data) == len(self._data_structure):
             if self._queue.full():
                 self._queue.get()
             self._queue.put(data)
         else:
             if self._queue_info.full():
                 self._queue_info.get()
@@ -412,14 +421,16 @@
 
 if __name__ == "__main__":
     from naneos.partector import Partector2, Partector2ProGarage  # noqa: F401
 
     def test_callback(state: bool) -> None:
         logger.info(f"Catalyst state changed to {state}.")
 
-    partector = Partector2ProGarage(serial_number=8440, callback_catalyst=test_callback)
+    partector = Partector2ProGarage(
+        serial_number=8421, callback_catalyst=test_callback, verb_freq=0
+    )
     # partector = Partector2(serial_number=8112)
 
-    time.sleep(5)
+    time.sleep(20)
 
     print(partector.get_data_pandas())
     partector.close(blocking=True)
```

### Comparing `naneos_devices-1.0.8/src/naneos/partector/partector1.py` & `naneos_devices-1.0.9/src/naneos/partector/partector1.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector/partector2.py` & `naneos_devices-1.0.9/src/naneos/partector/partector2.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector/partector2_pro.py` & `naneos_devices-1.0.9/src/naneos/partector/partector2_pro.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector/partector2_pro_garage.py` & `naneos_devices-1.0.9/src/naneos/partector/partector2_pro_garage.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,16 @@
     def _init_serial_data_structure(self) -> None:
         self._data_structure = PARTECTOR2_PRO_GARAGE_DATA_STRUCTURE
 
     def _set_verbose_freq(self, freq: int) -> None:
         if freq == 0:
             self._write_line("X0000!")
         else:
-            self._write_line("X0006!")
+            self._write_line("M0004!")  # activates size dist mode
+            self._write_line("X0006!")  # activates verbose mode
 
     def set_catalyst_state(self, state: str) -> None:
         """Sets the catalyst state to on, off or auto."""
         if not self._connected:
             return
 
         if state == "on":
@@ -81,14 +82,16 @@
         else:
             self._put_line_to_queue(line)
 
     def _put_line_to_queue(self, line: str, cs_command: Optional[bool] = None) -> None:
         unix_timestamp = int(datetime.now(tz=timezone.utc).timestamp())
         data = [unix_timestamp] + line.split("\t")
 
+        self._notify_message_received()
+
         if len(data) != len(self._data_structure):
             self._put_to_info_queue(data)
             return
 
         state: Optional[int] = None
         try:
             state = int(data[-1])
```

### Comparing `naneos_devices-1.0.8/src/naneos/partector/scan_for_partector.py` & `naneos_devices-1.0.9/src/naneos/partector/scan_for_partector.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector_ble/partector_ble.py` & `naneos_devices-1.0.9/src/naneos/partector_ble/partector_ble.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector_ble/partector_ble_device.py` & `naneos_devices-1.0.9/src/naneos/partector_ble/partector_ble_device.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/partector_ble/test.py` & `naneos_devices-1.0.9/src/naneos/partector_ble/test.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/protobuf/partector2_ble/partector2_ble.py` & `naneos_devices-1.0.9/src/naneos/protobuf/partector2_ble/partector2_ble.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/protobuf/protoV1.proto` & `naneos_devices-1.0.9/src/naneos/protobuf/protoV1.proto`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/protobuf/protoV1_pb2.py` & `naneos_devices-1.0.9/src/naneos/protobuf/protoV1_pb2.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/protobuf/protoV1_pb2.pyi` & `naneos_devices-1.0.9/src/naneos/protobuf/protoV1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/protobuf/protobuf.py` & `naneos_devices-1.0.9/src/naneos/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/src/naneos/serial_utils/list_serial_ports.py` & `naneos_devices-1.0.9/src/naneos/serial_utils/list_serial_ports.py`

 * *Files identical despite different names*

### Comparing `naneos_devices-1.0.8/PKG-INFO` & `naneos_devices-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naneos-devices
-Version: 1.0.8
+Version: 1.0.9
 Summary: Naneos gmbh python backend
 Home-page: https://github.com/naneos-org/python-naneos-devices
 License: MIT
 Author: Mario Huegi
 Author-email: mario.huegi@naneos.ch
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
```

