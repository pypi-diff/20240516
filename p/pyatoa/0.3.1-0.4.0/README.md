# Comparing `tmp/pyatoa-0.3.1.tar.gz` & `tmp/pyatoa-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatoa-0.3.1.tar", last modified: Fri Sep  8 02:54:41 2023, max compression
+gzip compressed data, was "pyatoa-0.4.0.tar", last modified: Thu May 16 19:45:08 2024, max compression
```

## Comparing `pyatoa-0.3.1.tar` & `pyatoa-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.178738 pyatoa-0.3.1/
--rw-r--r--   0 chow       (501) staff       (20)    35149 2022-12-07 21:52:28.000000 pyatoa-0.3.1/LICENSE.txt
--rw-r--r--   0 chow       (501) staff       (20)    43077 2023-09-08 02:54:41.178514 pyatoa-0.3.1/PKG-INFO
--rw-r--r--   0 chow       (501) staff       (20)     1732 2023-03-01 01:06:49.000000 pyatoa-0.3.1/README.md
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.172677 pyatoa-0.3.1/docs/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-21 00:49:30.000000 pyatoa-0.3.1/docs/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)     6472 2023-09-03 07:07:20.000000 pyatoa-0.3.1/docs/conf.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.172798 pyatoa-0.3.1/pyatoa/
--rw-r--r--   0 chow       (501) staff       (20)      672 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/__init__.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.173993 pyatoa-0.3.1/pyatoa/core/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/core/__init__.py
--rwxr-xr-x   0 chow       (501) staff       (20)    22043 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/core/config.py
--rwxr-xr-x   0 chow       (501) staff       (20)    12488 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/core/executive.py
--rwxr-xr-x   0 chow       (501) staff       (20)    50564 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/core/inspector.py
--rwxr-xr-x   0 chow       (501) staff       (20)    57375 2023-09-08 02:53:09.000000 pyatoa-0.3.1/pyatoa/core/manager.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.174560 pyatoa-0.3.1/pyatoa/scripts/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/scripts/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)     2254 2022-12-21 00:49:30.000000 pyatoa-0.3.1/pyatoa/scripts/data_data_example.py
--rw-r--r--   0 chow       (501) staff       (20)     2408 2023-02-28 22:36:23.000000 pyatoa-0.3.1/pyatoa/scripts/load_example_data.py
--rwxr-xr-x   0 chow       (501) staff       (20)     6262 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/scripts/process_data_w_mpi.py
--rw-r--r--   0 chow       (501) staff       (20)     2030 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/scripts/syn_syn_example.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.175674 pyatoa-0.3.1/pyatoa/tests/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/tests/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)     7038 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_asdf_utils.py
--rw-r--r--   0 chow       (501) staff       (20)     3023 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_config.py
--rw-r--r--   0 chow       (501) staff       (20)     3737 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/tests/test_executive.py
--rw-r--r--   0 chow       (501) staff       (20)     5915 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/tests/test_inspector.py
--rw-r--r--   0 chow       (501) staff       (20)    10352 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_manager.py
--rw-r--r--   0 chow       (501) staff       (20)     2832 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_mgmt_plot.py
--rw-r--r--   0 chow       (501) staff       (20)     4830 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_process_util.py
--rw-r--r--   0 chow       (501) staff       (20)     5940 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_utils.py
--rw-r--r--   0 chow       (501) staff       (20)     3431 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/tests/test_wave_maker.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.176666 pyatoa-0.3.1/pyatoa/utils/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)     2144 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/adjoint.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.177211 pyatoa-0.3.1/pyatoa/utils/asdf/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/asdf/__init__.py
--rwxr-xr-x   0 chow       (501) staff       (20)     5243 2023-02-28 22:36:23.000000 pyatoa-0.3.1/pyatoa/utils/asdf/add.py
--rwxr-xr-x   0 chow       (501) staff       (20)     4101 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/asdf/clean.py
--rwxr-xr-x   0 chow       (501) staff       (20)     9455 2023-02-28 22:36:23.000000 pyatoa-0.3.1/pyatoa/utils/asdf/load.py
--rwxr-xr-x   0 chow       (501) staff       (20)     5059 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/asdf/write.py
--rw-r--r--   0 chow       (501) staff       (20)     5344 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/utils/calculate.py
--rw-r--r--   0 chow       (501) staff       (20)     4620 2023-09-08 02:53:06.000000 pyatoa-0.3.1/pyatoa/utils/form.py
--rw-r--r--   0 chow       (501) staff       (20)     3300 2023-03-01 01:06:49.000000 pyatoa-0.3.1/pyatoa/utils/images.py
--rw-r--r--   0 chow       (501) staff       (20)    15421 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/utils/process.py
--rw-r--r--   0 chow       (501) staff       (20)    10688 2022-12-21 00:49:30.000000 pyatoa-0.3.1/pyatoa/utils/srcrcv.py
--rw-r--r--   0 chow       (501) staff       (20)     3378 2022-12-21 00:49:30.000000 pyatoa-0.3.1/pyatoa/utils/window.py
--rw-r--r--   0 chow       (501) staff       (20)    12221 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/utils/write.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.177995 pyatoa-0.3.1/pyatoa/visuals/
--rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/visuals/__init__.py
--rw-r--r--   0 chow       (501) staff       (20)    22952 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/visuals/comp_wave.py
--rw-r--r--   0 chow       (501) staff       (20)    19301 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/visuals/improve_wave.py
--rw-r--r--   0 chow       (501) staff       (20)    71783 2022-12-07 21:52:28.000000 pyatoa-0.3.1/pyatoa/visuals/insp_plot.py
--rw-r--r--   0 chow       (501) staff       (20)    17601 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/visuals/map_maker.py
--rw-r--r--   0 chow       (501) staff       (20)    34051 2023-09-03 07:07:20.000000 pyatoa-0.3.1/pyatoa/visuals/wave_maker.py
-drwxr-xr-x   0 chow       (501) staff       (20)        0 2023-09-08 02:54:41.173413 pyatoa-0.3.1/pyatoa.egg-info/
--rw-r--r--   0 chow       (501) staff       (20)    43077 2023-09-08 02:54:41.000000 pyatoa-0.3.1/pyatoa.egg-info/PKG-INFO
--rw-r--r--   0 chow       (501) staff       (20)     1340 2023-09-08 02:54:41.000000 pyatoa-0.3.1/pyatoa.egg-info/SOURCES.txt
--rw-r--r--   0 chow       (501) staff       (20)        1 2023-09-08 02:54:41.000000 pyatoa-0.3.1/pyatoa.egg-info/dependency_links.txt
--rw-r--r--   0 chow       (501) staff       (20)      100 2023-09-08 02:54:41.000000 pyatoa-0.3.1/pyatoa.egg-info/requires.txt
--rw-r--r--   0 chow       (501) staff       (20)        7 2023-09-08 02:54:41.000000 pyatoa-0.3.1/pyatoa.egg-info/top_level.txt
--rw-r--r--   0 chow       (501) staff       (20)      745 2023-09-08 02:53:43.000000 pyatoa-0.3.1/pyproject.toml
--rw-r--r--   0 chow       (501) staff       (20)       38 2023-09-08 02:54:41.178776 pyatoa-0.3.1/setup.cfg
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.927690 pyatoa-0.4.0/
+-rw-r--r--   0 chow       (501) staff       (20)    35149 2022-12-07 21:52:28.000000 pyatoa-0.4.0/LICENSE.txt
+-rw-r--r--   0 chow       (501) staff       (20)    43077 2024-05-16 19:45:08.927502 pyatoa-0.4.0/PKG-INFO
+-rw-r--r--   0 chow       (501) staff       (20)     1732 2023-03-01 01:06:49.000000 pyatoa-0.4.0/README.md
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.920804 pyatoa-0.4.0/docs/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-21 00:49:30.000000 pyatoa-0.4.0/docs/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)     6472 2024-05-16 19:31:31.000000 pyatoa-0.4.0/docs/conf.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.920925 pyatoa-0.4.0/pyatoa/
+-rw-r--r--   0 chow       (501) staff       (20)      672 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/__init__.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.922088 pyatoa-0.4.0/pyatoa/core/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/core/__init__.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    22043 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/core/config.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    12488 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/core/executive.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    67834 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/core/inspector.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    59979 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/core/manager.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.922767 pyatoa-0.4.0/pyatoa/scripts/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/scripts/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)     2254 2022-12-21 00:49:30.000000 pyatoa-0.4.0/pyatoa/scripts/data_data_example.py
+-rw-r--r--   0 chow       (501) staff       (20)     2408 2023-02-28 22:36:23.000000 pyatoa-0.4.0/pyatoa/scripts/load_example_data.py
+-rwxr-xr-x   0 chow       (501) staff       (20)     6262 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/scripts/process_data_w_mpi.py
+-rw-r--r--   0 chow       (501) staff       (20)     2030 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/scripts/syn_syn_example.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.924304 pyatoa-0.4.0/pyatoa/tests/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/tests/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)     7038 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/tests/test_asdf_utils.py
+-rw-r--r--   0 chow       (501) staff       (20)     3023 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/tests/test_config.py
+-rw-r--r--   0 chow       (501) staff       (20)     3737 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/tests/test_executive.py
+-rw-r--r--   0 chow       (501) staff       (20)     5443 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/tests/test_inspector.py
+-rw-r--r--   0 chow       (501) staff       (20)    10202 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/tests/test_manager.py
+-rw-r--r--   0 chow       (501) staff       (20)     2832 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/tests/test_mgmt_plot.py
+-rw-r--r--   0 chow       (501) staff       (20)     6100 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/tests/test_process_util.py
+-rw-r--r--   0 chow       (501) staff       (20)     5940 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/tests/test_utils.py
+-rw-r--r--   0 chow       (501) staff       (20)     3431 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/tests/test_wave_maker.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.925299 pyatoa-0.4.0/pyatoa/utils/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/utils/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)     2144 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/utils/adjoint.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.925869 pyatoa-0.4.0/pyatoa/utils/asdf/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/utils/asdf/__init__.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    10754 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/utils/asdf/add.py
+-rwxr-xr-x   0 chow       (501) staff       (20)     6888 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/utils/asdf/clean.py
+-rwxr-xr-x   0 chow       (501) staff       (20)    10082 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/utils/asdf/load.py
+-rwxr-xr-x   0 chow       (501) staff       (20)     5059 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/utils/asdf/write.py
+-rw-r--r--   0 chow       (501) staff       (20)     5344 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/utils/calculate.py
+-rw-r--r--   0 chow       (501) staff       (20)     4981 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/utils/form.py
+-rw-r--r--   0 chow       (501) staff       (20)     3300 2023-03-01 01:06:49.000000 pyatoa-0.4.0/pyatoa/utils/images.py
+-rw-r--r--   0 chow       (501) staff       (20)    16463 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/utils/process.py
+-rw-r--r--   0 chow       (501) staff       (20)    10688 2024-03-20 21:54:44.000000 pyatoa-0.4.0/pyatoa/utils/srcrcv.py
+-rw-r--r--   0 chow       (501) staff       (20)     3378 2022-12-21 00:49:30.000000 pyatoa-0.4.0/pyatoa/utils/window.py
+-rw-r--r--   0 chow       (501) staff       (20)    12221 2023-09-03 07:07:20.000000 pyatoa-0.4.0/pyatoa/utils/write.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.926848 pyatoa-0.4.0/pyatoa/visuals/
+-rw-r--r--   0 chow       (501) staff       (20)        0 2022-12-07 21:52:28.000000 pyatoa-0.4.0/pyatoa/visuals/__init__.py
+-rw-r--r--   0 chow       (501) staff       (20)    88494 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/visuals/insp_plot.py
+-rw-r--r--   0 chow       (501) staff       (20)    17601 2023-12-04 00:06:05.000000 pyatoa-0.4.0/pyatoa/visuals/map_maker.py
+-rw-r--r--   0 chow       (501) staff       (20)    34157 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/visuals/wave_maker.py
+-rw-r--r--   0 chow       (501) staff       (20)    14913 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyatoa/visuals/wave_train.py
+drwxr-xr-x   0 chow       (501) staff       (20)        0 2024-05-16 19:45:08.927030 pyatoa-0.4.0/pyatoa.egg-info/
+-rw-r--r--   0 chow       (501) staff       (20)    43077 2024-05-16 19:45:08.000000 pyatoa-0.4.0/pyatoa.egg-info/PKG-INFO
+-rw-r--r--   0 chow       (501) staff       (20)     1310 2024-05-16 19:45:08.000000 pyatoa-0.4.0/pyatoa.egg-info/SOURCES.txt
+-rw-r--r--   0 chow       (501) staff       (20)        1 2024-05-16 19:45:08.000000 pyatoa-0.4.0/pyatoa.egg-info/dependency_links.txt
+-rw-r--r--   0 chow       (501) staff       (20)      100 2024-05-16 19:45:08.000000 pyatoa-0.4.0/pyatoa.egg-info/requires.txt
+-rw-r--r--   0 chow       (501) staff       (20)        7 2024-05-16 19:45:08.000000 pyatoa-0.4.0/pyatoa.egg-info/top_level.txt
+-rw-r--r--   0 chow       (501) staff       (20)      745 2024-05-16 19:31:31.000000 pyatoa-0.4.0/pyproject.toml
+-rw-r--r--   0 chow       (501) staff       (20)       38 2024-05-16 19:45:08.927725 pyatoa-0.4.0/setup.cfg
```

### Comparing `pyatoa-0.3.1/LICENSE.txt` & `pyatoa-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/PKG-INFO` & `pyatoa-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatoa
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python's Adjoint Tomography Operations Assistant
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pyatoa-0.3.1/README.md` & `pyatoa-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/docs/conf.py` & `pyatoa-0.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 sys.path.insert(0, os.path.abspath('..'))
 
 import sphinx_rtd_theme
     
 # -- Project information -----------------------------------------------------
 
 project = 'Pyatoa'
-copyright = '2023, adjTomo'
+copyright = '2024, adjTomo'
 author = 'adjTomo Dev Team'
 
 # The short X.Y version
 # Grab version number from 'pyproject.toml'
 with open("../pyproject.toml", "r") as f:
     _lines = f.readlines()
 for _line in _lines:
```

### Comparing `pyatoa-0.3.1/pyatoa/__init__.py` & `pyatoa-0.4.0/pyatoa/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/core/config.py` & `pyatoa-0.4.0/pyatoa/core/config.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/core/executive.py` & `pyatoa-0.4.0/pyatoa/core/executive.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/core/inspector.py` & `pyatoa-0.4.0/pyatoa/core/inspector.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 A class to aggregate time windows, source-receiver information and misfit
 using Pandas.
 """
 import os
 import pyasdf
 import traceback
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from glob import glob
 from copy import deepcopy
 from fnmatch import filter as fnf
 from obspy.geodetics import gps2dist_azimuth
 from pyatoa import logger
@@ -22,38 +23,42 @@
     This plugin object will collect information from a Pyatoa run folder and
     allow the User to easily understand statistical information or generate
     statistical plots to help understand a seismic inversion.
 
     Inherits plotting capabilities from InspectorPlotter class to reduce clutter
     """
 
-    def __init__(self, tag="default", verbose=True):
+    def __init__(self, tag="inspector", verbose=False):
         """
         Inspector will automatically search for relevant file names using the
         tag attribute. If nothing is found, internal dataframes will be empty.
 
         :type tag: str
         :param tag: tag of a previously saved workflow to be used for reading
             in existing data from disk
         :type verbose: bool
         :param verbose: detail the files that are being read and their status
         """
         self.windows = pd.DataFrame()
         self.sources = pd.DataFrame()
         self.receivers = pd.DataFrame()
         self.tag = tag
-        self.verbose = verbose
 
         # Placeholder attributes for getters
         self._models = None
         self._srcrcv = None
         self._step_misfit = None
         self._event_misfit = None
         self._station_misfit = None
 
+        if verbose:
+            logger.setLevel("DEBUG")
+        else:
+            logger.setLevel("CRITICAL")
+
         # Try to load an already created Inspector
         try:
             self.read(tag=self.tag)
         except FileNotFoundError:
             pass
 
     def _get_str(self):
@@ -61,15 +66,16 @@
         Get the string representation once and save as internal attribute
         """
         # Get a list of internal public methods
         try:
             str_out = (f"{len(self.events):<4} event(s)\n"
                        f"{len(self.stations):<4} station(s)\n"
                        f"{len(self.iterations):<4} iteration(s)\n"
-                       f"{self.evaluations:<4} evaluation(s)")
+                       f"{self.evaluations:<4} evaluation(s)"
+                       )
 
         except KeyError:
             str_out = (f"{0:<4} event(s)\n"
                        f"{0:<4} station(s)\n"
                        f"{0:<4} iteration(s)\n"
                        f"{0:<4} evaluation(s)\n")
         return str_out
@@ -232,14 +238,260 @@
         return self._try_print("time")
 
     @property
     def depths(self):
         """Return a dictionary of event depths in units of meters"""
         return self._try_print("depth_km")
 
+    def generate_report(self, path_report=None, iteration=None,
+                        step_count=None, geographic=True, outliers=True,
+                        scatter=True, summary=True, nstd=2,
+                        dpi=200, **kwargs):
+        """
+        An aggregate function that generates a "report" by creating a number
+        of figures that summarize the misfit of the inversion. Makes it easier
+        for the User as they don't have to remember each of the functions in
+        the Inspector's wheelhouse, all relevant figures will be generated
+        automatically.
+
+        :type path_report: str
+        :param path_report: The path where the report will be saved. 
+            Defaults to "./report".
+        :type iteration: int
+        :param iteration: The iteration number.
+        :type step_count: int
+        :param step_count: The step count.
+        :type geographic: bool
+        :param geographic: If True, includes geographic data in the report. 
+            Defaults to True.
+        :type outliers: bool
+        :param outliers: If True, includes outliers in the report. 
+            Defaults to True.
+        :type scatter: bool
+        :param scatter: If True, includes a scatter plot in the report. 
+            Defaults to True.
+        :type summary: bool
+        :param summary: If True, includes a summary in the report. 
+            Defaults to True.
+        :type nstd: int
+        :param nstd: The number of standard deviations for outlier detection.  
+            Defaults to 2.
+        :type dpi: int
+        :param dpi: The resolution in dots per inch for the figures in the 
+            report. Defaults to 200.
+        :type kwargs: dict
+        :param kwargs: Additional keyword arguments.
+        """
+        # By default we generate a report for the final model 
+        iteration, step_count = self.validate_evaluation(iteration, step_count,
+                                                         choice="final")
+        if path_report is None:
+            path_report = f"./report_{iteration}{step_count}"
+        if not os.path.exists(path_report):
+            os.makedirs(path_report)
+
+        # Generate some geographic information
+        if geographic:
+            geographic_plot_functions = ["map", "travel_times", "raypaths",
+                                         "event_depths"]
+            for plot_function in geographic_plot_functions:
+                save = os.path.join(path_report, f"{plot_function}.png")
+                if os.path.exists(save):
+                    continue
+                getattr(self, plot_function)(iteration=iteration,
+                                             step_count=step_count,
+                                             show=False, dpi=dpi)
+                plt.close()
+
+        # Plot misfit spider plots of event misfit for events that are outside
+        # N standard deviations of the mean w.r.t misfit value
+        if outliers:
+            upper_outliers, lower_outliers, mean ,std = \
+                self.event_outliers(iteration, step_count, nstd=nstd)
+            
+            if upper_outliers.empty and lower_outliers.empty:
+                logger.warning("No outliers found, skipping outlier plots, " 
+                               "reduce `nstd` to reevaluate for outliers")
+            else:
+                for outliers, tag in zip([upper_outliers, lower_outliers],
+                                        ["upper_outlier", "lower_outlier"]):
+                    for event_name in outliers.index.to_list():
+                        self.event_station_misfit_map(
+                            event=event_name, iteration=iteration,
+                            step_count=step_count, 
+                            save=os.path.join(path_report,
+                                            f"{tag}_{event_name}.png"),
+                            show=False, dpi=dpi
+                        )
+                        plt.close()
+
+        # Create a few scatterplots comparing some parameters
+        if scatter:
+            for xy in [
+                ("distance_km", "cc_shift_in_seconds"),
+                ("backazimuth", "cc_shift_in_seconds"),
+                ("length_s", "cc_shift_in_seconds"),
+            ]:
+                x, y = xy
+                self.scatter(x=x, y=y, show=False, dpi=dpi,
+                             save=os.path.join(path_report, f"{x}_v_{y}.png")
+                             )
+
+        # Plot summary figures that show the status of inversion holistically
+        if summary:
+            self.convergence(normalize=True, show=False, dpi=dpi,
+                             save=os.path.join(path_report, "convergence.png")
+                             )
+
+            summary_functions = ["event_station_hist2d", "event_comparison",
+                                 "window_stack", "histogram_summary"]
+            for plot_function in summary_functions:
+                save = os.path.join(path_report, f"{plot_function}.png")
+                if os.path.exists(save):
+                    continue
+                # We want the histogram summary to be comparative
+                if plot_function == "histogram_summary":
+                    getattr(self, plot_function)(
+                        iteration="i01", step_count="s00", 
+                        iteration_comp=iteration, step_count_comp=step_count,
+                        save=save, show=False, dpi=dpi
+                        )
+                else:
+                    getattr(self, plot_function)(
+                        iteration=iteration, step_count=step_count, save=save, 
+                        show=False, dpi=dpi
+                        )
+                plt.close()
+
+        plt.close("all")
+
+        self.generate_report_text(path_report, nstd)
+            
+    def generate_report_text(self, path_report="./", nstd=1):
+        """
+        Generate a text report highlighting good/bad performing events and 
+        stations that will provide the User a quickly accessible summary of 
+        their inversion and may motivate looking at some waveforms
+        """       
+        line_break = "\n" + "=" * 80 +"\n"     
+        iter_end, step_end = self.validate_evaluation(
+            iteration=None, step_count=None, choice="final"
+            )
+        
+        # Get event mean and std for current evaluation
+        _, _, mean ,std = \
+                self.event_outliers(iter_end, step_end, nstd=nstd)
+        
+        # Get an ascended list of misfit/windows per event
+        _windows = self.windows  
+        self.windows = self.isolate(iteration=iter_end, step_count=step_end)
+
+        # Event specific window information
+        win_per_event = self.nwin(level="event")
+        avg_win_per_event = win_per_event.nwin.mean()
+
+        _tenwin = win_per_event.iloc[0].nwin
+        top_event_by_win = win_per_event.iloc[0].name[-1]
+
+        _benwin = win_per_event.iloc[-1].nwin
+        bot_event_by_win = win_per_event.iloc[-1].name[-1]
+
+        win_per_event_str = win_per_event.to_string()
+        
+        # Station specific window information
+        win_per_station = self.nwin(level="station")
+        avg_win_per_station = win_per_station.nwin.mean()
+
+        _tsnwin = win_per_station.iloc[0].nwin
+        top_sta_by_win = win_per_station.iloc[0].name[-1]
+
+        _bsnwin = win_per_station.iloc[-1].nwin
+        bot_sta_by_win = win_per_station.iloc[-1].name[-1]
+
+        win_per_station_str = win_per_station.to_string()
+
+        # Event specific misfit information
+        misfit_per_event = self.misfit(level="event", reset=True)
+
+        _temsft = misfit_per_event.iloc[0].misfit
+        highest_misfit_event = misfit_per_event.iloc[0].name[-1]
+        
+        _bemsft = misfit_per_event.iloc[-1].misfit
+        lowest_misfit_event = misfit_per_event.iloc[-1].name[-1]
+
+        misfit_per_event_str = misfit_per_event.sort_values(
+            "misfit", ascending=False).to_string()
+
+        # Station specific misfit information
+        misfit_per_sta = self.misfit(level="station", reset=True)
+
+        _tsmsft = misfit_per_sta.iloc[0].misfit
+        highest_misfit_sta = misfit_per_sta.iloc[0].name[-1]
+        
+        _bsmsft = misfit_per_sta.iloc[-1].misfit
+        lowest_misfit_sta = misfit_per_sta.iloc[-1].name[-1]
+
+        misfit_per_sta_str = misfit_per_sta.sort_values(
+            "misfit", ascending=False).to_string()
+                
+        # Get windows per component for the current evaluation
+        _windows_eval = self.windows
+        win_str = ""
+        for component in self.windows.component.unique():
+            self.windows = self.isolate(component=component)
+            # Sort of a hacky way of getting what we know is a single value
+            nwin_per_comp = self.nwin().nwin.to_list()[0]
+            win_str += f"- {component}: {nwin_per_comp}\n"
+            self.windows = _windows_eval
+
+        # Restore the original windows, just incase but likely not needed?
+        self.windows = _windows  
+
+        # Compile all the above information into a nice text output to be writ
+        srcrcv_summary = (
+            f"Avg windows per event:  {avg_win_per_event:.2f}\n"
+            f"- Evt w/ max win:       {top_event_by_win} ({_tenwin:.0f})\n"
+            f"- Evt w/ min win:       {bot_event_by_win} ({_benwin:.0f})\n"
+            f"- Evt w/ max msft:      {highest_misfit_event} ({_temsft:.2f})\n"
+            f"- Evt w/ min msft:      {lowest_misfit_event} ({_bemsft:.2f})\n"
+            "\n"
+            f"Avg windows per sta:    {avg_win_per_station:.2f}\n"
+            f"- Sta w/ max win:       {top_sta_by_win} ({_tsnwin:.0f})\n"
+            f"- Sta w/ min win:       {bot_sta_by_win} ({_bsnwin:.0f})\n"
+            f"- Sta w/ max msft:      {highest_misfit_sta} ({_tsmsft:.2f})\n"
+            f"- Sta w/ min msft:      {lowest_misfit_sta}  ({_bsmsft:.2f})\n"
+            "\n"
+            f"Windows per component:\n"
+            f"{win_str}"
+            )
+
+        # Header contains general information for understanding inversion
+        report = [
+            f"{'INSPECTOR REPORT':^80}",
+            f"{'SUMMARY':^80}",
+            f"{self._get_str()}", 
+            f"{f'SRCRCV SUMMARY [{iter_end}{step_end}]':^80}",
+            f"{srcrcv_summary}",
+            f"{'TOTAL WINDOWS':^80}",
+            f"{self.nwin().to_string()}",  
+            f"{'TOTAL MISFIT':^80}",
+            f"{self.misfit().to_string()}", 
+            f"{'WINDOWS PER EVENT':^80}",
+            f"{win_per_event_str}",  
+            f"{f'MISFIT PER EVENT (MEAN={mean:.2f}, {nstd}STD={std:.2f})':^80}",
+            f"{misfit_per_event_str}", 
+            f"{'WINDOWS PER STATION':^80}",
+            f"{win_per_station_str}",
+            f"{f'MISFIT PER STATION':^80}",
+            f"{misfit_per_sta_str}", 
+        ]
+    
+        with open(os.path.join(path_report, "inspector_report.txt"), "w") as f:
+            f.writelines(f"{line_break}".join(report))
+
     def _get_srcrcv_from_dataset(self, ds):
         """
         Get source and receiver information from dataset, this includes
         latitude and longitude values for both, and event information including
         magnitude, origin time, id, etc.
 
         Returns Dataframes for sources and receivers iff they are not already
