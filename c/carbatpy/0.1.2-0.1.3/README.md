# Comparing `tmp/carbatpy-0.1.2.tar.gz` & `tmp/carbatpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbatpy-0.1.2.tar", last modified: Tue Feb  6 11:25:58 2024, max compression
+gzip compressed data, was "carbatpy-0.1.3.tar", last modified: Thu May 16 13:33:44 2024, max compression
```

## Comparing `carbatpy-0.1.2.tar` & `carbatpy-0.1.3.tar`

### file list

```diff
@@ -1,99 +1,117 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.761918 carbatpy-0.1.2/
--rw-rw-rw-   0        0        0      174 2023-10-14 07:57:08.000000 carbatpy-0.1.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3661 2023-10-14 07:57:08.000000 carbatpy-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      228 2024-02-04 15:36:01.000000 carbatpy-0.1.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1093 2023-10-14 07:57:08.000000 carbatpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      377 2024-02-05 17:55:03.000000 carbatpy-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3186 2024-02-06 11:25:58.761918 carbatpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2173 2024-02-02 12:50:16.000000 carbatpy-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.618513 carbatpy-0.1.2/carbatpy/
--rw-rw-rw-   0        0        0     1072 2024-02-06 11:25:29.000000 carbatpy-0.1.2/carbatpy/__init__.py
--rw-rw-rw-   0        0        0      904 2024-02-04 10:28:20.000000 carbatpy-0.1.2/carbatpy/carbatpy0.py
--rw-rw-rw-   0        0        0      573 2024-02-05 15:22:44.000000 carbatpy-0.1.2/carbatpy/cb_config.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.577428 carbatpy-0.1.2/carbatpy/src/
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.644910 carbatpy-0.1.2/carbatpy/src/data/
--rw-rw-rw-   0        0        0     1514 2023-12-15 14:39:41.000000 carbatpy-0.1.2/carbatpy/src/data/ORC.gv
--rw-rw-rw-   0        0        0     1516 2023-12-15 15:04:55.000000 carbatpy-0.1.2/carbatpy/src/data/cycle.gv
--rw-rw-rw-   0        0        0    10812 2024-01-07 18:03:19.000000 carbatpy-0.1.2/carbatpy/src/data/hp_structure.xlsx
--rw-rw-rw-   0        0        0    10954 2024-01-07 18:05:37.000000 carbatpy-0.1.2/carbatpy/src/data/orc_structure.xlsx
--rw-rw-rw-   0        0        0      165 2023-12-15 12:35:13.000000 carbatpy-0.1.2/carbatpy/src/data/~$orc_structure.xlsx
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.649389 carbatpy-0.1.2/carbatpy/src/helpers/
--rw-rw-rw-   0        0        0        2 2024-02-04 10:38:35.000000 carbatpy-0.1.2/carbatpy/src/helpers/__init__.py
--rw-rw-rw-   0        0        0     1635 2024-02-04 15:40:43.000000 carbatpy-0.1.2/carbatpy/src/helpers/file_copy.py
--rw-rw-rw-   0        0        0     3647 2024-02-04 15:41:13.000000 carbatpy-0.1.2/carbatpy/src/helpers/uncertainty_vol_enthalpy.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.576422 carbatpy-0.1.2/carbatpy/src/models/
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.656170 carbatpy-0.1.2/carbatpy/src/models/components/
--rw-rw-rw-   0        0        0        0 2022-10-04 10:03:56.000000 carbatpy-0.1.2/carbatpy/src/models/components/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-12-16 09:25:05.000000 carbatpy-0.1.2/carbatpy/src/models/components/compressor_simple.py
--rw-rw-rw-   0        0        0    15369 2023-12-23 08:43:57.000000 carbatpy-0.1.2/carbatpy/src/models/components/heat_exchanger_thermo_v2.py
--rw-rw-rw-   0        0        0     1454 2023-11-04 17:22:23.000000 carbatpy-0.1.2/carbatpy/src/models/components/throttle_simple.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.670676 carbatpy-0.1.2/carbatpy/src/models/coupled/
--rw-rw-rw-   0        0        0        0 2022-10-04 10:03:56.000000 carbatpy-0.1.2/carbatpy/src/models/coupled/__init__.py
--rw-rw-rw-   0        0        0    20532 2024-02-05 15:52:07.000000 carbatpy-0.1.2/carbatpy/src/models/coupled/heat_pump_simple_v2.py
--rw-rw-rw-   0        0        0     5738 2024-02-04 16:16:35.000000 carbatpy-0.1.2/carbatpy/src/models/coupled/hp_for_opt.py
--rw-rw-rw-   0        0        0    16519 2024-02-05 16:11:45.000000 carbatpy-0.1.2/carbatpy/src/models/coupled/orc_simple_v2.py
--rw-rw-rw-   0        0        0     2717 2023-12-15 17:18:03.000000 carbatpy-0.1.2/carbatpy/src/models/coupled/read_cycle_structure.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.677825 carbatpy-0.1.2/carbatpy/src/models/fluids/
--rw-rw-rw-   0        0        0        0 2023-10-23 10:08:00.000000 carbatpy-0.1.2/carbatpy/src/models/fluids/__init__.py
--rw-rw-rw-   0        0        0     7456 2024-02-05 07:36:56.000000 carbatpy-0.1.2/carbatpy/src/models/fluids/fluid_props.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.691908 carbatpy-0.1.2/carbatpy/src/utils/
--rw-rw-rw-   0        0        0       93 2024-02-04 10:15:41.000000 carbatpy-0.1.2/carbatpy/src/utils/__init__.py
--rw-rw-rw-   0        0        0      924 2023-11-14 12:44:56.000000 carbatpy-0.1.2/carbatpy/src/utils/curve_min_distance_finder.py
--rw-rw-rw-   0        0        0     4614 2023-11-08 13:30:05.000000 carbatpy-0.1.2/carbatpy/src/utils/exergy_loss.py
--rw-rw-rw-   0        0        0     2570 2024-02-05 12:16:31.000000 carbatpy-0.1.2/carbatpy/src/utils/optimize.py
--rw-rw-rw-   0        0        0    12449 2024-02-05 07:37:38.000000 carbatpy-0.1.2/carbatpy/src/utils/property_eval_mixture.py
--rw-rw-rw-   0        0        0     3384 2024-02-02 16:12:18.000000 carbatpy-0.1.2/carbatpy/src/utils/run_heat_pump_simple.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.759661 carbatpy-0.1.2/carbatpy.egg-info/
--rw-rw-rw-   0        0        0     3186 2024-02-06 11:25:58.000000 carbatpy-0.1.2/carbatpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2538 2024-02-06 11:25:58.000000 carbatpy-0.1.2/carbatpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 11:25:58.000000 carbatpy-0.1.2/carbatpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-05 17:10:17.000000 carbatpy-0.1.2/carbatpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       83 2024-02-06 11:25:58.000000 carbatpy-0.1.2/carbatpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       62 2024-02-06 11:25:58.000000 carbatpy-0.1.2/carbatpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.731758 carbatpy-0.1.2/docs/
--rw-rw-rw-   0        0        0    21076 2023-11-06 12:31:19.000000 carbatpy-0.1.2/docs/2-storage_no_discharge.jpg
--rw-rw-rw-   0        0        0   661405 2023-10-25 12:03:31.000000 carbatpy-0.1.2/docs/2023-10-25-14-03EthProHexBut.png
--rw-rw-rw-   0        0        0    53322 2023-12-15 15:28:38.000000 carbatpy-0.1.2/docs/2023-12-15-16-28cycle.png
--rw-rw-rw-   0        0        0      629 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.580258 carbatpy-0.1.2/docs/_build/
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.586290 carbatpy-0.1.2/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.733758 carbatpy-0.1.2/docs/_build/html/_images/
--rw-rw-rw-   0        0        0   661405 2023-10-25 12:03:31.000000 carbatpy-0.1.2/docs/_build/html/_images/2023-10-25-14-03EthProHexBut.png
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.740079 carbatpy-0.1.2/docs/_build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-08-17 04:00:57.000000 carbatpy-0.1.2/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-08-17 04:00:57.000000 carbatpy-0.1.2/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-08-17 04:00:57.000000 carbatpy-0.1.2/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0       29 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/authors.rst
--rw-rw-rw-   0        0        0     1179 2023-12-15 16:55:32.000000 carbatpy-0.1.2/docs/components.rst
--rw-rw-rw-   0        0        0     6536 2024-02-05 15:00:21.000000 carbatpy-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/contributing.rst
--rw-rw-rw-   0        0        0   131534 2024-02-02 12:45:48.000000 carbatpy-0.1.2/docs/explanation-sketch-Ts-property_eval_mixture.jpg
--rw-rw-rw-   0        0        0     3524 2024-02-05 12:33:09.000000 carbatpy-0.1.2/docs/fluid_mixture_search.rst
--rw-rw-rw-   0        0        0     1283 2023-12-15 16:56:54.000000 carbatpy-0.1.2/docs/fluid_props.rst
--rw-rw-rw-   0        0        0     1592 2023-12-15 16:50:24.000000 carbatpy-0.1.2/docs/heat_pump_simple_v2.rst
--rw-rw-rw-   0        0        0     7856 2023-11-06 09:49:40.000000 carbatpy-0.1.2/docs/heat_pump_storage_pairs.png
--rw-rw-rw-   0        0        0       29 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/history.rst
--rw-rw-rw-   0        0        0      591 2023-11-06 09:34:23.000000 carbatpy-0.1.2/docs/index.rst
--rw-rw-rw-   0        0        0     1169 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/installation.rst
--rw-rw-rw-   0        0        0   242694 2023-11-06 07:21:00.000000 carbatpy-0.1.2/docs/last_T_H_dot_plot.png
--rw-rw-rw-   0        0        0   281079 2023-12-14 17:40:21.000000 carbatpy-0.1.2/docs/last_T_H_dot_plot_orc.png
--rwxrwxrwx   0        0        0      806 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0    54341 2023-12-15 16:34:36.000000 carbatpy-0.1.2/docs/orc_structure_Page1.png
--rw-rw-rw-   0        0        0    41372 2023-12-15 16:34:36.000000 carbatpy-0.1.2/docs/orc_structure_Page2.png
--rw-rw-rw-   0        0        0    34537 2023-12-15 16:34:37.000000 carbatpy-0.1.2/docs/orc_structure_Page3.png
--rw-rw-rw-   0        0        0       28 2023-10-14 07:57:08.000000 carbatpy-0.1.2/docs/readme.rst
--rw-rw-rw-   0        0        0      366 2024-02-05 15:18:41.000000 carbatpy-0.1.2/docs/usage.rst
--rw-rw-rw-   0        0        0      687 2024-02-02 16:12:18.000000 carbatpy-0.1.2/docs/utilities.rst
--rw-rw-rw-   0        0        0     1643 2024-02-06 10:39:00.000000 carbatpy-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      403 2024-02-06 11:25:58.773369 carbatpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1592 2024-02-06 10:38:56.000000 carbatpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.744456 carbatpy-0.1.2/tests/
--rw-rw-rw-   0        0        0       39 2023-10-14 07:57:08.000000 carbatpy-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     5768 2024-02-05 16:21:23.000000 carbatpy-0.1.2/tests/test_carbatpy.py
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.589739 carbatpy-0.1.2/tests/test_files/
-drwxrwxrwx   0        0        0        0 2024-02-06 11:25:58.756266 carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/
--rw-rw-rw-   0        0        0   750295 2024-02-05 07:37:53.000000 carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.csv
--rw-rw-rw-   0        0        0   156117 2024-02-05 07:37:53.000000 carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.png
--rw-rw-rw-   0        0        0      418 2024-02-05 07:37:49.000000 carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut_variablen.json
--rw-rw-rw-   0        0        0     1635 2024-02-05 07:37:49.000000 carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37property_eval_mixture.py
--rw-rw-rw-   0        0        0     7537 2024-02-04 14:55:07.000000 carbatpy-0.1.2/tests/test_fluid.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.875617 carbatpy-0.1.3/
+-rw-rw-rw-   0        0        0      174 2023-10-14 07:57:08.000000 carbatpy-0.1.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3661 2023-10-14 07:57:08.000000 carbatpy-0.1.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      228 2024-02-04 15:36:01.000000 carbatpy-0.1.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1093 2023-10-14 07:57:08.000000 carbatpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      377 2024-02-05 17:55:03.000000 carbatpy-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3093 2024-05-16 13:33:44.872241 carbatpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2080 2024-02-06 14:33:29.000000 carbatpy-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.306496 carbatpy-0.1.3/carbatpy/
+-rw-rw-rw-   0        0        0     1238 2024-05-16 13:29:42.000000 carbatpy-0.1.3/carbatpy/__init__.py
+-rw-rw-rw-   0        0        0      904 2024-02-04 10:28:20.000000 carbatpy-0.1.3/carbatpy/carbatpy0.py
+-rw-rw-rw-   0        0        0     1125 2024-02-10 11:09:55.000000 carbatpy-0.1.3/carbatpy/cb_config.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.212450 carbatpy-0.1.3/carbatpy/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.461087 carbatpy-0.1.3/carbatpy/src/data/
+-rw-rw-rw-   0        0        0     1514 2023-12-15 14:39:41.000000 carbatpy-0.1.3/carbatpy/src/data/ORC.gv
+-rw-rw-rw-   0        0        0     1516 2023-12-15 15:04:55.000000 carbatpy-0.1.3/carbatpy/src/data/cycle.gv
+-rw-rw-rw-   0        0        0    10812 2024-01-07 18:03:19.000000 carbatpy-0.1.3/carbatpy/src/data/hp_structure.xlsx
+-rw-rw-rw-   0        0        0    10954 2024-01-07 18:05:37.000000 carbatpy-0.1.3/carbatpy/src/data/orc_structure.xlsx
+-rw-rw-rw-   0        0        0      165 2023-12-15 12:35:13.000000 carbatpy-0.1.3/carbatpy/src/data/~$orc_structure.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.510792 carbatpy-0.1.3/carbatpy/src/helpers/
+-rw-rw-rw-   0        0        0        2 2024-02-04 10:38:35.000000 carbatpy-0.1.3/carbatpy/src/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1635 2024-02-04 15:40:43.000000 carbatpy-0.1.3/carbatpy/src/helpers/file_copy.py
+-rw-rw-rw-   0        0        0     3647 2024-02-04 15:41:13.000000 carbatpy-0.1.3/carbatpy/src/helpers/uncertainty_vol_enthalpy.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.211452 carbatpy-0.1.3/carbatpy/src/models/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.597869 carbatpy-0.1.3/carbatpy/src/models/components/
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:03:56.000000 carbatpy-0.1.3/carbatpy/src/models/components/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-12-16 09:25:05.000000 carbatpy-0.1.3/carbatpy/src/models/components/compressor_simple.py
+-rw-rw-rw-   0        0        0    56438 2024-05-10 10:58:36.000000 carbatpy-0.1.3/carbatpy/src/models/components/compressor_transfer_function.py
+-rw-rw-rw-   0        0        0    16713 2024-05-15 12:21:54.000000 carbatpy-0.1.3/carbatpy/src/models/components/heat_exchanger_thermo_v2.py
+-rw-rw-rw-   0        0        0     1454 2023-11-04 17:22:23.000000 carbatpy-0.1.3/carbatpy/src/models/components/throttle_simple.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.693998 carbatpy-0.1.3/carbatpy/src/models/coupled/
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:03:56.000000 carbatpy-0.1.3/carbatpy/src/models/coupled/__init__.py
+-rw-rw-rw-   0        0        0    20949 2024-05-15 09:02:03.000000 carbatpy-0.1.3/carbatpy/src/models/coupled/heat_pump_simple_v2.py
+-rw-rw-rw-   0        0        0     5738 2024-02-04 16:16:35.000000 carbatpy-0.1.3/carbatpy/src/models/coupled/hp_for_opt.py
+-rw-rw-rw-   0        0        0    17296 2024-04-10 07:49:23.000000 carbatpy-0.1.3/carbatpy/src/models/coupled/orc_simple_v2.py
+-rw-rw-rw-   0        0        0     2717 2023-12-15 17:18:03.000000 carbatpy-0.1.3/carbatpy/src/models/coupled/read_cycle_structure.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.703300 carbatpy-0.1.3/carbatpy/src/models/fluids/
+-rw-rw-rw-   0        0        0        0 2023-10-23 10:08:00.000000 carbatpy-0.1.3/carbatpy/src/models/fluids/__init__.py
+-rw-rw-rw-   0        0        0     8646 2024-02-12 15:19:32.000000 carbatpy-0.1.3/carbatpy/src/models/fluids/fluid_props.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.928450 carbatpy-0.1.3/carbatpy/src/utils/
+-rw-rw-rw-   0        0        0       93 2024-02-04 10:15:41.000000 carbatpy-0.1.3/carbatpy/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     1109 2024-02-17 16:39:21.000000 carbatpy-0.1.3/carbatpy/src/utils/costs_initial.py
+-rw-rw-rw-   0        0        0     6114 2024-05-10 12:55:01.000000 carbatpy-0.1.3/carbatpy/src/utils/curve_min_distance_finder.py
+-rw-rw-rw-   0        0        0      928 2024-02-11 17:52:00.000000 carbatpy-0.1.3/carbatpy/src/utils/curve_min_distance_finder_grad.py
+-rw-rw-rw-   0        0        0     4614 2023-11-08 13:30:05.000000 carbatpy-0.1.3/carbatpy/src/utils/exergy_loss.py
+-rw-rw-rw-   0        0        0     2046 2024-02-18 17:01:11.000000 carbatpy-0.1.3/carbatpy/src/utils/is_eff_xgbooost_sklearn_parallel.py
+-rw-rw-rw-   0        0        0     2850 2024-02-09 13:52:47.000000 carbatpy-0.1.3/carbatpy/src/utils/optimize.py
+-rw-rw-rw-   0        0        0    24041 2024-02-15 14:22:37.000000 carbatpy-0.1.3/carbatpy/src/utils/property_eval_mixture.py
+-rw-rw-rw-   0        0        0    25059 2024-02-28 07:41:04.000000 carbatpy-0.1.3/carbatpy/src/utils/property_eval_mixture_test.py
+-rw-rw-rw-   0        0        0     3384 2024-02-02 16:12:18.000000 carbatpy-0.1.3/carbatpy/src/utils/run_heat_pump_simple.py
+-rw-rw-rw-   0        0        0     3932 2024-02-15 16:02:35.000000 carbatpy-0.1.3/carbatpy/src/utils/run_screening_evaluation.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.868320 carbatpy-0.1.3/carbatpy.egg-info/
+-rw-rw-rw-   0        0        0     3093 2024-05-16 13:33:43.000000 carbatpy-0.1.3/carbatpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3731 2024-05-16 13:33:43.000000 carbatpy-0.1.3/carbatpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:33:43.000000 carbatpy-0.1.3/carbatpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-05 17:10:17.000000 carbatpy-0.1.3/carbatpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       83 2024-05-16 13:33:43.000000 carbatpy-0.1.3/carbatpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       62 2024-05-16 13:33:43.000000 carbatpy-0.1.3/carbatpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.412773 carbatpy-0.1.3/docs/
+-rw-rw-rw-   0        0        0    21076 2023-11-06 12:31:19.000000 carbatpy-0.1.3/docs/2-storage_no_discharge.jpg
+-rw-rw-rw-   0        0        0   661405 2023-10-25 12:03:31.000000 carbatpy-0.1.3/docs/2023-10-25-14-03EthProHexBut.png
+-rw-rw-rw-   0        0        0    53322 2023-12-15 15:28:38.000000 carbatpy-0.1.3/docs/2023-12-15-16-28cycle.png
+-rw-rw-rw-   0        0        0      629 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.215451 carbatpy-0.1.3/docs/_build/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:43.216451 carbatpy-0.1.3/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.419985 carbatpy-0.1.3/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0   661405 2023-10-25 12:03:31.000000 carbatpy-0.1.3/docs/_build/html/_images/2023-10-25-14-03EthProHexBut.png
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.451561 carbatpy-0.1.3/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-08-17 04:00:57.000000 carbatpy-0.1.3/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-08-17 04:00:57.000000 carbatpy-0.1.3/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-08-17 04:00:57.000000 carbatpy-0.1.3/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0       29 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     1179 2023-12-15 16:55:32.000000 carbatpy-0.1.3/docs/components.rst
+-rw-rw-rw-   0        0        0     6536 2024-02-05 15:00:21.000000 carbatpy-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/contributing.rst
+-rw-rw-rw-   0        0        0   131534 2024-02-02 12:45:48.000000 carbatpy-0.1.3/docs/explanation-sketch-Ts-property_eval_mixture.jpg
+-rw-rw-rw-   0        0        0     3524 2024-02-05 12:33:09.000000 carbatpy-0.1.3/docs/fluid_mixture_search.rst
+-rw-rw-rw-   0        0        0     1283 2023-12-15 16:56:54.000000 carbatpy-0.1.3/docs/fluid_props.rst
+-rw-rw-rw-   0        0        0     1592 2023-12-15 16:50:24.000000 carbatpy-0.1.3/docs/heat_pump_simple_v2.rst
+-rw-rw-rw-   0        0        0     7856 2023-11-06 09:49:40.000000 carbatpy-0.1.3/docs/heat_pump_storage_pairs.png
+-rw-rw-rw-   0        0        0       29 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/history.rst
+-rw-rw-rw-   0        0        0      591 2023-11-06 09:34:23.000000 carbatpy-0.1.3/docs/index.rst
+-rw-rw-rw-   0        0        0     1169 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/installation.rst
+-rw-rw-rw-   0        0        0   242694 2023-11-06 07:21:00.000000 carbatpy-0.1.3/docs/last_T_H_dot_plot.png
+-rw-rw-rw-   0        0        0   281079 2023-12-14 17:40:21.000000 carbatpy-0.1.3/docs/last_T_H_dot_plot_orc.png
+-rwxrwxrwx   0        0        0      806 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0    54341 2023-12-15 16:34:36.000000 carbatpy-0.1.3/docs/orc_structure_Page1.png
+-rw-rw-rw-   0        0        0    41372 2023-12-15 16:34:36.000000 carbatpy-0.1.3/docs/orc_structure_Page2.png
+-rw-rw-rw-   0        0        0    34537 2023-12-15 16:34:37.000000 carbatpy-0.1.3/docs/orc_structure_Page3.png
+-rw-rw-rw-   0        0        0       28 2023-10-14 07:57:08.000000 carbatpy-0.1.3/docs/readme.rst
+-rw-rw-rw-   0        0        0      601 2024-02-09 14:19:01.000000 carbatpy-0.1.3/docs/usage.rst
+-rw-rw-rw-   0        0        0      833 2024-02-11 17:58:04.000000 carbatpy-0.1.3/docs/utilities.rst
+-rw-rw-rw-   0        0        0     1643 2024-05-16 13:29:08.000000 carbatpy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      403 2024-05-16 13:33:44.888831 carbatpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1592 2024-02-06 10:38:56.000000 carbatpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.541433 carbatpy-0.1.3/tests/
+-rw-rw-rw-   0        0        0       39 2023-10-14 07:57:08.000000 carbatpy-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     8741 2024-02-12 14:54:37.000000 carbatpy-0.1.3/tests/test_carbatpy.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.598743 carbatpy-0.1.3/tests/test_files/
+-rw-rw-rw-   0        0        0  1110987 2024-02-27 17:13:12.000000 carbatpy-0.1.3/tests/test_files/evaluated.csv
+-rw-rw-rw-   0        0        0  1112630 2024-05-15 08:27:33.000000 carbatpy-0.1.3/tests/test_files/fluid-re-eval.csv
+drwxrwxrwx   0        0        0        0 2024-05-16 13:33:44.863318 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/
+-rw-rw-rw-   0        0        0   750295 2024-02-05 07:37:53.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.csv
+-rw-rw-rw-   0        0        0   156117 2024-02-05 07:37:53.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.png
+-rw-rw-rw-   0        0        0      418 2024-02-05 07:37:49.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut_variablen.json
+-rw-rw-rw-   0        0        0     1635 2024-02-05 07:37:49.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37property_eval_mixture.py
+-rw-rw-rw-   0        0        0   963105 2024-02-14 15:47:41.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-combined.csv
+-rw-rw-rw-   0        0        0   963105 2024-05-15 08:27:31.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-combined0.csv
+-rw-rw-rw-   0        0        0   199393 2024-02-08 10:52:03.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-compressor-Roskosch.csv
+-rw-rw-rw-   0        0        0       91 2024-02-09 13:52:47.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-objectives.txt
+-rw-rw-rw-   0        0        0   142517 2024-02-09 13:52:47.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-pareto.csv
+-rw-rw-rw-   0        0        0   137911 2024-02-09 13:52:47.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-plot.jpg
+-rw-rw-rw-   0        0        0   283480 2024-02-09 15:29:26.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-plot.png
+-rw-rw-rw-   0        0        0   340372 2024-05-15 08:27:32.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut-plot2.png
+-rw-rw-rw-   0        0        0   782200 2024-02-06 15:51:37.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut.csv
+-rw-rw-rw-   0        0        0      478 2024-02-06 15:51:30.000000 carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-06-16-51-ProEthPenBut_variablen.json
+-rw-rw-rw-   0        0        0     8025 2024-02-12 15:24:50.000000 carbatpy-0.1.3/tests/test_fluid.py
```

### Comparing `carbatpy-0.1.2/CONTRIBUTING.rst` & `carbatpy-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/LICENSE` & `carbatpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/PKG-INFO` & `carbatpy-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbatpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Calculate and optimize Carnot Batteries (Thermal energy storage)
 Home-page: https://git.uni-due.de/spp-2403/td-ude/carbatpy
 Author: Burak Atakan
 Author-email: Burak Atakan <b.atakan@uni-duisburg.de>
 License: MIT
 Project-URL: Repository, https://git.uni-due.de/spp-2403/td-ude/carbatpy
 Project-URL: Documentation, https://carbatpy-010.readthedocs.io/en/latest/
