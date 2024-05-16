# Comparing `tmp/geotifflib-0.0.1.tar.gz` & `tmp/geotifflib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotifflib-0.0.1.tar", last modified: Thu May 16 05:22:39 2024, max compression
+gzip compressed data, was "geotifflib-0.0.2.tar", last modified: Thu May 16 06:44:11 2024, max compression
```

## Comparing `geotifflib-0.0.1.tar` & `geotifflib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 05:22:39.291113 geotifflib-0.0.1/
--rw-r--r--   0 flemyng    (501) staff       (20)    11357 2024-05-15 00:50:28.000000 geotifflib-0.0.1/LICENSE
--rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-16 01:19:27.000000 geotifflib-0.0.1/MANIFEST.in
--rw-r--r--   0 flemyng    (501) staff       (20)      858 2024-05-16 05:22:39.290866 geotifflib-0.0.1/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      334 2024-05-16 03:37:39.000000 geotifflib-0.0.1/README.md
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 05:22:39.289171 geotifflib-0.0.1/geotifflib/
--rw-r--r--   0 flemyng    (501) staff       (20)       17 2024-05-16 05:17:54.000000 geotifflib-0.0.1/geotifflib/__init__.py
--rw-r--r--   0 flemyng    (501) staff       (20)    10209 2024-05-16 05:16:46.000000 geotifflib-0.0.1/geotifflib/io.py
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 05:22:39.290443 geotifflib-0.0.1/geotifflib.egg-info/
--rw-r--r--   0 flemyng    (501) staff       (20)      858 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      284 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/SOURCES.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/dependency_links.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       52 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/entry_points.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        6 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/requires.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       11 2024-05-16 05:22:39.000000 geotifflib-0.0.1/geotifflib.egg-info/top_level.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-16 05:22:39.291179 geotifflib-0.0.1/setup.cfg
--rw-r--r--   0 flemyng    (501) staff       (20)      861 2024-05-16 04:42:27.000000 geotifflib-0.0.1/setup.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.148890 geotifflib-0.0.2/
+-rw-r--r--   0 flemyng    (501) staff       (20)    11357 2024-05-15 00:50:28.000000 geotifflib-0.0.2/LICENSE
+-rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-16 01:19:27.000000 geotifflib-0.0.2/MANIFEST.in
+-rw-r--r--   0 flemyng    (501) staff       (20)     2745 2024-05-16 06:44:11.148628 geotifflib-0.0.2/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)     2222 2024-05-16 06:41:13.000000 geotifflib-0.0.2/README.md
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.147379 geotifflib-0.0.2/geotifflib/
+-rw-r--r--   0 flemyng    (501) staff       (20)       17 2024-05-16 05:17:54.000000 geotifflib-0.0.2/geotifflib/__init__.py
+-rw-r--r--   0 flemyng    (501) staff       (20)    11032 2024-05-16 06:30:29.000000 geotifflib-0.0.2/geotifflib/io.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-16 06:44:11.148290 geotifflib-0.0.2/geotifflib.egg-info/
+-rw-r--r--   0 flemyng    (501) staff       (20)     2745 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)      284 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/SOURCES.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/dependency_links.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       52 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/entry_points.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        6 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/requires.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       11 2024-05-16 06:44:11.000000 geotifflib-0.0.2/geotifflib.egg-info/top_level.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-16 06:44:11.148937 geotifflib-0.0.2/setup.cfg
+-rw-r--r--   0 flemyng    (501) staff       (20)      878 2024-05-16 06:03:29.000000 geotifflib-0.0.2/setup.py
```

### Comparing `geotifflib-0.0.1/LICENSE` & `geotifflib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geotifflib-0.0.1/geotifflib/io.py` & `geotifflib-0.0.2/geotifflib/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,66 +5,74 @@
 @Time    :   2024/04/23 15:10:20
 @Author  :   Flemyng 
 @Desc    :   GeoTiff kit for reading ,writing tiff file and ect.
 '''
 
 import os
 from pathlib import Path
-from typing import Tuple, Optional
+from typing import Tuple, Optional, Union
 
 from osgeo import gdal
 import numpy as np
 
 
 def read(
-    file_path: Path
+    file_path: Union[Path, str]
 ) -> Tuple[Optional[np.ndarray], Optional[tuple], Optional[str]]:
     '''
     Read tif file
 
