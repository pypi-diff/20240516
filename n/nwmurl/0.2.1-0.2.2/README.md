# Comparing `tmp/nwmurl-0.2.1.tar.gz` & `tmp/nwmurl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwmurl-0.2.1.tar", last modified: Tue Nov 14 21:48:11 2023, max compression
+gzip compressed data, was "nwmurl-0.2.2.tar", last modified: Thu Dec  7 21:44:13 2023, max compression
```

## Comparing `nwmurl-0.2.1.tar` & `nwmurl-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:48:11.538400 nwmurl-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-11-14 21:48:03.000000 nwmurl-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-11-14 21:48:11.538400 nwmurl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2023-11-14 21:48:03.000000 nwmurl-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:48:11.522400 nwmurl-0.2.1/nwmurl/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-14 21:48:03.000000 nwmurl-0.2.1/nwmurl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2023-11-14 21:48:03.000000 nwmurl-0.2.1/nwmurl/urlgennwm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:48:11.526399 nwmurl-0.2.1/nwmurl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-11-14 21:48:11.000000 nwmurl-0.2.1/nwmurl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-11-14 21:48:11.000000 nwmurl-0.2.1/nwmurl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 21:48:11.000000 nwmurl-0.2.1/nwmurl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 21:48:11.000000 nwmurl-0.2.1/nwmurl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 21:48:11.538400 nwmurl-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-14 21:48:03.000000 nwmurl-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:48:11.538400 nwmurl-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimExtend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimExtendNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimHawaii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimHawaiiNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimPuertorico.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_analysisAssimPuertoricoNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingAnalysisAssim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingAnalysisAssimExtend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingAnalysisAssimHawaii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingAnalysisAssimPuertorico.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingMediumRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingShortRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingShortRangeAssimHawaii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_forcingShortRangeAssimPuertorico.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_longRangeMem1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_longRangeMem2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_longRangeMem3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_longRangeMem4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMem6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeMemNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_mediumRangeNoDa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_shortRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_shortRangeAssimHawaii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_shortRangeAssimPuertorico.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-11-14 21:48:03.000000 nwmurl-0.2.1/test/test_shortRangeAssimPuertoricoNoDa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:44:13.618546 nwmurl-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-07 21:44:08.000000 nwmurl-0.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-07 21:44:13.618546 nwmurl-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2023-12-07 21:44:08.000000 nwmurl-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:44:13.610546 nwmurl-0.2.2/nwmurl/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-07 21:44:08.000000 nwmurl-0.2.2/nwmurl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18759 2023-12-07 21:44:08.000000 nwmurl-0.2.2/nwmurl/urlgennwm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:44:13.618546 nwmurl-0.2.2/nwmurl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-07 21:44:13.000000 nwmurl-0.2.2/nwmurl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2023-12-07 21:44:13.000000 nwmurl-0.2.2/nwmurl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:44:13.000000 nwmurl-0.2.2/nwmurl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-07 21:44:13.000000 nwmurl-0.2.2/nwmurl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 21:44:13.618546 nwmurl-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-07 21:44:08.000000 nwmurl-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:44:13.618546 nwmurl-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimExtend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimExtendNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimHawaii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimHawaiiNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimPuertorico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_analysisAssimPuertoricoNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingAnalysisAssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingAnalysisAssimExtend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingAnalysisAssimHawaii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingAnalysisAssimPuertorico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingMediumRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingShortRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingShortRangeAssimHawaii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_forcingShortRangeAssimPuertorico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_longRangeMem1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_longRangeMem2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_longRangeMem3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_longRangeMem4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMem6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeMemNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_mediumRangeNoDa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_shortRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_shortRangeAssimHawaii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_shortRangeAssimPuertorico.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-12-07 21:44:08.000000 nwmurl-0.2.2/test/test_shortRangeAssimPuertoricoNoDa.py
```

### Comparing `nwmurl-0.2.1/LICENSE.txt` & `nwmurl-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/PKG-INFO` & `nwmurl-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwmurl
-Version: 0.2.1
+Version: 0.2.2
 Summary: URL generator tool for National Water Model data
 Author: Sepehr Karimi (CIROH)
 Author-email: mkarimiziarani@ua.edu
 Keywords: python,NWM,url
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nwmurl-0.2.1/README.md` & `nwmurl-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ## Customize Your Data Retrieval for Retrospective Dataset
 - `start_date`: A string representing the starting date in the format \"YYYYMMDDHHMM".
 - `end_date`: A string representing the ending date in the same format.
 - `urlbaseinput `:  An integer representing the NWM dataset. Available options include:
 	- `1`: "https://noaa-nwm-retrospective-2-1-pds.s3.amazonaws.com/".
     - `2`: "s3://noaa-nwm-retrospective-2-1-pds/model_output/".
     - `3`: "https://ciroh-nwm-zarr-retrospective-data-copy.s3.amazonaws.com/noaa-nwm-retrospective-2-1-zarr-pds/".
+    - `4`: "https://noaa-nwm-retrospective-3-0-pds.s3.amazonaws.com/CONUS/netcdf/".
 - `selectet_object_type`: An integer representing the object type. Available options include:
 	- `1` for forcing data
 	- `2` for model_output
  
 - `Selectet_var_types`:  An integer or string representing the variable of interest within the NWM data. Available options include:
 	- `1`: ".CHRTOUT_DOMAIN1.comp"
     - `2`: ".GWOUT_DOMAIN1.comp"