@@ -31,33 +31,30 @@
 carbatpy
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/carbatpy.svg
         :target: https://pypi.python.org/pypi/carbatpy
 
-.. image:: https://img.shields.io/travis/h500034/carbatpy.svg
-        :target: https://travis-ci.com/h500034/carbatpy
 
-.. image:: https://readthedocs.org/projects/carbatpy/badge/?version=latest
-        :target: https://carbatpy.readthedocs.io/en/latest/?version=latest
+.. image:: https://readthedocs.org/projects/carbatpy-010/badge/?version=latest
+        :target: https://carbatpy-010.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 
-# carbatpy
 
 Modeling Carnot Batteries (Thermal Energy Storage), a Python package.
  ### THIS is the version with the new directory structure, several files from the previous version are not included yet! (2023-10-23)
 
 This is a project aiming to model thermal energy storages using heat pumps for 
 charging, organic Rankine cycles (ORC) for discharging and different kinds of 
 storages.
 For this, it is planned to use detailed fluid models (as implemented e.g. in 
 REFPROP, CoolProp, or TREND ) and setting up systems which can either be steady 
-state or (later) also unsteady.
+state or (later) also unsteady. For the moment a *Refprop* license is needed.
 Since this project just starts, do not expect too much.
 It is aimed to have heat exchangers, machines and storages as compounds, which 
 can be combined to different charging and dicharging configurations. For these, 
 the energy balance, mass balance and further relations will be applied/solved.
 Later on also thermo-economic calculations are planned.
 
 For the beginning, the solution of the spatially resolved heat exchanger
