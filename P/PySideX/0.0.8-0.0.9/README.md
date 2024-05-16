# Comparing `tmp/PySideX-0.0.8.tar.gz` & `tmp/PySideX-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.8.tar", last modified: Thu Apr 18 16:39:21 2024, max compression
+gzip compressed data, was "PySideX-0.0.9.tar", last modified: Thu May 16 19:13:15 2024, max compression
```

## Comparing `PySideX-0.0.8.tar` & `PySideX-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.426477 PySideX-0.0.8/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-18 16:39:21.426477 PySideX-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.385335 PySideX-0.0.8/PySideX/
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.404177 PySideX-0.0.8/PySideX/Assets/
--rw-rw-rw-   0        0        0      308 2024-04-08 00:19:30.000000 PySideX-0.0.8/PySideX/Assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.412310 PySideX-0.0.8/PySideX/Components/
--rw-rw-rw-   0        0        0       28 2024-04-18 15:52:34.000000 PySideX-0.0.8/PySideX/Components/__init__.py
--rw-rw-rw-   0        0        0     1291 2024-04-18 16:38:14.000000 PySideX-0.0.8/PySideX/Components/box.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.425468 PySideX-0.0.8/PySideX/Widgets/
--rw-rw-rw-   0        0        0      384 2024-04-18 15:52:15.000000 PySideX-0.0.8/PySideX/Widgets/__init__.py
--rw-rw-rw-   0        0        0     1319 2024-04-08 15:21:11.000000 PySideX-0.0.8/PySideX/Widgets/button.py
--rw-rw-rw-   0        0        0     1162 2024-04-18 02:48:36.000000 PySideX-0.0.8/PySideX/Widgets/dropdawn.py
--rw-rw-rw-   0        0        0      871 2024-04-08 15:12:02.000000 PySideX-0.0.8/PySideX/Widgets/frame.py
--rw-rw-rw-   0        0        0      300 2024-04-08 15:08:05.000000 PySideX-0.0.8/PySideX/Widgets/horizontalBoxLayout.py
--rw-rw-rw-   0        0        0      728 2024-04-08 16:26:56.000000 PySideX-0.0.8/PySideX/Widgets/image.py
--rw-rw-rw-   0        0        0     1286 2024-04-18 02:50:33.000000 PySideX-0.0.8/PySideX/Widgets/input.py
--rw-rw-rw-   0        0        0     1561 2024-04-10 03:02:16.000000 PySideX-0.0.8/PySideX/Widgets/label.py
--rw-rw-rw-   0        0        0     2570 2024-04-10 05:32:57.000000 PySideX-0.0.8/PySideX/Widgets/messagebox.py
--rw-rw-rw-   0        0        0      602 2024-04-08 14:52:08.000000 PySideX-0.0.8/PySideX/Widgets/spacerItem.py
--rw-rw-rw-   0        0        0     1298 2024-04-18 15:53:07.000000 PySideX-0.0.8/PySideX/Widgets/textArea.py
--rw-rw-rw-   0        0        0      300 2024-04-08 15:08:01.000000 PySideX-0.0.8/PySideX/Widgets/verticalBoxLayout.py
--rw-rw-rw-   0        0        0      956 2024-04-06 15:53:16.000000 PySideX-0.0.8/PySideX/Widgets/window.py
--rw-rw-rw-   0        0        0      386 2024-04-18 15:52:46.000000 PySideX-0.0.8/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:21.402672 PySideX-0.0.8/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-18 16:39:21.000000 PySideX-0.0.8/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      656 2024-04-18 16:39:21.000000 PySideX-0.0.8/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 16:39:21.000000 PySideX-0.0.8/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 16:39:21.000000 PySideX-0.0.8/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 16:39:21.000000 PySideX-0.0.8/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2024-04-18 05:26:16.000000 PySideX-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 16:39:21.426477 PySideX-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      670 2024-04-18 16:36:25.000000 PySideX-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.246709 PySideX-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2632 2024-05-16 19:13:15.245201 PySideX-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.205115 PySideX-0.0.9/PySideX/
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.229123 PySideX-0.0.9/PySideX/Assets/
+-rw-rw-rw-   0        0        0   123351 2024-04-26 12:44:29.000000 PySideX-0.0.9/PySideX/Assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.231123 PySideX-0.0.9/PySideX/Components/
+-rw-rw-rw-   0        0        0       28 2024-04-26 14:13:32.000000 PySideX-0.0.9/PySideX/Components/__init__.py
+-rw-rw-rw-   0        0        0     1291 2024-04-18 16:38:14.000000 PySideX-0.0.9/PySideX/Components/box.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.244190 PySideX-0.0.9/PySideX/Widgets/
+-rw-rw-rw-   0        0        0      384 2024-04-26 14:13:33.000000 PySideX-0.0.9/PySideX/Widgets/__init__.py
+-rw-rw-rw-   0        0        0     1319 2024-04-08 15:21:11.000000 PySideX-0.0.9/PySideX/Widgets/button.py
+-rw-rw-rw-   0        0        0     1162 2024-04-18 02:48:36.000000 PySideX-0.0.9/PySideX/Widgets/dropdawn.py
+-rw-rw-rw-   0        0        0      871 2024-04-08 15:12:02.000000 PySideX-0.0.9/PySideX/Widgets/frame.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:05.000000 PySideX-0.0.9/PySideX/Widgets/horizontalBoxLayout.py
+-rw-rw-rw-   0        0        0     1102 2024-04-26 12:33:01.000000 PySideX-0.0.9/PySideX/Widgets/image.py
+-rw-rw-rw-   0        0        0     1286 2024-04-18 16:55:43.000000 PySideX-0.0.9/PySideX/Widgets/input.py
+-rw-rw-rw-   0        0        0     1561 2024-04-10 03:02:16.000000 PySideX-0.0.9/PySideX/Widgets/label.py
+-rw-rw-rw-   0        0        0     2570 2024-04-10 05:32:57.000000 PySideX-0.0.9/PySideX/Widgets/messagebox.py
+-rw-rw-rw-   0        0        0      602 2024-04-08 14:52:08.000000 PySideX-0.0.9/PySideX/Widgets/spacerItem.py
+-rw-rw-rw-   0        0        0     1298 2024-04-18 15:53:07.000000 PySideX-0.0.9/PySideX/Widgets/textArea.py
+-rw-rw-rw-   0        0        0      300 2024-04-08 15:08:01.000000 PySideX-0.0.9/PySideX/Widgets/verticalBoxLayout.py
+-rw-rw-rw-   0        0        0     1527 2024-04-26 15:08:22.000000 PySideX-0.0.9/PySideX/Widgets/window.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 14:13:34.000000 PySideX-0.0.9/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:13:15.228131 PySideX-0.0.9/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     2632 2024-05-16 19:13:14.000000 PySideX-0.0.9/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-05-16 19:13:14.000000 PySideX-0.0.9/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:13:14.000000 PySideX-0.0.9/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 19:13:14.000000 PySideX-0.0.9/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 19:13:14.000000 PySideX-0.0.9/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1001 2024-05-16 19:11:31.000000 PySideX-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 19:13:15.246709 PySideX-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-05-16 19:06:35.000000 PySideX-0.0.9/setup.py
```

### Comparing `PySideX-0.0.8/LICENSE` & `PySideX-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Components/box.py` & `PySideX-0.0.9/PySideX/Components/box.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/button.py` & `PySideX-0.0.9/PySideX/Widgets/button.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/dropdawn.py` & `PySideX-0.0.9/PySideX/Widgets/dropdawn.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/frame.py` & `PySideX-0.0.9/PySideX/Widgets/frame.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/image.py` & `PySideX-0.0.9/PySideX/Widgets/image.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from PySide6.QtWidgets import QLabel
 from PySide6.QtGui import QPixmap
 
 
 class Image(QLabel):
