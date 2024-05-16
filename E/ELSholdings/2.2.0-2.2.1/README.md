# Comparing `tmp/elsholdings-2.2.0.tar.gz` & `tmp/elsholdings-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsholdings-2.2.0.tar", last modified: Wed May 15 23:49:20 2024, max compression
+gzip compressed data, was "elsholdings-2.2.1.tar", last modified: Thu May 16 01:43:28 2024, max compression
```

## Comparing `elsholdings-2.2.0.tar` & `elsholdings-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 23:49:20.951471 elsholdings-2.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:49:20.925401 elsholdings-2.2.0/ELSholdings/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:49:20.947181 elsholdings-2.2.0/ELSholdings/kenwoo/
--rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.0/ELSholdings/kenwoo/xls2ppt.py
--rw-rw-rw-   0        0        0    46067 2024-05-15 23:46:50.000000 elsholdings-2.2.0/ELSholdings/kenwoo/xls2ppt_pc.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:49:20.949294 elsholdings-2.2.0/ELSholdings.egg-info/
--rw-rw-rw-   0        0        0      425 2024-05-15 23:49:20.000000 elsholdings-2.2.0/ELSholdings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-15 23:49:20.000000 elsholdings-2.2.0/ELSholdings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 23:49:20.000000 elsholdings-2.2.0/ELSholdings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-15 23:49:20.000000 elsholdings-2.2.0/ELSholdings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2024-05-15 23:49:20.950420 elsholdings-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.0/README.md
--rw-rw-rw-   0        0        0      366 2024-05-15 23:49:06.000000 elsholdings-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 23:49:20.951471 elsholdings-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 01:43:28.303416 elsholdings-2.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-16 01:43:28.279076 elsholdings-2.2.1/ELSholdings/
+drwxrwxrwx   0        0        0        0 2024-05-16 01:43:28.297228 elsholdings-2.2.1/ELSholdings/kenwoo/
+-rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.1/ELSholdings/kenwoo/xls2ppt.py
+-rw-rw-rw-   0        0        0    46033 2024-05-16 01:43:06.000000 elsholdings-2.2.1/ELSholdings/kenwoo/xls2ppt_pc.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:43:28.299233 elsholdings-2.2.1/ELSholdings.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-16 01:43:28.000000 elsholdings-2.2.1/ELSholdings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-16 01:43:28.000000 elsholdings-2.2.1/ELSholdings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 01:43:28.000000 elsholdings-2.2.1/ELSholdings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 01:43:28.000000 elsholdings-2.2.1/ELSholdings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      425 2024-05-16 01:43:28.300375 elsholdings-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.1/README.md
+-rw-rw-rw-   0        0        0      366 2024-05-16 01:43:14.000000 elsholdings-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 01:43:28.303416 elsholdings-2.2.1/setup.cfg
```

### Comparing `elsholdings-2.2.0/ELSholdings/kenwoo/xls2ppt.py` & `elsholdings-2.2.1/ELSholdings/kenwoo/xls2ppt.py`

 * *Files identical despite different names*

### Comparing `elsholdings-2.2.0/ELSholdings/kenwoo/xls2ppt_pc.py` & `elsholdings-2.2.1/ELSholdings/kenwoo/xls2ppt_pc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue May 14 07:57:04 2024
+Created on Tue May 16 2024
 
 @author: S.T.Hwang
 """
 
-def colab_ppt(file):
-    # file_out_ppt= '/content/drive/MyDrive/PPT_Output.xlsx'
+def pptout(file_in,file_out):
+    file_out_ppt= file_out
 
     import pandas as pd
     import numpy as np
 
     df=pd.read_excel(file,skiprows=32,usecols=None)
```