```

### Comparing `carbatpy-0.1.2/README.rst` & `carbatpy-0.1.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,33 +2,30 @@
 carbatpy
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/carbatpy.svg
         :target: https://pypi.python.org/pypi/carbatpy
 
-.. image:: https://img.shields.io/travis/h500034/carbatpy.svg
-        :target: https://travis-ci.com/h500034/carbatpy
 
-.. image:: https://readthedocs.org/projects/carbatpy/badge/?version=latest
-        :target: https://carbatpy.readthedocs.io/en/latest/?version=latest
+.. image:: https://readthedocs.org/projects/carbatpy-010/badge/?version=latest
+        :target: https://carbatpy-010.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 
-# carbatpy
 
 Modeling Carnot Batteries (Thermal Energy Storage), a Python package.
  ### THIS is the version with the new directory structure, several files from the previous version are not included yet! (2023-10-23)
 
 This is a project aiming to model thermal energy storages using heat pumps for 
 charging, organic Rankine cycles (ORC) for discharging and different kinds of 
 storages.
 For this, it is planned to use detailed fluid models (as implemented e.g. in 
 REFPROP, CoolProp, or TREND ) and setting up systems which can either be steady 
-state or (later) also unsteady.
+state or (later) also unsteady. For the moment a *Refprop* license is needed.
 Since this project just starts, do not expect too much.
 It is aimed to have heat exchangers, machines and storages as compounds, which 
 can be combined to different charging and dicharging configurations. For these, 
 the energy balance, mass balance and further relations will be applied/solved.
 Later on also thermo-economic calculations are planned.
 
 For the beginning, the solution of the spatially resolved heat exchanger
