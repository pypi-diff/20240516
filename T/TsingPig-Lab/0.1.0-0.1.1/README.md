# Comparing `tmp/TsingPig_Lab-0.1.0.tar.gz` & `tmp/TsingPig_Lab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.0.tar", last modified: Thu May 16 06:10:51 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.1.tar", last modified: Thu May 16 06:32:19 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.0.tar` & `TsingPig_Lab-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.155794 TsingPig_Lab-0.1.0/
--rw-rw-rw-   0        0        0      769 2024-05-16 06:10:51.154790 TsingPig_Lab-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-16 05:29:42.000000 TsingPig_Lab-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.151001 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0      769 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 06:10:51.155794 TsingPig_Lab-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      782 2024-05-16 06:08:43.000000 TsingPig_Lab-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.153784 TsingPig_Lab-0.1.0/tsingpig_lab/
--rw-rw-rw-   0        0        0       86 2024-05-16 05:03:00.000000 TsingPig_Lab-0.1.0/tsingpig_lab/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-16 06:03:43.000000 TsingPig_Lab-0.1.0/tsingpig_lab/main.py
--rw-rw-rw-   0        0        0       42 2024-05-16 05:04:18.000000 TsingPig_Lab-0.1.0/tsingpig_lab/tsingpig_lab.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.931326 TsingPig_Lab-0.1.1/
+-rw-rw-rw-   0        0        0      804 2024-05-16 06:32:19.930326 TsingPig_Lab-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.925323 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0      804 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 06:32:19.000000 TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:32:19.931326 TsingPig_Lab-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:32:19.929325 TsingPig_Lab-0.1.1/tsingpig_lab/
+-rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.1/tsingpig_lab/ST.py
+-rw-rw-rw-   0        0        0      123 2024-05-16 06:31:01.000000 TsingPig_Lab-0.1.1/tsingpig_lab/__init__.py
+-rw-rw-rw-   0        0        0      209 2024-05-16 06:31:01.000000 TsingPig_Lab-0.1.1/tsingpig_lab/tsingpig_lab.py
```

### Comparing `TsingPig_Lab-0.1.0/PKG-INFO` & `TsingPig_Lab-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: TsingPig_Lab
-Version: 0.1.0
+Version: 0.1.1
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
-Author: tsingpig
+Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
         This is a python package for acm-algorithm which is developed by **tsingpig**.
         
         You can connect me by email: 1114196607@qq.com
         
         Thanks for your support!
         
+        Version: v0.1.1
+        
         ## 2. Functions
         ### 2.1. Data Structure
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/PKG-INFO` & `TsingPig_Lab-0.1.1/TsingPig_Lab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: TsingPig-Lab
-Version: 0.1.0
+Version: 0.1.1
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
-Author: tsingpig
+Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
         This is a python package for acm-algorithm which is developed by **tsingpig**.
         
         You can connect me by email: 1114196607@qq.com
         
         Thanks for your support!
         
+        Version: v0.1.1
+        
         ## 2. Functions
         ### 2.1. Data Structure
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `TsingPig_Lab-0.1.0/setup.py` & `TsingPig_Lab-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import tsingpig_lab
+
+__version__ = tsingpig_lab.__version__
+__author__ = tsingpig_lab.__author__
+__package_name__ = tsingpig_lab.__package_name__
+
 
 import setuptools
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name = "TsingPig_Lab",
-    version = "0.1.0",
-    author = "tsingpig",
+    name = __package_name__,
+    version = __version__,
+    author = __author__,
     author_email = "1114196607@qq.com",
     description = "TsingPig_Lab is a package for algorithm.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url="https://gitlab.com/tsingpig-code/tsingpig_lab",
     packages=setuptools.find_packages(),
     install_requires = [],
```

