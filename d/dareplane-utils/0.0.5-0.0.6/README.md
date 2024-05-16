# Comparing `tmp/dareplane_utils-0.0.5.tar.gz` & `tmp/dareplane_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dareplane_utils-0.0.5.tar", last modified: Tue Apr 23 18:28:24 2024, max compression
+gzip compressed data, was "dareplane_utils-0.0.6.tar", last modified: Thu May 16 10:14:37 2024, max compression
```

## Comparing `dareplane_utils-0.0.5.tar` & `dareplane_utils-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.758080 dareplane_utils-0.0.5/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     1069 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/LICENSE
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-04-23 18:28:24.757894 dareplane_utils-0.0.5/PKG-INFO
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3670 2024-04-23 18:24:44.000000 dareplane_utils-0.0.5/README.md
--rw-r--r--   0 matthias.dold   (502) staff       (20)      522 2024-04-23 18:27:30.000000 dareplane_utils-0.0.5/pyproject.toml
--rw-r--r--   0 matthias.dold   (502) staff       (20)       38 2024-04-23 18:28:24.758127 dareplane_utils-0.0.5/setup.cfg
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.754707 dareplane_utils-0.0.5/src/
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.754974 dareplane_utils-0.0.5/src/dareplane_utils/
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.756306 dareplane_utils-0.0.5/src/dareplane_utils/default_server/
--rw-r--r--   0 matthias.dold   (502) staff       (20)        0 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/__init__.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4295 2024-01-15 13:15:40.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/functions.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)    12801 2024-04-23 17:44:11.000000 dareplane_utils-0.0.5/src/dareplane_utils/default_server/server.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.756622 dareplane_utils-0.0.5/src/dareplane_utils/general/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     6827 2024-04-13 14:51:34.000000 dareplane_utils-0.0.5/src/dareplane_utils/general/ringbuffer.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)      777 2024-04-09 14:20:21.000000 dareplane_utils-0.0.5/src/dareplane_utils/general/time.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757014 dareplane_utils-0.0.5/src/dareplane_utils/logging/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     1559 2024-01-19 11:17:32.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/logger.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     5739 2024-04-23 17:29:50.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/server.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)      767 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/src/dareplane_utils/logging/ujson_socket_handler.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757140 dareplane_utils-0.0.5/src/dareplane_utils/stream_watcher/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4955 2024-04-12 09:08:14.000000 dareplane_utils-0.0.5/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757690 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/PKG-INFO
--rw-r--r--   0 matthias.dold   (502) staff       (20)      756 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/SOURCES.txt
--rw-r--r--   0 matthias.dold   (502) staff       (20)        1 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/dependency_links.txt
--rw-r--r--   0 matthias.dold   (502) staff       (20)       16 2024-04-23 18:28:24.000000 dareplane_utils-0.0.5/src/dareplane_utils.egg-info/top_level.txt
-drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-04-23 18:28:24.757519 dareplane_utils-0.0.5/tests/
--rw-r--r--   0 matthias.dold   (502) staff       (20)     2541 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/tests/test_default_server_process_book_keeping.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     2124 2023-06-06 11:52:12.000000 dareplane_utils-0.0.5/tests/test_default_server_thread_book_keeping.py
--rw-r--r--   0 matthias.dold   (502) staff       (20)     4120 2023-06-07 19:54:43.000000 dareplane_utils-0.0.5/tests/test_logging_server_client_communication.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.601512 dareplane_utils-0.0.6/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     1069 2023-06-06 11:52:12.000000 dareplane_utils-0.0.6/LICENSE
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-05-16 10:14:37.601288 dareplane_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3670 2024-04-23 18:24:44.000000 dareplane_utils-0.0.6/README.md
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      522 2024-05-16 10:13:40.000000 dareplane_utils-0.0.6/pyproject.toml
+-rw-r--r--   0 matthias.dold   (502) staff       (20)       38 2024-05-16 10:14:37.601559 dareplane_utils-0.0.6/setup.cfg
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.596748 dareplane_utils-0.0.6/src/
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.597019 dareplane_utils-0.0.6/src/dareplane_utils/
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.598389 dareplane_utils-0.0.6/src/dareplane_utils/default_server/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)        0 2023-06-06 11:52:12.000000 dareplane_utils-0.0.6/src/dareplane_utils/default_server/__init__.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     4295 2024-01-15 13:15:40.000000 dareplane_utils-0.0.6/src/dareplane_utils/default_server/functions.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)    12801 2024-04-23 17:44:11.000000 dareplane_utils-0.0.6/src/dareplane_utils/default_server/server.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.598752 dareplane_utils-0.0.6/src/dareplane_utils/general/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     5660 2024-05-16 10:11:09.000000 dareplane_utils-0.0.6/src/dareplane_utils/general/ringbuffer.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      777 2024-04-09 14:20:21.000000 dareplane_utils-0.0.6/src/dareplane_utils/general/time.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.599267 dareplane_utils-0.0.6/src/dareplane_utils/logging/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     1559 2024-01-19 11:17:32.000000 dareplane_utils-0.0.6/src/dareplane_utils/logging/logger.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     5739 2024-04-23 17:29:50.000000 dareplane_utils-0.0.6/src/dareplane_utils/logging/server.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      767 2023-06-06 11:52:12.000000 dareplane_utils-0.0.6/src/dareplane_utils/logging/ujson_socket_handler.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.599402 dareplane_utils-0.0.6/src/dareplane_utils/stream_watcher/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     5608 2024-05-16 10:11:09.000000 dareplane_utils-0.0.6/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.601052 dareplane_utils-0.0.6/src/dareplane_utils.egg-info/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     3995 2024-05-16 10:14:37.000000 dareplane_utils-0.0.6/src/dareplane_utils.egg-info/PKG-INFO
+-rw-r--r--   0 matthias.dold   (502) staff       (20)      809 2024-05-16 10:14:37.000000 dareplane_utils-0.0.6/src/dareplane_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias.dold   (502) staff       (20)        1 2024-05-16 10:14:37.000000 dareplane_utils-0.0.6/src/dareplane_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias.dold   (502) staff       (20)       16 2024-05-16 10:14:37.000000 dareplane_utils-0.0.6/src/dareplane_utils.egg-info/top_level.txt
+drwxr-xr-x   0 matthias.dold   (502) staff       (20)        0 2024-05-16 10:14:37.600806 dareplane_utils-0.0.6/tests/
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     2541 2023-06-06 11:52:12.000000 dareplane_utils-0.0.6/tests/test_default_server_process_book_keeping.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     2123 2024-05-16 10:11:09.000000 dareplane_utils-0.0.6/tests/test_default_server_thread_book_keeping.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     4120 2023-06-07 19:54:43.000000 dareplane_utils-0.0.6/tests/test_logging_server_client_communication.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     1011 2024-05-16 10:11:09.000000 dareplane_utils-0.0.6/tests/test_ringbuffer.py
+-rw-r--r--   0 matthias.dold   (502) staff       (20)     2653 2024-05-16 10:11:09.000000 dareplane_utils-0.0.6/tests/test_streamwatcher.py
```

### Comparing `dareplane_utils-0.0.5/LICENSE` & `dareplane_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/PKG-INFO` & `dareplane_utils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dareplane_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Default utilities for the dareplane platform
 Author-email: Matthias Dold <matthias.dold@gmx.net>
 Project-URL: homepage, https://github.com/matthiasdold/dareplane-pyutils
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dareplane_utils-0.0.5/README.md` & `dareplane_utils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/pyproject.toml` & `dareplane_utils-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dareplane_utils"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{name="Matthias Dold", email="matthias.dold@gmx.net"}]
 description = "Default utilities for the dareplane platform"
 readme ="README.md"
 requires-python = ">=3.10"
 
 [project.urls]
 "homepage" = "https://github.com/matthiasdold/dareplane-pyutils"
