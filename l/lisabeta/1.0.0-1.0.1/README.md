# Comparing `tmp/lisabeta-1.0.0.tar.gz` & `tmp/lisabeta-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisabeta-1.0.0.tar", last modified: Thu May 16 13:36:52 2024, max compression
+gzip compressed data, was "lisabeta-1.0.1.tar", last modified: Thu May 16 16:41:58 2024, max compression
```

## Comparing `lisabeta-1.0.0.tar` & `lisabeta-1.0.1.tar`

### file list

```diff
@@ -1,85 +1,110 @@
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.583000 lisabeta-1.0.0/
--rw-r--r--   0 maude     (1000) maude     (1000)      132 2024-05-16 13:36:52.583000 lisabeta-1.0.0/PKG-INFO
--rw-rw-r--   0 maude     (1000) maude     (1000)     2099 2023-11-06 19:47:55.000000 lisabeta-1.0.0/README.md
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.555000 lisabeta-1.0.0/lisabeta/
--rw-rw-r--   0 maude     (1000) maude     (1000)      360 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     5853 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/constants.h
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.559000 lisabeta-1.0.0/lisabeta/inference/
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    16662 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/inference.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     6712 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/multiemcee.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    20934 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/multiemcee_smbh.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    34846 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/ptemcee_smbh.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    19683 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/ptemcee_sobh.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    20629 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/ptemcee_sobh_agn.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     7324 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/pymultinest_lvk.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     8988 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/pymultinest_multiband.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     9826 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/pymultinest_smbh.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     8529 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/inference/pymultinest_sobh.py
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.567000 lisabeta-1.0.0/lisabeta/lisa/
--rw-rw-r--   0 maude     (1000) maude     (1000)    18703 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAgeometry.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     7291 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAgeometry.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    27026 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAnoise.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     6605 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAnoise.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    22142 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAresponse.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     6406 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/LISAresponse.h
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    12753 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/ldcnoise.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     9382 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/ldctools.py
--rw-rw-r--   0 maude     (1000) maude     (1000)   103711 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/lisa.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    24863 2024-05-16 11:37:19.000000 lisabeta-1.0.0/lisabeta/lisa/lisa_fisher.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    31973 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/lisatools.py
--rw-rw-r--   0 maude     (1000) maude     (1000)   561123 2024-05-16 13:36:43.000000 lisabeta-1.0.0/lisabeta/lisa/pyLISAnoise.c
--rw-rw-r--   0 maude     (1000) maude     (1000)  1176306 2024-05-16 13:36:44.000000 lisabeta-1.0.0/lisabeta/lisa/pyresponse.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    13649 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/lisa/snrtools.py
--rw-rw-r--   0 maude     (1000) maude     (1000)   217173 2024-05-16 13:36:44.000000 lisabeta-1.0.0/lisabeta/pyconstants.c
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.567000 lisabeta-1.0.0/lisabeta/struct/
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/struct/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)   281600 2024-05-16 13:36:44.000000 lisabeta-1.0.0/lisabeta/struct/pystruct.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    24959 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/struct/struct.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    12890 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/struct/struct.h
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.571000 lisabeta-1.0.0/lisabeta/tools/
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    15273 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/fresnel.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    19867 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/overlap.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     4399 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/overlap.h
--rw-rw-r--   0 maude     (1000) maude     (1000)   875345 2024-05-16 13:36:44.000000 lisabeta-1.0.0/lisabeta/tools/pyoverlap.c
--rw-rw-r--   0 maude     (1000) maude     (1000)  1189894 2024-05-16 13:36:46.000000 lisabeta-1.0.0/lisabeta/tools/pyspline.c
--rw-rw-r--   0 maude     (1000) maude     (1000)  2290098 2024-05-16 13:36:47.000000 lisabeta-1.0.0/lisabeta/tools/pytools.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    28802 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/spline.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     7365 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/spline.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    23848 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/tools.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     5394 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/tools/tools.h
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.571000 lisabeta-1.0.0/lisabeta/utils/
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/utils/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    37013 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/utils/corner_covar.py
--rw-rw-r--   0 maude     (1000) maude     (1000)    33824 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/utils/plotutils.py
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.575000 lisabeta-1.0.0/lisabeta/waveforms/
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/__init__.py
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.583000 lisabeta-1.0.0/lisabeta/waveforms/bbh/
--rw-rw-r--   0 maude     (1000) maude     (1000)    49447 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROM.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     5683 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROM.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    11074 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    71720 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     6942 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    60005 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD_internals.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    53455 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD_internals.h
--rw-rw-r--   0 maude     (1000) maude     (1000)    92583 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomHM.c
--rw-rw-r--   0 maude     (1000) maude     (1000)    15683 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomHM.h
--rw-rw-r--   0 maude     (1000) maude     (1000)     4209 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomInternalUtils.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     2121 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomUtils.c
--rw-rw-r--   0 maude     (1000) maude     (1000)     7992 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/RingdownCW.c
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/__init__.py
--rw-rw-r--   0 maude     (1000) maude     (1000)   961505 2024-05-16 13:36:48.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/pyEOBNRv2HMROM.c
--rw-rw-r--   0 maude     (1000) maude     (1000)  1085974 2024-05-16 13:36:49.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/pyIMRPhenomD.c
--rw-rw-r--   0 maude     (1000) maude     (1000)  1099966 2024-05-16 13:36:51.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/pyIMRPhenomHM.c
--rw-rw-r--   0 maude     (1000) maude     (1000)      930 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/setup.py
--rw-rw-r--   0 maude     (1000) maude     (1000)     9960 2023-11-06 19:47:55.000000 lisabeta-1.0.0/lisabeta/waveforms/bbh/tf2.py
-drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 13:36:52.583000 lisabeta-1.0.0/lisabeta.egg-info/
--rw-r--r--   0 maude     (1000) maude     (1000)      132 2024-05-16 13:36:52.000000 lisabeta-1.0.0/lisabeta.egg-info/PKG-INFO
--rw-rw-r--   0 maude     (1000) maude     (1000)     2226 2024-05-16 13:36:52.000000 lisabeta-1.0.0/lisabeta.egg-info/SOURCES.txt
--rw-rw-r--   0 maude     (1000) maude     (1000)        1 2024-05-16 13:36:52.000000 lisabeta-1.0.0/lisabeta.egg-info/dependency_links.txt
--rw-rw-r--   0 maude     (1000) maude     (1000)        9 2024-05-16 13:36:52.000000 lisabeta-1.0.0/lisabeta.egg-info/top_level.txt
--rw-rw-r--   0 maude     (1000) maude     (1000)      192 2024-05-16 13:36:33.000000 lisabeta-1.0.0/pyproject.toml
--rw-rw-r--   0 maude     (1000) maude     (1000)       38 2024-05-16 13:36:52.583000 lisabeta-1.0.0/setup.cfg
--rw-rw-r--   0 maude     (1000) maude     (1000)    11749 2023-11-06 19:47:55.000000 lisabeta-1.0.0/setup.py
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.217058 lisabeta-1.0.1/
+-rw-rw-r--   0 maude     (1000) maude     (1000)       79 2024-05-16 16:41:38.000000 lisabeta-1.0.1/MANIFEST.in
+-rw-r--r--   0 maude     (1000) maude     (1000)      132 2024-05-16 16:41:58.217058 lisabeta-1.0.1/PKG-INFO
+-rw-rw-r--   0 maude     (1000) maude     (1000)     2099 2023-11-06 19:47:55.000000 lisabeta-1.0.1/README.md
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.197059 lisabeta-1.0.1/lisabeta/
+-rw-rw-r--   0 maude     (1000) maude     (1000)      360 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     5853 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/constants.h
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.197059 lisabeta-1.0.1/lisabeta/inference/
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    16662 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/inference.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6712 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/multiemcee.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    20934 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/multiemcee_smbh.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    34846 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/ptemcee_smbh.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    19683 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/ptemcee_sobh.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    20629 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/ptemcee_sobh_agn.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     7324 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/pymultinest_lvk.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     8988 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/pymultinest_multiband.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     9826 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/pymultinest_smbh.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     8529 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/inference/pymultinest_sobh.py
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.201059 lisabeta-1.0.1/lisabeta/lisa/
+-rw-rw-r--   0 maude     (1000) maude     (1000)    18703 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAgeometry.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     7291 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAgeometry.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    27026 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAnoise.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6605 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAnoise.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    22142 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAresponse.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6406 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/LISAresponse.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    12753 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/ldcnoise.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     9382 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/ldctools.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)   103711 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/lisa.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    24863 2024-05-16 11:37:19.000000 lisabeta-1.0.1/lisabeta/lisa/lisa_fisher.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    31973 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/lisatools.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)   561123 2024-05-16 16:41:48.000000 lisabeta-1.0.1/lisabeta/lisa/pyLISAnoise.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     5089 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/pyLISAnoise.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)    11672 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/pyLISAnoise.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)  1176306 2024-05-16 16:41:49.000000 lisabeta-1.0.1/lisabeta/lisa/pyresponse.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1319 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/pyresponse.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)    12319 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/pyresponse.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)    13649 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/lisa/snrtools.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)   217173 2024-05-16 16:41:50.000000 lisabeta-1.0.1/lisabeta/pyconstants.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1066 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/pyconstants.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)      783 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/pyconstants.pyx
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.201059 lisabeta-1.0.1/lisabeta/struct/
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/struct/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)   281600 2024-05-16 16:41:50.000000 lisabeta-1.0.1/lisabeta/struct/pystruct.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     4533 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/struct/pystruct.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)      428 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/struct/pystruct.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)    24959 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/struct/struct.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)    12890 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/struct/struct.h
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.209058 lisabeta-1.0.1/lisabeta/tools/
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    15273 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/fresnel.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1650 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/fresnel.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    19867 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/overlap.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     4399 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/overlap.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)   875345 2024-05-16 16:41:50.000000 lisabeta-1.0.1/lisabeta/tools/pyoverlap.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)      874 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pyoverlap.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)    35139 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pyoverlap.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)  1189894 2024-05-16 16:41:52.000000 lisabeta-1.0.1/lisabeta/tools/pyspline.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1389 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pyspline.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)    19696 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pyspline.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)  2290098 2024-05-16 16:41:53.000000 lisabeta-1.0.1/lisabeta/tools/pytools.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1570 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pytools.pxd
+-rw-rw-r--   0 maude     (1000) maude     (1000)    42620 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/pytools.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)     3769 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/referenceframes.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)      871 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/referenceframes.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    28802 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/spline.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     7365 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/spline.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    23848 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/tools.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     5394 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/tools/tools.h
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.209058 lisabeta-1.0.1/lisabeta/utils/
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/utils/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    37013 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/utils/corner_covar.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)    33824 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/utils/plotutils.py
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.209058 lisabeta-1.0.1/lisabeta/waveforms/
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/__init__.py
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.217058 lisabeta-1.0.1/lisabeta/waveforms/bbh/
+-rw-rw-r--   0 maude     (1000) maude     (1000)    49447 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROM.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     5683 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROM.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    11074 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6529 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    71720 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6942 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    60005 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD_internals.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)    53455 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD_internals.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)    92583 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomHM.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)    15683 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomHM.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)     4209 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomInternalUtils.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)      669 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomInternalUtils.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)     2121 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomUtils.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)      512 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomUtils.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)     7992 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/RingdownCW.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     1940 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/RingdownCW.h
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/__init__.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)   961505 2024-05-16 16:41:54.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyEOBNRv2HMROM.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)     6519 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyEOBNRv2HMROM.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)  1085974 2024-05-16 16:41:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomD.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)    20392 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomD.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)  1099966 2024-05-16 16:41:56.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomHM.c
+-rw-rw-r--   0 maude     (1000) maude     (1000)    25178 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomHM.pyx
+-rw-rw-r--   0 maude     (1000) maude     (1000)      930 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/setup.py
+-rw-rw-r--   0 maude     (1000) maude     (1000)     9960 2023-11-06 19:47:55.000000 lisabeta-1.0.1/lisabeta/waveforms/bbh/tf2.py
+drwxrwxr-x   0 maude     (1000) maude     (1000)        0 2024-05-16 16:41:58.217058 lisabeta-1.0.1/lisabeta.egg-info/
+-rw-r--r--   0 maude     (1000) maude     (1000)      132 2024-05-16 16:41:58.000000 lisabeta-1.0.1/lisabeta.egg-info/PKG-INFO
+-rw-rw-r--   0 maude     (1000) maude     (1000)     3014 2024-05-16 16:41:58.000000 lisabeta-1.0.1/lisabeta.egg-info/SOURCES.txt
+-rw-rw-r--   0 maude     (1000) maude     (1000)        1 2024-05-16 16:41:58.000000 lisabeta-1.0.1/lisabeta.egg-info/dependency_links.txt
+-rw-rw-r--   0 maude     (1000) maude     (1000)        9 2024-05-16 16:41:58.000000 lisabeta-1.0.1/lisabeta.egg-info/top_level.txt
+-rw-rw-r--   0 maude     (1000) maude     (1000)      192 2024-05-16 16:41:22.000000 lisabeta-1.0.1/pyproject.toml
+-rw-rw-r--   0 maude     (1000) maude     (1000)       38 2024-05-16 16:41:58.217058 lisabeta-1.0.1/setup.cfg
+-rw-rw-r--   0 maude     (1000) maude     (1000)    11749 2023-11-06 19:47:55.000000 lisabeta-1.0.1/setup.py
```

### Comparing `lisabeta-1.0.0/README.md` & `lisabeta-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/constants.h` & `lisabeta-1.0.1/lisabeta/constants.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/inference.py` & `lisabeta-1.0.1/lisabeta/inference/inference.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/multiemcee.py` & `lisabeta-1.0.1/lisabeta/inference/multiemcee.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/multiemcee_smbh.py` & `lisabeta-1.0.1/lisabeta/inference/multiemcee_smbh.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/ptemcee_smbh.py` & `lisabeta-1.0.1/lisabeta/inference/ptemcee_smbh.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/ptemcee_sobh.py` & `lisabeta-1.0.1/lisabeta/inference/ptemcee_sobh.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/ptemcee_sobh_agn.py` & `lisabeta-1.0.1/lisabeta/inference/ptemcee_sobh_agn.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/pymultinest_lvk.py` & `lisabeta-1.0.1/lisabeta/inference/pymultinest_lvk.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/pymultinest_multiband.py` & `lisabeta-1.0.1/lisabeta/inference/pymultinest_multiband.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/pymultinest_smbh.py` & `lisabeta-1.0.1/lisabeta/inference/pymultinest_smbh.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/inference/pymultinest_sobh.py` & `lisabeta-1.0.1/lisabeta/inference/pymultinest_sobh.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAgeometry.c` & `lisabeta-1.0.1/lisabeta/lisa/LISAgeometry.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAgeometry.h` & `lisabeta-1.0.1/lisabeta/lisa/LISAgeometry.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAnoise.c` & `lisabeta-1.0.1/lisabeta/lisa/LISAnoise.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAnoise.h` & `lisabeta-1.0.1/lisabeta/lisa/LISAnoise.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAresponse.c` & `lisabeta-1.0.1/lisabeta/lisa/LISAresponse.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/LISAresponse.h` & `lisabeta-1.0.1/lisabeta/lisa/LISAresponse.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/ldcnoise.py` & `lisabeta-1.0.1/lisabeta/lisa/ldcnoise.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/ldctools.py` & `lisabeta-1.0.1/lisabeta/lisa/ldctools.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/lisa.py` & `lisabeta-1.0.1/lisabeta/lisa/lisa.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/lisa_fisher.py` & `lisabeta-1.0.1/lisabeta/lisa/lisa_fisher.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/lisatools.py` & `lisabeta-1.0.1/lisabeta/lisa/lisatools.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/lisa/pyLISAnoise.c` & `lisabeta-1.0.1/lisabeta/lisa/pyLISAnoise.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/lisa/LISAgeometry.h",
             "lisabeta/lisa/LISAnoise.h",
             "lisabeta/lisa/LISAresponse.h",
             "lisabeta/struct/struct.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/lisa",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
