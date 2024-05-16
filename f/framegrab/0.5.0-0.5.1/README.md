# Comparing `tmp/framegrab-0.5.0.tar.gz` & `tmp/framegrab-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.5.0.tar", max compression
+gzip compressed data, was "framegrab-0.5.1.tar", max compression
```

## Comparing `framegrab-0.5.0.tar` & `framegrab-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1071 2024-03-25 22:53:12.629022 framegrab-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     9217 2024-03-25 22:53:12.629022 framegrab-0.5.0/README.md
--rw-r--r--   0        0        0      732 2024-03-25 22:53:12.629022 framegrab-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      512 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/cli/__init__.py
--rw-r--r--   0        0        0     1600 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/cli/autodiscover.py
--rw-r--r--   0        0        0     2102 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/cli/clitools.py
--rwxr-xr-x   0        0        0      297 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/cli/main.py
--rw-r--r--   0        0        0     1843 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/cli/preview.py
--rw-r--r--   0        0        0    42916 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2533 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/motion.py
--rw-r--r--   0        0        0      698 2024-03-25 22:53:12.629022 framegrab-0.5.0/src/framegrab/unavailable_module.py
--rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 framegrab-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-16 19:05:28.745376 framegrab-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     9217 2024-05-16 19:05:28.745376 framegrab-0.5.1/README.md
+-rw-r--r--   0        0        0      732 2024-05-16 19:05:28.745376 framegrab-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      512 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/autodiscover.py
+-rw-r--r--   0        0        0     2102 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/clitools.py
+-rwxr-xr-x   0        0        0      297 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/main.py
+-rw-r--r--   0        0        0     1843 2024-05-16 19:05:28.745376 framegrab-0.5.1/src/framegrab/cli/preview.py
+-rw-r--r--   0        0        0    42610 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2533 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/motion.py
+-rw-r--r--   0        0        0      698 2024-05-16 19:05:28.749377 framegrab-0.5.1/src/framegrab/unavailable_module.py
+-rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 framegrab-0.5.1/PKG-INFO
```

### Comparing `framegrab-0.5.0/LICENSE.txt` & `framegrab-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/README.md` & `framegrab-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/pyproject.toml` & `framegrab-0.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "framegrab"
-version = "0.5.0"
+version = "0.5.1"
 description = "Easily grab frames from cameras or streams"
 authors = ["Groundlight <info@groundlight.ai>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.groundlight.ai/"
 repository = "https://github.com/groundlight/framegrab"
```

### Comparing `framegrab-0.5.0/src/framegrab/__init__.py` & `framegrab-0.5.1/src/framegrab/__init__.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/src/framegrab/cli/autodiscover.py` & `framegrab-0.5.1/src/framegrab/cli/autodiscover.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/src/framegrab/cli/clitools.py` & `framegrab-0.5.1/src/framegrab/cli/clitools.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/src/framegrab/cli/preview.py` & `framegrab-0.5.1/src/framegrab/cli/preview.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/src/framegrab/grabber.py` & `framegrab-0.5.1/src/framegrab/grabber.py`

 * *Files 3% similar despite different names*

```diff
@@ -312,20 +312,29 @@
                 "Pass in warmup_delay = 0 to suppress this behavior."
             )
             time.sleep(warmup_delay)
 
         return grabbers
 
     @abstractmethod
+    def _grab_implementation(self) -> np.ndarray:
+        """Each FrameGrabber must implement its own method of grabbing"""
+        pass
+
     def grab(self) -> np.ndarray:
