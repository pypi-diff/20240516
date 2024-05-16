# Comparing `tmp/pyllsm5dtools-1.0.5.tar.gz` & `tmp/pyllsm5dtools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllsm5dtools-1.0.5.tar", last modified: Mon Apr 29 22:29:58 2024, max compression
+gzip compressed data, was "pyllsm5dtools-1.1.0.tar", last modified: Wed May 15 20:48:53 2024, max compression
```

## Comparing `pyllsm5dtools-1.0.5.tar` & `pyllsm5dtools-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.0.5/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.062394 pyllsm5dtools-1.0.5/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6472 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3219 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-29 22:27:17.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-29 22:29:58.000000 pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.0.5/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-29 22:29:58.066394 pyllsm5dtools-1.0.5/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-29 22:28:38.000000 pyllsm5dtools-1.0.5/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-15 20:48:53.423208 pyllsm5dtools-1.1.0/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.1.0/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-15 20:48:53.423208 pyllsm5dtools-1.1.0/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-15 20:48:53.423208 pyllsm5dtools-1.1.0/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3564 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2957 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3118 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5072 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4972 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3074 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6120 2024-05-15 19:32:59.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6008 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3259 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3270 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3382 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2691 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-05-15 19:33:00.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8968 2024-05-15 19:32:48.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-15 20:48:53.423208 pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-05-15 20:48:53.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-05-15 20:48:53.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-15 20:48:53.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-05-15 20:48:53.000000 pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.1.0/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-15 20:48:53.423208 pyllsm5dtools-1.1.0/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-05-15 20:11:26.000000 pyllsm5dtools-1.1.0/setup.py
```

### Comparing `pyllsm5dtools-1.0.5/LICENSE.txt` & `pyllsm5dtools-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,34 @@
-import math
 import os
 import subprocess
 
 
