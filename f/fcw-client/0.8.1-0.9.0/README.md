# Comparing `tmp/fcw_client-0.8.1.tar.gz` & `tmp/fcw_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_client-0.8.1.tar", max compression
+gzip compressed data, was "fcw_client-0.9.0.tar", max compression
```

## Comparing `fcw_client-0.8.1.tar` & `fcw_client-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      232 2023-07-19 16:44:57.000000 fcw_client-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_client-0.8.1/examples/fcw_client_python/__init__.py
--rw-r--r--   0        0        0     5749 2023-12-11 18:41:41.000000 fcw_client-0.8.1/examples/fcw_client_python/client_python.py
--rw-r--r--   0        0        0     6604 2023-12-11 18:44:57.000000 fcw_client-0.8.1/examples/fcw_client_python/client_python_middleware.py
--rw-r--r--   0        0        0     4135 2023-12-11 18:46:26.000000 fcw_client-0.8.1/examples/fcw_client_python/client_python_simple.py
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_client-0.8.1/fcw_client/__init__.py
--rw-r--r--   0        0        0    12422 2023-12-11 16:44:15.000000 fcw_client-0.8.1/fcw_client/client_common.py
--rw-r--r--   0        0        0      859 2023-12-11 18:50:39.000000 fcw_client-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 fcw_client-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-07-19 16:44:57.000000 fcw_client-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_client-0.9.0/examples/fcw_client_python/__init__.py
+-rw-r--r--   0        0        0     5902 2023-12-18 10:08:07.000000 fcw_client-0.9.0/examples/fcw_client_python/client_python.py
+-rw-r--r--   0        0        0     6757 2023-12-18 10:08:16.000000 fcw_client-0.9.0/examples/fcw_client_python/client_python_middleware.py
+-rw-r--r--   0        0        0     4135 2023-12-11 18:46:26.000000 fcw_client-0.9.0/examples/fcw_client_python/client_python_simple.py
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_client-0.9.0/fcw_client/__init__.py
+-rw-r--r--   0        0        0    12422 2023-12-18 10:05:21.000000 fcw_client-0.9.0/fcw_client/client_common.py
+-rw-r--r--   0        0        0      941 2023-12-18 10:11:03.000000 fcw_client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 fcw_client-0.9.0/PKG-INFO
```

### Comparing `fcw_client-0.8.1/examples/fcw_client_python/client_python.py` & `fcw_client-0.9.0/examples/fcw_client_python/client_python.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import logging
 import signal
 import sys
 import time
 import traceback
 from argparse import ArgumentParser
 from pathlib import Path
+from typing import Optional
 
 import cv2
 
 # FCW and 5G-ERA stuff.
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.exceptions import BackPressureException
 from era_5g_interface.utils.rate_timer import RateTimer
 from fcw_client.client_common import CollisionWarningClient, StreamType
 
 # Set logging.
-logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
+logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
 logger = logging.getLogger("FCW client python")
 
 # Testing video file.
 TEST_VIDEO_FILE = str("../../../videos/video3.mp4")
 # TEST_VIDEO_FILE = str("rtsp://127.0.0.1:8554/webcam.h264")
 # TEST_VIDEO_FILE = str("../../../videos/bringauto_2023-03-20.mp4")
 
@@ -30,22 +31,26 @@
 
 # Testing camera settings - specific for the particular input
 CAMERA_CONFIG_FILE = Path("../../../videos/video3.yaml")
 # CAMERA_CONFIG_FILE = Path("../../../videos/bringauto.yaml")
 
 # stopped flag for SIGTERM handler (stopping video frames sending).
 stopped = False
-collision_warning_client = None
+collision_warning_client: Optional[CollisionWarningClient] = None
 
 
 def signal_handler(sig: int, *_) -> None:
     """Signal handler for SIGTERM and SIGINT."""
 
     logger.info(f"Terminating ({signal.Signals(sig).name}) ...")
     global stopped
+    if stopped:
+        if collision_warning_client is not None:
+            collision_warning_client.stop()
+        sys.exit(1)
     stopped = True
 
 
 signal.signal(signal.SIGTERM, signal_handler)
 signal.signal(signal.SIGINT, signal_handler)
 
 
@@ -127,21 +132,19 @@
             rate_timer.sleep()
         end_time = time.perf_counter_ns()
         logger.info(f"Total streaming time: {(end_time - start_time) * 1.0e-9:.3f}s")
         cap.release()
 
     except FailedToConnect as ex:
         logger.error(f"Failed to connect to server: {ex}")
-        sys.exit(1)
     except KeyboardInterrupt:
         logger.info("Terminating ...")
     except Exception as ex:
         traceback.print_exc()
         logger.error(f"Exception: {repr(ex)}")
-        sys.exit(1)
     finally:
         if collision_warning_client is not None:
             collision_warning_client.stop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fcw_client-0.8.1/examples/fcw_client_python/client_python_middleware.py` & `fcw_client-0.9.0/examples/fcw_client_python/client_python_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import os
 import signal
 import sys
 import time
 import traceback
 from argparse import ArgumentParser
 from pathlib import Path
