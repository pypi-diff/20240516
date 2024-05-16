# Comparing `tmp/geotifflib-0.0.2.tar.gz` & `tmp/geotifflib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotifflib-0.0.2.tar", last modified: Thu May 16 06:44:11 2024, max compression
+gzip compressed data, was "geotifflib-0.0.3.tar", last modified: Thu May 16 07:07:39 2024, max compression
```

## Comparing `geotifflib-0.0.2.tar` & `geotifflib-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.148890 geotifflib-0.0.2/
--rw-r--r--   0 flemyng    (501) staff       (20)    11357 2024-05-15 00:50:28.000000 geotifflib-0.0.2/LICENSE
--rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-16 01:19:27.000000 geotifflib-0.0.2/MANIFEST.in
--rw-r--r--   0 flemyng    (501) staff       (20)     2745 2024-05-16 06:44:11.148628 geotifflib-0.0.2/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)     2222 2024-05-16 06:41:13.000000 geotifflib-0.0.2/README.md
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.147379 geotifflib-0.0.2/geotifflib/
--rw-r--r--   0 flemyng    (501) staff       (20)       17 2024-05-16 05:17:54.000000 geotifflib-0.0.2/geotifflib/__init__.py
--rw-r--r--   0 flemyng    (501) staff       (20)    11032 2024-05-16 06:30:29.000000 geotifflib-0.0.2/geotifflib/io.py
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.148290 geotifflib-0.0.2/geotifflib.egg-info/
--rw-r--r--   0 flemyng    (501) staff       (20)     2745 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      284 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/SOURCES.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/dependency_links.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       52 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/entry_points.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        6 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/requires.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       11 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/top_level.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-16 06:44:11.148937 geotifflib-0.0.2/setup.cfg
--rw-r--r--   0 flemyng    (501) staff       (20)      878 2024-05-16 06:03:29.000000 geotifflib-0.0.2/setup.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 07:07:39.989971 geotifflib-0.0.3/
+-rw-r--r--   0 flemyng    (501) staff       (20)    11357 2024-05-15 00:50:28.000000 geotifflib-0.0.3/LICENSE
+-rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-16 01:19:27.000000 geotifflib-0.0.3/MANIFEST.in
+-rw-r--r--   0 flemyng    (501) staff       (20)     2547 2024-05-16 07:07:39.989755 geotifflib-0.0.3/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)     2024 2024-05-16 07:05:15.000000 geotifflib-0.0.3/README.md
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 07:07:39.987917 geotifflib-0.0.3/geotifflib/
+-rw-r--r--   0 flemyng    (501) staff       (20)       17 2024-05-16 05:17:54.000000 geotifflib-0.0.3/geotifflib/__init__.py
+-rw-r--r--   0 flemyng    (501) staff       (20)    10488 2024-05-16 07:04:41.000000 geotifflib-0.0.3/geotifflib/io.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 07:07:39.989392 geotifflib-0.0.3/geotifflib.egg-info/
+-rw-r--r--   0 flemyng    (501) staff       (20)     2547 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)      284 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/SOURCES.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/dependency_links.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       52 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/entry_points.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        6 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/requires.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       11 2024-05-16 07:07:39.000000 geotifflib-0.0.3/geotifflib.egg-info/top_level.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-16 07:07:39.990036 geotifflib-0.0.3/setup.cfg
+-rw-r--r--   0 flemyng    (501) staff       (20)      878 2024-05-16 07:06:29.000000 geotifflib-0.0.3/setup.py
```

### Comparing `geotifflib-0.0.2/LICENSE` & `geotifflib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geotifflib-0.0.2/PKG-INFO` & `geotifflib-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotifflib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python GeoTiff kit based on GDAL
 Home-page: https://github.com/Flemyng1999/geotifflib
 Author: flemyng feng
 Author-email: flemyng1999@outlook.com
 Keywords: python,tiff,geotiff,windows,mac,linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,40 +44,26 @@
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
 1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
-2. geotransform: tuple
-3. projection: str
-
-### read_array()
-
-根据文件路径读取GeoTiff数据。
-
-输入：
-
-1. 文件路径（Path or str）
-
-返回：
-
-1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 
 ### read_geo()
 
 根据文件路径读取GeoTiff数据形状、地理变换和投影。
 
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
-1. tiff的[宽，长]: tuple[int, int]
+1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 2. geotransform: tuple
 3. projection: str
 
 ### save()
 
 保存GeoTiff数据、地理变换和投影。