@@ -332,20 +584,21 @@
         misfit_windows = ds.auxiliary_data.MisfitWindows
         adjoint_sources = ds.auxiliary_data.AdjointSources
 
         # Initiation loop to get iteration and step count, allows for the case
         # where no step count is given (e.g., iteration == 'default')
         iters, steps = [], []
         for iter_ in misfit_windows.list():
-            iters.append(iter_)
             for step in misfit_windows[iter_].list():
                 # Ensure that step counts are formatted like: 's00'
                 # if not then we DONT have step counts in the dataset
                 if not step.startswith("s") and not len(step) == 3:
                     step = ""
+
+                iters.append(iter_)
                 steps.append(step)
 
         # Pulling out important information from the windows and adj src.
         for iter_, step in zip(iters, steps):
             # If any entries exist for a given event/model/step
             # ignore appending them to the internal structure as they've
             # already been collected
@@ -373,16 +626,15 @@
                                   f"{net}_{sta}_*{component}"
                                   )[0]
 
                     # This misfit value will be the same for mult windows
                     window["misfit"].append(adjoint_source_eval[
                                                 adj_tag].parameters["misfit"])
                 except IndexError:
-                    if self.verbose:
-                        print(f"No matching adjoint source for {cha_id}")
+                    logger.warning(f"No matching adjoint source for {cha_id}")
                     window["misfit"].append(np.nan)
 
                 # winfo keys match the keys of the Pyflex Window objects
                 for par in winfo:
                     winfo[par].append(win.parameters[par])
 
                 # get identifying information for this window
@@ -403,43 +655,59 @@
 
         # Only add to internal structure if something was collected
         if window["event"]:
             window.update(winfo)
             self.windows = pd.concat([self.windows, pd.DataFrame(window)],
                                      ignore_index=True)
 
-    def _parse_nonetype_eval(self, iteration, step_count):
+    def validate_evaluation(self, iteration, step_count, choice="final"):
         """
+        Provide acceptable values for 'iteration' and 'step_count' to underlying
+        functions that require it.
         Whenever a user does not choose an iteration or step count, e.g., in
         plotting functions, this function defines default values based on the
         initial model (if neither given), or the last step count for a given
-        iteration (if only iteration is given). Only step count is not allowed
+        iteration (if only iteration is given). Only step count is not allowed.
+        If both iteration and step count are provided, just check that these
+        are acceptable values
 
         :type iteration: str
         :param iteration: chosen iteration, formatted as e.g., 'i01'
         :type step_count: str
         :param step_count: chosen step count, formatted as e.g., 's00'
+        :type choice: str
+        :param choice: 'initial' or 'final' to set the default behavior of
+            NoneType iteration and step_count returning either the initial
+            model or the final model evaluation
         :rtype: tuple of str
         :return: (iteration, step_count) default values for the iteration
             and step_count
         """
         # Default iteration and step count if None are given
         if iteration is None and step_count is None:
-            iteration, step_count = self.initial_model
-            print(f"No iteration or step count given, defaulting to initial "
-                  f"model: {iteration}{step_count}")
+            if choice == "initial":
+                iteration, step_count = self.initial_model
+            elif choice == "final":
+                iteration, step_count = self.final_model
+            logger.debug(f"No iteration or step count given, defaulting to "
+                         f"{choice} model: {iteration}{step_count}")
         elif iteration and (step_count is None):
             step_count = self.steps[iteration][-1]
-            print(f"No step count given, defaulting to final step count within"
-                  f"given iteration: {iteration}{step_count}")
+
+            logger.debug(f"No step count given, defaulting to final step count "
+                         f"within given iteration: {iteration}{step_count}")
         elif (iteration is None) and (step_count is not None):
             raise ValueError("'step_count' cannot be provided by itself, you "
                              "must also set the variable: 'iteration'")
+        else:
+            assert (iteration in self.iterations and
+                    step_count in self.steps[iteration]), \
+                f"{iteration}{step_count} does not exist in Inspector"
         return iteration, step_count
-    
+
     def discover(self, path="./", ignore_symlinks=True):
         """
         Allow the Inspector to scour through a path and find relevant files,
         appending them to the internal structure as necessary.
 
         :type path: str
         :param path: path to the pyasdf.asdf_data_set.ASDFDataSets that were
@@ -448,26 +716,25 @@
         :param ignore_symlinks: skip over symlinked HDF5 files when discovering
         """
         dsfids = glob(os.path.join(path, "*.h5"))
         # remove symlinks from the list if requested
         if ignore_symlinks:
             dsfids = [_ for _ in dsfids if not os.path.islink(_)]
         for i, dsfid in enumerate(dsfids):
-            if self.verbose:
-                print(f"{os.path.basename(dsfid):<25} "
-                      f"{i+1:0>3}/{len(dsfids):0>3}",  end="..."
-                      )
+
             try:
                 self.append(dsfid)
-                if self.verbose:
-                    print("done")
+                logger.info(f"{os.path.basename(dsfid):<25} "
+                            f"{i + 1:0>3}/{len(dsfids):0>3}: done",
+                            )
             except KeyError as e:
-                if self.verbose:
-                    print(f"error: {e}")
-                    traceback.print_exc()
+                logger.info(f"{os.path.basename(dsfid):<25} "
+                            f"{i + 1:0>3}/{len(dsfids):0>3}: error {e}",
+                            )
+                traceback.print_exc()
                 continue
 
         return self
 
     def append(self, dsfid, srcrcv=True, windows=True):
         """
         Simple function to parse information from a
@@ -485,21 +752,19 @@
             with pyasdf.ASDFDataSet(dsfid) as ds:
                 if srcrcv:
                     self._get_srcrcv_from_dataset(ds)
                 if windows:
                     try:
                         self._get_windows_from_dataset(ds)
                     except AttributeError as e:
-                        if self.verbose:
-                            print("error reading dataset: "
-                                  "missing auxiliary data")
+                        logger.warning("error reading dataset: missing "
+                                       "auxiliary data")
                 return
         except OSError:
-            if self.verbose:
-                print(f"error reading dataset: already open")
+            logger.warning(f"error reading dataset: already open")
             return
 
     def extend(self, windows):
         """
         Extend the current Inspector data frames with the windows from another
         Inspector. This is useful for when an inversion has been run in legs, so
         two individual inspectors constitute a single inversion.
@@ -649,15 +914,15 @@
         """
         Simple function to wipe out all the internal attributes
         """
         self.windows = pd.DataFrame()
         self.sources = pd.DataFrame()
         self.receivers = pd.DataFrame()
 
-    def isolate(self, iteration=None, step_count=None,  event=None,
+    def isolate(self, iteration=None, step_count=None, event=None,
                 network=None, station=None, channel=None, component=None,
                 keys=None, exclude=None, unique_key=None):
         """
         Returns a new dataframe that is grouped by a given index if variable is
         None, defaults to returning all available values
 
         :type event: str
@@ -789,16 +1054,16 @@
                 return self._step_misfit
             elif level == "station" and self._station_misfit is not None:
                 return self._station_misfit
             elif level == "event" and self._event_misfit is not None:
                 return self._event_misfit
 
         # Various levels to sort the misfit by
-        group_list = ["iteration", "step", "event", "station", "component", 
-                      "misfit"]
+        group_list = ["iteration", "step", "event", "network", "station",
+                      "component", "misfit"]
         misfits = self.windows.loc[:, tuple(group_list)]
 
         # Count the number of windows on a per station basis
         nwin = misfits.groupby(
                 group_list[:-1]).misfit.apply(len).rename("nwin")
 
         # Misfit is unique per component, not window, drop repeat components
@@ -923,16 +1188,16 @@
         if pprint:
             max_key_len = max([len(_) for _ in minmax_dict.keys()])
             for key, val in minmax_dict.items():
                 print(f"{key + ':':<{max_key_len}} {val:.4f}")
 
         return minmax_dict
 
-    def compare(self, iteration_a=None, step_count_a=None, iteration_b=None,
-                step_count_b=None):
+    def compare_events(self, iteration_a=None, step_count_a=None, 
+                       iteration_b=None, step_count_b=None):
         """
         Compare the misfit and number of windows on an event by event basis
         between two evaluations. Provides absolute values as well as
         differences. Final dataframe is sorted by the difference in misfit,
         showing the most and least improved events.
 
         :type iteration_a: str
@@ -1045,15 +1310,78 @@
         df = pd.merge(windows_a, windows_b)
         # Take differences of all the comparison values, 'final - initial'
         initial, final = evals
         for val in comp_values:
             df[f"diff_{val}"] = df[f"{val}_{final}"] - df[f"{val}_{initial}"]
 
         return df
+    
+    def compare_misfits(self, iteration_a=None, step_count_a=None,
+                        iteration_b=None, step_count_b=None):
+        """
+        Compare the misfit values between the final and initial model for each
+        source receiver pair. Returns differences of unscaled misfit and 
+        difference in number of windows between two evaluations. 
+
+        .. note::
 
+            See also compare_events() for a similar function but for events only
+
+        :type iteration_a: str
+        :param iteration_a: initial iteration to use in comparison
+        :type step_count_a: str
+        :param step_count_a: initial step count to use in comparison
+        :type iteration_b: str
+        :param iteration_b: final iteration to use in comparison
+        :type step_count_b: str
+        :param step_count_b: final step count to use in comparison
+        :rtype: pandas.core.data_frame.DataFrame
+        :return: a data frame containing differences of misfit and number of
+            windows between final and initial models
+        """
+        iter_start, step_start = self.validate_evaluation(
+            iteration=iteration_a, step_count=step_count_a, choice="initial"
+            )
+        iter_end, step_end = self.validate_evaluation(
+            iteration=iteration_b, step_count=step_count_b, choice="final"
+            )
+        
+        _windows = self.windows  
+        self.windows = self.isolate(iteration=iter_start, step_count=step_start)
+        misfit_start = self.misfit(level="station", reset=True)
+
+        self.windows = _windows
+        self.windows = self.isolate(iteration=iter_end, step_count=step_end)
+        misfit_end = self.misfit(level="station", reset=True)
+
+        # Merge the two making sure they match event and station
+        sfx_start = f"{iter_start}{step_start}"
+        sfx_end = f"{iter_end}{step_end}"
+        df = pd.merge(misfit_start, misfit_end, 
+                      on=["event", "network", "station"], 
+                      suffixes=(f"_{sfx_start}", f"_{sfx_end}")
+                      )
+
+        # Calculate the difference between the two misfits
+        df["diff_misfit"] = \
+            df[f"unscaled_misfit_{sfx_end}"] - df[f"unscaled_misfit_{sfx_start}"]
+        df["diff_nwin"] = df[f"nwin_{sfx_end}"] - df[f"nwin_{sfx_start}"]
+
+        # Drop the original values
+        df.drop([f"unscaled_misfit_{sfx_end}", f"unscaled_misfit_{sfx_start}", 
+                 f"misfit_{sfx_end}", f"misfit_{sfx_start}", 
+                 f"nwin_{sfx_end}", f"nwin_{sfx_start}"], 
+                axis=1, inplace=True)
+
+        # Reset windows so User can still use the Inspector as advertised
+        self.windows = _windows
+
+        # Isolate the largest misfit offenders
+        return df.sort_values(by="diff_misfit")
+    
     def filter_sources(self, lat_min=None, lat_max=None, lon_min=None,
                        lon_max=None, depth_min=None, depth_max=None,
                        mag_min=None, mag_max=None, min_start=None,
                        max_start=None):
         """
         Go through misfits and windows and remove events that fall outside
         a certain bounding box. Return sources that fall within the box.
@@ -1105,14 +1433,56 @@
                     sources["time"] >= min_start].set_index("event_id")
             if max_start:
                 sources = sources.loc[
                     sources["time"] <= max_start].set_index("event_id")
 
         return sources
 
+    def event_outliers(self, iteration=None, step_count=None, choice="misfit",
+                       nstd=1):
+        """
+        Returns outliers for a given misfit measure (misfit or window number)
+        by calculating mean and standard deviation and finding events that
+        fall outside some integer multiple of standard deviations from the mean.
+        Used for plotting in `event_comparison` but also useful for quickly
+        assessing which events have anomalously low or high misfit values
+
+        :type iteration: str
+        :param iteration: iteration to choose for misfit
+        :type step_count: str
+        :param step_count: step count to query, e.g. 's00'
+        :type choice: str
+        :param choice: choice of misfit value, either 'misfit' or 'nwin' or
+            'unscaled_misfit'
+        :type nstd: int
+        :param nstd: number of standard deviations to set upper and lower
+            thresholds. Defaults to 1
+        :rtype: (Pandas.series, Pandas.series, float, float)
+        :return: (events above upper threshold, events below lower threshold,
+                  mean, standard deviation)
+        """
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
+
+        arr = self.misfit(
+            level="event")[choice][iteration][step_count].to_numpy()
+        index = self.misfit(level="event")[choice][iteration][step_count]
+        mean = np.mean(arr)
+        std = np.std(arr)
+
+        upper_thresh = mean + (nstd * std)
+        lower_thresh = mean - (nstd * std)
+
+        idx_upper_outliers = np.where(arr >= upper_thresh)
+        idx_lower_outliers = np.where(arr <= lower_thresh)
+
+        upper_outliers = index.iloc[idx_upper_outliers]
+        lower_outliers = index.iloc[idx_lower_outliers]
+
+        return upper_outliers, lower_outliers, mean, std
+
     def get_models(self):
         """
         Return a sorted list of misfits which correspond to accepted models,
         label discards of the line search, and differentiate the final accepted
         line search evaluation from the previous iteration and the initial
         evaluation of the current iteration.
 
@@ -1218,7 +1588,35 @@
         models.reset_index(drop=True, inplace=True)
         misfit = models.misfit.round(decimals=float_precision)
         identical_misfit = np.where(misfit.diff() == 0)[0]
         models.drop(axis=0, index=identical_misfit, inplace=True)
         models.reset_index(drop=True, inplace=True)
 
         return models
+
+
+if __name__ == "__main__":
+
+
+    """
+    Here we define a simple command-line tool for using the Inspector. Useful 
+    for Users who have already generated the inspector, and want to quickly 
+    make figures to explore the misfit of their inversion. Must be run in the
+    directory containing your '.csv' Inspector files. Kwargs can be passed as
+    later arguments in the format 'key=val'
+    
+    .. rubric::
+        
+        $ python inspector.py <function_name> <kwarg_key=kwarg_val> ...
+        e.g.,
+        $ python inspector.py event_station_hist2d iteration=1 step_count=2
+    """
+    import sys
+    insp = Inspector()
+    kwargs = {}
+    if len(sys.argv) > 2:
+        for arg in sys.argv[2:]:
+            key, val = arg.split("=")
+            kwargs[key] = val
+    getattr(insp, sys.argv[1])(**kwargs)
+
+
```

### Comparing `pyatoa-0.3.1/pyatoa/core/manager.py` & `pyatoa-0.4.0/pyatoa/core/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import numpy as np
 import pyflex
 import pyadjoint
 import warnings
 
 from copy import deepcopy
 from obspy.signal.filter import envelope
-from pyasdf import ASDFWarning
 
 from pyatoa import logger
 from pyatoa.core.config import Config
-from pyatoa.utils.asdf.add import add_misfit_windows, add_adjoint_sources
+from pyatoa.utils.asdf.add import (add_misfit_windows, add_adjoint_sources,
+                                   add_waveforms, add_config)
 
 from pyatoa.utils.asdf.load import load_windows, load_adjsrcs
 from pyatoa.utils.form import channel_code
 
 from pyatoa.utils.process import (apply_filter, trim_streams, zero_pad,
                                   match_npts, normalize, stf_convolve,
                                   is_preprocessed)
@@ -326,64 +326,60 @@
         elif ds._ASDFDataSet__file.mode == "r":  # NOQA
             logger.warning("dataset opened in read-only mode, cannot write")
             return
 
         if choice is None:
             choice = ["event", "inv", "st_obs", "st_syn", "windows", "adjsrcs",
                       "config"]
+            
+        logger.info(f"saving Manager attributes to ASDFDataSet")
 
+        # Events should only need to be added once to the ASDFDataSet
         if self.event and "event" in choice:
             try:
                 ds.add_quakeml(self.event)
+                logger.info("Event object added to ASDFDataSet")
             except ValueError:
-                logger.debug("Event already present, not added")
+                pass
+        
+        # StationXML files only need to be added once to the ASDFDataSet
         if self.inv and "inv" in choice:
             try:
                 ds.add_stationxml(self.inv)
+                logger.info("StationXML object added to ASDFDataSet")
             except TypeError:
-                logger.debug("StationXML already present, not added")
-        # Redirect PyASDF 'waveforms already present' warnings for cleaner look
+                pass
+
+        # Observed waveforms only need to be added once to the ASDFDataSet,
+        # do not overwrite existing waveforms because observed shouldn't change
         if self.st_obs and "st_obs" in choice:
-            with warnings.catch_warnings():
-                warnings.filterwarnings("error")
-                try:
-                    ds.add_waveforms(waveform=self.st_obs,
-                                     tag=self.config.observed_tag)
-                except ASDFWarning:
-                    logger.debug(f"{self.config.observed_tag} waveform already "
-                                 f"present, not added")
-                    pass
+            add_waveforms(st=self.st_obs, ds=ds, tag=self.config.observed_tag,
+                          overwrite=False)
+
+        # Synthetic waveforms should be allowed to overwrite, e.g., in the case
+        # that we are rerunning synthetics or restarting iterations
         if self.st_syn and "st_syn" in choice:
-            with warnings.catch_warnings():
-                warnings.filterwarnings("error")
-                try:
-                    ds.add_waveforms(waveform=self.st_syn,
-                                     tag=self.config.synthetic_tag)
-                except ASDFWarning:
-                    logger.debug(f"{self.config.synthetic_tag} waveform "
-                                 f"already present, not added")
-                    pass
+            add_waveforms(st=self.st_syn, ds=ds, tag=self.config.synthetic_tag,
+                          overwrite=True)
+
+        # Windows will overwrite if windows already exist for this evaluation
         if self.windows and "windows" in choice:
-            logger.debug("saving misfit windows to ASDFDataSet")
-            add_misfit_windows(self.windows, ds, path=self.config.aux_path)
+            add_misfit_windows(windows=self.windows, ds=ds, 
+                               path=self.config.aux_path, overwrite=True)
+
+        # AdjointSources will overwrite if they already exist for evaluation
         if self.adjsrcs and "adjsrcs" in choice:
-            logger.debug("saving adjoint sources to ASDFDataSet")
             add_adjoint_sources(adjsrcs=self.adjsrcs, ds=ds,
                                 path=self.config.aux_path,
-                                time_offset=self.stats.time_offset_sec)
+                                time_offset=self.stats.time_offset_sec,
+                                overwrite=True)
 
         if self.config and "config" in choice:
-            with warnings.catch_warnings():
-                warnings.filterwarnings("error")
-                try:
-                    self.config.write(write_to=ds, fmt="asdf")
-                except ASDFWarning:
-                    logger.debug(f"config already present, not added")
-                    pass
-
+            add_config(config=self.config, ds=ds, path=self.config.aux_path)
+ 
     def write_adjsrcs(self, path="./", write_blanks=True):
         """
         Write internally stored adjoint source traces into SPECFEM defined
         two-column ascii files. Filenames are based on what is expected by
         Specfem, that is: 'NN.SSS.CCC.adj'
 
         ..note::
@@ -547,16 +543,19 @@
             assert(iteration is not None and step_count is not None), (
                 f"`fix_windows` requires 'iteration' and 'step_count' to access"
                 f"windows from ASDFDataSet"
             )
 
         self.standardize(standardize_to=standardize_to)
         self.preprocess(**kwargs)
-        self.window(fix_windows=fix_windows, iteration=iteration,
-                    step_count=step_count)
+        if fix_windows:
+            self.retrieve_windows_from_dataset(iteration=iteration,
+                                               step_count=step_count)
+        else:
+            self.window()
         self.measure()
 
     def flow_multiband(self, periods, standardize_to="syn", fix_windows=False,
                        iteration=None, step_count=None, plot=False, **kwargs):
         """
         Run the full workflow for a number of distinct period bands, returning
         a final set of adjoint sources generated as a summation of adjoint
@@ -596,14 +595,22 @@
         :param plot: name of figure if given, will plot waveform and map for
             each period band and append period band to figure name `plot`
         :rtype: tuple of dict
         :return: (windows, adjoint_sources), returns all the collected
             measurements from each of the period bands
         :raises ManagerError: for any controlled exceptions
         """
+        if fix_windows:
+            assert(self.ds is not None), \
+                f"`fix_windows` requires ASDFDataSet `ds`"
+            assert(iteration is not None and step_count is not None), (
+                f"`fix_windows` requires 'iteration' and 'step_count' to access"
+                f"windows from ASDFDataSet"
+            )
+
         # Copy these waveforms to overwrite for each new period band
         st_obs_raw = self.st_obs.copy()
         st_syn_raw = self.st_syn.copy()
 
         # Do preprocessing once since
         self.check()
         self.standardize(standardize_to=standardize_to)
@@ -619,16 +626,19 @@
             self.config.min_period, self.config.max_period = period
 
             # Standard flow()
             try:
                 self.check()
                 self.standardize(standardize_to=standardize_to)
                 self.preprocess(**kwargs)
-                self.window(fix_windows=fix_windows, iteration=iteration,
-                            step_count=step_count)
+                if fix_windows:
+                    self.retrieve_windows_from_dataset(iteration=iteration,
+                                                       step_count=step_count)
+                else:
+                    self.window()
                 self.measure()
                 if plot:
                     save = f"{plot}_{tag}.png"
                     self.plot(choice="both", save=save)
             except ManagerError as e:
                 logger.warning(f"period band {tag}s error {e}, "
                                f"cannot return adjoint source for {tag}")
@@ -751,21 +761,21 @@
         if self.st_syn[0].stats.sampling_rate != \
                 self.st_obs[0].stats.sampling_rate: 
             if standardize_to == "syn":
                 self.st_obs.resample(self.st_syn[0].stats.sampling_rate)
             else:
                 self.st_syn.resample(self.st_obs[0].stats.sampling_rate)
 
-        # Match start and endtimes
+        # Match start/endtimes by trimming the 'obs' waveforms to match 'syn'
         self.st_obs, self.st_syn = trim_streams(
             st_a=self.st_obs, st_b=self.st_syn,
             force={"obs": "a", "syn": "b"}[standardize_to]
             )
 
-        # Match the number of samples 
+        # If 'obs' is not long enough, pad end of 'obs' with 0s
         self.st_obs, self.st_syn = match_npts(
             st_a=self.st_obs, st_b=self.st_syn,
             force={"obs": "a", "syn": "b"}[standardize_to]
             )
 
         # Allow normalization of waveform amplitudes to one another or to
         # a given value
@@ -859,16 +869,15 @@
         for key, st in preproc_list.items():
             # Remove response from 'obs' type data only
             if remove_response:
                 if (key == "obs" and self.config.st_obs_type == "obs") or (
                         key == "syn" and self.config.st_syn_type == "obs"):
                     st.remove_response(inventory=self.inv, plot=False, **kwargs)
 
-            # Detrend and taper pre-filter
-            st.detrend("simple")
+            # Set mean to 0 and taper ends to prep for filtering
             st.detrend("demean")
             st.taper(taper_percentage)
 
             if self.config.rotate_to_rtz and self.baz is not None:
                 logger.info(f"rotate {key} NE->RT by {self.baz} degrees")
                 st.rotate(method="NE->RT", back_azimuth=self.baz)
 
@@ -902,140 +911,175 @@
         self.stats.obs_processed = is_preprocessed(self.st_obs)
         self.stats.syn_processed = is_preprocessed(self.st_syn)
         self.stats.len_obs = len(self.st_obs)
         self.stats.len_syn = len(self.st_syn)
 
         return self
 
-    def window(self, fix_windows=False, iteration=None, step_count=None,
-               force=False):
+    def window(self, windows=None, force=False):
         """
         Evaluate misfit windows using Pyflex. Save windows to ASDFDataSet.
         Allows previously defined windows to be retrieved from ASDFDataSet.
 
         .. note::
             * Windows are stored as dictionaries of pyflex.Window objects.
             * All windows are saved into the ASDFDataSet, even if retrieved.
             * STA/LTA information is collected and stored internally.
 
-        :type fix_windows: bool
-        :param fix_windows: do not pick new windows, but load windows from the
-            given dataset from 'iteration' and 'step_count'
-        :type iteration: int or str
-        :param iteration: if 'fix_windows' is True, look for windows in this
-            iteration. If None, will check the latest iteration/step_count
-            in the given dataset
-        :type step_count: int or str
-        :param step_count: if 'fix_windows' is True, look for windows in this
-            step_count. If None, will check the latest iteration/step_count
-            in the given dataset
+        :type windows: dict
+        :param windows: optional argument for User to provide their own windows
+            to the window function. This will override the window selection
+            process and simply apply the window directly to the class and
+            adjust the stats `nwin` for the total number of windows.
         :type force: bool
         :param force: ignore flag checks and run function, useful if e.g.
             external preprocessing is used that doesn't meet flag criteria
         """
         # Pre-check to see if data has already been standardized
         self.check()
 
         if not self.stats.standardized and not force:
             raise ManagerError("cannot window, waveforms not standardized")
 
-        # Determine how to treat fixed windows
-        if fix_windows and not self.ds:
-            logger.warning("cannot fix window, no dataset")
-            fix_windows = False
-        elif fix_windows and (iteration is None or step_count is None):
-            # If no iteration/step_count values are given, automatically search
-            # the previous step_count for windows in relation to the current
-            # iteration/step_count
-            iteration = self.config.iteration
-            step_count = self.config.step_count
-            return_previous = True
-        else:
-            # If fix windows and iteration/step_count are given, search the
-            # dataset for windows under the current iteration/step_count
-            return_previous = False
-
         # Synthetic STA/LTA as Pyflex WindowSelector.calculate_preliminaries()
         for comp in self.config.component_list:
             try:
                 self.staltas[comp] = pyflex.stalta.sta_lta(
                     data=envelope(self.st_syn.select(component=comp)[0].data),
                     dt=self.st_syn.select(component=comp)[0].stats.delta,
                     min_period=self.config.min_period
                 )
             except IndexError:
                 continue
 
-        # Find misfit windows, from a dataset or through window selection
-        if fix_windows:
-            self.retrieve_windows(iteration, step_count, return_previous)
+        # If no windows provided, gather windows using waveform data
+        if not windows:
+            self._select_windows_plus()
         else:
-            self.select_windows_plus()
+            nwin = 0
+            for comp, window in windows.items():
+                nwin += len(window)
+
+            self.windows = windows
+            self.stats.nwin = sum(len(_) for _ in self.windows.values())
 
         logger.info(f"{self.stats.nwin} window(s) total found")
 
-        return self
+        # Print out some window stats for reference
+        for comp, windows_ in self.windows.items():
+            for w, win in enumerate(windows_):
+                logger.debug(f"{comp}_{w}: "
+                            f"cc={win.max_cc_value:.2f} / "
+                            f"dt={win.cc_shift * win.dt:.2f}s / "
+                            f"dlnA={win.dlnA:.2f}")
 
-    def retrieve_windows(self, iteration, step_count, return_previous):
-        """
-        Mid-level window selection function that retrieves windows from a 
-        PyASDF Dataset, recalculates window criteria, and attaches window 
-        information to Manager. No access to rejected window information.
+        return self
 
+    def retrieve_windows_from_dataset(self, ds=None, iteration=None,
+                                      step_count=None, components=None, 
+                                      revalidate=False):
+        """
+        Window selection function that retrieves previously saved windows from a
+        PyASDF ASDFDataset, recalculates window criteria using the old windows
+        with the current data, and attaches window information to Manager.
+
+        :type ds: pyasdf.ASDFDataSet
+        :param ds: ASDFDataSet with windows to select. If None given, will
+            search for internal definition of `ds`
         :type iteration: int or str
-        :param iteration: retrieve windows from the given iteration
+        :param iteration: retrieve windows from the given iteration. If None,
+            will search for the previous evaluation to select windows from
         :type step_count: int or str
         :param step_count: retrieve windows from the given step count
-            in the given dataset
-        :type return_previous: bool
-        :param return_previous: if True: return windows from the previous
-            step count in relation to the given iteration/step_count.
-            if False: return windows from the given iteration/step_count
+            in the given dataset. If None, will search for previous evaluation
+            to select windows from
+        :type components: list
+        :param components: if only windows from certain components should be 
+            returned from the dataset. If not given, defaults to Config 
+            `component_list`. Should be the inform of a list, e.g., ['N', 'E']
+        :type revalidate: bool
+        :param revalidate: check acceptability of waveform fit in the 
+            retrieved windows, that is, if time shift, dlna or cross correlation
+            fall outside of the accepted values defined in the Config object,
+            then the window will be rejected directly. IfFalse then
+            windows will be returned regardless of their newly assessed misfit.
         """
-        logger.info(f"retrieving windows from dataset")
+        if ds is None:
+            ds = self.ds
+        assert(ds is not None), f"ASDFDataSet `ds` required to retrieve windows"
+
+        # Determine how to treat fixed windows
+        if (iteration is None) or (step_count is None):
+            # If no iteration/step_count values are given, automatically search
+            # the previous step_count for windows in relation to the current
+            # iteration/step_count
+            iteration = self.config.iteration
+            step_count = self.config.step_count
+            return_previous = True
+        else:
+            # If fix windows and iteration/step_count are given, search the
+            # dataset for windows under the current iteration/step_count
+            return_previous = False
 
         net, sta, _, _ = self.st_obs[0].get_id().split(".")
         # Function will return empty dictionary if no acceptable windows found
-        windows = load_windows(ds=self.ds, net=net, sta=sta,
-                               iteration=iteration, step_count=step_count,
-                               return_previous=return_previous
-                               )
+        windows = load_windows(
+            ds=ds, net=net, sta=sta, iteration=iteration, step_count=step_count,
+            components=components or self.config.component_list,
+            return_previous=return_previous
+            )
 
         # Recalculate window criteria for new values for cc, tshift, dlnA etc...
-        logger.debug("recalculating window criteria")
         for comp, windows_ in windows.items():
+            # Use Pyflex machinery to re-evaluate the windows based on the
+            # current setup of waveforms
             try:
-                d = self.st_obs.select(component=comp)[0].data
-                s = self.st_syn.select(component=comp)[0].data
-                for w, win in enumerate(windows_):
-                    # Post the old and new values to the logger for sanity check
-                    logger.debug(f"{comp}{w}_old - "
-                                 f"cc:{win.max_cc_value:.2f} / "
-                                 f"dt:{win.cc_shift:.1f} / "
-                                 f"dlnA:{win.dlnA:.2f}")
-                    win._calc_criteria(d, s)
-                    logger.debug(f"{comp}{w}_new - "
-                                 f"cc:{win.max_cc_value:.2f} / "
-                                 f"dt:{win.cc_shift:.1f} / "
-                                 f"dlnA:{win.dlnA:.2f}")
+                obs = self.st_obs.select(component=comp)[0]
+                syn = self.st_syn.select(component=comp)[0]
+                if revalidate:
+                    logger.info("revalidating windows against Config criteria")
+                    ws = pyflex.WindowSelector(observed=obs, synthetic=syn,
+                            config=self.config.pyflex_config, event=self.event,
+                            station=self.inv)
+                    ws.windows = windows_
+                    ws.reject_based_on_data_fit_criteria()
+                    windows[comp] = ws.windows
+
+                # If no reject on data fit, simply recalculate the window 
+                # criteria and return all windows to User
+                else:
+                    logger.debug("recalculating window criteria (comp_#):")
+                    for w, win in enumerate(windows_):
+                        # Log for double check or manual review of new criteria
+                        logger.debug(f"{comp}_{w} (old): "
+                                    f"cc={win.max_cc_value:.2f} / "
+                                    f"dt={win.cc_shift * win.dt:.2f}s / "
+                                    f"dlnA={win.dlnA:.2f}")
+                        win._calc_criteria(obs.data, syn.data)
+                        logger.debug(f"{comp}_{w} (new): "
+                                    f"cc={win.max_cc_value:.2f} / "
+                                    f"dt={win.cc_shift * win.dt:.2f}s / "
+                                    f"dlnA={win.dlnA:.2f}")
+
             # IndexError thrown when trying to access an empty Stream
             except IndexError:
                 continue
 
         self.windows = windows
         self.stats.nwin = sum(len(_) for _ in self.windows.values())
 
-    def select_windows_plus(self):
+    def _select_windows_plus(self):
         """
         Mid-level custom window selection function that calls Pyflex select 
         windows, but includes additional window suppression functionality.
         Includes custom Pyflex addition of outputting rejected windows, which
         will be used internally for plotting.
 
         .. note::
+
             Pyflex will throw a ValueError if the arrival of the P-wave
             is too close to the initial portion of the waveform, considered the
             'noise' section. This happens for short source-receiver distances
             (< 100km).
 
             This error becomes a PyflexError if no event/station attributes
             are provided to the WindowSelector
@@ -1122,40 +1166,49 @@
             return
 
         # Check that data has been filtered and standardized
         if not self.stats.standardized and not force:
             raise ManagerError("cannot measure misfit, not standardized")
         elif self.stats.nwin == 0 and not force:
             raise ManagerError("cannot measure misfit, no windows recovered")
-        logger.debug(f"measure misfit of type: {self.config.adj_src_type}")
+        
+        logger.debug(f"measuring misfit with adjoint source type: "
+                     f"{self.config.adj_src_type}")
 
         # Create list of windows needed for Pyadjoint
         adjoint_windows = self._format_windows()
 
         # Run Pyadjoint to retrieve adjoint source objects
         total_misfit, adjoint_sources = 0, {}
         for comp, adj_win in adjoint_windows.items():
-            try:
-                adj_src = pyadjoint.calculate_adjoint_source(
-                    config=self.config.pyadjoint_config,
-                    observed=self.st_obs.select(component=comp)[0],
-                    synthetic=self.st_syn.select(component=comp)[0],
-                    windows=adj_win, plot=False
-                    )
-
-                # Re-format component name to reflect SPECFEM convention
-                adj_src.component = f"{channel_code(adj_src.dt)}X{comp}"
-
-                # Save adjoint sources in dictionary object. Sum total misfit
-                adjoint_sources[comp] = adj_src
-                logger.info(f"{comp}: {adj_src.misfit:.3f} misfit")
-                total_misfit += adj_src.misfit
-            except IndexError:
+            # Streams may not have matching components to given windows, e.g.,
+            # during an inversion 
+            observed = self.st_obs.select(component=comp)
+            synthetic = self.st_syn.select(component=comp)
+
+            if not observed or not synthetic:
+                logger.warning(f"no matching observed or synthetic data "
+                               f"for component {comp}, cannot measure")
                 continue
 
+            # Assuming that only one trace is available per stream
+            adj_src = pyadjoint.calculate_adjoint_source(
+                config=self.config.pyadjoint_config,
+                observed=observed[0], synthetic=synthetic[0],
+                windows=adj_win, plot=False
+                )
+
+            # Re-format component name to reflect SPECFEM convention
+            adj_src.component = f"{channel_code(adj_src.dt)}X{comp}"
+
+            # Save adjoint sources in dictionary object. Sum total misfit
+            adjoint_sources[comp] = adj_src
+            logger.info(f"{comp} component misfit == {adj_src.misfit:.3f}")
+            total_misfit += adj_src.misfit
+
         # Save adjoint source internally and to dataset
         self.adjsrcs = adjoint_sources
 
         # Run check to get total misfit
         self.check()
         logger.info(f"total misfit == {self.stats.misfit:.3f}")
```

### Comparing `pyatoa-0.3.1/pyatoa/scripts/data_data_example.py` & `pyatoa-0.4.0/pyatoa/scripts/data_data_example.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/scripts/load_example_data.py` & `pyatoa-0.4.0/pyatoa/scripts/load_example_data.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/scripts/process_data_w_mpi.py` & `pyatoa-0.4.0/pyatoa/scripts/process_data_w_mpi.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/scripts/syn_syn_example.py` & `pyatoa-0.4.0/pyatoa/scripts/syn_syn_example.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_asdf_utils.py` & `pyatoa-0.4.0/pyatoa/tests/test_asdf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     :return:
     """
     path = mgmt_post.config.aux_path
     add.add_misfit_windows(windows=mgmt_post.windows, ds=empty_dataset,
                            path=path)
 
     windows = empty_dataset.auxiliary_data.MisfitWindows[path]
-    assert(len(windows.list()) == 2)
+    assert(len(windows.list()) == 3)
 
     for comp, window_list in mgmt_post.windows.items():
         assert(len(window_list) == 1)
         window_check = window_list[0]
         # Dynamically construct station tags to access the individual parameters
         net, sta, loc, cha = window_check.channel_id.split(".")
         tag = f"{net}_{sta}_{comp}_0"
@@ -142,15 +142,15 @@
     path = mgmt_post.config.aux_path
     add.add_adjoint_sources(adjsrcs=mgmt_post.adjsrcs, ds=empty_dataset,
                             path=path,
                             time_offset=mgmt_post.stats.time_offset_sec
                             )
 
     adjsrcs = empty_dataset.auxiliary_data.AdjointSources[path]
-    assert(len(adjsrcs.list()) == 2)
+    assert(len(adjsrcs.list()) == 3)
 
     # Just check misfit value is correct
     for comp, adjsrc in mgmt_post.adjsrcs.items():
         tag = f"NZ_BFZ_BX{comp}"
         misfit_check = adjsrcs[tag].parameters["misfit"]
         assert(adjsrc.misfit == misfit_check)
```

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_config.py` & `pyatoa-0.4.0/pyatoa/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_executive.py` & `pyatoa-0.4.0/pyatoa/tests/test_executive.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_inspector.py` & `pyatoa-0.4.0/pyatoa/tests/test_inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,43 +157,20 @@
     Test the minmax printing function
     """
     insp = seisflows_inspector.copy()
     minmax = insp.minmax(pprint=False)
     assert(minmax["dlnA_max"] == pytest.approx(1.03947, .00001))
 
 
-def test_compare(seisflows_inspector):
+def test_compare_events(seisflows_inspector):
     """
     Test inter-event comparisons
     """
     insp = seisflows_inspector.copy()
-    assert(insp.compare().diff_nwin["2013p617227"] == -110)
-
-
-def test_compare_no_data():
-    """
-    Test that compare with no data returns NoneType
-    """
-    insp = Inspector()
-    assert(insp.compare() is None)
-
-
-def test_compare_windows(seisflows_inspector):
-    """
-    TODO Need fixed window inversion results to make this work
-    """
-    pass
-
-
-def test_no_step_information(seisflows_inspector):
-    """
-    TODO Test that when no step information is provided (only iteration),
-    TODO inspector can still handle data
-    """
-    pass
+    assert(insp.compare_events().diff_nwin["2013p617227"] == -110)
 
 
 def test_get_models(seisflows_inspector):
     """
     Test the model state tracker
     """
     states = [0, 1, -1, -1]
```

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_manager.py` & `pyatoa-0.4.0/pyatoa/tests/test_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,35 +62,14 @@
 def config():
     """
     Default Pyatoa Config object
     """
     return Config(event_id="2018p130600")
 
 
-# @pytest.fixture
-# def window():
-#     """
-#     Pre-gathered window for this specific source-receiver configuration
-#     This doesn't actually match the data... strange. Not used.
-#     """
-#     return json.load(open(
-#         "./test_data/test_window_NZ_BFZ_N_0_2018p130600.json"))["windows"][0]
-#
-#
-# @pytest.fixture
-# def adjoint_source():
-#     """
-#     Pre-gathered adjoint source for specific configuration to be compared with
-#     calculated adjoint source
-#     """
-#     return np.loadtxt(
-#         "./test_data/test_adjoint_source_NZ_BFZ_N_2018p130600.adj", unpack=True
-#         )
-
-
 @pytest.fixture
 def mgmt_pre(config, event, st_obs, st_syn, inv):
     """
     A manager filled with data but pre-workflow
     """
     return Manager(config=config, event=event, st_obs=st_obs, st_syn=st_syn, 
                    inv=inv)
