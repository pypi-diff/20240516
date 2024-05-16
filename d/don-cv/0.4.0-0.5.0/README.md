# Comparing `tmp/don_cv-0.4.0.tar.gz` & `tmp/don_cv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "don_cv-0.4.0.tar", last modified: Thu May 16 17:41:15 2024, max compression
+gzip compressed data, was "don_cv-0.5.0.tar", last modified: Thu May 16 17:42:50 2024, max compression
```

## Comparing `don_cv-0.4.0.tar` & `don_cv-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:41:15.709005 don_cv-0.4.0/
--rw-rw-rw-   0        0        0      115 2024-05-16 03:50:56.000000 don_cv-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      642 2024-05-16 17:41:15.708004 don_cv-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-05-16 04:45:23.000000 don_cv-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 17:41:15.698005 don_cv-0.4.0/config/
--rw-rw-rw-   0        0        0     3259 2024-05-16 04:32:04.000000 don_cv-0.4.0/config/resume_config.json
-drwxrwxrwx   0        0        0        0 2024-05-16 17:41:15.700005 don_cv-0.4.0/don_cv/
--rw-rw-rw-   0        0        0        0 2024-05-16 04:52:38.000000 don_cv-0.4.0/don_cv/__init__.py
--rw-rw-rw-   0        0        0      887 2024-05-16 17:39:55.000000 don_cv-0.4.0/don_cv/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:41:15.707004 don_cv-0.4.0/don_cv.egg-info/
--rw-rw-rw-   0        0        0      642 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 17:41:15.000000 don_cv-0.4.0/don_cv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 17:41:15.709005 don_cv-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      899 2024-05-16 17:40:23.000000 don_cv-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:42:50.840897 don_cv-0.5.0/
+-rw-rw-rw-   0        0        0      115 2024-05-16 03:50:56.000000 don_cv-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      642 2024-05-16 17:42:50.840897 don_cv-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-05-16 04:45:23.000000 don_cv-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:42:50.826228 don_cv-0.5.0/config/
+-rw-rw-rw-   0        0        0     3259 2024-05-16 04:32:04.000000 don_cv-0.5.0/config/resume_config.json
+drwxrwxrwx   0        0        0        0 2024-05-16 17:42:50.826228 don_cv-0.5.0/don_cv/
+-rw-rw-rw-   0        0        0        0 2024-05-16 04:52:38.000000 don_cv-0.5.0/don_cv/__init__.py
+-rw-rw-rw-   0        0        0      887 2024-05-16 17:39:55.000000 don_cv-0.5.0/don_cv/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:42:50.839897 don_cv-0.5.0/don_cv.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 17:42:50.000000 don_cv-0.5.0/don_cv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:42:50.841898 don_cv-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      899 2024-05-16 17:42:36.000000 don_cv-0.5.0/setup.py
```

### Comparing `don_cv-0.4.0/PKG-INFO` & `don_cv-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: don-cv
-Version: 0.4.0
+Version: 0.5.0
 Summary: A terminal GUI displaying a configurable resume
 Home-page: https://github.com/copyleftdev/don
 Author: Don Johnson
 Author-email: dj@codetestcode.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `don_cv-0.4.0/config/resume_config.json` & `don_cv-0.5.0/config/resume_config.json`

 * *Files identical despite different names*

### Comparing `don_cv-0.4.0/don_cv/cli.py` & `don_cv-0.5.0/don_cv/cli.py`

 * *Files identical despite different names*

### Comparing `don_cv-0.4.0/don_cv.egg-info/PKG-INFO` & `don_cv-0.5.0/don_cv.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: don-cv
-Version: 0.4.0
+Version: 0.5.0
 Summary: A terminal GUI displaying a configurable resume
 Home-page: https://github.com/copyleftdev/don
 Author: Don Johnson
 Author-email: dj@codetestcode.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `don_cv-0.4.0/setup.py` & `don_cv-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
         name="don-cv",
-        version="0.4.0",
+        version="0.5.0",
         packages=find_packages(),
         entry_points={
             'console_scripts': [
                 'don-cv=don_cv.cli:main',
             ],
         },
         install_requires=[
```