-    param: file_path: Path, tif file path
-    return: data: np.ndarray, geotransform: tuple, projection: str
+    param: file_path: Path or str, tif file path
+    return: data: np.ndarray [band, width, height], geotransform: tuple, projection: str
     '''
-    ds = gdal.Open(str(file_path))
+    # 如果输入是 Path，将其转换为 str 对象
+    if isinstance(file_path, Path):
+        file_path = str(file_path)
+
+    ds = gdal.Open(file_path)
     if ds is None:
         print(f"Cannot open {file_path}")
         return None, None, None
 
     width = ds.RasterXSize
     height = ds.RasterYSize
     data = ds.ReadAsArray(0, 0, width, height)
     geotransform = ds.GetGeoTransform()
     projection = ds.GetProjection()
 
     return data, geotransform, projection
 
 
 def read_array(
-    file: Path
+    file: Union[Path, str]
 ) -> Optional[np.ndarray]:
     '''
     Read tif file as array
 
     param: file: Path, tif file path
     return: data: np.ndarray
     '''
-    data_set = gdal.Open(str(file), gdal.GA_ReadOnly)
+    # 如果输入是 Path，将其转换为 str 对象
+    if isinstance(file_path, Path):
+        file_path = str(file_path)
+
+    data_set = gdal.Open(file, gdal.GA_ReadOnly)
     if data_set is None:
         print(f"Cannot open {file}")
         return None
 
     img_width = data_set.RasterXSize
     img_height = data_set.RasterYSize
     img_data = data_set.ReadAsArray(0, 0, img_width, img_height)
 
     return img_data
 
 
 def read_geo(
-    file_path: Path
+    file_path: Union[Path, str]
 ) -> Tuple[Optional[Tuple[int, int]], Optional[tuple], Optional[str]]:
     '''
     Read tif file and get geotransform and projection
 
     param: file_path: Path, tif file path
     return: size: Tuple[int, int], geotransform: tuple, projection: str
     '''
@@ -73,36 +81,40 @@
         height, width = data.shape[-2:]
         return (height, width), geotransform, projection
     else:
         return None, None, None
 
 
 def save_without_memory_mapping(
-    save_path: Path,
+    save_path: Union[Path, str],
     data: np.ndarray,
     geotransform: tuple,
     projection: str,
     output_dtype = gdal.GDT_Float32,
 ) -> None:
     '''
     Save tif file without memory mapping
 
     param: save_path: Path, tif file save path
     param: data: np.ndarray, tif file data
     param: geotransform: tuple, tif file geotransform
     param: projection: str, tif file projection
     param: output_dtype: gdal.GDT_Float32, tif file data type
     '''
+    # 如果输入是 Path，将其转换为 str 对象
+    if isinstance(save_path, Path):
+        save_path = str(save_path)
+
     im_bands = 1 if len(data.shape) == 2 else data.shape[0]
     im_height, im_width = data.shape[-2:]
 
     options = ["COMPRESS=LZW"]  # 使用LZW压缩
     driver = gdal.GetDriverByName("GTiff")
     new_dataset = driver.Create(
-        str(save_path),
+        save_path,
         im_width, im_height, im_bands,
         output_dtype, options=options
     )
     new_dataset.SetGeoTransform(geotransform)
     new_dataset.SetProjection(projection)
 
     if im_bands == 1:
@@ -112,29 +124,33 @@
             new_dataset.GetRasterBand(i + 1).WriteArray(data[i])
 
     new_dataset = None  # 确保数据被写入并释放资源
     driver = None
 
 
 def save(
-    save_path: Path,
+    save_path: Union[Path, str],
     data: np.ndarray,
     geotransform: tuple,
     projection: str,
     output_dtype=gdal.GDT_Float32
 ) -> None:
     '''
     Save tif file with memory mapping
 
     param: save_path: Path, tif file save path
     param: data: np.ndarray, tif file data
     param: geotransform: tuple, tif file geotransform
     param: projection: str, tif file projection
     param: output_dtype: gdal.GDT_Float32, tif file data type
     '''
+    # 如果输入是 Path，将其转换为 str 对象
+    if isinstance(save_path, Path):
+        save_path = str(save_path)
+
     im_bands = 1 if len(data.shape) == 2 else data.shape[0]
     im_height, im_width = data.shape[-2:]
 
     # 创建内存数据集
     mem_driver = gdal.GetDriverByName('MEM')
     mem_dataset = mem_driver.Create('', im_width, im_height, im_bands, output_dtype)
 
@@ -144,36 +160,40 @@
 
     # 写入数据到内存数据集
     for i in range(im_bands):
         mem_dataset.GetRasterBand(i + 1).WriteArray(data[i])
 
     # 将内存数据集保存到文件
     file_driver = gdal.GetDriverByName('GTiff')
-    file_driver.CreateCopy(str(save_path), mem_dataset, 0, ["COMPRESS=LZW"])
+    file_driver.CreateCopy(save_path, mem_dataset, 0, ["COMPRESS=LZW"])
 
     mem_dataset = None  # 释放内存数据集资源
 
 
 def save_array(
-    save_path: Path,
+    save_path: Union[Path, str],
     data: np.ndarray,
     output_dtype = gdal.GDT_Float32,
-):
+) -> None:
     '''
     Save tif file from array
 
     param: save_path: Path, tif file save path
     param: data: np.ndarray, tif file data
     param: output_dtype: gdal.GDT_Float32, tif file data type
     '''
+    # 如果输入是 Path，将其转换为 str 对象
+    if isinstance(save_path, Path):
+        save_path = str(save_path)
+
     im_bands = 1 if len(data.shape) == 2 else data.shape[0]
     im_height, im_width = data.shape[-2:]
 
     driver = gdal.GetDriverByName("GTiff")
-    new_dataset = driver.Create(str(save_path), im_width, im_height, im_bands, output_dtype)
+    new_dataset = driver.Create(save_path, im_width, im_height, im_bands, output_dtype)
 
     if im_bands == 1:
         new_dataset.GetRasterBand(1).WriteArray(data)
     else:
         for i in range(im_bands):
             new_dataset.GetRasterBand(i + 1).WriteArray(data[i])
 
@@ -342,7 +362,8 @@
     # output_path = Path('/Volumes/2023HSI/raw/2023_07_17/5ref/1and3_corr_elm.tif')
 
     # # 合并图像
     # merge(input_files_pathes, output_path)
 
     tif_path = Path('/Volumes/2023HSI/raw/2023_07_17/5ref/1and3_corr_elm.tif')
     data, geotransform, projection = read(tif_path)
+    save(tif_path.parent / 'test.tif', data, geotransform, projection)
```

### Comparing `geotifflib-0.0.1/setup.py` & `geotifflib-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 setup(
     name='geotifflib',
     version=VERSION,
     author='flemyng feng',
     author_email='flemyng1999@outlook.com',
     description='A Python GeoTiff kit based on GDAL',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     keywords=['python', 'tiff', 'geotiff','windows','mac','linux'],
     url='https://github.com/Flemyng1999/geotifflib',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     install_requires=[
         'numpy',
     ],
     entry_points={
         'console_scripts': [
             'geotifflib = geotifflib.main:main'
         ]
```