@@ -203,14 +182,24 @@
     mgmt_pre.standardize().preprocess(
         remove_response=True, output="DISP").window()
 
     # Ensure the correct number of windows are chosen
     for comp, nwin in {"N": 1, "E": 1}.items():
         assert(len(mgmt_pre.windows[comp]) == nwin)
 
+def test_provide_windows(mgmt_post):
+    """
+    Test User-provided windows given to the window function
+    """
+    windows = mgmt_post.windows
+    mgmt_post.windows = None
+    mgmt_post.stats.nwin = 0
+
+    mgmt_post.window(windows=mgmt_post.windows)
+    assert(mgmt_post.stats.nwin == 3)
 
 def test_save_and_retrieve_windows(tmpdir, mgmt_post):
     """
     Test retrieve_windows() and save_windows() by saving windows into a
     scratch dataset and retrieving them back. Window criteria will be
     recalculated but since the waveforms are the same, the values will be the
     same as before.
@@ -223,29 +212,29 @@
     mgmt_post.config.step_count = 0
     saved_windows = mgmt_post.windows
     mgmt_post.write_to_dataset(choice=["windows"])  # saved to path 'm00/s00'
 
     # Delete windows, iterate step, retrieve fixed windows
     mgmt_post.windows = None
     mgmt_post.config.step_count += 1
-    mgmt_post.window(fix_windows=True)
+    mgmt_post.retrieve_windows_from_dataset(ds=ds, iteration=0, step_count=0)
 
     # Just check some parameter for each window to make sure all goods
     for comp in mgmt_post.windows:
         for w, window in enumerate(mgmt_post.windows[comp]):
             for attr in ["left", "right", "cc_shift"]:
                 assert(getattr(window, attr) ==
                        getattr(saved_windows[comp][w], attr))
 
     # Delete windows, slightly change synthetic waveforms and check to make
     # sure that recalculated criteria are different
     mgmt_post.windows = None
     for tr in mgmt_post.st_syn:
         tr.data *= 2
-    mgmt_post.window(fix_windows=True)
+    mgmt_post.retrieve_windows_from_dataset(ds=ds, iteration=0, step_count=0)
 
     for comp in mgmt_post.windows:
         for w, window in enumerate(mgmt_post.windows[comp]):
             # Amplitude ratios will be different since we multipled them
             assert (getattr(window, "dlnA") !=
                     getattr(saved_windows[comp][w], "dlnA"))
 
@@ -285,18 +274,19 @@
     """
     Test that the workflow for multiple period bands returns a single
     adjoint source
     """
     mgmt_pre.flow_multiband(periods=[(1, 10), (10, 30), (15, 40)],
                             remove_response=True, output="DISP")
 
-    # Just check that the expected values don't change
-    assert(pytest.approx(mgmt_pre.adjsrcs["E"].misfit, .001) == 0.33739)
-    assert(pytest.approx(mgmt_pre.adjsrcs["N"].misfit, .001) == 0.52064)
-    assert(pytest.approx(mgmt_pre.adjsrcs["Z"].misfit, .001) == 0.29031)
+    # Just check that the expected values don't change too much. Large tolernace
+    # as floating point math will likely creep into the misfit values
+    assert(pytest.approx(mgmt_pre.adjsrcs["E"].misfit, 0.1) == 0.33)
+    assert(pytest.approx(mgmt_pre.adjsrcs["N"].misfit, 0.1) == 0.52)
+    assert(pytest.approx(mgmt_pre.adjsrcs["Z"].misfit, 0.1) == 0.29)
 
 
 def test_resample_numerical_noise(mgmt_pre):
     """
     Raised in Issue #34 by Ridvan O. (rdno).
     
     Numerical noise can be introduced by resampling a trace that already has
```

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_mgmt_plot.py` & `pyatoa-0.4.0/pyatoa/tests/test_mgmt_plot.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_process_util.py` & `pyatoa-0.4.0/pyatoa/tests/test_process_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -111,33 +111,73 @@
     for st, npts_check in zip(
             [st_pad_before, st_pad_after, st_pad_both],
             [pl_samples, pl_samples, pl_samples * 2]
     ):
         assert(st[0].stats.npts - npts == npts_check)
 
 
-def test_trim_streams_and_match_npts(st_obs, st_syn):
+def test_trim_streams(st_obs, st_syn):
+    """
+    Test Stream trimming functionality
+    """
+    st_a = st_obs.copy()
+    st_b = st_syn.copy()
+
+    # Resample first so that we can actually trim the exact same start and 
+    # end times
+    st_a.resample(st_b[0].stats.sampling_rate)
+
+    # Trim A so we know it is different from B
+    st_a.trim(starttime=st_b[0].stats.starttime + 100,
+              endtime=st_b[0].stats.endtime - 100)
+
+    for tr_a, tr_b in zip(st_a, st_b):
+        assert(tr_a.stats.starttime != tr_b.stats.starttime)
+        assert(tr_a.stats.endtime != tr_b.stats.endtime)
+
+    # Trim streams to the same time window
+    st_at, st_bt = process.trim_streams(st_a=st_a, st_b=st_b, force="a")
+
+    for tr_a, tr_b in zip(st_at, st_bt):
+        assert(tr_a.stats.starttime == tr_b.stats.starttime)
+        assert(tr_a.stats.endtime == tr_b.stats.endtime)
+
+    # Make sure this throws an error if it is unable to trim streams
+    with pytest.raises(AssertionError):
+        process.trim_streams(st_a=st_a, st_b=st_b, force="b")
+
+
+def test_match_npts(st_obs, st_syn):
     """
     Ensure that forcing number of points standardization works
     """
     st_a = st_obs.copy()
     st_b = st_syn.copy()
 
-    # Downsample observations to synthetics
+    # Resample A to B and trim A to B
     st_a.resample(st_b[0].stats.sampling_rate)
+
+    # Trim A so we know it is different from B
+    st_a.trim(starttime=st_b[0].stats.starttime + 100,
+              endtime=st_b[0].stats.endtime - 100)
     assert(st_a[0].stats.npts != st_b[0].stats.npts)
 
-    # Trim obs data down to match syn data
-    st_a, st_b = process.trim_streams(st_a=st_a, st_b=st_b, force="b")
-    assert(st_a[0].stats.npts == st_b[0].stats.npts)
-
-    # Purposefully mismatch npts and then pad with 0s
-    st_a[0].trim(endtime=st_a[0].stats.endtime - 1)
-    st_a, st_b = process.match_npts(st_a, st_b, force="b")
-    assert(st_a[0].stats.npts == st_b[0].stats.npts)
+    # Trim streams so that they are the same length
+    st_a, st_b = process.trim_streams(st_a=st_a, st_b=st_b, force="a")
+
+    # Force one stream to be slightly shorter
+    st_a.trim(endtime=st_a[0].stats.endtime - 1)
+    
+    # Check they're different
+    for tr_a, tr_b in zip(st_a, st_b):
+        assert(tr_a.stats.npts != tr_b.stats.npts)
+
+    # Match npts
+    st_at, st_bt = process.match_npts(st_a, st_b, force="b")
+    assert(st_at[0].stats.npts == st_bt[0].stats.npts)
 
 
 def test_is_preprocessed(st_obs):
     """
     Test the check function that determines if a stream is preprocessed
     """
     # Check for a few different, commonly used processing functions
```

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_utils.py` & `pyatoa-0.4.0/pyatoa/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/tests/test_wave_maker.py` & `pyatoa-0.4.0/pyatoa/tests/test_wave_maker.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/adjoint.py` & `pyatoa-0.4.0/pyatoa/utils/adjoint.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/asdf/load.py` & `pyatoa-0.4.0/pyatoa/utils/asdf/load.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from obspy import UTCDateTime
 from fnmatch import filter as fnf
 from pyflex.window import Window
 from pyadjoint.adjoint_source import AdjointSource
 from pyatoa.utils.form import format_iter, format_step
 
 
-def load_windows(ds, net, sta, iteration, step_count, return_previous=False):
+def load_windows(ds, net, sta, iteration, step_count, return_previous=False,
+                 components=None):
     """
     Returns misfit windows from an ASDFDataSet for a given iteration, step,
     network and station, as well as a count of windows returned.
 
     If given iteration and step are not present in dataset (e.g. during line 
     search, new step), will try to search the previous step, which may or 
     may not be contained in the previous iteration. 
@@ -34,41 +35,43 @@
     :type iteration: int or str
     :param iteration: current iteration, will be formatted by the function
     :type step_count: int or str
     :param step_count: step count, will be formatted by the function
     :type return_previous: bool
     :param return_previous: search the dataset for available windows
         from the previous iteration/step given the current iteration/step
+    :type components: str or list of str
+    :param components: if not None, only select windows by a given component,
+        else, just load all possible components. Can be a string like 'ZNE' or
+        a list of strings like ['Z', 'N', 'E']
     :rtype window_dict: dict
     :return window_dict: dictionary containing misfit windows, in a format
         expected by Pyatoa Manager class
     """
     # Ensure the tags are properly formatted
     iteration = format_iter(iteration)
     step_count = format_step(step_count)
     windows = ds.auxiliary_data.MisfitWindows
 
     window_dict = {}    
     if return_previous:
         # Retrieve windows from previous iter/step
-        prev_windows = previous_windows(windows=windows, iteration=iteration,
-                                        step_count=step_count
-                                        )
-        window_dict = dataset_windows_to_pyflex_windows(windows=prev_windows,
-                                                        network=net, station=sta
-                                                        )
+        window_attr = previous_windows(windows=windows, iteration=iteration,
+                                       step_count=step_count)
     else:
         if hasattr(windows, iteration) and \
                             hasattr(windows[iteration], step_count):
             # Attempt to retrieve windows from the given iter/step
             logger.debug(f"searching for windows in {iteration}{step_count}")
-            window_dict = dataset_windows_to_pyflex_windows(
-                windows=windows[iteration][step_count], network=net, 
-                station=sta
-                )
+            window_attr = windows[iteration][step_count]
+
+    # Convert the Windows axiliary data into PyFlex Windows objects
+    window_dict = dataset_windows_to_pyflex_windows(windows=window_attr,
+                                                    network=net, station=sta,
+                                                    components=components)
 
     return window_dict
 
 
 def load_adjsrcs(ds, net, sta, iteration, step_count):
     """
     Load adjoint sources from a pyasdf ASDFDataSet and return in the format
@@ -117,37 +120,44 @@
 
         # The parameter dicionary will have all the keywords necessary
         adjsrc_dict[component] = AdjointSource(**parameters)
 
     return adjsrc_dict
 
 
-def dataset_windows_to_pyflex_windows(windows, network, station):
+def dataset_windows_to_pyflex_windows(windows, network, station, 
+                                      components=None):
     """
     Convert the parameter dictionary of an ASDFDataSet MisfitWindow into a 
     dictionary of Pyflex Window objects, in the same format as Manager.windows
 
     Returns empty dict and 0 if no windows are found
 
     :type windows: pyasdf.utils.AuxiliaryDataAccessor
     :param windows: ds.auxiliary_data.MisfitWindows[iter][step]
     :type network: str
     :param network: network of the station related to the windows
     :type station: str
     :param station: station related to the windows
+    :type components: str or list of str
+    :param components: if not None, only select windows by a given component,
+        else, just load all possible components. Can be a string like 'ZNE' or
+        a list of strings like ['Z', 'N', 'E']
     :rtype: dict
     :return: dictionary of window attributes in the same format that Pyflex 
         outputs
     """
     window_dict, _num_windows = {}, 0
     for window_name in windows.list():
         net, sta, comp, n = window_name.split("_")
 
         # Check the title of the misfit window to see if applicable
         if (net == network) and (sta == station):
+            if components is not None and comp not in components:
+                continue
             par = windows[window_name].parameters
 
             # Create a Pyflex Window object
             window = Window(
                 left=par["left_index"], right=par["right_index"],
                 center=par["center_index"], dt=par["dt"],
                 time_of_first_sample=UTCDateTime(par["time_of_first_sample"]),
@@ -220,10 +230,11 @@
             # If nothing is found return the most recent windows available
             prev_iter, prev_step = iters[-1]
 
     # Format back into strings for accessing auxiliary data
     prev_iter = format_iter(prev_iter)
     prev_step = format_step(prev_step)
 
-    logger.debug(f"most recent windows: {prev_iter}{prev_step}")
+    logger.debug(f"loading misfit windows from evaluation "
+                 f"'{prev_iter}{prev_step}'")
 
     return windows[prev_iter][prev_step]
```

### Comparing `pyatoa-0.3.1/pyatoa/utils/asdf/write.py` & `pyatoa-0.4.0/pyatoa/utils/asdf/write.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/calculate.py` & `pyatoa-0.4.0/pyatoa/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/form.py` & `pyatoa-0.4.0/pyatoa/utils/form.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Pyatoa relies on data structure being ordered and consistent throughout all the
 various bits of data required, as well as a few standardized string formatters
 to keep everything playing nice. Functions here will aid in reshaping data
 into the correct formats.
 """
 from pyasdf import ASDFDataSet
 from obspy.core.event import Event
+from pyatoa import logger
 
 
 def channel_code(dt):
     """
     Specfem outputs seismograms with channel band codes set by IRIS. Instrument
     codes are always X for synthetics, but band code will vary with the sampling
     rate of the data, return the correct code given a sampling rate.
@@ -86,15 +87,18 @@
         stpcnt = None
 
     return stpcnt
 
 
 def format_event_name(ds_or_event):
     """
-    Formalize the definition of Event ID in Pyatoa
+    Formalize the definition of Event ID in Pyatoa by parsing it out of the 
+    resource_id attribute of the ObsPy Event object. Different data centers
+    will tag their resource IDs differently, so this function can parse some 
+    of the more popular ones.
 
     :type ds_or_event: pyasdf.ASDFDataSet or obspy.core.event.Event or str
     :param ds_or_event: get dataset event name from the event resource_id
     :rtype: str
     :return: the event name to be used for naming schema in the workflow
     """
     # Extract the resource id dependent on the input file type
@@ -105,30 +109,36 @@
     elif isinstance(ds_or_event, ASDFDataSet):
         rid = ds_or_event.events[0].resource_id.id
     else:
         raise TypeError("format_event_name() only accepts pyasdf.ASDFDataSet "
                         "or obspy.core.event.Event objects")
 
     rid_up = rid.upper()
+
     # GeoNet Client: smi:nz.org.geonet/2018p130600
     if "GEONET" in rid_up:
-        return rid.split("/")[-1]
+        event_name = rid.split("/")[-1]
     # IRIS Client: smi:service.iris.edu/fdsnws/event/1/query?eventid=5197722
     elif "IRIS" in rid_up:
-        return rid.split("eventid=")[-1]
+        event_name = rid.split("eventid=")[-1]
     # SPUD, GCMT: smi:local/ndk/C202005010101A/event
     # or CMTSOLUTION: smi:local/cmtsolution/2013p617227/event
     elif ("NDK" in rid_up) or ("CMTSOLUTION" in rid_up):
-        return rid.split("/")[-2]
+        event_name = rid.split("/")[-2]
     # USGS Client: quakeml:earthquake.usgs.gov/fdsnws/event/1/...
     #                          ...query?eventid=ak0198gdhuwa&format=quakeml
     elif "USGS" in rid_up:
-        rid_ = rid.split("eventid=")[-1]
-        return rid_.split("&")[0]
+        parts = rid.split("eventid=")[-1]
+        event_name = parts.split("&")[0]
     # USGS ANSS ComCat: quakeml:us.anss.org/event/20005ysu
     elif "ANSS" in rid_up:
-        return rid.split("event/")[-1]
+        event_name = rid.split("event/")[-1]
+    # PySEP reads SPECFEM source files and tags them 'SOURCE'
+    # smi:local/source/<SOURCE_NAME>/event
+    elif "SOURCE" in rid_up:
+        event_name = rid_up.split("/")[2]
     else:
-        raise NotImplementedError(f"Unexpected resource id format '{rid}', "
-                                  "Please raise a GitHub issue and the "
-                                  "developers will address this")
+        logger.warning("unknown resource ID type, tagging event with entire ID")
+        event_name = rid_up
+
+    return event_name
```

### Comparing `pyatoa-0.3.1/pyatoa/utils/images.py` & `pyatoa-0.4.0/pyatoa/utils/images.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/process.py` & `pyatoa-0.4.0/pyatoa/utils/process.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,28 +52,30 @@
     if not min_freq:
         min_freq = 1 / max_period
 
     # Bandpass if both bounds given
     if min_period and max_period:
         st.filter("bandpass", corners=corners, zerophase=zerophase,
                   freqmin=min_freq, freqmax=max_freq, **kwargs)
-        logger.info(f"bandpass filter: {min_period} - {max_period}s w/ "
-                    f"{corners} corners")
+        logger.debug(f"applying 'bandpass' filter: "
+                     f"{min_period} - {max_period}s w/ {corners} corners")
 
     # Minimum period only == lowpass filter
     elif min_period:
         st.filter("lowpass", freq=max_freq, corners=corners,
                   zerophase=zerophase, **kwargs)
-        logger.info(f"lowpass filter: {min_period}s w/ {corners} corners")
+        logger.debug(f"applying 'lowpass' filter: "
+                     f"{min_period}s w/ {corners} corners")
 
     # Maximum period only == highpass filter
     elif max_period:
         st.filter("highpass", freq=min_freq, corners=corners, 
                   zerophase=zerophase, **kwargs)
-        logger.info(f"highpass filter: {max_period}s w/ {corners} corners")
+        logger.debug(f"applying 'highpass' filter: "
+                     f"{max_period}s w/ {corners} corners")
 
     return st
 
 
 def taper_time_offset(st, taper_percentage=0.05, time_offset_sec=0):
     """
     Taper the leading edge of the waveform. If a time offset is given,
@@ -139,40 +141,31 @@
         tr.data = np.pad(array, (pad_before, pad_after), mode='constant')
         tr.stats.starttime -= pad_length_in_seconds
         logger.debug(f"new starttime {tr.id}: {tr.stats.starttime}")
 
     return st_pad
 
 
-def trim_streams(st_a, st_b, precision=1E-3, force=None):
+def trim_streams(st_a, st_b, force=None):
     """
-    Trim two streams to common start and end times,
-    Do some basic preprocessing before trimming.
-    Allows user to force one stream to conform to another.
-    Assumes all traces in a stream have the same time.
-    Prechecks make sure that the streams are actually different
-
+    Trim two streams to common start and end times, allowing user to `force` 
+    one stream to conform to another. Assumes all traces in a stream have the 
+    same time.
+    
     :type st_a: obspy.stream.Stream
     :param st_a: streams to be trimmed
     :type st_b: obspy.stream.Stream
     :param st_b: streams to be trimmed
-    :type precision: float
-    :param precision: precision to check UTCDateTime differences
     :type force: str
     :param force: "a" or "b"; force trim to the length of "st_a" or to "st_b",
         if not given, trims to the common time
     :rtype: tuple of obspy.stream.Stream
     :return: trimmed stream objects in the same order as input
+    :raises AssertionError: if the streams cannot be trimmed successfully
     """
-    # Check if the times are already the same
-    if st_a[0].stats.starttime - st_b[0].stats.starttime < precision and \
-            st_a[0].stats.endtime - st_b[0].stats.endtime < precision:
-        logger.debug(f"start and endtimes already match to {precision}")
-        return st_a, st_b
-
     # Force the trim to the start and end times of one of the streams
     if force:
         if force.lower() == "a":
             start_set = st_a[0].stats.starttime
             end_set = st_a[0].stats.endtime
         elif force.lower() == "b":
             start_set = st_b[0].stats.starttime
@@ -204,54 +197,84 @@
             dt = start_set - tr.stats.starttime
             if 0 < dt < tr.stats.sampling_rate:
                 logger.info(f"shifting {tr.id} starttime by {dt}s")
                 tr.stats.starttime = start_set
             elif dt >= tr.stats.delta:
                 logger.warning(f"{tr.id} starttime is {dt}s greater than delta")
 
+    for tr_a, tr_b in zip(st_a_out, st_b_out):
+        assert(tr_a.stats.starttime == tr_b.stats.starttime), \
+            "unable to trim streams and match starttimes"
+        assert(tr_a.stats.endtime == tr_b.stats.endtime), \
+            "unable to trim streams and match endtimes"
+
     return st_a_out, st_b_out
 
 
 def match_npts(st_a, st_b, force=None):
     """
     Resampling can cause sample number differences which will lead to failure
-    of some preprocessing or processing steps. This function ensures that `npts` 
-    matches between traces by extending one of the traces with zeros. 
-    A small taper is applied to ensure the new values do not cause 
-    discontinuities.
-
-    Note:
-        its assumed that all traces within a single stream have the same `npts`
+    of some preprocessing steps. This function ensures that `npts` 
+    matches between traces by extending one of the traces with zeros, or 
+    removing data from the end of the trace. 
+
+    This is used for the case where the 'obs' data is too short w.r.t 'syn' 
+    data, so we pad out the end of the 'obs' with 0s. 
+
+    .. warning::
+
+        It is assumed you have resampled and trimmed the streams and that this
+        function is only used to make up sub-second differences in the number of
+        samples. Also assumed you will taper the end of the trace otherwise the
+        appending of zeros will cause issues.
 
     :type st_a: obspy.stream.Stream
     :param st_a: one stream to match samples with
     :type st_b: obspy.stream.Stream
     :param st_b: one stream to match samples with
     :type force: str
     :param force: choose which stream to use as the default npts,
         defaults to 'a', options: 'a', 'b'
     :rtype: tuple (obspy.stream.Stream, obspy.stream.Stream)
     :return: streams that may or may not have adjusted npts, returned in the 
         same order as provided
+    :raises AssertionError: if the number of points cannot be matched
     """
+    # Quick check to make sure all traces have the same length within one stream
+    for st in [st_a, st_b]:
+        for tr in st:
+            assert(tr.stats.npts == st[0].stats.npts), \
+                "all traces in stream must have the same number of samples"
+
     # Assign the number of points, copy to avoid editing in place
