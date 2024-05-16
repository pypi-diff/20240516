# Comparing `tmp/openCV_movement_detection-1.4.tar.gz` & `tmp/openCV_movement_detection-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openCV_movement_detection-1.4.tar", last modified: Fri May 10 09:51:29 2024, max compression
+gzip compressed data, was "openCV_movement_detection-1.5.tar", last modified: Thu May 16 13:44:00 2024, max compression
```

## Comparing `openCV_movement_detection-1.4.tar` & `openCV_movement_detection-1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 09:51:29.906154 openCV_movement_detection-1.4/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:51:29.904649 openCV_movement_detection-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 09:51:29.890369 openCV_movement_detection-1.4/openCV_movement_detection/
--rw-rw-rw-   0        0        0        0 2024-05-10 09:26:55.000000 openCV_movement_detection-1.4/openCV_movement_detection/__init__.py
--rw-rw-rw-   0        0        0     2535 2024-05-10 09:19:53.000000 openCV_movement_detection-1.4/openCV_movement_detection/details_movement.py
--rw-rw-rw-   0        0        0     1684 2024-05-10 09:50:35.000000 openCV_movement_detection-1.4/openCV_movement_detection/video_movement_class.py
-drwxrwxrwx   0        0        0        0 2024-05-10 09:51:29.902648 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/
--rw-rw-rw-   0        0        0      194 2024-05-10 09:51:29.000000 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-10 09:51:29.000000 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 09:51:29.000000 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 09:51:29.000000 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-10 09:51:29.000000 openCV_movement_detection-1.4/openCV_movement_detection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 09:51:29.906154 openCV_movement_detection-1.4/setup.cfg
--rw-rw-rw-   0        0        0      299 2024-05-10 09:51:27.000000 openCV_movement_detection-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:44:00.648887 openCV_movement_detection-1.5/
+-rw-rw-rw-   0        0        0      203 2024-05-16 13:44:00.646868 openCV_movement_detection-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 13:44:00.634538 openCV_movement_detection-1.5/openCV_movement_detection/
+-rw-rw-rw-   0        0        0        0 2024-05-10 09:26:55.000000 openCV_movement_detection-1.5/openCV_movement_detection/__init__.py
+-rw-rw-rw-   0        0        0     2559 2024-05-16 12:28:53.000000 openCV_movement_detection-1.5/openCV_movement_detection/details_movement.py
+-rw-rw-rw-   0        0        0      290 2024-05-16 12:52:31.000000 openCV_movement_detection-1.5/openCV_movement_detection/test file.py
+-rw-rw-rw-   0        0        0     3069 2024-05-16 12:32:52.000000 openCV_movement_detection-1.5/openCV_movement_detection/video_movement_class.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:44:00.645846 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/
+-rw-rw-rw-   0        0        0      203 2024-05-16 13:44:00.000000 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2024-05-16 13:44:00.000000 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:44:00.000000 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-16 13:44:00.000000 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-16 13:44:00.000000 openCV_movement_detection-1.5/openCV_movement_detection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:44:00.648887 openCV_movement_detection-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      320 2024-05-16 12:48:20.000000 openCV_movement_detection-1.5/setup.py
```

### Comparing `openCV_movement_detection-1.4/openCV_movement_detection/details_movement.py` & `openCV_movement_detection-1.5/openCV_movement_detection/details_movement.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,17 +40,17 @@
             circularity = cv2.contourArea(contour) / (np.pi * radius ** 2)
             if circularity < circularity_threshold:
                 return True
 
 
 def text_movement(movement_detected, prev_count, count):
     if movement_detected:
-        return "Movement detected!" + " Between : " + str(prev_count) + " and " + str(count)
+        return "Movement detected!" + " Between : frame " + str(prev_count) + " and frame " + str(count)
     else:
-        return "No movement detected." + " Between : " + str(prev_count) + " and " + str(count)
+        return "No movement detected." + " Between : frame " + str(prev_count) + " and frame " + str(count)
 
 
 def make_video_no_roi(frame, no_rois):
     frame_roi = frame.copy()
     for no_roi in no_rois:
         startX, endX = int(no_roi['startX']), int(no_roi['endX'])
         startY, endY = int(no_roi['startY']), int(no_roi['endY'])
```

### Comparing `openCV_movement_detection-1.4/openCV_movement_detection/video_movement_class.py` & `openCV_movement_detection-1.5/openCV_movement_detection/video_movement_class.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,68 @@
-
+import os
 import cv2
+import imageio
+
 from openCV_movement_detection.details_movement import change_frame, get_mask, contour_movement, text_movement, \
     make_video_no_roi, make_video_roi
 
 
 class VideoMovementClass:
 
-    def detect_movement(self, path, rois=None, no_rois=None, min_contour_area=10, circularity_threshold=0.5, blur=1, brightness=1):
-        cap = cv2.VideoCapture(path)
+    def detect_movement(self, source_path, rois=None, no_rois=None, min_contour_area=10, circularity_threshold=0.5,
+                        blur=1,
+                        brightness=1, difference_between_frames=20, destination_path = '/movement_analysis/'):
+        if blur % 2 == 0:
+            blur -= 1
+        filename = os.path.basename(source_path)
+        cap = cv2.VideoCapture(source_path)
         ret, prev_frame = cap.read()
         prev_frame_gray = change_frame(prev_frame, brightness)
         if no_rois:
             prev_frame_gray = make_video_no_roi(prev_frame_gray, no_rois)
         if rois:
             prev_frame_gray = make_video_roi(prev_frame_gray, rois)
         text_list = []
         count = 0
         prev_count = 1
         while True:
             ret, next_frame = cap.read()
             if not ret:
                 break
             count += 1
-            if (count % 20) == 0:
+            if (count % difference_between_frames) == 0:
                 next_frame_gray = change_frame(next_frame, brightness)
                 if no_rois:
                     next_frame_gray = make_video_no_roi(next_frame_gray, no_rois)
                 if rois:
                     next_frame_gray = make_video_roi(next_frame_gray, rois)
                 mask = get_mask(prev_frame_gray, next_frame_gray, blur)
                 contours, _ = cv2.findContours(mask, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
                 movement_detected = contour_movement(contours, circularity_threshold, min_contour_area)
                 text_list.append(text_movement(movement_detected, prev_count, count))
+                self.save_animated_frames(filename, prev_frame, next_frame, prev_count, count, destination_path)
+                prev_frame = next_frame
                 prev_frame_gray = next_frame_gray
                 prev_count = count
         cap.release()
         return text_list
 
+    def save_animated_frames(self, filename, prev_frame, next_frame, prev_count, count, destination_path):
+        filename = filename.replace('.mp4', '_')
+        output_file = filename + str(prev_count) + '_' + str(count) + '.webp'
+        output_dir = os.path.join(destination_path, filename)
+        image_path = os.path.join(output_dir, output_file)
+        # Check if the directory already exists
+        if not os.path.exists(image_path):
+            os.makedirs(output_dir, exist_ok=True)
+
+            # Ensure consistent color space (e.g., convert BGR to RGB)
+            prev_frame_rgb = cv2.cvtColor(prev_frame, cv2.COLOR_BGR2RGB)
+            next_frame_rgb = cv2.cvtColor(next_frame, cv2.COLOR_BGR2RGB)
+
+            frames = [prev_frame_rgb, next_frame_rgb]
+            frame_duration = 0.01
+
+            # Save frames as an animated WebP
+            imageio.mimsave(image_path, frames, duration=frame_duration)
+
```

