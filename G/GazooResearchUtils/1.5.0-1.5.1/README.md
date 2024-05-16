# Comparing `tmp/GazooResearchUtils-1.5.0.tar.gz` & `tmp/GazooResearchUtils-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.5.0.tar", last modified: Thu May 16 13:58:22 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.5.1.tar", last modified: Thu May 16 15:17:02 2024, max compression
```

## Comparing `GazooResearchUtils-1.5.0.tar` & `GazooResearchUtils-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.062668 GazooResearchUtils-1.5.0/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 13:58:22.062443 GazooResearchUtils-1.5.0/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.060704 GazooResearchUtils-1.5.0/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.061115 GazooResearchUtils-1.5.0/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.062108 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     8153 2024-05-16 13:57:04.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 13:58:22.061770 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-16 13:58:22.000000 GazooResearchUtils-1.5.0/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-16 13:58:22.062713 GazooResearchUtils-1.5.0/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-16 13:57:27.000000 GazooResearchUtils-1.5.0/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:17:02.508702 GazooResearchUtils-1.5.1/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 15:17:02.508440 GazooResearchUtils-1.5.1/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:17:02.506539 GazooResearchUtils-1.5.1/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:17:02.506954 GazooResearchUtils-1.5.1/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      187 2024-05-16 13:57:19.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:17:02.508093 GazooResearchUtils-1.5.1/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     8171 2024-05-16 15:15:47.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-16 15:17:02.507693 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-16 15:17:02.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-16 15:17:02.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-16 15:17:02.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-16 15:17:02.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-16 15:17:02.000000 GazooResearchUtils-1.5.1/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-16 15:17:02.508754 GazooResearchUtils-1.5.1/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-16 15:16:34.000000 GazooResearchUtils-1.5.1/setup.py
```

### Comparing `GazooResearchUtils-1.5.0/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.5.1/app/GazooResearchUtils/src/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import numpy as np
 import pandas as pd
 from datetime import datetime
 from lifelines import KaplanMeierFitter
 import matplotlib.pyplot as plt
 
-
 def multilesion_transforation(data):
   """
   Transforms from patient level analysis to multi-target level analysis
 
   Parameters:
   data (DataFrame): dataframe from csv data
```

