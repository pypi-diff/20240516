# Comparing `tmp/ramanchada2-0.0.8.tar.gz` & `tmp/ramanchada2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanchada2-0.0.8.tar", last modified: Mon Jul 17 02:51:45 2023, max compression
+gzip compressed data, was "ramanchada2-0.0.9.tar", last modified: Fri Dec  1 23:30:38 2023, max compression
```

## Comparing `ramanchada2-0.0.8.tar` & `ramanchada2-0.0.9.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/README.pypi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:44.996699 ramanchada2-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.004699 ramanchada2-0.0.8/src/ramanchada2/
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.004699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.004699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.004699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.012699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
--rw-r--r--   0 runner    (1001) docker     (123)   185598 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184263 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187339 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187743 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   190431 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189952 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187633 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187638 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   191297 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187259 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.016699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35649 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171476 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35658 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171859 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35712 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16841 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171894 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16872 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35718 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171856 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35694 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171844 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35703 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171846 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171923 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35687 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
--rw-r--r--   0 runner    (1001) docker     (123)   171889 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.020699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
--rw-r--r--   0 runner    (1001) docker     (123)   182699 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184528 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   182774 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184434 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174788 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175407 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175468 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174802 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175123 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174660 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175356 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174887 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174718 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   173754 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   176673 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   177120 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   174707 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175243 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.028699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
--rw-r--r--   0 runner    (1001) docker     (123)   184364 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185045 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185328 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189806 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   201634 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189411 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189005 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187207 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   187573 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   186787 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189400 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   189244 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   188792 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185773 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   185317 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184476 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   183722 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184176 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184535 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184428 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184511 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
--rw-r--r--   0 runner    (1001) docker     (123)   184796 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.028699 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
--rw-r--r--   0 runner    (1001) docker     (123)   101150 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101182 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101185 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101119 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101189 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101169 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101184 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
--rw-r--r--   0 runner    (1001) docker     (123)   101413 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/HSDS.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/bw_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/read_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/experimental/two_column_spe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/output/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/output/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/simulated/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/lines_from_raw_dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/read_simulated_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/io/simulated/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    23672 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/plottable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.032699 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/misc/types/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/fit_peaks_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/peak_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/positive_not_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/pydantic_base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/applied_processings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/misc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/utils/argmin2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/misc/utils/svd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectral_components/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectral_components/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/baseline/analytical.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/baseline/baseline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/baseline/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/voigt.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/spectral_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectral_components/spectral_peak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectrum/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/mul.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/truediv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/add_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/baseline_rc1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/moving_minimum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.036699 ramanchada2-0.0.8/src/ramanchada2/spectrum/calc/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calc/central_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/by_deltas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/change_x_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/scale_xaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/scale_yaxis.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_chada.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_delta_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_test_spe.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/add_poisson_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/drop_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/pad_zeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/sharpen_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/trim_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/fit_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/spectrum/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.040699 ramanchada2-0.0.8/src/ramanchada2/theoretical_lines/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/theoretical_lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-17 02:51:28.000000 ramanchada2-0.0.8/src/ramanchada2/theoretical_lines/model_from_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:51:45.004699 ramanchada2-0.0.8/src/ramanchada2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 02:51:44.000000 ramanchada2-0.0.8/src/ramanchada2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-17 02:51:44.000000 ramanchada2-0.0.8/src/ramanchada2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:51:44.000000 ramanchada2-0.0.8/src/ramanchada2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-17 02:51:44.000000 ramanchada2-0.0.8/src/ramanchada2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 02:51:44.000000 ramanchada2-0.0.8/src/ramanchada2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.612456 ramanchada2-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 23:30:38.612456 ramanchada2-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.560456 ramanchada2-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.564456 ramanchada2-0.0.9/src/ramanchada2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.564456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.564456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.564456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.568456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/
+-rw-r--r--   0 runner    (1001) docker     (127)   185598 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184263 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187339 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187743 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   190431 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189952 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187633 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187638 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191297 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187259 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.576456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/
+-rw-r--r--   0 runner    (1001) docker     (127)    16858 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35649 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171476 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16871 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35658 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171859 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35712 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171856 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35709 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171894 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16872 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35718 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171856 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16867 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171844 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16876 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35703 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171846 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16869 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35695 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171923 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35687 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   171889 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.584456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/
+-rw-r--r--   0 runner    (1001) docker     (127)   182699 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184528 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   182774 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184434 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174788 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175407 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175468 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174802 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175123 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174660 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175356 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174887 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174718 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   173754 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   176673 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   177120 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   174707 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   175243 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.592456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/
+-rw-r--r--   0 runner    (1001) docker     (127)   184364 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185045 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185328 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189806 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   201634 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189411 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189005 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187207 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   187573 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   186787 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189400 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   189244 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   188792 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185773 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   185317 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184476 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   183722 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184176 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184535 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184428 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184511 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   184796 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.592456 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/
+-rw-r--r--   0 runner    (1001) docker     (127)   101150 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101182 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101185 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101119 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101189 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101169 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101184 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101184 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101413 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.592456 ramanchada2-0.0.9/src/ramanchada2/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/HSDS.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/bw_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/read_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/experimental/two_column_spe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/output/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/simulated/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/lines_from_raw_dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/read_simulated_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/io/simulated/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.596456 ramanchada2-0.0.9/src/ramanchada2/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23672 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/plottable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/dynamically_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/spectrum_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/misc/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/fit_peaks_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/peak_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/positive_not_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/pydantic_base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/applied_processings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/misc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/utils/argmin2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/misc/utils/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/spectral_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.600456 ramanchada2-0.0.9/src/ramanchada2/spectral_components/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/baseline/analytical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/baseline/baseline_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/baseline/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/voigt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/spectral_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectral_components/spectral_peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/mul.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/truediv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/add_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/baseline_rc1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/moving_minimum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectrum/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calc/central_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.604456 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/by_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/change_x_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/scale_xaxis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/scale_yaxis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/set_new_xaxis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_cache_or_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_chada.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_delta_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_test_spe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_theoretical_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/add_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/add_poisson_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/drop_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/pad_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/sharpen_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/trim_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/fit_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/spectrum/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/src/ramanchada2/theoretical_lines/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/theoretical_lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-12-01 23:30:28.000000 ramanchada2-0.0.9/src/ramanchada2/theoretical_lines/model_from_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 23:30:38.608456 ramanchada2-0.0.9/src/ramanchada2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-01 23:30:38.000000 ramanchada2-0.0.9/src/ramanchada2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2023-12-01 23:30:38.000000 ramanchada2-0.0.9/src/ramanchada2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 23:30:38.000000 ramanchada2-0.0.9/src/ramanchada2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-01 23:30:38.000000 ramanchada2-0.0.9/src/ramanchada2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-01 23:30:38.000000 ramanchada2-0.0.9/src/ramanchada2.egg-info/top_level.txt
```

### Comparing `ramanchada2-0.0.8/LICENSE` & `ramanchada2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/README.md` & `ramanchada2-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# ramanchada2
+
 [![build](https://github.com/h2020charisma/ramanchada2/workflows/build/badge.svg)](https://github.com/h2020charisma/ramanchada2/actions/workflows/build.yml)
 [![docs](https://github.com/h2020charisma/ramanchada2/workflows/docs/badge.svg)](https://h2020charisma.github.io/ramanchada2/index.html)
 
-Harmonising Raman Spectroscopy
-==============================
+Harmonising Raman spectroscopy: meant to fill the gap between the theoretical Raman analysis and the experimental Raman spectroscopy by providing means to compare data of different origin.
+
+- 📖 [Documentation](https://h2020charisma.github.io/ramanchada2/ramanchada2.html)
+- ⚗️ [Examples](https://github.com/h2020charisma/ramanchada2/tree/main/examples)
+
 
-RamanChada v2
---------------
+## Quick start
 
 Clone the repo using https
 ```bash
 git clone https://github.com/h2020charisma/ramanchada2.git
 ```
 or by using ssh
 ```
```

### Comparing `ramanchada2-0.0.8/README.pypi` & `ramanchada2-0.0.9/README.pypi`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ramanchada2
 
 ramanchada2 is meant to fill the gap between the theoretical Raman analysis and the experimental Raman spectroscopy by providing means to compare data of different origin.
 
 For more information, see:
 * https://github.com/h2020charisma/ramanchada2
 * https://h2020charisma.github.io/ramanchada2/ramanchada2.html
+* https://github.com/h2020charisma/ramanchada2/tree/main/examples
 
 ---
 🇪🇺 This project has received funding from the European Union’s Horizon 2020 research and innovation program under [grant agreement No. 952921](https://cordis.europa.eu/project/id/952921).
```

### Comparing `ramanchada2-0.0.8/setup.py` & `ramanchada2-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,28 +34,28 @@
 PACKAGE_DIR = {'': 'src'}
 
 PACKAGE_DATA = {'': ['auxiliary/**/*.txt']}
 
 DATA_FILES = []
 
 INSTALL_REQUIRES = [
+        "brukeropusreader",  # rc1-parser
         "h5py",
         "lmfit",
         "matplotlib",
         "numpy",
         "pandas",
         "pydantic==1.*",
         "pyhht",
+        "renishawWiRE",  # rc1-parser
         "scikit-learn",
         "scipy>=1.8.0",
+        "spc-io~=0.0.2",  # rc1-parser
         "statsmodels",
         "uncertainties",
-        "renishawWiRE",  # rc1-parser
-        "opusFC",  # rc1-parser
-        "spc-io~=0.0.2",  # rc1-parser
 ]
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Science/Research',
```

### Comparing `ramanchada2-0.0.8/src/ramanchada2/__init__.py` & `ramanchada2-0.0.9/src/ramanchada2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,104 +1,111 @@
 #!/usr/bin/env python3
 
 
 """
-# Ramanchada2
-
-## Purpose
+# Purpose
 `ramanchada2` software package is meant to fill the gap between the theoretical
 Raman analysis and the experimental Raman spectroscopy by providing means to
 compare data of different origin. The software is in early development stage
 but still able to solve practical problems.
 
-## Features
-
+# Features
 
-### Read simulated data
-Process simulated data by [VASP] and [CRYSTAL] and provide same interface.
+## Read simulated data
+Process simulated data by [VASP][] and [CRYSTAL][] and provide same interface.
 CRYSTAL data contain intensities for multiple orientations -- laser beam
 incidents perpendicularly or parallelly to the observation and information
 for mono-crystals. VASP data provide data only for poly-crystals but in
 different format. So the perpendicular and parallel intensities are calculated
-by an implemented [algorithm](https://doi.org/10.1103/PhysRevB.54.7830).
+by an implemented [algorithm][].
 
-### Models
-[LMFIT] theoretical models can be build by spectral information obtained by
+## Models
+[LMFIT][] theoretical models can be build by spectral information obtained by
 simulations or by provided by the user. These models can be fit to experimental
 data, providing calibration information. At poor initial calibration the minimisation
 procedure naturally fails. An iterative procedure aiming to solve this problem
 was adopted in the code. On the first iteration the experimental spectrum lines
 are artificially broadened. This makes it possible for the minimisation procedure
 to find a parameters that are close enough to be used as an initial guess for
 the second iteration. In few iterations the algorithm is able to fit to the original
 experimental data. This idea is implemented and is at proof-of-concept level.
 
-### Generate spectra
+## Generate spectra
 Spectra can be generated by the theoretical models. Random Poissonian noise and
 artificial random-generated baseline can be added to the generated spectra, making
 them convenient tools to test new methods for analysis.
 
-### Spectrum manipulation
+## Spectrum manipulation
 A number of filters can be applied to spectra (experimental and generated).
 Scaling on both x and y axes is possible. Scaling could be linear or arbitrary
 user defined function. A convolution is possible with set of predefined functions
 as well as user defined model.
 
-## Concept
+# Concept
 The code is object oriented, written in python. Main elements are Spectrum and
-theoretical models. Theoretical models are based on [LMFIT] library, while
+theoretical models. Theoretical models are based on LMFIT library, while
 Spectrum is a custom made class. Spectrum object contains data for x and y axes
 and metadata coming from experimental files or other sources. It is planned
 to add information about the uncertainties in x and y. All filters and manipulation
 procedures are available as class methods. Measures are taken to preserve spectrum
 instances immutable, so filters are generating new spectra, preserving the original
 unchanged. Additionally, Spectrum has information about its history -- the sequence
 of applied filters.
 
-## File formats
-### `.cha` vs [USID]/[NSID]
-`ramanchada`(1) software package introduced `.cha` file format, which is a [HDF5]
-with a specific architecture. Two spectroscopy specific file formats -- [USID] and
-[NSID] -- were considered as successors of `.cha`. [USID] and [NSID] are provided
-by [pycroscopy] package as an extension of [HDF5]. Several jupyter notebooks were
+# File formats
+
+## `.cha` vs USID/NSID
+[ramanchada][] software package introduced `.cha` file format, which is an [HDF5][]
+with a specific architecture. Two spectroscopy specific file formats -- [USID][] and
+[NSID][] -- were considered as successors of `.cha`. USID and NSID are provided
+by [pycroscopy][] package as an extension of HDF5. Several jupyter notebooks were
 created in order to assess the advantages and disadvantages of such a change. These
 file formats are designed to handle multidimensional spectral data, keeping track
 of the modifications. These file formats does not provide big advantage in our case,
-so currently `ramanchada2` supports `.cha` file format and does not support [USID]
-or [NSID].
+so currently `ramanchada2` supports `.cha` file format and does not support USID
+or NSID.
 
-### Cache
+## Cache
 The concept to keep previous variants of data is employed in `ramanchada2`. If
 configured so, the software saves the data for all Spectrum instances to a
 tree-organized `.cha` file. When a particular chain of operations is requested
 by the user, the software checks if the final result is present in the cache file,
 if so it is provided, otherwise the software checks for its parent. When a parent
 or some of the grand parents are present, they are taken as a starting point and
 the needed steps are applied to provide the final result. The current implementation
-uses [h5py] library to access local hdf files. It is foreseen to have implementation
-with [h5pyd] that support network operations.
+uses [h5py][] library to access local hdf files. It is foreseen to have implementation
+with [h5pyd][] that support network operations.
 
 
-[VASP]: https://www.vasp.at/
 [CRYSTAL]: https://www.crystal.unito.it/index.php
-[LMFIT]: https://lmfit.github.io/lmfit-py/index.html
 [HDF5]: https://hdfgroup.org/
+[LMFIT]: https://lmfit.github.io/lmfit-py/index.html
+[NSID]: https://pycroscopy.github.io/pyNSID
+[USID]: https://pycroscopy.github.io/USID
+[VASP]: https://www.vasp.at/
+[algorithm]: https://doi.org/10.1103/PhysRevB.54.7830
 [h5py]: https://h5py.org/
 [h5pyd]: https://github.com/HDFGroup/h5pyd
 [pycroscopy]: https://pycroscopy.github.io/pycroscopy/
-[USID]: https://pycroscopy.github.io/USID
-[NSID]: https://pycroscopy.github.io/pyNSID
+[ramanchada]: https://github.com/h2020charisma/ramanchada
 """
 
 from __future__ import annotations
 
 from . import spectrum
 from . import theoretical_lines
-__all__ = ['spectrum', 'theoretical_lines']
-__version__ = '0.0.8'
+__all__ = [
+    'auxiliary',
+    'io',
+    'misc',
+    'spectral_components',
+    'spectrum',
+    'theoretical_lines',
+]
+__version__ = '0.0.9'
 
 
 import logging
 
 
 class CustomFormatter(logging.Formatter):
     green = "\x1b[32m"
```

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_100msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/NeonSNQ043_iR532_Probe_5msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/PST10_iR532_Probe_100_3000msx7.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0B10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0N10_iR532_Probe_100_30000msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S0P10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/S1N10_iR532_Probe_100_22000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/Sil10_iR532_Probe_100_60000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/nCAL10_iR532_Probe_100_2500msx3.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_BW532/sCAL10_iR532_Probe_100_3200msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP01.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP02.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/NeonSNQ043_iR785_OP03.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP01_40000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP02_50000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/PST10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0B10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S0P10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/S1N10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP02_25000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/Sil10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP01_6000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP02_20000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/nCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP01_4000msx4.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP02_15000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/FMNT-M_Ho785/sCAL10_iR785_OP03_8000msx2.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_110ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_25ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/Ne_532nm_x50_800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z050_100_2500msx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/PST02_iRPlus532_Z100_100_50000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0B02_iRPlus532_Z100_100_22000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z050_100_40000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0N02_iRPlus532_Z100_100_28000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z050_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S0P02_iRPlus532_Z100_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z050_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/S1N02_iRPlus532_Z100_100_6500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z050_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/nCAL02_iRPlus532_Z100_100_30000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z050_100_20000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW532/sCAL02_iRPlus532_Z100_100_65000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z020_100_1300ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/PST02_iRPlus785_Z100_100_9000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z020_100_full.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z050_100_5500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0B02_iRPlus785_Z100_100_4700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z050_100_3200ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0N02_iRPlus785_Z100_100_3100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z020_100_12000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z050_100_5700ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S0P02_iRPlus785_Z100_100_4800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z020_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/S1N02_iRPlus785_Z100_100_2000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z020_100_1100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z050_100_2100ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/nCAL02_iRPlus785_Z100_100_6000ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z020_100_2400ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z050_100_3800ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/ICV_BW785/sCAL02_iRPlus785_Z100_100_9500ms.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Pol_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0B_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0N_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S0P_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/S1N_HLR633_Z010_100_10sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/Si_HLR633_Z010_100_40sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/nCAL_HLR633_Z010_100_5sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/neon_new2_Z010.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/TOP_Ho633/sCAL_HLR633_Z010_100_15sx5.txt`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py` & `ramanchada2-0.0.9/src/ramanchada2/auxiliary/spectra/datasets2/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/HSDS.py` & `ramanchada2-0.0.9/src/ramanchada2/io/HSDS.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/bw_format.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/bw_format.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/binary_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/io.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,24 +34,24 @@
     # store in metadata dictionary, and include in CHADA archive.
     metadata["Original file"] = os.path.basename(source_path)
     return x_data, y_data, metadata
 
 
 def cleanMeta(meta):
     # This cleans complex-strcutures metadata, and returns a dict
-    if type(meta) == dict:
+    if isinstance(meta, dict):
         meta = {i: meta[i] for i in meta if i != ""}
         for key, value in meta.items():
             meta[key] = cleanMeta(value)
-    if type(meta) == list:
+    if isinstance(meta, list):
         for ii, value in enumerate(meta):
             meta[ii] = cleanMeta(value)
-    if type(meta) == str:
+    if isinstance(meta, str):
         meta = meta.replace('\\x00', '')
         meta = meta.replace('\x00', '')
-    if type(meta) == bytes:
+    if isinstance(meta, bytes):
         try:
             meta = meta.decode('utf-8')
             meta = cleanMeta(meta)
         except Exception:
             meta = []
     return meta
```

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/third_party_readers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from renishawWiRE import WDFReader
 from spc_io import SPC
-import opusFC
+from brukeropusreader import read_file
 
 
 def readWDF(file):
     s = WDFReader(file)
     y_data = s.spectra
     x_data = s.xdata
     if np.mean(np.diff(x_data)) < 0:
@@ -30,10 +30,20 @@
     x_data = spc[0].xarray
     y_data = spc[0].yarray
     static_metadata = spc.log_book.text
     return x_data, y_data, static_metadata
 
 
 def readOPUS(file, obj_no=0):
-    c = opusFC.listContents(file)
-    data = opusFC.getOpusData(file, c[obj_no])
-    return data.x, data.y, data.parameters
+    opus_data = read_file(file)
+    x = opus_data.get_range("AB")
+    y = opus_data["AB"]
+    meta = {}
+    for key in opus_data:
+        if key == "AB":
+            continue
+        if isinstance(opus_data[key], dict):
+            for subkey in opus_data[key]:
+                meta["{}.{}".format(key, subkey)] = opus_data[key][subkey]
+        else:
+            meta[key] = opus_data[key]
+    return x, y, meta
```

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/rc1_parser/txt_format_readers.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/read_csv.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/read_csv.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/experimental/read_txt.py` & `ramanchada2-0.0.9/src/ramanchada2/io/experimental/read_txt.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py` & `ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/discrete_lines_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py` & `ramanchada2-0.0.9/src/ramanchada2/io/simulated/crystal/discrete_lines_out.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/simulated/read_simulated_lines.py` & `ramanchada2-0.0.9/src/ramanchada2/io/simulated/read_simulated_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py` & `ramanchada2-0.0.9/src/ramanchada2/io/simulated/vasp/vasp_simulation_dat.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/base_class.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/base_class.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/constants.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/constants.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/spectrum_constructor.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/spectrum_deco/spectrum_filter.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/types/fit_peaks_result.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/types/fit_peaks_result.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/types/peak_candidates.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/types/peak_candidates.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/types/positive_not_multiple.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/types/positive_not_multiple.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/applied_processings.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/applied_processings.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/types/spectrum/metadata.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/types/spectrum/metadata.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/utils/__init__.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/utils/argmin2d.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/utils/argmin2d.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py` & `ramanchada2-0.0.9/src/ramanchada2/misc/utils/ramanshift_to_wavelength.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/delta.py` & `ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/delta.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectral_components/peak_profile/gauss.py` & `ramanchada2-0.0.9/src/ramanchada2/spectral_components/peak_profile/gauss.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectral_components/spectral_component_collection.py` & `ramanchada2-0.0.9/src/ramanchada2/spectral_components/spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectral_components/spectral_peak.py` & `ramanchada2-0.0.9/src/ramanchada2/spectral_components/spectral_peak.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/__init__.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,7 @@
 from .creators.from_local_file import from_local_file
 from .creators.from_simulation import from_simulation
 from .creators.from_theoretical_lines import from_theoretical_lines
 from .creators.from_spectral_component_collection import from_spectral_component_collection
 from .creators.from_delta_lines import from_delta_lines
 from .creators.from_test_spe import from_test_spe
 from .creators.hdr_from_multi_exposure import hdr_from_multi_exposure
-
-
-__all__ = ['Spectrum',
-           'from_cache_or_calc',
-           'from_chada',
-           'from_local_file',
-           'from_simulation',
-           'from_test_spe',
-           'from_theoretical_lines',
-           'from_spectral_component_collection',
-           'from_delta_lines',
-           'hdr_from_multi_exposure',
-           ]
```

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/add.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/add.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/mul.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/mul.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/sub.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/sub.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/arithmetics/truediv.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/arithmetics/truediv.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/add_baseline.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/add_baseline.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/baseline_rc1.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/baseline_rc1.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/baseline/moving_minimum.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/baseline/moving_minimum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calc/central_moments.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calc/central_moments.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/by_deltas.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/by_deltas.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/change_x_units.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/change_x_units.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/normalize.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/normalize.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/scale_xaxis.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/scale_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/calibration/set_new_xaxis.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/calibration/set_new_xaxis.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_cache_or_calc.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_cache_or_calc.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_delta_lines.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_delta_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_local_file.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_local_file.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_simulation.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_simulation.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_spectral_component_collection.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_test_spe.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_test_spe.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/from_theoretical_lines.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/from_theoretical_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/creators/hdr_from_multi_exposure.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/add_gaussian_noise.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/add_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/add_poisson_noise.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/add_poisson_noise.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/convolve.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/convolve.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/drop_spikes.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/drop_spikes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/moving_average.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/moving_average.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/pad_zeros.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/pad_zeros.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/resampling.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/sharpen_lines.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/sharpen_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/smoothing.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/smoothing.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/filters/trim_axes.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/filters/trim_axes.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/find_peaks.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/find_peaks_BayesianGaussianMixture.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/fit_peaks.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/fit_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/peaks/get_fitted_peaks.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/spectrum/spectrum.py` & `ramanchada2-0.0.9/src/ramanchada2/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2/theoretical_lines/model_from_lines.py` & `ramanchada2-0.0.9/src/ramanchada2/theoretical_lines/model_from_lines.py`

 * *Files identical despite different names*

### Comparing `ramanchada2-0.0.8/src/ramanchada2.egg-info/SOURCES.txt` & `ramanchada2-0.0.9/src/ramanchada2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