```

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/default_server/functions.py` & `dareplane_utils-0.0.6/src/dareplane_utils/default_server/functions.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/default_server/server.py` & `dareplane_utils-0.0.6/src/dareplane_utils/default_server/server.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/general/time.py` & `dareplane_utils-0.0.6/src/dareplane_utils/general/time.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/logging/logger.py` & `dareplane_utils-0.0.6/src/dareplane_utils/logging/logger.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/logging/server.py` & `dareplane_utils-0.0.6/src/dareplane_utils/logging/server.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/logging/ujson_socket_handler.py` & `dareplane_utils-0.0.6/src/dareplane_utils/logging/ujson_socket_handler.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py` & `dareplane_utils-0.0.6/src/dareplane_utils/stream_watcher/lsl_stream_watcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 import xmltodict
 
 from dareplane_utils.general.ringbuffer import RingBuffer
 from dareplane_utils.logging.logger import get_logger
 
 logger = get_logger(__name__)
 
-# ch = logging.StreamHandler()
-# ch.setFormatter(logging.Formatter("%(levelname)s - %(asctime)s - %(message)s"))
-# logger.addHandler(ch)
-# logger.setLevel(10)
-#
-#
-
 
 class StreamWatcherNotConnected(ValueError):
     pass
 
 
 def get_streams_names() -> list[str]:
     """Get a list of all available lsl stream names.
@@ -76,15 +69,20 @@
         name : str
             Name tag to identify the manager -> could be same as the LSL stream
             it should be watching
         buffer_size_s : float
             the data buffer size in seconds
         """
         self.name = name
+        # this concerns the ringbuffer
         self.buffer_size_s = buffer_size_s
+
+        # the maximum number of samples to pull in one go
+        self.chunk_buffer_size = 1024 * 32
+
         self.stream = None
         self.inlet = None
         self.buffer = None
 
         # Set after connection
         self.samples: list[list[float]] = []
         self.times: list[float] = []
@@ -140,20 +138,39 @@
 
         # link properties
         self.buffer = self.ring_buffer.buffer
         self.buffer_t = self.ring_buffer.buffer_t
         self.last_t = self.ring_buffer.last_t
         self.curr_i = self.ring_buffer.curr_i
 
+        # to have input from pylsl as numpy directly -> float32 is important!
+        # as this is pylsl default
+        self.chunk_buffer = np.zeros(
+            (self.chunk_buffer_size, len(self.channel_names))
+        ).astype(np.float32)
+
     def update(self):
         """Look for new data and update the buffer"""
-        samples, times = self.inlet.pull_chunk()
-        self.ring_buffer.add_samples(samples, times)
+
+        # This logic works as long as the returned samples are not too many
+        # samples, times = self.inlet.pull_chunk()
+        # Better use the direct assignment
+
+        _, times = self.inlet.pull_chunk(
+            max_samples=self.chunk_buffer_size, dest_obj=self.chunk_buffer
+        )
+
+        if len(times) > 0:
+            samples = self.chunk_buffer[: len(times), :]
+            self.ring_buffer.add_samples(samples, times)
+            self.overwriting_samples(samples)
+            self.n_new += len(times)
+
+    def overwriting_samples(self, samples):
         self.samples = samples
-        self.n_new += len(samples)
 
     def unfold_buffer(self):
         return self.ring_buffer.unfold_buffer()
 
     def unfold_buffer_t(self):
         # Do hstack here as the time buffer will be of dim (n,1) anyways
         return self.ring_buffer.unfold_buffer_t()
```

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils.egg-info/PKG-INFO` & `dareplane_utils-0.0.6/src/dareplane_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dareplane_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Default utilities for the dareplane platform
 Author-email: Matthias Dold <matthias.dold@gmx.net>
 Project-URL: homepage, https://github.com/matthiasdold/dareplane-pyutils
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dareplane_utils-0.0.5/src/dareplane_utils.egg-info/SOURCES.txt` & `dareplane_utils-0.0.6/src/dareplane_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 src/dareplane_utils/general/time.py
 src/dareplane_utils/logging/logger.py
 src/dareplane_utils/logging/server.py
 src/dareplane_utils/logging/ujson_socket_handler.py
 src/dareplane_utils/stream_watcher/lsl_stream_watcher.py
 tests/test_default_server_process_book_keeping.py
 tests/test_default_server_thread_book_keeping.py
