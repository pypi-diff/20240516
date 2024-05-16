# Comparing `tmp/nightingalejsonadapter-2.9.0.tar.gz` & `tmp/nightingalejsonadapter-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-2.9.0.tar", last modified: Wed May  8 13:58:41 2024, max compression
+gzip compressed data, was "nightingalejsonadapter-3.0.0.tar", last modified: Thu May 16 15:29:32 2024, max compression
```

## Comparing `nightingalejsonadapter-2.9.0.tar` & `nightingalejsonadapter-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:58:41.305713 nightingalejsonadapter-2.9.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-08 13:58:41.305713 nightingalejsonadapter-2.9.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:58:41.305713 nightingalejsonadapter-2.9.0/nightingalejsonadapter/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/intervention_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      700 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/trigger_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      606 2024-05-04 00:53:27.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)     1019 2024-05-08 13:57:19.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:58:41.305713 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-08 13:58:41.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-08 13:58:41.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-08 13:58:41.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-08 13:58:41.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-08 13:58:41.000000 nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-08 13:58:41.305713 nightingalejsonadapter-2.9.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-08 13:57:31.000000 nightingalejsonadapter-2.9.0/setup.py
+drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      270 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/PKG-INFO
+drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/nightingalejsonadapter/
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/__init__.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      452 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/intervention_adapter.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      700 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      434 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/trigger_adapter.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      516 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/uuid_generator.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      776 2024-05-16 13:43:19.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      601 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_adapter.py
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)     1019 2024-05-13 08:50:47.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_response.py
+drwxr-xr-x   0 dtitestsystem  (1000) dtitestsystem  (1001)        0 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      270 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      578 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        1 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)        9 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)       23 2024-05-16 15:29:32.000000 nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)       38 2024-05-16 15:29:32.502914 nightingalejsonadapter-3.0.0/setup.cfg
+-rw-r--r--   0 dtitestsystem  (1000) dtitestsystem  (1001)      774 2024-05-16 15:27:08.000000 nightingalejsonadapter-3.0.0/setup.py
```

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter/patient_info_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter/vital_kafka_adapter.py` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter/vital_kafka_adapter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 from pydantic import BaseModel
 
 from datetime import datetime
+from typing import List, Optional
 
 
 class DateObserved(BaseModel):
     type: str
     value: datetime
 
 
 class Payload(BaseModel):
     victimid: str
     incidentid: str
     devicetype: str
-    respiratoryrate: float
-    systolicbloodpressure: float
-    diastolicbloodpressure: float
-    temperature: float
-    pulserate: float
-    heartratevariability: float
-    pulseoxymetry: float
-    skinmoisture: float
+    respiratoryrate: Optional[float] = None
+    systolicbloodpressure: Optional[float] = None
+    diastolicbloodpressure: Optional[float] = None
+    temperature: Optional[float] = None
+    pulserate: Optional[float] = None
+    heartratevariability: Optional[float] = None
+    pulseoxymetry: Optional[float] = None
+    skinmoisture: Optional[float] = None
     encounterdatetime: datetime
 
 
 class Model(BaseModel):
     id: str
     type: str
     dateObserved: DateObserved
```

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter/vitals_response.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.9.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-3.0.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.9.0/setup.py` & `nightingalejsonadapter-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.9.0' 
+VERSION = '3.0.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter",
```

