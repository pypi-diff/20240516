# Comparing `tmp/fnschool-20240516.1949.11.tar.gz` & `tmp/fnschool-20240516.2157.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240516.1949.11.tar", last modified: Thu May 16 11:49:15 2024, max compression
+gzip compressed data, was "fnschool-20240516.2157.4.tar", last modified: Thu May 16 13:57:08 2024, max compression
```

## Comparing `fnschool-20240516.1949.11.tar` & `fnschool-20240516.2157.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.677043 fnschool-20240516.1949.11/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240516.1949.11/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 11:49:15.676043 fnschool-20240516.1949.11/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240516.1949.11/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240516.1949.11/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 11:49:15.677043 fnschool-20240516.1949.11/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.655043 fnschool-20240516.1949.11/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.661043 fnschool-20240516.1949.11/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.668043 fnschool-20240516.1949.11/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6983 2024-05-16 06:04:05.000000 fnschool-20240516.1949.11/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240516.1949.11/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.669043 fnschool-20240516.1949.11/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240516.1949.11/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240516.1949.11/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240516.1949.11/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240516.1949.11/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1949.11/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1949.11/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.673043 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1870 2024-05-16 06:04:05.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1898 2024-05-16 06:04:05.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8948 2024-05-16 06:04:05.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9399 2024-05-16 06:04:06.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8266 2024-05-16 06:04:05.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9722 2024-05-16 11:41:38.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2294 2024-05-16 06:04:06.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1949.11/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.674043 fnschool-20240516.1949.11/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240516.1949.11/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.657043 fnschool-20240516.1949.11/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.656043 fnschool-20240516.1949.11/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.674043 fnschool-20240516.1949.11/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.656043 fnschool-20240516.1949.11/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.674043 fnschool-20240516.1949.11/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    18033 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.657043 fnschool-20240516.1949.11/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.675043 fnschool-20240516.1949.11/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.657043 fnschool-20240516.1949.11/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.675043 fnschool-20240516.1949.11/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.657043 fnschool-20240516.1949.11/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.675043 fnschool-20240516.1949.11/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:49:11.000000 fnschool-20240516.1949.11/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 04:52:14.000000 fnschool-20240516.1949.11/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:49:15.676043 fnschool-20240516.1949.11/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2184 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 11:49:15.000000 fnschool-20240516.1949.11/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.953235 fnschool-20240516.2157.4/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240516.2157.4/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-16 13:57:08.952235 fnschool-20240516.2157.4/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240516.2157.4/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240516.2157.4/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 13:57:08.953235 fnschool-20240516.2157.4/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.931235 fnschool-20240516.2157.4/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.937235 fnschool-20240516.2157.4/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.944235 fnschool-20240516.2157.4/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6983 2024-05-16 06:04:05.000000 fnschool-20240516.2157.4/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240516.2157.4/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.945235 fnschool-20240516.2157.4/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240516.2157.4/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240516.2157.4/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240516.2157.4/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240516.2157.4/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.2157.4/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.2157.4/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.949235 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1870 2024-05-16 06:04:05.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1898 2024-05-16 06:04:05.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8948 2024-05-16 06:04:05.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9399 2024-05-16 06:04:06.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8266 2024-05-16 06:04:05.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10536 2024-05-16 13:51:12.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2294 2024-05-16 06:04:06.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.2157.4/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.950235 fnschool-20240516.2157.4/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240516.2157.4/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.933235 fnschool-20240516.2157.4/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.932235 fnschool-20240516.2157.4/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.950235 fnschool-20240516.2157.4/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.932235 fnschool-20240516.2157.4/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.950235 fnschool-20240516.2157.4/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18082 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.933235 fnschool-20240516.2157.4/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.950235 fnschool-20240516.2157.4/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.933235 fnschool-20240516.2157.4/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.951235 fnschool-20240516.2157.4/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.933235 fnschool-20240516.2157.4/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.951235 fnschool-20240516.2157.4/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 13:57:04.000000 fnschool-20240516.2157.4/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 04:52:14.000000 fnschool-20240516.2157.4/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 13:57:08.951235 fnschool-20240516.2157.4/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2184 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 13:57:08.000000 fnschool-20240516.2157.4/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240516.1949.11/LICENSE` & `fnschool-20240516.2157.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/PKG-INFO` & `fnschool-20240516.2157.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240516.1949.11
+Version: 20240516.2157.4
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240516.1949.11/README.md` & `fnschool-20240516.2157.4/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/pyproject.toml` & `fnschool-20240516.2157.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/__init__.py` & `fnschool-20240516.2157.4/src/fnschool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.fnprint import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240516.1949.11"
+__version__ = "20240516.2157.04"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/bill.cp.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/bill.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/canteen.toml` & `fnschool-20240516.2157.4/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/config.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240516.2157.4/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240516.2157.4/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240516.2157.4/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/food.cp.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/food.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/food_classes.toml` & `fnschool-20240516.2157.4/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/operator.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/path.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/profile.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,40 +141,57 @@
                     (
                         _("New purchased food for date {0} is:")
                         if len(new_wbfoods) > 1
                         else _("New purchased foods for date {0} are:")
                     ).format(tn1.strftime("%Y.%m.%d"))
                 )
 