+from typing import Optional
 
 import cv2
 
 # FCW and 5G-ERA stuff.
 from era_5g_client.dataclasses import MiddlewareInfo
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.exceptions import BackPressureException
 from era_5g_interface.utils.rate_timer import RateTimer
 from fcw_client.client_common import CollisionWarningClient, StreamType, MiddlewareAllInfo
 
 # Set logging.
-logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
+logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s")
 logger = logging.getLogger("FCW client python")
 
 # Testing video file.
 TEST_VIDEO_FILE = str("../../../videos/video3.mp4")
 # TEST_VIDEO_FILE = str("rtsp://127.0.0.1:8554/webcam.h264")
 # TEST_VIDEO_FILE = str("../../../videos/bringauto_2023-03-20.mp4")
 
@@ -32,15 +33,15 @@
 
 # Testing camera settings - specific for the particular input
 CAMERA_CONFIG_FILE = Path("../../../videos/video3.yaml")
 # CAMERA_CONFIG_FILE = Path("../../../videos/bringauto.yaml")
 
 # stopped flag for SIGTERM handler (stopping video frames sending).
 stopped = False
-collision_warning_client = None
+collision_warning_client: Optional[CollisionWarningClient] = None
 
 MIDDLEWARE_ADDRESS = os.getenv("MIDDLEWARE_ADDRESS", "127.0.0.1")
 # middleware user ID
 MIDDLEWARE_USER = os.getenv("MIDDLEWARE_USER", "00000000-0000-0000-0000-000000000000")
 # middleware password
 MIDDLEWARE_PASSWORD = os.getenv("MIDDLEWARE_PASSWORD", "password")
 # middleware NetApp id (task id)
@@ -50,14 +51,18 @@
 
 
 def signal_handler(sig: int, *_) -> None:
     """Signal handler for SIGTERM and SIGINT."""
 
     logger.info(f"Terminating ({signal.Signals(sig).name}) ...")
     global stopped
+    if stopped:
+        if collision_warning_client is not None:
+            collision_warning_client.stop()
+        sys.exit(1)
     stopped = True
 
 
 signal.signal(signal.SIGTERM, signal_handler)
 signal.signal(signal.SIGINT, signal_handler)
 
 
@@ -144,21 +149,19 @@
             rate_timer.sleep()
         end_time = time.perf_counter_ns()
         logger.info(f"Total streaming time: {(end_time - start_time) * 1.0e-9:.3f}s")
         cap.release()
 
     except FailedToConnect as ex:
         logger.error(f"Failed to connect to server: {ex}")
-        sys.exit(1)
     except KeyboardInterrupt:
         logger.info("Terminating ...")
     except Exception as ex:
         traceback.print_exc()
         logger.error(f"Exception: {repr(ex)}")
-        sys.exit(1)
     finally:
         if collision_warning_client is not None:
             collision_warning_client.stop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fcw_client-0.8.1/examples/fcw_client_python/client_python_simple.py` & `fcw_client-0.9.0/examples/fcw_client_python/client_python_simple.py`

 * *Files identical despite different names*

### Comparing `fcw_client-0.8.1/fcw_client/client_common.py` & `fcw_client-0.9.0/fcw_client/client_common.py`

 * *Files identical despite different names*

### Comparing `fcw_client-0.8.1/pyproject.toml` & `fcw_client-0.9.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "fcw-client"
-version = "0.8.1"
+version = "0.9.0"
 description = "Early collision warning Network Application for Transportation use case - client part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_client"}, {include = "fcw_client_python", from = "examples"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pyyaml = ">=6.0"
 opencv-python = ">=4.8"
-era-5g-client = "^0.8.0"
-era-5g-interface = "^0.7.0"
-fcw-core-utils = "^0.8.0"
+era-5g-client = "^0.9.0"
+era-5g-interface = "^0.8.0"
+fcw-core-utils = "^0.9.0"
 
 [tool.poetry.scripts]
 fcw_client_python = "fcw_client_python.client_python:main"
+fcw_client_python_middleware = "fcw_client_python.client_python_middleware:main"
 fcw_client_python_simple = "fcw_client_python.client_python_simple:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fcw_client-0.8.1/PKG-INFO` & `fcw_client-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fcw-client
-Version: 0.8.1
+Version: 0.9.0
 Summary: Early collision warning Network Application for Transportation use case - client part
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
-Requires-Dist: era-5g-client (>=0.8.0,<0.9.0)
-Requires-Dist: era-5g-interface (>=0.7.0,<0.8.0)
-Requires-Dist: fcw-core-utils (>=0.8.0,<0.9.0)
+Requires-Dist: era-5g-client (>=0.9.0,<0.10.0)
+Requires-Dist: era-5g-interface (>=0.8.0,<0.9.0)
+Requires-Dist: fcw-core-utils (>=0.9.0,<0.10.0)
 Requires-Dist: opencv-python (>=4.8)
 Requires-Dist: pyyaml (>=6.0)
 Project-URL: Repository, https://github.com/5G-ERA/CollisionWarningService
 Description-Content-Type: text/markdown
 
 # Forward Collision Warning - client part
```

