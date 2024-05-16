# Comparing `tmp/fnschool-20240515.1802.50.tar.gz` & `tmp/fnschool-20240515.322.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240515.1802.50.tar", last modified: Wed May 15 10:02:55 2024, max compression
+gzip compressed data, was "fnschool-20240515.322.21.tar", last modified: Tue May 14 19:22:26 2024, max compression
```

## Comparing `fnschool-20240515.1802.50.tar` & `fnschool-20240515.322.21.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.702884 fnschool-20240515.1802.50/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240515.1802.50/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-15 10:02:55.702884 fnschool-20240515.1802.50/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240515.1802.50/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240515.1802.50/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-15 10:02:55.702884 fnschool-20240515.1802.50/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.675886 fnschool-20240515.1802.50/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.681886 fnschool-20240515.1802.50/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.690885 fnschool-20240515.1802.50/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-14 16:35:32.000000 fnschool-20240515.1802.50/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6359 2024-05-15 02:50:24.000000 fnschool-20240515.1802.50/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240515.1802.50/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      268 2024-05-15 01:57:27.000000 fnschool-20240515.1802.50/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.692885 fnschool-20240515.1802.50/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240515.1802.50/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240515.1802.50/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240515.1802.50/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240515.1802.50/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.1802.50/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.1802.50/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-14 18:35:22.000000 fnschool-20240515.1802.50/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-14 18:25:37.000000 fnschool-20240515.1802.50/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-14 18:25:37.000000 fnschool-20240515.1802.50/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.698884 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 18:25:37.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-14 18:45:28.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-14 17:46:32.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1862 2024-05-14 18:25:37.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-14 17:12:30.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8827 2024-05-15 09:58:44.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9357 2024-05-14 17:11:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     8248 2024-05-14 18:51:12.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     7636 2024-05-15 09:52:14.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9723 2024-05-15 01:20:53.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2286 2024-05-14 18:25:38.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-14 18:25:38.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-14 18:25:39.000000 fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-14 18:25:45.000000 fnschool-20240515.1802.50/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.1802.50/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.699884 fnschool-20240515.1802.50/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240515.1802.50/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1298 2024-05-14 18:25:39.000000 fnschool-20240515.1802.50/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.678886 fnschool-20240515.1802.50/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.676886 fnschool-20240515.1802.50/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.699884 fnschool-20240515.1802.50/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.677886 fnschool-20240515.1802.50/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.699884 fnschool-20240515.1802.50/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    17803 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.677886 fnschool-20240515.1802.50/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.700884 fnschool-20240515.1802.50/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.677886 fnschool-20240515.1802.50/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.700884 fnschool-20240515.1802.50/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.678886 fnschool-20240515.1802.50/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.700884 fnschool-20240515.1802.50/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-15 10:02:50.000000 fnschool-20240515.1802.50/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-14 16:34:25.000000 fnschool-20240515.1802.50/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-15 10:02:55.701884 fnschool-20240515.1802.50/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12296 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2180 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-15 10:02:55.000000 fnschool-20240515.1802.50/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240515.322.21/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240515.322.21/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240515.322.21/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-14 19:22:26.322032 fnschool-20240515.322.21/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.300031 fnschool-20240515.322.21/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.306031 fnschool-20240515.322.21/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      862 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.313032 fnschool-20240515.322.21/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-14 16:35:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6303 2024-05-14 19:01:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/consume.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.315032 fnschool-20240515.322.21/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255719 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1641 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      886 2024-05-14 13:17:04.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3211 2024-05-14 18:35:22.000000 fnschool-20240515.322.21/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1250 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-14 18:45:28.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10371 2024-05-14 17:46:32.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1862 2024-05-14 18:25:37.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1890 2024-05-14 17:12:30.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5695 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9357 2024-05-14 17:11:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     8248 2024-05-14 18:51:12.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7193 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9722 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2286 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4556 2024-05-14 18:25:38.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-14 18:25:45.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240515.322.21/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240515.322.21/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1017 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1298 2024-05-14 18:25:39.000000 fnschool-20240515.322.21/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.319032 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.301031 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    17269 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.302031 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.320032 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.303031 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-14 19:22:21.000000 fnschool-20240515.322.21/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      586 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1607 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-14 16:34:25.000000 fnschool-20240515.322.21/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-14 19:22:26.321032 fnschool-20240515.322.21/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12295 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2147 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-14 19:22:26.000000 fnschool-20240515.322.21/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240515.1802.50/LICENSE` & `fnschool-20240515.322.21/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/PKG-INFO` & `fnschool-20240515.322.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240515.1802.50
+Version: 20240515.322.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240515.1802.50/README.md` & `fnschool-20240515.322.21/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/pyproject.toml` & `fnschool-20240515.322.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/__init__.py` & `fnschool-20240515.322.21/src/fnschool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openpyxl import load_workbook
 from fnschool.language import _
 from fnschool.log import *
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 
-__version__ = "20240515.1802.50"
+__version__ = "20240515.0322.21"
 
 
 def print_app_name():
     app_name0 = [
         r" _____ _   _ ____   ____ _   _  ___   ___  _     ",
         r"|  ___| \ | / ___| / ___| | | |/ _ \ / _ \| |    ",
         r"| |_  |  \| \___ \| |   | |_| | | | | | | | |    ",
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/bill.cp.py` & `fnschool-20240515.322.21/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/bill.py` & `fnschool-20240515.322.21/src/fnschool/canteen/bill.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 import sys
 import calendar
 from fnschool import *
 
 from fnschool.canteen.spreadsheet.ctspreadsheet import *
 from fnschool.canteen.operator import *
 from fnschool.canteen.path import *
-from fnschool.canteen.currency import Currency
 
 
 class Bill:
     def __init__(self):
         self._spreadsheet = None
         self._foods = None
         self._time_nodes = None
         self._operator_name = None
         self._food_classes = None
         self._operator = None
-        self.currency = Currency().CNY
 
         print_app_name()
         pass
 
     def get_CNY_chars(self, value):
         format_word = [
             "分",
@@ -198,15 +196,17 @@
                     for name_like in name_likes:
                         if not name_like in user_name_likes:
                             user_name_likes.append(name_like)
                     self._food_classes[fclass] = user_name_likes
                 else:
                     self._food_classes[fclass] = name_likes
 
-            print_info(_("Ok! I know it. (Press any key to continue)"))
+            print_info(
+                _("Ok! I know it. (Press any key to continue)")
+            )
             input(">_ ")
 
         return self._food_classes
 
     @property
     def operator(self):
         if not self._operator:
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/canteen.toml` & `fnschool-20240515.322.21/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/config.py` & `fnschool-20240515.322.21/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240515.322.21/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/food.cp.py` & `fnschool-20240515.322.21/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/food.py` & `fnschool-20240515.322.21/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/food_classes.toml` & `fnschool-20240515.322.21/src/fnschool/canteen/food_classes.toml`

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
-    "*奶*!*馒*",
+    "*奶*!*奶香*",
 ]
 "油类"=[
     "*油*!*蚝油*!*花椒油*!*酱油*!*油麦菜*!*老干妈*",
 ]
 "调味类"=[
     "*葱*",
     "*姜*",
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/operator.py` & `fnschool-20240515.322.21/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/path.py` & `fnschool-20240515.322.21/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/profile.py` & `fnschool-20240515.322.21/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files 22% similar despite different names*

```diff
@@ -166,130 +166,27 @@
                     + "to food sheets, they will be saved "
                     + "for next updating."
                 )
             )
         else:
             self.bwb.save(bill_fpath0)
 