```

### Comparing `carbatpy-0.1.2/carbatpy/__init__.py` & `carbatpy-0.1.3/carbatpy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Top-level package for carbatpy."""
 
 __author__ = """Burak Atakan"""
 __email__ = 'burak.atakan@uni-due.de'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 # __all__ =[]
 import os
 import sys
+import pandas as pd
+
+pd.set_option("mode.copy_on_write", True)
 
 sys.path.insert(0,os.path.abspath('../carbatpy'))
 sys.path.insert(0,os.path.abspath('..'))
 
 try:
-    from cb_config import _T_SURROUNDING, _RESULTS_DIR, _P_SURROUNDING
+    from cb_config import _T_SURROUNDING, _RESULTS_DIR, \
+                            _P_SURROUNDING,_CARBATPY_BASE_DIR
 except:
-    from .cb_config import _T_SURROUNDING, _RESULTS_DIR, _P_SURROUNDING
+    from .cb_config import _T_SURROUNDING, _RESULTS_DIR, \
+                            _P_SURROUNDING,_CARBATPY_BASE_DIR
     
 
 
 import src.models as models
 import src.utils as utils
 import src.helpers as helpers
```

### Comparing `carbatpy-0.1.2/carbatpy/carbatpy0.py` & `carbatpy-0.1.3/carbatpy/carbatpy0.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/data/ORC.gv` & `carbatpy-0.1.3/carbatpy/src/data/ORC.gv`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/data/cycle.gv` & `carbatpy-0.1.3/carbatpy/src/data/cycle.gv`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/data/hp_structure.xlsx` & `carbatpy-0.1.3/carbatpy/src/data/hp_structure.xlsx`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/data/orc_structure.xlsx` & `carbatpy-0.1.3/carbatpy/src/data/orc_structure.xlsx`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/helpers/file_copy.py` & `carbatpy-0.1.3/carbatpy/src/helpers/file_copy.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/helpers/uncertainty_vol_enthalpy.py` & `carbatpy-0.1.3/carbatpy/src/helpers/uncertainty_vol_enthalpy.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/models/components/compressor_simple.py` & `carbatpy-0.1.3/carbatpy/src/models/components/compressor_simple.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/models/components/heat_exchanger_thermo_v2.py` & `carbatpy-0.1.3/carbatpy/src/models/components/heat_exchanger_thermo_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,19 @@
         if h_out_w < state_in_w[2]:
             self.heating = 1  # condenser (heating of the secondary fluid)
         self.calc_type = calc_type
         self.name = name
         self.all_states = np.zeros(
             (points, len(cb.fprop._THERMO_STRING.split(";"))))
         self.h_in_out = np.zeros((2, 4))
+        self.dt_mean = None
+        self.dt_min = None
+        self.dt_max = None
         self.warning = 0
+        self.warning_message = "All o.k."
 
     def pinch_calc(self,  verbose=False):
         """
         Calculate the changes in enthalpy and temperature in the heat exchanger
 
         counter-flow hex assumed! Both flows are isobaric.
         Is used to check, whether the second law is violated. The factor can
