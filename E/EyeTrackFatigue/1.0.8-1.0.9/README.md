# Comparing `tmp/EyeTrackFatigue-1.0.8.tar.gz` & `tmp/EyeTrackFatigue-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EyeTrackFatigue-1.0.8.tar", last modified: Tue Mar 26 13:08:01 2024, max compression
+gzip compressed data, was "EyeTrackFatigue-1.0.9.tar", last modified: Tue Mar 26 13:57:29 2024, max compression
```

## Comparing `EyeTrackFatigue-1.0.8.tar` & `EyeTrackFatigue-1.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.959775 EyeTrackFatigue-1.0.8/
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.913925 EyeTrackFatigue-1.0.8/EyeTrackFatigue/
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.936338 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/
--rw-rw-rw-   0        0        0      455 2024-02-27 21:04:37.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/GeoMetrics.py
--rw-rw-rw-   0        0        0     6890 2024-02-27 21:03:35.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/Movements.py
--rw-rw-rw-   0        0        0    11675 2024-02-27 20:50:23.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/Names.py
--rw-rw-rw-   0        0        0    49160 2024-02-27 21:37:14.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/ParsedData.py
--rw-rw-rw-   0        0        0     1394 2024-02-27 21:06:11.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/SecondaryMetrics.py
--rw-rw-rw-   0        0        0     1206 2024-02-27 21:06:58.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.940272 EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/
--rw-rw-rw-   0        0        0     2357 2024-02-22 12:28:39.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/DeviceHandler.py
--rw-rw-rw-   0        0        0     2732 2024-02-21 21:57:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/Synchronizer.py
--rw-rw-rw-   0        0        0      264 2024-02-27 20:43:32.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.947106 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/
--rw-rw-rw-   0        0        0     1873 2024-02-27 21:42:52.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/BasicEval.py
--rw-rw-rw-   0        0        0     6738 2024-02-27 21:57:08.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/DecisionTreeEval.py
--rw-rw-rw-   0        0        0      307 2024-02-27 21:49:04.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/Evaluator.py
--rw-rw-rw-   0        0        0     4850 2024-02-27 21:53:32.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/HybridEval.py
--rw-rw-rw-   0        0        0     8085 2024-02-27 22:02:07.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/MLPEval.py
--rw-rw-rw-   0        0        0     7140 2024-02-27 21:58:36.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/RandomForestEval.py
--rw-rw-rw-   0        0        0      791 2024-02-17 17:45:27.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.950988 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/
--rw-rw-rw-   0        0        0     7062 2024-02-22 13:18:24.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/InputSection.py
--rw-rw-rw-   0        0        0     1343 2024-02-22 13:16:56.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/SingleData.py
--rw-rw-rw-   0        0        0      758 2024-02-25 22:31:56.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.955867 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/
--rw-rw-rw-   0        0        0     1654 2023-07-19 18:29:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/EventTests.py
--rw-rw-rw-   0        0        0     1495 2024-01-19 16:37:12.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/Time_Test.py
--rw-rw-rw-   0        0        0     2609 2023-07-16 14:09:08.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/UnitTests.py
--rw-rw-rw-   0        0        0    16877 2024-02-27 12:30:55.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/videoProcessorAlpha.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.957822 EyeTrackFatigue-1.0.8/EyeTrackFatigue/UI/
--rw-rw-rw-   0        0        0    10092 2024-03-26 12:05:03.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/UI/DataGather.py
--rw-rw-rw-   0        0        0    30420 2024-02-28 21:18:20.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue/UI/EvalApp.py
-drwxrwxrwx   0        0        0        0 2024-03-26 13:08:01.958797 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/
--rw-rw-rw-   0        0        0     1055 2024-03-26 13:08:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2024-03-26 13:08:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 13:08:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-26 13:08:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-26 13:08:01.000000 EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-03-26 13:08:01.959775 EyeTrackFatigue-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    20222 2024-02-25 20:37:28.000000 EyeTrackFatigue-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 13:08:01.962707 EyeTrackFatigue-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1481 2024-03-26 13:07:52.000000 EyeTrackFatigue-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.208727 EyeTrackFatigue-1.0.9/
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.126730 EyeTrackFatigue-1.0.9/EyeTrackFatigue/
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.174555 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/
+-rw-rw-rw-   0        0        0      455 2024-02-27 21:04:37.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/GeoMetrics.py
+-rw-rw-rw-   0        0        0     6890 2024-02-27 21:03:35.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/Movements.py
+-rw-rw-rw-   0        0        0    11675 2024-02-27 20:50:23.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/Names.py
+-rw-rw-rw-   0        0        0    49160 2024-02-27 21:37:14.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/ParsedData.py
+-rw-rw-rw-   0        0        0     1394 2024-02-27 21:06:11.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/SecondaryMetrics.py
+-rw-rw-rw-   0        0        0     1206 2024-02-27 21:06:58.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.180415 EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/
+-rw-rw-rw-   0        0        0     2357 2024-02-22 12:28:39.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/DeviceHandler.py
+-rw-rw-rw-   0        0        0     2732 2024-02-21 21:57:01.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/Synchronizer.py
+-rw-rw-rw-   0        0        0      264 2024-02-27 20:43:32.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.190204 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/
+-rw-rw-rw-   0        0        0     1873 2024-02-27 21:42:52.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/BasicEval.py
+-rw-rw-rw-   0        0        0     6738 2024-02-27 21:57:08.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/DecisionTreeEval.py
+-rw-rw-rw-   0        0        0      307 2024-02-27 21:49:04.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/Evaluator.py
+-rw-rw-rw-   0        0        0     4850 2024-02-27 21:53:32.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/HybridEval.py
+-rw-rw-rw-   0        0        0     8085 2024-02-27 22:02:07.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/MLPEval.py
+-rw-rw-rw-   0        0        0     7140 2024-02-27 21:58:36.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/RandomForestEval.py
+-rw-rw-rw-   0        0        0      791 2024-02-17 17:45:27.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.194110 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/
+-rw-rw-rw-   0        0        0     7062 2024-02-22 13:18:24.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/InputSection.py
+-rw-rw-rw-   0        0        0     1343 2024-02-22 13:16:56.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/SingleData.py
+-rw-rw-rw-   0        0        0      758 2024-02-25 22:31:56.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.202868 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/
+-rw-rw-rw-   0        0        0     1654 2023-07-19 18:29:01.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/EventTests.py
+-rw-rw-rw-   0        0        0     1495 2024-01-19 16:37:12.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/Time_Test.py
+-rw-rw-rw-   0        0        0     2609 2023-07-16 14:09:08.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/UnitTests.py
+-rw-rw-rw-   0        0        0    16700 2024-03-26 13:16:05.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/videoProcessorAlpha.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.206774 EyeTrackFatigue-1.0.9/EyeTrackFatigue/UI/
+-rw-rw-rw-   0        0        0    10092 2024-03-26 12:05:03.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/UI/DataGather.py
+-rw-rw-rw-   0        0        0    30420 2024-02-28 21:18:20.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue/UI/EvalApp.py
+drwxrwxrwx   0        0        0        0 2024-03-26 13:57:29.207750 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/
+-rw-rw-rw-   0        0        0     1078 2024-03-26 13:57:28.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2024-03-26 13:57:29.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-26 13:57:28.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-03-26 13:57:28.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-03-26 13:57:28.000000 EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1078 2024-03-26 13:57:29.208727 EyeTrackFatigue-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    20222 2024-02-25 20:37:28.000000 EyeTrackFatigue-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-26 13:57:29.216543 EyeTrackFatigue-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2024-03-26 13:57:23.000000 EyeTrackFatigue-1.0.9/setup.py
```

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/Movements.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/Movements.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/Names.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/Names.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/ParsedData.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/ParsedData.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/SecondaryMetrics.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/SecondaryMetrics.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Analise/__init__.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Analise/__init__.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/DeviceHandler.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/DeviceHandler.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/DeviceManager/Synchronizer.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/DeviceManager/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/BasicEval.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/BasicEval.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/DecisionTreeEval.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/DecisionTreeEval.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/HybridEval.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/HybridEval.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/MLPEval.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/MLPEval.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/RandomForestEval.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/RandomForestEval.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Evaluate/__init__.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/InputSection.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/InputSection.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/SingleData.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/SingleData.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Input/__init__.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Input/__init__.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/EventTests.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/EventTests.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/Time_Test.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/Time_Test.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/UnitTests.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/UnitTests.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/Meta/videoProcessorAlpha.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/Meta/videoProcessorAlpha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import numpy as np
-import cv2 # для видеообработки требуется также библиоетка cv2, не включённая в основной список зависимостей
+import cv2 
 from math import pi
 import datetime
 import os.path
 import statistics as st
 from scipy import ndimage as ndi
 
 
@@ -341,15 +341,15 @@
         fileTxt.close()
 
 if __name__ == '__main__':
     # Пример использования
     inputVideoPath = "video_test.avi"
     outputPath = inputVideoPath + '+alpha.csv'
 
-    v = VideoProcessor(doLogging=True)
+    v = SceneProcessor(doLogging=True)
     v.EyetrackerHorizontalFOV = 82  # угол обзора камеры сцены айтрекера. Обычно есть в паспорте модели.
     v.LoadVideo(inputVideoPath)
     v.DoProcessing(5)  # рекомендуемое значение 1
     v.DoPostprocessing(5)  # рекомендуемое значение 1. Выше - для сильно зашумлённых данных.
     v.SaveToCSV(outputPath)
 
     print("Done!")
```

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/UI/DataGather.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/UI/DataGather.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue/UI/EvalApp.py` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue/UI/EvalApp.py`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/PKG-INFO` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EyeTrackFatigue
-Version: 1.0.8
+Version: 1.0.9
 Summary: проект FAEyeTON - Библиотека открытого кода для оценки функционального состояния утомления оператора на основе динамической активности взгляда и головы. Проект Код-ИИ-2022.
 Home-page: https://github.com/AI-group-72/FAEyeTON
 Author: Кашевник А.М. Кузнецов В.В. Брак И.В. Мамонов А.А. Коваленко С.Д.
 Author-email: anton.mamonov.golohvastogo@mail.ru
 License: GNU LGPL
 Project-URL: GitHub Project, https://github.com/AI-group-72/FAEyeTON
 Project-URL: Issue Tracker, https://github.com/AI-group-72/FAEyeTON/Meta/issues
@@ -12,9 +12,10 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: PyQt6
 Requires-Dist: opencv-python
+Requires-Dist: joblib
 
 https://github.com/AI-group-72/FAEyeTON/blob/main/README.md
```