-    if not force or force == "a":
+    if force is None or force == "a":
         npts = st_a[0].stats.npts
         st_const = st_a.copy()
         st_change = st_b.copy()
     else:
         npts = st_b[0].stats.npts
         st_const = st_b.copy()
         st_change = st_a.copy()
 
     for tr in st_change:
-        diff = abs(tr.stats.npts - npts)
-        if diff:
-            logger.info(f"appending {diff} zeros to {tr.get_id()}")
+        diff = npts - tr.stats.npts 
+        if diff > 0:
+            logger.info(f"appending {diff} zeros ({diff * tr.stats.delta}s) to "
+                        f"{tr.get_id()} to match npts")
             tr.data = np.append(tr.data, np.zeros(diff))
+        elif diff < 0:
+            logger.info(f"removing {diff} zeros ({diff * tr.stats.delta}s) "
+                        f"from {tr.get_id()} to match npts")
+            tr.data = tr.data[:diff]
+        elif diff == 0:
+            continue
+
+    for tr_a, tr_b in zip(st_const, st_change):
+        assert(tr_a.stats.npts == tr_b.stats.npts), \
+            "unable to match npts between streams"
 
     # Ensure streams are returned in the correct order
     if not force or force == "a":
         return st_const, st_change
     else:
         return st_change, st_const
```

### Comparing `pyatoa-0.3.1/pyatoa/utils/srcrcv.py` & `pyatoa-0.4.0/pyatoa/utils/srcrcv.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/window.py` & `pyatoa-0.4.0/pyatoa/utils/window.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/utils/write.py` & `pyatoa-0.4.0/pyatoa/utils/write.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/visuals/improve_wave.py` & `pyatoa-0.4.0/pyatoa/visuals/wave_train.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,486 +1,348 @@
 #!/usr/bin/env python3
 """
-Functions to create a figure showing progressive waveform improvement over
-the course of a seismic inversion.
+Iteration waveform plotter for ASDFDataSets generated by SeisFlows inversions. 
 
-Show the changes in synthetic waveforms with progressive model updates. 
-Each individual model gets its on row in the plot.
+Generates a multi column, multi row plot that shows data-synthetic comparisons
+for all (or chosen) models for a chosen station. Options for plotting windows
+and calculating VRL are also available.
+
+See Chow et al., 2020 Figure 10 for an example figure.
+
+.. rubric::
+
+        wt = WaveTrain(ds=ds)
+        wt.plot(station="NN.SSS", component_list=["Z", "N", "E"], 
+                min_period=30, max_period=50)
 """
-import os
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-import pyasdf
-from pyasdf import ASDFDataSet as asdf 
-from pyatoa import Manager, logger
-from pyatoa.utils.form import format_event_name
-from pyatoa.visuals.wave_maker import format_axis
-from pyflex import logger as pflogger
+from matplotlib.patches import Rectangle
 
-pflogger.setLevel("DEBUG")
-logger.setLevel("INFO")
+from pyatoa import Manager
+from pyatoa.utils.calculate import vrl
+from pyatoa.utils.form import format_event_name
 
 
-class ImproveWave:
+class WaveTrain:
     """
-    A class to plot waveform improvement for a given ASDFDataSet
-
-    .. code:: python
-
-        ds = pyasdf.ASDFDataSet("dataset.h5")
-        wi = WaveformImprovement(ds)
-        wi.gather("NZ.BFZ", 10, 30)
-        wi.plot()
-        wi.plot("NZ.KNZ", 8, 30)
+    Simple plotter class to show waveform improvements for a given station
+    whose data are saved inside an ASDFDataSet generated by a Pyaflowa SeisFlows
+    inversion. Only requires the ASDFDataSet as input.
     """
-    def __init__(self):
+    def __init__(self, ds, models=None):
         """
         Initiate empty objects and keep dataset as an internal attribute
 
         :type ds: pyasdf.ASDFDataSet
-        :param ds: dataset containing waveform data and windows
-        """
-        # self.ds = ds
-
-        self.st_obs = None
-        self.synthetics = None
-        self.windows = None
-        self.time_axis = None
-
-    def get_models(self):
-        """
-        Figure out which step goes to which iteration to get model numbers
-        """
-        models = {"m00": "i01/s00"}
-        iterations = self.ds.auxiliary_data.MisfitWindows.list()
-        for iter_ in iterations:
-            steps = self.ds.auxiliary_data.MisfitWindows[iter_]
-            if iter_.replace("i", "m") in models:
-                continue
-            elif "s00" in steps.list():
-                models[iter_.replace("i", "m")] = f"{iter_}/s00"
-            else:
-                models[iter_.replace("i", "m")] = \
-                    f"{prev_iter}/{prev_steps.list()[-1]}"
-            prev_iter = iter_
-            prev_steps = steps
-
-        # Get the last step
-        if prev_steps.list()[-1] != "s00":
-            final_model = f"m{int(prev_iter.split('i')[-1]) + 1:0>2}"
-            models[final_model] = f"{prev_iter}/{prev_steps.list()[-1]}"
-
-        return models
-
-    def gather(self, sta, min_period, max_period, rotate_to_rtz=False,
-               fix_windows=False, pyflex_preset=False):
-        """
-        Parse dataset for given station, gather observed and synthetic data, 
-        preprocess data and return as stream objects.
-
-        :type sta: str
-        :param sta: station to gather data for
+        :param ds: ASDFDataSet generated by a SeisFlows inversion
+        :type models: list
+        :param models: list of models to plot, which must match the available
+            iteration/step_count stored in the ASDFDataSet. Models should
+            be in the format i01/s00 (iteration/step_count). If not provided
+            the class will attempt to find all available models in the dataset,
+            by assuming that the first model is i01/s00, that each subsequent
+            model is i0?/s00, and that the final model is the last step of the
+            last iteration.
+        """
+        self.ds = ds
+        self.models = models
+        self.evaluations = self._get_all_evaluations()
+
+        if self.models:
+            assert set(self.models).issubset(set(self.evaluations)), \
+                   f"Models don't match expected evaluations in the ASDFDataSet"
+        else:
+            self.models = self.evaluations
+    
+    def _get_all_evaluations(self):
+        """Get all available evaluations in the dataset, used for validating
+        model names"""
+        evaluations = []
+        for iteration in self.ds.auxiliary_data.Configs.list():
+            for step in self.ds.auxiliary_data.Configs[iteration].list():
+                evaluations.append(f"{iteration}/{step}")
+        return evaluations  
+
+    def _gather(self, station, model, min_period=None, max_period=None,
+               **kwargs):
+        """
+        Gather data from an ASDFDataSet based on the given model (iter/step)
+
+        :type station: str
+        :param station: name of the station as listed in the ASDFDataSet, in
+            the format NN.SSS (N=network, S=station)
+        :type model: str
+        :param model: model to gather data for, in the format i01/s00
         :type min_period: float
-        :param min_period: minimum filter period in seconds
+        :param min_period: minimum period for the filter corners, if not given
+            no filter applied
         :type max_period: float
-        :param max_period: maximum filter period in seconds
-        :type rotate_to_rtz: bool
-        :param rotate_to_rtz: rotate components from NEZ to RTZ
-            Config. if False, instrument response will be removed from obs.
-        :type fix_windows: bool
-        :param fix_windows: dont recalculate windows when gathering
-        :type pyflex_preset: str
-        :param pyflex_preset: overwrite the pyflex preset provided in the
-            Config object
-        """
-        if min_period is None or max_period is None:
-            raise TypeError("must specify 'min_period' and 'max_period'")
+        :param max_period: maximum period for the filter corners, if not given
+            no filter applied
+        :rtype: (obspy.core.stream.Stream, obspy.core.stream.Stream, dict, 
+                 float)
+        :return: observed, synthetic, windows, time offset [s]
+        """
+        # Use the Manager class to load in waveform data
+        mgmt = Manager(ds=self.ds)
+        mgmt.load(code=station, path=model, windows=True)
+
+        # Overwrite the filter corners stored in the dataset
+        mgmt.config.min_period = min_period
+        mgmt.config.max_period = max_period
+        mgmt.standardize()
+        mgmt.preprocess(**kwargs)
 
-        assert(sta in self.ds.waveforms.list()), f"{sta} not in ASDFDataSet"
+        return mgmt.st_obs, mgmt.st_syn, mgmt.windows, \
+            mgmt.stats.time_offset_sec
 
-        models = self.get_models()
-
-        # Preprocess all traces using Pyatoa and store in dict
-        st_obs, synthetics, windows = None, {}, {}
-        for model, path in models.items():
-            # Gather synthetic data
-            mgmt = Manager(ds=self.ds)   
-            print(path)
-            mgmt.load(sta, path)
-
-            # Overwrite some config parameters
-            mgmt.config.min_period = min_period
-            mgmt.config.max_period = max_period
-            if rotate_to_rtz:
-                mgmt.config.rotate_to_rtz = rotate_to_rtz
-                mgmt.config.component_list = ["Z", "R", "T"]
-            if pyflex_preset:
-                mgmt.config.pyflex_preset = pyflex_preset
-                mgmt.config._check()
-
-            mgmt.standardize()
-            mgmt.preprocess() 
-            iter_, step_ = path.split("/")
-            mgmt.window(fix_windows=fix_windows, iteration=iter_,
-                        step_count=step_)
-
-            windows[model] = mgmt.windows
-            synthetics[model] = mgmt.st_syn.copy() 
-
-            # Observed waveform will be the same
-            if st_obs is None:
-                st_obs = mgmt.st_obs.copy()
-
-        # Internally used by plotting function
-        self.st_obs = st_obs
-        self.synthetics = synthetics
-        self.windows = windows
-        self.time_axis = self.st_obs[0].times(
-            reftime=st_obs[0].stats.starttime - mgmt.stats.time_offset_sec
-            ) 
-
-    def gather_simple(self, event, sta, min_period, max_period, path_dict=None,
-                      component=None):
-        """
-        Manually set the model values based on inspection of the Inspector
-        Don't return windows or anything, keep it simple
-        """
-
-        models = {"m00": ("i01/s00", "a"),
-                  "m03": ("i03/s03", "a"),
-                  "m09": ("i09/s02", "a"),
-                  "m12": ("i12/s04", "a"),
-                  "m17": ("i17/s01", "a"),
-                  "m24": ("i07/s01", "b"),
-                  "m28": ("i11/s03", "c"),
-                  }
-        st_obs, synthetics = None, {}
-        windows = None
-        for model, tup in models.items():
-            path, tag = tup
-            if path_dict:
-                ds_fid = os.path.join(path_dict[tag], f"{event_id}.h5")
-            else:
-                ds_fid = f"{event_id}{tag}.h5"
-            with asdf(ds_fid, mode="r") as ds:
-                mgmt = Manager(ds=ds)
-                mgmt.load(sta, path)
-                mgmt.config.min_period = min_period
-                mgmt.config.max_period = max_period
-                mgmt.standardize().preprocess()
-
-                if component:
-                    synthetics[model] = mgmt.st_syn.select(
-                                                     component=component).copy()
-                else:
-                    synthetics[model] = mgmt.st_syn.copy()
-                if st_obs is None:
-                    if component:
-                        st_obs = mgmt.st_obs.select(component=component).copy()
-                    else:
-                        st_obs = mgmt.st_obs.copy()
-
-        self.st_obs = st_obs
-        self.synthetics = synthetics
-
-    def setup_plot(self, nrows, ncols, **kwargs):
+    def _setup_plot(self, nrows, ncols, **kwargs):
         """
         Dynamically set up plots according to number_of given
         Returns a list of lists of axes objects
         e.g. axes[i][j] gives the ith column and the jth row
 
         :type nrows: int
         :param nrows: number of rows in the gridspec
         :type ncols: int
         :param ncols: number of columns in the gridspec
         :rtype axes: matplotlib axes
         :return axes: axis objects
         """
+        figure = kwargs.get("figure", None)
+        subplot_spec = kwargs.get("subplot_spec", None)
         dpi = kwargs.get("dpi", 150)
-        figsize = kwargs.get("figsize", (500/dpi, 800/dpi))
-        fontsize = kwargs.get("fontsize", 10)
+        figsize = kwargs.get("figsize", (1200 / dpi, (240 * nrows) / dpi))
+        fontsize = kwargs.get("fontsize", 12)
         axis_linewidth = kwargs.get("axis_linewidth", 2)
-
-        f = plt.figure(figsize=figsize, dpi=dpi)
-        gs = mpl.gridspec.GridSpec(nrows, ncols, hspace=0, wspace=0.025, 
-                                   width_ratios=[1] * ncols,
-                                   height_ratios=[3] * nrows
-                                   )
+        xticks = kwargs.get("xticks", True)
+        yticks = kwargs.get("yticks", True)
+        minor_ticks = kwargs.get("minor_ticks", False)
+
+        # Initiate the figure, allow for external figure objects
+        if figure is None:
+            f = plt.figure(figsize=figsize, dpi=dpi)
+        else:
+            f = figure
+
+        # Initiate gridspec, allow for nested grids
+        subplot_kwargs = {"hspace": 0, "wspace": 0.025, 
+                          "width_ratios": [5] * ncols, 
+                          "height_ratios": [1] * nrows}
+        if subplot_spec is None:
+            gs = mpl.gridspec.GridSpec(nrows, ncols, **subplot_kwargs)
+        else:
+            gs = mpl.gridspec.GridSpecFromSubplotSpec(nrows, ncols,
+                                                      subplot_spec=subplot_spec,
+                                                      **subplot_kwargs)
 
         axes = [[] for _ in range(nrows)]
         for row in range(0, gs.get_geometry()[0]):
             for col in range(0, gs.get_geometry()[1]):
-                # Ensure axis sharing
+                # First column can't share y-values
                 if col == 0:
                     sharey = None
                 else:
                     sharey = axes[row][0]
+                # First entry can't share x-values
                 if row == 0 and col == 0:
                     sharex = None
                 else:
                     sharex = axes[0][0]
 
                 ax = plt.subplot(gs[row, col], sharey=sharey, sharex=sharex)
+
                 ax.set_axisbelow(True)
-                ax.minorticks_on()
-                ax.tick_params(which='major', direction='in', top=True,
-                               right=False, left=False, labelsize=fontsize, 
-                               length=3, width=2*axis_linewidth/3)
-                ax.tick_params(which='minor', direction='in', length=1.5, 
-                               top=True, bottom=True, right=False, left=False, 
-                               width=2*axis_linewidth/3)
+                
+                left = bool(yticks)
+                bottom = bool(xticks) 
+
+                ax.tick_params(which='major', direction='in', top=False,
+                               right=False, left=left, bottom=bottom, 
+                               labelsize=fontsize,
+                               length=5, width=2*axis_linewidth/3)
+                if minor_ticks:
+                    ax.minorticks_on()
+                    ax.tick_params(which='minor', direction='in', length=3, 
+                                   top=False, bottom=bottom, right=False, 
+                                   left=left, width=2*axis_linewidth/3)
+                if col == 0:
+                    ax.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
+                    # Make sure the scientific notation has the same4fontsize
+                    ax.yaxis.get_offset_text().set_fontsize(fontsize)
 
                 for axis in ["top", "bottom", "left", "right"]:
                     ax.spines[axis].set_linewidth(axis_linewidth)
-               
-                # Turn off the y axes because we wont show units
-                ax.get_yaxis().set_ticks([])
 
+                # Set the grids on
                 axes[row].append(ax)
 
-
         # remove x-tick labels except for last axis
         for row in axes[:-1]:
             for col in row:
                 plt.setp(col.get_xticklabels(), visible=False)
 
-        return f, axes
+        # Turn off the y-tick labels and sci notation for columns except first
+        for row in axes:
+            # for col in row[1:]:
+            for col in row[:]:
+                plt.setp(col.get_yticklabels(), visible=False)
+                col.yaxis.get_offset_text().set_visible(False)
 
-    def plot(self, sta=None, event_id=None, min_period=None, max_period=None, 
-             plot_windows=False, trace_length=None, show=True, save=False, 
-             **kwargs):
-        """
-        Plot waveforms iterative based on model updates
+        return f, axes
 
-        :type sta: str
-        :param sta: station to gather data for, if None, skips gathering
-            assuming data has already been gathered
+    def plot(self, station, min_period=None, max_period=None, models=None,
+             component_list=None, title=None, label_tshift=True, xlim=None, 
+             calculate_vrl=True, show=True, save=False, **kwargs):
+        """
+        Plot waveforms iterative based on model updates. Calls `_gather`
+        to grab preprocessed waveform data from the internal ASDFDataSet `ds`.
+        Kwargs are passed to the underlying Manager.preprocess. function.
+
+        :type station: str
+        :param station: name of the station as listed in the ASDFDataSet, in
+            the format NN.SSS (N=network, S=station)
         :type min_period: float
-        :param min_period: minimum filter period for waveforms
+        :param min_period: minimum period for the filter corners, if not given
+            no filter applied
         :type max_period: float
-        :param max_period: maximum filter period for waveforms
-        :type plot_windows: bool
-        :param plot_windows: plot misfit windows above waveforms
-        :type trace_length: list of floats
-        :param trace_length: [trace_start, trace_end] will be used to set the x
-            limit on the waveform data. If none, no xlim will be set
+        :param max_period: maximum period for the filter corners, if not given
+            no filter applied
+        :type models: list
+        :param models: list of models to plot, if not set, all models plotted
+        :type component_list: list
+        :param component_list: list of components to plot, e.g. ["Z", "N", "E"]
+        :type title: str
+        :param title: title of the plot, if not set, the station code is used
+        :type xlim: list
+        :param xlim: x-axis limits for the plot, if not set, uses full time
+        :type calculate_vrl: bool
+        :param calculate_vrl: calculate the variance reduction for each model 
+            and annotate the value in the corner of each figure
+        :type label_tshift: bool
+        :param label_tshift: label the time shift in the top corner of each
+            window in units seconds
         :type show: bool
         :param show: Show the plot or do not
         :type save: str
         :param save: if given, save the figure to this path
         """
-        linewidth = kwargs.get("linewidth", 1.)
-        fontsize = kwargs.get("fontsize", 10)
-        anno_fontsize = kwargs.get("anno_fontsize", 8)
-        window_color = kwargs.get("window_color", "orange")
-        percent_over = kwargs.get("percent_over", 0.125)
-        anno_choice = kwargs.get("anno_choice", "all")
-
-        # Allows for skipping the gather call and including it directly in plot
-        if sta is not None:
-            self.gather(sta, min_period, max_period)
-
-        assert self.st_obs, "must collect data for a station before plotting"
-
-        # Instantiate the plotting object
-        f, axes = self.setup_plot(nrows=len(self.synthetics.keys()), 
-                                  ncols=len(self.st_obs), **kwargs)
-
-        # if not trace_length:
-        #     trace_length = [self.time_axis[0], self.time_axis[-1]]
-
-        # Plot each model on a different row
-        synthetic_keys = list(self.synthetics.keys())
-        synthetic_keys.sort()
-        for row, syn_key in enumerate(synthetic_keys):
-            ylab = syn_key.split('_')[-1]  # e.g. 'm00'
+        obs_lw = kwargs.get("obs_lw", 1.)
+        syn_lw = kwargs.get("syn_lw", 1.25)
+        fontsize = kwargs.get("fontsize", 12)
+        obs_color = kwargs.get("color_obs", "k")
+
+        # Colors for each component that generally work well together
+        syn_colors = ["orangered", "dodgerblue", "yellowgreen"]
+
+        # Dynamically retrieve component list from the dataset
+        if component_list is None:
+            component_list = [_.stats.component for _ in 
+                              self.ds.waveforms[station].observed]
+        # User set model values or not. Check if these are valid model values
+        if models is None:
+            models = self.models
+
+        # One row per component, one column for init and final each
+        f, axes = self._setup_plot(nrows=len(models), 
+                                   ncols=len(component_list), **kwargs)
+
+        # Plot each component in a different column
+        s_init = []
+        for row, model in enumerate(models):
+            obs, syn, windows, t_offset = self._gather(
+                station=station, min_period=min_period, max_period=max_period,
+                model=model, **kwargs
+                )  
+            # Loop through waveforms first to get max y value
+            max_amp = 0
+            for o, s in zip(obs, syn):
+                max_amp = max(max_amp, np.max(np.abs(o.data)), 
+                              np.max(np.abs(s.data))) * 1.05
 
-            # Plot each component in a different column
-            component_list = [_.stats.channel[-1] for _ in self.st_obs]
             for col, comp in enumerate(component_list):
-                obs = self.st_obs.select(component=comp)[0]
-                syn = self.synthetics[syn_key].select(component=comp)[0]
+                o = obs.select(component=comp)[0]
+                s = syn.select(component=comp)[0]
+                axes[row][col].plot(o.times() + t_offset, o.data, obs_color, 
+                                    zorder=10, linewidth=obs_lw)
+                axes[row][col].plot(s.times() + t_offset, s.data, 
+                                    syn_colors[col],  zorder=11, 
+                                    linewidth=syn_lw)
+                
+                # Plot the windows as rectangles if they are available
+                if comp in windows:
+                    for window in windows[comp]:
+                        tleft = window.left * window.dt + t_offset
+                        tright = window.right * window.dt
+                        r = Rectangle(xy=(tleft, -1 * max_amp),  
+                                    width=tright - tleft,
+                                    height=max_amp * 2, fc="orange", 
+                                    ec="k", alpha=0.1, zorder=10
+                                    )
+                        axes[row][col].add_patch(r)
+                        # Add timeshift label in top corner of window
+                        if label_tshift:
+                            tshift_s = window.cc_shift * window.dt
+                            sign = "+" if tshift_s > 0 else "-"
 