@@ -117,14 +121,16 @@
             properties of the working fluid along the heat exchanger
             (T,p,h, etc. see fluid class).
         s_array : array
             properties of the secondary fluid along the heat exchanger
             (T,p,h, etc. see fluid class).
 
         """
+        self.warning = 0
+        self.warning_message = "All o.k."
         w_in = copy.copy(self.fluids[0])
         s_in = copy.copy(self.fluids[1])
 
         w_out = copy.copy(self.fluids[0])  # not yet the correct state!
         s_out = copy.copy(self.fluids[1])
 
         #  fixed values
@@ -160,15 +166,34 @@
                               self.points)
 
         values = np.zeros((self.points, 2))
         values[:, 0] = h_array.T
         values[:, 1] = w_out.properties.pressure
 
         w_array = w_out.set_state_v(values, "HP")
+        # temperature difference, ok?
         d_tempall = w_array[:, 0]-s_array[:, 0]
+        self.dt_mean = d_tempall.mean()
+        self.dt_min = np.abs(d_tempall).min()
+        self.dt_max = np.abs(d_tempall).max()
+        if self.dt_min - self.d_temp_separation_min < -1e-3:
+            self.warning = 900
+            self.warning_message = "Below minumum approch temperature!"
+        positive = np.any(d_tempall > 0)
+        negative = np.any(d_tempall < 0)
+        below =True
+        if self.heating < 0: 
+            below =False
+
+        crossing = (positive > 0 and negative > 0)
+        wrong_side = (positive > 0 and not below) or (negative > 0 and below)
+        if crossing or wrong_side:
+            self.warning = 999
+            self.dt_mean = 1e6
+            self.warning_message = "Temperatures crossing or wrong side!"
 
         # if self.heating:
         #     d_tempall = w_array[:, 0]-s_array[:, 0]
         # else:
         #     d_tempall = w_array[:, 0] - np.flip(s_array[:, 0],axis=0)
         if verbose:
             if self.heating > 0:
@@ -209,23 +234,23 @@
         # reduce both their distance to the required minimum value.
 
         grad = np.gradient(d_temps)
         grad2 = np.gradient(grad)
         idx = np.where(np.sign(grad[:-1]) != np.sign(grad[1:]))[0] + 1
         idx_min = np.where(grad2[idx] > 0)
 
-        if len(idx) > 0:
+        if len(idx) > 0:pinch 
             # wanted =min(d_temps[idx] - self.d_temp_separation_min)
             sum_shifted = np.sum(shifted[idx[idx_min]])
         else:
             sum_shifted = mind_temp
 
         # print(h_out_s,idx, d_temps[idx])
 
-        if (mind_temp <= -5e-6) or (self.m_dot_s <= 0):
+        if (mind_temp <= -5e-6) or (self.m_dot_s <= 0) or self.warning>0:
             return -5e3*mind_temp
 
         # else:
             # mind_temp = np.abs(d_temps).min() # was here before
             # but two values should be at the minimum distance
 
             # value = np.sum(self.d_temp_separation_min -d_temps)
@@ -258,23 +283,24 @@
         verbose = False
 
         x0 = copy.copy(self.h_out_s)
 
         tolerance = 3e-3
 
         try:
-            result = minimize(self.pinch_root, x0)
+            result = minimize(self.pinch_root, x0, tol =tolerance)
 
             if verbose:
                 print(
                     f"result {result}, heating {self.heating}")
 
             if result.success or result.status == 2:
                 if result.status == 2:
                     self.warning = 2  # T-difference probably smaller
+                    self.warning_message ="Minimization problem: "+result.message
 
                 return result.x
 
         # except:
         except Exception as inst:
             print(type(inst))    # the exception type
             print(inst.args)     # arguments stored in .args
@@ -377,47 +403,54 @@
                                state_sec_out[2],
                                d_temp_separation_min=D_TEMP_MIN)
     # ms, d_tempall_first, w, s = hex0.pinch_calc()
     # f, ax_plot = plt.subplots(1)
     # ax_plot.plot((w[:, 2]-w[:, 2].min()) * hex0.m_dot_w, w[:, 0])
     # ax_plot.plot((s[:, 2]-s[:, 2].min()) * hex0.m_dot_s, s[:, 0])
     factor0 = hex0.find_pinch()
+    if hex0.warning> 0:
+        print(hex0.warning_message)
     ms0, d_tempall0, w0, s0 = hex0.pinch_plot("hex-plot.png")
     # print(f"w0 {w0[0]}")
 
     #  Evaporator: ----------------------------
 
     SEC_TEMP_IN = 300.0
-    SEC_TEMP_OUT = 279
+    SEC_TEMP_OUT = 292
     SEC_PRES_IN = 15e5
     H_DOT = 1e3
+    extra = 2
     # D_TEMP_SUPER = 5.
     D_TEMP_MIN = 6.0
     state_sec_out = secFluid.set_state([SEC_TEMP_OUT, SEC_PRES_IN], "TP")
     # this mus be the last set_state before the hex is constructed:
     state_sec_in = secFluid.set_state([SEC_TEMP_IN, SEC_PRES_IN], "TP")
 
     # WF_TEMP_IN = SEC_TEMP_OUT  # - D_TEMP_MIN
-    state_out = myFluid.set_state([SEC_TEMP_IN-D_TEMP_MIN, 1.0], "TQ")
-    state_in = myFluid.set_state([SEC_TEMP_OUT-D_TEMP_MIN, state_out[1]], "TP")
+    state_out = myFluid.set_state([SEC_TEMP_IN-D_TEMP_MIN- extra, 1.0], "TQ")
+    state_in = myFluid.set_state([SEC_TEMP_OUT-D_TEMP_MIN -extra, state_out[1]], "TP")
 
     # print("state in", state_in)
 
     hex1 = StaticHeatExchanger([myFluid, secFluid], H_DOT, state_out[2],
                                state_sec_out[2],
                                d_temp_separation_min=D_TEMP_MIN)
     # ms1, d_tempall1, w1, s1 = hex1.pinch_calc()
     f, ax_plot = plt.subplots(1)
     # ax_plot.plot((w1[:, 2]-w1[:, 2].min()) * hex1.m_dot_w, w1[:, 0])
     # ax_plot.plot((s1[:, 2]-s1[:, 2].min()) * hex1.m_dot_s, s1[:, 0], ":")
 
     factor_out = hex1.find_pinch()
-    ms, d_tempall_second, w1, s1 = hex1.pinch_plot()
-    ax_plot.plot((w1[:, 2]-w1[:, 2].min()) * hex1.m_dot_w, w1[:, 0])
-    ax_plot.plot((s1[:, 2]-s1[:, 2].min()) * hex1.m_dot_s, s1[:, 0], ":")
+    if hex1.warning > 2:
+        print("Second heat exchanger:", hex1.warning_message)
+    else:
+        
+        ms, d_tempall_second, w1, s1 = hex1.pinch_plot()
+        ax_plot.plot((w1[:, 2]-w1[:, 2].min()) * hex1.m_dot_w, w1[:, 0])
+        ax_plot.plot((s1[:, 2]-s1[:, 2].min()) * hex1.m_dot_s, s1[:, 0], ":")
     # # print(f"w {w[0]}")
     # print("hex:",hex1.h_in_out)
 
     # p_out = 5e5
 
     # state_out = throttle(p_out, myFluid)
     # print("Throttle:\nInput:", state_in,"\nOutput:",
```

### Comparing `carbatpy-0.1.2/carbatpy/src/models/components/throttle_simple.py` & `carbatpy-0.1.3/carbatpy/src/models/components/throttle_simple.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/models/coupled/heat_pump_simple_v2.py` & `carbatpy-0.1.3/carbatpy/src/models/coupled/heat_pump_simple_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,22 +34,26 @@
 
         storages at two different temperatures, always starting at room
         temperature (around 300K). The minimum and maximum temperatures aof all
         storags are fixed and the heat flow rate to the high-T storage are
         given. Also, isentropic efficiencies.
         Example for the fixed points::
 
-        fixed_points = {"eta_s": 0.65,
-                        "p_low": p_low,
-                        "p_high": p_high,
-                        "T_hh": _HIGH_T_STORAGE_HIGH_TEMP,
-                        "T_hl": _HIGH_T_STORAGE_LOW_TEMP,
-                        "T_lh": _LOW_T_STORAGE_HIGH_TEMP,
-                        "T_ll": _LOW_T_STORAGE_LOW_TEMP,
-                        "Q_dot_h": 3000.0,
+        fixed_points = {"eta_s": _ETA_S_,
+                        "p_low": state_out_evap[1],
+                        "p_high": state_in_cond[1],
+                        "T_hh": _STORAGE_T_OUT_,
+                        "h_h_out_sec": state_sec_out[2],
+                        "h_h_out_w": state_out_cond[2],
+                        "h_l_out_cold": state_cold_out[2],
+                        "h_l_out_w": state_out_evap[2],
+                        "T_hl": _STORAGE_T_IN_,
+                        "T_lh": _STORAGE_T_IN_,
+                        "T_ll": _COLD_STORAGE_T_OUT_,  # 256.0,
+                        "Q_dot_h": _Q_DOT_MIN_,
                         "d_temp_min": _D_T_MIN_}
 
         Parameters
         ----------
         fluids : list of three Fluid
             working fluid, secondary fluid to store at high T, cold fluid
             to store at low T.
@@ -68,14 +72,15 @@
 
         """
         self.components = components
         self.fixed_points = fixed_points
         self.fluids = fluids
         self.all_states = []
         self.m_dots = []