-        print_info(
-            _('Updated data has been saved to "{0}".').format(bill_fpath0)
-        )
-
         open_file(bill_fpath0)
 
         print_info(_("Updated data was saved."))
 
-    def print_summary(self, foods=None):
-        bfoods = foods or self.bill.foods
-        cfoods = [f for f in bfoods if not f.is_abandoned]
-        currency_mark = self.bill.currency.mark
-        summary = []
-        summary_len = 0
-        inventory_mm1 = sum([f.total_price for f in cfoods if f.is_inventory])
-        inventory_mm1 = (
-            _("Inventory of last month: ") + currency_mark + str(inventory_mm1)
-        )
-
-        warehousing_m = sum(
-            [f.total_price for f in cfoods if not f.is_inventory]
-        )
-        warehousing_m_cp = warehousing_m
-        warehousing_m = (
-            _("Warehousing of this month: ")
-            + currency_mark
-            + str(warehousing_m)
-        )
-        inventory_mm1_warehousing_m = (
-            _("Total: ")
-            + currency_mark
-            + str(sum([f.total_price for f in cfoods]))
-        )
-        consuming_m = 0
-        for f in cfoods:
-            f_consuming_m = sum([c for __, c in f.consumptions])
-            consuming_m += f_consuming_m * f.unit_price
-
-        consuming_m_cp = consuming_m
-        consuming_m = (
-            _("Consuming of this month: ") + currency_mark + str(consuming_m)
-        )
-
-        month_day_m1 = sorted([f.xdate for f in cfoods])[0]
-        for f in cfoods:
-            month_day_m1 = max(
-                [d for d, __ in f.consumptions] + [month_day_m1]
-            )
-
-        inventory_m = sum(
-            [
-                f.get_remainder(month_day_m1) * f.unit_price
-                for f in cfoods
-                if f.get_remainder(month_day_m1) > 0
-            ]
-        )
-        inventory_m_cp = inventory_m
-        inventory_m = (
-            _("Inventory of this month: ") + currency_mark + str(inventory_m)
-        )
-
-        consuming_m_inventory_m = (
-            _("Total: ") + currency_mark + str(consuming_m_cp + inventory_m_cp)
-        )
-
-        afoods = [f for f in bfoods if f.is_abandoned]
-        unwarehousing_m = (
-            _("Unwarehousing of this month: ")
-            + currency_mark
-            + str(sum([f.total_price for f in afoods]))
-        )
-
-        total_purchasing_m = (
-            _("Total purchasing of this month: ")
-            + currency_mark
-            + str(sum([f.total_price for f in bfoods if not f.is_inventory]))
-        )
-        summary = [
-            inventory_mm1,
-            warehousing_m,
-            inventory_mm1_warehousing_m,
-            consuming_m,
-            inventory_m,
-            consuming_m_inventory_m,
-            warehousing_m,
-            unwarehousing_m,
-            total_purchasing_m,
-        ]
-
-        summary_len = max([len(s) for s in summary])
-        summary_sep = "-" * summary_len
-        summary = (
-            summary[:3]
-            + [summary_sep]
-            + summary[3:6]
-            + [summary_sep]
-            + summary[6:]
-        )
-        summary = "\n".join(summary)
-        print()
-        print_info(_("Summary:"))
-        print_info(summary)
-        print()
-
     def update(self):
