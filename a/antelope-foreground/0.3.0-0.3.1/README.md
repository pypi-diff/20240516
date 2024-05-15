# Comparing `tmp/antelope_foreground-0.3.0.tar.gz` & `tmp/antelope_foreground-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antelope_foreground-0.3.0.tar", last modified: Thu Mar 21 22:50:52 2024, max compression
+gzip compressed data, was "antelope_foreground-0.3.1.tar", last modified: Wed May 15 23:10:20 2024, max compression
```

## Comparing `antelope_foreground-0.3.0.tar` & `antelope_foreground-0.3.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.122907 antelope_foreground-0.3.0/
--rw-r--r--   0 b          (500) b          (506)      808 2024-03-21 22:50:52.122907 antelope_foreground-0.3.0/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)      245 2021-09-23 01:24:18.000000 antelope_foreground-0.3.0/README.md
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.112907 antelope_foreground-0.3.0/antelope_foreground/
--rw-r--r--   0 b          (500) b          (506)       50 2020-11-05 09:29:01.000000 antelope_foreground-0.3.0/antelope_foreground/__init__.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.112907 antelope_foreground-0.3.0/antelope_foreground/data_sources/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-27 09:04:34.000000 antelope_foreground-0.3.0/antelope_foreground/data_sources/__init__.py
--rw-r--r--   0 b          (500) b          (506)    15880 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/data_sources/calrecycle_lca.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.116240 antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-27 09:05:24.000000 antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8813 2021-08-12 01:39:21.000000 antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/test_calrecycle.py
--rw-r--r--   0 b          (500) b          (506)     3414 2021-08-12 01:39:21.000000 antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/validate_calrecycle.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.116240 antelope_foreground-0.3.0/antelope_foreground/entities/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 22:38:35.000000 antelope_foreground-0.3.0/antelope_foreground/entities/__init__.py
--rw-r--r--   0 b          (500) b          (506)    18893 2023-08-22 20:32:12.000000 antelope_foreground-0.3.0/antelope_foreground/entities/fragment_editor.py
--rw-r--r--   0 b          (500) b          (506)    72490 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/entities/fragments.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.116240 antelope_foreground-0.3.0/antelope_foreground/entities/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 22:26:47.000000 antelope_foreground-0.3.0/antelope_foreground/entities/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)    24130 2023-12-23 00:20:36.000000 antelope_foreground-0.3.0/antelope_foreground/entities/tests/test_fragments.py
--rw-r--r--   0 b          (500) b          (506)     3195 2020-03-30 08:22:53.000000 antelope_foreground-0.3.0/antelope_foreground/entities/tree_isomorphism.py
--rw-r--r--   0 b          (500) b          (506)    24628 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/foreground_catalog.py
--rw-r--r--   0 b          (500) b          (506)     6694 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/foreground_query.py
--rw-r--r--   0 b          (500) b          (506)    22984 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/fragment_flows.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.116240 antelope_foreground-0.3.0/antelope_foreground/implementations/
--rw-r--r--   0 b          (500) b          (506)      145 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/implementations/__init__.py
--rw-r--r--   0 b          (500) b          (506)    36737 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/implementations/foreground.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/interfaces/
--rw-r--r--   0 b          (500) b          (506)       52 2023-08-19 06:42:40.000000 antelope_foreground-0.3.0/antelope_foreground/interfaces/__init__.py
--rw-r--r--   0 b          (500) b          (506)    11523 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/interfaces/iforeground.py
--rw-r--r--   0 b          (500) b          (506)     5507 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/lcia_dict.py
--rw-r--r--   0 b          (500) b          (506)    17982 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/models.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/providers/
--rw-r--r--   0 b          (500) b          (506)      679 2023-08-19 06:42:40.000000 antelope_foreground-0.3.0/antelope_foreground/providers/__init__.py
--rw-r--r--   0 b          (500) b          (506)    26840 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/providers/lc_foreground.py
--rw-r--r--   0 b          (500) b          (506)    12828 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/providers/oryx_client.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/providers/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_foreground-0.3.0/antelope_foreground/providers/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     4547 2023-08-19 06:33:14.000000 antelope_foreground-0.3.0/antelope_foreground/providers/tests/test_foreground.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/
--rw-r--r--   0 b          (500) b          (506)      145 2018-07-26 08:24:01.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/__init__.py
--rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/antelope_lcia.py
--rw-r--r--   0 b          (500) b          (506)    15241 2023-08-19 06:42:40.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/antelope_v1.py
--rw-r--r--   0 b          (500) b          (506)       45 2018-07-26 08:24:01.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/exceptions.py
--rw-r--r--   0 b          (500) b          (506)     2754 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/foreground.py
--rw-r--r--   0 b          (500) b          (506)      362 2020-10-18 05:43:46.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/index.py
--rw-r--r--   0 b          (500) b          (506)     5834 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/quantity.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-05-29 08:50:45.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/tests/test_antelope_v1_client.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.119573 antelope_foreground-0.3.0/antelope_foreground/refs/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 23:07:29.000000 antelope_foreground-0.3.0/antelope_foreground/refs/__init__.py
--rw-r--r--   0 b          (500) b          (506)     8235 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/refs/fragment_ref.py
--rw-r--r--   0 b          (500) b          (506)    37123 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/terminations.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.122907 antelope_foreground-0.3.0/antelope_foreground/tests/
--rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 23:01:51.000000 antelope_foreground-0.3.0/antelope_foreground/tests/__init__.py
--rw-r--r--   0 b          (500) b          (506)     5290 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/antelope_foreground/tests/test_flow_conversion.py
--rw-r--r--   0 b          (500) b          (506)     1445 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/tests/test_foreground_impl.py
--rw-r--r--   0 b          (500) b          (506)     3981 2023-07-21 22:36:48.000000 antelope_foreground-0.3.0/antelope_foreground/tests/test_terminations.py
-drwxr-xr-x   0 b          (500) b          (506)        0 2024-03-21 22:50:52.112907 antelope_foreground-0.3.0/antelope_foreground.egg-info/
--rw-r--r--   0 b          (500) b          (506)      808 2024-03-21 22:50:52.000000 antelope_foreground-0.3.0/antelope_foreground.egg-info/PKG-INFO
--rw-r--r--   0 b          (500) b          (506)     2221 2024-03-21 22:50:52.000000 antelope_foreground-0.3.0/antelope_foreground.egg-info/SOURCES.txt
--rw-r--r--   0 b          (500) b          (506)        1 2024-03-21 22:50:52.000000 antelope_foreground-0.3.0/antelope_foreground.egg-info/dependency_links.txt
--rw-r--r--   0 b          (500) b          (506)       21 2024-03-21 22:50:52.000000 antelope_foreground-0.3.0/antelope_foreground.egg-info/requires.txt
--rw-r--r--   0 b          (500) b          (506)       20 2024-03-21 22:50:52.000000 antelope_foreground-0.3.0/antelope_foreground.egg-info/top_level.txt
--rw-r--r--   0 b          (500) b          (506)       38 2024-03-21 22:50:52.122907 antelope_foreground-0.3.0/setup.cfg
--rw-r--r--   0 b          (500) b          (506)     1273 2024-03-18 22:32:35.000000 antelope_foreground-0.3.0/setup.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/
+-rw-r--r--   0 b          (500) b          (506)      844 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)      245 2021-09-23 01:24:18.000000 antelope_foreground-0.3.1/README.md
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.981316 antelope_foreground-0.3.1/antelope_foreground/
+-rw-r--r--   0 b          (500) b          (506)       50 2020-11-05 09:29:01.000000 antelope_foreground-0.3.1/antelope_foreground/__init__.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.981316 antelope_foreground-0.3.1/antelope_foreground/data_sources/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-27 09:04:34.000000 antelope_foreground-0.3.1/antelope_foreground/data_sources/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    15880 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/data_sources/calrecycle_lca.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.981316 antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-27 09:05:24.000000 antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     8807 2024-05-10 00:37:09.000000 antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/test_calrecycle.py
+-rw-r--r--   0 b          (500) b          (506)     3414 2021-08-12 01:39:21.000000 antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/validate_calrecycle.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.981316 antelope_foreground-0.3.1/antelope_foreground/entities/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 22:38:35.000000 antelope_foreground-0.3.1/antelope_foreground/entities/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    18893 2023-08-22 20:32:12.000000 antelope_foreground-0.3.1/antelope_foreground/entities/fragment_editor.py
+-rw-r--r--   0 b          (500) b          (506)    73212 2024-05-10 00:37:09.000000 antelope_foreground-0.3.1/antelope_foreground/entities/fragments.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.981316 antelope_foreground-0.3.1/antelope_foreground/entities/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 22:26:47.000000 antelope_foreground-0.3.1/antelope_foreground/entities/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    24100 2024-05-10 00:37:10.000000 antelope_foreground-0.3.1/antelope_foreground/entities/tests/test_fragments.py
+-rw-r--r--   0 b          (500) b          (506)     3195 2020-03-30 08:22:53.000000 antelope_foreground-0.3.1/antelope_foreground/entities/tree_isomorphism.py
+-rw-r--r--   0 b          (500) b          (506)    24804 2024-05-06 23:05:17.000000 antelope_foreground-0.3.1/antelope_foreground/foreground_catalog.py
+-rw-r--r--   0 b          (500) b          (506)     6763 2024-05-08 22:27:52.000000 antelope_foreground-0.3.1/antelope_foreground/foreground_query.py
+-rw-r--r--   0 b          (500) b          (506)    23273 2024-05-10 00:37:10.000000 antelope_foreground-0.3.1/antelope_foreground/fragment_flows.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/implementations/
+-rw-r--r--   0 b          (500) b          (506)      145 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/implementations/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    37037 2024-05-14 20:08:43.000000 antelope_foreground-0.3.1/antelope_foreground/implementations/foreground.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/interfaces/
+-rw-r--r--   0 b          (500) b          (506)       52 2023-08-19 06:42:40.000000 antelope_foreground-0.3.1/antelope_foreground/interfaces/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    11921 2024-05-06 23:05:19.000000 antelope_foreground-0.3.1/antelope_foreground/interfaces/iforeground.py
+-rw-r--r--   0 b          (500) b          (506)     5507 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/lcia_dict.py
+-rw-r--r--   0 b          (500) b          (506)    18006 2024-05-06 23:05:17.000000 antelope_foreground-0.3.1/antelope_foreground/models.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/providers/
+-rw-r--r--   0 b          (500) b          (506)      679 2023-08-19 06:42:40.000000 antelope_foreground-0.3.1/antelope_foreground/providers/__init__.py
+-rw-r--r--   0 b          (500) b          (506)    27157 2024-05-09 04:27:14.000000 antelope_foreground-0.3.1/antelope_foreground/providers/lc_foreground.py
+-rw-r--r--   0 b          (500) b          (506)    12920 2024-05-06 23:05:17.000000 antelope_foreground-0.3.1/antelope_foreground/providers/oryx_client.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/providers/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_foreground-0.3.1/antelope_foreground/providers/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     4547 2024-05-09 04:27:25.000000 antelope_foreground-0.3.1/antelope_foreground/providers/tests/test_foreground.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/
+-rw-r--r--   0 b          (500) b          (506)      145 2018-07-26 08:24:01.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/__init__.py
+-rw-r--r--   0 b          (500) b          (506)        0 2018-07-26 08:24:01.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/antelope_lcia.py
+-rw-r--r--   0 b          (500) b          (506)    15241 2023-08-19 06:42:40.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/antelope_v1.py
+-rw-r--r--   0 b          (500) b          (506)       45 2018-07-26 08:24:01.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/exceptions.py
+-rw-r--r--   0 b          (500) b          (506)     2754 2024-05-06 23:05:17.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/foreground.py
+-rw-r--r--   0 b          (500) b          (506)      362 2020-10-18 05:43:46.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/index.py
+-rw-r--r--   0 b          (500) b          (506)     5834 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/quantity.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-05-29 08:50:45.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     2056 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/tests/test_antelope_v1_client.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/refs/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 23:07:29.000000 antelope_foreground-0.3.1/antelope_foreground/refs/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     9620 2024-05-10 00:37:10.000000 antelope_foreground-0.3.1/antelope_foreground/refs/fragment_ref.py
+-rw-r--r--   0 b          (500) b          (506)    37607 2024-05-10 00:37:09.000000 antelope_foreground-0.3.1/antelope_foreground/terminations.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground/tests/
+-rw-r--r--   0 b          (500) b          (506)        0 2020-09-25 23:01:51.000000 antelope_foreground-0.3.1/antelope_foreground/tests/__init__.py
+-rw-r--r--   0 b          (500) b          (506)     5290 2024-05-06 23:05:17.000000 antelope_foreground-0.3.1/antelope_foreground/tests/test_flow_conversion.py
+-rw-r--r--   0 b          (500) b          (506)     1445 2023-07-21 22:36:48.000000 antelope_foreground-0.3.1/antelope_foreground/tests/test_foreground_impl.py
+-rw-r--r--   0 b          (500) b          (506)     3979 2024-05-10 00:37:09.000000 antelope_foreground-0.3.1/antelope_foreground/tests/test_terminations.py
+drwxr-xr-x   0 b          (500) b          (506)        0 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/antelope_foreground.egg-info/
+-rw-r--r--   0 b          (500) b          (506)      844 2024-05-15 23:10:20.000000 antelope_foreground-0.3.1/antelope_foreground.egg-info/PKG-INFO
+-rw-r--r--   0 b          (500) b          (506)     2221 2024-05-15 23:10:20.000000 antelope_foreground-0.3.1/antelope_foreground.egg-info/SOURCES.txt
+-rw-r--r--   0 b          (500) b          (506)        1 2024-05-15 23:10:20.000000 antelope_foreground-0.3.1/antelope_foreground.egg-info/dependency_links.txt
+-rw-r--r--   0 b          (500) b          (506)       21 2024-05-15 23:10:20.000000 antelope_foreground-0.3.1/antelope_foreground.egg-info/requires.txt
+-rw-r--r--   0 b          (500) b          (506)       20 2024-05-15 23:10:20.000000 antelope_foreground-0.3.1/antelope_foreground.egg-info/top_level.txt
+-rw-r--r--   0 b          (500) b          (506)       38 2024-05-15 23:10:20.984649 antelope_foreground-0.3.1/setup.cfg
+-rw-r--r--   0 b          (500) b          (506)     1453 2024-05-15 23:08:33.000000 antelope_foreground-0.3.1/setup.py
```

### Comparing `antelope_foreground-0.3.0/PKG-INFO` & `antelope_foreground-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: antelope_foreground
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/AntelopeLCA/foreground
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: antelope_core>=0.3.1
 
 ![](https://travis-ci.com/AntelopeLCA/foreground.svg?branch=master) ![](https://coveralls.io/repos/github/AntelopeLCA/foreground/badge.svg?branch=master)
 
 # foreground
 An interface and implementation for building and analyzing foreground models
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/data_sources/calrecycle_lca.py` & `antelope_foreground-0.3.1/antelope_foreground/data_sources/calrecycle_lca.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/test_calrecycle.py` & `antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/test_calrecycle.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,26 +83,26 @@
         self.assertSetEqual(set(uom.scenarios()), {'sp24', 'quell_eg'})
 
     def test_named_fragment(self):
         self.assertEqual(fg['fragments/43']['Name'], 'Fuels Displacement Mixer - distillate')
 
     def test_passthrough(self):
         lm = fg['fragments/3']
-        inv, _ = lm.unit_inventory(None, observed=True)
+        inv, _ = lm.unit_flows(None, observed=True)
         self.assertEqual(len(inv), 3)  # 3 inventory flows
         self.assertEqual(len(set(x.fragment.flow for x in inv)), 2)  # 2 distinct flows
         self.assertSetEqual(set(x.fragment.direction for x in inv if x.fragment.flow == lm.flow),
                             {'Input', 'Output'})  # 2 distinct directions for reference flow
         self.assertSetEqual(set(x.magnitude for x in inv), {1})  # all flows have magnitude 1
 
     def test_traversal(self):
         uom = fg['fragments/55']
         ffs = uom.traverse(None, observed=True)
         self.assertEqual(len(ffs), 322)  # some ffs went away with uslci bg change 43d35c7; a few came back with 110321a
-        inv = uom.inventory(None, observed=True)
+        inv = uom.cutoffs(None, observed=True)
         light_fuel = next(x for x in inv if x.flow['Name'].startswith('Light Fuel'))
         self.assertEqual(floor(light_fuel.value), 116915718)
         incin = next(x for x in inv if x.flow['Name'].startswith('UO to Incin'))
         self.assertEqual(floor(incin.value), 484433)
 
     def test_lcia_0_indicators(self):
         """
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/data_sources/tests/validate_calrecycle.py` & `antelope_foreground-0.3.1/antelope_foreground/data_sources/tests/validate_calrecycle.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/entities/fragment_editor.py` & `antelope_foreground-0.3.1/antelope_foreground/entities/fragment_editor.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/entities/fragments.py` & `antelope_foreground-0.3.1/antelope_foreground/entities/fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 
 
 """
 
 import uuid
+import logging
 # from collections import defaultdict
 
-from antelope import comp_dir, check_direction, PropertyExists, CatalogRef, RxRef, QuantityRequired
+from antelope import comp_dir, check_direction, PropertyExists, CatalogRef, RxRef, QuantityRequired, RefQuantityRequired
 
-from ..fragment_flows import group_ios, FragmentFlow, ios_exchanges, frag_flow_lcia
+from ..fragment_flows import group_ios, FragmentFlow, ios_exchanges, frag_flow_lcia, FragmentInventoryDeprecated
 from antelope_core.entities import LcEntity, LcFlow
 from antelope_core.exchanges import ExchangeValue
 # from lcatools.interact import ifinput, parse_math
 from ..terminations import FlowTermination, MissingFlow
 from ..foreground_query import MissingResource
 
 class InvalidParentChild(Exception):
@@ -204,15 +205,19 @@
                         stagename = termination.name
                     except AttributeError:
                         pass
                 finally:
                     self._d['StageName'] = stagename
         # set EV last
         if balance_flow:
-            self.set_balance_flow()
+            try:
+                self.set_balance_flow()
+            except RefQuantityRequired:
+                # nothing much to do but notify
+                logging.warning('%s: Balance flow missing reference entity' % self.link)
         else:
             if exchange_value is not None:
                 self.set_exchange_value(0, exchange_value, units=units)
             if observe:
                 self.observed_ev = self.cached_ev
 
     def __hash__(self):
@@ -922,15 +927,15 @@
         The cf of the current flow in balanced units (if a balance flow exists)
         :return:
         """
         if self._balance_child is None:
             return None
         else:
             if self._balance_child.flow.reference_entity is None:
-                raise TypeError('Flow %s has no reference quantity' % self._balance_child.flow.link)
+                raise RefQuantityRequired('Flow %s has no reference quantity' % self._balance_child.flow.link)
             try:
                 return self._balance_child.flow.reference_entity.cf(self.flow)
             except (QuantityRequired, MissingResource):
                 return 0.0
 
     '''
     def balance(self, scenario=None, observed=False):
@@ -1219,15 +1224,15 @@
         Report proximal terminal nodes for the fragment (recurse until a nondescend is reached)
         :param scenario: [None]
         :param descend: [True] if False, yield subfragments as nodes
         :return: generator of terminal nodes
         """
         term = self.termination(scenario)
         yds = set()
-        if term.is_process or term.is_context:
+        if term.is_process or term.is_context or term.is_unresolved:
             if term.term_node not in yds:
                 yield term.term_node
                 yds.add(term.term_node)
         elif term.is_subfrag:
             if term.descend and descend:
                 for n in term.term_node.nodes(scenario, descend=descend):
                     if n not in yds:
@@ -1277,34 +1282,42 @@
 
         ffs = top.traverse(scenario=scenario, observed=observed)
 
         act = [k for k in ffs if k.fragment.top() is top]
         return act
 
     def inventory(self, scenario=None, scale=1.0, observed=False):
+        raise FragmentInventoryDeprecated('"inventory" is an exchange method. Use "cutoffs" instead.')
+
+    def cutoffs(self, scenario=None, scale=1.0, observed=False):
         """
         Converts unit inventory into a set of exchanges for easy display
         :param scenario:
         :param scale:
         :param observed:
         :return:
         """
-        ios, _ = self.unit_inventory(scenario=scenario, observed=observed)
+        ios, _ = self.unit_flows(scenario=scenario, observed=observed)
         return ios_exchanges(ios, ref=self)
 
     def exchanges(self, scenario=None):
         """
         Generator for query compatibility with processes
         :param scenario:
         :return:
         """
-        for x in self.inventory(scenario=scenario):
+        for x in self.child_flows:
+            yield x
+        for x in self.termination(scenario).unobserved_exchanges():
             yield x
 
     def unit_inventory(self, scenario=None, observed=False, frags_seen=None):
+        raise FragmentInventoryDeprecated('"inventory" is an exchange method. "unit_flows" replaces unit_inventory.')
+
+    def unit_flows(self, scenario=None, observed=False, frags_seen=None):
         """
         Traverses the fragment containing self, and returns a set of FragmentFlows indicating the net input/output
          with respect to a *unit node weight of the reference fragment*.
 
         Within the set of fragment flows:
          * all will have null terminations
          * every flow appears with only one direction
@@ -1324,14 +1337,15 @@
 
         ffs = top.traverse(scenario, observed=observed, frags_seen=frags_seen)
 
         ios, internal = group_ios(self, ffs)
 
         return ios, internal
 
+    '''
     def cutoffs(self, scenario=None, observed=False, aggregate=True):
         """
         Return a comprehensive list of cut-offs from a traversal result. Include implicit cutoffs from background
          computations.
         :param scenario:
         :param observed:
         :param aggregate: [True] if True, group cutoffs from different nodes together by flow.  If False, report each
@@ -1341,33 +1355,34 @@
         ffs = self.traverse(scenario, observed=observed)
         cos = []
         for ff in ffs:
             if ff.term.is_null:
                 cos.append(ff)
             else:
                 if ff.fragment.is_background:
-                    '''extend ff with background node cut-off flows.
-                    Need to think about this for a minute because self.is_background could be terminated to either
-                    a process or a fragment.  If it's a process, then for fragment LCIA we will be computing bg_lcia,
-                    so assuming a CatalogRef with background access.
-                    '''
+                    #extend ff with background node cut-off flows.
+                    #Need to think about this for a minute because self.is_background could be terminated to either
+                    #a process or a fragment.  If it's a process, then for fragment LCIA we will be computing bg_lcia,
+                    #so assuming a CatalogRef with background access.
+                    
                     ref = ff.term.term_node
                     cos.extend([FragmentFlow.cutoff(ff.fragment, i.flow, i.direction, i.value * ff.node_weight)
                                 for i in ref.lci(ref_flow=ff.term.term_flow.external_ref)
                                 if i.type in ('cutoff', 'context')])
                 elif ff.term.is_process:
                     # TODO: add in cutoffs from unobserved exchanges
                     pass
 
         if aggregate:
             cos, _ = group_ios(self, cos, include_ref_flow=False)
 
         return sorted([ExchangeValue(f.fragment, f.fragment.flow, f.fragment.direction, value=f.magnitude)
                        for f in cos], key=lambda x: (x.direction == 'Input', x.flow.context,
                                                      x.flow['Name'], x.value), reverse=True)
+    '''
 
     def traverse(self, scenario=None, observed=False, frags_seen=None):
         if isinstance(scenario, set):
             scenarios = set(scenario)
         elif isinstance(scenario, tuple) or isinstance(scenario, list):
             scenarios = set(scenario)
         elif scenario is None:
@@ -1683,45 +1698,45 @@
     """
     This turns out to be surprisingly complicated. So we now have:
      - LcFragment._traverse_node <-- which is called recursively
       + scenario matching + finds ev and term
       - selects handler based on term type:
        - LcFragment._subfragment_traversal
        |- invokes (static) _do_subfragment_traversal (YOU ARE HERE)
-       ||- calls [internally recursive] term_node.unit_inventory, which is just a wrapper for
+       ||- calls [internally recursive] term_node.unit_flows, which is just a wrapper for
        || - (static) group_ios
        ||  + reference flow and autoconsumption handling
        || /
        ||/
        |+ reference flow matching and normalizing
        + child flow matching and further recursion --> into LcFragment._traverse_node
       /
      /
      ffs, conserved_val
 
 
      - (static) group_ios
-     - nested inside LcFragment.unit_inventory, which is really just a wrapper
+     - nested inside LcFragment.unit_flows, which is really just a wrapper
      - called from
      - called from
 
     :param ff: The FragmentFlow whose subfragment is being traversed
     :param scenarios: to pass to subfragment
     :return: ffs [subfragment traversal appended], unit_inv [with reference flow removed], downstream node weight
     """
     term = ff.term  # note that we ignore term.direction in subfragment traversal
     node_weight = ff.node_weight
     self = ff.fragment
 
-    unit_inv, subfrags = term.term_node.unit_inventory(scenario=scenarios, frags_seen=frags_seen)
+    unit_inv, subfrags = term.term_node.unit_flows(scenario=scenarios, frags_seen=frags_seen)
 
     # find the inventory flow that matches us
     # use term_flow over term_node.flow because that allows client code to specify inverse traversal knowing
     #  only the sought flow.
-    # unit_inventory guarantees that there is exactly one of these flows (except in the case of cumulating flows!
+    # unit_flows guarantees that there is exactly one of these flows (except in the case of cumulating flows!
     # see group_ios)
     try:
         match = next(k for k in unit_inv if k.fragment.flow == term.term_flow)
     except StopIteration:
         print('Flow mismatch Traversing:\n%s' % self)
         print('Term flow: %s' % term.term_flow.link)
         print(term.serialize())
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/entities/tests/test_fragments.py` & `antelope_foreground-0.3.1/antelope_foreground/entities/tests/test_fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,21 +274,21 @@
         af is a very simple fragment with one reference flow and one foreground flow, which is a stand-in for an
         aggregated process inventory.
         :return:
         """
         ffs = self.af.traverse(None)
         self._check_fragmentflows(ffs, f4, 'Input', 1, 1)
 
-    def test_af_unit_inventory(self):
+    def test_af_unit_flows(self):
         """
-        A unit inventory reports two separate sets of fragment flows: cutoffs (cross system boundary) and nodes (within
+        unit flows reports two separate sets of fragment flows: cutoffs (cross system boundary) and nodes (within
         system boundary).  For af, there is one cutoff (the reference flow) and two internal, both foreground fragments.
         :return:
         """
-        io, ff = self.af.unit_inventory()
+        io, ff = self.af.unit_flows()
         self._check_fragmentflows(io, f4, 'Output', 1)
         self.assertEqual(len(ff), 2)
         # foreground <=> term is self -- to_foreground() replaced with termination to NullContext
         self.assertSetEqual({self.af, NullContext}, {f.term.term_node for f in ff})
 
     def test_unit_conversion_on_fragment_creation(self):
         self.assertEqual(self.a2.exchange_value(), a2_mj)
@@ -356,18 +356,18 @@
         should use the modeler's observed values, which default to zero.  Fragment a1 is not observed whereas fragment
         a2 is auto-observed to apply cached values as observed values throughout.
         Note: these tests rely on the behavior that LcFragment.traverse() by default uses cached (not observed) EVs
         This contrasts with traversal via the foreground interface, which uses observed EVs by default
 
         :return:
         """
-        ff1 = self.a1.inventory()
-        ff1o = self.a1.inventory(observed=True)
-        ff2 = self.a2.inventory()
-        ff2o = self.a2.inventory(observed=True)
+        ff1 = self.a1.cutoffs()
+        ff1o = self.a1.cutoffs(observed=True)
+        ff2 = self.a2.cutoffs()
+        ff2o = self.a2.cutoffs(observed=True)
         self.assertEqual(ff2, ff2o)
         self.assertNotEqual(ff1, ff1o)
         ff1t = self.a1.traverse(observed=True)
         fbal = next(f for f in ff1t if f.fragment is self.a1.balance_flow)
         self.assertEqual(fbal.magnitude, self.a1.exchange_value() - a1_addl_obs)
 
     def test_scenarios_detection(self):
@@ -398,15 +398,15 @@
         """
         fragment self.aa produces f7 "ancillary flows" in the amount of one unit.  but it also depends on fragment
         self.a2, which has a cutoff input requirement for f7.  The inventory results for self.aa should report only
         net production of f7
         :return:
         """
         f7_autoconsumption = aa_mj_in / self.a2.exchange_value() * a2_private * a2_item
-        inv = self.aa.inventory()
+        inv = self.aa.cutoffs()
         f7_out = next(f for f in inv if f.flow is f7)
         f5_in = next(f for f in inv if f.flow is f5)
         self.assertEqual((f7_out.direction, f7_out.value), ('Output', 1 - f7_autoconsumption))
         self.assertEqual((f5_in.direction, f5_in.value), ('Input', aa_in))
 
     def test_nonreference_subfragment(self):
         """
@@ -461,19 +461,19 @@
         ffs = self.aa.traverse('nondescend')  # ensure that the subfragment's dependence on af is concealed
         for f in ffs:
             if f.fragment.top() is self.af:
                 self.assertTrue(f.node_weight < 0, '%s' % f)
 
     def test_descend_equivalence(self):
         """
-        Inventory results should not vary regardless of descend (this may require more robust testing)
+        Cutoffs results should not vary regardless of descend (this may require more robust testing)
         :return:
         """
-        inv_d = self.aa.inventory()
-        inv_nd = self.aa.inventory('nondescend')
+        inv_d = self.aa.cutoffs()
+        inv_nd = self.aa.cutoffs('nondescend')
         self.assertEqual(inv_d, inv_nd)
 
     def test_nondescend_privacy(self):
         """
         The internal fragment of fp in self.a2 should be concealed when descend=False, visible when descend=True
         :return:
         """
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/entities/tree_isomorphism.py` & `antelope_foreground-0.3.1/antelope_foreground/entities/tree_isomorphism.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/foreground_catalog.py` & `antelope_foreground-0.3.1/antelope_foreground/foreground_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                 self._missing_o.remove(key)
 
     def new_resource(self, reference, source, ds_type, store=True, **kwargs):
         res = super(ForegroundCatalog, self).new_resource(reference, source, ds_type, store=store, **kwargs)
         self._check_missing_o(res)
         return res
 
-    def add_resource(self, resource, store=True):
-        super(ForegroundCatalog, self).add_resource(resource, store=store)
+    def add_resource(self, resource, **kwargs):
+        super(ForegroundCatalog, self).add_resource(resource, **kwargs)
         self._check_missing_o(resource)
 
     def is_in_queue(self, home):
         """
         This tells us whether the foreground named in home is actively being instantiated
         :param home:
         :return:
@@ -198,37 +198,44 @@
             try:
                 for k in super(ForegroundCatalog, self).gen_interfaces(origin, itype=itype, strict=strict):
                     yield k
             except (UnknownOrigin, InterfaceError):
                 self._missing_o.add((origin, itype))
                 raise MissingResource(origin, itype)
 
+    @property
+    def test(self):
+        return bool(self._test)
+
     def create_foreground(self, ref, path=None, quiet=True):
         """
         Creates foreground resource and returns an interface to that resource.
         By default creates in a subdirectory of the catalog root with the ref as the folder
         :param ref:
         :param path:
         :param quiet:
         :return:
         """
         assert bool(foreground_origin_regexp.match(ref)), "Foreground reference not valid: %s" % ref
-        if path is None:
-            path = os.path.join(self._rootdir, ref)  # should really sanitize this somehow
-            # localpath = ref
+        if self._test:
+            local_path = ref
         else:
-            if os.path.isabs(path):
-                pass
-                # localpath = None
+            if path is None:
+                path = os.path.join(self._rootdir, ref)  # should really sanitize this somehow
+                # localpath = ref
             else:
-                # localpath = path
-                path = os.path.join(self._rootdir, path)
+                if os.path.isabs(path):
+                    pass
+                    # localpath = None
+                else:
+                    # localpath = path
+                    path = os.path.join(self._rootdir, path)
 
-        abs_path = os.path.abspath(path)
-        local_path = self._localize_source(abs_path)
+            abs_path = os.path.abspath(path)
+            local_path = self._localize_source(abs_path)
 
         res = self.new_resource(ref, local_path, 'LcForeground',
                                 interfaces=['basic', 'index', 'foreground', 'quantity'],
                                 quiet=quiet)
 
         return self._check_foreground(res)
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/foreground_query.py` & `antelope_foreground-0.3.1/antelope_foreground/foreground_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,40 @@
             return self._catalog.foreground(origin)
         return super(ForegroundQuery, self).cascade(origin)
 
     """
     Add foreground interface to query object.
     We also need to add lubricating code to translate between pydantic models and operable objects
     """
-    def make_term_from_anchor(self, parent, anchor, scenario, flow_conversion):
+    def make_term_from_anchor(self, parent, anchor, scenario, flow_conversion=None):
         if anchor.is_null:
             term = FlowTermination.null(parent)
         else:
             if anchor.anchor_flow:
                 term_flow = self.get(anchor.anchor_flow.entity_id,
                                      origin=anchor.anchor_flow.origin)
             else:
                 term_flow = None
 
             """
             def characterize(self, flowable, ref_quantity, query_quantity, value, context=None, location='GLO', **kws):
             """
             if anchor.context:
                 cx = self.get_context(anchor.context)
-                if term_flow is not None and flow_conversion != 1.0:
+                if term_flow is not None and flow_conversion is not None and flow_conversion != 1.0:
                     print('Term CF %s : %s [%g]' % (parent.link, cx, flow_conversion))
                     # log reported flow conversion.  Some shit to sort out w/r/t/ context
                     self.characterize(parent.flow.name, parent.flow.reference_entity, term_flow.reference_entity,
                                       flow_conversion, context=cx)
 
                 term = FlowTermination(parent, cx, term_flow=term_flow,
                                        descend=anchor.descend)
             elif anchor.node:
                 term_node = self.get(anchor.node.entity_id, origin=anchor.node.origin)
-                if flow_conversion != 1.0:
+                if flow_conversion is not None and flow_conversion != 1.0:
                     rx = term_node.reference(term_flow)
                     print('Term CF %s : %s [%g]' % (parent.link, term_node.link, flow_conversion))
                     # log reported flow conversion.  Some shit to sort out w/r/t/ context
                     self.characterize(parent.flow.name, parent.flow.reference_entity, rx.flow.reference_entity,
                                       flow_conversion, context=(term_node.origin, term_node.external_ref))
 
                 term = FlowTermination(parent, term_node, term_flow=term_flow,
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/fragment_flows.py` & `antelope_foreground-0.3.1/antelope_foreground/fragment_flows.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from .terminations import FlowTermination, UnCachedScore, UnresolvedAnchor
 from antelope_core.lcia_results import LciaResult, DetailedLciaResult, SummaryLciaResult
 
 from collections import defaultdict
 import uuid
 
 
+class FragmentInventoryDeprecated(Exception):
+    """
+    The "inventory" term for fragmnts is deprecated.  "unit_inventory" is now "unit_flows" and "inventory"
+    is what it has always been: "cutoffs".  And the old "cutoffs" is gone because it literally never worked.
+    """
+    pass
+
+
 class CumulatingFlows(Exception):
     """
     when a fragment includes multiple instances of the reference flow having consistent (i.e. not complementary)
     directions. Not handled in subfragment traversal bc no valid test case
     """
     pass
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/implementations/foreground.py` & `antelope_foreground-0.3.1/antelope_foreground/implementations/foreground.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,19 +271,28 @@
                         raise TypeError("ref quantity (%s) doesn't match supplied (%s)" % (t.reference_entity,
                                                                                            reference))
                 elif t.entity_type == 'quantity':
                     if t.unit != reference:
                         raise TypeError("ref unit (%s) doesn't match supplied (%s)" % (t.unit, reference))
                 if t['Name'] != name:
                     raise ValueError("Name (%s) doesn't match supplied(%s)" % (t['Name'], name))
+            else:
+                if t['Name'] != name:
+                    t['Name'] = name
+            for k, v in kwargs.items():
+                if v is not None:
+                    t[k] = v
             return t
 
         except EntityNotFound:
             try:
-                return self.new_flow(name, ref_quantity=reference, external_ref=external_ref, context=group, **kwargs)
+                cx = kwargs.pop('context', group)
+                if group:
+                    kwargs['group'] = group
+                return self.new_flow(name, ref_quantity=reference, external_ref=external_ref, context=cx, **kwargs)
             except UnknownRefQuantity:
                 # assume reference is a unit string specification
                 return self.new_quantity(name, ref_unit=reference, external_ref=external_ref, group=group, **kwargs)
 
     def new_flow(self, name, ref_quantity=None, **kwargs):
         """
 
@@ -550,16 +559,15 @@
                 return False
         self._archive.delete_fragment(fragment)
         for c in fragment.child_flows:
             self.delete_fragment(c)
         return True
 
     def save(self, save_unit_scores=False):
-        self._archive.save(save_unit_scores=save_unit_scores)
-        return True
+        return self._archive.save(save_unit_scores=save_unit_scores)
 
     def tree(self, fragment, **kwargs):
         """
 
         :param fragment:
         :param kwargs:
         :return:
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/interfaces/iforeground.py` & `antelope_foreground-0.3.1/antelope_foreground/interfaces/iforeground.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,24 @@
         :param name:
         :param kwargs:
         :return:
         """
         return self._perform_query(_interface, 'add_or_retrieve', ForegroundRequired,
                                    external_ref, reference, name, **kwargs)
 
+    def post_entity_refs(self, entity_refs, **kwargs):
+        """
+        Add entities to the foreground by reference. mostly useful when working with remote foregrounds.
+        :param entity_refs:
+        :param kwargs:
+        :return:
+        """
+        return self._perform_query(_interface, 'post_entity_refs', ForegroundRequired,
+                                   entity_refs, **kwargs)
+
     def create_fragment_from_node(self, process_ref, ref_flow=None, include_elementary=False):
         """
         a synonym for create_process_model
         :param process_ref: a ProcessRef
         :param ref_flow:
         :param include_elementary:
         :return:
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/lcia_dict.py` & `antelope_foreground-0.3.1/antelope_foreground/lcia_dict.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/models.py` & `antelope_foreground-0.3.1/antelope_foreground/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
 
 
 class LcForeground(ResponseModel):
 
     catalogNames: Dict[str, List[str]]  #
     dataSource: str  #
     dataSourceType: str  #
-    flows: List[Dict]  #
+    flows: List[Dict]  # these should be removed
     initArgs: Dict  #
     quantities: List[Dict]  #
     termManager: Optional[TermManager]  #
     models: List[LcModel]
     resources: List[ResourceSpec]
 
     @classmethod
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/__init__.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/lc_foreground.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/lc_foreground.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 A foreground archive is an LcArchive that also knows how to access, serialize, and deserialize fragments.
 """
 import json
 import os
 import re
+import logging
 
 from typing import Optional
 
 from collections import defaultdict
 from pydantic import ValidationError
 
 from ..foreground_query import DelayedQuery, ForegroundNotSafe, QueryIsDelayed, MissingResource
@@ -446,14 +447,16 @@
         This must be done in two steps, since fragments refer to other fragments in their definition.
         First step: create all fragments.
         Second step: set reference entities and terminations
         :return:
         """
         fragments = []
         if not os.path.exists(self._fragment_dir):
+            if self._catalog and self._catalog.test:
+                return
             os.makedirs(self._fragment_dir)
         for file in os.listdir(self._fragment_dir):
             if os.path.isdir(os.path.join(self._fragment_dir, file)):
                 continue
             with open(os.path.join(self._fragment_dir, file), 'r') as fp:
                 j = json.load(fp)
 
@@ -479,20 +482,25 @@
         for leftover in current_files:
             if not os.path.isdir(os.path.join(self._fragment_dir, leftover)):
                 print('deleting %s' % leftover)
                 os.remove(os.path.join(self._fragment_dir, leftover))
 
     def save_metadata(self):
         if not os.path.isdir(self.source):
+            if self._catalog and self._catalog.test:
+                return
             os.makedirs(self.source)
 
         with open(self._metadata_file, 'w') as fp:
             json.dump(self._metadata.model_dump(), fp, indent=2)
 
     def save(self, save_unit_scores=False):
+        if self._catalog and self._catalog.test:
+            logging.info('Cannot save foregrounds during tester operation')
+            return False
         if not os.path.isdir(self.source):
             os.makedirs(self.source)
 
         self.write_to_file(self._archive_file, gzip=False, characterizations=True, values=True, domesticate=False)
 
         self.save_metadata()
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/oryx_client.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/oryx_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,16 @@
         llargs = {k.lower(): v for k, v in kwargs.items()}
         return [self._archive.get_or_make(k) for k in self._archive.r.get_many(FragmentRefModel, 'fragments', **llargs)]
 
     def post_foreground(self, fg, save_unit_scores=False):
         pydantic_fg = LcForeground.from_foreground_archive(fg.archive, save_unit_scores=save_unit_scores)
         return self._archive.r.post_return_one(pydantic_fg.dict(), OriginCount, 'post_foreground')
 
-    def post_entity_refs(self, post_ents: List[EntityRef]):
+    def post_entity_refs(self, entities, **kwargs):
+        post_ents = [p if isinstance(p, EntityRef) else EntityRef.from_entity(p) for p in entities]
         return self._archive.r.post_return_one([p.model_dump() for p in post_ents], OriginCount, 'entity_refs')
 
     def save(self):
         return self._archive.r.post_return_one(None, bool, 'save_foreground')
 
     def restore(self):
         return self._archive.r.post_return_one(None, bool, 'restore_foreground')
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/tests/test_foreground.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/tests/test_foreground.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/antelope_v1.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/antelope_v1.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/foreground.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/foreground.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/quantity.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/quantity.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/providers/v1_client/tests/test_antelope_v1_client.py` & `antelope_foreground-0.3.1/antelope_foreground/providers/v1_client/tests/test_antelope_v1_client.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/refs/fragment_ref.py` & `antelope_foreground-0.3.1/antelope_foreground/refs/fragment_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from antelope.refs.base import EntityRef
 from antelope.refs import RxRef
 from antelope import comp_dir
-from ..fragment_flows import group_ios, ios_exchanges
+from ..fragment_flows import group_ios, ios_exchanges, FragmentInventoryDeprecated
 from ..models import Anchor
 """
 Not sure what to do about Fragment Refs, whether they belong in the main interface. I'd like to think no, but
 for now we will just deprecate them and remove functionality,
 """
 
 
@@ -130,22 +130,26 @@
             self._load_anchors()
             return self._anchors[scenario]
 
     @property
     def child_flows(self):
         return self._query.child_flows(self)
 
+    @property
+    def is_background(self):
+        return len(self.child_flows) == 0  # self._background
+
     def set_name(self, name, **kwargs):
         return self._query.name_fragment(self, name, **kwargs)
 
     '''
     Process compatibility
     '''
-    def inventory(self, scenario=None, **kwargs):
-        ios, _ = self.unit_inventory(scenario=scenario, **kwargs)  # in the future, may want to cache this
+    def cutoffs(self, scenario=None, **kwargs):
+        ios, _ = self.unit_flows(scenario=scenario, **kwargs)  # in the future, may want to cache this
         return ios_exchanges(ios, ref=self)
 
     def activity(self, scenario=None, **kwargs):
         """
         Report interior nodes of the fragments and their activity levels-- converse of inventory()
         :return:
         """
@@ -209,14 +213,42 @@
                 cur_stage = _print_branch(branch, cur_stage)
 
         # finish up by capping off remaining levels
         while len(pnts) > 0:
             pnts.pop()
             print('   %s    x ' % _pfx())  # end cap
 
+    def nodes(self, scenario=None, descend=True):
+        """
+        Report proximal terminal nodes for the fragment (recurse until a nondescend is reached)
+        :param scenario: [None]
+        :param descend: [True] if False, yield subfragments as nodes
+        :return: generator of terminal nodes
+        """
+        term = self.anchor(scenario)
+        yds = set()
+        if term.is_process or term.is_context or term.is_unresolved:
+            if term.term_node not in yds:
+                yield term.term_node
+                yds.add(term.term_node)
+        elif term.is_subfrag:
+            if term.descend and descend:
+                for n in term.term_node.nodes(scenario, descend=descend):
+                    if n not in yds:
+                        yield n
+                        yds.add(n)
+            else:
+                yield term.term_node
+            # foreground, null: do nothing
+        for c in self.child_flows:
+            for n in c.nodes(scenario, descend=descend):
+                if n not in yds:
+                    yield n
+                    yds.add(n)
+
     def traverse(self, scenario=None, **kwargs):
         return self._query.traverse(self, scenario=scenario, **kwargs)
 
     def lci(self, scenario=None):
         """
         TODO
         complex process that will require a recursive traversal and accumulation of LCIs from self + child fragments
@@ -236,14 +268,17 @@
         """
         return self._query.fragment_lcia(self, lcia_qty, scenario=scenario, mode=mode, **kwargs)
 
     def bg_lcia(self, lcia_qty, scenario=None, **kwargs):
         return self.fragment_lcia(self, lcia_qty, scenario=scenario, **kwargs)
 
     def unit_inventory(self, scenario=None, observed=None):
+        raise FragmentInventoryDeprecated('"inventory" is an exchange method. Use "unit_flows" instead.')
+
+    def unit_flows(self, scenario=None, observed=None):
         """
 
         :param scenario:
         :param observed: ignored; supplied only for signature consistency
         :return:
         """
         '''
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/terminations.py` & `antelope_foreground-0.3.1/antelope_foreground/terminations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Flow Terminations are model-defined links between a particular flow and a process that terminates it.
 
 They originated as part of LcFragments but in fact they are more general. A FlowTermination is actually the same
 as a ProductFlow in lca-matrix, plus features to compute LCIA.  It should be easy to construct either one from the
 other.
 """
+import logging
 
 from antelope import (BackgroundRequired, check_direction, comp_dir, QuantityRequired, MultipleReferences,
-                      NoReference, ConversionReferenceMismatch, EntityNotFound)
+                      NoReference, ConversionReferenceMismatch, EntityNotFound, NoCatalog)
 
 from antelope_core.contexts import NullContext
 from antelope_core.exchanges import ExchangeValue
 from antelope_core.lcia_results import LciaResult
 from antelope_core.implementations.quantity import do_lcia
 from .lcia_dict import LciaResults
 from .models import Anchor, EntityRef, UNRESOLVED_ANCHOR_TYPE
@@ -132,15 +133,15 @@
         descend = j.pop('descend', True)
         try:
             term = cls(fragment, term_node, _direction=direction, term_flow=term_flow, descend=descend)
         except MultipleReferences:
             raise TerminationFromJson('term_flow missing and ambiguous: %s (%s)' % (fragment.link, scenario))
         except FlowConversionError:
             t = term_flow or term_node
-            raise TerminationFromJson('Flow Conversion Error %s =/= %s' % (fragment.flow.link, t.link))
+            raise TerminationFromJson('Flow Conversion Error %s =/= %s' % (fragment.link, t.link))
         if 'scoreCache' in j.keys():
             term._deserialize_score_cache(fg, j['scoreCache'], scenario)
         return term
 
     '''
     @classmethod
     def from_exchange_ref(cls, fragment, exchange_ref):
@@ -209,14 +210,20 @@
 
         self.term_flow = term_flow
         self.direction = _direction
         self.descend = descend
 
     @property
     def term_node(self):
+        if self._term:
+            if self._term.entity_type == UNRESOLVED_ANCHOR_TYPE:
+                try:
+                    self._term = self._term.resolve()
+                except NoCatalog:
+                    pass
         return self._term
 
     @property
     def term_flow(self):
         if self._term_flow is None:
             if self.is_process:
                 raise AttributeError('[%s] term_flow was not specified for process term!' % self._parent.external_ref)
@@ -254,15 +261,15 @@
                 except NoReference:  # we need to allow processes with no reference to be used as term nodes
                     self._term_flow = term_flow
                 except KeyError:
                     raise MissingFlow(term_flow)
             elif self.is_frag:
                 if term_flow == self.term_node.flow:  # don't need the inventory every time
                     self._term_flow = term_flow
-                elif term_flow in (x.flow for x in self.term_node.inventory()):
+                elif term_flow in (x.flow for x in self.term_node.cutoffs()):
                     self._term_flow = term_flow
                 else:
                     raise MissingFlow(term_flow)
             else:
                 self._term_flow = term_flow
         if self.valid and self.node_weight_multiplier == 0:  # we don't need to re-validate the flow
             print('Warning: 0 node weight multiplier for term of %s' % self._parent.external_ref)
@@ -424,14 +431,18 @@
         return self.is_frag and not self.is_fg  # or self.is_bg or self.term_is_bg)
 
     @property
     def is_null(self):
         return self._term is None
 
     @property
+    def is_unresolved(self):
+        return self._term is not None and self._term.entity_type == UNRESOLVED_ANCHOR_TYPE
+
+    @property
     def descend(self):
         return self._descend
 
     @descend.setter
     def descend(self, value):
         if value is None:
             return
@@ -494,26 +505,28 @@
 
         "hey look at me, net calorific value. see that mass flow f4- a unit of it is worth 35 of me"
         is how the database is constructed.
         
         but each call to quantity_relation should check for both forward and reverse matches
         '''
         if not self.valid:
-            print('WE ARE NOT EVEN TRYING')
+            logging.warning('Flow Conversion attempted on invalid term node %5.5s' % self._parent.uuid)
             return 1.0
         # if not self.term_flow.validate():
         #     return 1.0
         if self.term_flow is None:
             raise MissingFlow(self)
         if self._parent.flow is None:
             raise MalformedParent(self._parent)
         if self.term_flow.reference_entity == self._parent.flow.reference_entity:
             return 1.0
         parent_q = self._parent.flow.reference_entity
         term_q = self.term_flow.reference_entity
+        if term_q is None:
+            return 0.0
 
         # first - natural - ask our parent flow if fit can convert to term quantity
         try:
             rev = self._parent.flow.cf(term_q, context=self.term_node.external_ref)
         except (QuantityRequired, NotImplementedError, ConversionReferenceMismatch):
             rev = None
 
@@ -588,15 +601,15 @@
     def unit(self):
         if self.is_null:
             return '--'
         if self.term_node.entity_type == 'fragment':  # fg, bg, or subfragment
             return '%4g unit' % self.inbound_exchange_value
         return '%4g %s' % (self.inbound_exchange_value, self.term_flow.unit)  # process
 
-    def _unobserved_exchanges(self, refresh=False):
+    def unobserved_exchanges(self, refresh=False):
         """
         Generator which yields exchanges from the term node's inventory that are not found among the child flows, for
           LCIA purposes
 
         Challenge here going forward: we made some kind of normative decision early on that terminations do not know
         their own scenarios, that the fragment maps scenario to termination. The problem is that now terminations
         cannot themselves carry out traversal on the term_node because they don't know what scenarios to pass.
@@ -667,15 +680,15 @@
                 locale = 'GLO'
 
             try:
                 res = self.term_node.bg_lcia(quantity_ref, observed=self._parent.child_flows, ref_flow=self.term_flow,
                                              refresh=refresh, locale=locale, **kwargs)
             except (QuantityRequired, EntityNotFound, NotImplementedError):
                 try:
-                    res = quantity_ref.do_lcia(self._unobserved_exchanges(refresh=refresh), locale=locale,
+                    res = quantity_ref.do_lcia(self.unobserved_exchanges(refresh=refresh), locale=locale,
                                                refresh=refresh, **kwargs)
                 except (BackgroundRequired, NotImplementedError):
                     res = self._fallback_lcia(quantity_ref, locale, **kwargs)
             except BackgroundRequired:
                 res = self._fallback_lcia(quantity_ref, locale, **kwargs)
 
         if isinstance(res, list):
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground/tests/test_flow_conversion.py` & `antelope_foreground-0.3.1/antelope_foreground/tests/test_flow_conversion.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/tests/test_foreground_impl.py` & `antelope_foreground-0.3.1/antelope_foreground/tests/test_foreground_impl.py`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/antelope_foreground/tests/test_terminations.py` & `antelope_foreground-0.3.1/antelope_foreground/tests/test_terminations.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,28 +47,28 @@
         self.assertFalse(term.is_null)
         self.assertFalse(term.is_subfrag)
         self.assertTrue(term.is_bg)  # bg now means "no child flows"
         self.assertFalse(term.term_is_bg)
 
     def test_unobserved(self):
         term = self._petro_term()
-        ux = [x for x in term._unobserved_exchanges()]
+        ux = [x for x in term.unobserved_exchanges()]
         self.assertEqual(len(ux), 42)
 
     def _frag_with_child(self):
         frag = self._petro_frag()
         frag.terminate(self.petro.make_ref(self.A.query), term_flow=frag.flow)
         lead = next(x for x in self.petro.inventory(frag.flow) if x.flow['Name'].startswith('Lead'))
         c = create_fragment(flow=lead.flow, direction=lead.direction, parent=frag, value=lead.value)
         c.terminate(self.A.tm[lead.flow.context])
         return frag
 
     def test_unobserved_with_child(self):
         frag = self._frag_with_child()
-        ux = [x for x in frag.term._unobserved_exchanges()]
+        ux = [x for x in frag.term.unobserved_exchanges()]
         self.assertEqual(len(ux), 41)
 
     def _get_coolness(self):
         q = next(self.A.search('quantity', Name='coolness'))
         return q.make_ref(self.A.query)
 
     def test_lcia(self):
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground.egg-info/PKG-INFO` & `antelope_foreground-0.3.1/antelope_foreground.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: antelope-foreground
-Version: 0.3.0
+Name: antelope_foreground
+Version: 0.3.1
 Home-page: https://github.com/AntelopeLCA/foreground
 Author: Brandon Kuczenski
 Author-email: bkuczenski@ucsb.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: antelope_core>=0.3.1
 
 ![](https://travis-ci.com/AntelopeLCA/foreground.svg?branch=master) ![](https://coveralls.io/repos/github/AntelopeLCA/foreground/badge.svg?branch=master)
 
 # foreground
 An interface and implementation for building and analyzing foreground models
```

### Comparing `antelope_foreground-0.3.0/antelope_foreground.egg-info/SOURCES.txt` & `antelope_foreground-0.3.1/antelope_foreground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antelope_foreground-0.3.0/setup.py` & `antelope_foreground-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 
 requires = [
-    'antelope_core>=0.3.0'
+    'antelope_core>=0.3.1'
 ]
 
 """
 Revision history
 
+0.3.1   2024-05-15 - "inventory" operations on fragments deprecated
+                     tester catalogs now filesystem-free
+                     handle unresolved anchor issues 
+
 0.3.0   2024-01-05 - 0.3-branch development version, supporting end-user access to vault.lc resources 
 
 # ^ 0.3.* 0.3-branch fork   
 # v 0.2.* main / master for legacy projects
 
 0.2.1 - 21 Jul 2023 - Subfrags comes home-- complete changes throughout the system, impossible to recount.
```