-        """Read a frame from the camera, zoom and crop if called for, and then perform any camera-specific
-        postprocessing operations.
+        """Read a frame from the camera and perform post processing operations such as zoom, crop and rotation if necessary.
         Returns a frame.
         """
-        pass
+        frame = self._grab_implementation()
+
+        # apply post processing operations
+        frame = self._crop(frame)
+        frame = self._digital_zoom(frame)
+        frame = self._rotate(frame)
+        return frame
 
     def _autogenerate_name(self) -> None:
         """For generating and assigning unique names for unnamed FrameGrabber objects.
 
         Attempts to incorporate a unique identifier (serial number, url, etc.) into each
         camera name. If no unique identifier is available, a counter is used instead.
         """
@@ -343,22 +352,14 @@
             FrameGrabber.unnamed_grabber_count += 1
             unnamed_grabber_id = FrameGrabber.unnamed_grabber_count
 
         input_type = self.config["input_type"]
         autogenerated_name = f"{input_type.upper()} Camera - {unnamed_grabber_id}"
         self.config["name"] = autogenerated_name
 
-    def _process_frame(self, frame: np.ndarray) -> np.ndarray:
-        """Apply _crop, _digital_zoom, and _rotate to the provided frame.
-        as specified in options."""
-        frame = self._crop(frame)
-        frame = self._digital_zoom(frame)
-        frame = self._rotate(frame)
-        return frame
-
     def _crop(self, frame: np.ndarray) -> np.ndarray:
         """Looks at FrameGrabber's options and decides to either crop by pixels or
         in a relative manner (normalized).
 
         Returns a cropped frame.
         """
         options = self.config.get("options", {})
@@ -554,22 +555,21 @@
         # A valid capture has been found, saving it for later
         self.capture = capture
 
         # Log the current camera index as 'in use' to prevent other GenericUSBFrameGrabbers from stepping on it
         self.idx = idx
         GenericUSBFrameGrabber.indices_in_use.add(idx)
 
-    def grab(self) -> np.ndarray:
+    def _grab_implementation(self) -> np.ndarray:
         # OpenCV VideoCapture buffers frames by default. It's usually not possible to turn buffering off.
         # Buffer can be set as low as 1, but even still, if we simply read once, we will get the buffered (stale) frame.
         # Assuming buffer size of 1, we need to read twice to get the current frame.
         for _ in range(2):
             _, frame = self.capture.read()
 
-        frame = self._process_frame(frame)
         return frame
 
     def release(self) -> None:
         GenericUSBFrameGrabber.indices_in_use.remove(self.idx)
         self.capture.release()
 
     def _apply_camera_specific_options(self, options: dict) -> None:
@@ -704,15 +704,15 @@
         logger.debug(f"Initialized video capture with backend={self.capture.getBackendName()}")
 
     def _close_connection(self):
         with self.lock:
             if self.capture is not None:
                 self.capture.release()
 
-    def grab(self) -> np.ndarray:
+    def _grab_implementation(self) -> np.ndarray:
         if not self.keep_connection_open:
             self._open_connection()
             try:
                 return self._grab_open()
             finally:
                 self._close_connection()
         else:
@@ -789,23 +789,20 @@
         self.config["id"] = {"serial_number": curr_serial_number}
 
         # A valid camera has been found, remember the serial_number to prevent
         # other FrameGrabbers from using it
         self.camera = camera
         BaslerFrameGrabber.serial_numbers_in_use.add(self.config["id"]["serial_number"])
 
-    def grab(self) -> np.ndarray:
+    def _grab_implementation(self) -> np.ndarray:
         with self.camera.GrabOne(2000) as result:
             if result.GrabSucceeded():
                 # Convert the image to BGR for OpenCV
                 image = self.converter.Convert(result)
                 frame = image.GetArray()
-
-                # crop, zoom, rotate as needed
-                frame = self._process_frame(frame)
             else:
                 error_info = {
                     "ErrorCode": result.GetErrorCode(),
                     "PayloadSize": result.GetPayloadSize(),
                     "ID": result.GetID(),
                     "BlockID": result.GetBlockID(),
                     "Width": result.GetWidth(),
@@ -880,30 +877,26 @@
         # A valid pipeline was found, save the pipeline and RealSense config for later
         self.pipeline = pipeline
         self.rs_config = rs_config
 
         # In case the serial_number wasn't provided by the user, add it to the config
         self.config["id"] = {"serial_number": curr_serial_number}
 
-    def grab(self) -> np.ndarray:
+    def _grab_implementation(self) -> np.ndarray:
         frames = self.pipeline.wait_for_frames()
 
         # Convert color images to numpy arrays and convert from RGB to BGR
         color_frame = frames.get_color_frame()
         color_image = cv2.cvtColor(np.asanyarray(color_frame.get_data()), cv2.COLOR_BGR2RGB)
 
-        # Crop, zoom and rotate as needed
-        color_image = self._process_frame(color_image)
-
         # If side_by_side is enabled, get a depth frame and horizontally stack it with color frame
         display_side_by_side = self.config.get("options", {}).get("depth", {}).get("side_by_side")
         if display_side_by_side:
             depth_frame = frames.get_depth_frame()
             depth_image = np.asanyarray(depth_frame.get_data())
-            depth_image = self._process_frame(depth_image)
             return self._horizontally_stack(depth_image, color_image)
         else:
             return color_image
 
     def _horizontally_stack(self, depth_image: np.ndarray, color_image: np.ndarray) -> np.ndarray:
         """Merges color image and depth image into a wider image, all in RGB"""
 
@@ -973,23 +966,18 @@
             )
 
         MockFrameGrabber.serial_numbers_in_use.add(curr_serial_number)
 
         # In case the serial_number wasn't provided by the user, add it to the config
         self.config["id"] = {"serial_number": curr_serial_number}
 
-    def grab(self) -> np.ndarray:
+    def _grab_implementation(self) -> np.ndarray:
         width = self.config.get("options", {}).get("resolution", {}).get("width", 640)
         height = self.config.get("options", {}).get("resolution", {}).get("height", 480)
 
-        frame = np.zeros((height, width, 3), dtype=np.uint8)
-
-        # Crop, zoom and rotate as needed
-        frame = self._process_frame(frame)
-
-        return frame
+        return np.zeros((height, width, 3), dtype=np.uint8)
 
     def release(self) -> None:
         MockFrameGrabber.serial_numbers_in_use.remove(self.config["id"]["serial_number"])
 
     def _apply_camera_specific_options(self, options: dict) -> None:
         pass  # no action necessary for mock cameras
```

### Comparing `framegrab-0.5.0/src/framegrab/motion.py` & `framegrab-0.5.1/src/framegrab/motion.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/src/framegrab/unavailable_module.py` & `framegrab-0.5.1/src/framegrab/unavailable_module.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.5.0/PKG-INFO` & `framegrab-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.5.0
+Version: 0.5.1
 Summary: Easily grab frames from cameras or streams
 Home-page: https://www.groundlight.ai/
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

