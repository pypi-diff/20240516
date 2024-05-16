# Comparing `tmp/nrstitcher_utils-0.1.0.dev8.tar.gz` & `tmp/nrstitcher_utils-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrstitcher_utils-0.1.0.dev8.tar", last modified: Fri Apr 26 13:01:25 2024, max compression
+gzip compressed data, was "nrstitcher_utils-0.1.0.dev9.tar", last modified: Wed May 15 07:05:31 2024, max compression
```

## Comparing `nrstitcher_utils-0.1.0.dev8.tar` & `nrstitcher_utils-0.1.0.dev9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/
--rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/LICENSE
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      251 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/README.md
--rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/pyproject.toml
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/setup.cfg
--rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/setup.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/app/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/app/__init__.py
--rwxr-xr-x   0 payno     (1000) payno     (1000)     8306 2024-04-26 12:57:26.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3144 2024-04-26 12:57:47.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/h5_settings.py
--rw-r--r--   0 payno     (1000) payno     (1000)     8258 2024-04-26 12:59:47.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/ht_vol.py
--rw-r--r--   0 payno     (1000) payno     (1000)     3460 2024-04-26 12:52:46.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/utils.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/resources/
--rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/resources/__init__.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/resources/config_files/
--rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/resources/config_files/__init__.py
--rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-04-26 13:01:18.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/version.py
-drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-04-26 13:01:25.856637 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/
--rw-r--r--   0 payno     (1000) payno     (1000)     3612 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/entry_points.txt
--rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/requires.txt
--rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-04-26 13:01:25.000000 nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/
+-rw-r--r--   0 payno     (1000) payno     (1000)     1241 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/LICENSE
+-rw-r--r--   0 payno     (1000) payno     (1000)     3773 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      411 2024-05-15 07:05:10.000000 nrstitcher_utils-0.1.0.dev9/README.md
+-rw-r--r--   0 payno     (1000) payno     (1000)     2131 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/setup.cfg
+-rw-r--r--   0 payno     (1000) payno     (1000)       38 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/setup.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/app/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/app/__init__.py
+-rwxr-xr-x   0 payno     (1000) payno     (1000)     8527 2024-05-15 07:05:10.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/app/nrs_config_id16a_ht.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3144 2024-05-15 07:05:10.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/h5_settings.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     8310 2024-05-15 07:05:10.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/ht_vol.py
+-rw-r--r--   0 payno     (1000) payno     (1000)     3460 2024-05-15 07:05:10.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/utils.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/resources/
+-rw-r--r--   0 payno     (1000) payno     (1000)      282 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/resources/__init__.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/resources/config_files/
+-rw-r--r--   0 payno     (1000) payno     (1000)        0 2024-04-26 11:40:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/resources/config_files/__init__.py
+-rw-r--r--   0 payno     (1000) payno     (1000)       45 2024-05-15 07:05:14.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/version.py
+drwxr-xr-x   0 payno     (1000) payno     (1000)        0 2024-05-15 07:05:31.824512 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/
+-rw-r--r--   0 payno     (1000) payno     (1000)     3773 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1000) payno     (1000)      706 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)        1 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       86 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/entry_points.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)      138 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/requires.txt
+-rw-r--r--   0 payno     (1000) payno     (1000)       17 2024-05-15 07:05:31.000000 nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/top_level.txt
```

### Comparing `nrstitcher_utils-0.1.0.dev8/LICENSE` & `nrstitcher_utils-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev8/PKG-INFO` & `nrstitcher_utils-0.1.0.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
         
@@ -71,7 +71,11 @@
 The goal of this project is to ease usage of ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html) with esrf datasets
 
 ## how to access it from esrf infrascture
 
 ``` bash
 module load nrstitcher_utils
 ```
