# Comparing `tmp/openclip_service-0.1.0.tar.gz` & `tmp/openclip_service-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openclip_service-0.1.0.tar", max compression
+gzip compressed data, was "openclip_service-0.1.1.tar", max compression
```

## Comparing `openclip_service-0.1.0.tar` & `openclip_service-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      171 2024-03-27 10:59:44.000000 openclip_service-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 openclip_service-0.1.0/openclip_service/__init__.py
--rw-r--r--   0        0        0    10933 2024-05-06 14:17:15.000000 openclip_service-0.1.0/openclip_service/clip_worker.py
--rw-r--r--   0        0        0     9077 2024-04-04 09:11:24.000000 openclip_service-0.1.0/openclip_service/service.py
--rw-r--r--   0        0        0      820 2024-04-08 12:47:57.000000 openclip_service-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 openclip_service-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2024-03-27 10:59:44.000000 openclip_service-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 openclip_service-0.1.1/openclip_service/__init__.py
+-rw-r--r--   0        0        0    12489 2024-05-13 14:11:52.000000 openclip_service-0.1.1/openclip_service/clip_worker.py
+-rw-r--r--   0        0        0     9077 2024-04-04 09:11:24.000000 openclip_service-0.1.1/openclip_service/service.py
+-rw-r--r--   0        0        0      871 2024-05-16 15:54:05.000000 openclip_service-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 openclip_service-0.1.1/PKG-INFO
```

### Comparing `openclip_service-0.1.0/openclip_service/clip_worker.py` & `openclip_service-0.1.1/openclip_service/clip_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import open_clip
 import torch
 import yaml
 from PIL import Image
 from torch import Tensor
 
 from era_5g_interface.interface_helpers import LatencyMeasurements
