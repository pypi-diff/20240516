# Comparing `tmp/albucore-0.0.1.tar.gz` & `tmp/albucore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albucore-0.0.1.tar", last modified: Wed May 15 02:11:09 2024, max compression
+gzip compressed data, was "albucore-0.0.2.tar", last modified: Wed May 15 20:26:44 2024, max compression
```

## Comparing `albucore-0.0.1.tar` & `albucore-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-15 02:11:09.357896 albucore-0.0.1/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1075 2024-05-14 02:01:45.000000 albucore-0.0.1/LICENSE
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3934 2024-05-15 02:11:09.357689 albucore-0.0.1/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2227 2024-05-15 02:09:12.000000 albucore-0.0.1/README.md
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-15 02:11:09.356277 albucore-0.0.1/albucore/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       48 2024-05-15 02:10:15.000000 albucore-0.0.1/albucore/__init__.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1726 2024-05-14 02:01:45.000000 albucore-0.0.1/albucore/functions.py
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3690 2024-05-14 02:01:45.000000 albucore-0.0.1/albucore/utils.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-15 02:11:09.357467 albucore-0.0.1/albucore.egg-info/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3934 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/PKG-INFO
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)      316 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/SOURCES.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/dependency_links.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        1 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/not-zip-safe
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       57 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/requires.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)        9 2024-05-15 02:11:09.000000 albucore-0.0.1/albucore.egg-info/top_level.txt
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     2598 2024-05-14 02:01:45.000000 albucore-0.0.1/pyproject.toml
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)       38 2024-05-15 02:11:09.357951 albucore-0.0.1/setup.cfg
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     3574 2024-05-15 02:09:12.000000 albucore-0.0.1/setup.py
-drwxr-xr-x   0 vladimiriglovikov   (501) staff       (20)        0 2024-05-15 02:11:09.357117 albucore-0.0.1/tests/
--rw-r--r--   0 vladimiriglovikov   (501) staff       (20)     1515 2024-05-14 02:01:45.000000 albucore-0.0.1/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:44.377675 albucore-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-15 20:26:27.000000 albucore-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-15 20:26:44.377675 albucore-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-15 20:26:27.000000 albucore-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:44.377675 albucore-0.0.2/albucore/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-15 20:26:27.000000 albucore-0.0.2/albucore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-15 20:26:27.000000 albucore-0.0.2/albucore/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-15 20:26:27.000000 albucore-0.0.2/albucore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:44.377675 albucore-0.0.2/albucore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 20:26:44.000000 albucore-0.0.2/albucore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-15 20:26:27.000000 albucore-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:26:44.377675 albucore-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-15 20:26:27.000000 albucore-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:26:44.377675 albucore-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-15 20:26:27.000000 albucore-0.0.2/tests/test_functions.py
```

### Comparing `albucore-0.0.1/LICENSE` & `albucore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `albucore-0.0.1/PKG-INFO` & `albucore-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.1
+Version: 0.0.2
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: opencv-python-headless>=4.9.0
+Requires-Dist: opencv-python-headless>=4.5.5.64
 
 # Albucore
 
 Albucore is a high-performance image processing library designed to optimize operations on images using Python and OpenCV, building upon the foundations laid by the popular Albumentations library. It offers specialized optimizations for different image data types and aims to provide faster processing times through efficient algorithm implementations.
 
 ## Features
```

### Comparing `albucore-0.0.1/README.md` & `albucore-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `albucore-0.0.1/albucore/functions.py` & `albucore-0.0.2/albucore/functions.py`

 * *Files identical despite different names*

### Comparing `albucore-0.0.1/albucore/utils.py` & `albucore-0.0.2/albucore/utils.py`

 * *Files identical despite different names*

### Comparing `albucore-0.0.1/albucore.egg-info/PKG-INFO` & `albucore-0.0.2/albucore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albucore
-Version: 0.0.1
+Version: 0.0.2
 Summary: A high-performance image processing library designed to optimize and extend the Albumentations library with specialized functions for advanced image transformations. Perfect for developers working in computer vision who require efficient and scalable image augmentation.
 Home-page: https://github.com/albumentations-team/albucore
 Author: Vladimir I. Iglovikov
 License: MIT
 Keywords: Image Processing,Computer Vision,Image Augmentation,Albumentations,Optimization,Machine Learning,Deep Learning,Python Imaging,Data Augmentation,Performance,Efficiency,High-Performance,CV,OpenCV,Automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: tomli>=2.0.1
-Requires-Dist: opencv-python-headless>=4.9.0
+Requires-Dist: opencv-python-headless>=4.5.5.64
 
 # Albucore
 
 Albucore is a high-performance image processing library designed to optimize operations on images using Python and OpenCV, building upon the foundations laid by the popular Albumentations library. It offers specialized optimizations for different image data types and aims to provide faster processing times through efficient algorithm implementations.
 
 ## Features
```

### Comparing `albucore-0.0.1/pyproject.toml` & `albucore-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `albucore-0.0.1/setup.py` & `albucore-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     "numpy>=1.24.4",
     "tomli>=2.0.1",
 ]
 
+MIN_OPENCV_VERSION = "4.5.5.64"
+
 CHOOSE_INSTALL_REQUIRES = [
     (
-        ("opencv-python>=4.9.0", "opencv-contrib-python>=4.9.0", "opencv-contrib-python-headless>=4.9.0"),
-        "opencv-python-headless>=4.9.0",
+        (f"opencv-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python>={MIN_OPENCV_VERSION}", f"opencv-contrib-python-headless>={MIN_OPENCV_VERSION}"),
+        f"opencv-python-headless>={MIN_OPENCV_VERSION}",
     ),
 ]
 
 def get_version() -> str:
     current_dir = Path(__file__).parent
     version_file = current_dir / "albucore" / "__init__.py"
     with open(version_file, encoding="utf-8") as f:
```

### Comparing `albucore-0.0.1/tests/test_functions.py` & `albucore-0.0.2/tests/test_functions.py`

 * *Files identical despite different names*

