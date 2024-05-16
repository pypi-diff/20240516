# Comparing `tmp/TsingPig_Lab-0.0.2.tar.gz` & `tmp/TsingPig_Lab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.0.2.tar", last modified: Thu May 16 05:31:25 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.0.tar", last modified: Thu May 16 06:10:51 2024, max compression
```

## Comparing `TsingPig_Lab-0.0.2.tar` & `TsingPig_Lab-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.812849 TsingPig_Lab-0.0.2/
--rw-rw-rw-   0        0        0      769 2024-05-16 05:31:25.812849 TsingPig_Lab-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-16 05:29:42.000000 TsingPig_Lab-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.809837 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0      769 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 05:31:25.814226 TsingPig_Lab-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-16 05:31:05.000000 TsingPig_Lab-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.811844 TsingPig_Lab-0.0.2/tsingpig_lab/
--rw-rw-rw-   0        0        0       86 2024-05-16 05:03:00.000000 TsingPig_Lab-0.0.2/tsingpig_lab/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-16 05:04:18.000000 TsingPig_Lab-0.0.2/tsingpig_lab/tsingpig_lab.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.155794 TsingPig_Lab-0.1.0/
+-rw-rw-rw-   0        0        0      769 2024-05-16 06:10:51.154790 TsingPig_Lab-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-16 05:29:42.000000 TsingPig_Lab-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.151001 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0      769 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 06:10:51.000000 TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:10:51.155794 TsingPig_Lab-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      782 2024-05-16 06:08:43.000000 TsingPig_Lab-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:10:51.153784 TsingPig_Lab-0.1.0/tsingpig_lab/
+-rw-rw-rw-   0        0        0       86 2024-05-16 05:03:00.000000 TsingPig_Lab-0.1.0/tsingpig_lab/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 06:03:43.000000 TsingPig_Lab-0.1.0/tsingpig_lab/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 05:04:18.000000 TsingPig_Lab-0.1.0/tsingpig_lab/tsingpig_lab.py
```

### Comparing `TsingPig_Lab-0.0.2/PKG-INFO` & `TsingPig_Lab-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig_Lab
-Version: 0.0.2
+Version: 0.1.0
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: tsingpig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
```

### Comparing `TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/PKG-INFO` & `TsingPig_Lab-0.1.0/TsingPig_Lab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig-Lab
-Version: 0.0.2
+Version: 0.1.0
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: tsingpig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # tsingpig_lab
         ## 1. Introduction
```

### Comparing `TsingPig_Lab-0.0.2/setup.py` & `TsingPig_Lab-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import setuptools
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "TsingPig_Lab",
-    version = "0.0.2",
+    version = "0.1.0",
     author = "tsingpig",
     author_email = "1114196607@qq.com",
     description = "TsingPig_Lab is a package for algorithm.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url="https://gitlab.com/tsingpig-code/tsingpig_lab",
     packages=setuptools.find_packages(),
-    install_requires=['math'],
+    install_requires = [],
     # add any additional packages that needs to be installed along with SSAP package.
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