```

### Comparing `geotifflib-0.0.2/README.md` & `geotifflib-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,40 +28,26 @@
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
 1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
-2. geotransform: tuple
-3. projection: str
-
-### read_array()
-
-根据文件路径读取GeoTiff数据。
-
-输入：
-
-1. 文件路径（Path or str）
-
-返回：
-
-1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 
 ### read_geo()
 
 根据文件路径读取GeoTiff数据形状、地理变换和投影。
 
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
-1. tiff的[宽，长]: tuple[int, int]
+1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 2. geotransform: tuple
 3. projection: str
 
 ### save()
 
 保存GeoTiff数据、地理变换和投影。
```

### Comparing `geotifflib-0.0.2/geotifflib/io.py` & `geotifflib-0.0.3/geotifflib/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pathlib import Path
 from typing import Tuple, Optional, Union
 
 from osgeo import gdal
 import numpy as np
 
 
-def read(
+def read_geo(
     file_path: Union[Path, str]
 ) -> Tuple[Optional[np.ndarray], Optional[tuple], Optional[str]]:
     '''
     Read tif file
 
     param: file_path: Path or str, tif file path
     return: data: np.ndarray [band, width, height], geotransform: tuple, projection: str
@@ -38,15 +38,15 @@
     data = ds.ReadAsArray(0, 0, width, height)
     geotransform = ds.GetGeoTransform()
     projection = ds.GetProjection()
 
     return data, geotransform, projection
 
 
-def read_array(
+def read(
     file: Union[Path, str]
 ) -> Optional[np.ndarray]:
     '''
     Read tif file as array
 
     param: file: Path, tif file path
     return: data: np.ndarray
@@ -63,31 +63,14 @@
     img_width = data_set.RasterXSize
     img_height = data_set.RasterYSize
     img_data = data_set.ReadAsArray(0, 0, img_width, img_height)
 
     return img_data
 
 
-def read_geo(
-    file_path: Union[Path, str]
-) -> Tuple[Optional[Tuple[int, int]], Optional[tuple], Optional[str]]:
-    '''
-    Read tif file and get geotransform and projection
-
-    param: file_path: Path, tif file path
-    return: size: Tuple[int, int], geotransform: tuple, projection: str
-    '''
-    data, geotransform, projection = read_tif(file_path)
-    if data is not None:
-        height, width = data.shape[-2:]
-        return (height, width), geotransform, projection
-    else:
-        return None, None, None
-
-
 def save_without_memory_mapping(
     save_path: Union[Path, str],
     data: np.ndarray,
     geotransform: tuple,
     projection: str,
     output_dtype = gdal.GDT_Float32,
 ) -> None:
```

### Comparing `geotifflib-0.0.2/geotifflib.egg-info/PKG-INFO` & `geotifflib-0.0.3/geotifflib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotifflib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python GeoTiff kit based on GDAL
 Home-page: https://github.com/Flemyng1999/geotifflib
 Author: flemyng feng
 Author-email: flemyng1999@outlook.com
 Keywords: python,tiff,geotiff,windows,mac,linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -44,40 +44,26 @@
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
 1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
-2. geotransform: tuple
-3. projection: str
-
-### read_array()
-
-根据文件路径读取GeoTiff数据。
-
-输入：
-
-1. 文件路径（Path or str）
-
-返回：
-
-1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 
 ### read_geo()
 
 根据文件路径读取GeoTiff数据形状、地理变换和投影。
 
 输入：
 
 1. 文件路径（Path or str）
 
 返回：
 
-1. tiff的[宽，长]: tuple[int, int]
+1. tiff的数据矩阵（np.array）：shape = [波段，宽，长]
 2. geotransform: tuple
 3. projection: str
 
 ### save()
 
 保存GeoTiff数据、地理变换和投影。
```

### Comparing `geotifflib-0.0.2/setup.py` & `geotifflib-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 setup(
     name='geotifflib',
     version=VERSION,
     author='flemyng feng',
     author_email='flemyng1999@outlook.com',
     description='A Python GeoTiff kit based on GDAL',
```