-    def __init__(self,img:str,id="image") -> None:
+    def __init__(self,img,id="image") -> None:
         super().__init__()
         self._img = img
         self._id = id
         self.__config__()
 
     def __config__(self):
         self.setObjectName(self._id)
         self.setText('')
-        pixmap = QPixmap(self._img)
-        self.setPixmap(pixmap)
-        self.setScaledContents(True)
+        self._setImageIcon()
+
+    def _setImageIcon(self):
+        if isinstance(self._img, str):
+            pixmap = QPixmap(self._img)
+            self.setPixmap(pixmap)
+            self.setScaledContents(True)
+        elif isinstance(self._img, bytes):
+            pixmap = QPixmap()
+            pixmap.loadFromData(self._img)
+            self.setPixmap(pixmap)
+            self.setScaledContents(True)
+        else:
+            raise ValueError("Unknown icon type")
 
     def click(self, target):
         """Every function expects to receive an event"""
         self.mousePressEvent = target
 
     def setStyleSheetFile(self, file):
         with open(file, "r") as f:
```

### Comparing `PySideX-0.0.8/PySideX/Widgets/input.py` & `PySideX-0.0.9/PySideX/Widgets/input.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/label.py` & `PySideX-0.0.9/PySideX/Widgets/label.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/messagebox.py` & `PySideX-0.0.9/PySideX/Widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/spacerItem.py` & `PySideX-0.0.9/PySideX/Widgets/spacerItem.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX/Widgets/textArea.py` & `PySideX-0.0.9/PySideX/Widgets/textArea.py`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/PySideX.egg-info/SOURCES.txt` & `PySideX-0.0.9/PySideX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.8/setup.py` & `PySideX-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = arq.read()
 
 with open("LICENSE", "r") as arq:
     licence = arq.read()
 
 setup(
     name="PySideX",
-    version="0.0.8",
+    version="0.0.9",
     license=licence,
     author="Ryan Souza Anselmo",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="ryansouza.cwb@email.com",
     keywords="pysidex",
     description="Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology",
```

