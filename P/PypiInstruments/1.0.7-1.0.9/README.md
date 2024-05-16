# Comparing `tmp/PypiInstruments-1.0.7.tar.gz` & `tmp/PypiInstruments-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PypiInstruments-1.0.7.tar", last modified: Mon May 13 03:22:55 2024, max compression
+gzip compressed data, was "PypiInstruments-1.0.9.tar", last modified: Mon May 13 03:36:07 2024, max compression
```

## Comparing `PypiInstruments-1.0.7.tar` & `PypiInstruments-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.816334 PypiInstruments-1.0.7/
--rw-rw-rw-   0        0        0       83 2024-05-13 03:22:55.815330 PypiInstruments-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.711899 PypiInstruments-1.0.7/PypiInstruments.egg-info/
--rw-rw-rw-   0        0        0       83 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2024-05-13 03:22:55.000000 PypiInstruments-1.0.7/PypiInstruments.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.795984 PypiInstruments-1.0.7/instruments/
--rw-rw-rw-   0        0        0     2120 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/DP821A.py
--rw-rw-rw-   0        0        0     3815 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/Multimemter.py
--rw-rw-rw-   0        0        0      982 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/SMU_Examples.py
--rw-rw-rw-   0        0        0      201 2024-05-13 03:22:46.000000 PypiInstruments-1.0.7/instruments/__init__.py
--rw-rw-rw-   0        0        0      297 2024-04-28 10:28:19.000000 PypiInstruments-1.0.7/instruments/device_scan.py
--rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.7/instruments/instruments_name.py
--rw-rw-rw-   0        0        0    11485 2024-05-09 03:56:02.000000 PypiInstruments-1.0.7/instruments/smu_keithley_2450.py
-drwxrwxrwx   0        0        0        0 2024-05-13 03:22:55.814827 PypiInstruments-1.0.7/one/
--rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.7/one/__init__.py
--rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.7/one/hello.py
--rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.7/one/main.py
--rw-rw-rw-   0        0        0       42 2024-05-13 03:22:55.816334 PypiInstruments-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-05-13 03:22:50.000000 PypiInstruments-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:36:07.768903 PypiInstruments-1.0.9/
+-rw-rw-rw-   0        0        0       83 2024-05-13 03:36:07.767907 PypiInstruments-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 03:36:07.759582 PypiInstruments-1.0.9/PypiInstruments.egg-info/
+-rw-rw-rw-   0        0        0       83 2024-05-13 03:36:07.000000 PypiInstruments-1.0.9/PypiInstruments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2024-05-13 03:36:07.000000 PypiInstruments-1.0.9/PypiInstruments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 03:36:07.000000 PypiInstruments-1.0.9/PypiInstruments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 10:18:59.000000 PypiInstruments-1.0.9/PypiInstruments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2024-05-13 03:36:07.000000 PypiInstruments-1.0.9/PypiInstruments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 03:36:07.765913 PypiInstruments-1.0.9/instruments/
+-rw-rw-rw-   0        0        0     2132 2024-05-13 03:35:26.000000 PypiInstruments-1.0.9/instruments/DP821A.py
+-rw-rw-rw-   0        0        0     3827 2024-05-13 03:35:26.000000 PypiInstruments-1.0.9/instruments/Multimemter.py
+-rw-rw-rw-   0        0        0     1006 2024-05-13 03:35:50.000000 PypiInstruments-1.0.9/instruments/SMU_Examples.py
+-rw-rw-rw-   0        0        0      201 2024-05-13 03:22:46.000000 PypiInstruments-1.0.9/instruments/__init__.py
+-rw-rw-rw-   0        0        0      309 2024-05-13 03:35:26.000000 PypiInstruments-1.0.9/instruments/device_scan.py
+-rw-rw-rw-   0        0        0      740 2024-04-29 02:13:11.000000 PypiInstruments-1.0.9/instruments/instruments_name.py
+-rw-rw-rw-   0        0        0    11497 2024-05-13 03:35:50.000000 PypiInstruments-1.0.9/instruments/smu_keithley_2450.py
+drwxrwxrwx   0        0        0        0 2024-05-13 03:36:07.767907 PypiInstruments-1.0.9/one/
+-rw-rw-rw-   0        0        0        0 2024-05-06 09:46:19.000000 PypiInstruments-1.0.9/one/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-05-04 13:35:48.000000 PypiInstruments-1.0.9/one/hello.py
+-rw-rw-rw-   0        0        0        0 2024-05-04 13:27:19.000000 PypiInstruments-1.0.9/one/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-13 03:36:07.768903 PypiInstruments-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      273 2024-05-13 03:36:02.000000 PypiInstruments-1.0.9/setup.py
```

### Comparing `PypiInstruments-1.0.7/instruments/DP821A.py` & `PypiInstruments-1.0.9/instruments/DP821A.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 BP821A functions
 """
 import pyvisa
 import pyvisa
 import time
-from instruments_name import *
+from instruments.instruments_name import *
 class Power_DP821A:
 
     def __init__(self, pRmObject, pInstruID):
         """
         actual object initial
         :param pRmObject: visa object name
         :param pInstruID: instrument ID
```

### Comparing `PypiInstruments-1.0.7/instruments/Multimemter.py` & `PypiInstruments-1.0.9/instruments/Multimemter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pyvisa
 import time
-from instruments_name import *
+from instruments.instruments_name import *
 
 """
 Brand : Gwinstek
 Function : dmm_gwinstek_api to get voltage current and frequnecy
 
 """
```

### Comparing `PypiInstruments-1.0.7/instruments/SMU_Examples.py` & `PypiInstruments-1.0.9/instruments/SMU_Examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from smu_keithley_2450 import *
 import hid
-from instruments_name import *
+from instruments.instruments_name import *
 
 """使用SMU测试的例子"""
-from instruments_name import *
+from instruments.instruments_name import *
 
 smuid = smu_2460_id
 
 smu = SmuKeithley(pyvisa.ResourceManager(), smuid)
 
 # smu.smu2450_reset()
```

### Comparing `PypiInstruments-1.0.7/instruments/instruments_name.py` & `PypiInstruments-1.0.9/instruments/instruments_name.py`

 * *Files identical despite different names*

### Comparing `PypiInstruments-1.0.7/instruments/smu_keithley_2450.py` & `PypiInstruments-1.0.9/instruments/smu_keithley_2450.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     @Description : None \n
     @Create Time : 2023/6/8 15:14 \n
     Modified by Shuai
 """
 
 import pyvisa
 import time
-from instruments_name import *
+from instruments.instruments_name import *
 
 """
     Class name: SmuKeithley
     Summary: keithley smu class
 """
 
 class SmuKeithley:
```