+from era_5g_interface.measuring import Measuring
 
 logger = logging.getLogger(__name__)
 
 
 class CLIPWorker(Thread):
     """CLIP worker. Reads data from passed queue, performs CLIP processing and returns results using callback.
 
@@ -198,39 +199,77 @@
                 continue
 
             self._process_image(metadata, image)
 
         logger.info(f"{self.name} thread is stopping.")
 
 
+measuring_items = {
+    "key_timestamp": 0,
+    "final_timestamp": 0,
+    "worker_recv_timestamp": 0,
+    "worker_before_process_timestamp": 0,
+    "worker_after_process_timestamp": 0,
+    "worker_send_timestamp": 0,
+}
+prefix = f"client-final"
+measuring = Measuring(measuring_items, enabled=True, filename_prefix=prefix)
+
 def visualization(results: [Dict[str, Any]]) -> None:
     """Testing send function - visualization."""
 
+    results_timestamp = time.perf_counter_ns()
+
+    if "timestamp" in results:
+        key_timestamp = results.get("timestamp")
+        recv_timestamp = results.get("recv_timestamp", key_timestamp)
+        send_timestamp = results.get("send_timestamp", 0)
+        timestamp_before_process = results.get("timestamp_before_process", 0)
+        timestamp_after_process = results.get("timestamp_after_process", 0)
+
+    measuring.log_measuring(key_timestamp, "final_timestamp", results_timestamp)
+
+    # Log other misc timestamps from the received message
+    measuring.log_measuring(key_timestamp, "worker_recv_timestamp", recv_timestamp)
+    measuring.log_measuring(
+        key_timestamp,
+        "worker_before_process_timestamp",
+        timestamp_before_process,
+    )
+    measuring.log_measuring(
+        key_timestamp,
+        "worker_after_process_timestamp",
+        timestamp_after_process,
+    )
+    measuring.log_measuring(key_timestamp, "worker_send_timestamp", send_timestamp)
+
+    measuring.store_measuring(key_timestamp)
+
     logger.info(f"{results['texts']}: {results['probs']}")
     logger.info(
         f"delay: "
         f"{(results.get('timestamp_after_process', 0) - results.get('timestamp_before_process', 0)) * 1.0e-9:.3f}s"
     )
-    font = cv2.FONT_HERSHEY_SIMPLEX
-    cv2.putText(
-        results["frame"],
-        f"{results['texts']}: {results['probs']}",
-        (20, 20),
-        font,
-        0.5,
-        (0, 255, 0),
-        1,
-        cv2.LINE_AA,
-    )
-
-    try:
-        cv2.imshow("Results", results["frame"])
-        cv2.waitKey(1)
-    except Exception as ex:
-        logger.error(repr(ex))
+    # font = cv2.FONT_HERSHEY_SIMPLEX
+    # cv2.putText(
+    #     results["frame"],
+    #     f"{results['texts']}: {results['probs']}",
+    #     (20, 20),
+    #     font,
+    #     0.5,
+    #     (0, 255, 0),
+    #     1,
+    #     cv2.LINE_AA,
+    # )
+    #
+    # try:
+    #     cv2.imshow("Results", results["frame"])
+    #     cv2.waitKey(1)
+    # except Exception as ex:
+    #     logger.error(repr(ex))
 
 
 def main() -> None:
     """CLIP worker testing."""
 
     logging.basicConfig(
         stream=sys.stdout, level=logging.DEBUG, format="%(asctime)s [%(levelname)s] %(name)s: %(message)s"
@@ -254,28 +293,30 @@
         ["big car", "small car", "bicycle", "person"],
         ["car on the right", "car on the left", "car in front"],
         ["one person", "no person", "more than 5 people"],
         ["colored cars", "black and white cars"],
         ["the sun shines from the right side", "the sun shines from the left side"],
         ["stone road", "asphalt road", "concrete road", "dirt road"],
         ["I drive in the city", "I drive in the forest", "I drive outside the city"],
-        ["there is a traffic light in front of me",
-         "there is no traffic light in front of me",
-         "there is a traffic sign in front of me",
-         "no sign or traffic light"],
+        [
+            "there is a traffic light in front of me",
+            "there is no traffic light in front of me",
+            "there is a traffic sign in front of me",
+            "no sign or traffic light",
+        ],
         ["the traffic light is red", "the traffic light is green", "the traffic light is orange"],
-        ["it's cloudy, it's clear, it's raining"]
+        ["it's cloudy", "it's clear", "it's raining"],
     ]
 
     while True:
         ret, frame = cap.read()
         if not ret:
             break
 
-        metadata = {
+        metadata = {"timestamp": time.perf_counter_ns(),
             "metadata": {"model_name": "ViT-B-32", "texts": random.choice(texts)}}
         #metadata = {"metadata": {"model_name": "ViT-B-32", "texts": ["car", "road"]}}
         clip_worker._process_image(metadata, frame)
         # time.sleep(1 / 30)
 
 
 if __name__ == "__main__":
```

### Comparing `openclip_service-0.1.0/openclip_service/service.py` & `openclip_service-0.1.1/openclip_service/service.py`

 * *Files identical despite different names*

### Comparing `openclip_service-0.1.0/pyproject.toml` & `openclip_service-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openclip-service"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLIP Service Network Application - service part"
 authors = ["Petr Kleparnik <p.kleparnik@cognitechna.cz>", "Roman Juranek <r.juranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CLIPService"
 packages = [{include = "openclip_service"}]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 pyyaml = ">=6.0.1"
 torch = ">=2.1.0"
 torchvision = ">=0.16.0"
 torchaudio = ">=2.1.0"
 
 [tool.poetry.scripts]
 openclip_service = "openclip_service.service:main"
+clip_worker = "openclip_service.clip_worker:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `openclip_service-0.1.0/PKG-INFO` & `openclip_service-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclip-service
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLIP Service Network Application - service part
 Home-page: https://github.com/5G-ERA/CLIPService
 Author: Petr Kleparnik
 Author-email: p.kleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