-
         self.inventory.update()
         self.warehousing.update()
         self.unwarehousing.update()
         self.consuming.update()
         self.sfood.update()
         self.purchasingsum.update()
         self.consumingsum.update()
         self.cover.update()
 
-        self.print_summary()
-
         self.save_workbook()
 
         print_info(_("Update completely!"))
 
 
 # The end.
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import sys
 import calendar
 from datetime import datetime, timedelta
-import math
 
 from fnschool import *
 from fnschool.canteen.food import *
 from fnschool.canteen.path import *
 from fnschool.canteen.spreadsheet.base import *
 
 
@@ -141,29 +140,22 @@
                     (
                         _("New purchased food for date {0} is:")
                         if len(new_wbfoods) > 1
                         else _("New purchased foods for date {0} are:")
                     ).format(tn1.strftime("%Y.%m.%d"))
                 )
 
-                new_wbfood_tips = [
-                    f"({i+1}){f.name} {f.count} {f.unit_name}"
-                    for i, f in enumerate(new_wbfoods)
-                ]
-                new_wbfood_tips_len_sqrt = math.ceil(
-                    len(new_wbfood_tips) ** 0.5
-                )
-                new_wbfood_tip_len = max([len(t) for t in new_wbfood_tips])
-                new_wbfood_tips_value = ""
-                for i, t in enumerate(new_wbfood_tips):
-                    new_wbfood_tips_value += f"{t: <{new_wbfood_tip_len+1}}"
-                    if (i + 1) % new_wbfood_tips_len_sqrt == 0:
-                        new_wbfood_tips_value += "\n"
-                print_warning(new_wbfood_tips_value)
-
+                print_info(
+                    "  ".join(
+                        [
+                            f"({i+1}){f.name} {f.count} {f.unit_name}"
+                            for i, f in enumerate(new_wbfoods)
+                        ]
+                    )
+                )
                 print_warning(_("Negligible foods are not listed."))
             else:
                 print_info(
                     _("There is no purchased food for {0}.").format(
                         tn1.strftime("%Y.%m.%d")
                     )
                 )
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,9 @@
             if self.inventory_col_name:
                 _food.is_inventory = not pd.isna(food[self.inventory_col_name])
             _foods.append(_food)
 
         foods = _foods
         foods = sorted(foods, key=lambda f: f.xdate)
         self.spreadsheet.preconsuming.pre_consume_foods(foods)
