# Comparing `tmp/fnschool-20240516.1348.55.tar.gz` & `tmp/fnschool-20240516.1947.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240516.1348.55.tar", last modified: Thu May 16 05:48:59 2024, max compression
+gzip compressed data, was "fnschool-20240516.1947.26.tar", last modified: Thu May 16 11:47:31 2024, max compression
```

## Comparing `fnschool-20240516.1348.55.tar` & `fnschool-20240516.1947.26.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.777818 fnschool-20240516.1348.55/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240516.1348.55/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 05:48:59.776818 fnschool-20240516.1348.55/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240516.1348.55/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240516.1348.55/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 05:48:59.777818 fnschool-20240516.1348.55/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.755818 fnschool-20240516.1348.55/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.761818 fnschool-20240516.1348.55/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.768818 fnschool-20240516.1348.55/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7010 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240516.1348.55/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.769818 fnschool-20240516.1348.55/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.773818 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1872 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1900 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8924 2024-05-16 04:56:25.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9404 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8268 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9222 2024-05-16 05:44:05.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2296 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.773818 fnschool-20240516.1348.55/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240516.1348.55/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.756818 fnschool-20240516.1348.55/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.756818 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    17983 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2184 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.038534 fnschool-20240516.1947.26/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240516.1947.26/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 11:47:31.038534 fnschool-20240516.1947.26/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240516.1947.26/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240516.1947.26/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 11:47:31.039533 fnschool-20240516.1947.26/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.016533 fnschool-20240516.1947.26/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.022534 fnschool-20240516.1947.26/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.030533 fnschool-20240516.1947.26/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6983 2024-05-16 06:04:05.000000 fnschool-20240516.1947.26/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240516.1947.26/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.031534 fnschool-20240516.1947.26/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240516.1947.26/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240516.1947.26/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240516.1947.26/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240516.1947.26/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1947.26/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1947.26/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.035534 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1870 2024-05-16 06:04:05.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1898 2024-05-16 06:04:05.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8948 2024-05-16 06:04:05.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9399 2024-05-16 06:04:06.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8266 2024-05-16 06:04:05.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9722 2024-05-16 11:41:38.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2294 2024-05-16 06:04:06.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1947.26/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.035534 fnschool-20240516.1947.26/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240516.1947.26/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.019533 fnschool-20240516.1947.26/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.017533 fnschool-20240516.1947.26/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.036533 fnschool-20240516.1947.26/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.018533 fnschool-20240516.1947.26/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.036533 fnschool-20240516.1947.26/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18033 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.018533 fnschool-20240516.1947.26/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.036533 fnschool-20240516.1947.26/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.019533 fnschool-20240516.1947.26/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.037533 fnschool-20240516.1947.26/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.019533 fnschool-20240516.1947.26/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.037533 fnschool-20240516.1947.26/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 11:47:26.000000 fnschool-20240516.1947.26/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 04:52:14.000000 fnschool-20240516.1947.26/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 11:47:31.037533 fnschool-20240516.1947.26/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 11:47:30.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2184 2024-05-16 11:47:31.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 11:47:30.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 11:47:30.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 11:47:30.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 11:47:30.000000 fnschool-20240516.1947.26/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240516.1348.55/LICENSE` & `fnschool-20240516.1947.26/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/PKG-INFO` & `fnschool-20240516.1947.26/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240516.1348.55
+Version: 20240516.1947.26
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240516.1348.55/README.md` & `fnschool-20240516.1947.26/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/pyproject.toml` & `fnschool-20240516.1947.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/__init__.py` & `fnschool-20240516.1947.26/src/fnschool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.fnprint import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240516.1348.55"
+__version__ = "20240516.1947.26"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/bill.cp.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/bill.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/bill.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,31 +111,28 @@
 
     @property
     def spreadsheet(self):
         if not self._spreadsheet:
             self._spreadsheet = CtSpreadSheet(self)
         return self._spreadsheet
 
