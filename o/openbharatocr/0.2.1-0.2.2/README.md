# Comparing `tmp/openbharatocr-0.2.1.tar.gz` & `tmp/openbharatocr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.2.1.tar", last modified: Tue Apr 30 09:06:41 2024, max compression
+gzip compressed data, was "openbharatocr-0.2.2.tar", last modified: Tue Apr 30 09:56:46 2024, max compression
```

## Comparing `openbharatocr-0.2.1.tar` & `openbharatocr-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.706052 openbharatocr-0.2.1/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/passport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/openbharatocr/ocr/voter_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:06:41.000000 openbharatocr-0.2.1/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 09:06:41.710052 openbharatocr-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 09:06:37.000000 openbharatocr-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:56:46.087514 openbharatocr-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:56:46.087514 openbharatocr-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:56:46.083514 openbharatocr-0.2.2/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:56:46.087514 openbharatocr-0.2.2/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/openbharatocr/ocr/voter_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 09:56:46.087514 openbharatocr-0.2.2/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-30 09:56:46.000000 openbharatocr-0.2.2/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 09:56:46.000000 openbharatocr-0.2.2/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:56:46.000000 openbharatocr-0.2.2/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 09:56:45.000000 openbharatocr-0.2.2/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 09:56:46.000000 openbharatocr-0.2.2/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 09:56:46.000000 openbharatocr-0.2.2/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 09:56:46.087514 openbharatocr-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 09:56:41.000000 openbharatocr-0.2.2/setup.py
```

### Comparing `openbharatocr-0.2.1/LICENSE` & `openbharatocr-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/PKG-INFO` & `openbharatocr-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.2.1
+Version: 0.2.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openbharatocr-0.2.1/README.md` & `openbharatocr-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.2.2/openbharatocr/ocr/aadhaar.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.2.2/openbharatocr/ocr/driving_licence.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,26 +137,25 @@
         if found:
             break
 
     return address
 
 
 def extract_address(image_path):
-
     image = Image.open(image_path)
     text = pytesseract.image_to_string(image)
 
     if "Add" not in text and "ADD" not in text:
         return ""
     rgb = image.convert("RGB")
     with tempfile.TemporaryDirectory() as tempdir:
         tempfile_path = f"{tempdir}/{str(uuid.uuid4())}.jpg"
         rgb.save(tempfile_path)
 
-        image = cv2.imread(image_path)
+        image = cv2.imread(tempfile_path)
 
         gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
         config = r"--oem 3 --psm 6"
         boxes_data = pytesseract.image_to_data(gray_image, config=config)
 
         boxes = boxes_data.splitlines()
