# Comparing `tmp/TsingPig_Lab-0.0.1.tar.gz` & `tmp/TsingPig_Lab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.0.1.tar", last modified: Thu May 16 05:09:43 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.0.2.tar", last modified: Thu May 16 05:31:25 2024, max compression
```

## Comparing `TsingPig_Lab-0.0.1.tar` & `TsingPig_Lab-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 05:09:43.139898 TsingPig_Lab-0.0.1/
--rw-rw-rw-   0        0        0      481 2024-05-16 05:09:43.139898 TsingPig_Lab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-05-16 04:51:39.000000 TsingPig_Lab-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 05:09:43.135620 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0      481 2024-05-16 05:09:43.000000 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-16 05:09:43.000000 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 05:09:43.000000 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 05:09:43.000000 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 05:09:43.000000 TsingPig_Lab-0.0.1/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 05:09:43.139898 TsingPig_Lab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      786 2024-05-16 05:04:18.000000 TsingPig_Lab-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 05:09:43.137596 TsingPig_Lab-0.0.1/tsingpig_lab/
--rw-rw-rw-   0        0        0       86 2024-05-16 05:03:00.000000 TsingPig_Lab-0.0.1/tsingpig_lab/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-16 05:04:18.000000 TsingPig_Lab-0.0.1/tsingpig_lab/tsingpig_lab.py
+drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.812849 TsingPig_Lab-0.0.2/
+-rw-rw-rw-   0        0        0      769 2024-05-16 05:31:25.812849 TsingPig_Lab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-16 05:29:42.000000 TsingPig_Lab-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.809837 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0      769 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 05:31:25.000000 TsingPig_Lab-0.0.2/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 05:31:25.814226 TsingPig_Lab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      786 2024-05-16 05:31:05.000000 TsingPig_Lab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 05:31:25.811844 TsingPig_Lab-0.0.2/tsingpig_lab/
+-rw-rw-rw-   0        0        0       86 2024-05-16 05:03:00.000000 TsingPig_Lab-0.0.2/tsingpig_lab/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 05:04:18.000000 TsingPig_Lab-0.0.2/tsingpig_lab/tsingpig_lab.py
```

### Comparing `TsingPig_Lab-0.0.1/setup.py` & `TsingPig_Lab-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "TsingPig_Lab",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "tsingpig",
     author_email = "1114196607@qq.com",
     description = "TsingPig_Lab is a package for algorithm.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url="https://gitlab.com/tsingpig-code/tsingpig_lab",
     packages=setuptools.find_packages(),
```