-
         return foods
         pass
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240515.322.21/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/test.py` & `fnschool-20240515.322.21/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/canteen/workbook.py` & `fnschool-20240515.322.21/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/entry.py` & `fnschool-20240515.322.21/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/external.py` & `fnschool-20240515.322.21/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/language.py` & `fnschool-20240515.322.21/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240515.322.21/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-15 17:58+0800\n"
-"PO-Revision-Date: 2024-05-15 17:59+0800\n"
+"POT-Creation-Date: 2024-05-15 03:02+0800\n"
+"PO-Revision-Date: 2024-05-15 03:02+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -67,17 +67,14 @@
 
 msgid "Configuration file '%s' was copied to '%s'."
 msgstr "配置文件 “%s” 被复制到 “%s” 。"
 
 msgid "Consuming days:"
 msgstr "耗材日期："
 
-msgid "Consuming of this month: "
-msgstr "本月出库："
-
 msgid "Consuming records:"
 msgstr "消耗记录："
 
 msgid "Consumptions were read."
 msgstr "每日食材消耗已被读取。"
 
 msgid "Copying workbook..."
@@ -194,20 +191,14 @@
 msgstr "如果您觉得 {0} 项目很棒，请您赞助它。您的赞助会让项目继续活下去。"
 
 msgid ""
 "If you save updated data to \"{0}\", data of food sheets will be saved for "
 "every month."
 msgstr "如果您把已更新的数据保存到 “{0}”，那每个月的食材台账表都会被保存下来。"
 
-msgid "Inventory of last month: "
-msgstr "上月盘存："
-
-msgid "Inventory of this month: "
-msgstr "本月盘存："
-
 msgid "Is neglibible"
 msgstr "非入库食材"
 
 msgid "Is residue"
 msgstr "是库存食材"
 
 msgid ""
@@ -395,17 +386,14 @@
 
 msgid "Spreadsheet Files"
 msgstr "工作簿文件。"
 
 msgid "Spreadsheet {0} was copied to {1} ."
 msgstr "工作簿 “{0}” 被复制到 “{1}” 。"
 
-msgid "Summary:"
-msgstr "汇总："
-
 msgid "Supplier name 1"
 msgstr "供应商1"
 
 msgid "Supplier name 2"
 msgstr "供应商2"
 
 msgid "Suppliers:"
@@ -484,48 +472,33 @@
 "盘存食材的以下信息需要被添加：\n"
 "\t1、盘存时间：食材的盘存时间。\n"
 "\t2、组织名 或 学校名。\n"
 "\t3、食材名。\n"
 "\t4、食材数量，如果您的表格有多个数量列，把所有数量列都填上。\n"
 "\t5、食材总价。"
 
-msgid "Total purchasing of this month: "
-msgstr "本月总购入："
-
-msgid "Total: "
-msgstr "总计："
-
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
 
-msgid "Unwarehousing of this month: "
-msgstr "本月未入库："
-
 msgid "Update completely!"
 msgstr "更新完成！"
 
-msgid "Updated data has been saved to \"{0}\"."
-msgstr "更新的数据已被保存到 “{0}”。"
-
 msgid "Updated data was saved."
 msgstr "被更改的数据已保存。"
 
-msgid "Warehousing of this month: "
-msgstr "本月入库："
-
 msgid "Workbook %s was read."
 msgstr "已读取 工作簿 “%s” 。"
 
 msgid "Workbook '%s' has been used."
 msgstr "使用工作薄 “%s” 。"
 
 msgid "Workbook '%s' was saved."
```

### Comparing `fnschool-20240515.1802.50/src/fnschool/log.py` & `fnschool-20240515.322.21/src/fnschool/log.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/path.py` & `fnschool-20240515.322.21/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool/test.py` & `fnschool-20240515.322.21/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240515.1802.50/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240515.322.21/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240515.1802.50
+Version: 20240515.322.21
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240515.1802.50/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240515.322.21/src/fnschool.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 src/fnschool/canteen/__init__.py
 src/fnschool/canteen/__main__.py
 src/fnschool/canteen/bill.cp.py
 src/fnschool/canteen/bill.py
 src/fnschool/canteen/canteen.toml
 src/fnschool/canteen/config.py
 src/fnschool/canteen/consume.py
-src/fnschool/canteen/currency.py
 src/fnschool/canteen/food.cp.py
 src/fnschool/canteen/food.py
 src/fnschool/canteen/food_classes.toml
 src/fnschool/canteen/food_recount.toml
 src/fnschool/canteen/food_recounts.toml
 src/fnschool/canteen/operator.py
 src/fnschool/canteen/path.py
```

