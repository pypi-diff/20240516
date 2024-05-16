# Comparing `tmp/desalsim-1.0.1.tar.gz` & `tmp/desalsim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desalsim-1.0.1.tar", last modified: Wed May  8 13:06:26 2024, max compression
+gzip compressed data, was "desalsim-1.0.2.tar", last modified: Thu May 16 13:59:05 2024, max compression
```

## Comparing `desalsim-1.0.1.tar` & `desalsim-1.0.2.tar`

### file list

```diff
@@ -1,63 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.157386 desalsim-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.156390 desalsim-1.0.1/DesalSim.egg-info/
--rw-rw-rw-   0        0        0    10098 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1295 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 13:06:26.000000 desalsim-1.0.1/DesalSim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.121482 desalsim-1.0.1/Desalsim/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-1.0.1/Desalsim/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.1/Desalsim/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/Desalsim/density_calc.py
--rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-1.0.1/Desalsim/economic_f.py
--rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-1.0.1/Desalsim/ed_unit_f.py
--rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-1.0.1/Desalsim/edbm_unit_f.py
--rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-1.0.1/Desalsim/efc_unit_f.py
--rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/med_unit_f.py
--rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-1.0.1/Desalsim/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-1.0.1/Desalsim/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/Desalsim/scaleup.py
--rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-1.0.1/Desalsim/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    10098 2024-05-08 13:06:26.157252 desalsim-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9620 2024-05-08 13:01:14.000000 desalsim-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.137440 desalsim-1.0.1/example/
--rw-rw-rw-   0        0        0      786 2024-05-08 06:53:49.000000 desalsim-1.0.1/example/__init__.py
--rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0.1/example/comparison.py
--rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0.1/example/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/example/density_calc.py
--rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/economic_f.py
--rw-rw-rw-   0        0        0     8681 2024-05-08 08:11:06.000000 desalsim-1.0.1/example/ed_unit_f.py
--rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-1.0.1/example/edbm_unit_f.py
--rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-1.0.1/example/efc_unit_f.py
--rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/example_1.py
--rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/example_2.py
--rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/med_unit_f.py
--rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/ro_unit.py
--rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.1/example/ro_unit_f.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/example/scaleup.py
--rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-1.0.1/example/thermal_cryst_f.py
--rw-rw-rw-   0        0        0       42 2024-05-08 13:06:26.157386 desalsim-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-08 13:06:16.000000 desalsim-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:06:26.155391 desalsim-1.0.1/tests/
--rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.1/tests/constants.py
--rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.1/tests/density_calc.py
--rw-rw-rw-   0        0        0     9108 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/economic_f.py
--rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0.1/tests/economic_unittest.py
--rw-rw-rw-   0        0        0     3040 2024-05-08 12:31:10.000000 desalsim-1.0.1/tests/ed_unit_f.py
--rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0.1/tests/ed_unittest.py
--rw-rw-rw-   0        0        0    12683 2024-05-08 08:13:45.000000 desalsim-1.0.1/tests/edbm_unit_f.py
--rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/edbm_unittest.py
--rw-rw-rw-   0        0        0     4508 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/med_unit_f.py
--rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/med_unittest.py
--rw-rw-rw-   0        0        0    10426 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/mfpfr_unit_f.py
--rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/mfpfr_unittest.py
--rw-rw-rw-   0        0        0     6984 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/nanofiltration_unit_f.py
--rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0.1/tests/nanofiltration_unittest.py
--rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.1/tests/scaleup.py
--rw-rw-rw-   0        0        0     8730 2024-05-08 08:01:54.000000 desalsim-1.0.1/tests/thermal_cryst_f.py
--rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0.1/tests/thermal_cryst_unittest.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.838813 desalsim-1.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.833830 desalsim-1.0.2/DesalSim.egg-info/
+-rw-rw-rw-   0        0        0     7300 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 13:59:05.000000 desalsim-1.0.2/DesalSim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.764013 desalsim-1.0.2/Desalsim/
+-rw-rw-rw-   0        0        0      786 2024-05-08 06:53:28.000000 desalsim-1.0.2/Desalsim/__init__.py
+-rw-rw-rw-   0        0        0     1927 2024-02-13 13:45:06.000000 desalsim-1.0.2/Desalsim/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.2/Desalsim/density_calc.py
+-rw-rw-rw-   0        0        0     8836 2024-05-08 07:40:34.000000 desalsim-1.0.2/Desalsim/economic_f.py
+-rw-rw-rw-   0        0        0     3007 2024-05-08 12:26:00.000000 desalsim-1.0.2/Desalsim/ed_unit_f.py
+-rw-rw-rw-   0        0        0    11748 2024-05-08 08:38:05.000000 desalsim-1.0.2/Desalsim/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    46932 2024-05-08 09:51:24.000000 desalsim-1.0.2/Desalsim/efc_unit_f.py
+-rw-rw-rw-   0        0        0     4504 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/med_unit_f.py
+-rw-rw-rw-   0        0        0    10067 2024-05-08 12:42:08.000000 desalsim-1.0.2/Desalsim/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     7011 2024-05-08 07:40:14.000000 desalsim-1.0.2/Desalsim/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/Desalsim/scaleup.py
+-rw-rw-rw-   0        0        0     8749 2024-05-08 07:58:46.000000 desalsim-1.0.2/Desalsim/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0     1086 2024-02-13 14:36:58.000000 desalsim-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7300 2024-05-16 13:59:05.835820 desalsim-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6806 2024-05-16 13:48:24.000000 desalsim-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.813880 desalsim-1.0.2/example/
+-rw-rw-rw-   0        0        0      786 2024-05-16 13:53:14.000000 desalsim-1.0.2/example/__init__.py
+-rw-rw-rw-   0        0        0     4531 2024-05-08 09:04:36.000000 desalsim-1.0.2/example/comparison.py
+-rw-rw-rw-   0        0        0     1888 2024-05-06 15:42:19.000000 desalsim-1.0.2/example/constants.py
+-rw-rw-rw-   0        0        0      468 2024-04-10 15:15:58.000000 desalsim-1.0.2/example/density_calc.py
+-rw-rw-rw-   0        0        0    11995 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/economic_f.py
+-rw-rw-rw-   0        0        0     8681 2024-05-16 13:54:25.000000 desalsim-1.0.2/example/ed_unit_f.py
+-rw-rw-rw-   0        0        0    17109 2024-05-08 08:09:55.000000 desalsim-1.0.2/example/edbm_unit_f.py
+-rw-rw-rw-   0        0        0    49455 2024-05-08 09:52:39.000000 desalsim-1.0.2/example/efc_unit_f.py
+-rw-rw-rw-   0        0        0    33308 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/example_1.py
+-rw-rw-rw-   0        0        0    21717 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/example_2.py
+-rw-rw-rw-   0        0        0     8542 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/med_unit_f.py
+-rw-rw-rw-   0        0        0    14939 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/mfpfr_unit_f.py
+-rw-rw-rw-   0        0        0     9445 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/nanofiltration_unit_f.py
+-rw-rw-rw-   0        0        0     7020 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/ro_unit.py
+-rw-rw-rw-   0        0        0     4409 2024-05-08 07:58:46.000000 desalsim-1.0.2/example/ro_unit_f.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/example/scaleup.py
+-rw-rw-rw-   0        0        0    12280 2024-05-08 08:07:20.000000 desalsim-1.0.2/example/thermal_cryst_f.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:59:05.838813 desalsim-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      829 2024-05-16 13:55:11.000000 desalsim-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:59:05.830835 desalsim-1.0.2/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-08 06:54:08.000000 desalsim-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2060 2024-05-08 12:33:36.000000 desalsim-1.0.2/tests/economic_unittest.py
+-rw-rw-rw-   0        0        0     3249 2024-05-08 12:30:44.000000 desalsim-1.0.2/tests/ed_unittest.py
+-rw-rw-rw-   0        0        0     8395 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/edbm_unittest.py
+-rw-rw-rw-   0        0        0     1564 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/med_unittest.py
+-rw-rw-rw-   0        0        0     2752 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/mfpfr_unittest.py
+-rw-rw-rw-   0        0        0     1786 2024-05-08 07:58:46.000000 desalsim-1.0.2/tests/nanofiltration_unittest.py
+-rw-rw-rw-   0        0        0      347 2023-10-30 09:38:14.000000 desalsim-1.0.2/tests/scaleup.py
+-rw-rw-rw-   0        0        0     4611 2024-05-08 08:01:32.000000 desalsim-1.0.2/tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-1.0.1/DesalSim.egg-info/SOURCES.txt` & `desalsim-1.0.2/DesalSim.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 Desalsim/efc_unit_f.py
 Desalsim/med_unit_f.py
 Desalsim/mfpfr_unit_f.py
 Desalsim/nanofiltration_unit_f.py
 Desalsim/ro_unit_f.py
 Desalsim/scaleup.py
 Desalsim/thermal_cryst_f.py