-    def get_consuming_year(self,foods = None):
+    def get_consuming_year(self, foods=None):
         if not self._consuming_year:
             foods = foods or self.foods
             foods = sorted(foods, key=lambda f: f.xdate)
             self._consuming_year = foods[-1].xdate.year
         return self._consuming_year
 
-    def get_consuming_month(self,foods = None):
+    def get_consuming_month(self, foods=None):
         if not self._consuming_month:
             foods = foods or self.foods
             foods = sorted(foods, key=lambda f: f.xdate)
             self._consuming_month = foods[-1].xdate.month
         return self._consuming_month
 
-            
-        
-
     @property
     def foods(self):
         if not self._foods:
             self._foods = self.spreadsheet.purchasing.read_pfoods()
         return self._foods
 
     @property
@@ -157,16 +154,16 @@
         print_warning("\t" + _("Sponsor URL: {0}").format(get_sponsor_url()))
         print()
         pass
 
     @property
     def time_nodes(self):
         if not self._time_nodes:
-            year = self.get_consuming_year() 
-            month = self.get_consuming_month() 
+            year = self.get_consuming_year()
+            month = self.get_consuming_month()
             self._time_nodes = sorted(
                 list(
                     set(
                         [f.xdate for f in self.foods]
                         + [
                             datetime(
                                 year,
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/canteen.toml` & `fnschool-20240516.1947.26/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/config.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240516.1947.26/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240516.1947.26/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240516.1947.26/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/food.cp.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/food.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/food_classes.toml` & `fnschool-20240516.1947.26/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/operator.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/path.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/profile.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def __init__(self, bill):
         super().__init__(bill)
         self.sheet_name = self.s.consumingsum_name
         pass
 
     def update(self):
         cssheet = self.sheet
-        year = self.bill.get_consuming_year() 
-        month = self.bill.get_consuming_month() 
+        year = self.bill.get_consuming_year()
+        month = self.bill.get_consuming_month()
         day = self.consuming_day_m1
         foods = [f for f in self.bfoods if not f.is_abandoned]
 
         total_price = 0.0
         for row in cssheet.iter_rows(
             min_row=4, max_row=10, min_col=1, max_col=3
         ):
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 class Cover(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
         self.sheet_name = self.s.cover_name
         pass
 
     def update(self):
-        year = self.bill.get_consuming_year() 
-        month = self.bill.get_consuming_month() 
+        year = self.bill.get_consuming_year()
+        month = self.bill.get_consuming_month()
         day = self.consuming_day_m1
 
         cvsheet = self.sheet
         cvsheet.cell(
             1,
             1,
             self.purchaser + f"{year}年{month}月份食堂食品采购统计表",
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,17 @@
             inventory_m,
             consuming_m_inventory_m,
             warehousing_m,
             unwarehousing_m,
             total_purchasing_m,
         ]
 
-        summary_len = max([len(s)+len([c for c in s if is_zh_CN_char(c)]) for s in summary])
+        summary_len = max(
+            [len(s) + len([c for c in s if is_zh_CN_char(c)]) for s in summary]
+        )
         summary_sep = "-" * summary_len
         summary = (
             [summary_sep]
             + summary[:3]
             + [summary_sep]
             + summary[3:6]
             + [summary_sep]
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/food.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         print_info(
             _("Sheet {0} has been reformatted.").format(self.sheet.title)
         )
 
     def get_form_index(self, sheet):
         indexes = self.get_form_indexes(sheet)
-        index_range = indexes[self.bill.get_consuming_month()  - 1]
+        index_range = indexes[self.bill.get_consuming_month() - 1]
         return index_range
 
     def get_form_indexes(self, sheet):
         indexes = []
         for row in sheet.iter_rows(
             min_row=1, max_row=sheet.max_row, min_col=1, max_col=14
         ):
@@ -110,16 +110,16 @@
 
             if row[2].value and "合计" in str(row[2].value).replace(" ", ""):
                 indexes[-1][1] = row[0].row + 1
         return indexes
 
     def update(self):
 
-        year = self.bill.get_consuming_year() 
-        month = self.bill.get_consuming_month() 
+        year = self.bill.get_consuming_year()
+        month = self.bill.get_consuming_month()
         cfoods = [f for f in self.bfoods if not f.is_abandoned]
         food_names = list(set([f.name for f in cfoods]))
         wb = self.bwb
 
         rfoods = [
             f for f in self.bfoods if (not f.is_abandoned and f.is_inventory)
         ]
@@ -176,15 +176,15 @@
             cdates = sorted(list(set(cdates)))
 
             consuming_n = 1
             warehousing_n = 1
             for cdate in cdates:
                 for food in m_cfoods:
 
-                    if (food.xdate == cdate and food.xdate.month == month):
+                    if food.xdate == cdate and food.xdate.month == month:
                         sheet.cell(row_index, 1, cdate.month)
                         sheet.cell(row_index, 2, cdate.day)
                         sheet.cell(row_index, 4, food.count)
                         sheet.cell(row_index, 5, food.unit_price)
                         sheet.cell(row_index, 6, food.count * food.unit_price)
                         sheet.cell(row_index, 9, "")
                         sheet.cell(row_index, 10, food.count)
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         return None
 
     @property
     def foods(self):
         foods = []
         bfoods = [f for f in self.bfoods if not f.is_abandoned]
-        year = self.bill.get_consuming_year() 
-        month = self.bill.get_consuming_month() 
+        year = self.bill.get_consuming_year()
+        month = self.bill.get_consuming_month()
 
         consuming_dates = []
         for bfood in bfoods:
             for d, __ in bfood.consumptions:
                 consuming_dates.append(d)
         consuming_dates = list(set(consuming_dates))
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         self.sheet_name0 = self.s.preconsuming_name0
 
     def pre_consume_foods(self, foods):
         cfoods = [f for f in foods if not f.is_abandoned]
         if len(cfoods) < 1:
             print_error(_("No food found, exit."))
             exit()
-        year = self.bill.get_consuming_year(foods) 
-        month = self.bill.get_consuming_month(foods) 
+        year = self.bill.get_consuming_year(foods)
+        month = self.bill.get_consuming_month(foods)
         residual_mark = _("(Remaining)")
         time_nodes = sorted(
             list(
                 set(
                     [f.xdate for f in cfoods]
                     + [
                         datetime(
@@ -148,26 +148,33 @@
                 new_wbfood_tips = [
                     f"({i+1}){f.name} {f.count} {f.unit_name}"
                     for i, f in enumerate(new_wbfoods)
                 ]
                 new_wbfood_tips_len_sqrt = math.ceil(
                     len(new_wbfood_tips) ** 0.5
                 )
-                new_wbfood_tip_len = max(
-                    [
-                        len(t) + len([c for c in t if is_zh_CN_char(c)])
-                        for t in new_wbfood_tips
-                    ]
-                )+1
+                new_wbfood_tip_len = (
+                    max(
+                        [
+                            len(t) + len([c for c in t if is_zh_CN_char(c)])
+                            for t in new_wbfood_tips
+                        ]
+                    )
+                    + 1
+                )
                 new_wbfood_tips_value = ""
                 for i, t in enumerate(new_wbfood_tips):
-                    tip_len = new_wbfood_tip_len - len([c for c in t if is_zh_CN_char(c)])
+                    tip_len = new_wbfood_tip_len - len(
+                        [c for c in t if is_zh_CN_char(c)]
+                    )
                     new_wbfood_tips_value += f"{t:<{tip_len}}"
                     if (i + 1) % new_wbfood_tips_len_sqrt == 0:
-                        new_wbfood_tips_value = new_wbfood_tips_value.strip() + "\n"
+                        new_wbfood_tips_value = (
+                            new_wbfood_tips_value.strip() + "\n"
+                        )
                 print_warning(new_wbfood_tips_value)
 
                 print_warning(_("Negligible foods are not listed."))
             else:
                 print_info(
                     _("There is no purchased food for {0}.").format(
                         tn1.strftime("%Y.%m.%d")
@@ -216,44 +223,45 @@
                     col_index += 1
                 f_index += 1
             wb.close()
             sheet = None
         self.print_consuming_days(cfoods)
         pass
 
-    def print_consuming_days(self,foods):
+    def print_consuming_days(self, foods):
         consumption_days = []
-        year =  self.bill.get_consuming_year(foods)
+        year = self.bill.get_consuming_year(foods)
         month = self.bill.get_consuming_month(foods)
-        year_month = f"{year}.{month}"
+        year_month = f"{year}.{month:0>2}"
 
         for f in foods:
-            for d,c in f.consumptions:
-                if not d in consumption_days:
+            for d, c in f.consumptions:
+                if not d.day in consumption_days:
                     consumption_days.append(d.day)
         consumption_days_value = ""
         space_len = 5
-        for week in calendar.monthcalendar(
-           year,month        ):
+        for week in calendar.monthcalendar(year, month):
             for d in week:
                 if d == 0:
-                    consumption_days_value += " "*space_len
+                    consumption_days_value += " " * space_len
                 elif d in consumption_days:
                     consumption_day = f"({d})"
                     consumption_days_value += f"{consumption_day:>{space_len}}"
                 else:
                     consumption_days_value += f"{d:>{space_len}}"
             consumption_days_value += "\n"
-        
+
         print()
-        print_error(
-            _("Consuming days of {0}:").format(year_month)
-        )
+        print_error(_("Consuming days of {0}:").format(year_month))
         print_warning(f"{year_month:^{space_len*7}}")
-        print_info(consumption_days_value)
+        if consumption_days_value.endswith("\n"):
+            consumption_days_value = consumption_days_value[:-1]
+        print_info(consumption_days_value[:-1])
+        consumption_days_len = len(consumption_days)
+        total_days =(_("{0} days in total.") if consumption_days_len > 1 else _("{0} day in total.")).format(consumption_days_len)
+        print_warning(f"{total_days:^{space_len*7}}")
         print_info(_("Yes, they are all right. (Press any key to continue)"))
         input(">_")
-        return 
-
+        return
 
 
 # The end.
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         super().__init__(bill)
         self.sheet_name = self.s.purchasingsum_name
         pass
 
     def update(self):
 
         pssheet = self.sheet
-        year = self.bill.get_consuming_year() 
-        month = self.bill.get_consuming_month() 
+        year = self.bill.get_consuming_year()
+        month = self.bill.get_consuming_month()
         day = self.consuming_day_m1
 
         pssheet.cell(
             2,
             1,
             f"编制单位：{self.purchaser}"
             + f"        "
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/test.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/canteen/workbook.py` & `fnschool-20240516.1947.26/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/entry.py` & `fnschool-20240516.1947.26/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/external.py` & `fnschool-20240516.1947.26/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/fnprint.py` & `fnschool-20240516.1947.26/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/language.py` & `fnschool-20240516.1947.26/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240516.1947.26/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-16 13:44+0800\n"
-"PO-Revision-Date: 2024-05-16 13:44+0800\n"
+"POT-Creation-Date: 2024-05-16 19:40+0800\n"
+"PO-Revision-Date: 2024-05-16 19:40+0800\n"
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
 
+msgid "{0} days in total."
+msgstr "共 {0} 天。"
+
 msgid ""
 "{0} need a purchasing list file, and it's file type should be '.xlsx'. The "
 "column names of it:"
 msgstr ""
 "{0} 需要一个购入食材的列表文件，这个列表文件的类型应为 “.xlsx”。它的列（表"
 "头）为："
```

### Comparing `fnschool-20240516.1348.55/src/fnschool/path.py` & `fnschool-20240516.1947.26/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool/test.py` & `fnschool-20240516.1947.26/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240516.1348.55/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240516.1947.26/src/fnschool.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240516.1348.55
+Version: 20240516.1947.26
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240516.1348.55/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240516.1947.26/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