-tests/test_logging_server_client_communication.py
+tests/test_logging_server_client_communication.py
+tests/test_ringbuffer.py
+tests/test_streamwatcher.py
```

### Comparing `dareplane_utils-0.0.5/tests/test_default_server_process_book_keeping.py` & `dareplane_utils-0.0.6/tests/test_default_server_process_book_keeping.py`

 * *Files identical despite different names*

### Comparing `dareplane_utils-0.0.5/tests/test_default_server_thread_book_keeping.py` & `dareplane_utils-0.0.6/tests/test_default_server_thread_book_keeping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import pytest
-import time
 import socket
-import psutil
 import threading
+import time
 
-from tests.resources.shared import get_test_thread
-
+import psutil
+import pytest
 
 from dareplane_utils.default_server.server import DefaultServer
 from dareplane_utils.logging.logger import get_logger
+from tests.resources.shared import get_test_thread
 
 logger = get_logger("testlogger")
 
 
 # for checking which process is running at a given port, we can use netstat with e.g.
 # `netstat -anv -p tcp | grep 8080`
```

### Comparing `dareplane_utils-0.0.5/tests/test_logging_server_client_communication.py` & `dareplane_utils-0.0.6/tests/test_logging_server_client_communication.py`

 * *Files identical despite different names*