+                new_wbfoods_count_len = len(str(len(new_wbfoods)))
                 new_wbfood_tips = [
-                    f"({i+1}){f.name} {f.count} {f.unit_name}"
+                    f"{i+1:0>{new_wbfoods_count_len}} {f.name} {f.count} {f.unit_name}"
                     for i, f in enumerate(new_wbfoods)
                 ]
-                new_wbfood_tips_len_sqrt = math.ceil(
-                    len(new_wbfood_tips) ** 0.5
-                )
+                new_wbfood_tips_len = len(new_wbfood_tips)
+                new_wbfood_tips_len_sqrt = math.ceil(new_wbfood_tips_len**0.5)
                 new_wbfood_tip_len = (
                     max(
                         [
                             len(t) + len([c for c in t if is_zh_CN_char(c)])
                             for t in new_wbfood_tips
                         ]
                     )
                     + 1
                 )
                 new_wbfood_tips_value = ""
-                for i, t in enumerate(new_wbfood_tips):
-                    tip_len = new_wbfood_tip_len - len(
-                        [c for c in t if is_zh_CN_char(c)]
-                    )
-                    new_wbfood_tips_value += f"{t:<{tip_len}}"
-                    if (i + 1) % new_wbfood_tips_len_sqrt == 0:
-                        new_wbfood_tips_value = (
-                            new_wbfood_tips_value.strip() + "\n"
+                new_wbfood_tips_col_count = new_wbfood_tips_len_sqrt
+
+                for col_index in range(0, new_wbfood_tips_col_count):
+                    col_values = [
+                        (i, new_wbfood_tips[i])
+                        for i in range(0, new_wbfood_tips_len)
+                        if i % new_wbfood_tips_col_count == col_index
+                    ]
+
+                    row_len = max(
+                        [
+                            len(v) + len([cc for cc in v if is_zh_CN_char(cc)])
+                            for i, v in col_values
+                        ]
+                    )+1
+                    for i, v in col_values:
+                        v_len = row_len - len(
+                            [c for c in v if is_zh_CN_char(c)]
                         )
+                        new_wbfood_tips[i] = f"{v:<{v_len}}"
+
+                for i, new_wbfood_tip in enumerate(new_wbfood_tips):
+                    if i % new_wbfood_tips_col_count == 0 and i != 0:
+                        new_wbfood_tips_value += "\n"
+                    new_wbfood_tips_value += new_wbfood_tip 
+
                 print_warning(new_wbfood_tips_value)
 
                 print_warning(_("Negligible foods are not listed."))
             else:
                 print_info(
                     _("There is no purchased food for {0}.").format(
                         tn1.strftime("%Y.%m.%d")
@@ -253,15 +270,19 @@
         print()
         print_error(_("Consuming days of {0}:").format(year_month))
         print_warning(f"{year_month:^{space_len*7}}")
         if consumption_days_value.endswith("\n"):
             consumption_days_value = consumption_days_value[:-1]
         print_info(consumption_days_value[:-1])
         consumption_days_len = len(consumption_days)
-        total_days =(_("{0} days in total.") if consumption_days_len > 1 else _("{0} day in total.")).format(consumption_days_len)
+        total_days = (
+            _("{0} days in total.")
+            if consumption_days_len > 1
+            else _("{0} day in total.")
+        ).format(consumption_days_len)
         print_warning(f"{total_days:^{space_len*7}}")
         print_info(_("Yes, they are all right. (Press any key to continue)"))
         input(">_")
         return
 
 
 # The end.
```

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/test.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/canteen/workbook.py` & `fnschool-20240516.2157.4/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/entry.py` & `fnschool-20240516.2157.4/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/external.py` & `fnschool-20240516.2157.4/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/fnprint.py` & `fnschool-20240516.2157.4/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/language.py` & `fnschool-20240516.2157.4/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240516.2157.4/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-16 19:40+0800\n"
-"PO-Revision-Date: 2024-05-16 19:40+0800\n"
+"POT-Creation-Date: 2024-05-16 21:56+0800\n"
+"PO-Revision-Date: 2024-05-16 21:56+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -583,14 +583,17 @@
 
 msgid "preconsuming"
 msgstr "预出库"
 
 msgid "values length is less than %s."
 msgstr "值的长度小于 %s 。"
 
+msgid "{0} day in total."
+msgstr "共 {0} 天。"
+
 msgid "{0} days in total."
 msgstr "共 {0} 天。"
 
 msgid ""
 "{0} need a purchasing list file, and it's file type should be '.xlsx'. The "
 "column names of it:"
 msgstr ""
```

### Comparing `fnschool-20240516.1949.11/src/fnschool/path.py` & `fnschool-20240516.2157.4/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool/test.py` & `fnschool-20240516.2157.4/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1949.11/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240516.2157.4/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240516.1949.11
+Version: 20240516.2157.4
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240516.1949.11/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240516.2157.4/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