+            "lisabeta/struct",
+            "./lisabeta/struct",
             "./lisabeta/lisa",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools"
         ],
         "language": "c",
         "libraries": [
             "gsl",
@@ -1075,177 +1075,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1275,42 +1275,42 @@
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 struct __pyx_obj_8lisabeta_4lisa_11pyLISAnoise_LISANoisePSDFunction;
 struct __pyx_obj_8lisabeta_4lisa_11pyLISAnoise_LISANoisePSDFunction3Chan;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6717,15 +6717,15 @@
   __Pyx_XDECREF(__pyx_v_Sn3_vals);
   __Pyx_XDECREF(__pyx_v_Sndata);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6734,29 +6734,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6767,15 +6767,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6784,29 +6784,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6817,15 +6817,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6834,29 +6834,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6867,15 +6867,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6884,29 +6884,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6917,15 +6917,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6934,29 +6934,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6967,89 +6967,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7057,33 +7057,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7091,96 +7091,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7196,15 +7196,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7212,53 +7212,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -7266,30 +7266,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7304,15 +7304,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7328,15 +7328,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7344,53 +7344,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -7398,30 +7398,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7436,15 +7436,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7460,15 +7460,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7476,53 +7476,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -7530,30 +7530,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7568,176 +7568,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8220,26 +8220,26 @@
  *         Sn1_splineClass = pyspline.CubicSpline(freq_Sn, Sn1_data)
  *         Sn2_splineClass = pyspline.CubicSpline(freq_Sn, Sn2_data)
  */
   __pyx_tuple__16 = PyTuple_Pack(2, __pyx_slice__12, __pyx_int_3); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(2, 948, __pyx_L1_error)
@@ -9169,15 +9169,15 @@
  * #
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `lisabeta-1.0.0/lisabeta/lisa/pyresponse.c` & `lisabeta-1.0.1/lisabeta/lisa/pyresponse.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/lisa/LISAgeometry.h",
             "lisabeta/lisa/LISAresponse.h",
             "lisabeta/struct/struct.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/lisa",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "lisabeta/struct",
+            "./lisabeta/struct",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools"
         ],
         "language": "c",
         "libraries": [
             "gsl",
@@ -1146,177 +1146,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1349,42 +1349,42 @@
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 struct __pyx_obj_8lisabeta_4lisa_10pyresponse_LISAFDresponseTDI3Chan;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -7335,15 +7335,15 @@
   __Pyx_XDECREF(__pyx_v_d0_shapiro);
   __Pyx_XDECREF(__pyx_v_td);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7352,29 +7352,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7385,15 +7385,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7402,29 +7402,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7435,15 +7435,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7452,29 +7452,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7485,15 +7485,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7502,29 +7502,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7535,15 +7535,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7552,29 +7552,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7585,89 +7585,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7675,33 +7675,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7709,96 +7709,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7814,15 +7814,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7830,53 +7830,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -7884,30 +7884,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7922,15 +7922,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7946,15 +7946,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7962,53 +7962,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -8016,30 +8016,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8054,15 +8054,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8078,15 +8078,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8094,53 +8094,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -8148,30 +8148,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8186,176 +8186,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23084,26 +23084,26 @@
  *     spline_amp = spline_ampClass.get_spline()
  *     spline_phi = spline_phiClass.get_spline()
  */
   __pyx_tuple__11 = PyTuple_Pack(2, __pyx_slice__8, __pyx_int_2); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/lisa/snrtools.py` & `lisabeta-1.0.1/lisabeta/lisa/snrtools.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/pyconstants.c` & `lisabeta-1.0.1/lisabeta/pyconstants.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/struct",
             "lisabeta/tools",
             "lisabeta/lisa"
         ],
         "language": "c",
@@ -1025,177 +1025,177 @@
 
 static const char *__pyx_f[] = {
   "__init__.pxd",
   "lisabeta/pyconstants.pyx",
   "type.pxd",
 };
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1222,42 +1222,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1752,15 +1752,15 @@
 static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 /* Late includes */
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -1769,29 +1769,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -1802,15 +1802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -1819,29 +1819,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -1852,15 +1852,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -1869,29 +1869,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -1902,15 +1902,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -1919,29 +1919,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -1952,15 +1952,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -1969,29 +1969,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2002,89 +2002,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2092,33 +2092,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2126,96 +2126,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2231,15 +2231,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2247,53 +2247,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 942, __pyx_L5_except_error)
@@ -2301,30 +2301,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2339,15 +2339,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2363,15 +2363,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2379,53 +2379,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 948, __pyx_L5_except_error)
@@ -2433,30 +2433,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2471,15 +2471,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2495,15 +2495,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2511,53 +2511,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 954, __pyx_L5_except_error)
@@ -2565,30 +2565,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2603,176 +2603,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -2875,26 +2875,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 948, __pyx_L1_error)
@@ -3608,15 +3608,15 @@
  * #
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `lisabeta-1.0.0/lisabeta/struct/pystruct.c` & `lisabeta-1.0.1/lisabeta/struct/pystruct.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/struct/struct.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/struct",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
@@ -1061,177 +1061,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1259,42 +1259,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2503,15 +2503,15 @@
   __Pyx_AddTraceback("lisabeta.struct.pystruct.py_object_function.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2520,29 +2520,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2553,15 +2553,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2570,29 +2570,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2603,15 +2603,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2620,29 +2620,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2653,15 +2653,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2670,29 +2670,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2703,15 +2703,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2720,29 +2720,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2753,89 +2753,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2843,33 +2843,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -2877,96 +2877,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2982,15 +2982,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2998,53 +2998,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -3052,30 +3052,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3090,15 +3090,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3114,15 +3114,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3130,53 +3130,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -3184,30 +3184,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3222,15 +3222,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3246,15 +3246,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3262,53 +3262,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -3316,30 +3316,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3354,176 +3354,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3736,26 +3736,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.obfn cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_self_obfn_cannot_be_converted_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 948, __pyx_L1_error)
@@ -4143,15 +4143,15 @@
  *     raise TypeError("self.obfn cannot be converted to a Python object for pickling")
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `lisabeta-1.0.0/lisabeta/struct/struct.c` & `lisabeta-1.0.1/lisabeta/struct/struct.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/struct/struct.h` & `lisabeta-1.0.1/lisabeta/struct/struct.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/fresnel.c` & `lisabeta-1.0.1/lisabeta/tools/fresnel.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/overlap.c` & `lisabeta-1.0.1/lisabeta/tools/overlap.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/overlap.h` & `lisabeta-1.0.1/lisabeta/tools/overlap.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/pyoverlap.c` & `lisabeta-1.0.1/lisabeta/tools/pyoverlap.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/tools/overlap.h",
             "lisabeta/tools/spline.h"
         ],
         "extra_compile_args": [
             "-std=c99"
@@ -20,15 +20,15 @@
         "include_dirs": [
             "lisabeta/tools",
             "lisabeta/struct",
             "./lisabeta/struct",
             "./lisabeta/tools",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
             "gsl",
@@ -1075,177 +1075,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1273,42 +1273,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -13674,15 +13674,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13691,29 +13691,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -13724,15 +13724,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13741,29 +13741,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -13774,15 +13774,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13791,29 +13791,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -13824,15 +13824,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13841,29 +13841,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -13874,15 +13874,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13891,29 +13891,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -13924,89 +13924,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -14014,33 +14014,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -14048,96 +14048,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14153,15 +14153,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -14169,53 +14169,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -14223,30 +14223,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -14261,15 +14261,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14285,15 +14285,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14301,53 +14301,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -14355,30 +14355,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14393,15 +14393,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14417,15 +14417,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -14433,53 +14433,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -14487,30 +14487,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -14525,176 +14525,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -15025,26 +15025,26 @@
  *     return overlap
  * 
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Type_of_brute_force_overlap_not); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 948, __pyx_L1_error)
@@ -15565,15 +15565,15 @@
  * #
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `lisabeta-1.0.0/lisabeta/tools/pyspline.c` & `lisabeta-1.0.1/lisabeta/tools/pyspline.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/tools/spline.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/tools",
             "lisabeta/struct",
             "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
             "gsl",
@@ -1142,177 +1142,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1346,42 +1346,42 @@
 struct __pyx_obj_8lisabeta_5tools_8pyspline_CubicSpline;
 struct __pyx_obj_8lisabeta_5tools_8pyspline_QuadSpline;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -9223,15 +9223,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_xold.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9240,29 +9240,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -9273,15 +9273,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9290,29 +9290,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -9323,15 +9323,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9340,29 +9340,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -9373,15 +9373,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9390,29 +9390,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -9423,15 +9423,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9440,29 +9440,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -9473,89 +9473,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9563,33 +9563,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -9597,96 +9597,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9702,15 +9702,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -9718,53 +9718,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -9772,30 +9772,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -9810,15 +9810,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9834,15 +9834,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9850,53 +9850,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -9904,30 +9904,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9942,15 +9942,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -9966,15 +9966,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -9982,53 +9982,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -10036,30 +10036,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -10074,176 +10074,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25085,26 +25085,26 @@
  * 
  *     # Cast C double array to numpy via a MemoryView
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Call_to_EvalQuadSplineOnVector_f); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/tools/pytools.c` & `lisabeta-1.0.1/lisabeta/tools/pytools.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/tools/tools.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/tools",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "lisabeta/struct",
+            "./lisabeta/struct",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
             "gsl",
@@ -1142,177 +1142,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1348,42 +1348,42 @@
 struct __pyx_obj_8lisabeta_5tools_7pytools_FrequencyGrid;
 struct __pyx_obj_8lisabeta_5tools_7pytools_MergeGrids;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -29017,15 +29017,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_w2.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -29034,29 +29034,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -29067,15 +29067,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -29084,29 +29084,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -29117,15 +29117,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -29134,29 +29134,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -29167,15 +29167,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -29184,29 +29184,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -29217,15 +29217,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -29234,29 +29234,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -29267,89 +29267,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -29357,33 +29357,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -29391,96 +29391,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -29496,15 +29496,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -29512,53 +29512,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -29566,30 +29566,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -29604,15 +29604,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -29628,15 +29628,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -29644,53 +29644,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -29698,30 +29698,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -29736,15 +29736,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -29760,15 +29760,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -29776,53 +29776,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -29830,30 +29830,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -29868,176 +29868,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -45698,26 +45698,26 @@
  *     cdef double complex* alpha0_data = <double complex *> &alpha0[0,0,0]
  *     Calpha0 = complex_array_3d_view(alpha0_data, alpha0.shape[0],
  */
   __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_Input_numpy_array_w2_is_not_C_CO); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 1043, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__36);
   __Pyx_GIVEREF(__pyx_tuple__36);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/tools/spline.c` & `lisabeta-1.0.1/lisabeta/tools/spline.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/spline.h` & `lisabeta-1.0.1/lisabeta/tools/spline.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/tools.c` & `lisabeta-1.0.1/lisabeta/tools/tools.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/tools/tools.h` & `lisabeta-1.0.1/lisabeta/tools/tools.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/utils/corner_covar.py` & `lisabeta-1.0.1/lisabeta/utils/corner_covar.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/utils/plotutils.py` & `lisabeta-1.0.1/lisabeta/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROM.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROM.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROM.h` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROM.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD.h` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD_internals.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD_internals.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomD_internals.h` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomD_internals.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomHM.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomHM.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomHM.h` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomHM.h`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomInternalUtils.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomInternalUtils.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/IMRPhenomUtils.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/IMRPhenomUtils.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/RingdownCW.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/RingdownCW.c`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/pyEOBNRv2HMROM.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/pyEOBNRv2HMROM.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/waveforms/bbh/EOBNRv2HMROM.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/waveforms/bbh",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "lisabeta/struct",