+        self.warning = 0
         self.evaluation = {"Q_dot_h": self.fixed_points["Q_dot_h"],
                            "Power": 0.0,
                            "T_hh": self.fixed_points["T_hh"],
                            "T_ll": self.fixed_points["T_ll"],
                            "exergy_loss_rate": 0}
 
     def calculate_hex(self, fluid_numbers, h_dot_min_, h_out_w_, h_limit_s_=np.NAN,
@@ -121,14 +126,17 @@
         hex_act = \
             cb.hex_th.StaticHeatExchanger([w_actual,
                                            s_actual],
                                           h_dot_min_, h_out_w_, h_limit_s_,
                                           d_temp_separation_min=d_temp_separation_min_,
                                           name=name_)
         h_s_out = hex_act.find_pinch()
+        if hex_act.warning>0: 
+            print("Heat-Exchanger problem: ", hex_act.warning, hex_act.warning_message)
+            self.warning = 999
         m_dot_s, d_tempall, wf_states, sf_states =\
             hex_act.pinch_plot(plotting=verbose_)
 
         self.all_states.append(wf_states)
         self.all_states.append(sf_states)
         self.m_dots.append(hex_act.m_dot_w)
         self.m_dots.append(m_dot_s)
@@ -157,15 +165,15 @@
 
     def calc_p_high(self, temps_wanted, verbose=False):
         """
         calculate a simple compression heat pump
 
         working with two sensible storages (or source and sink). At the moment
         the compressor model is just for a constant isentropic efficiency.
-        An isenthalpic throttle is used for expnsion. The initial states are provided
+        An isenthalpic throttle is used for expansion. The initial states are provided
         by the Fluid-instances. The pressures have to be selected carefully,
         they are not tested at the moment. The two desired storage temperatures
         are an input, and will be varied to meet the desired minmum approach
         temperatures in the heat exchangers.
         For optimization, the pressure levels of the cycle could be used within
         a second script. Several parameters are fixed
         along a calculation, this is in the dictionary "self.fixed_points".
@@ -379,15 +387,15 @@
                    delimiter=";", header=";".join(names))
 
 
 if __name__ == "__main__":
 
     FLUID = "Propane * Butane * Pentane * Hexane"
     comp = [.75, 0.05, 0.15, 0.05]
-    # comp = [0.4,	0.3,	0.3, 0.0]  # [0.164,.3330,.50300,0.0]
+    comp = [0.4,	0.3,	0.3, 0.0]  # [0.164,.3330,.50300,0.0]
 
     FLS = "Water"  #
     FLCOLD = "Methanol"  # "Water"  #
 
     flm = cb.fprop.FluidModel(FLUID)
     myFluid = cb.fprop.Fluid(flm, comp)
```

### Comparing `carbatpy-0.1.2/carbatpy/src/models/coupled/hp_for_opt.py` & `carbatpy-0.1.3/carbatpy/src/models/coupled/hp_for_opt.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/models/coupled/orc_simple_v2.py` & `carbatpy-0.1.3/carbatpy/src/models/coupled/orc_simple_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,26 +32,38 @@
     def __init__(self,  fluids, fixed_points, components=[]):
         """
         Heat pump class for simple thermodynamic calculations for energy storage
 
         storages at two different temperatures, always starting at room
         temperature (around 300K). The minimum and maximum temperatures aof all
         storags are fixed and the heat flow rate to the high-T storage are
-        given. Also, isentropic efficiencies.
+        given. Also, isentropic efficiencies. The COP_charging is important
+        to reach a steady state. At the moment you will have to look it up from
+        the heat pump calculation. It is used to divide the energy transfered to
+        the envoronment and to the low temperature storage.
         Example for::
 
-        fixed_points = {"eta_s": 0.65,
+        fixed_points = {"eta_s": _ETA_S_,  # expander
+                        "eta_s_p": _ETA_S_P_,  # pump
                         "p_low": p_low,
                         "p_high": p_high,
-                        "T_hh": _HIGH_T_STORAGE_HIGH_TEMP,
-                        "T_hl": _HIGH_T_STORAGE_LOW_TEMP,
-                        "T_lh": _LOW_T_STORAGE_HIGH_TEMP,
-                        "T_ll": _LOW_T_STORAGE_LOW_TEMP,
-                        "Q_dot_h": 3000.0,
-                        "d_temp_min": _D_T_MIN_}
+                        "T_hh": _STORAGE_T_IN_,
+                        "h_h_out_sec": state_sec_out[2],
+                        "h_h_out_w": state_out_evap[2],
+                        "h_l_out_cold": state_cold_out[2],
+                        "h_l_out_w": state_out_cond[2],
+                        "h_env_in": state_env_in[2],
+                        "h_env_out": state_env_out[2],
+                        "T_hl": _STORAGE_T_OUT_,
+                        "T_lh": _COLD_STORAGE_T_OUT_,
+                        "T_ll": _COLD_STORAGE_T_IN_,  # 256.0,
+                        "Q_dot_h": _Q_DOT_MIN_,
+                        "d_temp_min": _D_T_MIN_,
+                        "cop_charging": _COP_CHARGING  # needed to calculate Q_env_discharging
+                        }
 
         Parameters
         ----------
         fluids : list of three Fluid
             working fluid, secondary fluid to store at high T, cold fluid
             to store at low T.
         fixed_points : Dictionary
@@ -321,15 +333,15 @@
     _COLD_STORAGE_T_IN_ = 260.15
     _STORAGE_P_IN_ = 5e5
     _COLD_STORAGE_P_IN_ = 5e5
     _ENV_P_IN_ = 5e5
     _Q_DOT_MIN_ = 1e3  # and heat_flow rate (W)
     _D_T_SUPER_ = 5  # super heating of working fluid
     _D_T_MIN_ = 4.  # minimum approach temperature (pinch point)
-    _COP_CHARGING = 3.14  # needed to calculate Q_env_discharging
+    _COP_CHARGING = 3.144  # needed to calculate Q_env_discharging
     _T_REDUCTION_EVAP = -27  # if the curves cross in the evaporator this parameter may help
 
     # environment for heat transfer
     state_env_out = envFluid.set_state([_ENV_T_OUT_, _ENV_P_IN_], "TP")
     state_env_in = envFluid.set_state([_ENV_T_IN_, _ENV_P_IN_], "TP")
 
     # high T-storages
```

### Comparing `carbatpy-0.1.2/carbatpy/src/models/coupled/read_cycle_structure.py` & `carbatpy-0.1.3/carbatpy/src/models/coupled/read_cycle_structure.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/models/fluids/fluid_props.py` & `carbatpy-0.1.3/carbatpy/src/models/fluids/fluid_props.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 import os
 # from time import time
 from ctREFPROP.ctREFPROP import REFPROPFunctionLibrary
 import numpy as np
 # import CoolProp.CoolProp as CP
 
 
-os.environ['RPPREFIX'] = r'C:/Program Files (x86)/REFPROP'
-os.environ['RPPREFIXs'] = r'C:/Program Files (x86)/REFPROP/secondCopyREFPROP'
+# os.environ['RPPREFIX'] = r'C:/Program Files (x86)/REFPROP'
+# os.environ['RPPREFIXs'] = r'C:/Program Files (x86)/REFPROP/secondCopyREFPROP'
 _PROPS = "REFPROP"  # or "CoolProp"
 
 _fl_properties_names = ("Temperature", "Pressure", "spec_Enthalpy",
                         "spec_Volume", "spec_Entropy", "quality",
                         "spec_internal_Energy",
                         "viscosity", "thermal_conductivity",
-                        "Prandtl_number", "k_viscosity", "molecular_mass")
+                        "Prandtl_number", "k_viscosity", "molecular_mass",
+                        "speed_of_sound")
 _THERMO_STRING = "T;P;H;V;S;QMASS;E"
-_TRANS_STRING = _THERMO_STRING + ";VIS;TCX;PRANDTL;KV;M"
+_TRANS_STRING = _THERMO_STRING + ";VIS;TCX;PRANDTL;KV;M;W"
 _TV_STRING = "T;V"
 _T_SURROUNDING = 288.15 # K
 
 # order for coolprop,alle_0:[_temp, p,  h, 1/ rho, s,x,cp, mu,  lambda_s,
 # prandtl, phase]"
 _UNITS = 21
 rp_instance = ""
@@ -118,24 +119,33 @@
         self.sp_volume = state.Output[1]
         self.state = state.Output[:1]
 
 
 class FluidStateTransport(FluidState):
     def __init__(self, state):
         super().__init__(state)
-        # ";VIS;TCX;PRANDTL;KV;M"
+        # ";VIS;TCX;PRANDTL;KV;M;W"
         self.viscosity = state.Output[7]
         self.thermal_conductivity = state.Output[8]
         self.prandtl = state.Output[9]
         self.kin_viscosity = state.Output[10]
         self.molecular_mass = state.Output[11]
-        self.transport = state.Output[7:12]
+        self.speed_of_sound =state.Output[12]
+        self.transport = state.Output[7:13]
+        self.state = state.Output[:13]
 
 
 class Fluid:
+    """ 
+    The Fluid class is used to set, get, and print states of  a fluid with a given
+    
+    model (e.g. RefProp). The compounds are set in the fluidmodel, while the
+    composition is also set here.
+    
+    """
 
     def __init__(self, fluidmodel, composition=[1.0],
                  option=1):
         self.fluidmodel = fluidmodel
         self.composition = composition
         self.option = option
         self.no_compounds = len(composition)
@@ -190,14 +200,37 @@
     def print_state(self):
         pr = self.properties
         flm = self.fluidmodel
         print(f"\n{flm.fluid}, composition: {self.composition}")
         print(f"T:{pr.temperature:.2f} K, p: {pr.pressure/1e5 :.2f} bar,  h: {pr.enthalpy/1000: .2f} kJ/kg, s: {pr.entropy/1000:.3f} kJ/kg K\n")
         if pr.quality >= 0:
             print(f"Quality: {pr.quality :.3f}")
+            
+    def calc_temp_mean(self, h_final):
+        """
+        Calculate the thermodynamic mean temperature between the actual state
+        
+        and the final enthalpy along an isobaric (Delta h /Delta s)
+
+        Parameters
+        ----------
+        h_final : float
+            enthalpy of he final stat.
+
+        Returns
+        -------
+        temp_mean : float
+            the thermodynamic mean temperature.
+
+        """
+        actual_props = self.properties.state
+        final_props = self.set_state([h_final, actual_props[1]], "HP")
+        temp_mean = (final_props[2] - actual_props[2]) \
+            / (final_props[4] - actual_props[4]) 
+        return temp_mean
     
 
 if __name__ == "__main__":
     FLUID = "Propane * Pentane"
     comp = [.50, 0.5]
     flm = FluidModel(FLUID)
     myFluid = Fluid(flm, comp)
@@ -205,13 +238,16 @@
     st1 = myFluid.set_state([300., 1e5], "TP",
                             _TRANS_STRING)
     print(st0, st1)
     myFluid.print_state()
     myFluid.set_composition([.2, .8])
     st0 = myFluid.set_state([300., 1e5], "TP", composition=[.35, .65])
     myFluid.print_state()
+    
+    mean_temp_act = myFluid.calc_temp_mean(st0[2]+1e5)
+    print(f"Mean Temperature {mean_temp_act} K")
 
     # value_vec = np.array([[300, 1e5], [400, 1e5], [500, 1e5]])
     # stv = myFluid.set_state_v(value_vec, "TP")
 
     # print(myFluid.set_state_v(value_vec, "TP"))
     # print(myFluid.set_state([300., 1.], "TQ"))
```

### Comparing `carbatpy-0.1.2/carbatpy/src/utils/curve_min_distance_finder.py` & `carbatpy-0.1.3/carbatpy/src/utils/curve_min_distance_finder_grad.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 @author: atakan
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 
+
 x = np.linspace(0, 12)
 shift =1
 line = -1.9*x + 5+shift