```

### Comparing `openbharatocr-0.2.1/openbharatocr/ocr/pan.py` & `openbharatocr-0.2.2/openbharatocr/ocr/pan.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/openbharatocr/ocr/passport.py` & `openbharatocr-0.2.2/openbharatocr/ocr/passport.py`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/openbharatocr/ocr/voter_id.py` & `openbharatocr-0.2.2/openbharatocr/ocr/voter_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 import cv2
 import pytesseract
 from PIL import Image
 import numpy as np
 import os
+import tempfile
+import uuid
 
 # Download the models from links and set in the environment
 YOLO_CFG = os.environ.get(
     "YOLO_CFG", "yolov3_custom.cfg"
 )  # https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
 YOLO_WEIGHT = os.environ.get(
     "YOLO_WEIGHT", "yolov3_custom_6000.weights"
@@ -27,74 +29,79 @@
         binary, -1, np.array([[0, -1, 0], [-1, 5, -1], [0, -1, 0]])
     )
 
     return sharpened
 
 
 def extract_voter_details_yolo(image_path):
-
+    image = Image.open(image_path)
     net = cv2.dnn.readNetFromDarknet(YOLO_CFG, YOLO_WEIGHT)
     classes = ["elector", "relation", "voterid"]
 
-    img = cv2.imread(image_path)
-    if img is None:
-        print("Error: Unable to read the input image.")
-        exit()
-
-    height, width, _ = img.shape
-    blob = cv2.dnn.blobFromImage(
-        img, 1 / 255, (416, 416), (0, 0, 0), swapRB=True, crop=False
-    )
+    rgb = image.convert("RGB")
+    with tempfile.TemporaryDirectory() as tempdir:
+        tempfile_path = f"{tempdir}/{str(uuid.uuid4())}.jpg"
+        rgb.save(tempfile_path)
+
+        img = cv2.imread(tempfile_path)
+        if img is None:
+            print("Error: Unable to read the input image.")
+            exit()
+
+        height, width, _ = img.shape
+        blob = cv2.dnn.blobFromImage(
+            img, 1 / 255, (416, 416), (0, 0, 0), swapRB=True, crop=False
+        )
+
+        net.setInput(blob)
+        output_layers_name = net.getUnconnectedOutLayersNames()
+        layerOutputs = net.forward(output_layers_name)
+
+        boxes = []
+        confidences = []
+        class_ids = []
+        detected_texts = {}
+
+        for output in layerOutputs:
+            for detection in output:
+                scores = detection[5:]
+                class_id = np.argmax(scores)
+                confidence = scores[class_id]
+                if confidence > 0.5:
+                    center_x = int(detection[0] * width)
+                    center_y = int(detection[1] * height)
+                    w = int(detection[2] * width)
+                    h = int(detection[3] * height)
+
+                    x = int(center_x - w / 2)
+                    y = int(center_y - h / 2)
+
+                    boxes.append([x, y, w, h])
+                    confidences.append(float(confidence))
+                    class_ids.append(class_id)
+
+        indexes = cv2.dnn.NMSBoxes(boxes, confidences, 0.5, 0.4)
+
+        for i in range(len(boxes)):
+            if i in indexes:
+                x, y, w, h = boxes[i]
+
+                x = max(0, x)
+                y = max(0, y)
+                w = min(width - x, w)
+                h = min(height - y, h)
+
+                label = str(classes[class_ids[i]])
+                crop_img = img[y : y + h, x : x + w]
+                if crop_img.size == 0:
+                    continue
+                text = pytesseract.image_to_string(crop_img, config="--psm 6")
+                detected_texts[label] = text.strip()
 
-    net.setInput(blob)
-    output_layers_name = net.getUnconnectedOutLayersNames()
-    layerOutputs = net.forward(output_layers_name)
-
-    boxes = []
-    confidences = []
-    class_ids = []
-    detected_texts = {}
-
-    for output in layerOutputs:
-        for detection in output:
-            scores = detection[5:]
-            class_id = np.argmax(scores)
-            confidence = scores[class_id]
-            if confidence > 0.5:
-                center_x = int(detection[0] * width)
-                center_y = int(detection[1] * height)
-                w = int(detection[2] * width)
-                h = int(detection[3] * height)
-
-                x = int(center_x - w / 2)
-                y = int(center_y - h / 2)
-
-                boxes.append([x, y, w, h])
-                confidences.append(float(confidence))
-                class_ids.append(class_id)
-
-    indexes = cv2.dnn.NMSBoxes(boxes, confidences, 0.5, 0.4)
-
-    for i in range(len(boxes)):
-        if i in indexes:
-            x, y, w, h = boxes[i]
-
-            x = max(0, x)
-            y = max(0, y)
-            w = min(width - x, w)
-            h = min(height - y, h)
-
-            label = str(classes[class_ids[i]])
-            crop_img = img[y : y + h, x : x + w]
-            if crop_img.size == 0:
-                continue
-            text = pytesseract.image_to_string(crop_img, config="--psm 6")
-            detected_texts[label] = text.strip()
-
-    return detected_texts
+        return detected_texts
 
 
 def extract_voter_id(input):
 
     regex = r".{0,3}[0-9]{7}"
     match = re.search(regex, input)
     voter_id = match.group(0) if match else ""
@@ -165,43 +172,47 @@
     names = extract_names(extracted_text)
     electors_name = names[0] if len(names) > 0 else ""
     fathers_name = names[1] if len(names) > 1 else ""
 
     gender = extract_gender(extracted_text)
 
     dob = extract_date(extracted_text)
-
-    image = cv2.imread(image_path)
-    preprocessed = preprocess_for_bold_text(image)
-    cv2.imwrite("preprocessed_image.jpg", preprocessed)
-
-    image = Image.open("preprocessed_image.jpg")
-    clean_text = pytesseract.image_to_string(image)
-
-    if electors_name == "":
-        names = extract_lines_with_uppercase_words(clean_text)
-        electors_name = names[-2] if len(names) > 1 else ""
-        fathers_name = names[-1] if len(names) > 0 else ""
-
-    if dob == "":
-        dob = extract_date(clean_text)
-
-    if voter_id == "":
-        voter_id = extract_voter_id(clean_text)
-
-    if gender == "":
-        gender = extract_gender(clean_text)
-
-    return {
-        "Voter ID": voter_id,
-        "Elector's Name": electors_name,
-        "Father's Name": fathers_name,
-        "Gender": gender,
-        "Date of Birth": dob,
-    }
+    rgb = image.convert("RGB")
+    with tempfile.TemporaryDirectory() as tempdir:
+        tempfile_path = f"{tempdir}/{str(uuid.uuid4())}.jpg"
+        rgb.save(tempfile_path)
+
+        image = cv2.imread(tempfile_path)
+        preprocessed = preprocess_for_bold_text(image)
+        cv2.imwrite("preprocessed_image.jpg", preprocessed)
+
+        image = Image.open("preprocessed_image.jpg")
+        clean_text = pytesseract.image_to_string(image)
+
+        if electors_name == "":
+            names = extract_lines_with_uppercase_words(clean_text)
+            electors_name = names[-2] if len(names) > 1 else ""
+            fathers_name = names[-1] if len(names) > 0 else ""
+
+        if dob == "":
+            dob = extract_date(clean_text)
+
+        if voter_id == "":
+            voter_id = extract_voter_id(clean_text)
+
+        if gender == "":
+            gender = extract_gender(clean_text)
+
+        return {
+            "Voter ID": voter_id,
+            "Elector's Name": electors_name,
+            "Father's Name": fathers_name,
+            "Gender": gender,
+            "Date of Birth": dob,
+        }
 
 
 def extract_voterid_details_back(image_path):
 
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
```

### Comparing `openbharatocr-0.2.1/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.2.2/openbharatocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.2.1
+Version: 0.2.2
 Summary: openbharatocr is an opensource python library for ocr Indian government documents 
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openbharatocr-0.2.1/openbharatocr.egg-info/SOURCES.txt` & `openbharatocr-0.2.2/openbharatocr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.2.1/setup.py` & `openbharatocr-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.2.1",
+    version="0.2.2",
     description="openbharatocr is an opensource python library for ocr Indian government documents ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
```

