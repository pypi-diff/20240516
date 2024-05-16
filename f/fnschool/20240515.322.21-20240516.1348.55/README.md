# Comparing `tmp/fnschool-20240515.322.21.tar.gz` & `tmp/fnschool-20240516.1348.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240515.322.21.tar", last modified: Tue May 14 19:22:26 2024, max compression
+gzip compressed data, was "fnschool-20240516.1348.55.tar", last modified: Thu May 16 05:48:59 2024, max compression
```

## Comparing `fnschool-20240515.322.21.tar` & `fnschool-20240516.1348.55.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240515.322.21/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240515.322.21/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240515.322.21/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.300031 fnschool-20240515.322.21/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.306031 fnschool-20240515.322.21/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.313032 fnschool-20240515.322.21/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-14 16:35:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6303 2024-05-14 19:01:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/consume.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.315032 fnschool-20240515.322.21/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-14 18:35:22.000000 fnschool-20240515.322.21/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-14 18:45:28.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-14 17:46:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1862 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-14 17:12:30.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5695 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9357 2024-05-14 17:11:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8248 2024-05-14 18:51:12.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7193 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9722 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2286 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-14 18:25:45.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240515.322.21/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1298 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    17269 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.303031 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.777818 fnschool-20240516.1348.55/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240516.1348.55/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 05:48:59.776818 fnschool-20240516.1348.55/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240516.1348.55/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240516.1348.55/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-16 05:48:59.777818 fnschool-20240516.1348.55/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.755818 fnschool-20240516.1348.55/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.761818 fnschool-20240516.1348.55/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.768818 fnschool-20240516.1348.55/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7010 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240516.1348.55/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.769818 fnschool-20240516.1348.55/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240516.1348.55/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.773818 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1872 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1900 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8924 2024-05-16 04:56:25.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9404 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8268 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9222 2024-05-16 05:44:05.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2296 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240516.1348.55/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.773818 fnschool-20240516.1348.55/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240516.1348.55/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1302 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      776 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.756818 fnschool-20240516.1348.55/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.756818 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    17983 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.774818 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.757818 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-16 05:48:55.000000 fnschool-20240516.1348.55/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1611 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-16 04:52:14.000000 fnschool-20240516.1348.55/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-16 05:48:59.775818 fnschool-20240516.1348.55/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2184 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-16 05:48:59.000000 fnschool-20240516.1348.55/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240515.322.21/LICENSE` & `fnschool-20240516.1348.55/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/PKG-INFO` & `fnschool-20240516.1348.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240515.322.21
+Version: 20240516.1348.55
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240515.322.21/README.md` & `fnschool-20240516.1348.55/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/pyproject.toml` & `fnschool-20240516.1348.55/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/__init__.py` & `fnschool-20240516.1348.55/src/fnschool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import argparse
 from pathlib import Path
 
 import pandas as pd
 import numpy as np
 from openpyxl import load_workbook
 from fnschool.language import _
-from fnschool.log import *
+from fnschool.fnprint import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240515.0322.21"
+__version__ = "20240516.1348.55"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/bill.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/bill.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 import sys
 import calendar
 from fnschool import *
 
 from fnschool.canteen.spreadsheet.ctspreadsheet import *
 from fnschool.canteen.operator import *
 from fnschool.canteen.path import *
+from fnschool.canteen.currency import Currency
 
 
 class Bill:
     def __init__(self):
         self._spreadsheet = None
         self._foods = None
         self._time_nodes = None
         self._operator_name = None
         self._food_classes = None
         self._operator = None
