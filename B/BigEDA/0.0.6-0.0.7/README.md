# Comparing `tmp/BigEDA-0.0.6.tar.gz` & `tmp/bigeda-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BigEDA-0.0.6.tar", last modified: Sat Dec  9 16:32:59 2023, max compression
+gzip compressed data, was "bigeda-0.0.7.tar", last modified: Thu May 16 21:19:10 2024, max compression
```

## Comparing `BigEDA-0.0.6.tar` & `bigeda-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-12-09 16:32:59.720794 BigEDA-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-12-09 16:32:59.694319 BigEDA-0.0.6/BigEDA/
--rw-rw-rw-   0        0        0       76 2023-12-09 16:04:49.000000 BigEDA-0.0.6/BigEDA/EDA.py
--rw-rw-rw-   0        0        0       33 2023-12-09 15:31:13.000000 BigEDA-0.0.6/BigEDA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 16:32:59.708980 BigEDA-0.0.6/BigEDA.egg-info/
--rw-rw-rw-   0        0        0      868 2023-12-09 16:32:59.000000 BigEDA-0.0.6/BigEDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-12-09 16:32:59.000000 BigEDA-0.0.6/BigEDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-09 16:32:59.000000 BigEDA-0.0.6/BigEDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-12-09 16:32:59.000000 BigEDA-0.0.6/BigEDA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-12-09 16:32:59.000000 BigEDA-0.0.6/BigEDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 BigEDA-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      868 2023-12-09 16:32:59.708980 BigEDA-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 BigEDA-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-12-09 16:32:59.720794 BigEDA-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-12-09 16:32:06.000000 BigEDA-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.394977 bigeda-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.352593 bigeda-0.0.7/BigEDA/
+-rw-rw-rw-   0        0        0      783 2024-03-31 16:22:20.000000 bigeda-0.0.7/BigEDA/__init__.py
+-rw-rw-rw-   0        0        0    26808 2024-05-13 16:49:56.000000 bigeda-0.0.7/BigEDA/descriptive.py
+-rw-rw-rw-   0        0        0    78541 2024-05-13 23:16:09.000000 bigeda-0.0.7/BigEDA/plots.py
+-rw-rw-rw-   0        0        0    11707 2024-04-14 01:24:57.000000 bigeda-0.0.7/BigEDA/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:10.392428 bigeda-0.0.7/BigEDA.egg-info/
+-rw-rw-rw-   0        0        0      870 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 21:19:10.000000 bigeda-0.0.7/BigEDA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 bigeda-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      870 2024-05-16 21:19:10.393459 bigeda-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 bigeda-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 21:19:10.394977 bigeda-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      838 2024-05-16 21:18:22.000000 bigeda-0.0.7/setup.py
```

### Comparing `BigEDA-0.0.6/BigEDA.egg-info/PKG-INFO` & `bigeda-0.0.7/BigEDA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.6
-Summary: This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
+Version: 0.0.7
+Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `BigEDA-0.0.6/LICENSE` & `bigeda-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BigEDA-0.0.6/PKG-INFO` & `bigeda-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.6
-Summary: This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
+Version: 0.0.7
+Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `BigEDA-0.0.6/setup.py` & `bigeda-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="BigEDA",
-    version="0.0.6",
+    version="0.0.7",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
-    description="This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.",
+    description="This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/EDA_Package",  # add your project URL here
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