-def XR_FSC_analysis_wrapper(dataPaths, **kwargs):
-    function_name = "XR_FSC_analysis_wrapper"
-    XR_FSC_analysis_wrapper_dict = {
-        "outDirstr": [kwargs.get("outDirstr", "FSCs"), "char"],
-        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
-        "dz": [kwargs.get("dz", 0.1), "numericScalar"],
-        "dr": [kwargs.get("dr", 1), "numericScalar"],
-        "dtheta": [kwargs.get("dtheta", math.pi/12), "numericScalar"],
-        "resThreshMethod": [kwargs.get("resThreshMethod", "fixed"), "char"],
-        "resThresh": [kwargs.get("resThresh", 0.2), "numericScalar"],
-        "N": [kwargs.get("N", [251,251,251]), "numericArr"],
-        "bbox": [kwargs.get("bbox", []), "numericScalar"],
-        "resAxis": [kwargs.get("resAxis", "xz"), "char"],
-        "skipConeRegion": [kwargs.get("skipConeRegion", True), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['tif']), "cell"],
-        "Channels": [kwargs.get("Channels", [488,560]), "numericArr"],
-        "multiRegions": [kwargs.get("multiRegions", False), "logical"],
-        "regionInterval": [kwargs.get("regionInterval", [50,50,-1]), "numericArr"],
-        "regionGrid": [kwargs.get("regionGrid", []), "numericScalar"],
-        "clipPer": [kwargs.get("clipPer", []), "numericScalar"],
-        "suffix": [kwargs.get("suffix", "decon"), "char"],
-        "iterInterval": [kwargs.get("iterInterval", 5), "numericScalar"],
+def XR_zarrToTiff_wrapper(dataPaths, **kwargs):
+    function_name = "XR_zarrToTiff_wrapper"
+    XR_zarrToTiff_wrapper_dict = {
+        "resultDirName": [kwargs.get("resultDirName", "tiffs"), "char"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA','CamB']), "cell"],
+        "usrFcn": [kwargs.get("usrFcn", ""), "err"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
+        "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
+        "uuid": [kwargs.get("uuid", ""), "char"],
+        "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
+        "unitWaitTime": [kwargs.get("unitWaitTime", 30), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
-    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
+    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
     
-    for key, value in XR_FSC_analysis_wrapper_dict.items():
+    for key, value in XR_zarrToTiff_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_MIP_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import subprocess
 
 
 def XR_MIP_wrapper(dataPaths, **kwargs):
     function_name = "XR_MIP_wrapper"
     XR_MIP_wrapper_dict = {
+        "resultDirName": [kwargs.get("resultDirName", "MIPs"), "char"],
         "axis": [kwargs.get("axis", [0,0,1]), "numericArr"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
-        "BatchSize": [kwargs.get("BatchSize", [2048,2048,2048]), "numericArr"],
-        "Save16bit": [kwargs.get("Save16bit", True), "logical"],
+        "batchSize": [kwargs.get("batchSize", [2048,2048,2048]), "numericArr"],
+        "save16bit": [kwargs.get("save16bit", True), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "parseParfor": [kwargs.get("parseParfor", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 3), "numericScalar"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs/"), "char"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "debug": [kwargs.get("debug", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_crop_dataset.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import os
 import subprocess
 
 
-def XR_crop_dataset(dataPaths, resultPaths, bbox, **kwargs):
+def XR_crop_dataset(dataPaths, inputBbox, **kwargs):
     function_name = "XR_crop_dataset"
     XR_crop_dataset_dict = {
+        "resultDirName": [kwargs.get("resultDirName", "Cropped"), "char"],
         "cropType": [kwargs.get("cropType", "fixed"), "char"],
         "pad": [kwargs.get("pad", False), "logical"],
-        "lastStart": [kwargs.get("lastStart", []), "numericArr"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
+        "lastStartCoords": [kwargs.get("lastStartCoords", []), "numericArr"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "largeZarr": [kwargs.get("largeZarr", False), "logical"],
         "saveZarr": [kwargs.get("saveZarr", False), "logical"],
-        "BlockSize": [kwargs.get("BlockSize", [500,500,500]), "numericArr"],
-        "Save16bit": [kwargs.get("Save16bit", False), "logical"],
+        "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
+        "save16bit": [kwargs.get("save16bit", False), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
-    resultPathsString = "{" + ",".join(f"'{item}'" for item in resultPaths) + "}"
-    bboxString = "[" + ",".join(str(item) for item in bbox) + "]"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" \"{resultPathsString}\" \"{bboxString}\" "
+    inputBboxString = "[" + ",".join(str(item) for item in inputBbox) + "]"
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" \"{inputBboxString}\" "
     
     for key, value in XR_crop_dataset_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_decon_data_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 import os
 import subprocess
 
 
-def XR_decon_data_wrapper(dataPaths, **kwargs):
-    function_name = "XR_decon_data_wrapper"
-    XR_decon_data_wrapper_dict = {
-        "deconPathstr": [kwargs.get("deconPathstr", ""), "char"],
-        "Overwrite": [kwargs.get("Overwrite", False), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
-        "Channels": [kwargs.get("Channels", [488,560,642]), "numericArr"],
-        "SkewAngle": [kwargs.get("SkewAngle", 32.45), "numericScalar"],
-        "dz": [kwargs.get("dz", 0.5), "numericScalar"],
+def XR_matlab_stitching_wrapper(dataPath, imageListFileName, **kwargs):
+    function_name = "XR_matlab_stitching_wrapper"
+    XR_matlab_stitching_wrapper_dict = {
+        "streaming": [kwargs.get("streaming", False), "logical"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
+        "multiLoc": [kwargs.get("multiLoc", False), "logical"],
+        "processedDirStr": [kwargs.get("processedDirStr", ""), "char"],
+        "stitchInfoFullpath": [kwargs.get("stitchInfoFullpath", ""), "char"],
+        "DS": [kwargs.get("DS", False), "logical"],
+        "DSR": [kwargs.get("DSR", False), "logical"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
-        "Reverse": [kwargs.get("Reverse", True), "logical"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "sCMOSCameraFlip": [kwargs.get("sCMOSCameraFlip", False), "logical"],
-        "Save16bit": [kwargs.get("Save16bit", False), "logical"],
-        "onlyFirstTP": [kwargs.get("onlyFirstTP", False), "logical"],
+        "dz": [kwargs.get("dz", 0.5), "numericScalar"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
+        "reverse": [kwargs.get("reverse", False), "logical"],
         "parseSettingFile": [kwargs.get("parseSettingFile", False), "logical"],
-        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
-        "Decon": [kwargs.get("Decon", True), "logical"],
-        "cudaDecon": [kwargs.get("cudaDecon", False), "logical"],
-        "cppDecon": [kwargs.get("cppDecon", False), "logical"],
-        "cppDeconPath": [kwargs.get("cppDeconPath", "/global/home/groups/software/sl-7.x86_64/modules/RLDecon_CPU/20200718/build-cluster/cpuDeconv"), "char"],
-        "loadModules": [kwargs.get("loadModules", "moduleloadgcc/4.8.5;moduleloadfftw/3.3.6-gcc;moduleloadboost/1.65.1-gcc;moduleloadlibtiff/4.1.0;"), "char"],
-        "cudaDeconPath": [kwargs.get("cudaDeconPath", "/global/home/groups/software/sl-7.x86_64/modules/cudaDecon/bin/cudaDeconv"), "char"],
-        "OTFGENPath": [kwargs.get("OTFGENPath", "/global/home/groups/software/sl-7.x86_64/modules/cudaDecon/bin/radialft"), "char"],
-        "Background": [kwargs.get("Background", []), "numericScalar"],
-        "dzPSF": [kwargs.get("dzPSF", 0.1), "numericScalar"],
-        "EdgeErosion": [kwargs.get("EdgeErosion", 8), "numericScalar"],
-        "ErodeByFTP": [kwargs.get("ErodeByFTP", True), "logical"],
-        "deconRotate": [kwargs.get("deconRotate", False), "logical"],
-        "psfFullpaths": [kwargs.get("psfFullpaths", ['','','']), "cell"],
-        "rotatePSF": [kwargs.get("rotatePSF", False), "logical"],
-        "DeconIter": [kwargs.get("DeconIter", 15), "numericScalar"],
-        "RLMethod": [kwargs.get("RLMethod", "simplified"), "char"],
-        "wienerAlpha": [kwargs.get("wienerAlpha", 0.005), "numericScalar"],
-        "OTFCumThresh": [kwargs.get("OTFCumThresh", 0.9), "numericScalar"],
-        "hanWinBounds": [kwargs.get("hanWinBounds", [0.8,1.0]), "numericArr"],
-        "skewed": [kwargs.get("skewed", []), "logical"],
-        "fixIter": [kwargs.get("fixIter", False), "logical"],
-        "errThresh": [kwargs.get("errThresh", []), "numericScalar"],
-        "debug": [kwargs.get("debug", False), "logical"],
-        "saveStep": [kwargs.get("saveStep", 5), "numericScalar"],
-        "psfGen": [kwargs.get("psfGen", True), "logical"],
-        "GPUJob": [kwargs.get("GPUJob", False), "logical"],
-        "BatchSize": [kwargs.get("BatchSize", [1024,1024,1024]), "numericArr"],
-        "BlockSize": [kwargs.get("BlockSize", [256,256,256]), "numericArr"],
-        "zarrSubSize": [kwargs.get("zarrSubSize", []), "numericArr"],
-        "largeFile": [kwargs.get("largeFile", False), "logical"],
-        "largeMethod": [kwargs.get("largeMethod", "inmemory"), "char"],
+        "axisOrder": [kwargs.get("axisOrder", "x,y,z"), "char"],
+        "dataOrder": [kwargs.get("dataOrder", "y,x,z"), "char"],
+        "objectiveScan": [kwargs.get("objectiveScan", False), "logical"],
+        "IOScan": [kwargs.get("IOScan", False), "logical"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
-        "saveZarr": [kwargs.get("saveZarr", False), "logical"],
-        "damper": [kwargs.get("damper", 1), "numericScalar"],
-        "scaleFactor": [kwargs.get("scaleFactor", []), "numericScalar"],
-        "deconOffset": [kwargs.get("deconOffset", 0), "numericScalar"],
-        "deconMaskFns": [kwargs.get("deconMaskFns", []), "cell"],
+        "largeZarr": [kwargs.get("largeZarr", False), "logical"],
+        "poolSize": [kwargs.get("poolSize", []), "numericScalar"],
+        "batchSize": [kwargs.get("batchSize", [500,500,500]), "numericArr"],
+        "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
+        "shardSize": [kwargs.get("shardSize", []), "numericArr"],
+        "resampleType": [kwargs.get("resampleType", "xy_isotropic"), "char"],
+        "resampleFactor": [kwargs.get("resampleFactor", []), "numericArr"],
+        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
+        "tileOutBbox": [kwargs.get("tileOutBbox", []), "numericArr"],
+        "tileOffset": [kwargs.get("tileOffset", 0), "numericScalar"],
+        "resultDirName": [kwargs.get("resultDirName", "matlab_stitch"), "char"],
+        "blendMethod": [kwargs.get("blendMethod", "none"), "char"],
+        "overlapType": [kwargs.get("overlapType", ""), "char"],
+        "xcorrShift": [kwargs.get("xcorrShift", True), "logical"],
+        "xyMaxOffset": [kwargs.get("xyMaxOffset", 300), "numericArr"],
+        "zMaxOffset": [kwargs.get("zMaxOffset", 50), "numericScalar"],
+        "xcorrDownsample": [kwargs.get("xcorrDownsample", [2,2,1]), "numericArr"],
+        "xcorrThresh": [kwargs.get("xcorrThresh", 0.25), "numericScalar"],
+        "padSize": [kwargs.get("padSize", []), "numericArr"],
+        "outBbox": [kwargs.get("outBbox", []), "numericArr"],
+        "xcorrMode": [kwargs.get("xcorrMode", "primaryFirst"), "char"],
+        "shiftMethod": [kwargs.get("shiftMethod", "grid"), "char"],
+        "axisWeight": [kwargs.get("axisWeight", [1,0.1,10]), "numericArr"],
+        "groupFile": [kwargs.get("groupFile", ""), "char"],
+        "primaryCh": [kwargs.get("primaryCh", ""), "char"],
+        "usePrimaryCoords": [kwargs.get("usePrimaryCoords", False), "logical"],
+        "save16bit": [kwargs.get("save16bit", False), "logical"],
+        "edgeArtifacts": [kwargs.get("edgeArtifacts", 0), "numericScalar"],
+        "distBboxes": [kwargs.get("distBboxes", []), "numericArr"],
+        "saveMIP": [kwargs.get("saveMIP", True), "logical"],
+        "stitchMIP": [kwargs.get("stitchMIP", []), "logicalArr"],
+        "onlineStitch": [kwargs.get("onlineStitch", False), "logical"],
+        "processFunPath": [kwargs.get("processFunPath", ""), "cell"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
-        "parseParfor": [kwargs.get("parseParfor", False), "logical"],
+        "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 8), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
-        "unitWaitTime": [kwargs.get("unitWaitTime", 10), "numericScalar"],
-        "maxWaitLoopNum": [kwargs.get("maxWaitLoopNum", 10), "numericScalar"],
+        "unitWaitTime": [kwargs.get("unitWaitTime", 0.1), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"],
-        "GPUConfigFile": [kwargs.get("GPUConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
-    dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
+    dataPathString = "{" + ",".join(f"'{item}'" for item in dataPath) + "}"
+    imageListFileNameString = "{" + ",".join(f"'{item}'" for item in imageListFileName) + "}"
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathString}\" \"{imageListFileNameString}\" "
     
-    for key, value in XR_decon_data_wrapper_dict.items():
+    for key, value in XR_matlab_stitching_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import os
 import subprocess
 
 
-def XR_deskew_rotate_data_wrapper(dataPaths, **kwargs):
-    function_name = "XR_deskew_rotate_data_wrapper"
-    XR_deskew_rotate_data_wrapper_dict = {
-        "DSDirStr": [kwargs.get("DSDirStr", "DS/"), "char"],
-        "DSRDirStr": [kwargs.get("DSRDirStr", "DSR/"), "char"],
-        "Deskew": [kwargs.get("Deskew", True), "logical"],
-        "Rotate": [kwargs.get("Rotate", True), "logical"],
-        "Overwrite": [kwargs.get("Overwrite", False), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
+def XR_decon_data_wrapper(dataPaths, **kwargs):
+    function_name = "XR_decon_data_wrapper"
+    XR_decon_data_wrapper_dict = {
+        "resultDirName": [kwargs.get("resultDirName", "matlab_decon"), "char"],
+        "overwrite": [kwargs.get("overwrite", False), "logical"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
         "dz": [kwargs.get("dz", 0.5), "numericScalar"],
-        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
-        "SkewAngle": [kwargs.get("SkewAngle", 32.45), "numericScalar"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "ZstageScan": [kwargs.get("ZstageScan", False), "logical"],
-        "Reverse": [kwargs.get("Reverse", False), "logical"],
-        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
+        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericArr"],
+        "save16bit": [kwargs.get("save16bit", False), "logical"],
         "parseSettingFile": [kwargs.get("parseSettingFile", False), "logical"],
-        "Crop": [kwargs.get("Crop", False), "logical"],
-        "DSRCombined": [kwargs.get("DSRCombined", True), "logical"],
-        "LLFFCorrection": [kwargs.get("LLFFCorrection", False), "logical"],
-        "BKRemoval": [kwargs.get("BKRemoval", False), "logical"],
-        "LowerLimit": [kwargs.get("LowerLimit", 0.4), "numericScalar"],
-        "constOffset": [kwargs.get("constOffset", []), "numericScalar"],
-        "LSImagePaths": [kwargs.get("LSImagePaths", ['','','']), "cell"],
-        "BackgroundPaths": [kwargs.get("BackgroundPaths", ['','','']), "cell"],
-        "Save16bit": [kwargs.get("Save16bit", False), "logical"],
-        "save3DStack": [kwargs.get("save3DStack", True), "logical"],
-        "SaveMIP": [kwargs.get("SaveMIP", True), "logical"],
+        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
+        "background": [kwargs.get("background", []), "numericScalar"],
+        "dzPSF": [kwargs.get("dzPSF", 0.1), "numericScalar"],
+        "edgeErosion": [kwargs.get("edgeErosion", 8), "numericScalar"],
+        "erodeByFTP": [kwargs.get("erodeByFTP", True), "logical"],
+        "psfFullpaths": [kwargs.get("psfFullpaths", ['','','']), "cell"],
+        "deconIter": [kwargs.get("deconIter", 15), "numericScalar"],
+        "RLMethod": [kwargs.get("RLMethod", "simplified"), "char"],
+        "wienerAlpha": [kwargs.get("wienerAlpha", 0.005), "numericScalar"],
+        "OTFCumThresh": [kwargs.get("OTFCumThresh", 0.9), "numericScalar"],
+        "hannWinBounds": [kwargs.get("hannWinBounds", [0.8,1.0]), "numericArr"],
+        "skewed": [kwargs.get("skewed", []), "logical"],
+        "debug": [kwargs.get("debug", False), "logical"],
+        "saveStep": [kwargs.get("saveStep", 5), "numericScalar"],
+        "psfGen": [kwargs.get("psfGen", True), "logical"],
+        "GPUJob": [kwargs.get("GPUJob", False), "logical"],
+        "deconRotate": [kwargs.get("deconRotate", False), "logical"],
+        "batchSize": [kwargs.get("batchSize", [1024,1024,1024]), "numericArr"],
+        "blockSize": [kwargs.get("blockSize", [256,256,256]), "numericArr"],
         "largeFile": [kwargs.get("largeFile", False), "logical"],
+        "largeMethod": [kwargs.get("largeMethod", "inmemory"), "char"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "saveZarr": [kwargs.get("saveZarr", False), "logical"],
-        "BatchSize": [kwargs.get("BatchSize", [1024,1024,1024]), "numericArr"],
-        "BlockSize": [kwargs.get("BlockSize", [256,256,256]), "numericArr"],
-        "zarrSubSize": [kwargs.get("zarrSubSize", [20,20,20]), "numericArr"],
-        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
-        "taskSize": [kwargs.get("taskSize", []), "numericScalar"],
-        "resample": [kwargs.get("resample", []), "numericArr"],
-        "Interp": [kwargs.get("Interp", "linear"), "char"],
-        "maskFns": [kwargs.get("maskFns", []), "cell"],
-        "suffix": [kwargs.get("suffix", ""), "char"],
+        "dampFactor": [kwargs.get("dampFactor", 1), "numericScalar"],
+        "scaleFactor": [kwargs.get("scaleFactor", []), "numericScalar"],
+        "deconOffset": [kwargs.get("deconOffset", 0), "numericScalar"],
+        "deconMaskFns": [kwargs.get("deconMaskFns", []), "cell"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "parseParfor": [kwargs.get("parseParfor", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
-        "debug": [kwargs.get("debug", False), "logical"],
+        "unitWaitTime": [kwargs.get("unitWaitTime", 1), "numericScalar"],
+        "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"],
+        "GPUConfigFile": [kwargs.get("GPUConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
     
-    for key, value in XR_deskew_rotate_data_wrapper_dict.items():
+    for key, value in XR_decon_data_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
 import subprocess
 
 
 def XR_fftSpectrumComputingWrapper(dataPaths, **kwargs):
     function_name = "XR_fftSpectrumComputingWrapper"
     XR_fftSpectrumComputingWrapper_dict = {
-        "Overwrite": [kwargs.get("Overwrite", False), "logical"],
+        "resultDirName": [kwargs.get("resultDirName", "FFT"), "char"],
+        "overwrite": [kwargs.get("overwrite", False), "logical"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "dz": [kwargs.get("dz", 0.1), "numericScalar"],
+        "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "outPixelSize": [kwargs.get("outPixelSize", []), "numericScalar"],
-        "N": [kwargs.get("N", [1001,1001,1001]), "numericArr"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", []), "cell"],
+        "outSize": [kwargs.get("outSize", [1001,1001,1001]), "numericArr"],
+        "channelPatterns": [kwargs.get("channelPatterns", []), "cell"],
         "save3DStack": [kwargs.get("save3DStack", False), "logical"],
         "background": [kwargs.get("background", 0), "numericScalar"],
-        "Interp": [kwargs.get("Interp", "linear"), "char"],
+        "interpMethod": [kwargs.get("interpMethod", "linear"), "char"],
+        "parseCluster": [kwargs.get("parseCluster", False), "logical"],
+        "masterCompute": [kwargs.get("masterCompute", True), "logical"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 3), "numericScalar"],
+        "debug": [kwargs.get("debug", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,67 @@
 import os
 import subprocess
 
 
-def XR_matlab_stitching_wrapper(dataPath, imageListFileName, **kwargs):
-    function_name = "XR_matlab_stitching_wrapper"
-    XR_matlab_stitching_wrapper_dict = {
-        "Streaming": [kwargs.get("Streaming", False), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
-        "multiLoc": [kwargs.get("multiLoc", False), "logical"],
-        "ProcessedDirStr": [kwargs.get("ProcessedDirStr", ""), "char"],
-        "stitchInfoFullpath": [kwargs.get("stitchInfoFullpath", ""), "char"],
-        "DS": [kwargs.get("DS", False), "logical"],
-        "DSR": [kwargs.get("DSR", False), "logical"],
-        "SkewAngle": [kwargs.get("SkewAngle", 32.45), "numericScalar"],
-        "Reverse": [kwargs.get("Reverse", False), "logical"],
+def XR_deskew_rotate_data_wrapper(dataPaths, **kwargs):
+    function_name = "XR_deskew_rotate_data_wrapper"
+    XR_deskew_rotate_data_wrapper_dict = {
+        "DSDirName": [kwargs.get("DSDirName", "DS"), "char"],
+        "DSRDirName": [kwargs.get("DSRDirName", "DSR"), "char"],
+        "deskew": [kwargs.get("deskew", True), "logical"],
+        "rotate": [kwargs.get("rotate", True), "logical"],
+        "overwrite": [kwargs.get("overwrite", False), "logical"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
+        "dz": [kwargs.get("dz", 0.5), "numericScalar"],
+        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericArr"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
+        "objectiveScan": [kwargs.get("objectiveScan", False), "logical"],
+        "zStageScan": [kwargs.get("zStageScan", False), "logical"],
+        "reverse": [kwargs.get("reverse", False), "logical"],
+        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
         "parseSettingFile": [kwargs.get("parseSettingFile", False), "logical"],
-        "axisOrder": [kwargs.get("axisOrder", "x,y,z"), "char"],
-        "dataOrder": [kwargs.get("dataOrder", "y,x,z"), "char"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "IOScan": [kwargs.get("IOScan", False), "logical"],
-        "zarrFile": [kwargs.get("zarrFile", False), "logical"],
-        "largeZarr": [kwargs.get("largeZarr", False), "logical"],
-        "poolSize": [kwargs.get("poolSize", []), "numericScalar"],
-        "batchSize": [kwargs.get("batchSize", [500,500,500]), "numericArr"],
-        "blockSize": [kwargs.get("blockSize", [500,500,500]), "numericArr"],
-        "shardSize": [kwargs.get("shardSize", []), "numericArr"],
-        "resampleType": [kwargs.get("resampleType", "xy_isotropic"), "char"],
-        "resample": [kwargs.get("resample", []), "numericArr"],
-        "InputBbox": [kwargs.get("InputBbox", []), "numericArr"],
-        "tileOutBbox": [kwargs.get("tileOutBbox", []), "numericArr"],
-        "TileOffset": [kwargs.get("TileOffset", 0), "numericScalar"],
-        "Resolution": [kwargs.get("Resolution", [0.108,0.5]), "numericArr"],
-        "resultDir": [kwargs.get("resultDir", "matlab_stitch"), "char"],
-        "BlendMethod": [kwargs.get("BlendMethod", "none"), "char"],
-        "overlapType": [kwargs.get("overlapType", ""), "char"],
-        "xcorrShift": [kwargs.get("xcorrShift", True), "logical"],
-        "xyMaxOffset": [kwargs.get("xyMaxOffset", 300), "numericScalar"],
-        "zMaxOffset": [kwargs.get("zMaxOffset", 50), "numericScalar"],
-        "xcorrDownsample": [kwargs.get("xcorrDownsample", [2,2,1]), "numericArr"],
-        "xcorrThresh": [kwargs.get("xcorrThresh", 0.25), "numericScalar"],
-        "padSize": [kwargs.get("padSize", []), "numericArr"],
-        "boundboxCrop": [kwargs.get("boundboxCrop", []), "numericArr"],
-        "zNormalize": [kwargs.get("zNormalize", False), "logical"],
-        "onlyFirstTP": [kwargs.get("onlyFirstTP", False), "logical"],
-        "timepoints": [kwargs.get("timepoints", []), "numericArr"],
-        "subtimepoints": [kwargs.get("subtimepoints", []), "numericArr"],
-        "xcorrMode": [kwargs.get("xcorrMode", "primaryFirst"), "char"],
-        "shiftMethod": [kwargs.get("shiftMethod", "grid"), "char"],
-        "axisWeight": [kwargs.get("axisWeight", [1,0.1,10]), "numericArr"],
-        "groupFile": [kwargs.get("groupFile", ""), "char"],
-        "primaryCh": [kwargs.get("primaryCh", ""), "char"],
-        "usePrimaryCoords": [kwargs.get("usePrimaryCoords", False), "logical"],
-        "Save16bit": [kwargs.get("Save16bit", False), "logical"],
-        "EdgeArtifacts": [kwargs.get("EdgeArtifacts", 0), "numericScalar"],
-        "distBboxes": [kwargs.get("distBboxes", []), "numericArr"],
+        "crop": [kwargs.get("crop", False), "logical"],
+        "DSRCombined": [kwargs.get("DSRCombined", True), "logical"],
+        "FFCorrection": [kwargs.get("FFCorrection", False), "logical"],
+        "BKRemoval": [kwargs.get("BKRemoval", False), "logical"],
+        "lowerLimit": [kwargs.get("lowerLimit", 0.4), "numericScalar"],
+        "constOffset": [kwargs.get("constOffset", []), "numericScalar"],
+        "FFImagePaths": [kwargs.get("FFImagePaths", ['','','']), "cell"],
+        "backgroundPaths": [kwargs.get("backgroundPaths", ['','','']), "cell"],
+        "save16bit": [kwargs.get("save16bit", False), "logical"],
+        "save3DStack": [kwargs.get("save3DStack", True), "logical"],
         "saveMIP": [kwargs.get("saveMIP", True), "logical"],
-        "stitchMIP": [kwargs.get("stitchMIP", []), "logicalArr"],
-        "onlineStitch": [kwargs.get("onlineStitch", False), "logical"],
-        "bigStitchData": [kwargs.get("bigStitchData", False), "logical"],
-        "pipeline": [kwargs.get("pipeline", "zarr"), "char"],
-        "processFunPath": [kwargs.get("processFunPath", ), "cell"],
+        "largeFile": [kwargs.get("largeFile", False), "logical"],
+        "zarrFile": [kwargs.get("zarrFile", False), "logical"],
+        "saveZarr": [kwargs.get("saveZarr", False), "logical"],
+        "batchSize": [kwargs.get("batchSize", [1024,1024,1024]), "numericArr"],
+        "blockSize": [kwargs.get("blockSize", [256,256,256]), "numericArr"],
+        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
+        "taskSize": [kwargs.get("taskSize", []), "numericScalar"],
+        "resampleFactor": [kwargs.get("resampleFactor", []), "numericArr"],
+        "interpMethod": [kwargs.get("interpMethod", "linear"), "char"],
+        "maskFns": [kwargs.get("maskFns", []), "cell"],
+        "suffix": [kwargs.get("suffix", ""), "char"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
+        "parseParfor": [kwargs.get("parseParfor", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 8), "numericScalar"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
-        "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
-        "unitWaitTime": [kwargs.get("unitWaitTime", 0.1), "numericScalar"],
+        "debug": [kwargs.get("debug", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
-    dataPathString = "{" + ",".join(f"'{item}'" for item in dataPath) + "}"
-    imageListFileNameString = "{" + ",".join(f"'{item}'" for item in imageListFileName) + "}"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathString}\" \"{imageListFileNameString}\" "
+    dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
     
-    for key, value in XR_matlab_stitching_wrapper_dict.items():
+    for key, value in XR_deskew_rotate_data_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,71 @@
 import os
 import subprocess
 
 
 def XR_microscopeAutomaticProcessing(dataPaths, **kwargs):
     function_name = "XR_microscopeAutomaticProcessing"
     XR_microscopeAutomaticProcessing_dict = {
-        "Overwrite": [kwargs.get("Overwrite", False), "logical"],
-        "Streaming": [kwargs.get("Streaming", True), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
-        "Channels": [kwargs.get("Channels", [488,560,642]), "numericArr"],
-        "SkewAngle": [kwargs.get("SkewAngle", 32.45), "numericScalar"],
+        "overwrite": [kwargs.get("overwrite", False), "logical"],
+        "streaming": [kwargs.get("streaming", True), "logical"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0']), "cell"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
         "dz": [kwargs.get("dz", 0.5), "numericScalar"],
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
-        "Reverse": [kwargs.get("Reverse", True), "logical"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "ZstageScan": [kwargs.get("ZstageScan", False), "logical"],
-        "sCMOSCameraFlip": [kwargs.get("sCMOSCameraFlip", False), "logical"],
-        "Save16bit": [kwargs.get("Save16bit", [False,False,False,False]), "logicalArr"],
+        "reverse": [kwargs.get("reverse", True), "logical"],
+        "objectiveScan": [kwargs.get("objectiveScan", False), "logical"],
+        "zStageScan": [kwargs.get("zStageScan", False), "logical"],
+        "save16bit": [kwargs.get("save16bit", [False,False,False,False]), "logicalArr"],
         "onlyFirstTP": [kwargs.get("onlyFirstTP", False), "logical"],
         "dzFromEncoder": [kwargs.get("dzFromEncoder", False), "logical"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
         "saveZarr": [kwargs.get("saveZarr", False), "logical"],
         "save3DStack": [kwargs.get("save3DStack", True), "logical"],
-        "Deskew": [kwargs.get("Deskew", True), "logical"],
-        "Rotate": [kwargs.get("Rotate", True), "logical"],
-        "Stitch": [kwargs.get("Stitch", False), "logical"],
-        "Decon": [kwargs.get("Decon", True), "logical"],
-        "RotateAfterDecon": [kwargs.get("RotateAfterDecon", False), "logical"],
+        "deskew": [kwargs.get("deskew", True), "logical"],
+        "rotate": [kwargs.get("rotate", True), "logical"],
+        "stitch": [kwargs.get("stitch", False), "logical"],
         "parseSettingFile": [kwargs.get("parseSettingFile", False), "logical"],
         "flipZstack": [kwargs.get("flipZstack", False), "logical"],
         "DSRCombined": [kwargs.get("DSRCombined", True), "logical"],
-        "LLFFCorrection": [kwargs.get("LLFFCorrection", False), "logical"],
+        "FFCorrection": [kwargs.get("FFCorrection", False), "logical"],
         "BKRemoval": [kwargs.get("BKRemoval", False), "logical"],
-        "LowerLimit": [kwargs.get("LowerLimit", 0.4), "numericScalar"],
+        "lowerLimit": [kwargs.get("lowerLimit", 0.4), "numericScalar"],
         "constOffset": [kwargs.get("constOffset", []), "numericScalar"],
-        "LSImagePaths": [kwargs.get("LSImagePaths", ['','','']), "cell"],
-        "BackgroundPaths": [kwargs.get("BackgroundPaths", ['','','']), "cell"],
+        "FFImagePaths": [kwargs.get("FFImagePaths", ['','','']), "cell"],
+        "backgroundPaths": [kwargs.get("backgroundPaths", ['','','']), "cell"],
         "resampleType": [kwargs.get("resampleType", "isotropic"), "char"],
-        "resample": [kwargs.get("resample", []), "numericArr"],
-        "InputBbox": [kwargs.get("InputBbox", []), "numericArr"],
+        "resampleFactor": [kwargs.get("resampleFactor", []), "numericArr"],
+        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
         "stitchPipeline": [kwargs.get("stitchPipeline", "zarr"), "char"],
-        "stitchResultDir": [kwargs.get("stitchResultDir", ""), "char"],
-        "imageListFullpaths": [kwargs.get("imageListFullpaths", ), "cell"],
+        "stitchResultDirName": [kwargs.get("stitchResultDirName", ""), "char"],
+        "imageListFullpaths": [kwargs.get("imageListFullpaths", ""), "cell"],
         "axisOrder": [kwargs.get("axisOrder", "xyz"), "char"],
-        "BlendMethod": [kwargs.get("BlendMethod", "none"), "char"],
+        "blendMethod": [kwargs.get("blendMethod", "none"), "char"],
         "xcorrShift": [kwargs.get("xcorrShift", False), "logical"],
         "xcorrMode": [kwargs.get("xcorrMode", "primaryFirst"), "char"],
         "xyMaxOffset": [kwargs.get("xyMaxOffset", 300), "numericScalar"],
         "zMaxOffset": [kwargs.get("zMaxOffset", 50), "numericScalar"],
-        "EdgeArtifacts": [kwargs.get("EdgeArtifacts", 2), "numericScalar"],
-        "timepoints": [kwargs.get("timepoints", []), "numericArr"],
-        "boundboxCrop": [kwargs.get("boundboxCrop", []), "numericArr"],
+        "edgeArtifacts": [kwargs.get("edgeArtifacts", 2), "numericScalar"],
         "primaryCh": [kwargs.get("primaryCh", ""), "char"],
         "stitchMIP": [kwargs.get("stitchMIP", []), "logicalArr"],
         "onlineStitch": [kwargs.get("onlineStitch", False), "logical"],
         "generateImageList": [kwargs.get("generateImageList", ""), "char"],
-        "cudaDecon": [kwargs.get("cudaDecon", False), "logical"],
-        "cppDecon": [kwargs.get("cppDecon", False), "logical"],
-        "cppDeconPath": [kwargs.get("cppDeconPath", "/global/home/groups/software/sl-7.x86_64/modules/RLDecon_CPU/20200718/build-cluster/cpuDeconv"), "char"],
-        "loadModules": [kwargs.get("loadModules", "moduleloadgcc/4.8.5;moduleloadfftw/3.3.6-gcc;moduleloadboost/1.65.1-gcc;moduleloadlibtiff/4.1.0;"), "char"],
-        "cudaDeconPath": [kwargs.get("cudaDeconPath", "/global/home/groups/software/sl-7.x86_64/modules/cudaDecon/bin/cudaDeconv"), "char"],
-        "OTFGENPath": [kwargs.get("OTFGENPath", "/global/home/groups/software/sl-7.x86_64/modules/cudaDecon/bin/radialft"), "char"],
-        "DS": [kwargs.get("DS", False), "logical"],
-        "DSR": [kwargs.get("DSR", False), "logical"],
-        "Background": [kwargs.get("Background", []), "numericScalar"],
-        "dzPSF": [kwargs.get("dzPSF", 0.1), "numericScalar"],
-        "EdgeErosion": [kwargs.get("EdgeErosion", 8), "numericScalar"],
-        "ErodeByFTP": [kwargs.get("ErodeByFTP", True), "logical"],
-        "deconRotate": [kwargs.get("deconRotate", False), "logical"],
-        "psfFullpaths": [kwargs.get("psfFullpaths", ['','','']), "cell"],
-        "DeconIter": [kwargs.get("DeconIter", 15), "numericScalar"],
-        "rotatedPSF": [kwargs.get("rotatedPSF", False), "logical"],
-        "RLMethod": [kwargs.get("RLMethod", "simplified"), "char"],
-        "fixIter": [kwargs.get("fixIter", False), "logical"],
-        "errThresh": [kwargs.get("errThresh", []), "numericScalar"],
-        "debug": [kwargs.get("debug", False), "logical"],
-        "GPUJob": [kwargs.get("GPUJob", False), "logical"],
         "largeFile": [kwargs.get("largeFile", False), "logical"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
+        "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
         "unitWaitTime": [kwargs.get("unitWaitTime", 1), "numericScalar"],
         "minModifyTime": [kwargs.get("minModifyTime", 1), "numericScalar"],
         "maxModifyTime": [kwargs.get("maxModifyTime", 10), "numericScalar"],
         "maxWaitLoopNum": [kwargs.get("maxWaitLoopNum", 10), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"],
+        "configFile": [kwargs.get("configFile", ""), "char"],
         "GPUConfigFile": [kwargs.get("GPUConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import os
 import subprocess
 
 
-def XR_psf_analysis_wrapper(dataPaths, **kwargs):
-    function_name = "XR_psf_analysis_wrapper"
-    XR_psf_analysis_wrapper_dict = {
-        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
-        "dz": [kwargs.get("dz", 0.1), "numericScalar"],
-        "angle": [kwargs.get("angle", 32.45), "numericScalar"],
-        "Deskew": [kwargs.get("Deskew", True), "logical"],
-        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
-        "ObjectiveScan": [kwargs.get("ObjectiveScan", False), "logical"],
-        "ZstageScan": [kwargs.get("ZstageScan", False), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
-        "Channels": [kwargs.get("Channels", [488,560]), "numericArr"],
-        "Save16bit": [kwargs.get("Save16bit", True), "logical"],
-        "bgFactor": [kwargs.get("bgFactor", 1.5), "numericScalar"],
-        "RWFn": [kwargs.get("RWFn", ['/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_515em_128_128_101_100nmSteps.tif','/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_605em_128_128_101_100nmSteps.tif']), "cell"],
-        "sourceStr": [kwargs.get("sourceStr", "test"), "char"],
+def XR_resample_dataset(dataPaths, resampleFactor, **kwargs):
+    function_name = "XR_resample_dataset"
+    XR_resample_dataset_dict = {
+        "resultDirName": [kwargs.get("resultDirName", "resampled"), "char"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
+        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
+        "interpMethod": [kwargs.get("interpMethod", "linear"), "char"],
+        "save16bit": [kwargs.get("save16bit", True), "logical"],
+        "zarrFile": [kwargs.get("zarrFile", False), "logical"],
+        "largeZarr": [kwargs.get("largeZarr", False), "logical"],
+        "saveZarr": [kwargs.get("saveZarr", False), "logical"],
+        "blockSize": [kwargs.get("blockSize", [256,256,256]), "numericArr"],
+        "batchSize": [kwargs.get("batchSize", [512,512,512]), "numericArr"],
+        "borderSize": [kwargs.get("borderSize", [5,5,5]), "numericArr"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
-        "masterCompute": [kwargs.get("masterCompute", False), "logical"],
+        "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
+        "masterCompute": [kwargs.get("masterCompute", True), "logical"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
+        "uuid": [kwargs.get("uuid", ""), "char"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
-    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
+    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
+    resampleFactorString = "[" + ",".join(str(item) for item in resampleFactor) + "]"
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" \"{resampleFactorString}\" "
     
-    for key, value in XR_psf_analysis_wrapper_dict.items():
+    for key, value in XR_resample_dataset_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     XR_psf_detection_and_analysis_wrapper_dict = {
         "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
         "dz": [kwargs.get("dz", 0.1), "numericScalar"],
         "angle": [kwargs.get("angle", 32.45), "numericScalar"],
         "cropSize": [kwargs.get("cropSize", [256,128,201]), "numericArr"],
         "flipZstack": [kwargs.get("flipZstack", False), "logical"],
         "distThresh": [kwargs.get("distThresh", [256,128,201]), "numericArr"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
-        "Channels": [kwargs.get("Channels", [488,560]), "numericArr"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
+        "channels": [kwargs.get("channels", [488,560]), "numericArr"],
         "RWFn": [kwargs.get("RWFn", ['/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_515em_128_128_101_100nmSteps.tif','/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_605em_128_128_101_100nmSteps.tif']), "cell"],
         "sourceStr": [kwargs.get("sourceStr", "test"), "char"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "masterCompute": [kwargs.get("masterCompute", False), "logical"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_resample_dataset.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import os
 import subprocess
 
 
-def XR_resample_dataset(dataPaths, rsfactor, **kwargs):
-    function_name = "XR_resample_dataset"
-    XR_resample_dataset_dict = {
-        "outDirStr": [kwargs.get("outDirStr", "resampled"), "char"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
-        "bbox": [kwargs.get("bbox", []), "numericScalar"],
-        "Interp": [kwargs.get("Interp", "linear"), "char"],
-        "Save16bit": [kwargs.get("Save16bit", True), "logical"],
-        "zarrFile": [kwargs.get("zarrFile", False), "logical"],
-        "largeZarr": [kwargs.get("largeZarr", False), "logical"],
-        "saveZarr": [kwargs.get("saveZarr", False), "logical"],
-        "blockSize": [kwargs.get("blockSize", [256,256,256]), "numericArr"],
-        "batchSize": [kwargs.get("batchSize", [512,512,512]), "numericArr"],
-        "BorderSize": [kwargs.get("BorderSize", [5,5,5]), "numericArr"],
+def XR_psf_analysis_wrapper(dataPaths, **kwargs):
+    function_name = "XR_psf_analysis_wrapper"
+    XR_psf_analysis_wrapper_dict = {
+        "xyPixelSize": [kwargs.get("xyPixelSize", 0.108), "numericScalar"],
+        "dz": [kwargs.get("dz", 0.1), "numericScalar"],
+        "skewAngle": [kwargs.get("skewAngle", 32.45), "numericScalar"],
+        "deskew": [kwargs.get("deskew", True), "logical"],
+        "flipZstack": [kwargs.get("flipZstack", False), "logical"],
+        "objectiveScan": [kwargs.get("objectiveScan", False), "logical"],
+        "zStageScan": [kwargs.get("zStageScan", False), "logical"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['CamA_ch0','CamB_ch0']), "cell"],
+        "channels": [kwargs.get("channels", [488,560]), "numericArr"],
+        "save16bit": [kwargs.get("save16bit", True), "logical"],
+        "bgFactor": [kwargs.get("bgFactor", 1.5), "numericScalar"],
+        "RWFn": [kwargs.get("RWFn", ['/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_515em_128_128_101_100nmSteps.tif','/clusterfs/fiona/Gokul/RW_PSFs/PSF_RW_605em_128_128_101_100nmSteps.tif']), "cell"],
+        "sourceStr": [kwargs.get("sourceStr", "test"), "char"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
-        "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
-        "masterCompute": [kwargs.get("masterCompute", True), "logical"],
-        "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
-        "uuid": [kwargs.get("uuid", ""), "char"],
+        "masterCompute": [kwargs.get("masterCompute", False), "logical"],
+        "cpusPerTask": [kwargs.get("cpusPerTask", 8), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
-    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
+    mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux_with_jvm/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
     dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
-    rsfactorString = "[" + ",".join(str(item) for item in rsfactor) + "]"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" \"{rsfactorString}\" "
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
     
-    for key, value in XR_resample_dataset_dict.items():
+    for key, value in XR_psf_analysis_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
             if not value[0]:
                 continue
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import os
 import subprocess
 
 
-def XR_tiffToZarr_wrapper(tiffFullpaths, **kwargs):
+def XR_tiffToZarr_wrapper(dataPaths, **kwargs):
     function_name = "XR_tiffToZarr_wrapper"
     XR_tiffToZarr_wrapper_dict = {
-        "zarrPathstr": [kwargs.get("zarrPathstr", "zarr"), "char"],
+        "tiffFullpaths": [kwargs.get("tiffFullpaths", ""), "cell"],
+        "resultDirName": [kwargs.get("resultDirName", "zarr"), "char"],
         "locIds": [kwargs.get("locIds", []), "numericScalar"],
         "blockSize": [kwargs.get("blockSize", [500,500,250]), "numericArr"],
         "shardSize": [kwargs.get("shardSize", []), "numericArr"],
         "flippedTile": [kwargs.get("flippedTile", []), "logical"],
-        "resample": [kwargs.get("resample", []), "numericArr"],
+        "resampleFactor": [kwargs.get("resampleFactor", []), "numericArr"],
         "partialFile": [kwargs.get("partialFile", False), "logical"],
-        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['tif']), "cell"],
-        "InputBbox": [kwargs.get("InputBbox", []), "numericArr"],
+        "channelPatterns": [kwargs.get("channelPatterns", ['tif']), "cell"],
+        "inputBbox": [kwargs.get("inputBbox", []), "numericArr"],
         "tileOutBbox": [kwargs.get("tileOutBbox", []), "numericArr"],
-        "processFunPath": [kwargs.get("processFunPath", ), "cell"],
+        "processFunPath": [kwargs.get("processFunPath", ""), "cell"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "bigData": [kwargs.get("bigData", True), "logical"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 1), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "maxTrialNum": [kwargs.get("maxTrialNum", 3), "numericScalar"],
-        "unitWaitTime": [kwargs.get("unitWaitTime", 30), "numericScalar"],
+        "unitWaitTime": [kwargs.get("unitWaitTime", 3), "numericScalar"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
-        "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
+        "configFile": [kwargs.get("configFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
-    tiffFullpathsString = "{" + ",".join(f"'{item}'" for item in tiffFullpaths) + "}"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{tiffFullpathsString}\" "
+    dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" "
     
     for key, value in XR_tiffToZarr_wrapper_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/__init__.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/generatePythonWrapper.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 varTypes[i] = "numericScalar"
         elif "@(x)isempty(x)||ischar(x)" in param:
             varTypes[i] = "char"
         else:
             varTypes[i] = "err"
         if i < numRequired:
             continue
-        if varTypes[i] == "char":
+        if varTypes[i] == "char" or not extracted_string:
             extracted_string = f"\"{extracted_string}\""
         if firstString == "parseCluster":
             extracted_string = "False"
         functionString = functionString + f"\"{firstString}\": [kwargs.get(\"{firstString}\", {extracted_string}), \"{varTypes[i]}\"],\n        "
     if len(input_parser_params) > numRequired:
         functionString = functionString[:-10] + "\n    }\n\n    "
     else:
```

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools/generate_config_file.py` & `pyllsm5dtools-1.1.0/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/PyLLSM5DTools.egg-info/SOURCES.txt` & `pyllsm5dtools-1.1.0/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/README.md` & `pyllsm5dtools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyllsm5dtools-1.0.5/setup.py` & `pyllsm5dtools-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.0.5'
+version = '1.1.0'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