-                # Plot waveforms
-                a1, = axes[row][col].plot(obs.times(), obs.data, 'k', 
-                                          zorder=10, label="Obs", 
-                                          linewidth=linewidth)
-                a2, = axes[row][col].plot(syn.times(), syn.data, 
-                                          ["r", "b", "g"][col], zorder=10,
-                                          label="Syn", linewidth=linewidth)
-
-                # Format the axes for a standardized look
-                format_axis(axes[row][col], percent_over=percent_over)
-
-                # Plot windows if available for this given component
-                tshift_max = 0  # temporary
-                if plot_windows:
-                    windows = self.windows[syn_key].get(comp, [])
-                    for w, win in enumerate(windows):
-                        ymin, ymax = axes[row][col].get_ylim()
-
-                        tleft = win.left * win.dt + self.time_axis[0]
-                        tright = win.right * win.dt + self.time_axis[0]
-                        tshift = win.cc_shift * win.dt
-
-                        axes[row][col].add_patch(mpl.patches.Rectangle(
-                                      xy=(tleft, ymin), width=tright-tleft, 
-                                      ec='k', fc=window_color,
-                                      height=(ymax + np.abs(ymin)), 
-                                      alpha=(win.max_cc_value **2) / 4)
-                        )
-                        # Outline the rectangle with solid lines
-                        for t_ in [tleft, tright]:
-                            axes[row][col].axvline(x=t_, ymin=0, ymax=1, 
-                                                   color="k", alpha=1., 
-                                                   zorder=11)
-
-                        # Annotate time shift value into window,
-                        # Alternate height if multiple windows so no overlap
-                        if anno_choice == "all":
                             axes[row][col].text(
-                                s=f"{tshift:.2f}s", x=tleft, 
-                                y=(ymax-ymin)*[0.7, 0.06][w%2]+ymin,
-                                fontsize=anno_fontsize, zorder=11
+                                x=tleft, y=max_amp - max_amp * 0.05, 
+                                s=f"{sign}{np.abs(tshift_s):.2f}s",  
+                                verticalalignment="top", 
+                                fontsize=6, 
                                 )
+                
+                # Turn off y-ticks, they carry no information
+                axes[row][col].set_yticks([])
 
-                        # If only annotate the largest timeshift
-                        if abs(tshift) > abs(tshift_max):
-                            tshift_max = tshift
-                            tleft_max = tleft
-                            # tright_max = tright
+                # Set all y-max values to the maximum amplitude in the row
+                axes[row][col].set_ylim([-1 * max_amp, max_amp])
 
-                    # If annotate largesttime shift value into window
-                    if tshift_max and anno_choice == "max":
+                # First row gets the component formatted into the corner
+                if row == 0:
+                    axes[row][col].text(
+                        x=0.99, y=0.01, s=comp.upper(), fontsize=fontsize, 
+                        c=syn_colors[col], horizontalalignment="right", 
+                        verticalalignment="bottom", 
+                        transform=axes[row][col].transAxes
+                        )
+                    s_init.append(s)
+                # All other rows get the VRL value which determines improvement
+                else:
+                    if calculate_vrl:
+                        vrl_val = vrl(o.data, s.data, s_init[col].data)
                         axes[row][col].text(
-                            s=f"{tshift_max:.2f}s", x=tleft_max, 
-                            y=(ymax-ymin)*0.06 + ymin,
-                            fontsize=anno_fontsize, zorder=11
+                            x=1., y=.95, s=f"VRL={vrl_val:.2f}", 
+                            fontsize=8, 
+                            horizontalalignment="right", 
+                            verticalalignment="top",
+                            transform=axes[row][col].transAxes
                             )
-
-                if row == 0:
-                    # determine how long the traces should be
-                    # hardcode the trace length based on user params
-                    if isinstance(trace_length, list):
-                        axes[row][col].set_xlim(trace_length)
-                    # else:
-                    #     axes[row][col].set_xlim([
-                    #         np.maximum(self.time_axis[0], -10), t[-1]
-                    #         ])
-
-                    # Set titles for the first row, middle column
-                    if col == len(self.st_obs) // 2:
-                        title = (f"{self.st_obs[0].stats.network}."
-                                 f"{self.st_obs[0].stats.station} "
-                                 f"{event_id} Z")
-                        axes[row][col].set_title(title, fontsize=fontsize)
             
-                    # Append component to bottom right of subplot  
-                    if False:
-                        axes[row][col].text(
-                                    x=0.95, y=0.15, s=comp.upper(),
-                                    horizontalalignment="center",
-                                    verticalalignment="center",
-                                    transform=axes[row][col].transAxes)
-          
-            # y-label after all the processing has occurred
-            axes[row][0].set_ylabel(ylab, rotation="horizontal", ha="right",
-                                    fontsize=fontsize)
-
-        # Label the time axis on the bottom row, middle column
-        axes[-1][len(self.st_obs) // 2].set_xlabel("time [s]", 
-                                                   fontsize=fontsize)
+            # Write the model number in the y-label of the leftmost column
+            axes[row][0].set_ylabel(model, fontsize=fontsize)
+                    
+        # Finalize plot looks: set time axis label
+        middle_column = len(component_list) // 2
+        axes[-1][middle_column].set_xlabel("Time [s]", fontsize=fontsize)
+
+        # Set the time axes which should be the same for all
+        if xlim is None:
+            xlim = [_ + t_offset for _ in [o.times()[0], o.times()[-1]]]
+        plt.xlim(xlim)
+
+        # Set title
+        if title is None:
+            title = (f"{format_event_name(self.ds)} -> {station} "
+                     f"({min_period}-{max_period}s)")
+        plt.suptitle(title, fontsize=fontsize)
 
         # Save the generated figure
         if save:
             plt.savefig(save)
         if show:
             plt.show()
 
         return f, axes
 
-    def gather_simple(self, models, event_id, sta, component,  min_period,
-                      max_period):
-        """
-        Gather waveforms from manually input model values, usually determined
-        by using the Inspector class
-
-        :type models: dict of tuples
-        :param models: model values as keys, (iter/step, tag) as tuple value.
-            Tags allow multiple datasets to be used, e.g. if an inversion
-            spans over multiple legs and more than one dataset is used to
-            store waveform data
-        :type event_id: str
-        :param event_id: name of the event, used to access the ASDFDataSet
-        ;type sta: str
-        :param sta: station id to gather data for
-        :type min_period: float
-        :param min_period: period to filter data at
-        :type max_period: float
-        :param max_period: period to filter data at
-        """
-        st_obs, synthetics = None, {}
-
-if __name__ == "__main__":
-    pairs = [
-         ("2013p617227", "NZ.TOZ", "Z"),
-         # ("2014p952799", "NZ.NTVZ", "N"),
-         # ("2016p105478", "NZ.PUZ", "Z"),
-         # ("2016p881118", "NZ.MWZ", "E"),
-         # ("2018p465580", "NZ.KHEZ", "E"),
-         # ("2019p738432", "NZ.KHZ", "Z"),
-         # ("2019p754447", "NZ.HIZ", "Z"),
-         # ("2019p927023", "NZ.VRZ", "Z"),
-         ]    
-    
-    path_dict = {"a": "../waveform_comparisons/aspen/",
-                 "b": "/home/chowbr/current/birch/scratch/preprocess/datasets/i07_corrupted/",
-                 "c": "../waveform_comparisons/birch/"}
-
-    for event_id, sta, comp in pairs:
-        wi = ImproveWave()
-        wi.gather_simple(event_id, sta, 6, 30, path_dict=path_dict, component=comp)
-        wi.plot(show=False, save=f"{event_id}_{sta}.png", event_id=event_id,
-                trace_length=[70,290])
-    a=1/0
-
-    # MAIN
-    event_id = "2019p927023"
-    with asdf(f"{event_id}a.h5") as ds:
-        stations = ds.waveforms.list()
-        self.st_obs = st_obs
-        self.synthetics = synthetics
-
-
-if __name__ == "__main__":
-    event_id = "2013p507880"
-    component = "Z"
-    models = {"m00": ("i01/s00", ""),
-              "m01": ("i01/s04", ""),
-              "m02": ("i02/s01", ""),
-              "m02": ("i03/s00", ""),
-              "m03": ("i03/s01", ""),
-              "m03": ("i04/s00", ""),
-              "m04": ("i04/s04", ""),
-              "m04": ("i05/s00", ""),
-              "m05": ("i05/s04", ""),
-              "m05": ("i06/s00", ""),
-              "m06": ("i06/s01", ""),
-              "m07": ("i07/s01", ""),
-              "m08": ("i08/s03", ""),
-              "m09": ("i09/s01", ""),
-              "m10": ("i10/s04", ""),
-              "m10": ("i11/s00", ""),
-              "m11": ("i11/s03", ""),
-              "m12": ("i12/s01", ""),
-              "m13": ("i13/s01", ""),}
-
-    # with asdf(f"{event_id}.h5") as ds:
-    #     stations = ds.waveforms.list()
-    stations = ["NZ.TOZ"]
-
-        
-    for sta in stations:
-        wi = ImproveWave()
-        wi.gather_simple(models, event_id, sta, component, 4, 30)
-        wi.plot()
```

### Comparing `pyatoa-0.3.1/pyatoa/visuals/insp_plot.py` & `pyatoa-0.4.0/pyatoa/visuals/insp_plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 common_labels = {"cc_shift_in_seconds": "Time Shift (s)",
                  "dlnA": "$\Delta\ln$(A)",
                  "misfit": "Misfit",
                  "length_s": "Window Length (s)",
                  "max_cc_value": "Peak Cross Correlation",
                  "relative_starttime": "Relative Start Time (s)",
                  "relative_endtime": "Relative End Time (s)",
+                 "nwin": "Number of Windows per Event",
+                 "nwin_sta": "Number of Windows per Station",
                  }
+# Allow quick adjustment of the dots per inch for figures
+DEFAULT_DPI = 150
 
 
 class InspectorPlotter:
     """
     A class of methods for plotting statistics from an Inspector.
     Should not be called on its own, these functions will be inherited by
     the Inspector class automatically.
@@ -41,24 +45,27 @@
         :type station: str or list
         :param station: particular station or list of stations to plot
         :type show: bool
         :param show: Show the plot
         :type save: str
         :param save: fid to save the given figure
         """
+        markersize = kwargs.get("markersize", 10)
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
         # For isolating parameters, ensure they are lists. quack
         if isinstance(event, str):
             event = [event]
         if isinstance(network, str):
             network = [network]
         if isinstance(station, str):
             station = [station]
 
-        markersize = kwargs.get("markersize", 10)
-        f, ax = plt.subplots()
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
 
         if not self.sources.empty:
             # Allow for isolation of particular events
             if event is not None:
                 srcs = self.sources.loc[event]
             else:
                 srcs = self.sources
@@ -114,47 +121,112 @@
             hover_on_plot(f, ax, sc_sources, src_names)
             for rcvs, rcv_names in zip(sc_receiver_list, sc_receiver_names):
                 hover_on_plot(f, ax, rcvs, rcv_names)
             plt.show()
 
         return f, ax
 
-    def scatter(self, x, y, iteration=None, step_count=None, save=None,
-                show=True, **kwargs):
+    def event_depths(self, xaxis="longitude", show=True, save=None, **kwargs):
+        """
+        Create a scatter plot of events at depth. Compresses all events onto a
+        single slice, optional choice of showing the x-axis or the y-axis
+
+        :type xaxis: str
+        :param xaxis: variable to use as the x-axis on the plot
+            'latitude' or 'longitude'
+        :type show: bool
+        :param show: show the plot
+        :type save: str
+        :param save: fid to save the figure
+        """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
+        if xaxis == "latitude":
+            x_vals = self.sources.latitude.to_numpy()
+        elif xaxis == "longitude":
+            x_vals = self.sources.longitude.to_numpy()
+        else:
+            raise NotImplementedError(
+                "'xaxis' must be 'latitude' or 'longitude"
+            )
+
+        # Plot initializations
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
+        depths = self.sources.depth_km.to_numpy()
+        mags = self.sources.magnitude.to_numpy()
+        mags = normalize_a_to_b(mags, 100, 500)
+        names = self.sources.index
+
+        # Inverted axis for positive depth values
+        if depths[0] > 0:
+            plt.gca().invert_yaxis()
+
+        # Scatter plot
+        sc = plt.scatter(x_vals, depths, s=mags, c="None", marker="o",
+                         edgecolors="k")
+        plt.xlabel(xaxis.capitalize())
+        plt.ylabel("Depth (km)")
+        plt.title(f"N={len(depths)}")
+        plt.grid(which="both", linestyle=":", alpha=0.5)
+        hover_on_plot(f, ax, sc, names, dissapear=True)
+
+        default_axes(ax, **kwargs)
+
+        if save:
+            plt.savefig(save)
+        if show:
+            plt.show
+
+        return f, ax
+
+    def scatter(self, x, y, iteration=None, step_count=None, event=None,
+                network=None, station=None, channel=None, component=None,
+                save=None, show=True, **kwargs):
         """
         Create a scatter plot between two chosen keys in the windows attribute
 
         :type x: str
         :param x: key to choose for the x axis of the plot
         :type y: str
         :param y: key to chooose for the y axis of the plot
         :type iteration: str
         :param iteration: the chosen iteration to plot for, if None will default
             to the latest iteration available
         :type step_coutn: str
         :param step_count: chosen step count. If None, defaults to latest
         """
-        if iteration is None:
-            iteration, _ = self.initial_model
-        if step_count is None:
-            step_count = self.steps.loc[iteration][-1]
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+        marker = kwargs.get("marker", "o")
+        s = kwargs.get("s", 8)
+        c = kwargs.get("c", "None")
+        edgecolors = kwargs.get("edgecolor", "k")
+        linewidths = kwargs.get("linewidths", 1)
+
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
         # Ensure we have distance and backazimuth values in the dataframe
-        df = self.isolate(iteration=iteration, step_count=step_count, **kwargs)
+        df = self.isolate(iteration=iteration, step_count=step_count,
+                          event=event, network=network, station=station, 
+                          channel=channel, component=component)
         df = df.merge(self.srcrcv, on=["event", "network", "station"])
 
         assert(x in df.keys()), f"X value {x} does not match keys {df.keys()}"
         assert(y in df.keys()), f"Y value {y} does not match keys {df.keys()}"
 
-        f, ax = plt.subplots(figsize=(8, 6))
-        plt.scatter(df[x].to_numpy(), df[y].to_numpy(), **kwargs)
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
+        plt.scatter(df[x].to_numpy(), df[y].to_numpy(), zorder=11,
+                    marker=marker, c=c, s=s, edgecolors=edgecolors,
+                    linewidths=linewidths)
         plt.xlabel(x)
         plt.ylabel(y)
-        plt.title(f"{x} vs. {y}; N={len(x)}")
+        plt.title(f"{x} vs. {y}; N={len(df[x].to_numpy())}")
         default_axes(ax, **kwargs)
+        plt.grid(zorder=10)
 
         if save:
             plt.savefig(save)
         if show:
             plt.show()
 
         return f, ax
@@ -188,27 +260,27 @@
         :param hist: create a histogram binning the approximate seismic 
             velocities
         :type plot_end: bool
         :param plot_end: if True, plots the beginning and end of the misfit 
             window as a vertical line. If False, plots only the beginning of 
             the misfit window
         """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
         hist_color = kwargs.get("hist_color", "deepskyblue")
         title_plot = kwargs.get("title_plot", None)
         title_hist = kwargs.get("title_hist", None)
         markersize = kwargs.get("markersize", 1)
         markertype = kwargs.get("markertype", "x")
         legend_fontsize = kwargs.get("legend_fontsize", 8)
         ylim = kwargs.get("ylim", None)
         xlim = kwargs.get("xlim", None)
 
-        if iteration is None:
-            iteration, _ = self.final_model
-        if step_count is None:
-            step_count = self.steps.loc[iteration][-1]
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
         # Ensure we have distance and backazimuth values in the dataframe
         df = self.isolate(iteration=iteration, step_count=step_count,
                           component=component)
         df = df.merge(self.srcrcv, on=["event", "network", "station"])
 
         # Assuming that isolate has only picked values from a single iterstep
@@ -221,15 +293,15 @@
         # Shift relative starttimes by the user-defined offset
         start -= t_offset
         end -= t_offset
 
         # size of the markers based on the length of the window
         length = normalize_a_to_b(length, .5, .5)
 
-        f, ax = plt.subplots(figsize=(8, 6))
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
        
         # Either plot the window start only, or plot the entire window
         if not plot_end:
             plt.scatter(dist, start, c="k", s=markersize, marker=markertype, 
                         zorder=5, alpha=0.5)
         else:
             for d_, s_, e_ in zip(dist, start, end):
@@ -298,66 +370,14 @@
             default_axes(plt.gca(), **kwargs)
 
             if save:
                 plt.savefig(f"hist_{save}")
             if show:
                 plt.show()
 
-
-    def event_depths(self, xaxis="longitude", show=True, save=None, **kwargs):
-        """
-        Create a scatter plot of events at depth. Compresses all events onto a
-        single slice, optional choice of showing the x-axis or the y-axis
-
-        :type xaxis: str
-        :param xaxis: variable to use as the x-axis on the plot
-            'latitude' or 'longitude'
-        :type show: bool
-        :param show: show the plot
-        :type save: str
-        :param save: fid to save the figure
-        """
-        if xaxis == "latitude":
-            x_vals = self.sources.latitude.to_numpy()
-        elif xaxis == "longitude":
-            x_vals = self.sources.longitude.to_numpy()
-        else:
-            raise NotImplementedError(
-                "'xaxis' must be 'latitude' or 'longitude"
-            )
-
-        # Plot initializations
-        f, ax = plt.subplots(figsize=(8, 6))
-        depths = self.sources.depth_km.to_numpy()
-        mags = self.sources.magnitude.to_numpy()
-        mags = normalize_a_to_b(mags, 100, 500)
-        names = self.sources.index
-
-        # Inverted axis for positive depth values
-        if depths[0] > 0:
-            plt.gca().invert_yaxis()
-
-        # Scatter plot
-        sc = plt.scatter(x_vals, depths, s=mags, c="None", marker="o",
-                         edgecolors="k")
-        plt.xlabel(xaxis.capitalize())
-        plt.ylabel("Depth (km)")
-        plt.title(f"N={len(depths)}")
-        plt.grid(which="both", linestyle=":", alpha=0.5)
-        hover_on_plot(f, ax, sc, names, dissapear=True)
-
-        default_axes(ax, **kwargs)
-
-        if save:
-            plt.savefig(save)
-        if show:
-            plt.show
-
-        return f, ax
-
     def raypaths(self, iteration=None, step_count=None, color_by=None,
                  show=True, save=False, vmin=None, vmax=None, **kwargs):
         """
         Plot rays connecting sources and receivers based on the availability
         of measurements. Useful for getting an approximation of resolution.
 
         :type iteration: int
@@ -369,31 +389,41 @@
             nwin: color rays by the number of windows available for that path
             misfit: color rays by total misfit
         :type show: bool
         :param show: show the plot
         :type save: str
         :param save: fid to save the figure
         """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
         cmap = kwargs.get("cmap", "viridis")
         ray_color = kwargs.get("ray_color", "k")
         ray_linewidth = kwargs.get("ray_linewidth", 1)
         ray_alpha = kwargs.get("ray_alpha", 0.1)
         station_color = kwargs.get("station_color", "c")
         event_color = kwargs.get("event_color", "orange")
-        figsize = kwargs.get("figsize", (8, 8))
         markersize = kwargs.get("markersize", 25)
 
-        f, ax = plt.subplots(figsize=figsize)
-
-        iteration, step_count = self._parse_nonetype_eval(iteration, step_count)
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
         df = self.misfit(level="station").loc[iteration, step_count]
+        # Rearranging the index so that the separate multi indices of 'network'
+        # and 'station' are combined to become 'network'.'station'
+        df.index = [df.index.get_level_values(0),
+                    df.index.map('{0[1]}.{0[2]}'.format)]
 
         # Get lat/lon information from sources and receivers
-        stations = self.receivers.droplevel(0)  # remove network index
+        stations = self.receivers
+        netstas = self.netsta.to_numpy()
+        netstas = [f"{net}.{sta}" for net, sta in netstas]
+
+        # Drop duplicate station names, assuming that they will have the same
+        # coordinates. This is to deal with e.g., TA -> AK networks
+        stations = stations[~stations.index.duplicated(keep="first")]
         events = self.sources.drop(["time", "magnitude", "depth_km"], axis=1)
 
         # Set up the normalized colorbar 
         cbar, extend = None, None
         if color_by is not None:
             assert(color_by in df.keys()), f"{color_by} must be in {df.keys()}"
             if vmin is None:
@@ -410,17 +440,20 @@
 
             sm, norm, cbar = colormap_colorbar(cmap, vmin=vmin, vmax=vmax,
                                                cbar_label=color_by.capitalize(),
                                                extend=extend
                                                )
 
         plotted, names = [], []
-        for event, sta in df.index.to_numpy():
+        for event, netsta in df.index.to_numpy():
             elon, elat = events.loc[event].longitude, events.loc[event].latitude
-            slon, slat = stations.loc[sta].longitude, stations.loc[sta].latitude
+
+            net, sta = netsta.split(".")
+            slon = stations.loc[net].loc[sta].longitude
+            slat = stations.loc[net].loc[sta].latitude
             # Plot a marker for each event and station
             if event not in plotted:
                 plt.scatter(elon, elat, marker="o", c=event_color,
                             edgecolors="k", s=markersize, zorder=100)
                 plotted.append(event)
             if sta not in plotted:
                 plt.scatter(slon, slat, marker="v", c=station_color,
@@ -428,25 +461,26 @@
                 plotted.append(event)
 
             if color_by is not None:
                 ray_color = sm.cmap(norm(df.loc[event].loc[sta][color_by]))
 
             # Connect source and receiver with a line
             plt.plot([elon, slon], [elat, slat], color=ray_color, linestyle="-",
-                     alpha=0.1, zorder=50, linewidth=ray_linewidth)
+                     alpha=0.05, zorder=50, linewidth=ray_linewidth)
 
         plt.xlabel("Longitude")
         plt.ylabel("Latitude")
         plt.title(f"{len(df)} raypaths")
         # plt.title(f"{len(df)} raypaths ({len(events)} events, "
         #           f"{len(stations)} stations)")
 
         # Calculate aspect ratio based on latitude
         w = 1 / np.cos(np.radians(elat))
         plt.gca().set_aspect(w)
+        default_axes(ax, **kwargs)
 
         if save:
             plt.savefig(save)
         if show:
             plt.show()
 
         return f, ax
@@ -470,25 +504,37 @@
         :type bin_spacing_km: float
         :param bin_spacing_km: the bin size in km of the 2d histogram. If
             the same as 'point_spacing_km' then you'll probably just see the
             lines. Should be larger than 'point_spacing_km' for a more
             contour plot looking feel.
         """
         figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
         event_color = kwargs.get("event_color", "orange")
         station_color = kwargs.get("station_color", "cyan")
         markersize = kwargs.get("markersize", 26)
 