-second = np.sin(x) - 2 * x + 4
+second = 5*np.sin(x) + 5 * x + 4
 
 f,ax = plt.subplots(1,1)
 ax.plot(x,line)
 ax.plot(x,second)
 difference =line-second
 #difference[25] =1
 ax.plot(x,difference,"v")
```

### Comparing `carbatpy-0.1.2/carbatpy/src/utils/exergy_loss.py` & `carbatpy-0.1.3/carbatpy/src/utils/exergy_loss.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy/src/utils/optimize.py` & `carbatpy-0.1.3/carbatpy/src/utils/optimize.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,22 +57,26 @@
         return results
 
     print("keys do not fit, they should be one of:", c_names)
     return []
 
 
 if __name__ == "__main__":
-    FILENAME_ACT = r"C:\Users\atakan\sciebo\results\testing\\"
-    FILENAME_ACT += r"test_data_ProEthPenBut\2024-02-05-08-37-ProEthPenBut.csv"
-    objectives_act = ['p_ratio', 'T_glide_h', 'spec_Volume_sup', 'COP_is'] # 'spec. Volume_sup',
+    FILENAME_ACT = r"C:\Users\atakan\sciebo\Python\carbatpy\tests\test_files\test_data_ProEthPenBut"
+    FILENAME_ACT += r"\\2024-02-06-16-51-ProEthPenBut"
+    objectives_act = ['p_ratio', 'T_glide_h', 'spec_Volume_sup', 'COP_is80'] # 'spec. Volume_sup',
     sense = ["min", "min", "min", "max"]
     obj_sense = [objectives_act, sense]
-    res = pandas.read_csv(FILENAME_ACT)
+    res = pandas.read_csv(FILENAME_ACT+".csv")
 
-    opti = pareto(FILENAME_ACT, obj_sense)
+    opti = pareto(FILENAME_ACT+".csv", obj_sense)
     optimal_data = opti["all_values"][opti["optimal_mask"]]
+    optimal_data.to_csv(FILENAME_ACT+"-pareto.csv")
+    with open(FILENAME_ACT+"-objectives.txt", "w", encoding="utf-8") as file:
+              file.write(str(list(zip(objectives_act,sense))))
 
     graph = sbn.relplot(data=optimal_data,
                         y=objectives_act[-1],
                         hue=objectives_act[0],
                         size=objectives_act[1],
                         x=r'spec_Volume_sup')
+    graph.savefig(FILENAME_ACT+"-plot.jpg", dpi =300)
```

### Comparing `carbatpy-0.1.2/carbatpy/src/utils/run_heat_pump_simple.py` & `carbatpy-0.1.3/carbatpy/src/utils/run_heat_pump_simple.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/carbatpy.egg-info/PKG-INFO` & `carbatpy-0.1.3/carbatpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbatpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Calculate and optimize Carnot Batteries (Thermal energy storage)
 Home-page: https://git.uni-due.de/spp-2403/td-ude/carbatpy
 Author: Burak Atakan
 Author-email: Burak Atakan <b.atakan@uni-duisburg.de>
 License: MIT
 Project-URL: Repository, https://git.uni-due.de/spp-2403/td-ude/carbatpy
 Project-URL: Documentation, https://carbatpy-010.readthedocs.io/en/latest/
@@ -31,33 +31,30 @@
 carbatpy
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/carbatpy.svg
         :target: https://pypi.python.org/pypi/carbatpy
 
-.. image:: https://img.shields.io/travis/h500034/carbatpy.svg
-        :target: https://travis-ci.com/h500034/carbatpy
 
-.. image:: https://readthedocs.org/projects/carbatpy/badge/?version=latest
-        :target: https://carbatpy.readthedocs.io/en/latest/?version=latest
+.. image:: https://readthedocs.org/projects/carbatpy-010/badge/?version=latest
+        :target: https://carbatpy-010.readthedocs.io/en/latest/
         :alt: Documentation Status
 
 
-# carbatpy
 
 Modeling Carnot Batteries (Thermal Energy Storage), a Python package.
  ### THIS is the version with the new directory structure, several files from the previous version are not included yet! (2023-10-23)
 
 This is a project aiming to model thermal energy storages using heat pumps for 
 charging, organic Rankine cycles (ORC) for discharging and different kinds of 
 storages.
 For this, it is planned to use detailed fluid models (as implemented e.g. in 
 REFPROP, CoolProp, or TREND ) and setting up systems which can either be steady 
-state or (later) also unsteady.
+state or (later) also unsteady. For the moment a *Refprop* license is needed.
 Since this project just starts, do not expect too much.
 It is aimed to have heat exchangers, machines and storages as compounds, which 
 can be combined to different charging and dicharging configurations. For these, 
 the energy balance, mass balance and further relations will be applied/solved.
 Later on also thermo-economic calculations are planned.
 
 For the beginning, the solution of the spatially resolved heat exchanger
```

### Comparing `carbatpy-0.1.2/docs/2-storage_no_discharge.jpg` & `carbatpy-0.1.3/docs/2-storage_no_discharge.jpg`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/2023-10-25-14-03EthProHexBut.png` & `carbatpy-0.1.3/docs/2023-10-25-14-03EthProHexBut.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/2023-12-15-16-28cycle.png` & `carbatpy-0.1.3/docs/2023-12-15-16-28cycle.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/Makefile` & `carbatpy-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/_build/html/_images/2023-10-25-14-03EthProHexBut.png` & `carbatpy-0.1.3/docs/_build/html/_images/2023-10-25-14-03EthProHexBut.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/components.rst` & `carbatpy-0.1.3/docs/components.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/conf.py` & `carbatpy-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/explanation-sketch-Ts-property_eval_mixture.jpg` & `carbatpy-0.1.3/docs/explanation-sketch-Ts-property_eval_mixture.jpg`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/fluid_mixture_search.rst` & `carbatpy-0.1.3/docs/fluid_mixture_search.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/fluid_props.rst` & `carbatpy-0.1.3/docs/fluid_props.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/heat_pump_simple_v2.rst` & `carbatpy-0.1.3/docs/heat_pump_simple_v2.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/heat_pump_storage_pairs.png` & `carbatpy-0.1.3/docs/heat_pump_storage_pairs.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/index.rst` & `carbatpy-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/installation.rst` & `carbatpy-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/last_T_H_dot_plot.png` & `carbatpy-0.1.3/docs/last_T_H_dot_plot.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/last_T_H_dot_plot_orc.png` & `carbatpy-0.1.3/docs/last_T_H_dot_plot_orc.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/make.bat` & `carbatpy-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/orc_structure_Page1.png` & `carbatpy-0.1.3/docs/orc_structure_Page1.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/orc_structure_Page2.png` & `carbatpy-0.1.3/docs/orc_structure_Page2.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/orc_structure_Page3.png` & `carbatpy-0.1.3/docs/orc_structure_Page3.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/docs/utilities.rst` & `carbatpy-0.1.3/docs/utilities.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 
 
 .. automodule:: src.utils.exergy_loss
     :members:
     :undoc-members:
     :show-inheritance:
     :inherited-members:
+    
+
+.. automodule:: src.utils.curve_min_distance_finder
+    :members:
+    :undoc-members:
+    :show-inheritance:
+    :inherited-members:
 
 
 
 Helpers
 ====================
 
 Some helper functions, found at src\\helpers
```

### Comparing `carbatpy-0.1.2/pyproject.toml` & `carbatpy-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2263 6172 6261 7470  .name = "carbatp
 00000070: 7922 0d0a 7665 7273 696f 6e20 3d20 2230  y"..version = "0
