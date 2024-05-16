# Comparing `tmp/strainchoosr-0.1.4.tar.gz` & `tmp/strainchoosr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strainchoosr-0.1.4.tar", last modified: Thu May 16 17:48:18 2024, max compression
+gzip compressed data, was "strainchoosr-0.1.5.tar", last modified: Thu May 16 18:12:43 2024, max compression
```

## Comparing `strainchoosr-0.1.4.tar` & `strainchoosr-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.107815 strainchoosr-0.1.4/
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     1088 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/LICENSE
--rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/PKG-INFO
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     3536 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/README.rst
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       38 2024-05-16 17:48:18.107815 strainchoosr-0.1.4/setup.cfg
--rwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)      806 2024-05-16 17:46:35.000000 strainchoosr-0.1.4/setup.py
-drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.105815 strainchoosr-0.1.4/strainchoosr/
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-15 19:24:40.000000 strainchoosr-0.1.4/strainchoosr/__init__.py
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    23277 2024-05-16 17:39:07.000000 strainchoosr-0.1.4/strainchoosr/strainchoosr.py
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    12225 2024-05-15 19:24:40.000000 strainchoosr-0.1.4/strainchoosr/strainchoosr_gui.py
-drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/strainchoosr.egg-info/
--rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/PKG-INFO
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      359 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/SOURCES.txt
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        1 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/dependency_links.txt
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      209 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/entry_points.txt
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       27 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/requires.txt
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       13 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/top_level.txt
-drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/tests/
--rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    13962 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/tests/test_strainchoosr.py
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 18:12:43.526609 strainchoosr-0.1.5/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     1088 2024-05-15 17:43:00.000000 strainchoosr-0.1.5/LICENSE
+-rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 18:12:43.525609 strainchoosr-0.1.5/PKG-INFO
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     3536 2024-05-15 17:43:00.000000 strainchoosr-0.1.5/README.rst
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       38 2024-05-16 18:12:43.526609 strainchoosr-0.1.5/setup.cfg
+-rwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)      806 2024-05-16 18:12:12.000000 strainchoosr-0.1.5/setup.py
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 18:12:43.524609 strainchoosr-0.1.5/strainchoosr/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-15 19:24:40.000000 strainchoosr-0.1.5/strainchoosr/__init__.py
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    23277 2024-05-16 17:39:07.000000 strainchoosr-0.1.5/strainchoosr/strainchoosr.py
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    12225 2024-05-15 19:24:40.000000 strainchoosr-0.1.5/strainchoosr/strainchoosr_gui.py
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 18:12:43.525609 strainchoosr-0.1.5/strainchoosr.egg-info/
+-rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/PKG-INFO
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      359 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        1 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      209 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/entry_points.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       27 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/requires.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       13 2024-05-16 18:12:43.000000 strainchoosr-0.1.5/strainchoosr.egg-info/top_level.txt
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 18:12:43.525609 strainchoosr-0.1.5/tests/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    13962 2024-05-15 17:43:00.000000 strainchoosr-0.1.5/tests/test_strainchoosr.py
```

### Comparing `strainchoosr-0.1.4/LICENSE` & `strainchoosr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.4/README.rst` & `strainchoosr-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.4/setup.py` & `strainchoosr-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='strainchoosr',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'strainchoosr = strainchoosr.strainchoosr:main',
             'strainchoosr_gui = strainchoosr.strainchoosr_gui:main',
             'strainchoosr_drawimage = strainchoosr.strainchoosr_gui: \
                 draw_image_wrapper'
```

### Comparing `strainchoosr-0.1.4/strainchoosr/strainchoosr.py` & `strainchoosr-0.1.5/strainchoosr/strainchoosr.py`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.4/strainchoosr/strainchoosr_gui.py` & `strainchoosr-0.1.5/strainchoosr/strainchoosr_gui.py`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.4/tests/test_strainchoosr.py` & `strainchoosr-0.1.5/tests/test_strainchoosr.py`

 * *Files identical despite different names*

