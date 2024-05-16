# Comparing `tmp/strainchoosr-0.1.3.tar.gz` & `tmp/strainchoosr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strainchoosr-0.1.3.tar", last modified: Tue Nov  2 14:40:09 2021, max compression
+gzip compressed data, was "strainchoosr-0.1.4.tar", last modified: Thu May 16 17:48:18 2024, max compression
```

## Comparing `strainchoosr-0.1.3.tar` & `strainchoosr-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2021-11-02 14:40:09.338693 strainchoosr-0.1.3/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     1088 2020-08-20 18:55:34.000000 strainchoosr-0.1.3/LICENSE
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      247 2021-11-02 14:40:09.338693 strainchoosr-0.1.3/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)     3536 2020-08-20 18:55:34.000000 strainchoosr-0.1.3/README.rst
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       38 2021-11-02 14:40:09.338693 strainchoosr-0.1.3/setup.cfg
--rwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)      835 2021-11-02 14:39:47.000000 strainchoosr-0.1.3/setup.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2021-11-02 14:40:09.334692 strainchoosr-0.1.3/strainchoosr/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        0 2020-08-20 18:55:34.000000 strainchoosr-0.1.3/strainchoosr/__init__.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    23277 2020-10-02 17:19:33.000000 strainchoosr-0.1.3/strainchoosr/strainchoosr.py
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)    12225 2020-08-20 18:55:34.000000 strainchoosr-0.1.3/strainchoosr/strainchoosr_gui.py
-drwxrwxr-x   0 adamkoziol  (1000) adamkoziol  (1000)        0 2021-11-02 14:40:09.338693 strainchoosr-0.1.3/strainchoosr.egg-info/
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      247 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/PKG-INFO
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      332 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/SOURCES.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)        1 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/dependency_links.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)      193 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/entry_points.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       26 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/requires.txt
--rw-rw-r--   0 adamkoziol  (1000) adamkoziol  (1000)       13 2021-11-02 14:40:09.000000 strainchoosr-0.1.3/strainchoosr.egg-info/top_level.txt
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.107815 strainchoosr-0.1.4/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     1088 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/LICENSE
+-rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/PKG-INFO
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)     3536 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/README.rst
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       38 2024-05-16 17:48:18.107815 strainchoosr-0.1.4/setup.cfg
+-rwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)      806 2024-05-16 17:46:35.000000 strainchoosr-0.1.4/setup.py
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.105815 strainchoosr-0.1.4/strainchoosr/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-15 19:24:40.000000 strainchoosr-0.1.4/strainchoosr/__init__.py
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    23277 2024-05-16 17:39:07.000000 strainchoosr-0.1.4/strainchoosr/strainchoosr.py
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    12225 2024-05-15 19:24:40.000000 strainchoosr-0.1.4/strainchoosr/strainchoosr_gui.py
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/strainchoosr.egg-info/
+-rw-r--r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      257 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/PKG-INFO
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      359 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/SOURCES.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)        1 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/dependency_links.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)      209 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/entry_points.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       27 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/requires.txt
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)       13 2024-05-16 17:48:18.000000 strainchoosr-0.1.4/strainchoosr.egg-info/top_level.txt
+drwxrwxr-x   0 cfiaadmin  (1000) cfiaadmin  (1000)        0 2024-05-16 17:48:18.106815 strainchoosr-0.1.4/tests/
+-rw-rw-r--   0 cfiaadmin  (1000) cfiaadmin  (1000)    13962 2024-05-15 17:43:00.000000 strainchoosr-0.1.4/tests/test_strainchoosr.py
```

### Comparing `strainchoosr-0.1.3/LICENSE` & `strainchoosr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.3/README.rst` & `strainchoosr-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.3/setup.py` & `strainchoosr-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='strainchoosr',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'strainchoosr = strainchoosr.strainchoosr:main',
             'strainchoosr_gui = strainchoosr.strainchoosr_gui:main',
-            'strainchoosr_drawimage = strainchoosr.strainchoosr_gui:draw_image_wrapper'
+            'strainchoosr_drawimage = strainchoosr.strainchoosr_gui: \
+                draw_image_wrapper'
         ],
     },
     author='Andrew Low',
     author_email='andrew.low@canada.ca',
     url='https://github.com/lowandrew/StrainChoosr',
-    #setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     install_requires=['pytest',
                       'ete3',
-                      'PyQt5==5.11.3',  # Apparently required by ete3 for visualisation, but not listed in that setup.py...
+                      # Required by ete3 for visualisation, but not listed
+                      'PyQt5==5.15.10',
                       ]
 )
```

### Comparing `strainchoosr-0.1.3/strainchoosr/strainchoosr.py` & `strainchoosr-0.1.4/strainchoosr/strainchoosr.py`

 * *Files identical despite different names*

### Comparing `strainchoosr-0.1.3/strainchoosr/strainchoosr_gui.py` & `strainchoosr-0.1.4/strainchoosr/strainchoosr_gui.py`

 * *Files identical despite different names*