### Comparing `EyeTrackFatigue-1.0.8/EyeTrackFatigue.egg-info/SOURCES.txt` & `EyeTrackFatigue-1.0.9/EyeTrackFatigue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/PKG-INFO` & `EyeTrackFatigue-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EyeTrackFatigue
-Version: 1.0.8
+Version: 1.0.9
 Summary: проект FAEyeTON - Библиотека открытого кода для оценки функционального состояния утомления оператора на основе динамической активности взгляда и головы. Проект Код-ИИ-2022.
 Home-page: https://github.com/AI-group-72/FAEyeTON
 Author: Кашевник А.М. Кузнецов В.В. Брак И.В. Мамонов А.А. Коваленко С.Д.
 Author-email: anton.mamonov.golohvastogo@mail.ru
 License: GNU LGPL
 Project-URL: GitHub Project, https://github.com/AI-group-72/FAEyeTON
 Project-URL: Issue Tracker, https://github.com/AI-group-72/FAEyeTON/Meta/issues
@@ -12,9 +12,10 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: PyQt6
 Requires-Dist: opencv-python
+Requires-Dist: joblib
 
 https://github.com/AI-group-72/FAEyeTON/blob/main/README.md
```

### Comparing `EyeTrackFatigue-1.0.8/README.md` & `EyeTrackFatigue-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `EyeTrackFatigue-1.0.8/setup.py` & `EyeTrackFatigue-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 
 def get_long_description():
     return 'https://github.com/AI-group-72/FAEyeTON/blob/main/README.md'
 
 def get_requirements():
-    return ['pandas', 'openpyxl', 'scikit-learn', 'numpy', 'PyQt6', 'opencv-python',]
+    return ['pandas', 'openpyxl', 'scikit-learn', 'numpy', 'PyQt6', 'opencv-python', 'joblib']
 
 setup(
     name="EyeTrackFatigue",
-    version="1.0.8",
+    version="1.0.9",
     description="проект FAEyeTON - Библиотека открытого кода для оценки функционального состояния утомления оператора на основе динамической активности взгляда и головы. Проект Код-ИИ-2022.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Кашевник А.М. Кузнецов В.В. Брак И.В. Мамонов А.А. Коваленко С.Д.",
     author_email="anton.mamonov.golohvastogo@mail.ru",
     url="https://github.com/AI-group-72/FAEyeTON",
     project_urls={
```