+        self.currency = Currency().CNY
+        self._consuming_year = None
+        self._consuming_month = None
 
         print_app_name()
         pass
 
     def get_CNY_chars(self, value):
         format_word = [
             "分",
@@ -107,14 +111,31 @@
 
     @property
     def spreadsheet(self):
         if not self._spreadsheet:
             self._spreadsheet = CtSpreadSheet(self)
         return self._spreadsheet
 
+    def get_consuming_year(self,foods = None):
+        if not self._consuming_year:
+            foods = foods or self.foods
+            foods = sorted(foods, key=lambda f: f.xdate)
+            self._consuming_year = foods[-1].xdate.year
+        return self._consuming_year
+
+    def get_consuming_month(self,foods = None):
+        if not self._consuming_month:
+            foods = foods or self.foods
+            foods = sorted(foods, key=lambda f: f.xdate)
+            self._consuming_month = foods[-1].xdate.month
+        return self._consuming_month
+
+            
+        
+
     @property
     def foods(self):
         if not self._foods:
             self._foods = self.spreadsheet.purchasing.read_pfoods()
         return self._foods
 
     @property
@@ -136,16 +157,16 @@
         print_warning("\t" + _("Sponsor URL: {0}").format(get_sponsor_url()))
         print()
         pass
 
     @property
     def time_nodes(self):
         if not self._time_nodes:
-            year = self.foods[-1].xdate.year
-            month = self.foods[-1].xdate.month
+            year = self.get_consuming_year() 
+            month = self.get_consuming_month() 
             self._time_nodes = sorted(
                 list(
                     set(
                         [f.xdate for f in self.foods]
                         + [
                             datetime(
                                 year,
@@ -196,17 +217,15 @@
                     for name_like in name_likes:
                         if not name_like in user_name_likes:
                             user_name_likes.append(name_like)
                     self._food_classes[fclass] = user_name_likes
                 else:
                     self._food_classes[fclass] = name_likes
 
-            print_info(
-                _("Ok! I know it. (Press any key to continue)")
-            )
+            print_info(_("Ok! I know it. (Press any key to continue)"))
             input(">_ ")
 
         return self._food_classes
 
     @property
     def operator(self):
         if not self._operator:
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml` & `fnschool-20240516.1348.55/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/config.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from pathlib import Path
 import tomllib
 
 from fnschool.path import *
 from fnschool.canteen.path import *
-from fnschool.log import *
+from fnschool.fnprint import *
 from fnschool.external import *
 
 
 class Config:
     def __init__(self):
         self.user_config = None
         self.app_config = None
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240516.1348.55/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240516.1348.55/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240516.1348.55/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/food.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml` & `fnschool-20240516.1348.55/src/fnschool/canteen/food_classes.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "*米线",
     "*卷粉",
     "*圆粉",
     "*扁粉"
 ]
 "蛋奶及糕点类"=[
     "*蛋*!*蛋黄派*",
-    "*奶*!*奶香*",
+    "*奶*!*馒*",
 ]
 "油类"=[
     "*油*!*蚝油*!*花椒油*!*酱油*!*油麦菜*!*老干妈*",
 ]
 "调味类"=[
     "*葱*",
     "*姜*",
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/operator.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/path.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/profile.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import os
 import sys
-from fnschool.canteen.food import *
+from fnschool import *
 from fnschool.canteen.spreadsheet.base import *
 
 
-class ConsumingSum(SpreadsheetBase):
+class Cover(SpreadsheetBase):
     def __init__(self, bill):
         super().__init__(bill)
-        self.sheet_name = self.s.consumingsum_name
+        self.sheet_name = self.s.cover_name
         pass
 
     def update(self):
-        cssheet = self.sheet
-        year = self.bfoods[-1].xdate.year
-        month = self.bfoods[-1].xdate.month
+        year = self.bill.get_consuming_year() 
+        month = self.bill.get_consuming_month() 
         day = self.consuming_day_m1
-        foods = [f for f in self.bfoods if not f.is_abandoned]
 
+        cvsheet = self.sheet
+        cvsheet.cell(
+            1,
+            1,
+            self.purchaser + f"{year}年{month}月份食堂食品采购统计表",
+        )
+        foods = [f for f in self.bfoods if (not f.is_inventory)]
+        wfoods = [f for f in foods if not f.is_abandoned]
+        uwfoods = [f for f in foods if f.is_abandoned]
         total_price = 0.0
-        for row in cssheet.iter_rows(
-            min_row=4, max_row=10, min_col=1, max_col=3
+        for row in cvsheet.iter_rows(
+            min_row=3, max_row=9, min_col=1, max_col=3
         ):
             class_name = row[0].value.replace(" ", "")
             m_total_price = 0.0
-            for food in foods:
-                if food.fclass == class_name:
-                    m_total_price += sum(
-                        [
-                            _count * food.unit_price
-                            for _date, _count in food.consumptions
-                        ]
-                    )
+            for f in foods:
+                if f.fclass == class_name:
+                    m_total_price += f.count * f.unit_price
+            cvsheet.cell(row[0].row, 2, m_total_price)
+
             total_price += m_total_price
-            cssheet.cell(row[0].row, 2, m_total_price)
-            cssheet.cell(row[0].row, 2).number_format = (
-                numbers.FORMAT_NUMBER_00
-            )
-
-        total_price_CNY = self.bill.get_CNY_chars(total_price)
-        cssheet.cell(
-            2,
-            1,
-            f"编制单位：{self.purchaser}       "
-            + f"单位：元         "
-            + f"{year}年{month}月{day}日",
+        cvsheet.cell(10, 2, total_price)
+
+        w_seasoning_total_price = sum(
+            [f.count * f.unit_price for f in wfoods if ("调味" in f.fclass)]
         )
-        cssheet.cell(
-            11,
-            1,
-            (f"总金额（大写)：{total_price_CNY}    " + f"¥{total_price:.2f}"),
+        unw_seasoning_total_price = sum(
+            [f.count * f.unit_price for f in uwfoods if ("调味" in f.fclass)]
+        )
+
+        for row_index in range(3, 11):
+            cvsheet.cell(row_index, 3, "")
+
+        cvsheet.cell(
+            8,
+            3,
+            f"入库：{w_seasoning_total_price:.2f}元；"
+            + f"未入库：{unw_seasoning_total_price:.2f}元",
         )
-        cssheet.cell(12, 1, f"经办人：{self.operator.name}  ")
 
         wb = self.bwb
-        wb.active = cssheet
+        wb.active = cvsheet
 
         print_info(_("Sheet '%s' was updated.") % self.sheet.title)
 
 
 # The end.
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 25% similar despite different names*

```diff
@@ -166,27 +166,132 @@
                     + "to food sheets, they will be saved "
                     + "for next updating."
                 )
             )
         else:
             self.bwb.save(bill_fpath0)
 
+        print_info(
+            _('Updated data has been saved to "{0}".').format(bill_fpath0)
+        )
+
         open_file(bill_fpath0)
 
         print_info(_("Updated data was saved."))
 
+    def print_summary(self, foods=None):
+        bfoods = foods or self.bill.foods
+        cfoods = [f for f in bfoods if not f.is_abandoned]
+        currency_mark = self.bill.currency.mark
+        summary = []
+        summary_len = 0
+        inventory_mm1 = sum([f.total_price for f in cfoods if f.is_inventory])
+        inventory_mm1 = (
+            _("Inventory of last month: ") + currency_mark + str(inventory_mm1)
+        )
+
+        warehousing_m = sum(
+            [f.total_price for f in cfoods if not f.is_inventory]
+        )
+        warehousing_m_cp = warehousing_m
+        warehousing_m = (
+            _("Warehousing of this month: ")
+            + currency_mark
+            + str(warehousing_m)
+        )
+        inventory_mm1_warehousing_m = (
+            _("Total: ")
+            + currency_mark
+            + str(sum([f.total_price for f in cfoods]))
+        )
+        consuming_m = 0
+        for f in cfoods:
+            f_consuming_m = sum([c for __, c in f.consumptions])
+            consuming_m += f_consuming_m * f.unit_price
+
+        consuming_m_cp = consuming_m
+        consuming_m = (
+            _("Consuming of this month: ") + currency_mark + str(consuming_m)
+        )
+
+        month_day_m1 = sorted([f.xdate for f in cfoods])[0]
+        for f in cfoods:
+            month_day_m1 = max(
+                [d for d, __ in f.consumptions] + [month_day_m1]
+            )
+
+        inventory_m = sum(
+            [
+                f.get_remainder(month_day_m1) * f.unit_price
+                for f in cfoods
+                if f.get_remainder(month_day_m1) > 0
+            ]
+        )
+        inventory_m_cp = inventory_m
+        inventory_m = (
+            _("Inventory of this month: ") + currency_mark + str(inventory_m)
+        )
+
+        consuming_m_inventory_m = (
+            _("Total: ") + currency_mark + str(consuming_m_cp + inventory_m_cp)
+        )
+
+        afoods = [f for f in bfoods if f.is_abandoned]
+        unwarehousing_m = (
+            _("Unwarehousing of this month: ")
+            + currency_mark
+            + str(sum([f.total_price for f in afoods]))
+        )
+
+        total_purchasing_m = (
+            _("Total purchasing of this month: ")
+            + currency_mark
+            + str(sum([f.total_price for f in bfoods if not f.is_inventory]))
+        )
+        summary = [
+            inventory_mm1,
+            warehousing_m,
+            inventory_mm1_warehousing_m,
+            consuming_m,
+            inventory_m,
+            consuming_m_inventory_m,
+            warehousing_m,
+            unwarehousing_m,
+            total_purchasing_m,
+        ]
+
+        summary_len = max([len(s)+len([c for c in s if is_zh_CN_char(c)]) for s in summary])
+        summary_sep = "-" * summary_len
+        summary = (
+            [summary_sep]
+            + summary[:3]
+            + [summary_sep]
+            + summary[3:6]
+            + [summary_sep]
+            + summary[6:]
+            + [summary_sep]
+        )
+        summary = "\n".join(summary)
+        print()
+        print_error(_("Summary:"))
+        print_info(summary)
+        print()
+
     def update(self):
+
         self.inventory.update()
         self.warehousing.update()
         self.unwarehousing.update()
         self.consuming.update()
         self.sfood.update()
         self.purchasingsum.update()
         self.consumingsum.update()
         self.cover.update()
 
+        self.print_summary()
+
         self.save_workbook()
 
         print_info(_("Update completely!"))
 
 
 # The end.
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/food.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         print_info(
             _("Sheet {0} has been reformatted.").format(self.sheet.title)
         )
 
     def get_form_index(self, sheet):
         indexes = self.get_form_indexes(sheet)
-        index_range = indexes[self.bfoods[-1].xdate.month - 1]
+        index_range = indexes[self.bill.get_consuming_month()  - 1]
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
 
-        year = self.bfoods[-1].xdate.year
-        month = self.bfoods[-1].xdate.month
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
 
-                    if food.xdate == cdate:
+                    if (food.xdate == cdate and food.xdate.month == month):
                         sheet.cell(row_index, 1, cdate.month)
                         sheet.cell(row_index, 2, cdate.day)
                         sheet.cell(row_index, 4, food.count)
                         sheet.cell(row_index, 5, food.unit_price)
                         sheet.cell(row_index, 6, food.count * food.unit_price)
                         sheet.cell(row_index, 9, "")
                         sheet.cell(row_index, 10, food.count)
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         return None
 
     @property
     def foods(self):
         foods = []
         bfoods = [f for f in self.bfoods if not f.is_abandoned]
-        year = bfoods[-1].xdate.year
-        month = bfoods[-1].xdate.month
+        year = self.bill.get_consuming_year() 
+        month = self.bill.get_consuming_month() 
 
         consuming_dates = []
         for bfood in bfoods:
             for d, __ in bfood.consumptions:
                 consuming_dates.append(d)
         consuming_dates = list(set(consuming_dates))
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,9 +258,10 @@
             if self.inventory_col_name:
                 _food.is_inventory = not pd.isna(food[self.inventory_col_name])
             _foods.append(_food)
 
         foods = _foods
         foods = sorted(foods, key=lambda f: f.xdate)
         self.spreadsheet.preconsuming.pre_consume_foods(foods)
+
         return foods
         pass
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         super().__init__(bill)
         self.sheet_name = self.s.purchasingsum_name
         pass
 
     def update(self):
 
         pssheet = self.sheet
-        year = self.bfoods[-1].xdate.year
-        month = self.bfoods[-1].xdate.month
+        year = self.bill.get_consuming_year() 
+        month = self.bill.get_consuming_month() 
         day = self.consuming_day_m1
 
         pssheet.cell(
             2,
             1,
             f"编制单位：{self.purchaser}"
             + f"        "
```

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/test.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/canteen/workbook.py` & `fnschool-20240516.1348.55/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/entry.py` & `fnschool-20240516.1348.55/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/external.py` & `fnschool-20240516.1348.55/src/fnschool/external.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import subprocess
 
 from fnschool.language import *
-from fnschool.log import *
+from fnschool.fnprint import *
 from fnschool.path import *
 
 
 def sys_is_linux():
     return "inux" in sys.platform
```

### Comparing `fnschool-20240515.322.21/src/fnschool/language.py` & `fnschool-20240516.1348.55/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240516.1348.55/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-15 03:02+0800\n"
-"PO-Revision-Date: 2024-05-15 03:02+0800\n"
+"POT-Creation-Date: 2024-05-16 13:44+0800\n"
+"PO-Revision-Date: 2024-05-16 13:44+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -64,17 +64,23 @@
 
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
 msgstr "配置文件 “%s” 被复制到 “%s” 。"
 
+msgid "Consuming days of {0}:"
+msgstr "{0} 的出库日期："
+
 msgid "Consuming days:"
 msgstr "耗材日期："
 
+msgid "Consuming of this month: "
+msgstr "本月出库："
+
 msgid "Consuming records:"
 msgstr "消耗记录："
 
 msgid "Consumptions were read."
 msgstr "每日食材消耗已被读取。"
 
 msgid "Copying workbook..."
@@ -191,14 +197,20 @@
 msgstr "如果您觉得 {0} 项目很棒，请您赞助它。您的赞助会让项目继续活下去。"
 
 msgid ""
 "If you save updated data to \"{0}\", data of food sheets will be saved for "
 "every month."
 msgstr "如果您把已更新的数据保存到 “{0}”，那每个月的食材台账表都会被保存下来。"
 
+msgid "Inventory of last month: "
+msgstr "上月盘存："
+
+msgid "Inventory of this month: "
+msgstr "本月盘存："
+
 msgid "Is neglibible"
 msgstr "非入库食材"
 
 msgid "Is residue"
 msgstr "是库存食材"
 
 msgid ""
@@ -386,14 +398,17 @@
 
 msgid "Spreadsheet Files"
 msgstr "工作簿文件。"
 
 msgid "Spreadsheet {0} was copied to {1} ."
 msgstr "工作簿 “{0}” 被复制到 “{1}” 。"
 
+msgid "Summary:"
+msgstr "汇总："
+
 msgid "Supplier name 1"
 msgstr "供应商1"
 
 msgid "Supplier name 2"
 msgstr "供应商2"
 
 msgid "Suppliers:"
@@ -472,33 +487,48 @@
 "盘存食材的以下信息需要被添加：\n"
 "\t1、盘存时间：食材的盘存时间。\n"
 "\t2、组织名 或 学校名。\n"
 "\t3、食材名。\n"
 "\t4、食材数量，如果您的表格有多个数量列，把所有数量列都填上。\n"
 "\t5、食材总价。"
 
+msgid "Total purchasing of this month: "
+msgstr "本月总购入："
+
+msgid "Total: "
+msgstr "总计："
+
 msgid "Unable to find food name column, exitt."
 msgstr "未找到食材名称列，退出。"
 
 msgid ""
 "Unable to find {0} from {1}, You can input it (1 base) directly or give "
 "feedback to the maintainers --> {2} ."
 msgstr ""
 "从 {1} 中未找到 {0} ，您可以直接输入它（以1开始）或这给项目维护人员反馈 —> "
 "{2} 。"
 
 msgid "Unexpected input was got."
 msgstr "获取异常输入。"
 
+msgid "Unwarehousing of this month: "
+msgstr "本月未入库："
+
 msgid "Update completely!"
 msgstr "更新完成！"
 
+msgid "Updated data has been saved to \"{0}\"."
+msgstr "更新的数据已被保存到 “{0}”。"
+
 msgid "Updated data was saved."
 msgstr "被更改的数据已保存。"
 
+msgid "Warehousing of this month: "
+msgstr "本月入库："
+
 msgid "Workbook %s was read."
 msgstr "已读取 工作簿 “%s” 。"
 
 msgid "Workbook '%s' has been used."
 msgstr "使用工作薄 “%s” 。"
 
 msgid "Workbook '%s' was saved."
@@ -514,14 +544,17 @@
 "Workbook '{0}' was updated, please design the daily foods consumption and "
 "press ANY key to continue."
 msgstr "工作簿 “{0}” 已更新，请设计每天的食材消耗然后按任意键继续。"
 
 msgid "Workbook {0} doesn't exist."
 msgstr "工作簿 {0} 不存在。"
 
+msgid "Yes, they are all right. (Press any key to continue)"
+msgstr "是的，都是对的。（按任意键继续）"
+
 msgid ""
 "You can fill in the monthly missing data to food sheets, they will be saved "
 "for next updating."
 msgstr ""
 "您可以把 食材台账表 里面没有更新的月份的数据更新了，这些数据会被保存下来的。"
 
 msgid "Your food classes were read from \"{0}\". It will be used first."
```

### Comparing `fnschool-20240515.322.21/src/fnschool/path.py` & `fnschool-20240516.1348.55/src/fnschool/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path, PosixPath
 import shutil
 import getpass
 import platform
 import subprocess
 
 from appdirs import AppDirs
-from fnschool.log import *
+from fnschool.fnprint import *
 from fnschool.app import *
 
 
 user_name = getpass.getuser()
 
 dirs = AppDirs(app_name, app_author)
```

### Comparing `fnschool-20240515.322.21/src/fnschool/test.py` & `fnschool-20240516.1348.55/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240516.1348.55/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240515.322.21
+Version: 20240516.1348.55
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240516.1348.55/src/fnschool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 README.md
 pyproject.toml
 src/fnschool/__init__.py
 src/fnschool/__main__.py
 src/fnschool/app.py
 src/fnschool/entry.py
 src/fnschool/external.py
+src/fnschool/fnprint.py
 src/fnschool/language.py
-src/fnschool/log.py
 src/fnschool/path.py
 src/fnschool/test.py
 src/fnschool.egg-info/PKG-INFO
 src/fnschool.egg-info/SOURCES.txt
 src/fnschool.egg-info/dependency_links.txt
 src/fnschool.egg-info/entry_points.txt
 src/fnschool.egg-info/requires.txt
@@ -19,14 +19,15 @@
 src/fnschool/canteen/__init__.py
 src/fnschool/canteen/__main__.py
 src/fnschool/canteen/bill.cp.py
 src/fnschool/canteen/bill.py
 src/fnschool/canteen/canteen.toml
 src/fnschool/canteen/config.py
 src/fnschool/canteen/consume.py
+src/fnschool/canteen/currency.py
 src/fnschool/canteen/food.cp.py
 src/fnschool/canteen/food.py
 src/fnschool/canteen/food_classes.toml
 src/fnschool/canteen/food_recount.toml
 src/fnschool/canteen/food_recounts.toml
 src/fnschool/canteen/operator.py
 src/fnschool/canteen/path.py
```