+
+## documentation
+
+Latest build documentation can be found [here](https://nrstitcher-utils-tomotools-7f52d4ab174ba161998ecb1bcc6adfcada61.gitlab-pages.esrf.fr/)
```

### Comparing `nrstitcher_utils-0.1.0.dev8/pyproject.toml` & `nrstitcher_utils-0.1.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/app/nrs_config_id16a_ht.py` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/app/nrs_config_id16a_ht.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import argparse
 import glob
 import os
 import shutil
 import sys
 import logging
+from pathlib import Path
 
 # import from pi2 / NRstitcher -> see https://github.com/arttumiettinen/pi2/blob/master/python_scripts/default_stitch_settings.py
 from default_stitch_settings import write_stitch_settings  # pylint: disable=E0401
 from nrstitcher_utils.core.h5_settings import H5Settings
 from nrstitcher_utils.core.ht_vol import HTVol
 from nrstitcher_utils.core import utils
 from nrstitcher_utils.resources import get_config_file
@@ -35,15 +36,15 @@
         Arguments:
         None
 
         Returns:
         Name of the h5 file as a string.
         """
 
-        h5_filename = glob.glob(h5_folder + "*.h5")[0]
+        h5_filename = glob.glob(h5_folder + "/*.h5")[0]
 
         return h5_filename
 
     argv = sys.argv[1:]
     argparser = argparse.ArgumentParser(
         description="Creates input file for nr_stitcher.py program from id16a holotomography scan settings."
     )
@@ -167,15 +168,18 @@
 
         # Assume standard image size pf 3216 x 3216 x 3216 px^3
         Xdim_ref = 3216
         Ydim_ref = 3216
         Zdim_ref = 3216
 
         # Get scan settings from .h5 file (the one from the experiment, containing all the scans)
-        settings_file = get_h5file(h5_folder=args.base_dir + "../")
+        settings_folder = Path(args.base_dir).parent
+        _logger.info(f"try to get settings from {settings_folder}")
+        # try to read the setting from the proposal file (like ls "ls2892-id16a.h5")
+        settings_file = get_h5file(str(settings_folder))
         first_dist = args.distances[0]
         scan_settings = H5Settings(settings_file, vol, scan_suffix=f"_{first_dist}_")
         motor_positions = scan_settings.get_motor_positions()
         tomo_params = scan_settings.get_tomo_parameters()
 
         sx = motor_positions["sx"]
         sz = motor_positions["sz"]
```

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/h5_settings.py` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/h5_settings.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/ht_vol.py` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/ht_vol.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
             vol = self.pi.newimage(ImageDataType.FLOAT32, self.y, self.x, self.z)
         elif dtype == "uint32":
             vol = self.pi.newimage(ImageDataType.UINT32, self.y, self.x, self.z)
         elif dtype == "uint16":
             vol = self.pi.newimage(ImageDataType.UINT16, self.y, self.x, self.z)
         elif dtype == "uint8":
             vol = self.pi.newimage(ImageDataType.UINT8, self.y, self.x, self.z)
+        else:
+            raise NotImplementedError
 
         return vol
 
     def bit_conversion(self):
         """
         Convert volume from original datatype to new datatype with specified range.
```

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils/core/utils.py` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/PKG-INFO` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrstitcher_utils
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: NRStitcher utils for esrf usage
 Author: Arttu Miettenen, Yervand Azatian
 Author-email: Jayde Livingstone <jayde.livingstone@gmail.com>, Henri Payno <henri.payno@esrf.fr>
 License: The nrstitcher_utils library goal is to ease usage of nrstitcher at esrf
         
         nrstitcher_utils is distributed under the MIT license.
         
@@ -71,7 +71,11 @@
 The goal of this project is to ease usage of ![NRSticher program](https://pi2-docs.readthedocs.io/en/latest/nr_stitcher.html) with esrf datasets
 
 ## how to access it from esrf infrascture
 
 ``` bash
 module load nrstitcher_utils
 ```
+
+## documentation
+
+Latest build documentation can be found [here](https://nrstitcher-utils-tomotools-7f52d4ab174ba161998ecb1bcc6adfcada61.gitlab-pages.esrf.fr/)
```

### Comparing `nrstitcher_utils-0.1.0.dev8/src/nrstitcher_utils.egg-info/SOURCES.txt` & `nrstitcher_utils-0.1.0.dev9/src/nrstitcher_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

