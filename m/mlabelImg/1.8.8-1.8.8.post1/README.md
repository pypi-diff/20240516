# Comparing `tmp/mlabelimg-1.8.8.tar.gz` & `tmp/mlabelimg-1.8.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlabelimg-1.8.8.tar", last modified: Mon May 13 08:39:49 2024, max compression
+gzip compressed data, was "mlabelimg-1.8.8.post1.tar", last modified: Thu May 16 03:30:18 2024, max compression
```

## Comparing `mlabelimg-1.8.8.tar` & `mlabelimg-1.8.8.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.693939 mlabelimg-1.8.8/
--rw-rw-rw-   0        0        0       83 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1659 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1197 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/LICENSE
--rw-rw-rw-   0        0        0      300 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3233 2024-05-13 08:39:49.693939 mlabelimg-1.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     2133 2024-05-10 04:26:51.000000 mlabelimg-1.8.8/README.md
--rw-rw-rw-   0        0        0        0 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.651054 mlabelimg-1.8.8/data/
--rw-rw-rw-   0        0        0      145 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/data/predefined_classes.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.672995 mlabelimg-1.8.8/libs/
--rw-rw-rw-   0        0        0       76 2024-05-13 08:37:20.000000 mlabelimg-1.8.8/libs/__init__.py
--rw-rw-rw-   0        0        0    27971 2024-05-10 04:09:45.000000 mlabelimg-1.8.8/libs/canvas.py
--rw-rw-rw-   0        0        0     1295 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/colorDialog.py
--rw-rw-rw-   0        0        0     1151 2024-05-13 08:35:32.000000 mlabelimg-1.8.8/libs/combobox.py
--rw-rw-rw-   0        0        0      668 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/constants.py
--rw-rw-rw-   0        0        0     3852 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/create_ml_io.py
--rw-rw-rw-   0        0        0      784 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/hashableQListWidgetItem.py
--rw-rw-rw-   0        0        0     3153 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/labelDialog.py
--rw-rw-rw-   0        0        0     6341 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/labelFile.py
--rw-rw-rw-   0        0        0     6324 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/pascal_voc_io.py
--rw-rw-rw-   0        0        0   641015 2024-05-13 07:19:21.000000 mlabelimg-1.8.8/libs/resources.py
--rw-rw-rw-   0        0        0     1238 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/settings.py
--rw-rw-rw-   0        0        0     6604 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/shape.py
--rw-rw-rw-   0        0        0     2506 2024-05-13 04:49:14.000000 mlabelimg-1.8.8/libs/stringBundle.py
--rw-rw-rw-   0        0        0     1192 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/toolBar.py
--rw-rw-rw-   0        0        0      534 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/ustr.py
--rw-rw-rw-   0        0        0     2897 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/utils.py
--rw-rw-rw-   0        0        0     4998 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/yolo_io.py
--rw-rw-rw-   0        0        0      780 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/libs/zoomWidget.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:39:49.692942 mlabelimg-1.8.8/mlabelImg.egg-info/
--rw-rw-rw-   0        0        0     3233 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 04:17:09.000000 mlabelimg-1.8.8/mlabelImg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 08:39:49.000000 mlabelimg-1.8.8/mlabelImg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    68154 2024-05-13 08:36:14.000000 mlabelimg-1.8.8/mlabelImg.py
--rw-rw-rw-   0        0        0     2078 2021-10-11 20:15:19.000000 mlabelimg-1.8.8/resources.qrc
--rw-rw-rw-   0        0        0      149 2024-05-13 08:39:49.695934 mlabelimg-1.8.8/setup.cfg
--rw-rw-rw-   0        0        0     3668 2024-05-10 04:35:47.000000 mlabelimg-1.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:30:18.260899 mlabelimg-1.8.8.post1/
+-rw-rw-rw-   0        0        0       83 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1659 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1197 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/LICENSE
+-rw-rw-rw-   0        0        0      300 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3239 2024-05-16 03:30:18.260899 mlabelimg-1.8.8.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2133 2024-05-10 04:26:51.000000 mlabelimg-1.8.8.post1/README.md
+-rw-rw-rw-   0        0        0        0 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:30:18.217011 mlabelimg-1.8.8.post1/data/
+-rw-rw-rw-   0        0        0      145 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/data/predefined_classes.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 03:30:18.239955 mlabelimg-1.8.8.post1/libs/
+-rw-rw-rw-   0        0        0       85 2024-05-16 03:27:39.000000 mlabelimg-1.8.8.post1/libs/__init__.py
+-rw-rw-rw-   0        0        0    27971 2024-05-10 04:09:45.000000 mlabelimg-1.8.8.post1/libs/canvas.py
+-rw-rw-rw-   0        0        0     1295 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/colorDialog.py
+-rw-rw-rw-   0        0        0     1151 2024-05-16 03:26:20.000000 mlabelimg-1.8.8.post1/libs/combobox.py
+-rw-rw-rw-   0        0        0      668 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/constants.py
+-rw-rw-rw-   0        0        0     3852 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/create_ml_io.py
+-rw-rw-rw-   0        0        0      784 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/hashableQListWidgetItem.py
+-rw-rw-rw-   0        0        0     3153 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/labelDialog.py
+-rw-rw-rw-   0        0        0     6341 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/labelFile.py
+-rw-rw-rw-   0        0        0     6324 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/pascal_voc_io.py
+-rw-rw-rw-   0        0        0   641015 2024-05-13 07:19:21.000000 mlabelimg-1.8.8.post1/libs/resources.py
+-rw-rw-rw-   0        0        0     1238 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/settings.py
+-rw-rw-rw-   0        0        0     6604 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/shape.py
+-rw-rw-rw-   0        0        0     2506 2024-05-13 04:49:14.000000 mlabelimg-1.8.8.post1/libs/stringBundle.py
+-rw-rw-rw-   0        0        0     1192 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/toolBar.py
+-rw-rw-rw-   0        0        0      534 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/ustr.py
+-rw-rw-rw-   0        0        0     2897 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/utils.py
+-rw-rw-rw-   0        0        0     4998 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/yolo_io.py
+-rw-rw-rw-   0        0        0      780 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/libs/zoomWidget.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:30:18.260899 mlabelimg-1.8.8.post1/mlabelImg.egg-info/
+-rw-rw-rw-   0        0        0     3239 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      753 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 04:17:09.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-16 03:30:18.000000 mlabelimg-1.8.8.post1/mlabelImg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    68224 2024-05-14 08:36:43.000000 mlabelimg-1.8.8.post1/mlabelImg.py
+-rw-rw-rw-   0        0        0     2078 2021-10-11 20:15:19.000000 mlabelimg-1.8.8.post1/resources.qrc
+-rw-rw-rw-   0        0        0      149 2024-05-16 03:30:18.263406 mlabelimg-1.8.8.post1/setup.cfg
+-rw-rw-rw-   0        0        0     3668 2024-05-10 04:35:47.000000 mlabelimg-1.8.8.post1/setup.py
```

### Comparing `mlabelimg-1.8.8/HISTORY.rst` & `mlabelimg-1.8.8.post1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/LICENSE` & `mlabelimg-1.8.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/PKG-INFO` & `mlabelimg-1.8.8.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlabelImg
-Version: 1.8.8
+Version: 1.8.8.post1
 Summary: LabelImg is a graphical image annotation tool and label object bounding boxes in images (Modified Version)
 Home-page: https://github.com/PD-Mera/mlabelImg
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 License: MIT license
 Keywords: labelImg labelTool development annotation deeplearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlabelimg-1.8.8/README.md` & `mlabelimg-1.8.8.post1/README.md`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/canvas.py` & `mlabelimg-1.8.8.post1/libs/canvas.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/colorDialog.py` & `mlabelimg-1.8.8.post1/libs/colorDialog.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/combobox.py` & `mlabelimg-1.8.8.post1/libs/combobox.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/constants.py` & `mlabelimg-1.8.8.post1/libs/constants.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/create_ml_io.py` & `mlabelimg-1.8.8.post1/libs/create_ml_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/hashableQListWidgetItem.py` & `mlabelimg-1.8.8.post1/libs/hashableQListWidgetItem.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/labelDialog.py` & `mlabelimg-1.8.8.post1/libs/labelDialog.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/labelFile.py` & `mlabelimg-1.8.8.post1/libs/labelFile.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/pascal_voc_io.py` & `mlabelimg-1.8.8.post1/libs/pascal_voc_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/resources.py` & `mlabelimg-1.8.8.post1/libs/resources.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/settings.py` & `mlabelimg-1.8.8.post1/libs/settings.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/shape.py` & `mlabelimg-1.8.8.post1/libs/shape.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/stringBundle.py` & `mlabelimg-1.8.8.post1/libs/stringBundle.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/toolBar.py` & `mlabelimg-1.8.8.post1/libs/toolBar.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/ustr.py` & `mlabelimg-1.8.8.post1/libs/ustr.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/utils.py` & `mlabelimg-1.8.8.post1/libs/utils.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/yolo_io.py` & `mlabelimg-1.8.8.post1/libs/yolo_io.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/libs/zoomWidget.py` & `mlabelimg-1.8.8.post1/libs/zoomWidget.py`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/mlabelImg.egg-info/PKG-INFO` & `mlabelimg-1.8.8.post1/mlabelImg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlabelImg
-Version: 1.8.8
+Version: 1.8.8.post1
 Summary: LabelImg is a graphical image annotation tool and label object bounding boxes in images (Modified Version)
 Home-page: https://github.com/PD-Mera/mlabelImg
 Author: PD-Mera
 Author-email: phuongdong1772000@gmail.com
 License: MIT license
 Keywords: labelImg labelTool development annotation deeplearning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mlabelimg-1.8.8/mlabelImg.egg-info/SOURCES.txt` & `mlabelimg-1.8.8.post1/mlabelImg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/mlabelImg.py` & `mlabelimg-1.8.8.post1/mlabelImg.py`

 * *Files 0% similar despite different names*

```diff
@@ -890,16 +890,18 @@
     def copy_selected_shape(self):
         self.add_label(self.canvas.copy_selected_shape())
         # fix copy and delete
         self.shape_selection_changed(True)
 
     def combo_selection_changed(self, index):
         text = self.combo_box.cb.itemText(index)
+        text = "" if text == "[SHOW ALL]" else text
+            
         for i in range(self.label_list.count()):
-            if text == "[SHOW ALL]":
+            if text == "": #"[SHOW ALL]":
                 self.label_list.item(i).setCheckState(2)
             elif text == "[HIDE ALL]":
                 self.label_list.item(i).setCheckState(0)
             elif text != self.label_list.item(i).text():
                 self.label_list.item(i).setCheckState(0)
             else:
                 self.label_list.item(i).setCheckState(2)
```

### Comparing `mlabelimg-1.8.8/resources.qrc` & `mlabelimg-1.8.8.post1/resources.qrc`

 * *Files identical despite different names*

### Comparing `mlabelimg-1.8.8/setup.py` & `mlabelimg-1.8.8.post1/setup.py`

 * *Files identical despite different names*

