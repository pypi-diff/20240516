# Comparing `tmp/don-cv-0.1.0.tar.gz` & `tmp/don-cv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "don-cv-0.1.0.tar", last modified: Thu May 16 04:48:35 2024, max compression
+gzip compressed data, was "don-cv-0.2.0.tar", last modified: Thu May 16 04:56:53 2024, max compression
```

## Comparing `don-cv-0.1.0.tar` & `don-cv-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 04:48:35.819893 don-cv-0.1.0/
--rw-rw-rw-   0        0        0      115 2024-05-16 03:50:56.000000 don-cv-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      642 2024-05-16 04:48:35.819893 don-cv-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-05-16 04:45:23.000000 don-cv-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 04:48:35.804893 don-cv-0.1.0/config/
--rw-rw-rw-   0        0        0     3259 2024-05-16 04:32:04.000000 don-cv-0.1.0/config/resume_config.json
-drwxrwxrwx   0        0        0        0 2024-05-16 04:48:35.818894 don-cv-0.1.0/don_cv.egg-info/
--rw-rw-rw-   0        0        0      642 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:48:35.000000 don-cv-0.1.0/don_cv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 04:48:35.820893 don-cv-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      896 2024-05-16 04:45:13.000000 don-cv-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:56:53.939015 don-cv-0.2.0/
+-rw-rw-rw-   0        0        0      115 2024-05-16 03:50:56.000000 don-cv-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      642 2024-05-16 04:56:53.938015 don-cv-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-16 04:45:23.000000 don-cv-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 04:56:53.918017 don-cv-0.2.0/config/
+-rw-rw-rw-   0        0        0     3259 2024-05-16 04:32:04.000000 don-cv-0.2.0/config/resume_config.json
+drwxrwxrwx   0        0        0        0 2024-05-16 04:56:53.919015 don-cv-0.2.0/don_cv/
+-rw-rw-rw-   0        0        0        0 2024-05-16 04:52:38.000000 don-cv-0.2.0/don_cv/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-05-16 04:13:46.000000 don-cv-0.2.0/don_cv/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 04:56:53.938015 don-cv-0.2.0/don_cv.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 04:56:53.000000 don-cv-0.2.0/don_cv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 04:56:53.939015 don-cv-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      899 2024-05-16 04:53:28.000000 don-cv-0.2.0/setup.py
```

### Comparing `don-cv-0.1.0/PKG-INFO` & `don-cv-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: don-cv
-Version: 0.1.0
+Version: 0.2.0
 Summary: A terminal GUI displaying a configurable resume
 Home-page: https://github.com/copyleftdev/don
 Author: Don Johnson
 Author-email: dj@codetestcode.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `don-cv-0.1.0/config/resume_config.json` & `don-cv-0.2.0/config/resume_config.json`

 * *Files identical despite different names*

### Comparing `don-cv-0.1.0/don_cv.egg-info/PKG-INFO` & `don-cv-0.2.0/don_cv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: don-cv
-Version: 0.1.0
+Version: 0.2.0
 Summary: A terminal GUI displaying a configurable resume
 Home-page: https://github.com/copyleftdev/don
 Author: Don Johnson
 Author-email: dj@codetestcode.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `don-cv-0.1.0/setup.py` & `don-cv-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
 from setuptools import setup, find_packages
 
 setup(
         name="don-cv",
-        version="0.1.0",
+        version="0.2.0",
         packages=find_packages(),
         entry_points={
             'console_scripts': [
-                'don-cv=don.cli:main',
+                'don-cv=don_cv.cli:main',
             ],
         },
         install_requires=[
             'rich',
             'PyYAML',
         ],
         author="Don Johnson",
```

