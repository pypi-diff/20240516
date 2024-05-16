# Comparing `tmp/py2saber-0.15.6.tar.gz` & `tmp/py2saber-0.15.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2saber-0.15.6.tar", last modified: Tue May 14 16:37:11 2024, max compression
+gzip compressed data, was "py2saber-0.15.7.tar", last modified: Wed May 15 19:22:37 2024, max compression
```

## Comparing `py2saber-0.15.6.tar` & `py2saber-0.15.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 16:37:11.928532 py2saber-0.15.6/
--rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.6/COPYING
--rw-r--r--   0 jramboz    (501) staff       (20)       35 2024-05-13 18:09:11.000000 py2saber-0.15.6/MANIFEST.in
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-14 16:37:11.928328 py2saber-0.15.6/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.6/README.md
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 16:37:11.911437 py2saber-0.15.6/py2saber/
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 16:37:11.927744 py2saber-0.15.6/py2saber/OpenCore_OEM/
--rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/BEEP.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_10_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_9_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/HUM_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/POWEROFF_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/POWERON_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWING.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
--rw-r--r--   0 jramboz    (501) staff       (20)      239 2024-05-14 16:36:57.000000 py2saber-0.15.6/py2saber/__init__.py
--rw-r--r--   0 jramboz    (501) staff       (20)       77 2024-05-14 14:49:39.000000 py2saber-0.15.6/py2saber/__main__.py
--rw-r--r--   0 jramboz    (501) staff       (20)    30549 2024-05-14 16:36:57.000000 py2saber-0.15.6/py2saber/py2saber.py
-drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-14 16:37:11.928017 py2saber-0.15.6/py2saber.egg-info/
--rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/PKG-INFO
--rw-r--r--   0 jramboz    (501) staff       (20)     1524 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/SOURCES.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/dependency_links.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       57 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/entry_points.txt
--rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/requires.txt
--rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-14 16:37:11.000000 py2saber-0.15.6/py2saber.egg-info/top_level.txt
--rw-r--r--   0 jramboz    (501) staff       (20)      802 2024-05-14 16:36:57.000000 py2saber-0.15.6/pyproject.toml
--rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-14 16:37:11.928569 py2saber-0.15.6/setup.cfg
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-15 19:22:37.348498 py2saber-0.15.7/
+-rw-r--r--   0 jramboz    (501) staff       (20)    35149 2023-05-23 13:52:35.000000 py2saber-0.15.7/COPYING
+-rw-r--r--   0 jramboz    (501) staff       (20)       35 2024-05-13 18:09:11.000000 py2saber-0.15.7/MANIFEST.in
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-15 19:22:37.348278 py2saber-0.15.7/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     2047 2024-03-20 16:03:37.000000 py2saber-0.15.7/README.md
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-15 19:22:37.333205 py2saber-0.15.7/py2saber/
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-15 19:22:37.347735 py2saber-0.15.7/py2saber/OpenCore_OEM/
+-rw-r--r--   0 jramboz    (501) staff       (20)    12004 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/BEEP.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88656 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_10_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_9_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/HUM_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/POWEROFF_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    88200 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/POWERON_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWING.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)    82592 2024-05-13 14:59:27.000000 py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW
+-rw-r--r--   0 jramboz    (501) staff       (20)      239 2024-05-15 19:22:10.000000 py2saber-0.15.7/py2saber/__init__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)       77 2024-05-14 14:49:39.000000 py2saber-0.15.7/py2saber/__main__.py
+-rw-r--r--   0 jramboz    (501) staff       (20)    30932 2024-05-15 19:22:10.000000 py2saber-0.15.7/py2saber/py2saber.py
+drwxr-xr-x   0 jramboz    (501) staff       (20)        0 2024-05-15 19:22:37.348000 py2saber-0.15.7/py2saber.egg-info/
+-rw-r--r--   0 jramboz    (501) staff       (20)    43211 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/PKG-INFO
+-rw-r--r--   0 jramboz    (501) staff       (20)     1524 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/SOURCES.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        1 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/dependency_links.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       57 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/entry_points.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)       23 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/requires.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)        9 2024-05-15 19:22:37.000000 py2saber-0.15.7/py2saber.egg-info/top_level.txt
+-rw-r--r--   0 jramboz    (501) staff       (20)      802 2024-05-15 19:22:10.000000 py2saber-0.15.7/pyproject.toml
+-rw-r--r--   0 jramboz    (501) staff       (20)       38 2024-05-15 19:22:37.348529 py2saber-0.15.7/setup.cfg
```

### Comparing `py2saber-0.15.6/COPYING` & `py2saber-0.15.7/COPYING`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/PKG-INFO` & `py2saber-0.15.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.6
+Version: 0.15.7
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.6/README.md` & `py2saber-0.15.7/README.md`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/BEEP.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/BEEP.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_10_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_10_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_1_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_2_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_3_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_4_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_5_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_6_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_7_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_8_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/CLASH_9_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/CLASH_9_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/HUM_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/HUM_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/POWEROFF_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/POWEROFF_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/POWERON_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/POWERON_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWING.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWING.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGH_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_1_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_2_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_3_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_4_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_5_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_6_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_7_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW` & `py2saber-0.15.7/py2saber/OpenCore_OEM/SMOOTHSWINGL_8_0.RAW`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/py2saber/py2saber.py` & `py2saber-0.15.7/py2saber/py2saber.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import errno
 from getch import pause_exit
 import glob
 import time
 
 basedir = os.path.dirname(os.path.realpath(__file__))
 
-script_version = '0.15.6'
+script_version = '0.15.7'
 script_authors = 'Jason Ramboz'
 script_repo = 'https://github.com/jramboz/py2saber'
 
 # adapted from https://stackoverflow.com/a/66491013
 class DocDefaultException(Exception):
     """Subclass exceptions use docstring as default message"""
     def __init__(self, msg=None, *args, **kwargs):
@@ -480,22 +480,24 @@
                 return
         
         cmd = cmd + bytes(str(bank),'ascii') + b'=' + self.rgbw_to_byte_str(r, g, b, w) + b'\n'
         self.send_command(cmd)
         response = self.read_line()
         if response[:2] != b'OK':
             raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+        self.save_config()
     
     def set_active_bank(self, bank:int):
         '''Sets the active bank (0-7)'''
         cmd = b'B=' + bytes(str(bank), 'ascii') + b'\n'
         self.send_command(cmd)
         response = self.read_line()
         if response[:2] != b'OK':
             raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+        self.save_config()
     
     @staticmethod
     def _get_cmd_for_sound_effect(effect: str) -> bytes:
         '''returns the command header for the given sound effect. Calling function needs to either add '?' or '=' to the end.'''
         match effect:
             case 'on':
                 return b'sON'
@@ -518,26 +520,35 @@
         '''Sets the sound list for a given effect.'''
         self.log.debug(f'Setting sound files {str(files)} for effect "{effect}".')
         cmd = self._get_cmd_for_sound_effect(effect) + b'=' + ','.join(files).encode('utf-8')
         self.send_command(cmd)
         response = self.read_line()
         if response != b'OK ' + cmd + b'\n':
             raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+        self.save_config()
 
     def get_sounds_for_effect(self, effect: str) -> list[str]:
         '''Returns a list of filenames Anima is using for the specified effect.'''
         self.log.debug(f'Retrieving list of sound files for effect "{effect}".')
         cmd = self._get_cmd_for_sound_effect(effect) + b'?'
         self.send_command(cmd)
         response = self.read_line()
         r = response.split(b'=')
         if r[0] != self._get_cmd_for_sound_effect(effect):
             raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
         return r[1].decode().strip().split(',')
 
+    def save_config(self):
+        '''Save the current configuration to the saber.'''
+        cmd = b'SAVE'
+        self.send_command(cmd)
+        response = self.read_line()
+        if response != b'OK SAVE\n':
+            raise InvalidSaberResponseException(f'Command: {cmd}\nResponse: {response}')
+
 # ---------------------------------------------------------------------- #
 # Command Line Operations                                                #
 # ---------------------------------------------------------------------- #
 
 def error_handler(e: DocDefaultException):
     '''Print an exception to the log.'''
     log = logging.getLogger()
```

### Comparing `py2saber-0.15.6/py2saber.egg-info/PKG-INFO` & `py2saber-0.15.7/py2saber.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2saber
-Version: 0.15.6
+Version: 0.15.7
 Summary: Python-based utility for OpenCore lightsabers
 Author-email: Jason Ramboz <jramboz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `py2saber-0.15.6/py2saber.egg-info/SOURCES.txt` & `py2saber-0.15.7/py2saber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2saber-0.15.6/pyproject.toml` & `py2saber-0.15.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py2saber"
-version = "0.15.6"
+version = "0.15.7"
 description = "Python-based utility for OpenCore lightsabers"
 readme = "README.md"
 authors = [{name = "Jason Ramboz", email = "jramboz@gmail.com"}]
 license = {file = "COPYING"}
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

