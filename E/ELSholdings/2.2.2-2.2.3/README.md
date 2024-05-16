# Comparing `tmp/elsholdings-2.2.2.tar.gz` & `tmp/elsholdings-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elsholdings-2.2.2.tar", last modified: Thu May 16 01:55:45 2024, max compression
+gzip compressed data, was "elsholdings-2.2.3.tar", last modified: Thu May 16 02:01:43 2024, max compression
```

## Comparing `elsholdings-2.2.2.tar` & `elsholdings-2.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 01:55:45.073692 elsholdings-2.2.2/
-drwxrwxrwx   0        0        0        0 2024-05-16 01:55:45.038756 elsholdings-2.2.2/ELSholdings/
-drwxrwxrwx   0        0        0        0 2024-05-16 01:55:45.068679 elsholdings-2.2.2/ELSholdings/kenwoo/
--rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.2/ELSholdings/kenwoo/xls2ppt.py
--rw-rw-rw-   0        0        0    46051 2024-05-16 01:55:02.000000 elsholdings-2.2.2/ELSholdings/kenwoo/xls2ppt_pc.py
-drwxrwxrwx   0        0        0        0 2024-05-16 01:55:45.070680 elsholdings-2.2.2/ELSholdings.egg-info/
--rw-rw-rw-   0        0        0      425 2024-05-16 01:55:44.000000 elsholdings-2.2.2/ELSholdings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-16 01:55:45.000000 elsholdings-2.2.2/ELSholdings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 01:55:45.000000 elsholdings-2.2.2/ELSholdings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 01:55:45.000000 elsholdings-2.2.2/ELSholdings.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      425 2024-05-16 01:55:45.071680 elsholdings-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.2/README.md
--rw-rw-rw-   0        0        0      366 2024-05-16 01:55:12.000000 elsholdings-2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 01:55:45.073692 elsholdings-2.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.995366 elsholdings-2.2.3/
+drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.961809 elsholdings-2.2.3/ELSholdings/
+drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.990366 elsholdings-2.2.3/ELSholdings/kenwoo/
+-rw-rw-rw-   0        0        0    46067 2024-05-15 22:45:21.000000 elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt.py
+-rw-rw-rw-   0        0        0    46032 2024-05-16 02:01:15.000000 elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt_pc.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:01:43.992365 elsholdings-2.2.3/ELSholdings.egg-info/
+-rw-rw-rw-   0        0        0      425 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 02:01:43.000000 elsholdings-2.2.3/ELSholdings.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      425 2024-05-16 02:01:43.994366 elsholdings-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2024-05-13 23:52:45.000000 elsholdings-2.2.3/README.md
+-rw-rw-rw-   0        0        0      366 2024-05-16 02:01:26.000000 elsholdings-2.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 02:01:43.995366 elsholdings-2.2.3/setup.cfg
```

### Comparing `elsholdings-2.2.2/ELSholdings/kenwoo/xls2ppt.py` & `elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt.py`

 * *Files identical despite different names*

### Comparing `elsholdings-2.2.2/ELSholdings/kenwoo/xls2ppt_pc.py` & `elsholdings-2.2.3/ELSholdings/kenwoo/xls2ppt_pc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Tue May 16 2024
 
 @author: S.T.Hwang
 """
 
-def pptout(file_in,file_out):
-    file=file_in
+def pptout(file,file_out):
+
     file_out_ppt= file_out
 
     import pandas as pd
     import numpy as np
 
     df=pd.read_excel(file,skiprows=32,usecols=None)
```