```

### Comparing `nwmurl-0.2.1/nwmurl/urlgennwm.py` & `nwmurl-0.2.2/nwmurl/urlgennwm.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 
 objecttypes = {1: "forcing/", 2: "model_output/"}
 
 urlbasedict_retro = {
     1: "https://noaa-nwm-retrospective-2-1-pds.s3.amazonaws.com/",
     2: "s3://noaa-nwm-retrospective-2-1-pds/",
     3: "https://ciroh-nwm-zarr-retrospective-data-copy.s3.amazonaws.com/noaa-nwm-retrospective-2-1-zarr-pds/",
+    4: "https://noaa-nwm-retrospective-3-0-pds.s3.amazonaws.com/CONUS/netcdf/",
 }
 
 
 def selecturlbase(urlbasedict, urlbaseinput, defaulturlbase=""):
     if urlbaseinput in urlbasedict:
         return urlbasedict[urlbaseinput]
     else:
```

### Comparing `nwmurl-0.2.1/nwmurl.egg-info/PKG-INFO` & `nwmurl-0.2.2/nwmurl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwmurl
-Version: 0.2.1
+Version: 0.2.2
 Summary: URL generator tool for National Water Model data
 Author: Sepehr Karimi (CIROH)
 Author-email: mkarimiziarani@ua.edu
 Keywords: python,NWM,url
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nwmurl-0.2.1/nwmurl.egg-info/SOURCES.txt` & `nwmurl-0.2.2/nwmurl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/setup.py` & `nwmurl-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from nwmurl import generate_url
 
     url = generate_url(model="short_range", comid=12345, datetime="2023-10-29T12:00:00Z")
 
 """
 
 # Other information
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 DESCRIPTION = "URL generator tool for National Water Model data"
 
 setup(
     name="nwmurl",
     version=VERSION,
     author="Sepehr Karimi (CIROH)",
     author_email="mkarimiziarani@ua.edu",
```

### Comparing `nwmurl-0.2.1/test/test_analysisAssim.py` & `nwmurl-0.2.2/test/test_analysisAssim.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimExtend.py` & `nwmurl-0.2.2/test/test_analysisAssimExtend.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimExtendNoDa.py` & `nwmurl-0.2.2/test/test_analysisAssimExtendNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimHawaii.py` & `nwmurl-0.2.2/test/test_analysisAssimHawaii.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimHawaiiNoDa.py` & `nwmurl-0.2.2/test/test_analysisAssimHawaiiNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimNoDa.py` & `nwmurl-0.2.2/test/test_analysisAssimNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimPuertorico.py` & `nwmurl-0.2.2/test/test_analysisAssimPuertorico.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_analysisAssimPuertoricoNoDa.py` & `nwmurl-0.2.2/test/test_analysisAssimPuertoricoNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_cases.py` & `nwmurl-0.2.2/test/test_cases.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingAnalysisAssim.py` & `nwmurl-0.2.2/test/test_forcingAnalysisAssim.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingAnalysisAssimExtend.py` & `nwmurl-0.2.2/test/test_forcingAnalysisAssimExtend.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingAnalysisAssimHawaii.py` & `nwmurl-0.2.2/test/test_forcingAnalysisAssimHawaii.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingAnalysisAssimPuertorico.py` & `nwmurl-0.2.2/test/test_forcingAnalysisAssimPuertorico.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingMediumRange.py` & `nwmurl-0.2.2/test/test_forcingMediumRange.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingShortRange.py` & `nwmurl-0.2.2/test/test_forcingShortRange.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingShortRangeAssimHawaii.py` & `nwmurl-0.2.2/test/test_forcingShortRangeAssimHawaii.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_forcingShortRangeAssimPuertorico.py` & `nwmurl-0.2.2/test/test_forcingShortRangeAssimPuertorico.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_longRangeMem1.py` & `nwmurl-0.2.2/test/test_longRangeMem1.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_longRangeMem2.py` & `nwmurl-0.2.2/test/test_longRangeMem2.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_longRangeMem3.py` & `nwmurl-0.2.2/test/test_longRangeMem3.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_longRangeMem4.py` & `nwmurl-0.2.2/test/test_longRangeMem4.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem1.py` & `nwmurl-0.2.2/test/test_mediumRangeMem1.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem2.py` & `nwmurl-0.2.2/test/test_mediumRangeMem2.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem3.py` & `nwmurl-0.2.2/test/test_mediumRangeMem3.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem4.py` & `nwmurl-0.2.2/test/test_mediumRangeMem4.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem5.py` & `nwmurl-0.2.2/test/test_mediumRangeMem5.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMem6.py` & `nwmurl-0.2.2/test/test_mediumRangeMem6.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeMemNoDa.py` & `nwmurl-0.2.2/test/test_mediumRangeMemNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_mediumRangeNoDa.py` & `nwmurl-0.2.2/test/test_mediumRangeNoDa.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_shortRange.py` & `nwmurl-0.2.2/test/test_shortRange.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_shortRangeAssimHawaii.py` & `nwmurl-0.2.2/test/test_shortRangeAssimHawaii.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_shortRangeAssimPuertorico.py` & `nwmurl-0.2.2/test/test_shortRangeAssimPuertorico.py`

 * *Files identical despite different names*

### Comparing `nwmurl-0.2.1/test/test_shortRangeAssimPuertoricoNoDa.py` & `nwmurl-0.2.2/test/test_shortRangeAssimPuertoricoNoDa.py`

 * *Files identical despite different names*