-00000080: 2e31 2e32 220d 0a61 7574 686f 7273 203d  .1.2"..authors =
+00000080: 2e31 2e33 220d 0a61 7574 686f 7273 203d  .1.3"..authors =
 00000090: 205b 0d0a 2020 2020 7b20 6e61 6d65 203d   [..    { name =
 000000a0: 2022 4275 7261 6b20 4174 616b 616e 222c   "Burak Atakan",
 000000b0: 2065 6d61 696c 203d 2022 622e 6174 616b   email = "b.atak
 000000c0: 616e 4075 6e69 2d64 7569 7362 7572 672e  an@uni-duisburg.
 000000d0: 6465 227d 2c0d 0a20 2020 205d 0d0a 6465  de"},..    ]..de
 000000e0: 7363 7269 7074 696f 6e20 3d20 2243 616c  scription = "Cal
 000000f0: 6375 6c61 7465 2061 6e64 206f 7074 696d  culate and optim
```

### Comparing `carbatpy-0.1.2/setup.py` & `carbatpy-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/tests/test_carbatpy.py` & `carbatpy-0.1.3/tests/test_carbatpy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python
 
 """Tests for `carbatpy` package."""
 
 import os
 import unittest
+import numpy as np
+import pandas as pd
 
 import carbatpy as cbp
 
 
 class TestCarbatpy(unittest.TestCase):
     """Tests for `carbatpy` package."""
 
@@ -15,24 +17,24 @@
         """Set up test fixtures, if any."""
 
     def tearDown(self):
         """Tear down test fixtures, if any."""
 
     def test_000_pareto_opt_screened(self):
         """Test the pareto function within utils.optimize."""
-        global _DIR
-        directory = os.getcwd()
-        filename =  directory + r"\\tests\\test_files\\"
+
+        directory = cbp._CARBATPY_BASE_DIR
+        filename = directory + r"\\tests\\test_files\\"
         filename += r"test_data_ProEthPenBut\2024-02-05-08-37-ProEthPenBut.csv"
-        objectives = objectives_act =['p_ratio', 'T_glide_h','COP_is']
+        objectives = objectives_act = ['p_ratio', 'T_glide_h', 'COP_is']
         sense = ["min", "min", "max"]
-        obj_sense =[objectives_act, sense]
+        obj_sense = [objectives_act, sense]
         optimal_values = cbp.utils.optimize.pareto(filename, obj_sense)
         self.assertTrue(len(optimal_values) > 0)
-        
+
     def test_001_simple_orc(self):
         """Test the simple orc calculation with two storages and 
         heat transfer to the environment."""
         FLUID = "Propane * Butane * Pentane * Hexane"
         comp = [.75, 0.05, 0.15, 0.05]
         comp = [0.4,	0.3,	0.3, 0.0]  # [0.164,.3330,.50300,0.0]
 
@@ -73,16 +75,18 @@
         _T_REDUCTION_EVAP = -27  # if the curves cross in the evaporator this parameter may help
 
         # environment for heat transfer
         state_env_out = envFluid.set_state([_ENV_T_OUT_, _ENV_P_IN_], "TP")
         state_env_in = envFluid.set_state([_ENV_T_IN_, _ENV_P_IN_], "TP")
 
         # high T-storages
-        state_sec_out = secFluid.set_state([_STORAGE_T_OUT_, _STORAGE_P_IN_], "TP")
-        state_sec_in = secFluid.set_state([_STORAGE_T_IN_, _STORAGE_P_IN_], "TP")
+        state_sec_out = secFluid.set_state(
+            [_STORAGE_T_OUT_, _STORAGE_P_IN_], "TP")
+        state_sec_in = secFluid.set_state(
+            [_STORAGE_T_IN_, _STORAGE_P_IN_], "TP")
 
         #  low T sorages:
         state_cold_out = coldFluid.set_state(
             [_COLD_STORAGE_T_OUT_, _COLD_STORAGE_P_IN_], "TP")
         state_cold_in = coldFluid.set_state(
             [_COLD_STORAGE_T_IN_, _COLD_STORAGE_P_IN_], "TP")
 
@@ -95,15 +99,16 @@
         T_OUT = _STORAGE_T_IN_ - _D_T_MIN_
         # Evaporator input comes from the pump-output
 
         state_out_evap = myFluid.set_state([p_high,
                                             T_OUT], "PT")
         # low pressure, condenser # BA 2023-11-14 three points needed: low, environment and slightly higher
         T_SATL = _COLD_STORAGE_T_IN_ + _D_T_MIN_
-        state_out_cond = myFluid.set_state([T_SATL, 0.], "TQ")  # find low pressure
+        state_out_cond = myFluid.set_state(
+            [T_SATL, 0.], "TQ")  # find low pressure
         p_low = state_out_cond[1]
         # BA changed 2023-12-13 the fixed starting point for the cycle is the  fluid
         # state before the pump now.
 
         # the other states in the condenser are fixed by the expander outlet and
         # the Q_total : Q_low_stored ratio    eventually p_low must be varied until
         # the balance is fulfilled, since m_dot_w is fixed by the evaporator!
@@ -125,12 +130,73 @@
                         "Q_dot_h": _Q_DOT_MIN_,
                         "d_temp_min": _D_T_MIN_,
                         "cop_charging": _COP_CHARGING  # needed to calculate Q_env_discharging
                         }
 
         orc0 = cbp.orc_simple.OrganicRankineCycle(
             [myFluid, secFluid, envFluid, coldFluid], FIXED_POINTS)
-        eta_dis = orc0.calc_orc(True)
+        eta_dis = orc0.calc_orc(False)
         self.assertAlmostEqual(0.053007094612255716, eta_dis, places=14)
 
+    def test_002_combine_fluid_screening_data_frames(self):
+        """Test the combination of two dataframes function within
+        utils.optimize."""
+
+        directory = cbp._CARBATPY_BASE_DIR
+        directory += "\\tests\\test_files\\"
+
+        filename1 = directory + r"test_data_ProEthPenBut\2024-02-06-16-51-ProEthPenBut.csv"
+        filename2 = directory + \
+            r"test_data_ProEthPenBut\2024-02-06-16-51-ProEthPenBut-compressor-Roskosch.csv"
+        combined_data = cbp.utils.property_eval_mixture.combine([filename1,
+                                                                filename2],
+                                                                filename_out="automatic")
+
+        self.assertTrue(len(combined_data) > 0)
+
+    def test_003_plot_data_frame(self):
+        """Tplot the columns of a dataframe within
+        utils.optimize."""
+
+        directory = cbp._CARBATPY_BASE_DIR
+        directory += "\\tests\\test_files\\"
+
+        filename = directory + r"test_data_ProEthPenBut\2024-02-06-16-51-ProEthPenBut.csv"
+        what = {"x": 'spec_Volume_sup', "y": 'COP_is80', "hue": 'T_glide_h',
+                "size": 'p_ratio', 'style': 'Temperature_hplt'}
+        success = cbp.utils.property_eval_mixture.data_plot(filename, what,
+                                                            filename_out="automatic")
+
+        self.assertTrue(success)
+
+    def test_004_evaluate_data_(self):
+        """Evaluate the data in the dataFrame, when the isentropic efficiencies
+        are calculated. Typically using '-combined'-files"""
+
+        directory = cbp._CARBATPY_BASE_DIR
+        directory += "\\tests\\test_files\\"
+        filename = directory + r"test_data_ProEthPenBut\2024-02-06-16-51-ProEthPenBut-combined.csv"
+        data = pd.read_csv(filename)
+        initial =len(data.columns)
+
+        data_out = cbp.utils.property_eval_mixture.eval_is_eff_roskosch(data,
+                                                                        file_out=directory+"fluid-re-eval.csv")
+        self.assertTrue(len(data_out.columns) > initial)
+        
+    def test_005_curve_dist_find(self):
+        """Evaluate the data in the dataFrame, when the isentropic efficiencies
+        are calculated. Typically using '-combined'-files"""
+
+        x_val = np.linspace(1, 12)
+        # test points
+        y_val = -5*np.sin(x_val) + 5 * x_val + 4 - 100/x_val
+        values_act = np.array([x_val, y_val])
+        solution_below = cbp.curve_min_distance_finder.find_min_approach(values_act, True)
+        solution_above = cbp.curve_min_distance_finder.find_min_approach(values_act, False)
+        self.assertTrue(solution_below["success"])
+        self.assertTrue(solution_above["success"])
+        self.assertAlmostEqual(solution_below["integral"],
+                               356.82447354719505, places=14)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.csv` & `carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.csv`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.png` & `carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37-ProEthPenBut.png`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37property_eval_mixture.py` & `carbatpy-0.1.3/tests/test_files/test_data_ProEthPenBut/2024-02-05-08-37property_eval_mixture.py`

 * *Files identical despite different names*

### Comparing `carbatpy-0.1.2/tests/test_fluid.py` & `carbatpy-0.1.3/tests/test_fluid.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,28 @@
         self.flm = cb.fprop.FluidModel(fluid_mixture)
         print(self.flm.fluid)
         comp = [.50, 0.5]
         self.my_fluid = cb.fprop.Fluid(self.flm, comp)
         st0 = self.my_fluid.set_state([300., 1e5], "TP")
         self.assertAlmostEqual(self.my_fluid.properties.enthalpy,
                                453021.3769789692, places=14)
+        # transport properties, speed od sound
+        st1 = self.my_fluid.set_state([300., 1e5], "TP",
+                                cb.fprop._TRANS_STRING)
+        self.assertAlmostEqual(self.my_fluid.properties.speed_of_sound,
+                               2.1158293060385915e+02, places=14)
 
         # fluid, different composition
         st0 = self.my_fluid.set_state([300., 1e5], "TP", composition=[.35, .65])
         self.assertAlmostEqual(self.my_fluid.properties.enthalpy,
                                414499.55081964, places=14)
+        
+        mean_temp_act = self.my_fluid.calc_temp_mean(st0[2]+1e5)
+        self.assertAlmostEqual(mean_temp_act,
+                               327.2548125203546, places=14)
 
         # Water
         self.flm = cb.fprop.FluidModel("Water")
         self.my_fluid = cb.fprop.Fluid(self.flm, [1])
         st0 = self.my_fluid.set_state([300., 1e5], "TP")
         self.assertAlmostEqual(self.my_fluid.properties.enthalpy,
                                112653.67968890067, places=14)
```