-        iteration, step_count = self._parse_nonetype_eval(iteration, step_count)
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
-        f, ax = plt.subplots(figsize=figsize)
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         df = self.misfit(level="station").loc[iteration, step_count]
+        # Rearranging the index so that the separate multi indices of 'network'
+        # and 'station' are combined to become 'network'.'station'
+        df.index = [df.index.get_level_values(0),
+                    df.index.map('{0[1]}.{0[2]}'.format)]
 
         # Get lat/lon information from sources and receivers
-        stations = self.receivers.droplevel(0)  # remove network index
+        stations = self.receivers
+
+        # Get lat/lon information from sources and receivers
+        netstas = self.netsta.to_numpy()
+        netstas = [f"{net}.{sta}" for net, sta in netstas]
+
+        # Drop duplicate station names, assuming that they will have the same
+        # coordinates. This is to deal with e.g., TA -> AK networks
         events = self.sources.drop(["time", "magnitude", "depth_km"], axis=1)
 
         # Determine grid bounds and required number of bins for histograms
         x_min = min(stations.longitude.min(), events.longitude.min())
         x_max = max(stations.longitude.max(), events.longitude.max())
         y_min = min(stations.latitude.min(), events.latitude.min())
         y_max = max(stations.latitude.max(), events.latitude.max())
@@ -501,17 +547,20 @@
         # Convert station names and event ids into coordinates
         dx = point_spacing_km / 111.11  # grid spacing in degrees
 
         # Initiate empty arrays to be filled
         x = np.array([])
         y = np.array([])
         plotted = []
-        for event, sta in df.index.to_numpy():
+        for event, netsta in df.index.to_numpy():
             elon, elat = events.loc[event].longitude, events.loc[event].latitude
-            slon, slat = stations.loc[sta].longitude, stations.loc[sta].latitude
+
+            net, sta = netsta.split(".")
+            slon = stations.loc[net].loc[sta].longitude
+            slat = stations.loc[net].loc[sta].latitude
 
             # Plot a marker for each event and station
             if event not in plotted:
                 plt.scatter(elon, elat, marker="o", c=event_color,
                             edgecolors="k", s=markersize, zorder=100)
                 plotted.append(event)
             if sta not in plotted:
@@ -529,15 +578,15 @@
 
             x = np.concatenate((x, x_))
             y = np.concatenate((y, y_))
 
         # Create the 2D histogram of raypath density
         plt.hist2d(x, y, bins=(x_bins, y_bins), cmap=plt.get_cmap(cmap), 
                    zorder=5)
-        cbar = plt.colorbar(label="counts", shrink=0.9, pad=0.025)
+        cbar = plt.colorbar(label="counts", shrink=0.75, pad=0.025)
 
         plt.title(f"Raypath Density {iteration}{step_count} "
                   f"(N={len(df)} src-rcv pairs)")
         plt.xlabel("Longitude")
         plt.ylabel("Latitude")
 
         # Calculate aspect ratio based on latitude
@@ -549,23 +598,29 @@
         if save:
             plt.savefig(save)
         if show:
             plt.show()
 
         plt.close()
 
-    def event_hist(self, choice, show=True, save=None):
+    def event_hist(self, choice, show=True, save=None, **kwargs):
         """
-        Make a histogram of event information
-        :return:
+        Make a histogram of event information for a given parameter `choice`.
+
+        :type choice: str
+        :param choice: event parameter choice. For available choice see the keys
+            of the Inspector `sources` dataframe
         """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
         assert choice in self.sources.keys(), \
             f"Choice must be in {self.sources.keys()}"
 
-        f, ax = plt.subplots()
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         arr = self.sources[choice].to_numpy()
 
         # Compare iterations, plot original iteration on top
         n, bins, patches = plt.hist(x=arr, color="w", histtype="bar",
                                     bins=list(np.arange(4.5, 6.1, .1)),
                                     edgecolor="black", linewidth=2.,
                                     label=choice, alpha=1., zorder=20
@@ -580,17 +635,66 @@
             plt.savefig(save)
         if show:
             plt.show()
 
         plt.close()
 
         return f, ax
+    
+    def events_over_inversion(self, choice="misfit", normalize=True, 
+                              show=True, save=None,  **kwargs):
+        """
+        Line plot where the X axis represents iterations in the inversion and
+        the Y axis represents event misfit or window number. Each line 
+        represents a different event.
+
+        :type choice: str
+        :param choice: choice of plot value, either 'misfit' or 'nwin' or 
+            'unscaled_misfit'
+        """
+        # Get the iteration and step counts of evals which contribute models
+        evals = self.good_models[["iteration", "step_count"]].values.tolist()
+        misfit = self.misfit(level="event")
+
+        plot_dict = {}
+        for event in self.events:
+            plot_dict[event] = []
+            for eval_ in evals:
+                iter_, step = eval_
+                val = misfit.loc[iter_, step, event][choice]
+                plot_dict[event].append(val)
+            if normalize:
+                plot_dict[event] /= max(plot_dict[event])
+
+        f, ax = plt.subplots()
+        for i, (event, vals) in enumerate(plot_dict.items()):
+            linestyle = ["-", "--", ":", "-."][i % 9 % 3]
+            plt.plot(vals, ls=linestyle, marker=".", markerfacecolor="None", 
+                     markeredgecolor="k", markeredgewidth=0.5, c=f"C{i}", 
+                     label=event)
+
+        plt.xlabel("Model Number")
+        if normalize:
+            ylabel = "Normalized " + common_labels[choice]
+        else:
+            ylabel = common_labels[choice]
+        plt.ylabel(ylabel)
+        plt.yscale("log")
+        plt.title(f"Event {common_labels[choice]} over Inversion "
+                  f"(N={len(self.events)})")
+        plt.legend()
+        default_axes(ax)
+        
+        if save:
+            plt.savefig(save)
+        if show:
+            plt.show()
 
     def measurement_hist(self, iteration=None, step_count=None, choice="event",
-                         show=True, save=False):
+                         show=True, save=False, **kwargs):
         """
         Make histograms of measurements for stations or events to show the 
         distribution of measurements. 
 
         :type iteration: str
         :param iteration: iteration number e.g. 'i00'
         :type step_count: str
@@ -598,15 +702,19 @@
         :type choice: str
         :param choice: choice of making hist by 'event' or 'station'
         :type show: bool
         :param show: Show the plot
         :type save: str
         :param save: fid to save the given figure
         """