+            "./lisabeta/struct",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
@@ -1143,177 +1143,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1346,42 +1346,42 @@
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 struct __pyx_obj_8lisabeta_9waveforms_3bbh_14pyEOBNRv2HMROM_EOBNRv2HMROM;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4441,15 +4441,15 @@
   __Pyx_AddTraceback("lisabeta.waveforms.bbh.pyEOBNRv2HMROM.EOBNRv2HMROM.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4458,29 +4458,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4491,15 +4491,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4508,29 +4508,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4541,15 +4541,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4558,29 +4558,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4591,15 +4591,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4608,29 +4608,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4641,15 +4641,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4658,29 +4658,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4691,89 +4691,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -4781,33 +4781,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -4815,96 +4815,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4920,15 +4920,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4936,53 +4936,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -4990,30 +4990,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5028,15 +5028,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5052,15 +5052,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5068,53 +5068,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -5122,30 +5122,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5160,15 +5160,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5184,15 +5184,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5200,53 +5200,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -5254,30 +5254,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5292,176 +5292,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -20020,26 +20020,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.listhlm cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_self_listhlm_cannot_be_converted); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/pyIMRPhenomD.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomD.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/waveforms/bbh/IMRPhenomD.h",
             "lisabeta/waveforms/bbh/IMRPhenomD_internals.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/waveforms/bbh",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "lisabeta/struct",
+            "./lisabeta/struct",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
@@ -1147,177 +1147,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1351,42 +1351,42 @@
 struct __pyx_obj_8lisabeta_9waveforms_3bbh_12pyIMRPhenomD_IMRPhenomD;
 struct __pyx_obj_8lisabeta_9waveforms_3bbh_12pyIMRPhenomD_IMRPhenomDh22AmpPhase;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6927,15 +6927,15 @@
   __Pyx_AddTraceback("lisabeta.waveforms.bbh.pyIMRPhenomD.IMRPhenomDh22AmpPhase.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6944,29 +6944,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6977,15 +6977,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6994,29 +6994,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7027,15 +7027,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7044,29 +7044,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7077,15 +7077,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7094,29 +7094,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7127,15 +7127,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7144,29 +7144,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7177,89 +7177,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7267,33 +7267,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7301,96 +7301,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7406,15 +7406,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7422,53 +7422,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -7476,30 +7476,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7514,15 +7514,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7538,15 +7538,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7554,53 +7554,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -7608,30 +7608,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7646,15 +7646,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7670,15 +7670,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7686,53 +7686,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -7740,30 +7740,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7778,176 +7778,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22944,26 +22944,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.Cextraparams,self.Cfreq,self.Cmodgrparams,self.Ctf,self.h22 cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_self_Cextraparams_self_Cfreq_sel); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/pyIMRPhenomHM.c` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/pyIMRPhenomHM.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "lisabeta/constants.h",
             "lisabeta/struct/struct.h",
             "lisabeta/waveforms/bbh/IMRPhenomD_internals.h",
             "lisabeta/waveforms/bbh/IMRPhenomHM.h"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "lisabeta/waveforms/bbh",
-            "lisabeta/struct",
-            "./lisabeta/struct",
             "lisabeta",
             "./lisabeta",
-            "/tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/core/include",
+            "lisabeta/struct",
+            "./lisabeta/struct",
+            "/tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include",
             "lisabeta/",
             "lisabeta/tools",
             "lisabeta/lisa"
         ],
         "language": "c",
         "libraries": [
@@ -1148,177 +1148,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":688
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":695
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":702
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":712
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1351,42 +1351,42 @@
 struct __pyx_obj_8lisabeta_6struct_8pystruct_py_object_function;
 struct __pyx_obj_8lisabeta_9waveforms_3bbh_13pyIMRPhenomHM_IMRPhenomHMhlmAmpPhase;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -7209,15 +7209,15 @@
   __Pyx_AddTraceback("lisabeta.waveforms.bbh.pyIMRPhenomHM.IMRPhenomHMhlmAmpPhase.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7226,29 +7226,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":732
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":731
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7259,15 +7259,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7276,29 +7276,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7309,15 +7309,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7326,29 +7326,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7359,15 +7359,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7376,29 +7376,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7409,15 +7409,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7426,29 +7426,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7459,89 +7459,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":748
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":747
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7549,33 +7549,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":927
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 928, __pyx_L1_error)
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":926
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7583,96 +7583,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":933
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":932
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7688,15 +7688,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7704,53 +7704,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":940
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 940, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 942, __pyx_L5_except_error)
@@ -7758,30 +7758,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":939
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":938
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7796,15 +7796,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7820,15 +7820,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7836,53 +7836,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":946
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 946, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 948, __pyx_L5_except_error)
@@ -7890,30 +7890,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":945
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7928,15 +7928,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7952,15 +7952,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7968,53 +7968,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":952
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 952, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 954, __pyx_L5_except_error)
@@ -8022,30 +8022,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":951
+    /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8060,176 +8060,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":976
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":964
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":991
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1001
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1008
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+/* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1015
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22968,26 +22968,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.Cextraparams,self.Cfreq_21,self.Cfreq_22,self.Cfreq_32,self.Cfreq_33,self.Cfreq_43,self.Cfreq_44,self.Cmodgrparams,self.listhlm cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_self_Cextraparams_self_Cfreq_21); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
 
-  /* "../../../tmp/build-env-o39o4y97/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../tmp/build-env-kel866lx/lib/python3.10/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 948, __pyx_L1_error)
```

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/setup.py` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/setup.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta/waveforms/bbh/tf2.py` & `lisabeta-1.0.1/lisabeta/waveforms/bbh/tf2.py`

 * *Files identical despite different names*

### Comparing `lisabeta-1.0.0/lisabeta.egg-info/SOURCES.txt` & `lisabeta-1.0.1/lisabeta.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 lisabeta/__init__.py
 lisabeta/constants.h
 lisabeta/pyconstants.c
+lisabeta/pyconstants.pxd
+lisabeta/pyconstants.pyx
 lisabeta.egg-info/PKG-INFO
 lisabeta.egg-info/SOURCES.txt
 lisabeta.egg-info/dependency_links.txt
 lisabeta.egg-info/top_level.txt
 lisabeta/inference/__init__.py
 lisabeta/inference/inference.py
 lisabeta/inference/multiemcee.py
@@ -28,46 +31,68 @@
 lisabeta/lisa/__init__.py
 lisabeta/lisa/ldcnoise.py
 lisabeta/lisa/ldctools.py
 lisabeta/lisa/lisa.py
 lisabeta/lisa/lisa_fisher.py
 lisabeta/lisa/lisatools.py
 lisabeta/lisa/pyLISAnoise.c
+lisabeta/lisa/pyLISAnoise.pxd
+lisabeta/lisa/pyLISAnoise.pyx
 lisabeta/lisa/pyresponse.c
+lisabeta/lisa/pyresponse.pxd
+lisabeta/lisa/pyresponse.pyx
 lisabeta/lisa/snrtools.py
 lisabeta/struct/__init__.py
 lisabeta/struct/pystruct.c
+lisabeta/struct/pystruct.pxd
+lisabeta/struct/pystruct.pyx
 lisabeta/struct/struct.c
 lisabeta/struct/struct.h
 lisabeta/tools/__init__.py
 lisabeta/tools/fresnel.c
+lisabeta/tools/fresnel.h
 lisabeta/tools/overlap.c
 lisabeta/tools/overlap.h
 lisabeta/tools/pyoverlap.c
+lisabeta/tools/pyoverlap.pxd
+lisabeta/tools/pyoverlap.pyx
 lisabeta/tools/pyspline.c
+lisabeta/tools/pyspline.pxd
+lisabeta/tools/pyspline.pyx
 lisabeta/tools/pytools.c
+lisabeta/tools/pytools.pxd
+lisabeta/tools/pytools.pyx
+lisabeta/tools/referenceframes.c
+lisabeta/tools/referenceframes.h
 lisabeta/tools/spline.c
 lisabeta/tools/spline.h
 lisabeta/tools/tools.c
 lisabeta/tools/tools.h
 lisabeta/utils/__init__.py
 lisabeta/utils/corner_covar.py
 lisabeta/utils/plotutils.py
 lisabeta/waveforms/__init__.py
 lisabeta/waveforms/bbh/EOBNRv2HMROM.c
 lisabeta/waveforms/bbh/EOBNRv2HMROM.h
 lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.c
+lisabeta/waveforms/bbh/EOBNRv2HMROMstruct.h
 lisabeta/waveforms/bbh/IMRPhenomD.c
 lisabeta/waveforms/bbh/IMRPhenomD.h
 lisabeta/waveforms/bbh/IMRPhenomD_internals.c
 lisabeta/waveforms/bbh/IMRPhenomD_internals.h
 lisabeta/waveforms/bbh/IMRPhenomHM.c
 lisabeta/waveforms/bbh/IMRPhenomHM.h
 lisabeta/waveforms/bbh/IMRPhenomInternalUtils.c
+lisabeta/waveforms/bbh/IMRPhenomInternalUtils.h
 lisabeta/waveforms/bbh/IMRPhenomUtils.c
+lisabeta/waveforms/bbh/IMRPhenomUtils.h
 lisabeta/waveforms/bbh/RingdownCW.c
+lisabeta/waveforms/bbh/RingdownCW.h
 lisabeta/waveforms/bbh/__init__.py
 lisabeta/waveforms/bbh/pyEOBNRv2HMROM.c
+lisabeta/waveforms/bbh/pyEOBNRv2HMROM.pyx
 lisabeta/waveforms/bbh/pyIMRPhenomD.c
+lisabeta/waveforms/bbh/pyIMRPhenomD.pyx
 lisabeta/waveforms/bbh/pyIMRPhenomHM.c
+lisabeta/waveforms/bbh/pyIMRPhenomHM.pyx
 lisabeta/waveforms/bbh/setup.py
 lisabeta/waveforms/bbh/tf2.py
```

### Comparing `lisabeta-1.0.0/setup.py` & `lisabeta-1.0.1/setup.py`

 * *Files identical despite different names*