+desalsim.egg-info/PKG-INFO
+desalsim.egg-info/SOURCES.txt
+desalsim.egg-info/dependency_links.txt
+desalsim.egg-info/requires.txt
+desalsim.egg-info/top_level.txt
 example/__init__.py
 example/comparison.py
 example/constants.py
 example/density_calc.py
 example/economic_f.py
 example/ed_unit_f.py
 example/edbm_unit_f.py
@@ -33,24 +38,15 @@
 example/mfpfr_unit_f.py
 example/nanofiltration_unit_f.py
 example/ro_unit.py
 example/ro_unit_f.py
 example/scaleup.py
 example/thermal_cryst_f.py
 tests/__init__.py
-tests/constants.py
-tests/density_calc.py
-tests/economic_f.py
 tests/economic_unittest.py
-tests/ed_unit_f.py
 tests/ed_unittest.py
-tests/edbm_unit_f.py
 tests/edbm_unittest.py
-tests/med_unit_f.py
 tests/med_unittest.py
-tests/mfpfr_unit_f.py
 tests/mfpfr_unittest.py
-tests/nanofiltration_unit_f.py
 tests/nanofiltration_unittest.py
 tests/scaleup.py
-tests/thermal_cryst_f.py
 tests/thermal_cryst_unittest.py