-        iteration, step_count = self._parse_nonetype_eval(iteration, step_count)
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
 
         arr = self.nwin(
             level=choice).loc[iteration, step_count].nwin.to_numpy()
 
         n, bins, patches = plt.hist(x=arr, color="orange", histtype="bar",
                                     edgecolor="black", linewidth=4.,
                                     label=choice, alpha=1., zorder=20
@@ -617,68 +725,84 @@
         plt.axvline(x=mu, ymin=0, ymax=1, linewidth=2, c="k",
                     linestyle="--", zorder=15, alpha=0.5)
         for sign in [-1, 1]:
             plt.axvline(x=mu + sign * std, ymin=0, ymax=1, linewidth=2,
                         c="k", linestyle=":", zorder=15, alpha=0.5)
 
         default_axes(plt.gca())
-        plt.xlabel(f"{choice} number of measurements")
+        plt.xlabel(f"number of measurements per {choice}")
         plt.ylabel("count")
         plt.title(f"{iteration}{step_count}; N={len(arr)}\n"
                   f"solid line = mean; dashed line = 1 std")
 
         if save:
             plt.savefig(save)
         if show:
             plt.show()
         else:
             plt.close()
 
-    def station_event_misfit_map(self, station, iteration, step_count, choice,
-                                 show=True, save=False, **kwargs):
+    def station_event_misfit_map(self, station, iteration=None, step_count=None,
+                                 choice="misfit", cmap="viridis", show=True,
+                                 save=False, **kwargs):
         """
         Plot a single station and all events that it has measurements for.
         Events will be colored by choice of value: misfit or nwin (num windows)
 
         :type station: str
         :param station: specific station to use for map
         :type iteration: str
         :param iteration: iteration number e.g. 'i00'
         :type step_count: str
         :param step_count: step count e.g. 's00'
         :type choice: str
         :param choice: choice of misfit value, either 'misfit' or 'nwin'
+        :type cmap: str
+        :param cmpa: matplotlib colormap to represent misfit choice
         :type show: bool
         :param show: Show the plot
         :type save: str
         :param save: fid to save the given figure
         """
-        assert (station in self.stations), "station name not found"
-        cmap = kwargs.get("cmap", "viridis")
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
 
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
+
+        assert (station in self.stations), f"station not found: {self.stations}"
         sta = self.receivers.droplevel(0).loc[station]
 
         # Get misfit on a per-station basis 
         df = self.misfit(level="station").loc[
             iteration, step_count].swaplevel(0, 1)
         df = df.sort_values(by="station").loc[station]
 
         # Get source lat/lon values as a single dataframe with same index name
         src = self.sources.drop(["time", "magnitude", "depth_km"], axis=1)
         src.index.names = ["event"]
 
         # This is a dataframe of events corresponding to a single station
         df = df.merge(src, on="event")
 
-        f, ax = plt.subplots()
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         src = plt.scatter(sta.longitude, sta.latitude, marker="v", c="orange",
-                          edgecolors="k", s=25, zorder=100)
+                          edgecolors="k", s=40, zorder=100)
+        # Plot each station colored by its respective misfit
         plt.scatter(df.longitude.to_numpy(), df.latitude.to_numpy(),
-                    c=df[choice].to_numpy(), marker="o", s=25, zorder=99,
-                    cmap=cmap)
+                    c=df[choice].to_numpy(), marker="o", s=50, zorder=99,
+                    cmap=cmap, ec="k", linewidth=1.5)
+        # Plot connecting lines for source to receiver with the same color
+        norm = mpl.colors.Normalize(vmin=df[choice].min(),
+                                    vmax=df[choice].max(), clip=True)
+        mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+        for lon, lat, val in zip(df.longitude.to_numpy(),
+                                 df.latitude.to_numpy(),
+                                 df[choice].to_numpy()):
+            plt.plot([sta.longitude, lon], [sta.latitude, lat], "-", alpha=0.5,
+                      zorder=98, c=mapper.to_rgba(val), lw=1.5)
 
         plt.xlabel("Longitude")
         plt.ylabel("Latitude")
         plt.title(f"{station} {iteration}{step_count}; {len(df)} events")
 
         _, _, cbar = colormap_colorbar(cmap, vmin=df[choice].to_numpy().min(),
                                        vmax=df[choice].to_numpy().max(), 
@@ -690,16 +814,17 @@
             plt.savefig(save)
         if show:
             hover_on_plot(f, ax, src, df.index.to_numpy())
             plt.show()
 
         return f, ax
 
-    def event_station_misfit_map(self, event, iteration, step_count, choice,
-                                 show=True, save=False, **kwargs):
+    def event_station_misfit_map(self, event, iteration=None, step_count=None,
+                                 choice="misfit", cmap="viridis", vmin=None,
+                                 vmax=None, show=True, save=False, **kwargs):
         """
         Plot a single event and all stations with measurements. Stations are
         colored by choice of value: misfit or nwin (number of windows)
 
         :type event: str
         :param event: specific event to use for map
         :type iteration: str
@@ -709,40 +834,53 @@
         :type choice: str
         :param choice: choice of misfit value, either 'misfit' or 'nwin'
         :type show: bool
         :param show: Show the plot
         :type save: str
         :param save: fid to save the given figure
         """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
         assert (event in self.sources.index), "event name not found"
-        cmap = kwargs.get("cmap", "viridis")
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
-        f, ax = plt.subplots()
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         source = self.sources.loc[event]
         src = plt.scatter(source.longitude, source.latitude, marker="o", c="r",
                           edgecolors="k", s=20, zorder=100)
 
         # Go through each of the stations corresponding to this source
         df = self.misfit(level="station").loc[iteration, step_count, event]
         assert (choice in df.columns), f"choice must be in {df.columns}"
 
         # Get lat lon values for receivers
         df = df.merge(self.receivers, on="station")
         misfit_values = df[choice].to_numpy()
         rcvs = plt.scatter(df.longitude.to_numpy(), df.latitude.to_numpy(),
-                           c=misfit_values, marker="v", s=15, zorder=100,
-                           cmap=cmap
+                           c=misfit_values, marker="v", s=50, zorder=100,
+                           cmap=cmap, ec="k", lw=1.5, vmin=vmin, vmax=vmax
                            )
 
+        # Plot connecting lines for source to receiver with the same color
+        norm = mpl.colors.Normalize(vmin=vmin or df[choice].min(),
+                                    vmax=vmax or df[choice].max(), clip=True)
+        mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+        for lon, lat, val in zip(df.longitude.to_numpy(),
+                                 df.latitude.to_numpy(),
+                                 df[choice].to_numpy()):
+            plt.plot([source.longitude, lon], [source.latitude, lat], "-",
+                     alpha=0.5, zorder=98, c=mapper.to_rgba(val), lw=1.5)
+
         plt.xlabel("Longitude")
         plt.ylabel("Latitude")
         plt.title(f"{event} {iteration}{step_count}; {len(df)} stations")
 
-        _, _, cbar = colormap_colorbar(cmap, vmin=misfit_values.min(),
-                                       vmax=misfit_values.max(), 
+        _, _, cbar = colormap_colorbar(cmap, vmin=vmin or misfit_values.min(),
+                                       vmax=vmax or misfit_values.max(),
                                        cbar_label=choice,)
 
         default_axes(ax, cbar, **kwargs)
 
         if save:
             plt.savefig(save)
         if show:
@@ -764,25 +902,25 @@
         :param choice: choice of misfit value, either 'misfit' or 'nwin' or
             'unscaled_misfit'
         :type show: bool
         :param show: Show the plot
         :type save: str
         :param save: fid to save the given figure
         """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
         cmap = kwargs.get("cmap", "viridis")
         markersize = kwargs.get("markersize", 20)
         marker = kwargs.get("marker", "o")
 
-        if iteration is None:
-            iteration, step_count = self.final_model
-
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
         if choice is None:
             choice = "misfit"
 
-        f, ax = plt.subplots()
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         sources = self.sources.drop(["time", "magnitude", "depth_km"], axis=1)
         # Rename from event_id to event to match the naming of the dataframe
         sources.rename_axis("event", inplace=True)
         df = self.misfit(level="event").loc[iteration, step_count]
         df = df.merge(sources, on="event")
 
         srcs = plt.scatter(df.longitude.to_numpy(), df.latitude.to_numpy(),
@@ -803,127 +941,313 @@
             plt.savefig(save)
         if show:
             hover_on_plot(f, ax, srcs, df.index.to_numpy())
             plt.show()
 
         return f, ax
 
-    def hist(self, iteration=None, step_count=None, iteration_comp=None,
-             step_count_comp=None, f=None, ax=None, event=None, station=None,
-             choice="cc_shift_in_seconds", binsize=None, show=True, save=None,
-             **kwargs):
+    def event_comparison(self, iteration=None, step_count=None, choice="misfit",
+                          show=True, save=None, **kwargs):
+        """
+        Create a scatterplot where the X axis is the event index and the Y axis
+        is a summary statistic for that event, either misfit or window number or
+        lengths. Useful for a quick-glance view of how events compare to one
+        another to determine if outlier events are under or overperforming the
+        average.
+
+        :type iteration: str
+        :param iteration: iteration to choose for misfit
+        :type step_count: str
+        :param step_count: step count to query, e.g. 's00'
+        :type choice: str
+        :param choice: choice of misfit value, either 'misfit' or 'nwin' or
+            'unscaled_misfit'
+        """
+        figsize = kwargs.get("figsize", (8, 4))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+        cmap = kwargs.get("cmap", "plasma")
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
+
+        if choice == "misfit":
+            other_choice = "nwin"
+        elif choice == "nwin":
+            other_choice = "misfit"
+
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
+        # Assuming that the values are ordered by event-name alphabetical
+        arr = self.misfit(
+            level="event")[choice][iteration][step_count].to_numpy()
+        # Color the markers by the other choice that wasn't selected
+        carr = self.misfit(
+            level="event")[other_choice][iteration][step_count].to_numpy()
+
+        sc = plt.scatter(range(0, len(arr)), arr, c=carr, marker="o",
+                         ec="k", lw=1.5, zorder=99, cmap=cmap)
+        # Colorbar to show the 'other choice'
+        cbar = plt.colorbar(label=other_choice, shrink=0.9, pad=0.025)
+        # Plot statistics (mean and 1 std. deviation)
+        mean = np.mean(arr)
+        std = np.std(arr)
+        plt.axhline(mean, c="k", ls="-", lw=2, zorder=95)
+        plt.text(x=0, y=mean, s=f"mean={mean:.2f}", fontsize=12, zorder=96)
+        for sign in [1, -1]:
+            plt.axhline(mean + sign * std, c="k", ls='--', lw=1.75, zorder=95)
+        plt.text(x=0, y=mean + std, s=f"std={std:.2f}", fontsize=12, zorder=96)
+
+        # Plot accoutrements
+        plt.xticks(np.arange(0, len(arr), 1))
+        plt.xlim([-0.5, len(arr)-0.5])
+        plt.xlabel("Event Index")
+        plt.ylabel(choice)
+        plt.title(f"Event Comparison {iteration}{step_count} "
+                  f"(N_events={len(arr)})")
+        plt.grid(which="both", axis="both")
+        default_axes(ax, cbar=cbar, **kwargs)
+
+        if save:
+            plt.savefig(save)
+        if show:
+            # Get index names assuming indices go iter, step, name
+            names = self.misfit(
+                level="event")["misfit"].index.get_level_values(2)
+            hover_on_plot(f, ax, sc, names)
+            plt.show()
+
+    def event_station_hist2d(self, iteration=None, step_count=None,
+                             choice="misfit", minval=None, maxval=None,
+                             show=True, save=None, **kwargs):
+        """
+        2D histogram of misfit or window number where one axis represents
+        event indices, and the other axis represents station indices. That way
+        a User can get an overview of all event-station pairs in one figure
+        where colors will help distinguish good or bad event-station pairs,
+        and entire rows and columns will help show if an event or station has
+        missing data or entires.
+
+        The figure is generated assuming that there are more receivers than
+        events used, so we are making a long rectangle of a plot
+
+        .. note::
+
+            Takes advantage of some index merging operations that are not
+            easily readable:
+            https://stackoverflow.com/questions/41987743/\
+                merge-two-multiindex-levels-into-one-in-pandas
+        """
+        figsize = kwargs.get("figsize", (16, 10))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+        cmap = kwargs.get("cmap", "viridis")
+        nstd = kwargs.get("nstd", 3)
+        vmax_color = kwargs.get("vmax_color", "red")
+        zero_color = kwargs.get("zero_color", "gray")
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
+
+        f, ax = plt.subplots(figsize=figsize, dpi=dpi)
+
+        # Get a misfit dataframe that contains only event and station as index
+        df = self.misfit(level="station")[choice][iteration][step_count]
+        # Rearranging the index so that the separate multi indices of 'network'
+        # and 'station' are combined to become 'network'.'station'. See note
+        df.index = [df.index.get_level_values(0),
+                    df.index.map('{0[1]}.{0[2]}'.format)]
+        # Initialize empty matrix that we will fill
+        ny = len(self.events)
+        nx = len(self.netsta)
+        data = np.zeros(shape=(ny, nx))
+
+        netstas = self.netsta.to_numpy()
+        netstas = [f"{net}.{sta}" for net, sta in netstas]
+
+        # Use mean and 2std to get bounds of colormap, values that fall outside
+        # will be colored differently to make them stand out more
+        # Values of zero will be set to white
+        mean = df.to_numpy().mean()
+        std = df.to_numpy().std()
+        vmax = mean + nstd * std
+
+        # Loop through all misfit data and assign to matrix location
+        for i, src in enumerate(sorted(self.events)):
+            try:
+                src_df = df[src]
+            except KeyError:
+                continue
+            for j, rcv in enumerate(sorted(netstas)):
+                try:
+                    val = src_df[rcv]
+                except KeyError:
+                    continue
+                data[i, j] = val
+
+        n = len(data[np.where(data!=0)])
+        data[np.where(data==0)] = -999
+        # Create a colormap that highlights over and under values
+        cmap = plt.get_cmap(cmap, 17)
+        cmap.set_under(zero_color)
+        cmap.set_over(vmax_color)
+
+        ims = plt.imshow(data, cmap=cmap, vmin=0, vmax=vmax)
+        cbar = plt.colorbar(label=choice, shrink=0.25, pad=0.025,
+                            extend="both")
+
+        # Grid out every data point
+        ax.set_xticks(np.arange(0, nx, 5), minor=False)
+        ax.set_yticks(np.arange(0, ny, 5), minor=False)
+        ax.set_xticks(np.arange(0.5, nx, 1), minor=True)
+        ax.set_yticks(np.arange(0.5, ny, 1), minor=True)
+        plt.xticks(rotation=90)
+        plt.grid(c="k", alpha=0.5, which="minor")
+
+        # Labels and such
+        plt.xlim([-0.5, nx-0.5])
+        plt.ylim([-0.5, ny-0.5])
+        plt.xlabel("Receiver Index")
+        plt.ylabel("Event Index")
+        plt.title(f"N={n}; mean={mean:.2f}; std={std:.2f}; vmax={nstd}*std")
+        ax.set_aspect("equal")
+
+        default_axes(ax, tick_length=0, cbar=cbar)
+
+        if save:
+            plt.savefig(save)
+        if show:
+            plt.show()
+
+    def hist(self, iteration=None, step_count=None, iteration_comp=None, 
+             step_count_comp=None, compare=True, f=None, ax=None,
+             event=None, station=None, choice="cc_shift_in_seconds",
+             binsize=None, show=True, save=None, **kwargs):
         """
         Create a histogram of misfit information for either time shift or
         amplitude differences. Option to compare against different iterations,
         and to look at different choices.
 
         Choices are any column value in the Inspector.windows attribute
 
+        :type choice: str
+        :param choice: any choice from the keys of Inspector.windows, typical
+            choices are 'cc_shift_in_seconds', 'dlnA', 'max_cc_value', 'misfit',
+            OR to plot the number of windows per event or station, use 'nwin' or
+            'nwin_sta' respectively
         :type iteration: str
         :param iteration: iteration to choose for misfit
         :type step_count: str
         :param step_count: step count to query, e.g. 's00'
+        :type compare: bool
+        :param compare: compare two superimposed histograms from different
+            evaluations. will use parameters `iteration_comp` and
+            `step_count_comp` to choose the second histogram, which default to
+            the final model. If False, only plot one histogram, defined by
+            `iteration` and `step_count`
         :type iteration_comp: str
         :param iteration_comp: iteration to compare with, will be plotted in
             front of `iteration`
         :type step_count_comp: str
         :param step_count_comp: step to compare with
         :type f: matplotlib.figure
         :param f: plot to an existing figure
         :type ax: matplotlib.axes._subplots.AxesSubplot
         :param ax: plot to an existing axis e.g. to string together histograms
         :type event: str
         :param event: filter for measurements for a given event
         :type station: str
         :param station: filter for measurements for a given station
-        :type choice: str
-        :param choice: choice of 'cc_shift_s' for time shift, or 'dlnA' as
-            amplitude
         :type binsize: float
         :param binsize: size of the histogram bins
         :type show: bool
         :param show: show the plot
         :type save: str
         :param save: fid to save the figure
         """
         # Optional kwargs for fine tuning figure parameters
+        figsize = kwargs.get("figsize", (8, 6))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
         title = kwargs.get("title", "")
         xlim = kwargs.get("xlim", None)
         color = kwargs.get("color", "darkorange")
         color_comp = kwargs.get("color_comp", "deepskyblue")
         fontsize = kwargs.get("fontsize", 12)
-        figsize = kwargs.get("figsize", (8, 6))
         legend = kwargs.get("legend", True)
         legend_loc = kwargs.get("legend_loc", "best")
         label_range = kwargs.get("label_range", False)
         xstep = kwargs.get("xstep", 2)
         ymax = kwargs.get("ymax", None)
         xlabel = kwargs.get("xlabel", None)
         zeroline = kwargs.get("zeroline", False)
         meanline = kwargs.get("meanline", False)
         stdline = kwargs.get("stdline", False)
         linewidth = kwargs.get("linewidth", 2.5)
         label = kwargs.get("label", None)
         label_comp = kwargs.get("label_comp", None)
 
-        # If no arguments are given, default to first and last evaluations
-        if iteration is None and iteration_comp is None:
-            iteration, step_count = self.initial_model
-            iteration_comp, step_count_comp = self.final_model
-
-        # Check that the provided values are available in the Inspector
-        assert iteration in self.iterations, \
-            f"iteration must be in {self.iterations}"
-        if step_count is None:
-            assert step_count in self.steps.loc[iteration], \
-                f"step must be in {self.steps.loc[iteration]}"
-        if iteration_comp is not None:
-            assert iteration_comp in self.iterations, \
-                f"iteration_comp must be in {self.iterations}"
-            assert step_count_comp in self.steps.loc[iteration_comp], \
-                f"step_comp must be in {self.steps.loc[iteration_comp]}"
+        # Get iteration and step count if User did not specify
+        iteration, step_count = self.validate_evaluation(iteration, step_count,
+                                                         choice="initial")
 
-        # Try to set a default binsize that may or may not work 
+        iteration_comp, step_count_comp = self.validate_evaluation(
+            iteration_comp, step_count_comp, choice="final")
+
+        # Try to set a default binsize that may or may not work
         if binsize is None:
             try:
                 binsize = {"cc_shift_in_seconds": 1,
-                           "dlnA": 0.25,
+                           "dlnA": 0.1,
                            "max_cc_value": 0.05,
-                           "misfit": 10,
-                           "relative_starttime": 15,
-                           "relative_endtime": 15}[choice]
+                           "misfit": 1,
+                           "relative_starttime": 50,
+                           "relative_endtime": 50,
+                           "length_s": 50,
+                           "max_cc_value": 0.1,
+                           "nwin": 50,
+                           "nwin_sta": 10,
+                           }[choice]
             except KeyError:
                 binsize = 1
 
+        # Helper function to get the values and limits of the histogram
         def get_values(m, s, e, sta):
-            """short hand to get the data, and the maximum value in DataFrame"""
-            df_a = self.isolate(iteration=m, step_count=s, event=e, station=sta)
-            try:
-                val_ = df_a.loc[:, choice].to_numpy()
-            except KeyError as e:
-                raise KeyError(f"Inspector.windows has no key {choice}") from e
-            lim_ = max(abs(np.floor(min(val_))), abs(np.ceil(max(val_))))
+            """
+            Short hand to get the data, and the maximum value in DataFrame
+            m: iteration; s: step_count; e: event; sta: station
+            """
+            if "nwin" in choice:
+                assert(m is not None and s is not None), \
+                    "choice `nwin` cannot be used with event or station select"
+                if choice == "nwin":
+                    df_a = self.nwin(level="event").loc[m, s].nwin
+                elif choice == "nwin_sta":
+                    df_a = self.nwin(level="station").loc[m, s].nwin
+                val_ = df_a.to_numpy()
+                lim_ = max(abs(np.floor(min(val_))), abs(np.ceil(max(val_))))
+            # Normal keys in windows, get the values and limits
+            else:
+                df_a = self.isolate(iteration=m, step_count=s, 
+                                    event=e, station=sta)
+                try:
+                    val_ = df_a.loc[:, choice].to_numpy()
+                except KeyError as e:
+                    raise KeyError(f"Inspector has no key {choice}") from e
+                lim_ = max(abs(np.floor(min(val_))), abs(np.ceil(max(val_))))
             return val_, lim_
 
         # Instantiate the plot objects and 'goforyourlifemate'
         if f is None:
-            f, ax = plt.subplots(figsize=figsize)
+            f, ax = plt.subplots(figsize=figsize, dpi=dpi)
         if ax is None:
             ax = plt.gca()
 
         val, lim = get_values(iteration, step_count, event, station)
 
-        if iteration_comp:
+        if compare:
             val_comp, lim_comp = get_values(iteration_comp, step_count_comp,
                                             event, station)
 
             # Reset the limit to be the greater of the two
             lim = max(lim, lim_comp)
 
-            # Compare iterations, plot original iteration on top 
+            # Compare iterations, plot original iteration on top
             n, bins, patches = plt.hist(
                 x=val, bins=np.arange(-1 * lim, lim + .1, binsize),
                 color=color, histtype="bar", edgecolor="black",
                 linewidth=linewidth,
                 label=(label or f"{iteration}{step_count}") + f"; N={len(val)}",
                 zorder=11, alpha=1.
             )
@@ -987,15 +1311,15 @@
         if ymax:
             plt.ylim([0, ymax])
 
         # Stats in the title by default
         if not title:
             tit_fmt = "mean: {mean:.2f} / std: {std:.2f} / med: {med:.2f}"
             title = tit_fmt.format(mean=mean, std=std, med=med)
-            if iteration_comp:
+            if compare:
                 tit_comp = tit_fmt.format(mean=mean_comp, std=std_comp,
                                           med=med_comp)
                 title = " ".join([f"[{label or iteration}]", title, "\n",
                                   f"[{label_comp or iteration_comp}]", tit_comp
                                   ])
 
         # Finalize plot details
@@ -1008,39 +1332,79 @@
             except KeyError:
                 xlab_ = choice
 
         plt.xlabel(xlab_, fontsize=fontsize)
         plt.ylabel("Count", fontsize=fontsize)
         plt.title(title)
         if label_range:
-            plt.xticks(np.arange(-1 * label_range, label_range + .1, 
+            plt.xticks(np.arange(-1 * label_range, label_range + .1,
                                  step=xstep))
 
         if legend:
             leg = plt.legend(fontsize=fontsize / 1.25, loc=legend_loc)
             # Thin border around legend objects, unnecessarily thick bois
             for leg_ in leg.legendHandles:
                 leg_.set_linewidth(1.5)
 
         default_axes(ax, **kwargs)
 
-        plt.tight_layout()
-
         if save:
             plt.savefig(save)
         if show:
             plt.show()
 
         return f, ax
 
-    def plot_windows(self, iteration=None, step_count=None, iteration_comp=None,
+    def histogram_summary(self, iteration=None, step_count=None,
+                          iteration_comp=None, step_count_comp=None,
+                          show=True, save=False, **kwargs):
+        """
+        Generate a multi-panel figure of different histrograms that represent
+        a few key measurements that is useful for understanding the statistical
+        misfit characteristics
+        """
+        figsize = kwargs.get("figsize", (8, 8))
+        dpi = kwargs.get("dpi", DEFAULT_DPI)
+
+        choices = [
+            ["cc_shift_in_seconds", "dlnA", "max_cc_value"],
+            [ "relative_starttime", "relative_endtime", "length_s"],
+            ["nwin", "nwin_sta", "misfit"]
+        ]
+        nrows = len(choices)
+        ncols = max([len(_) for _ in choices])
+
+        f = plt.figure(figsize=figsize, dpi=dpi)
+        gs = mpl.gridspec.GridSpec(nrows, ncols, wspace=0.5, hspace=0.5)
+
+        for row in range(0, nrows):
+            for col in range(0, ncols):
+                ax = plt.subplot(gs[row, col])
+                self.hist(choice=choices[row][col], iteration=iteration,
+                          step_count=step_count, iteration_comp=iteration_comp, 
+                          compare=True,
+                          step_count_comp=step_count_comp, f=f, ax=ax,
+                          show=False, figsize=(figsize[0] / nrows,
+                                               figsize[1] / ncols),
+                          fontsize=8, title_fontsize=8, label_fontsize=8, 
+                          tick_fontsize=8,
+                          **kwargs
+                          )
+
+        if save:
+            plt.savefig(save)
+        if show:
+            plt.show()
+
+    def window_stack(self, iteration=None, step_count=None, iteration_comp=None,
                      step_count_comp=None, choice="cc_shift_in_seconds",
                      event=None, network=None, station=None, component=None,
-                     no_overlap=True, distances=False, annotate=False,
-                     bounds=False, show=True, save=False, **kwargs):
+                     no_overlap=True, abs_distances=False, annotate=False,
+                     bounds=False, show=True, save=False,
+                     **kwargs):
         """
         Show lengths of windows chosen based on source-receiver distance, akin
         to Tape's Thesis or to the LASIF plots. These are useful for showing
         which phases are chosen, and window choosing behavior as distance
         increases and (probably) misfit increases.
 
         :type iteration: str
@@ -1067,19 +1431,19 @@
         :type no_overlap: bool
         :param no_overlap: If real distances are used, many src-rcv pairs are
             at the same or very similar distances, leading to overlapping
             rectangles. If this is set to True, to minimize overlap, the
             function will try to shift the distance to a value that hasn't yet
             been plotted. It will alternate larger positive and negative values
             until something is found. Will lead to non-real distances.
-        :type distances: bool
-        :param distances: If set False, just plot one window atop the other,
-            which makes for more concise, easier to view plots, but
+        :type abs_distances: bool
+        :param abs_distances: If set False (default), just plot one window atop
+            the other, which makes for more concise, easier to view plots, but
             then real distance information is lost, only relative distance
-            kept.
+            kept. If True, the y-axis corresponds to actual source rec. distance
         :type annotate: bool
         :param annotate: If True, will annotate event and station information
             for each window. May get messy if `distances == True` and
             `no_overlap == False` because you will get many overlapping
             annotations. Works ideally if `distances == False`.
         :type bounds: bool or list of float
         :param bounds:
@@ -1101,26 +1465,26 @@
                 The label for the colorbar
             float rectangle_height:
                 The vertical size of the rectangles, defaults to 1.
             float anno_shift:
                 The distance in seconds to shift the plot to accomodate
                 annotations. This needs to be played as its based on the length
                 of the strings that are used in the annotations.
+            str facecolor:
+                Set the background color of the figure. Defaults to 'w'hite but
+                some colorscales may be more vibrant with darker color faces
         """
-        alpha = kwargs.get("alpha", 0.6)
+        alpha = kwargs.get("alpha", 1)
         cmap = kwargs.get("cmap", "viridis")
         cbar_label = kwargs.get("cbar_label", None)
         rectangle_height = kwargs.get("rectangle_height", 1.0)
         anno_shift = kwargs.get("anno_shift", 50)
+        facecolor = kwargs.get("facecolor", "w")
 
-        iteration, step_count = self._parse_nonetype_eval(iteration, step_count)
-
-        assert(iteration in self.iterations and
-               step_count in self.steps[iteration]), \
-            f"{iteration}{step_count} does not exist in Inspector"
+        iteration, step_count = self.validate_evaluation(iteration, step_count)
 
         assert(choice in self.windows.keys()), (f"Color by choice {choice} not "
                                                 f"in list of available keys")
 
         # Filter out the specific windows that we're interested in
         df = self.isolate(iteration=iteration, step_count=step_count,
                           event=event, network=network, station=station,
@@ -1163,14 +1527,15 @@
                     ].sort_values(by="distance_km")
         if df.empty:
             logger.warning("Filtered dataframe is empty, no windows to plot")
             return
 
         # Plotting begins here
         f, ax = plt.subplots(figsize=(8, 6))
+        ax.set_facecolor(facecolor)
 
         # Create a custom color scale based on the min and max values of choice
         if cbar_label is None:
             try:
                 # For cleaner formatting of colorbar label
                 cbar_label = common_labels[choice]
             except KeyError:
@@ -1198,46 +1563,29 @@
             xmin -= anno_shift
         xmax = df.relative_endtime.max()
 
         dist_values, y_value = [], 0  # keep track of what y-values are used
         for window in df.to_numpy():
             ev, sta, comp, start, end, dist, value = window
 
-            if not distances:
+            if not abs_distances:
                 # Ignore distances and simply plot linearly
                 dist_ = y_value
                 y_value += rectangle_height
             else:
-                # Try not to overlap windows that are very close in distance
-                dist_ = int(dist)
-                if no_overlap:
-                    if dist_ in dist_values:
-                        shift, sign = 1, -1
-                        while dist_ in dist_values:
-                            dist_ += shift
-                            # Alternate shift so that we search
-                            # 1, -1, 2, -2, 3, -3, etc...
-                            shift = sign * (abs(shift) + rectangle_height)
-                            sign *= -1
-                        dist_values.append(dist_)
-                        logger.warning(f"Shifted {ev} {sta}: {dist - dist_}km")
-                    else:
-                        dist_values.append(dist_)
+                dist_ = dist
 
             # Plot the windows as rectangles to sort of match waveform plots
             ax.add_patch(Rectangle(xy=(start, dist_ - rectangle_height / 2),
-                                   width=end - start, ec="k", alpha=alpha,
+                                   width=end - start, alpha=alpha,
                                    height=rectangle_height, 
                                    fc=sm.cmap(norm(value)),
                                    zorder=12)
                          )
-            # Black background line for frame of reference / gridding
-            ax.hlines(y=dist_, xmin=xmin, xmax=xmax, colors="k",
-                      alpha=0.3, linewidth=0.3, zorder=10
-                      )
+
             # Annotate event, station, component, distance and value for
             # easier identification. Can be messy with a lot of windows
             if annotate:
                 plt.text(xmin, dist_,
                          f"{ev} {sta} {comp} {dist:.2f}km {value:.2f}",
                          fontsize=4.5, zorder=11)
 
@@ -1246,23 +1594,26 @@
                   f"[{iteration}{step_count}] "
                   f"[{iteration_comp}{step_count_comp}]\n"
                   f"Event: {event} / Station: {station} / Network: {network} / "
                   f"Component: {component}")
         plt.xlabel("Time [s]")
         plt.xlim([xmin, xmax])
 
-        if distances:
+        if abs_distances:
             plt.ylabel("Distance [km]")
             plt.ylim([df.distance_km.min() - 10, df.distance_km.max() + 10])
         else:
             # Relative distances means the y-axis values are useless
             plt.ylabel("Relative Distance")
             plt.ylim([-rectangle_height, dist_ + rectangle_height])
             ax.yaxis.set_ticks([])
 
+        default_axes(ax, **kwargs)
+        ax.grid(which="major", axis="x")
+
         if save:
             plt.savefig(save)
         if show:
             plt.show()
         else:
             plt.close()
 
@@ -1547,36 +1898,53 @@
             plt.savefig(save)
         if show:
             plt.show()
 
         return f, ax
 
 
-def default_axes(ax, cbar=None, **kwargs):
+def default_axes(ax, cbar=None, tick_fontsize=10, tick_linewidth=1.5,
+                 tick_length=5, tick_direction="in", label_fontsize=12,
+                 axis_linewidth=2, title_fontsize=14, cbar_tick_fontsize=10,
+                 cbar_label_fontsize=12, cbar_outline_color="k",
+                 cbar_linewidth=2., **kwargs):
     """
     Ensure that all plots have the same default look. Should be more flexible
     than setting rcParams or having a style sheet. Also allows the same kwargs 
     to be thrown by all functions so that the function calls have the same 
     format.
 
-    Keyword Arguments
-    ::
+    :type ax: matplotlib.axes.Axes
+    :param ax: Axes object that should be modified
+    :type cbar: matplotlib.cbar
+    :param cbar: if the figure has a colorbar, also provide a default look
+    :type tick_fontsize: float
+    :param tick_fontsize: fontsize for the tick labels on the X and Y axes
+    :type tick_linewidth: float
+    :param tick_linewidth: thickness of the tick marks on your axis
+    :type tick_length: float
+    :param tick_length: how far the ticks extend from the axis line
+    :type tick_direction: str
+    :param tick_direction: which way the ticks face, 'in' or 'out' from the axis
+        line
+    :type label_fontsize: float
+    :param label_fontsize: how big the labels for the X and Y axis are
+    :type axis_linewidth: float
+    :param axis_linewidth: thickness of the spines of the axis bounding your fig
+    :type title_fontsize: float
+    :param title_fontsize: fontsize for the title object
+    :type cbar_tick_fontsize: if `cbar` is given, the fontsize of the tick
+        labels accompanying the cbar
+    :type cbar_label_fontsize: float
+    :param cbar_label_fontsize: font size for the single label of the cbar
+    type cbar_outline_color: str
+    :param cbar_outline_color: color of the outline bounding box for the cbar
+    :type cbar_linewidth: float
+    :param cbar_linewidth: thickness of the bounding box on the cbar
     """
-    tick_fontsize = kwargs.get("tick_fontsize", 10)
-    tick_linewidth = kwargs.get("tick_linewidth", 1.5)
-    tick_length = kwargs.get("tick_length", 5)
-    tick_direction = kwargs.get("tick_direction", "in")
-    label_fontsize = kwargs.get("label_fontsize", 12)
-    axis_linewidth = kwargs.get("axis_linewidth", 2.)
-    title_fontsize = kwargs.get("title_fontsize", 14)
-    cbar_tick_fontsize = kwargs.get("cbar_tick_fontsize", 10)
-    cbar_label_fontsize = kwargs.get("cbar_label_fontsize", 12)
-    cbar_outline_color = kwargs.get("cbar_outline_color", "k")
-    cbar_linewidth = kwargs.get("cbar_linewdith", 2.)
-
     # Re-set font sizes for labels already created
     ax.title.set_fontsize(title_fontsize)
     ax.xaxis.label.set_fontsize(label_fontsize)
     ax.yaxis.label.set_fontsize(label_fontsize)
     ax.tick_params(axis="both", which="both", width=tick_linewidth, 
                    direction=tick_direction, labelsize=tick_fontsize, 
                    length=tick_length)
```

### Comparing `pyatoa-0.3.1/pyatoa/visuals/map_maker.py` & `pyatoa-0.4.0/pyatoa/visuals/map_maker.py`

 * *Files identical despite different names*

### Comparing `pyatoa-0.3.1/pyatoa/visuals/wave_maker.py` & `pyatoa-0.4.0/pyatoa/visuals/wave_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,16 @@
         # Determine heights for the annotations, allow alternating heights so 
         # that adjacent windows don't write over one another
         ymin, ymax = ax.get_ylim()
         y_anno = window_anno_height * (ymax - ymin) + ymin
 
         # Default window annotation string
         if window_anno is None:
-            window_anno = "cc={max_cc:.2f} / dT={cc_shift:.2f} / dA={dlnA:.2f}"
+            window_anno = \
+                "cc={max_cc:.2f} / dT={sign}{cc_shift:.2f} / dA={dlnA:.2f}"
 
         for j, window in enumerate(windows):
             tleft = window.left * window.dt + self.time_axis[0]
             tright = window.right * window.dt + self.time_axis[0]
 
             # Misfit windows as rectangle; taken from Pyflex
             ax.add_patch(Rectangle(xy=(tleft, ymin), width=tright - tleft, 
@@ -338,15 +339,16 @@
 
             if plot_window_annos:
                 # Annotate window information into each window
                 t_anno = (tright - tleft) * 0.025 + tleft
                 s_anno = window_anno.format(
                                 i=j+1,
                                 max_cc=window.max_cc_value,
-                                cc_shift=window.cc_shift * window.dt,
+                                sign="+" if window.cc_shift > 0 else "-",
+                                cc_shift=np.abs(window.cc_shift * window.dt),
                                 dlnA=window.dlnA,
                                 left=tleft,
                                 length=tright - tleft)
                 ax.annotate(s_anno, ha=window_anno_ha, va=window_anno_va,
                             xy=(t_anno, y_anno),
                             zorder=12, fontsize=window_anno_fontsize,
                             rotation=window_anno_rotation,
```

### Comparing `pyatoa-0.3.1/pyatoa.egg-info/PKG-INFO` & `pyatoa-0.4.0/pyatoa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatoa
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python's Adjoint Tomography Operations Assistant
 Author: adjTomo Dev Team
 Author-email: adjtomo@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `pyatoa-0.3.1/pyatoa.egg-info/SOURCES.txt` & `pyatoa-0.4.0/pyatoa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,12 +40,11 @@
 pyatoa/utils/write.py
 pyatoa/utils/asdf/__init__.py
 pyatoa/utils/asdf/add.py
 pyatoa/utils/asdf/clean.py
 pyatoa/utils/asdf/load.py
 pyatoa/utils/asdf/write.py
 pyatoa/visuals/__init__.py
-pyatoa/visuals/comp_wave.py
-pyatoa/visuals/improve_wave.py
 pyatoa/visuals/insp_plot.py
 pyatoa/visuals/map_maker.py
-pyatoa/visuals/wave_maker.py
+pyatoa/visuals/wave_maker.py
+pyatoa/visuals/wave_train.py
```

### Comparing `pyatoa-0.3.1/pyproject.toml` & `pyatoa-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyatoa"
-version = "0.3.1"
+version = "0.4.0"
 description = "Python's Adjoint Tomography Operations Assistant"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "adjTomo Dev Team"},
     {email = "adjtomo@gmail.com"}
```

