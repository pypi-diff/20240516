# Comparing `tmp/RF_Track-2.2.2a0-cp310-cp310-manylinux_2_34_x86_64.whl.zip` & `tmp/RF_Track-2.2.2b0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2410075 bytes, number of entries: 7
--rw-rw-r--  2.0 unx   122238 b- defN 24-May-09 19:26 RF_Track.py
--rwxrwxr-x  2.0 unx  7245344 b- defN 24-May-09 19:55 _RF_Track.cpython-310-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      638 b- defN 24-May-09 19:55 RF_Track-2.2.2a0.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     1748 b- defN 24-May-09 19:55 RF_Track-2.2.2a0.dist-info/METADATA
--rw-rw-r--  2.0 unx      114 b- defN 24-May-09 19:55 RF_Track-2.2.2a0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 24-May-09 19:55 RF_Track-2.2.2a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      575 b- defN 24-May-09 19:55 RF_Track-2.2.2a0.dist-info/RECORD
-7 files, 7370676 bytes uncompressed, 2409063 bytes compressed:  67.3%
+Zip file size: 2293800 bytes, number of entries: 7
+-rw-r--r--  2.0 unx   122238 b- defN 24-May-11 14:48 RF_Track.py
+-rwxr-xr-x  2.0 unx  7895536 b- defN 24-May-11 15:42 _RF_Track.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      638 b- defN 24-May-11 15:43 RF_Track-2.2.2b0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1767 b- defN 24-May-11 15:43 RF_Track-2.2.2b0.dist-info/METADATA
+-rw-r--r--  2.0 unx      111 b- defN 24-May-11 15:43 RF_Track-2.2.2b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-11 15:42 RF_Track-2.2.2b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      574 b- defN 24-May-11 15:43 RF_Track-2.2.2b0.dist-info/RECORD
+7 files, 8020883 bytes uncompressed, 2292790 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: RF_Track.py
 Comment: 
 
-Filename: _RF_Track.cpython-310-x86_64-linux-gnu.so
+Filename: _RF_Track.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: RF_Track-2.2.2a0.dist-info/LICENSE.md
+Filename: RF_Track-2.2.2b0.dist-info/LICENSE.md
 Comment: 
 
-Filename: RF_Track-2.2.2a0.dist-info/METADATA
+Filename: RF_Track-2.2.2b0.dist-info/METADATA
 Comment: 
 
-Filename: RF_Track-2.2.2a0.dist-info/WHEEL
+Filename: RF_Track-2.2.2b0.dist-info/WHEEL
 Comment: 
 
-Filename: RF_Track-2.2.2a0.dist-info/top_level.txt
+Filename: RF_Track-2.2.2b0.dist-info/top_level.txt
 Comment: 
 
-Filename: RF_Track-2.2.2a0.dist-info/RECORD
+Filename: RF_Track-2.2.2b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `RF_Track-2.2.2a0.dist-info/LICENSE.md` & `RF_Track-2.2.2b0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `RF_Track-2.2.2a0.dist-info/METADATA` & `RF_Track-2.2.2b0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: RF-Track
-Version: 2.2.2a0
+Version: 2.2.2b0
 Summary: The CERN tracking code RF-Track
 Home-page: https://gitlab.cern.ch/rf-track
 Author: Andrea Latina
 Author-email: andrea.latina@cern.ch
 License: Proprietary
 Project-URL: Documentation, https://gitlab.cern.ch/rf-track/download/-/raw/master/RF-Track-2.2.2a0/RF_Track_reference_manual.pdf?ref_type=heads
 Project-URL: Tracker, https://gitlab.cern.ch/groups/rf-track/-/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: C++
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
@@ -19,7 +20,8 @@
 Requires-Dist: numpy
 
 RF-Track is a tracking code developed at CERN for the optimization of particle accelerators, which offers outstanding flexibility and rapid simulation speed.
 
 RF-Track can simulate beams of particles with arbitrary energy, mass, and charge, even mixed, solving fully relativistic equations of motion.  It can simulate the effects of space-charge forces, both in bunched and continuous-wave beams. It can transport the beams through common elements as well as through special ones: 1D, 2D, and 3D static or oscillating radio-frequency electromagnetic field maps (real and complex), flux concentrators, and electron coolers. It allows element overlap, and direct and indirect space-charge calculation using fast parallel algorithms.
 
 RF-Track is written in optimized and parallel C++ and uses the scripting languages Octave and Python as user interfaces. General knowledge of Octave or Python is recommended to get the best out of RF-Track.
+
```

