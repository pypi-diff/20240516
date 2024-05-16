# Comparing `tmp/esi_shakelib-1.0.5.tar.gz` & `tmp/esi_shakelib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_shakelib-1.0.5.tar", last modified: Tue Apr 23 17:52:06 2024, max compression
+gzip compressed data, was "esi_shakelib-1.0.6.tar", last modified: Thu May 16 18:39:27 2024, max compression
```

## Comparing `esi_shakelib-1.0.5.tar` & `esi_shakelib-1.0.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      517 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1522 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.078262 esi_shakelib-1.0.5/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imt.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/correlation/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/ccf_base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/dummy.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/loth_baker_2013.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/directivity/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/bayless2013.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25636 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/rowshandel2013.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    26785 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/ffsimmer.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7274 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/generic_site_amplitication.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/gmice/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/ak07.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/fm11.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/gmice.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/wald99.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/wgrw12.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10920 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/readme
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3225 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nullgmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    43334 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/multigmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/multiutils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/plotting/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/contour.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/plotrupture.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/sites.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/station.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/containers.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/imt_string.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11907 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6723 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/virtualipe.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3491 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      470 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      517 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1522 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.134951 esi_shakelib-1.0.6/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imt.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.138951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/correlation/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/ccf_base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/dummy.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/correlation/loth_baker_2013.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.142951 esi_shakelib-1.0.6/src/esi_shakelib/directivity/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/bayless2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25636 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/directivity/rowshandel2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27220 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/ffsimmer.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7274 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/generic_site_amplitication.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmice/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/ak07.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/fm11.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/gmice.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/wald99.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmice/wgrw12.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10920 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/readme
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3225 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nullgmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    43334 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/multigmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/multiutils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.146950 esi_shakelib-1.0.6/src/esi_shakelib/plotting/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/contour.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/plotting/plotrupture.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/sites.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/station.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/src/esi_shakelib/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:38:21.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/containers.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/exception.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/imt_string.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11907 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/utils/utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6723 2024-05-16 18:23:26.000000 esi_shakelib-1.0.6/src/esi_shakelib/virtualipe.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-16 18:39:27.150950 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3491 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      470 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2024-05-16 18:39:27.000000 esi_shakelib-1.0.6/src/esi_shakelib.egg-info/top_level.txt
```

### Comparing `esi_shakelib-1.0.5/LICENSE.md` & `esi_shakelib-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/PKG-INFO` & `esi_shakelib-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.5
+Version: 1.0.6
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `esi_shakelib-1.0.5/README.md` & `esi_shakelib-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/pyproject.toml` & `esi_shakelib-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imc.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imc.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imt.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/convert_imt.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/boore_kishida_2017.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/boore_kishida_2017.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/newmark_hall_1982.py` & `esi_shakelib-1.0.6/src/esi_shakelib/conversions/imt/newmark_hall_1982.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/correlation/ccf_base.py` & `esi_shakelib-1.0.6/src/esi_shakelib/correlation/ccf_base.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/correlation/dummy.py` & `esi_shakelib-1.0.6/src/esi_shakelib/correlation/dummy.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/correlation/loth_baker_2013.py` & `esi_shakelib-1.0.6/src/esi_shakelib/correlation/loth_baker_2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/directivity/bayless2013.py` & `esi_shakelib-1.0.6/src/esi_shakelib/directivity/bayless2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/directivity/rowshandel2013.py` & `esi_shakelib-1.0.6/src/esi_shakelib/directivity/rowshandel2013.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/ffsimmer.py` & `esi_shakelib-1.0.6/src/esi_shakelib/ffsimmer.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,28 @@
 
 class FFSimmer:
     """
     Class to perform monte carlo simulations of finite faults to derive mean ground
     motions
     """
 
-    def __init__(self, origin, rff):
+    def __init__(self, origin, rff, measure="median"):
         """
         origin: (Origin object)
             The earthquake origin
         gmpe: (MultiGMPE object)
             The MultiGMPE to be used for the simulations
         rff: (RandomFiniteFault object)
             An object initialized to a set of random faults
         nsim: (int)
             The number of simulations to perform
         """
+        if measure not in ("mean", "median"):
+            raise ValueError(f"Unknown measure of central tendency: {measure}")
+        self.measure = measure
         warnings.simplefilter("ignore", ConvergenceWarning)
         self.origin = copy.copy(origin)
         self.rff = rff
 
     def compute_grid(self, grid, gmpes, myimts):
         """
         Args:
@@ -197,15 +200,18 @@
         gdepth = np.zeros_like(glon)
         grepi = rupt.computeRepi(glon, glat, gdepth)
 
         # Compute Mean, Sigma, Phi, and Tau for each IMT
         mean_residuals = np.empty((nsim, nx * ny))
         distances = np.empty((nsim, nx * ny))
         for iimt in range(nimt):
-            mean_means = np.mean(means[iimt], axis=0)
+            if self.measure == "median":
+                mean_means = np.median(means[iimt], axis=0)
+            else:
+                mean_means = np.mean(means[iimt], axis=0)
             for idx in range(nsim):
                 mean_residuals[idx] = means[iimt, idx] - mean_means
                 distances[idx, :] = idx
             extra_sigmas = np.var(means[iimt], axis=0)
 
             df = pd.DataFrame(
                 {
@@ -337,15 +343,18 @@
         # Compute Mean, Sigma, Phi, and Tau for each IMT
         mean_residuals = np.empty((nsim, nporig))
         distances = np.empty((nsim, nporig))
         for iimt in range(nimt):
             outdict[myimts[iimt]] = {}
             for ictx, ctx_name in enumerate(ctxt_names):
                 # Take the mean over the realizations
-                mean_means = np.mean(means[ictx, iimt], axis=0)
+                if self.measure == "median":
+                    mean_means = np.median(means[ictx, iimt], axis=0)
+                else:
+                    mean_means = np.mean(means[ictx, iimt], axis=0)
                 # Compute the residuals at each distance, index the distances
                 for idx in range(nsim):
                     mean_residuals[idx] = means[ictx, iimt, idx] - mean_means
                     distances[idx, :] = idx
                 # Find the variance over the realizations
                 extra_sigmas = np.var(means[ictx, iimt], axis=0)
 
@@ -501,21 +510,21 @@
 
     Args:
         origin:
             An Origin object.
     """
 
     mech = getattr(origin, "mech", "ALL")
-    if not hasattr(origin, "_tectonic_region"):
+    if not hasattr(origin, "tectonic_region"):
         mscale = MagScaling.WC94
         # smech = Mechanism.A
         mindip_deg = 35.0
         maxdip_deg = 90.0
         aspect = 1.7
-    elif origin._tectonic_region == "Active":
+    elif origin.tectonic_region == "Active":
         mscale = MagScaling.HB08
         aspect = 1.7
         if mech == "ALL":
             # HB08 doesn't have an 'ALL' mechanism, so use WC94
             mscale = MagScaling.WC94
             # smech = Mechanism.A
             mindip_deg = 35.0
@@ -528,15 +537,15 @@
             # smech = Mechanism.N
             mindip_deg = 40.0
             maxdip_deg = 60.0
         elif mech == "SS":
             # smech = Mechanism.SS
             mindip_deg = 75.0
             maxdip_deg = 90.0
-    elif origin._tectonic_region == "Stable":
+    elif origin.tectonic_region == "Stable":
         mscale = MagScaling.S14
         aspect = 1.0
         if mech == "ALL":
             # smech = Mechanism.A
             mindip_deg = 35.0
             maxdip_deg = 90.0
         elif mech == "RS":
@@ -547,15 +556,15 @@
             # smech = Mechanism.N
             mindip_deg = 40.0
             maxdip_deg = 60.0
         elif mech == "SS":
             # smech = Mechanism.SS
             mindip_deg = 60.0
             maxdip_deg = 90.0
-    elif origin._tectonic_region == "Subduction":
+    elif origin.tectonic_region == "Subduction":
         aspect = 1.7
         if mech == "ALL":
             mscale = MagScaling.Sea10_interface
             # smech = Mechanism.A
             mindip_deg = 35.0
             maxdip_deg = 90.0
         elif mech == "RS":
```

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/generic_site_amplitication.py` & `esi_shakelib-1.0.6/src/esi_shakelib/generic_site_amplitication.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmice/ak07.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmice/ak07.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmice/fm11.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmice/fm11.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmice/gmice.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmice/gmice.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmice/wald99.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmice/wald99.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmice/wgrw12.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmice/wgrw12.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt` & `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat` & `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nullgmpe.py` & `esi_shakelib-1.0.6/src/esi_shakelib/gmpe/nullgmpe.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/multigmpe.py` & `esi_shakelib-1.0.6/src/esi_shakelib/multigmpe.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/multiutils.py` & `esi_shakelib-1.0.6/src/esi_shakelib/multiutils.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/plotting/contour.py` & `esi_shakelib-1.0.6/src/esi_shakelib/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/plotting/plotrupture.py` & `esi_shakelib-1.0.6/src/esi_shakelib/plotting/plotrupture.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/sites.py` & `esi_shakelib-1.0.6/src/esi_shakelib/sites.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/station.py` & `esi_shakelib-1.0.6/src/esi_shakelib/station.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/utils/containers.py` & `esi_shakelib-1.0.6/src/esi_shakelib/utils/containers.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/utils/imt_string.py` & `esi_shakelib-1.0.6/src/esi_shakelib/utils/imt_string.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/utils/utils.py` & `esi_shakelib-1.0.6/src/esi_shakelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib/virtualipe.py` & `esi_shakelib-1.0.6/src/esi_shakelib/virtualipe.py`

 * *Files identical despite different names*

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib.egg-info/PKG-INFO` & `esi_shakelib-1.0.6/src/esi_shakelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.5
+Version: 1.0.6
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `esi_shakelib-1.0.5/src/esi_shakelib.egg-info/SOURCES.txt` & `esi_shakelib-1.0.6/src/esi_shakelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