```

### Comparing `desalsim-1.0.1/Desalsim/__init__.py` & `desalsim-1.0.2/Desalsim/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/constants.py` & `desalsim-1.0.2/Desalsim/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/economic_f.py` & `desalsim-1.0.2/Desalsim/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/ed_unit_f.py` & `desalsim-1.0.2/Desalsim/ed_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/edbm_unit_f.py` & `desalsim-1.0.2/Desalsim/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/efc_unit_f.py` & `desalsim-1.0.2/Desalsim/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/med_unit_f.py` & `desalsim-1.0.2/Desalsim/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/mfpfr_unit_f.py` & `desalsim-1.0.2/Desalsim/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/nanofiltration_unit_f.py` & `desalsim-1.0.2/Desalsim/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/ro_unit_f.py` & `desalsim-1.0.2/Desalsim/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/Desalsim/thermal_cryst_f.py` & `desalsim-1.0.2/Desalsim/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/LICENSE` & `desalsim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/README.md` & `desalsim-1.0.2/DesalSim.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: desalsim
+Version: 1.0.2
+Home-page: https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
+Author: rodoulak
+Author-email: r.ktori@tudelft.nl
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.21.5
+Requires-Dist: pandas==1.4.4
+Requires-Dist: scipy==1.9.1
+Requires-Dist: matplotlib==3.5.2
+Requires-Dist: scikit-learn==1.0.2
+Requires-Dist: plotly>=5.9.0
+Requires-Dist: openpyxl==3.0.10
+
 # DesalSim: Desalination and Brine Treatment simulation model
 
  
 ## Overview 
 This project comprises a package of simulation models for desalination and brine treatment technologies, including reverse osmosis, nanofiltration, multi-effect distillation, chemical precipitation, eutectic freeze crystallization, electrodialysis, and thermal crystallization. These technologies are utilized for desalination, ion separation, and salt recovery processes in various industrial and environmental applications.
 
 The simulation models implemented here calculate various parameters such as salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs. They provide insights into the performance and economics of the technologies under different operating conditions and input parameters. Additionally, the models allow for the integration of different technologies in various configurations to optimize process efficiency and resource utilization.
