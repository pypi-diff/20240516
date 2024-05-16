# Comparing `tmp/TsingPig_Lab-0.1.1.tar.gz` & `tmp/TsingPig_Lab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.1.tar", last modified: Thu May 16 06:32:19 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.2.tar", last modified: Thu May 16 07:10:23 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.1.tar` & `TsingPig_Lab-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.931326 TsingPig_Lab-0.1.1/
--rw-rw-rw-   0        0        0      804 2024-05-16 06:32:19.930326 TsingPig_Lab-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.925323 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0      804 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 06:32:19.931326 TsingPig_Lab-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.929325 TsingPig_Lab-0.1.1/tsingpig_lab/
--rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.1/tsingpig_lab/ST.py
--rw-rw-rw-   0        0        0      123 2024-05-16 06:31:01.000000 TsingPig_Lab-0.1.1/tsingpig_lab/__init__.py
--rw-rw-rw-   0        0        0      209 2024-05-16 06:31:01.000000 TsingPig_Lab-0.1.1/tsingpig_lab/tsingpig_lab.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.698287 TsingPig_Lab-0.1.2/
+-rw-rw-rw-   0        0        0      804 2024-05-16 07:10:23.697286 TsingPig_Lab-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.689801 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0      804 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:10:23.698287 TsingPig_Lab-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.696287 TsingPig_Lab-0.1.2/tsingpig_lab/
+-rw-rw-rw-   0        0        0     2075 2024-05-16 07:06:31.000000 TsingPig_Lab-0.1.2/tsingpig_lab/BaseConverter.py
+-rw-rw-rw-   0        0        0      413 2024-05-16 07:06:31.000000 TsingPig_Lab-0.1.2/tsingpig_lab/Bin.py
+-rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.2/tsingpig_lab/ST.py
+-rw-rw-rw-   0        0        0      260 2024-05-16 07:10:16.000000 TsingPig_Lab-0.1.2/tsingpig_lab/__init__.py
+-rw-rw-rw-   0        0        0      195 2024-05-16 07:09:51.000000 TsingPig_Lab-0.1.2/tsingpig_lab/tsingpig_lab.py
```

### Comparing `TsingPig_Lab-0.1.1/PKG-INFO` & `TsingPig_Lab-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig_Lab
-Version: 0.1.1
+Version: 0.1.2
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
```

### Comparing `TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/PKG-INFO` & `TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig-Lab
-Version: 0.1.1
+Version: 0.1.2
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
```

### Comparing `TsingPig_Lab-0.1.1/setup.py` & `TsingPig_Lab-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.1/tsingpig_lab/ST.py` & `TsingPig_Lab-0.1.2/tsingpig_lab/ST.py`

 * *Files identical despite different names*