@@ -17,58 +34,39 @@
 * [Authors and Acknowledgements](#authors-and-acknowledgements)
 * [License](#license)
 
 ## Purpose 
 The purpose of this software suite is to provide researchers, engineers, and policymakers with a powerful tool for evaluating the performance and economics of desalination and brine treatment systems. By integrating technical process models with economic and environmental analyses, the suite enables users to make informed decisions about technology integration, process optimization, and resource management.
 
 
-## Key features 
-- Simulation models for various desalination and brine treatment technologies
-- Analysis of salt concentration profiles, ion fluxes, energy consumption, and chemical usage
-- Integration of different technologies to optimize process efficiency and resource utilization
-- Economic models for technologies and integrated systems 
-- Output visualization and data export for further analysis 
-
-### File Descriptions
-
-Here is a brief overview of each file in the project:
-
-- `README.md`: This README file providing an overview of the project, usage instructions, and other details.
-- `nanofiltration_unit_f.py`: This file contains the main script for running the simulation model of Nanofiltration (NF) unit.
-- `ro_unit.py`: This file contains the main script for running the simulation model of Reverse Osmosis (RO) unit.
-- `med_unit_f.py`: This file contains the main script for running the simulation model of Multi-effect distillation (MED) unit.
-- `mfpfr_unit.py`: This file contains the main script for running the simulation model of Multiple Feed Plug Flow Reactor (MF-PFR) unit.
-- `economic_f.py`: This file contains the main script for running the economic model of a technology or a system of technologies.
-- `ed_unit_f.py`: This file contains the main script for running the simulation model of Electrodialysis (ED) unit.
-- `edbm_unit_f.py`: This file contains the main script for running the simulation model of Electrodialysis With Bipolar Membranes (EDBM) unit.
-- `efc_unit_f.py`: This file contains the main script for running the simulation model of Eutectic freeze crystallization (EFC) unit.
-- `thermal_cryst_unit_f.py`: This file contains the main script for running the simulation model of Thermal crystallizer (Tcr) unit.
-- `example1.py`: Example script demonstrating the usage of the simulation suite for a specific treatment chain.
-- `example2.py`: Another example script showcasing a different treatment chain simulation.
-- `comparison.py`: Script for results intrepetation. It compares the results of example1 and example2 simulations.
-- `constants.py`: This file contains the main script for input contant parameters.
-- `density_calc.py`: This file contains the main script for calculating density of a solution based on the tempretaure and the concentration of the solution.
-- `scaleup.py`: This file contains the main script for scaling-up a technology with known capacity using the six-tenths factor rule (m=0.6).
-- `LICENSE`: License file containing the MIT License terms.
-
 ## Installation  
 The easiest way is through pip, in command-line interface:   
 ```
-pip install DesalSim==1.0.1
+pip install desalsim==1.0.2
 ```
 
 If you want to install the latest GitHub verstion:
 1. Download the repository to your local machine:
 ```
 https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-
 ```
 2. Install the required dependencies:
  ```
 pip install -r requirements.txt
  ```
+## Key features 
+- Simulation models for various desalination and brine treatment technologies
+- Analysis of salt concentration profiles, ion fluxes, energy consumption, and chemical usage
+- Integration of different technologies to optimize process efficiency and resource utilization
+- Economic models for technologies and integrated systems 
+- Output visualization and data export for further analysis 
+
+### File Descriptions
+
+A brief overview of each file in the project can be found in (https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/file-description). 
 
 ## Usage 
 Each simulation model serves as a standalone tool for analyzing the performance of a specific desalination or brine treatment technology. Before running the simulation, ensure that you have provided the necessary input parameters, such as feed flow rates, salinity levels, membrane properties, heat sources, and operating conditions.
 
 The simulation results, including salt concentration profiles, ion fluxes, energy consumption, chemical consumption, and operational costs, will be generated based on the specified inputs and displayed in the console output or saved to output files for further analysis.
 
 However, simulation models of more than one technology can be combined to simulate and evaluate the performance of a treatment chain (desalination and brine treatment system). In this case, the output flow rates and stream concentrate are the input data for the next technology. 
@@ -76,24 +74,15 @@
 Additionally, two example files are provided to demonstrate the usage of the simulation suite (see [Example Folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example), [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py) and [Example 2](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_2.py)). These examples simulate and evaluate two different treatment chains, showcasing the integration of multiple technologies. The economic evaluation of the treatment chain is given in [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py) and in the [Economic Tutorial](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Economic_Tutorial.md). 
 
 Furthermore, a [comparison file](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/comparison.py) is included, where the results of the two examples are compared in terms of various parameters. Users can extend this comparison by adding more indicators as needed.
 
 For more details on input/output parameters and assumption see [Link to Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md).
 
 ### Documentation 
-You can find Tutorials and documents at: 
-1. [Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md)
-2. [Tutorial for Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Example_1_Tutorial.md)
-3. [Economic Tutorial](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Economic_Tutorial.md)
-4. The mathematical description of each technology is given in [Mathematical description](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/paper/Mathematical_description.pdf)
-5. [Example 1](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_1.py)
-6. [Example 2](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/example_2.py)
-7. [Scenarios comparison](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/comparison.py)
-
-Additionally, you can find tests for every process unit and the economic model in the [tests folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/tests) that verify that the code is running properly. 
+You can find Tutorials and documents at [Tutorial File](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/example/Tutorial.md). Additionally, you can find tests for every process unit and the economic model in the [tests folder](https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-/tree/main/tests) that verify that the code is running properly. 
 
 
 ## Contributing
 Contributions to the project are welcome! If you'd like to contribute, please follow the standard GitHub workflow:
 1. Fork the repository.
 2. Create a new branch (git checkout -b feature/improvement).
 3. Make your changes and commit them (git commit -am 'Add new feature').
```

### Comparing `desalsim-1.0.1/example/__init__.py` & `desalsim-1.0.2/example/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # __init__.py
-from Desalsim import density_calc
-from Desalsim import constants
+from desalsim import density_calc
+from desalsim import constants
 
-from Desalsim.nanofiltration_unit_f import NFMass
-from Desalsim.nanofiltration_unit_f import OsmoticPressure
-from Desalsim.nanofiltration_unit_f import NfEnergy
+from desalsim.nanofiltration_unit_f import NFMass
+from desalsim.nanofiltration_unit_f import OsmoticPressure
+from desalsim.nanofiltration_unit_f import NfEnergy
 
-from Desalsim.med_unit_f import MEDCalculator
+from desalsim.med_unit_f import MEDCalculator
 
-from Desalsim.thermal_cryst_f import thermal_calc
-from Desalsim.thermal_cryst_f import conc_cal
-from Desalsim.thermal_cryst_f import calculate_energy
+from desalsim.thermal_cryst_f import thermal_calc
+from desalsim.thermal_cryst_f import conc_cal
+from desalsim.thermal_cryst_f import calculate_energy
 
-from Desalsim.mfpfr_unit_f import MFPFRCALC
-from Desalsim.mfpfr_unit_f import HClAddition
-from Desalsim.mfpfr_unit_f import energycons
+from desalsim.mfpfr_unit_f import MFPFRCALC
+from desalsim.mfpfr_unit_f import HClAddition
+from desalsim.mfpfr_unit_f import energycons
 
-from Desalsim.ed_unit_f import ElectrodialysisCalc
+from desalsim.ed_unit_f import ElectrodialysisCalc
 
-from Desalsim.edbm_unit_f import EDBMCalc
+from desalsim.edbm_unit_f import EDBMCalc
 
-from Desalsim.economic_f import econom
-from Desalsim.economic_f import revenue
+from desalsim.economic_f import econom
+from desalsim.economic_f import revenue
```

### Comparing `desalsim-1.0.1/example/comparison.py` & `desalsim-1.0.2/example/comparison.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/constants.py` & `desalsim-1.0.2/example/constants.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/economic_f.py` & `desalsim-1.0.2/example/economic_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/ed_unit_f.py` & `desalsim-1.0.2/example/ed_unit_f.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import math
-from Desalsim.density_calc import density_calc 
-from Desalsim import constants 
-from Desalsim import scaleup
+from desalsim.density_calc import density_calc 
+from desalsim import constants 
+from desalsim import scaleup
 
 #%% Calculations 
 """
 A class used to represent Mass Balance for Electrodialysis
 
 ...
```

### Comparing `desalsim-1.0.1/example/edbm_unit_f.py` & `desalsim-1.0.2/example/edbm_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/efc_unit_f.py` & `desalsim-1.0.2/example/efc_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/example_1.py` & `desalsim-1.0.2/example/example_1.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/example_2.py` & `desalsim-1.0.2/example/example_2.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/med_unit_f.py` & `desalsim-1.0.2/example/med_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/mfpfr_unit_f.py` & `desalsim-1.0.2/example/mfpfr_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/nanofiltration_unit_f.py` & `desalsim-1.0.2/example/nanofiltration_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/ro_unit.py` & `desalsim-1.0.2/example/ro_unit.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/ro_unit_f.py` & `desalsim-1.0.2/example/ro_unit_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/example/thermal_cryst_f.py` & `desalsim-1.0.2/example/thermal_cryst_f.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/setup.py` & `desalsim-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f: 
     description =f.read()
 
 setup(
-      name='DesalSim',
-      version='1.0.1',
+      name='desalsim',
+      version='1.0.2',
       packages=find_packages(),
       url="https://github.com/rodoulak/Desalination-and-Brine-Treatment-Simulation-",
       author="rodoulak",
       author_email="r.ktori@tudelft.nl",
       license="MIT",
       install_requires=[
-          "numpy>=1.0",
-          "pandas>=1.0",  # Include pandas as a dependency
-          "scipy>=1.0", # For figures 
-          "matplotlib>=1.0", # For figures 
-          "scikit-learn>=1.0",
-          "plotly>=1.0", 
-          "openpyxl>=1.0",  #read data from excel file
+          "numpy==1.21.5",
+          "pandas==1.4.4",  # Include pandas as a dependency
+          "scipy==1.9.1", # For figures 
+          "matplotlib==3.5.2", # For figures 
+          "scikit-learn==1.0.2",
+          "plotly>=5.9.0", 
+          "openpyxl==3.0.10",  #read data from excel file
       ],
       long_description= description,
       long_description_content_type="text/markdown",
       )
```

### Comparing `desalsim-1.0.1/tests/__init__.py` & `desalsim-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/economic_unittest.py` & `desalsim-1.0.2/tests/economic_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/ed_unittest.py` & `desalsim-1.0.2/tests/ed_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/edbm_unittest.py` & `desalsim-1.0.2/tests/edbm_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/med_unittest.py` & `desalsim-1.0.2/tests/med_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/mfpfr_unittest.py` & `desalsim-1.0.2/tests/mfpfr_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/nanofiltration_unittest.py` & `desalsim-1.0.2/tests/nanofiltration_unittest.py`

 * *Files identical despite different names*

### Comparing `desalsim-1.0.1/tests/thermal_cryst_unittest.py` & `desalsim-1.0.2/tests/thermal_cryst_unittest.py`

 * *Files identical despite different names*

