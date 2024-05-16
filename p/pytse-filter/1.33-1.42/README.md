# Comparing `tmp/pytse_filter-1.33.tar.gz` & `tmp/pytse_filter-1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytse_filter-1.33.tar", last modified: Thu Apr 18 12:16:00 2024, max compression
+gzip compressed data, was "pytse_filter-1.42.tar", last modified: Wed May  1 13:58:53 2024, max compression
```

## Comparing `pytse_filter-1.33.tar` & `pytse_filter-1.42.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.860867 pytse_filter-1.33/
--rw-rw-rw-   0        0        0       94 2024-03-21 14:02:36.000000 pytse_filter-1.33/MANIFEST.in
--rw-rw-rw-   0        0        0     4798 2024-04-18 12:16:00.856871 pytse_filter-1.33/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.253515 pytse_filter-1.33/docs/
--rw-rw-rw-   0        0        0   187418 2024-04-06 17:46:37.000000 pytse_filter-1.33/docs/HistoryVariables.xlsx
--rw-rw-rw-   0        0        0    11144 2024-04-16 14:08:03.000000 pytse_filter-1.33/docs/RealTimeVariables.xlsx
--rw-rw-rw-   0        0        0     9994 2024-03-31 17:57:17.000000 pytse_filter-1.33/docs/user guide.md
--rw-rw-rw-   0        0        0    29893 2024-04-09 20:03:39.000000 pytse_filter-1.33/docs/راهنمای کاربر.docx
--rw-rw-rw-   0        0        0    13618 2024-03-31 17:57:42.000000 pytse_filter-1.33/docs/راهنمای کاربر.md
--rw-rw-rw-   0        0        0  1142189 2024-04-09 20:05:37.000000 pytse_filter-1.33/docs/راهنمای کاربر.pdf
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.486081 pytse_filter-1.33/examples/
--rw-rw-rw-   0        0        0      250 2024-03-18 16:27:50.000000 pytse_filter-1.33/examples/code2code.py
--rw-rw-rw-   0        0        0       69 2024-04-10 10:30:47.000000 pytse_filter-1.33/examples/code2code.txt
--rw-rw-rw-   0        0        0      672 2024-04-10 10:31:43.000000 pytse_filter-1.33/examples/combine_history_realtime.py
--rw-rw-rw-   0        0        0      807 2024-03-18 15:57:39.000000 pytse_filter-1.33/examples/disappear_sell_queue.py
--rw-rw-rw-   0        0        0      803 2024-04-10 12:42:17.000000 pytse_filter-1.33/examples/hot_money.py
--rw-rw-rw-   0        0        0     1754 2024-03-18 16:31:29.000000 pytse_filter-1.33/examples/market_overview.py
--rw-rw-rw-   0        0        0     1024 2024-04-10 10:28:48.000000 pytse_filter-1.33/examples/simple_history_filters.py
--rw-rw-rw-   0        0        0     1091 2024-04-10 10:27:24.000000 pytse_filter-1.33/examples/simple_realtime_filters.py
--rw-rw-rw-   0        0        0     1110 2024-02-22 12:28:42.000000 pytse_filter-1.33/license.md
--rw-rw-rw-   0        0        0     3463 2024-03-22 16:16:51.000000 pytse_filter-1.33/readme.md
--rw-rw-rw-   0        0        0      331 2024-04-09 21:03:15.000000 pytse_filter-1.33/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 12:16:00.860867 pytse_filter-1.33/setup.cfg
--rw-rw-rw-   0        0        0     1286 2024-04-18 12:11:31.000000 pytse_filter-1.33/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.043576 pytse_filter-1.33/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.800902 pytse_filter-1.33/src/pytse_filter/
--rw-rw-rw-   0        0        0      255 2024-03-16 15:42:50.000000 pytse_filter-1.33/src/pytse_filter/__init__.py
--rw-rw-rw-   0        0        0     1252 2024-03-27 15:23:51.000000 pytse_filter-1.33/src/pytse_filter/calculate_client_data.py
--rw-rw-rw-   0        0        0     2430 2024-04-09 20:58:03.000000 pytse_filter-1.33/src/pytse_filter/calculate_indicators.py
--rw-rw-rw-   0        0        0     1178 2024-03-27 15:25:25.000000 pytse_filter-1.33/src/pytse_filter/client_setting.py
--rw-rw-rw-   0        0        0     3815 2024-04-16 13:55:34.000000 pytse_filter-1.33/src/pytse_filter/config.py
--rw-rw-rw-   0        0        0     6211 2024-04-18 12:13:27.000000 pytse_filter-1.33/src/pytse_filter/download_history.py
--rw-rw-rw-   0        0        0     9564 2024-04-16 13:54:25.000000 pytse_filter-1.33/src/pytse_filter/download_realtime.py
--rw-rw-rw-   0        0        0     8407 2024-04-16 13:43:24.000000 pytse_filter-1.33/src/pytse_filter/history.py
--rw-rw-rw-   0        0        0     5065 2024-03-20 10:48:40.000000 pytse_filter-1.33/src/pytse_filter/inds_setting.py
--rw-rw-rw-   0        0        0     7347 2024-03-30 10:57:00.000000 pytse_filter-1.33/src/pytse_filter/realtime.py
--rw-rw-rw-   0        0        0    32725 2024-03-18 15:21:37.000000 pytse_filter-1.33/src/pytse_filter/syms.json
--rw-rw-rw-   0        0        0     1401 2024-03-18 16:46:27.000000 pytse_filter-1.33/src/pytse_filter/syms_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:16:00.854871 pytse_filter-1.33/src/pytse_filter.egg-info/
--rw-rw-rw-   0        0        0     4798 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-18 12:16:00.000000 pytse_filter-1.33/src/pytse_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      312 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 12:15:59.000000 pytse_filter-1.33/src/pytse_filter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.811277 pytse_filter-1.42/
+-rw-rw-rw-   0        0        0       94 2024-03-21 14:02:36.000000 pytse_filter-1.42/MANIFEST.in
+-rw-rw-rw-   0        0        0     4826 2024-05-01 13:58:53.803274 pytse_filter-1.42/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.180629 pytse_filter-1.42/docs/
+-rw-rw-rw-   0        0        0   187418 2024-04-06 17:46:37.000000 pytse_filter-1.42/docs/HistoryVariables.xlsx
+-rw-rw-rw-   0        0        0    11144 2024-04-16 14:08:03.000000 pytse_filter-1.42/docs/RealTimeVariables.xlsx
+-rw-rw-rw-   0        0        0     9994 2024-03-31 17:57:17.000000 pytse_filter-1.42/docs/user guide.md
+-rw-rw-rw-   0        0        0    29893 2024-04-09 20:03:39.000000 pytse_filter-1.42/docs/راهنمای کاربر.docx
+-rw-rw-rw-   0        0        0    13618 2024-03-31 17:57:42.000000 pytse_filter-1.42/docs/راهنمای کاربر.md
+-rw-rw-rw-   0        0        0  1142189 2024-04-09 20:05:37.000000 pytse_filter-1.42/docs/راهنمای کاربر.pdf
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.255587 pytse_filter-1.42/examples/
+-rw-rw-rw-   0        0        0      250 2024-03-18 16:27:50.000000 pytse_filter-1.42/examples/code2code.py
+-rw-rw-rw-   0        0        0       69 2024-04-10 10:30:47.000000 pytse_filter-1.42/examples/code2code.txt
+-rw-rw-rw-   0        0        0      672 2024-04-10 10:31:43.000000 pytse_filter-1.42/examples/combine_history_realtime.py
+-rw-rw-rw-   0        0        0      807 2024-03-18 15:57:39.000000 pytse_filter-1.42/examples/disappear_sell_queue.py
+-rw-rw-rw-   0        0        0      803 2024-04-10 12:42:17.000000 pytse_filter-1.42/examples/hot_money.py
+-rw-rw-rw-   0        0        0     1754 2024-03-18 16:31:29.000000 pytse_filter-1.42/examples/market_overview.py
+-rw-rw-rw-   0        0        0     1024 2024-04-10 10:28:48.000000 pytse_filter-1.42/examples/simple_history_filters.py
+-rw-rw-rw-   0        0        0     1091 2024-04-10 10:27:24.000000 pytse_filter-1.42/examples/simple_realtime_filters.py
+-rw-rw-rw-   0        0        0     1110 2024-02-22 12:28:42.000000 pytse_filter-1.42/license.md
+-rw-rw-rw-   0        0        0     3463 2024-03-22 16:16:51.000000 pytse_filter-1.42/readme.md
+-rw-rw-rw-   0        0        0      501 2024-05-01 13:42:10.000000 pytse_filter-1.42/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 13:58:53.812269 pytse_filter-1.42/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-05-01 13:43:56.000000 pytse_filter-1.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.112668 pytse_filter-1.42/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.516439 pytse_filter-1.42/src/pytse_filter/
+-rw-rw-rw-   0        0        0      255 2024-03-16 15:42:50.000000 pytse_filter-1.42/src/pytse_filter/__init__.py
+-rw-rw-rw-   0        0        0     1252 2024-03-27 15:23:51.000000 pytse_filter-1.42/src/pytse_filter/calculate_client_data.py
+-rw-rw-rw-   0        0        0     2430 2024-04-09 20:58:03.000000 pytse_filter-1.42/src/pytse_filter/calculate_indicators.py
+-rw-rw-rw-   0        0        0     1178 2024-03-27 15:25:25.000000 pytse_filter-1.42/src/pytse_filter/client_setting.py
+-rw-rw-rw-   0        0        0     3877 2024-05-01 13:42:10.000000 pytse_filter-1.42/src/pytse_filter/config.py
+-rw-rw-rw-   0        0        0     6211 2024-04-18 12:13:27.000000 pytse_filter-1.42/src/pytse_filter/download_history.py
+-rw-rw-rw-   0        0        0     9564 2024-04-16 13:54:25.000000 pytse_filter-1.42/src/pytse_filter/download_realtime.py
+-rw-rw-rw-   0        0        0     8407 2024-04-16 13:43:24.000000 pytse_filter-1.42/src/pytse_filter/history.py
+-rw-rw-rw-   0        0        0     5065 2024-03-20 10:48:40.000000 pytse_filter-1.42/src/pytse_filter/inds_setting.py
+-rw-rw-rw-   0        0        0     7347 2024-03-30 10:57:00.000000 pytse_filter-1.42/src/pytse_filter/realtime.py
+-rw-rw-rw-   0        0        0    26357 2024-05-01 13:54:42.000000 pytse_filter-1.42/src/pytse_filter/syms.json
+-rw-rw-rw-   0        0        0     5843 2024-05-01 13:52:37.000000 pytse_filter-1.42/src/pytse_filter/syms_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 13:58:53.801275 pytse_filter-1.42/src/pytse_filter.egg-info/
+-rw-rw-rw-   0        0        0     4826 2024-05-01 13:58:53.000000 pytse_filter-1.42/src/pytse_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-05-01 13:58:53.000000 pytse_filter-1.42/src/pytse_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 13:58:53.000000 pytse_filter-1.42/src/pytse_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      324 2024-05-01 13:58:53.000000 pytse_filter-1.42/src/pytse_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-01 13:58:53.000000 pytse_filter-1.42/src/pytse_filter.egg-info/top_level.txt
```

### Comparing `pytse_filter-1.33/PKG-INFO` & `pytse_filter-1.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytse_filter
-Version: 1.33
+Version: 1.42
 Summary: A user-friendly project to filter symbols of Tehran Stock Exchange
 Home-page: https://github.com/farhad-mohammadi/pytse_filter
 Author: Farhad Mohammadi
 Author-email: farhad.mohammadi60@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,15 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: tzdata==2024.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: jalali_core==1.0.0
 Requires-Dist: jdatetime==5.0.0
+Requires-Dist: lxml==5.2.1
 
 # pytse-filter: Tehran Stock Exchange Data Processing Library
 
 Welcome to the **pytse-filter** library, a Python package designed for processing and analyzing Tehran Stock Exchange (TSE) symbol data through user-defined text filters. This library simplifies the task of filtering TSE data based on various conditions, making it an essential tool for traders and analysts.
 
 ## Prerequisites
```

### Comparing `pytse_filter-1.33/docs/HistoryVariables.xlsx` & `pytse_filter-1.42/docs/HistoryVariables.xlsx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/docs/RealTimeVariables.xlsx` & `pytse_filter-1.42/docs/RealTimeVariables.xlsx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/docs/user guide.md` & `pytse_filter-1.42/docs/user guide.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/docs/راهنمای کاربر.docx` & `pytse_filter-1.42/docs/راهنمای کاربر.docx`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/docs/راهنمای کاربر.md` & `pytse_filter-1.42/docs/راهنمای کاربر.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/docs/راهنمای کاربر.pdf` & `pytse_filter-1.42/docs/راهنمای کاربر.pdf`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/combine_history_realtime.py` & `pytse_filter-1.42/examples/combine_history_realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/disappear_sell_queue.py` & `pytse_filter-1.42/examples/disappear_sell_queue.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/hot_money.py` & `pytse_filter-1.42/examples/hot_money.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/market_overview.py` & `pytse_filter-1.42/examples/market_overview.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/simple_history_filters.py` & `pytse_filter-1.42/examples/simple_history_filters.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/examples/simple_realtime_filters.py` & `pytse_filter-1.42/examples/simple_realtime_filters.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/license.md` & `pytse_filter-1.42/license.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/readme.md` & `pytse_filter-1.42/readme.md`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/setup.py` & `pytse_filter-1.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 from os import path
 
-__version__ = 1.33
+__version__ = 1.42
 
 with open( ".\\readme.md", "r") as f:
     long_description = f.read()
 
 with open(".\\requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
```

### Comparing `pytse_filter-1.33/src/pytse_filter/calculate_client_data.py` & `pytse_filter-1.42/src/pytse_filter/calculate_client_data.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/calculate_indicators.py` & `pytse_filter-1.42/src/pytse_filter/calculate_indicators.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/client_setting.py` & `pytse_filter-1.42/src/pytse_filter/client_setting.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/config.py` & `pytse_filter-1.42/src/pytse_filter/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 HEADERS  = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
 PRICE_URL = "http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx"
 CLIENT_URL = "http://old.tsetmc.com/tsev2/data/clienttypeall.aspx"
 PRICE_HISTORY = "http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={}&Top={}&A=0"
 ADJUSTED_PRICE_HISTORY = "https://members.tsetmc.com/tsev2/chart/data/Financial.aspx?i={}&t=ph&a=1"
 CLIENT_HISTORY ="http://cdn.tsetmc.com/api/ClientType/GetClientTypeHistory/{}"
+SYMBOLS = "http://old.tsetmc.com/Loader.aspx?ParTree=151114"
 
 REALTIME_COLUMNS = [
     'code', 'symbol', 'name', 'pf', 'pmin', 'pmax', 'pl', 'pc', 'py', 'tno', 'tvol', 'tval',
     'eps', 'bvol', 'tmax', 'tmin', 
     'plp', 'pcp', 'pfp', 'pminp', 'pmaxp', 'tminp', 'tmaxp',  'z',
     'buy_i_count', 'buy_n_count',
     'buy_i_volume', 'buy_n_volume', 'sell_i_count', 'sell_n_count',
```

### Comparing `pytse_filter-1.33/src/pytse_filter/download_history.py` & `pytse_filter-1.42/src/pytse_filter/download_history.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/download_realtime.py` & `pytse_filter-1.42/src/pytse_filter/download_realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/history.py` & `pytse_filter-1.42/src/pytse_filter/history.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/inds_setting.py` & `pytse_filter-1.42/src/pytse_filter/inds_setting.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/realtime.py` & `pytse_filter-1.42/src/pytse_filter/realtime.py`

 * *Files identical despite different names*

### Comparing `pytse_filter-1.33/src/pytse_filter/syms.json` & `pytse_filter-1.42/src/pytse_filter/syms.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5941176470588235%*

 * *Differences: {"'آذرین'": "'43358402418932595'",*

 * * "'آریان'": "'31987503418964901'",*

 * * "'آسامید'": "'24869832924911721'",*

 * * "'آفرین'": "'37028614515926436'",*

 * * "'آلا'": "'19828734979381742'",*

 * * "'آلتون'": "'28374437855144739'",*

 * * "'آکام'": "'490987973229371'",*

 * * "'آکورد'": "'30282299500988269'",*

 * * "'اتوآگاه'": "'6328167131743522'",*

 * * "'اردستان'": "'35331248532537562'",*

 * * "'ارزش مسکن'": "'71945594172117613'",*

 * * "'ارمغان'": "'31366347648583654'",*

 * * "'استیل'": "'24907784641855842'",*

 * * "'اصیل'": "'8021561335311415'",*

 * * "'اعتبار'": "'35163 […]*

```diff
@@ -1,831 +1,670 @@
 {
     "\u0622 \u0633 \u067e": "17617474823279712",
     "\u0622\u0628\u0627\u062f\u0627": "37661500521100963",
-    "\u0622\u0628\u06cc\u0646": "9987529074833218",
     "\u0622\u062a\u06cc\u0645\u0633": "22839330962768817",
+    "\u0622\u0630\u0631\u06cc\u0646": "43358402418932595",
     "\u0622\u0631\u0627\u0645": "14230681955555738",
-    "\u0622\u0631\u0645\u0627\u0646": "38738476064699383",
     "\u0622\u0631\u06cc\u0627": "55127657985997520",
-    "\u0622\u0631\u06cc\u0627\u0646": "6506179926371994",
-    "\u0622\u0631\u06cc\u0627\u06462": "51584388430602252",
+    "\u0622\u0631\u06cc\u0627\u0646": "31987503418964901",
     "\u0622\u0633\u0627\u0633": "66682662312253625",
     "\u0622\u0633\u0627\u0645": "36592972482259020",
+    "\u0622\u0633\u0627\u0645\u06cc\u062f": "24869832924911721",
     "\u0622\u0633\u06cc\u0627": "51106317433079213",
-    "\u0622\u0641\u0627\u0642": "37073830945037165",
-    "\u0622\u0641\u0627\u06422": "48471618473277756",
+    "\u0622\u0641\u0631\u06cc\u0646": "37028614515926436",
+    "\u0622\u0644\u0627": "19828734979381742",
+    "\u0622\u0644\u062a\u0648\u0646": "28374437855144739",
     "\u0622\u0648\u0627": "18007109712724189",
     "\u0622\u0648\u0646\u062f": "31039212000825988",
-    "\u0622\u0648\u0646\u062f2": "63931778908484911",
     "\u0622\u067e": "55254206302462116",
+    "\u0622\u06a9\u0627\u0645": "490987973229371",
+    "\u0622\u06a9\u0648\u0631\u062f": "30282299500988269",
     "\u0622\u06af\u0627\u0633": "33887145736684266",
-    "\u0622\u06af\u0627\u06332": "48702596863145683",
-    "\u0622\u06cc\u0646\u062f\u0647": "17933573078185644",
-    "\u0627\u062a\u06a9\u0627\u0633\u0627": "68644622102682218",
+    "\u0627\u062a\u0648\u0622\u06af\u0627\u0647": "6328167131743522",
     "\u0627\u062a\u06a9\u0627\u0645": "27405735172634593",
     "\u0627\u062a\u06a9\u0627\u06cc": "39751275523025334",
     "\u0627\u062e\u0627\u0628\u0631": "22811176775480091",
+    "\u0627\u0631\u062f\u0633\u062a\u0627\u0646": "35331248532537562",
     "\u0627\u0631\u0632\u0634": "43443105991896600",
-    "\u0627\u0631\u0632\u06342": "26958329630564882",
+    "\u0627\u0631\u0632\u0634 \u0645\u0633\u06a9\u0646": "71945594172117613",
     "\u0627\u0631\u0641\u0639": "59266699437480384",
-    "\u0627\u0633\u062a\u0627\u0631\u0632": "4395741730355818",
+    "\u0627\u0631\u0645\u063a\u0627\u0646": "31366347648583654",
+    "\u0627\u0633\u062a\u06cc\u0644": "24907784641855842",
     "\u0627\u0633\u06cc\u0627\u062a\u06a9": "14079693677610396",
+    "\u0627\u0635\u06cc\u0644": "8021561335311415",
     "\u0627\u0637\u0644\u0633": "11427939669935844",
-    "\u0627\u0637\u0644\u06332": "69065132449283302",
+    "\u0627\u0639\u062a\u0628\u0627\u0631": "35163287528816137",
     "\u0627\u0639\u062a\u0644\u0627": "36773155987365094",
+    "\u0627\u0639\u062a\u0645\u0627\u062f": "66818022341772870",
     "\u0627\u0641\u0631\u0627": "52792903131341205",
-    "\u0627\u0641\u0631\u0627\u06462": "64701620739344512",
-    "\u0627\u0641\u0631\u0627\u06464": "54162468776731366",
     "\u0627\u0641\u0642": "49502666250908008",
     "\u0627\u0641\u0642 \u0645\u0644\u062a": "15451317146134956",
     "\u0627\u0644\u0628\u0631\u0632": "70270965300262393",
     "\u0627\u0644\u0645\u0627\u0633": "28788598290160782",
     "\u0627\u0645\u06cc\u062f": "18599703143458101",
     "\u0627\u0645\u06cc\u0646": "58873907630765023",
+    "\u0627\u0645\u06cc\u0646 \u0634\u0647\u0631": "70814244102598215",
     "\u0627\u0646\u0627\u0631": "30215634246748564",
-    "\u0627\u0646\u0631\u0698\u06cc3": "49641108336531623",
+    "\u0627\u0646\u0631\u0698\u06cc": "49641108336531623",
     "\u0627\u0647\u0631\u0645": "17914401175772326",
     "\u0627\u0648\u0627\u0646": "69847139870135237",
     "\u0627\u0648\u062c": "62575434414985179",
-    "\u0627\u0648\u0635\u062a\u06272": "42927746927909254",
+    "\u0627\u0648\u0635\u062a\u0627": "57761388729898548",
     "\u0627\u067e\u0627\u0644": "655060129740445",
     "\u0627\u067e\u0631\u062f\u0627\u0632": "63830424809501048",
-    "\u0628\u0627\u0631\u0627\u0646": "26882843763780650",
+    "\u0627\u06a9\u0633\u06cc\u0631": "33677077231841786",
+    "\u0627\u06a9\u0633\u06cc\u0698\u0646": "50094941173290382",
+    "\u0628\u0627\u0632\u0628\u06cc\u0645\u0647": "61483657213051835",
     "\u0628\u0627\u0644\u0627\u0633": "8646067353086740",
     "\u0628\u0627\u0644\u0628\u0631": "62952165421099192",
-    "\u0628\u0627\u06cc\u06a9\u0627": "23891830829322971",
     "\u0628\u062a\u0631\u0627\u0646\u0633": "46752599569017089",
-    "\u0628\u062a\u06a9": "54369290104873523",
     "\u0628\u062c\u0647\u0631\u0645": "33629260529503413",
     "\u0628\u062e\u0627\u0648\u0631": "5599691633622269",
     "\u0628\u0630\u0631": "37222720235819361",
     "\u0628\u0631\u0644\u06cc\u0627\u0646": "4216536645718658",
     "\u0628\u0631\u06a9\u062a": "34557241988629814",
     "\u0628\u0632\u0627\u06af\u0631\u0633": "29882244560576007",
     "\u0628\u0633\u0627\u0645\u0627": "41625340598198551",
     "\u0628\u0633\u0648\u06cc\u0686": "47377315952751604",
     "\u0628\u0634\u0647\u0627\u0628": "69454539056549106",
     "\u0628\u0641\u062c\u0631": "46178280540110577",
+    "\u0628\u0645\u0627\u0646": "52551569846042389",
     "\u0628\u0645\u0648\u062a\u0648": "22086876724551482",
+    "\u0628\u0645\u0648\u0644\u062f": "48261930411425125",
     "\u0628\u0645\u067e\u0646\u0627": "39807886630843041",
-    "\u0628\u0645\u06cc\u0644\u0627": "16553062355259729",
     "\u0628\u0646\u0648": "54493234408301135",
     "\u0628\u0646\u06cc\u0631\u0648": "20453828618330936",
     "\u0628\u0647\u067e\u0627\u06a9": "12746730665870442",
-    "\u0628\u0647\u06cc\u0631": "60289595205403229",
+    "\u0628\u0647\u06cc\u0646 \u0631\u0648": "42799209630949274",
     "\u0628\u0648\u0631\u0633": "60523145697836739",
+    "\u0628\u0648\u0639\u0644\u06cc": "50247622569476338",
     "\u0628\u067e\u0627\u0633": "51971068201094874",
     "\u0628\u067e\u06cc\u0648\u0646\u062f": "64619251116188373",
     "\u0628\u06a9\u0627\u0628": "70219663893822560",
+    "\u0628\u06a9\u0627\u0628\u0644": "62107151670661969",
     "\u0628\u06a9\u0627\u0645": "22382156782768756",
     "\u0628\u06a9\u0647\u0646\u0648\u062c": "7628308021169118",
     "\u0628\u06af\u06cc\u0644\u0627\u0646": "71068313834275501",
-    "\u062a\u0627\u0628\u0627": "51459202425114449",
-    "\u062a\u0627\u062a\u0645\u0633": "35543935713999309",
+    "\u062a\u0627\u0628\u0634": "9089296888187061",
     "\u062a\u0627\u0631\u0627\u0632": "24651394045981418",
     "\u062a\u0627\u0635\u06cc\u06a9\u0648": "23293437377896568",
     "\u062a\u0627\u067e\u06a9\u06cc\u0634": "50002340308486819",
     "\u062a\u0627\u067e\u06cc\u06a9\u0648": "22560050433388046",
     "\u062a\u0627\u06cc\u0631\u0627": "19298748452450329",
     "\u062a\u0628\u0631\u06a9": "53204330224889981",
     "\u062a\u062c\u0644\u06cc": "1301069819790264",
-    "\u062a\u0634\u062a\u0627\u062f": "66127247173352975",
-    "\u062a\u0635\u0645\u06cc\u06452": "10367678011039964",
-    "\u062a\u0641\u0627\u0631\u0633": "22276798221643766",
+    "\u062a\u062e\u062a \u06af\u0627\u0632": "30507739597192201",
+    "\u062a\u0631\u0645\u0647": "42705920381780437",
     "\u062a\u0644\u06cc\u0633\u0647": "41781090739318251",
     "\u062a\u0645\u0627\u0648\u0646\u062f": "60162288821230099",
-    "\u062a\u0645\u062d\u0631\u06a9\u0647": "22427604495160869",
+    "\u062a\u0645\u0634\u06a9": "53145304508578701",
     "\u062a\u0645\u0644\u062a": "11129387075131725",
     "\u062a\u0646\u0648\u06cc\u0646": "25357135030606405",
+    "\u062a\u0648\u0627\u0646": "41927452991671109",
     "\u062a\u0648\u0631\u06cc\u0644": "37389789764168256",
     "\u062a\u0648\u0633\u0646": "66315581735594751",
     "\u062a\u067e\u0633\u06cc": "3839324986781871",
     "\u062a\u067e\u0645\u067e\u06cc": "43062880954780884",
-    "\u062a\u067e\u0648\u0644\u0627": "22308305646551497",
-    "\u062a\u067e\u06a9\u0648": "54509759694064219",
+    "\u062a\u06a9\u0627\u0631\u062f\u0627\u0646": "52932092555708556",
     "\u062a\u06a9\u0634\u0627": "62258804563636993",
     "\u062a\u06a9\u0645\u0628\u0627": "30719054967088301",
-    "\u062a\u06a9\u0646\u0627\u0631": "52455922800537930",
     "\u062a\u06a9\u0646\u0648": "3654864906585643",
+    "\u062a\u06a9\u067e\u0627\u062f": "1825060609227181",
+    "\u062a\u06cc\u0627\u0645": "16578517055478811",
     "\u062a\u06cc\u067e\u06cc\u06a9\u0648": "29758477602878557",
-    "\u062b\u0627\u0628\u0627\u062f": "59612098290740355",
     "\u062b\u0627\u062e\u062a": "17800036702302776",
-    "\u062b\u0627\u0635\u0641\u0627": "7503669593172728",
     "\u062b\u0627\u0644\u0648\u0646\u062f": "16693610252404739",
     "\u062b\u0627\u0645\u0627\u0646": "66456062140680461",
     "\u062b\u0627\u0645\u06cc\u062f": "18568733593280948",
-    "\u062b\u0627\u0698\u0646": "40650252484299134",
     "\u062b\u0628\u0627\u062a": "26780282166315918",
-    "\u062b\u0628\u0627\u062a2": "5051727550286539",
-    "\u062b\u0628\u0627\u062a4": "32954653822770119",
     "\u062b\u0628\u0627\u063a": "68909035712962732",
     "\u062b\u0628\u0647\u0633\u0627\u0632": "14744445176220774",
     "\u062b\u062a\u0631\u0627\u0646": "20926459161497908",
-    "\u062b\u062a\u0648\u0633\u0627": "47702059190622416",
-    "\u062b\u062c\u0648\u0627\u0646": "30507152381699953",
+    "\u062b\u062c\u0646\u0648\u0628": "60887982279284651",
     "\u062b\u0631\u0648\u062a\u0645": "71672399601682259",
     "\u062b\u0631\u0648\u062f": "18883380772506226",
-    "\u062b\u0632\u0627\u06af\u0631\u0633": "28854105556435129",
     "\u062b\u0634\u0627\u0647\u062f": "63481599728522324",
     "\u062b\u0634\u0631\u0642": "6043384171800349",
-    "\u062b\u0639\u062a\u0645\u0627": "64707090254488560",
     "\u062b\u0639\u0645\u0631\u0627": "15726796686853780",
     "\u062b\u063a\u0631\u0628": "17939384202383793",
     "\u062b\u0641\u0627\u0631\u0633": "30852391633490755",
-    "\u062b\u0642\u0632\u0648\u06cc": "12965822877128721",
     "\u062b\u0645\u0633\u06a9\u0646": "3863538898378476",
     "\u062b\u0645\u06cc\u0646": "66721204145017523",
-    "\u062b\u0646\u0627\u0645": "831325835570803",
-    "\u062b\u0646\u0638\u0627\u0645": "45066064863062755",
-    "\u062b\u0646\u0648\u0631": "63315013743060811",
+    "\u062b\u0646\u0627": "32112121249636248",
     "\u062b\u0646\u0648\u0633\u0627": "32845891587040106",
+    "\u062b\u0647\u0627\u0645": "38713440086361985",
     "\u062b\u067e\u0631\u062f\u06cc\u0633": "53999651992586159",
+    "\u062c\u0627\u0648\u062f\u0627\u0646": "49531112577387255",
     "\u062c\u0645": "32357363984168442",
     "\u062c\u0645 \u067e\u06cc\u0644\u0646": "27096851668435724",
-    "\u062c\u0647\u0631\u0645": "49674915481184052",
-    "\u062c\u0648\u06cc\u0646": "23269285154135003",
-    "\u062d\u0622\u0633\u0627": "44625249840480397",
+    "\u062c\u0647\u0634": "7681671915916933",
+    "\u062c\u0648\u0627\u0647\u0631": "38544104313215500",
     "\u062d\u0622\u0641\u0631\u06cc\u0646": "21432551703060846",
-    "\u062d\u0627\u0631\u06cc\u0627": "56798822689379375",
-    "\u062d\u0628\u0646\u062f\u0631": "63704201144621295",
     "\u062d\u062a\u0627\u06cc\u062f": "3722699128879020",
     "\u062d\u062a\u0648\u06a9\u0627": "22260326095996531",
     "\u062d\u062e\u0632\u0631": "28253678449273505",
-    "\u062d\u0631\u0647\u0634\u0627": "30443839313522574",
     "\u062d\u0631\u06cc\u0644": "5564768007356822",
     "\u062d\u0633\u06cc\u0631": "13281937213456378",
     "\u062d\u0633\u06cc\u0646\u0627": "1625149423498289",
-    "\u062d\u0634\u06a9\u0648\u0647": "50587892784913370",
     "\u062d\u0641\u0627\u0631\u0633": "35424116338766901",
     "\u062d\u0641\u0627\u0631\u06cc": "28809886765682162",
-    "\u062d\u067e\u0627\u0631\u0633\u0627": "917857106093847",
     "\u062d\u067e\u062a\u0631\u0648": "16369313804633525",
+    "\u062d\u067e\u0631\u062a\u0648": "4885314541377431",
     "\u062d\u06a9\u0634\u062a\u06cc": "60610861509165508",
-    "\u062d\u06af\u0631\u062f\u0634": "53334304751609770",
     "\u062d\u06af\u0647\u0631": "47756003257788498",
-    "\u062e\u0627\u062a\u0645": "18865325633315847",
     "\u062e\u0627\u0630\u06cc\u0646": "42075223783409640",
     "\u062e\u0627\u0647\u0646": "7483280423474368",
-    "\u062e\u0627\u0648\u0631": "16315910303613772",
-    "\u062e\u0627\u0648\u0631\u062d": "23657236334749347",
-    "\u062e\u0628\u0627\u0632\u0631\u0633": "19310456400689867",
+    "\u062e\u0627\u0648\u0631": "49270349234092953",
     "\u062e\u0628\u0647\u0645\u0646": "26824673819862694",
     "\u062e\u062a\u0631\u0627\u06a9": "22903901709044823",
     "\u062e\u062a\u0648\u0631": "50185721305191887",
     "\u062e\u062a\u0648\u0642\u0627": "70289374539527245",
     "\u062e\u062f\u06cc\u0632\u0644": "38084304113529336",
     "\u062e\u0631\u0627\u0633\u0627\u0646": "43552974795606067",
     "\u062e\u0631\u06cc\u062e\u062a": "12752224677923341",
     "\u062e\u0631\u06cc\u0646\u06af": "45895339414786358",
     "\u062e\u0632\u0627\u0645\u06cc\u0627": "2589887561569709",
     "\u062e\u0632\u0631": "32821908911812078",
     "\u062e\u0633\u0627\u067e\u0627": "44891482026867833",
     "\u062e\u0634\u0631\u0642": "63915926161403347",
-    "\u062e\u0641\u0646\u0627\u0648\u0631": "58180284328186631",
     "\u062e\u0641\u0646\u0631": "28033133021443774",
-    "\u062e\u0641\u0648\u0644\u0627": "23049019886587905",
     "\u062e\u0644\u0646\u062a": "14957056743925737",
-    "\u062e\u0644\u06cc\u0628\u0644": "50117925085549635",
+    "\u062e\u0644\u06cc\u062c": "26458514535443899",
     "\u062e\u0645\u062d\u0631\u06a9\u0647": "39436183727126211",
     "\u062e\u0645\u062d\u0648\u0631": "7457232989848872",
     "\u062e\u0645\u0647\u0631": "17330546482145553",
     "\u062e\u0645\u0648\u062a\u0648\u0631": "57273529732791251",
     "\u062e\u0646\u0635\u06cc\u0631": "17834623106317041",
+    "\u062e\u0648\u062f\u0631\u0627\u0646": "67261627618765635",
     "\u062e\u0648\u062f\u0631\u0648": "65883838195688438",
-    "\u062e\u0648\u062f\u06a9\u0641\u0627": "22956708386610464",
+    "\u062e\u0648\u0631\u0634\u06cc\u062f": "4523009251964699",
     "\u062e\u0648\u0633\u0627\u0632": "31879190587976736",
-    "\u062e\u067e\u0627\u0631\u0633": "42354736493447489",
     "\u062e\u067e\u0648\u06cc\u0634": "4758266259250794",
     "\u062e\u0686\u0631\u062e\u0634": "33783140337377394",
     "\u062e\u06a9\u0627\u0631": "59217041815333317",
-    "\u062e\u06a9\u0627\u0648\u0647": "64842837716888827",
-    "\u062e\u06a9\u0631\u0645\u0627\u0646": "29527985620948695",
+    "\u062e\u06a9\u0631\u0645\u0627\u0646": "58482817740704549",
     "\u062e\u06a9\u0645\u06a9": "19257295292088310",
     "\u062e\u06af\u0633\u062a\u0631": "48990026850202503",
     "\u062f\u0627\u0628\u0648\u0631": "61332057061846617",
-    "\u062f\u0627\u0628\u0648\u0631\u062d": "32679348534913643",
+    "\u062f\u0627\u062a\u0627\u0645": "68863997659126807",
+    "\u062f\u0627\u0631\u0627": "62012736978844991",
     "\u062f\u0627\u0631\u0627 \u06cc\u06a9\u0645": "62235397452612911",
-    "\u062f\u0627\u0631\u0627\u0628": "27299841173245405",
     "\u062f\u0627\u0631\u0648": "67988012428906654",
     "\u062f\u0627\u0631\u06cc\u0648\u0634": "58789178087946067",
-    "\u062f\u0627\u0631\u06cc\u0648\u06342": "63926091058479942",
+    "\u062f\u0627\u0631\u06cc\u06a9": "71076372178147339",
     "\u062f\u0627\u0633\u0648\u0647": "12387472624849835",
     "\u062f\u0627\u0644\u0628\u0631": "60451823714332895",
     "\u062f\u0627\u0645\u06cc\u0646": "50100062518826135",
     "\u062f\u0627\u0646\u0627": "48511238766369097",
+    "\u062f\u0627\u0646\u06cc\u06a9": "67717913151786055",
     "\u062f\u0627\u0648\u0647": "5305844922895340",
-    "\u062f\u0628\u0627\u0644\u06a9": "71510396252618330",
     "\u062f\u062a\u0645\u0627\u062f": "34641719089573667",
     "\u062f\u062a\u0648\u0632\u06cc\u0639": "66726992874614788",
-    "\u062f\u062a\u0648\u0632\u06cc\u0639\u062d": "71980027636215726",
     "\u062f\u062a\u0648\u0644\u06cc\u062f": "18093681647131179",
     "\u062f\u062c\u0627\u0628\u0631": "33406621820337161",
-    "\u062f\u062d\u0627\u0648\u06cc": "43374709930371268",
     "\u062f\u062f\u0627\u0645": "66450490505950110",
-    "\u062f\u062f\u0627\u0646\u0627": "69540585676934415",
     "\u062f\u0631\u0627\u0632\u06a9": "22255783119783047",
-    "\u062f\u0631\u0627\u0632\u06a9\u062d": "38007943162762758",
     "\u062f\u0631\u0627\u0632\u06cc": "16567465928886309",
     "\u062f\u0631\u0633\u0627": "34581754264880199",
     "\u062f\u0631\u0647\u0622\u0648\u0631": "13243992182070788",
     "\u062f\u0631\u0648\u0632": "40262275031537922",
+    "\u062f\u0631\u06cc\u0627": "11285885633824855",
+    "\u062f\u0631\u06cc\u0646": "21077182490095731",
     "\u062f\u0632\u0647\u0631\u0627\u0648\u06cc": "8915450910866216",
     "\u062f\u0633\u0627\u0646\u06a9\u0648": "47348197320716810",
     "\u062f\u0633\u0628\u062d\u0627": "43622578471330344",
-    "\u062f\u0633\u0628\u062d\u0627\u062d": "51063357877632134",
     "\u062f\u0633\u0628\u062d\u0627\u0646": "5866848234665627",
     "\u062f\u0633\u06cc\u0646\u0627": "11432067920374603",
-    "\u062f\u0634\u06cc\u0631\u06cc": "63084741752814852",
     "\u062f\u0634\u06cc\u0645\u06cc": "33603212156438463",
-    "\u062f\u0634\u06cc\u0645\u06cc\u062d": "16630588761222078",
     "\u062f\u0639\u0628\u06cc\u062f": "49054891736433700",
     "\u062f\u0641\u0627\u0631\u0627": "56550776668133562",
     "\u062f\u0641\u0631\u0627": "18303237082155264",
-    "\u062f\u0642\u0627\u0636\u06cc": "64289770858657141",
+    "\u062f\u0642\u0627\u0636\u06cc": "46801030346547943",
     "\u062f\u0644\u0631": "4384288570322406",
-    "\u062f\u0644\u0631\u062d": "42538255636473499",
     "\u062f\u0644\u0642\u0645\u0627": "29247915161590165",
     "\u062f\u0645\u0627\u0648\u0646\u062f": "66142616039907394",
-    "\u062f\u0647\u062f\u0634\u062a": "15374483986949695",
     "\u062f\u067e\u0627\u0631\u0633": "70474983732269112",
     "\u062f\u06a9\u0648\u062b\u0631": "23353689102956991",
-    "\u062f\u06a9\u067e\u0633\u0648\u0644": "52382684379473036",
     "\u062f\u06a9\u06cc\u0645\u06cc": "20024911381434086",
-    "\u062f\u06cc": "44818950263583523",
     "\u062f\u06cc\u0631\u0627\u0646": "69090868458637360",
+    "\u062f\u06cc\u0648\u0627\u0646": "26547362091465395",
     "\u0630\u0648\u0628": "71483646978964608",
+    "\u0631\u0627\u0628\u06cc\u0646": "33527290777160784",
     "\u0631\u0627\u0641\u0632\u0627": "68941822863885255",
     "\u0631\u0627\u0646\u0641\u0648\u0631": "40505767672724777",
     "\u0631\u062a\u0627\u067e": "41048299027409941",
     "\u0631\u0634\u062f": "48287767791629523",
-    "\u0631\u0634\u062f2": "67652526762453420",
     "\u0631\u0645\u0627\u0633": "22002589755112021",
     "\u0631\u0645\u067e\u0646\u0627": "67126881188552864",
     "\u0631\u0646\u06cc\u06a9": "33854964748757477",
     "\u0631\u0648\u06cc\u0634": "15124889255100138",
+    "\u0631\u0648\u06cc\u06cc\u0646": "53059909885484371",
     "\u0631\u06a9\u06cc\u0634": "27952969918967492",
-    "\u0631\u06a9\u06cc\u0634\u062d": "21500060221654011",
     "\u0631\u06cc\u0634\u0645\u06a9": "6478064539164167",
     "\u0632\u0627\u06af\u0631\u0633": "13235547361447092",
     "\u0632\u0628\u06cc\u0646\u0627": "54482686501491508",
     "\u0632\u062f\u0634\u062a": "25180702353416009",
     "\u0632\u0631": "33254899395816171",
     "\u0632\u0631\u0641\u0627\u0645": "33144542989832366",
     "\u0632\u0631\u06cc\u0646": "50139638026536387",
     "\u0632\u0634\u0631\u06cc\u0641": "26547785441834730",
     "\u0632\u0634\u06af\u0632\u0627": "26259366519412975",
+    "\u0632\u0641\u062c\u0631": "36844527173896115",
     "\u0632\u0641\u06a9\u0627": "5427792638736934",
     "\u0632\u0642\u06cc\u0627\u0645": "71290297158948749",
-    "\u0632\u0645\u0627\u0647\u0627\u0646": "4507558419857064",
-    "\u0632\u0645\u0644\u0627\u0631\u062f": "14916489896692147",
     "\u0632\u0645\u06af\u0633\u0627": "5054819322815158",
-    "\u0632\u0646\u062c\u0627\u0646": "12303918642491681",
     "\u0632\u0646\u06af\u0627\u0646": "67170215467608124",
     "\u0632\u067e\u0627\u0631\u0633": "33420285433308219",
     "\u0632\u06a9\u0634\u062a": "7300125658580126",
     "\u0632\u06a9\u0648\u062b\u0631": "42599305106713939",
     "\u0632\u06af\u0644\u062f\u0634\u062a": "10024128313803797",
     "\u0632\u06cc\u062a\u0648\u0646": "28551661889797217",
-    "\u0632\u06cc\u062a\u0648\u06462": "10495792182142221",
     "\u0633\u0622\u0628\u06cc\u06a9": "70883594945615893",
     "\u0633\u0627\u062d\u0644": "62708526880913292",
-    "\u0633\u0627\u0630\u0631\u06cc": "64155926828410021",
     "\u0633\u0627\u0631\u0627\u0628": "4563413583000719",
     "\u0633\u0627\u0631\u0628\u06cc\u0644": "34890845654517313",
     "\u0633\u0627\u0631\u0648\u062c": "25417476013479486",
-    "\u0633\u0627\u0631\u0648\u0645": "15949743338644220",
-    "\u0633\u0627\u0631\u0648\u0645\u062d": "14983273215576895",
-    "\u0633\u0627\u0645\u0627\u0646": "38179358042686391",
+    "\u0633\u0627\u0645\u0627\u0646": "22312990497291517",
     "\u0633\u0627\u0648\u0647": "32347247706508046",
-    "\u0633\u0627\u06cc\u0631\u0627": "62558705479545830",
     "\u0633\u0627\u06cc\u0646\u0627": "64298008532791199",
-    "\u0633\u0628\u0627\u0642\u0631": "24807173016704795",
     "\u0633\u0628\u062c\u0646\u0648": "66295665969375744",
     "\u0633\u0628\u0632\u0648\u0627": "611986653700161",
     "\u0633\u0628\u0647\u0627\u0646": "32525655729432562",
     "\u0633\u062a\u0631\u0627\u0646": "30829203706095076",
-    "\u0633\u062c\u0627\u0645": "20034264486679145",
+    "\u0633\u062c\u0627\u0645": "28328083629154916",
     "\u0633\u062d\u0631\u062e\u06cc\u0632": "51200575796028449",
     "\u0633\u062e\u0627\u0634": "4470657233334072",
     "\u0633\u062e\u0632\u0631": "67327029014085707",
-    "\u0633\u062e\u0648\u0627\u0641": "55959112038778737",
+    "\u0633\u062e\u0646\u062f": "59598536122397373",
     "\u0633\u062e\u0648\u0632": "41974758296041288",
     "\u0633\u062f\u0628\u06cc\u0631": "64341992373049080",
     "\u0633\u062f\u0634\u062a": "27000326841257664",
     "\u0633\u062f\u0648\u0631": "27218386411183410",
     "\u0633\u0631\u0648": "64942549055019553",
-    "\u0633\u0631\u06482": "36273975537785965",
     "\u0633\u0631\u0648\u062f": "11964419322927535",
     "\u0633\u0631\u0686\u0634\u0645\u0647": "35948133957468680",
     "\u0633\u0634\u0631\u0642": "26997316501080743",
     "\u0633\u0634\u0645\u0627\u0644": "6757220448540984",
     "\u0633\u0635\u0641\u0647\u0627": "10568944722570445",
     "\u0633\u0635\u0648\u0641\u06cc": "13227300125161435",
     "\u0633\u063a\u062f\u06cc\u0631": "21096748051392414",
     "\u0633\u063a\u0631\u0628": "52220424531578944",
     "\u0633\u0641\u0627\u0631": "41227201752535311",
     "\u0633\u0641\u0627\u0631\u0633": "15521712617204216",
-    "\u0633\u0641\u0627\u0631\u0648\u062f": "4686607974846832",
-    "\u0633\u0641\u0627\u0633\u06cc": "34721884030854211",
     "\u0633\u0641\u0627\u0646\u0648": "4528607775462304",
     "\u0633\u0642\u0627\u06cc\u0646": "60654872678917533",
-    "\u0633\u0644\u0627\u0631": "61664227282090067",
     "\u0633\u0644\u0627\u0645": "70541934393301867",
-    "\u0633\u0644\u0627\u06452": "9745557270186358",
     "\u0633\u0645\u0627\u0632\u0646": "33808206014018431",
-    "\u0633\u0645\u0627\u06cc\u0647": "43913530989262989",
-    "\u0633\u0645\u062a\u0627\u0632": "58035444268544991",
+    "\u0633\u0645\u0627\u0646": "40473515538481093",
     "\u0633\u0645\u06af\u0627": "46741025610365786",
-    "\u0633\u0646\u0648\u06cc\u0646": "36995197800118822",
     "\u0633\u0646\u06cc\u0631": "14231831499205396",
     "\u0633\u0647\u0631\u0645\u0632": "29747059672582491",
     "\u0633\u0647\u06af\u0645\u062a": "41284516796232939",
-    "\u0633\u067e": "71856634742001725",
-    "\u0633\u067e\u0627\u0633": "39453972158399542",
     "\u0633\u067e\u0627\u0647\u0627": "35669480110084448",
-    "\u0633\u067e\u0631": "17226661368470120",
-    "\u0633\u067e\u0631\u0645\u06cc": "27668158733246204",
     "\u0633\u067e\u06cc\u062f": "45519261544951819",
     "\u0633\u067e\u06cc\u062f\u0627\u0631": "29590002988360984",
     "\u0633\u067e\u06cc\u062f\u0645\u0627": "2161110547458064",
-    "\u0633\u067e\u06cc\u062f\u0645\u06272": "69081464170052337",
-    "\u0633\u06a9\u0627\u0631\u0648\u0646": "15930821245168534",
     "\u0633\u06a9\u0631\u062f": "65321970913593427",
     "\u0633\u06a9\u0631\u0645\u0627": "15472396110662150",
     "\u0633\u06cc\u062a\u0627": "10171945867136336",
     "\u0633\u06cc\u062f\u06a9\u0648": "37281199178613855",
     "\u0633\u06cc\u0633\u062a\u0645": "47749661205825616",
     "\u0633\u06cc\u0644\u0627\u0645": "14617104402836487",
+    "\u0633\u06cc\u0645\u0627\u0646\u0648": "62069100905581368",
     "\u0633\u06cc\u0645\u0631\u063a": "28450080638096732",
     "\u0633\u06cc\u0646\u0627\u062f": "31913287805282551",
     "\u0634\u0627\u0631\u0627\u06a9": "7711282667602555",
     "\u0634\u0627\u0631\u0648\u0645": "3407806799514469",
     "\u0634\u0627\u0645\u0644\u0627": "16959429956899455",
-    "\u0634\u0627\u0645\u0644\u0627\u062d": "14153483684603257",
     "\u0634\u0627\u0648\u0627\u0646": "60247433951600827",
     "\u0634\u0628\u0631\u06cc\u0632": "48753732042176709",
-    "\u0634\u0628\u0631\u06cc\u0632\u062d": "7632696113249142",
     "\u0634\u0628\u0635\u06cc\u0631": "68517032834363488",
     "\u0634\u0628\u0646\u062f\u0631": "35366681030756042",
     "\u0634\u0628\u0647\u0631\u0646": "22667016906590506",
+    "\u0634\u062a\u0627\u0628": "64216772923447100",
     "\u0634\u062a\u0631\u0627\u0646": "51617145873056483",
-    "\u0634\u062a\u0647\u0631\u0627\u0646": "31049085025064185",
-    "\u0634\u062a\u0648\u0644\u06cc": "66210395067138534",
-    "\u0634\u062a\u0648\u06a9\u0627": "38555056423456635",
     "\u0634\u062c\u0645": "6116572045021585",
     "\u0634\u062e\u0627\u0631\u06a9": "70934270174405743",
     "\u0634\u062f\u0648\u0635": "40611478183231802",
-    "\u0634\u0631\u0627\u0632": "33683240001985963",
+    "\u0634\u0631\u0627\u0632": "14031158866706953",
     "\u0634\u0631\u0627\u0646\u0644": "44013656953678055",
-    "\u0634\u0631\u0646\u06af\u06cc": "40025799067544201",
-    "\u0634\u0632\u0646\u06af": "65490886290565185",
-    "\u0634\u0633\u0627\u062e\u062a": "15282093177363578",
     "\u0634\u0633\u062a\u0627": "2400322364771558",
-    "\u0634\u0633\u062a\u0627\u0646": "3173544097113770",
-    "\u0634\u0633\u0645": "59800986739603675",
     "\u0634\u0633\u067e\u0627": "49188729526980541",
     "\u0634\u0633\u06cc\u0646\u0627": "30974710508383145",
-    "\u0634\u0635\u062f\u0641": "204092872752957",
-    "\u0634\u0635\u0641\u0647\u0627": "18346219759153870",
     "\u0634\u063a\u062f\u06cc\u0631": "21772258644715569",
     "\u0634\u0641\u0627": "36899214178084525",
-    "\u0634\u0641\u0627\u0631\u0627": "16673205196919832",
     "\u0634\u0641\u0627\u0631\u0633": "43781018754867729",
     "\u0634\u0641\u0646": "65122215875355555",
-    "\u0634\u0644\u0631\u062f": "56429431740318486",
     "\u0634\u0644\u0639\u0627\u0628": "39116664428676213",
-    "\u0634\u0644\u06cc\u0627": "26025177574491991",
-    "\u0634\u0645\u0648\u0627\u062f": "28251956446987982",
+    "\u0634\u0645\u0644\u06cc": "55862580907068610",
     "\u0634\u0646\u0641\u062a": "14073782708315535",
+    "\u0634\u0647\u0631": "9098178887955847",
     "\u0634\u0648\u06cc\u0646\u062f\u0647": "3493306453706327",
     "\u0634\u067e\u0627\u0631\u0633": "61102694810476197",
     "\u0634\u067e\u0627\u0633": "35178706978554988",
     "\u0634\u067e\u0627\u06a9\u0633\u0627": "11622051128546106",
-    "\u0634\u067e\u062a\u0631\u0648": "71957984642204570",
-    "\u0634\u067e\u062a\u0631\u0648\u062d": "65472108074101196",
     "\u0634\u067e\u062f\u06cc\u0633": "20562694899904339",
-    "\u0634\u067e\u0644\u06cc": "28845264556937486",
     "\u0634\u067e\u0646\u0627": "7745894403636165",
     "\u0634\u06a9\u0627\u0645": "69446612239102459",
-    "\u0634\u06a9\u0628\u06cc\u0631": "56574323121551263",
     "\u0634\u06a9\u0631\u0628\u0646": "27308217070238237",
-    "\u0634\u06a9\u0641": "58602432837130018",
     "\u0634\u06a9\u0644\u0631": "62177651435283872",
     "\u0634\u06af\u0644": "44153164692325703",
     "\u0634\u06af\u0648\u06cc\u0627": "5987841496184505",
     "\u0634\u06cc\u0631\u0627\u0632": "38568786927478796",
     "\u0634\u06cc\u0631\u0627\u0646": "35796086458096255",
-    "\u0635\u0628\u0627": "45392752356003555",
+    "\u0635\u0627\u06cc\u0646\u062f": "45205530868811305",
+    "\u0635\u0628\u0627": "33938004134399485",
+    "\u0635\u062f\u0641": "51285326016186930",
     "\u0635\u0646\u0645": "47125023640770480",
     "\u0635\u0646\u0648\u06cc\u0646": "68203878405672734",
+    "\u0636\u0645\u0627\u0646": "38356837895042988",
     "\u0637\u0644\u0627": "46700660505281786",
-    "\u0637\u0644\u06272": "68285083509815728",
-    "\u0639\u0642\u06cc\u0642": "45452221088910484",
-    "\u0639\u0642\u06cc\u06422": "39559020160976191",
+    "\u0639\u0627\u0644\u06cc\u0633": "34213522001938649",
     "\u0639\u06cc\u0627\u0631": "34144395039913458",
-    "\u0639\u06cc\u0627\u06312": "43531447361624437",
     "\u063a\u0627\u0630\u0631": "35158826900216508",
     "\u063a\u0627\u0644\u0628\u0631": "24303422207378456",
     "\u063a\u0628\u0634\u0647\u0631": "42387718866026650",
-    "\u063a\u0628\u0647\u0627\u0631": "71666521540545716",
     "\u063a\u0628\u0647\u0646\u0648\u0634": "17059960254855208",
     "\u063a\u062f\u0627\u0645": "2254054929817435",
+    "\u063a\u062f\u0627\u0646\u0647": "8234855558996646",
     "\u063a\u062f\u0634\u062a": "2434703913394836",
     "\u063a\u062f\u06cc\u0633": "3492952121304423",
     "\u063a\u0632\u0631": "4369934250728330",
     "\u063a\u0633\u0627\u0644\u0645": "28672095850798501",
     "\u063a\u0634\u0627\u0630\u0631": "59921975187856916",
     "\u063a\u0634\u0627\u0646": "31791737198597563",
     "\u063a\u0634\u0635\u0641\u0627": "61506294208022391",
     "\u063a\u0634\u0647\u062f": "20487994977117557",
     "\u063a\u0634\u0647\u062f\u0627\u0628": "33611155027418901",
-    "\u063a\u0634\u0648\u06a9\u0648": "51294484197536070",
     "\u063a\u0635\u06cc\u0646\u0648": "71758511001096824",
     "\u063a\u0641\u0627\u0631\u0633": "16410724132711490",
-    "\u063a\u0645\u0627\u0631\u06af": "52975109254504632",
+    "\u063a\u0645\u0627\u06cc\u0647": "59461185672081215",
     "\u063a\u0645\u0647\u0631\u0627": "6131290133202745",
     "\u063a\u0645\u06cc\u0646\u0648": "5516102131364383",
-    "\u063a\u0646\u0627\u0628": "42470251469508137",
     "\u063a\u0646\u0648\u0634": "48619517949257749",
     "\u063a\u0648\u06cc\u062a\u0627": "37842793167868642",
     "\u063a\u067e\u0622\u0630\u0631": "45518744711972166",
     "\u063a\u067e\u0627\u06a9": "34032872653290886",
     "\u063a\u067e\u0648\u0646\u0647": "61978776664766359",
     "\u063a\u067e\u06cc\u0646\u0648": "18401147983387689",
     "\u063a\u0686\u06cc\u0646": "44850033148208596",
     "\u063a\u06a9\u0648\u0631\u0634": "62404730109947970",
     "\u063a\u06af\u0631\u062c\u06cc": "31024260997481994",
     "\u063a\u06af\u0644": "22299894048845903",
     "\u063a\u06af\u0644\u0633\u062a\u0627": "64843936383937546",
     "\u063a\u06af\u0644\u067e\u0627": "14312030900097668",
     "\u063a\u06af\u06cc\u0644\u0627": "57300230097485720",
+    "\u0641\u0627\u062e\u0631": "56344907495802692",
     "\u0641\u0627\u0630\u0631": "38547060135156069",
     "\u0641\u0627\u0631\u0627\u06a9": "20865316761157979",
     "\u0641\u0627\u0631\u0633": "25244329144808274",
+    "\u0641\u0627\u0631\u0645\u0627 \u06a9\u06cc\u0627\u0646": "40422084765096890",
     "\u0641\u0627\u0633\u0645\u06cc\u0646": "66701874099226162",
-    "\u0641\u0627\u0641\u0632\u0627": "66021783818850713",
-    "\u0641\u0627\u0641\u0642": "22424135367941584",
-    "\u0641\u0627\u0644\u0648\u0645": "19367527798307032",
+    "\u0641\u0627\u0644\u0648\u0645": "71571639927013317",
     "\u0641\u0627\u0645\u0627": "34673681828119297",
-    "\u0641\u0627\u0647\u0648\u0627\u0632": "44296315953738727",
     "\u0641\u0627\u06cc\u0631\u0627": "65004959184388996",
     "\u0641\u0628\u0627\u0647\u0646\u0631": "66772024744156373",
-    "\u0641\u0628\u0633\u062a\u0645": "4159532151694984",
-    "\u0641\u0628\u06cc\u0631\u0627": "49399017998386087",
     "\u0641\u062a\u0648\u0633\u0627": "55373808401388162",
     "\u0641\u062c\u0627\u0645": "30765727085936322",
     "\u0641\u062c\u0631": "41302553376174581",
     "\u0641\u062c\u0647\u0627\u0646": "45507655586782998",
-    "\u0641\u062c\u0647\u0627\u0646\u062d": "8790413783522890",
-    "\u0641\u062c\u0648\u0634": "64485827086284311",
     "\u0641\u062e\u0627\u0633": "4733285133017464",
     "\u0641\u062e\u0648\u0632": "28864540805361867",
     "\u0641\u0631\u0622\u0648\u0631": "408934423224097",
     "\u0641\u0631\u0627\u0628\u0648\u0631\u0633": "58741071099161284",
     "\u0641\u0631\u0627\u0632": "13666407494621646",
-    "\u0641\u0631\u062f\u0627": "65249046611427924",
-    "\u0641\u0631\u062f\u06272": "12277500298791438",
+    "\u0641\u0631\u0648\u062f": "51017863148152520",
     "\u0641\u0631\u0648\u0633": "54419429862704331",
-    "\u0641\u0631\u0648\u06332": "44152655770483369",
     "\u0641\u0631\u0648\u0633\u06cc\u0644": "44846320603450383",
+    "\u0641\u0631\u0648\u0698": "69817338460284329",
     "\u0641\u0631\u0648\u06cc": "29974853866926823",
     "\u0641\u0632\u0631": "8175784894140974",
     "\u0641\u0632\u0631\u06cc\u0646": "43716452378323683",
-    "\u0641\u0633\u0627": "318005355896147",
     "\u0641\u0633\u0627\u0632\u0627\u0646": "12874072841236826",
     "\u0641\u0633\u0628\u0632\u0648\u0627\u0631": "37284308569715577",
-    "\u0641\u0633\u062f\u06cc\u062f": "20966291817819448",
     "\u0641\u0633\u0631\u0628": "54277068923045214",
     "\u0641\u0633\u0648\u0698": "56375665074210467",
     "\u0641\u0633\u067e\u0627": "8977441217024425",
+    "\u0641\u0635\u0628\u0627": "23557166059925779",
     "\u0641\u063a\u062f\u06cc\u0631": "28147934478934110",
-    "\u0641\u0644\u0627\u062a": "60633055620418060",
     "\u0641\u0644\u0627\u0645\u06cc": "25286509736208688",
+    "\u0641\u0644\u0632\u0641\u0627\u0631\u0627\u0628\u06cc": "43664630566988630",
     "\u0641\u0644\u0648\u0644\u0647": "48623320733330408",
     "\u0641\u0645\u0631\u0627\u062f": "18004480270695404",
     "\u0641\u0645\u0644\u06cc": "35425587644337450",
-    "\u0641\u0646 \u0622\u0648\u0627": "55201604487356053",
-    "\u0641\u0646\u0631\u0698\u06cc": "63965059137798192",
-    "\u0641\u0646\u0641\u062a": "59342912854668427",
+    "\u0641\u0646 \u0627\u0641\u0632\u0627\u0631": "69171897374421261",
+    "\u0641\u0646\u0631": "27276541005386425",
     "\u0641\u0646\u0648\u0627\u0644": "57875847776839336",
     "\u0641\u0646\u0648\u0631\u062f": "56324206651661881",
     "\u0641\u0648\u0644\u0627\u062f": "46348559193224090",
     "\u0641\u0648\u0644\u0627\u0698": "40808043719554948",
     "\u0641\u0648\u0644\u0627\u06cc": "14800142337291217",
-    "\u0641\u0648\u06a9\u0627": "66514709341259550",
-    "\u0641\u0648\u06a9\u06272": "21834964005487744",
     "\u0641\u067e\u0646\u062a\u0627": "68488673556087148",
-    "\u0641\u06a9\u0645\u0646\u062f": "70309338813767186",
     "\u0641\u06af\u0633\u062a\u0631": "8725363201030474",
-    "\u0641\u06cc\u0631\u0648\u0632\u06272": "7371541335638078",
     "\u0641\u06cc\u0631\u0648\u0632\u0647": "66036975502302203",
-    "\u0642\u0627\u0631\u0648\u0645": "10831074117626896",
     "\u0642\u0627\u0633\u0645": "34540569618314880",
-    "\u0642\u062a\u0631\u0628\u062a": "35515916857426389",
-    "\u0642\u062a\u0631\u0628\u062a\u062d": "44166254491540191",
     "\u0642\u062b\u0627\u0628\u062a": "44967158778304588",
-    "\u0642\u062c\u0627\u0645": "28230238564334914",
     "\u0642\u0631\u0646": "39610074039667804",
     "\u0642\u0632\u0648\u06cc\u0646": "15259343650667588",
-    "\u0642\u0634\u0631\u06cc\u0646": "36671655475498480",
     "\u0642\u0634\u0647\u062f": "37631109616997982",
     "\u0642\u0634\u06a9\u0631": "35964395659427029",
     "\u0642\u0634\u06cc\u0631": "71523986304961239",
     "\u0642\u0635\u0641\u0647\u0627": "40411537531154482",
     "\u0642\u0644\u0631\u0633\u062a": "56820995669577571",
     "\u0642\u0645\u0631\u0648": "43342306308122676",
-    "\u0642\u0646\u0642\u0634": "3050342257199174",
     "\u0642\u0646\u06cc\u0634\u0627": "63380098535169030",
-    "\u0642\u0646\u06cc\u0634\u0627\u062d": "55205982891279789",
     "\u0642\u0647\u06a9\u0645\u062a": "14398278072324784",
     "\u0642\u067e\u06cc\u0631\u0627": "67030488744129337",
     "\u0642\u0686\u0627\u0631": "23600798892801694",
-    "\u0642\u06cc\u0633\u062a\u0648": "4267564158935326",
     "\u0644\u0627\u0628\u0633\u0627": "63363116407864462",
-    "\u0644\u0627\u0632\u0645\u0627": "50368344235826302",
     "\u0644\u0628\u062e\u0646\u062f": "31569200988534548",
     "\u0644\u0628\u0648\u062a\u0627\u0646": "30650426998863332",
-    "\u0644\u062e\u0627\u0646\u0647": "56006915451245411",
     "\u0644\u062e\u0632\u0631": "65414507129586385",
     "\u0644\u0633\u0631\u0645\u0627": "55897939403232751",
     "\u0644\u0637\u06cc\u0641": "16422980660132735",
     "\u0644\u0648\u062a\u0648\u0633": "59142194115401696",
-    "\u0644\u0648\u062a\u0648\u0633\u062d": "43455612336353491",
     "\u0644\u067e\u0627\u0631\u0633": "5187018329202415",
-    "\u0644\u067e\u06cc\u0627\u0645": "793710053482057",
-    "\u0644\u06a9\u0645\u0627": "45641540066710190",
     "\u0645\u0627": "29860265627578401",
     "\u0645\u0627\u062f\u06cc\u0631\u0627": "15917865009187760",
     "\u0645\u0627\u0631\u0648\u0646": "53449700212786324",
-    "\u0645\u0627\u0646\u06cc": "61265100181977543",
     "\u0645\u0628\u06cc\u0646": "27922860956133067",
+    "\u0645\u062a\u0627\u0644": "70515583859928047",
     "\u0645\u062b\u0642\u0627\u0644": "32469128621155736",
-    "\u0645\u062b\u0642\u0627\u06442": "19275594209412785",
     "\u0645\u062f\u0627\u0631\u0627\u0646": "65999092673039059",
     "\u0645\u062f\u06cc\u0631": "65576885779918210",
     "\u0645\u062f\u06cc\u0631\u06cc\u062a": "12490072956930435",
-    "\u0645\u0631\u0642\u0627\u0645": "23838634016123354",
     "\u0645\u0631\u0648\u0627\u0631\u06cc\u062f": "31248540252187559",
-    "\u0645\u0639\u06cc\u0627\u0631": "50580753680043015",
     "\u0645\u0641\u0627\u062e\u0631": "4247709727327181",
     "\u0645\u0644\u062a": "13611044044646901",
-    "\u0645\u0645\u0633\u0646\u06cc": "7505990056227818",
+    "\u0645\u0648\u062c": "67141987086032267",
     "\u0645\u06cc\u062f\u06a9\u0648": "33441514568901717",
-    "\u0645\u06cc\u062f\u06a9\u0648\u062d": "18733719742989734",
     "\u0645\u06cc\u0647\u0646": "26543014712914772",
-    "\u0646\u0628\u0631\u0648\u062c": "10843114830116591",
-    "\u0646\u062a\u0648\u0633": "22950683624908253",
+    "\u0646\u0627\u0628": "30582275818828857",
+    "\u0646\u0627\u0631\u06cc\u0646": "30430907997908005",
+    "\u0646\u0627\u0645\u0627": "10411249540376641",
+    "\u0646\u062e\u0631\u06cc\u0633": "46878429508891351",
     "\u0646\u062e\u0644": "27797446447955609",
-    "\u0646\u062e\u06444": "38538071931688978",
     "\u0646\u0634\u0627\u0646": "1241998328504490",
     "\u0646\u0637\u0631\u06cc\u0646": "64699417405634265",
+    "\u0646\u0641\u06cc\u0633": "4626686276232042",
     "\u0646\u0645\u0631\u06cc\u0646\u0648": "30231789123900526",
     "\u0646\u0647\u0627\u0644": "12913156843322499",
     "\u0646\u0648\u0631\u06cc": "19040514831923530",
     "\u0646\u0648\u06cc\u0646": "59866041653103343",
     "\u0646\u06af\u06cc\u0646": "10145129193828624",
-    "\u0646\u06cc\u0631\u0648": "39481233087768672",
-    "\u0647\u0627\u0645\u0631\u0632": "50503654866742146",
+    "\u0646\u06cc\u0627\u0646": "20652241232631918",
+    "\u0646\u06cc\u0644\u06cc": "31188566503248753",
+    "\u0647\u0627\u0645\u0648\u0646": "63514093298304639",
     "\u0647\u0627\u06cc \u0648\u0628": "43362635835198978",
     "\u0647\u062c\u0631\u062a": "5317427172344706",
-    "\u0647\u062c\u0631\u062a\u062d": "52675650218385169",
     "\u0647\u0631\u0645\u0632": "70498485598181604",
     "\u0647\u0645 \u0648\u0632\u0646": "47041908051542008",
-    "\u0647\u0645 \u0648\u0632\u06462": "16888365520630451",
-    "\u0647\u0645\u0627\u06cc": "15494954332657697",
-    "\u0647\u0645\u0627\u06cc2": "45928267225042656",
     "\u0647\u0645\u0631\u0627\u0647": "68635710163497089",
-    "\u0648\u0622\u062a\u0648\u0633": "17269972595370241",
+    "\u0647\u0648\u0634\u06cc\u0627\u0631": "9375107506435996",
+    "\u0647\u06cc\u0648\u0627": "62845384302495432",
     "\u0648\u0622\u0630\u0631": "1358190916156744",
-    "\u0648\u0622\u0631\u06cc\u0646": "24212636157410845",
-    "\u0648\u0622\u0641\u0631": "45991797190214892",
-    "\u0648\u0622\u0641\u0631\u06cc": "19839750988634567",
+    "\u0648\u0622\u0641\u0631\u06cc": "589599697502308",
+    "\u0648\u0622\u0648\u0627": "22490169030401337",
     "\u0648\u0627\u062a\u06cc": "33541897671561960",
-    "\u0648\u0627\u062d\u0635\u0627": "53647874954005806",
-    "\u0648\u0627\u062d\u06cc\u0627": "17284166795866794",
-    "\u0648\u0627\u0631\u0633": "53686258677793038",
     "\u0648\u0627\u0639\u062a\u0628\u0627\u0631": "47841327496247362",
     "\u0648\u0627\u0644\u0628\u0631": "57944184894703821",
-    "\u0648\u0627\u0644\u0628\u0631\u062d": "38188825207508209",
+    "\u0648\u0627\u0644\u0645\u0627\u0633": "36282416082320053",
     "\u0648\u0627\u0645\u06cc\u062f": "52232388263291380",
-    "\u0648\u0627\u0645\u06cc\u0631": "67213778593531096",
-    "\u0648\u0627\u0645\u06cc\u0646": "23843877872814145",
-    "\u0648\u0627\u06cc\u0631\u0627": "9141577977527107",
-    "\u0648\u0627\u06cc\u0631\u0627\u0646": "3149396562827132",
     "\u0648\u0628\u0627\u0632\u0627\u0631": "41286608288791633",
     "\u0648\u0628\u0627\u0646\u06a9": "48010225447410247",
-    "\u0648\u0628\u0631\u0642": "61298636307861167",
     "\u0648\u0628\u0634\u0647\u0631": "13937270451301973",
     "\u0648\u0628\u0635\u0627\u062f\u0631": "28320293733348826",
     "\u0648\u0628\u0645\u0644\u062a": "778253364357513",
     "\u0648\u0628\u0647\u0645\u0646": "18063426072758458",
-    "\u0648\u0628\u0647\u0645\u06462": "69758610266463962",
     "\u0648\u0628\u0648\u0639\u0644\u06cc": "28328710198554144",
     "\u0648\u0628\u06cc\u0645\u0647": "11773403764702778",
     "\u0648\u062a\u062c\u0627\u0631\u062a": "63917421733088077",
     "\u0648\u062a\u0639\u0627\u0648\u0646": "5920901446678689",
     "\u0648\u062a\u0648\u0633": "68117765376081366",
     "\u0648\u062a\u0648\u0633\u0645": "17528249960294496",
     "\u0648\u062a\u0648\u0634\u0647": "54676885047867737",
     "\u0648\u062a\u0648\u0635\u0627": "2944500421562364",
     "\u0648\u062a\u0648\u06a9\u0627": "47232550823972469",
-    "\u0648\u062b\u062e\u0648\u0632": "40043919653526083",
-    "\u0648\u062b\u0646\u0648": "44986797317463049",
-    "\u0648\u062b\u0646\u0648\u062d": "53373305024733919",
-    "\u0648\u062b\u0648\u0642": "59839275647597021",
-    "\u0648\u062c\u0627\u0645\u06cc": "57600064931636077",
-    "\u0648\u062d\u0627\u0641\u0638": "5128151910501174",
-    "\u0648\u062d\u06a9\u0645\u062a": "12777578088653944",
     "\u0648\u062e\u0627\u0631\u0632\u0645": "7395271748414592",
     "\u0648\u062e\u0627\u0648\u0631": "47333458678352378",
-    "\u0648\u062f\u0627\u0646\u0627": "66424163876658304",
     "\u0648\u062f\u06cc": "43966385447049549",
-    "\u0648\u0631\u0627\u0632\u06cc": "60079434631497942",
     "\u0648\u0631\u0646\u0627": "7385624172574740",
     "\u0648\u0633\u0627\u062e\u062a": "25514780181345713",
-    "\u0648\u0633\u0627\u0644\u062a": "23175320865252772",
     "\u0648\u0633\u0627\u067e\u0627": "37614886280396031",
     "\u0648\u0633\u0628\u062d\u0627\u0646": "43283802997035462",
-    "\u0648\u0633\u062f\u06cc\u062f": "41713045190742691",
-    "\u0648\u0633\u0631\u0645\u062f": "43291783149314349",
-    "\u0648\u0633\u0646\u0627": "24662567615903665",
     "\u0648\u0633\u067e\u0647": "2328862017676109",
-    "\u0648\u0633\u067e\u0647\u062d": "54287510798838485",
     "\u0648\u0633\u067e\u0647\u0631": "114312662654155",
     "\u0648\u0633\u06a9\u0627\u0628": "11258722998911897",
-    "\u0648\u0633\u06cc\u0646": "56591881518499520",
     "\u0648\u0633\u06cc\u0646\u0627": "45050389997905274",
-    "\u0648\u0634\u0645\u0627\u0644": "9761381741308262",
-    "\u0648\u0634\u0647\u0631": "41379697187196382",
     "\u0648\u0635\u0646\u0627": "46982154647719707",
     "\u0648\u0635\u0646\u062f\u0648\u0642": "37204371816016200",
     "\u0648\u0635\u0646\u0639\u062a": "57309221039930244",
     "\u0648\u0637\u0648\u0628\u06cc": "3955332316338258",
     "\u0648\u063a\u062f\u06cc\u0631": "26014913469567886",
-    "\u0648\u0641\u062a\u062e\u0627\u0631": "27148572013604038",
-    "\u0648\u0644\u0627\u0646\u0627": "66830065858417081",
     "\u0648\u0644\u0628\u0647\u0645\u0646": "48287670503317419",
-    "\u0648\u0644\u062a\u062c\u0627\u0631": "34621618468546063",
-    "\u0648\u0644\u0631\u0627\u0632": "12901875871456398",
+    "\u0648\u0644\u062a\u062c\u0627\u0631": "50011948410571353",
     "\u0648\u0644\u0633\u0627\u067e\u0627": "45174198424472334",
     "\u0648\u0644\u0634\u0631\u0642": "31078457170311964",
     "\u0648\u0644\u0635\u0646\u0645": "71744682148776880",
     "\u0648\u0644\u063a\u062f\u0631": "23086515493897579",
-    "\u0648\u0644\u0642\u0645\u0627\u0646": "31959715133485440",
     "\u0648\u0644\u0645\u0644\u062a": "11403770140000603",
     "\u0648\u0644\u067e\u0627\u0631\u0633": "48241092863917835",
     "\u0648\u0644\u06a9\u0627\u0631": "61469668095573716",
-    "\u0648\u0644\u06cc\u0632": "20946530370469828",
     "\u0648\u0645\u062f\u06cc\u0631": "30447901674051381",
-    "\u0648\u0645\u0634\u0627\u0646": "35369183060321179",
     "\u0648\u0645\u0639\u0627\u062f\u0646": "58931793851445922",
-    "\u0648\u0645\u0639\u0627\u062f\u0646\u062d": "66240430785255272",
     "\u0648\u0645\u0639\u0644\u0645": "6847536925606808",
-    "\u0648\u0645\u0644\u062a": "10055255678920880",
-    "\u0648\u0645\u0644\u0644": "24644999329120295",
     "\u0648\u0645\u0644\u06cc": "41796741644273824",
-    "\u0648\u0645\u0647\u0627\u0646": "58964593134314938",
+    "\u0648\u0645\u0647\u0627\u0646": "47026464823464687",
     "\u0648\u0646\u0641\u062a": "33931218652865616",
     "\u0648\u0646\u0648\u06cc\u0646": "47302318535715632",
     "\u0648\u0646\u06cc\u0631\u0648": "62603302940123327",
     "\u0648\u0646\u06cc\u06a9\u06cc": "25336820825905643",
-    "\u0648\u0646\u06cc\u06a9\u06cc\u062d": "26090464295830176",
     "\u0648\u0647\u0627\u0645\u0648\u0646": "19348717261145458",
-    "\u0648\u0647\u0646\u0631": "60783654574662426",
     "\u0648\u0647\u0648\u0631": "25215182208950217",
     "\u0648\u067e\u0627\u0631\u0633": "33293588228706998",
     "\u0648\u067e\u0627\u0633\u0627\u0631": "9536587154100457",
     "\u0648\u067e\u062a\u0631\u0648": "59486059679335017",
     "\u0648\u067e\u062e\u0634": "7183333492448248",
-    "\u0648\u067e\u0633\u0627": "11560002870991149",
     "\u0648\u067e\u0633\u062a": "22087269603540841",
     "\u0648\u067e\u0648\u06cc\u0627": "24785665268004766",
-    "\u0648\u067e\u0648\u06cc\u0627\u062d": "24864955678633428",
-    "\u0648\u06a9\u0627\u062f\u0648": "56717416662584054",
     "\u0648\u06a9\u0627\u0631": "47996917271187218",
     "\u0648\u06a9\u0628\u0647\u0645\u0646": "64973252728260903",
-    "\u0648\u06af\u0631\u062f\u0634": "7920014658832193",
+    "\u0648\u06a9\u063a\u062f\u06cc\u0631": "40553302624764543",
     "\u0648\u06af\u0633\u062a\u0631": "43951910415124966",
-    "\u0648\u06af\u0633\u062a\u0631\u062d": "39722227263011028",
-    "\u0648\u06cc\u0633\u0627": "69472361926040823",
     "\u0648\u06cc\u0633\u062a\u0627": "58852293795036597",
     "\u067e\u0627\u062f\u0627": "67522512921942106",
     "\u067e\u0627\u062f\u0627\u0634": "43267179898797137",
-    "\u067e\u0627\u062f\u0627\u06342": "24198960406596014",
     "\u067e\u0627\u0631\u062a\u0627": "72044846109864381",
     "\u067e\u0627\u0631\u0633": "6110133418282108",
     "\u067e\u0627\u0631\u0633\u0627\u0646": "23441366113375722",
     "\u067e\u0627\u0631\u0633\u06cc\u0627\u0646": "9481703061634967",
-    "\u067e\u0627\u0631\u0633\u06cc\u0627\u0646\u062d": "50201903966895115",
     "\u067e\u0627\u0631\u0646\u062f": "70595828753641750",
     "\u067e\u0627\u0633\u0627": "63580313877463104",
     "\u067e\u0627\u0644\u0627\u06cc\u0634": "67675656072510693",
     "\u067e\u0627\u06a9\u0634\u0648": "62786156501584862",
+    "\u067e\u0627\u06cc\u0627": "55070742656326885",
     "\u067e\u062a\u0627\u06cc\u0631": "41935584690956944",
+    "\u067e\u062a\u0631\u0648\u0622\u0628\u0627\u0646": "18757639286384873",
+    "\u067e\u062a\u0631\u0648\u0622\u06af\u0627\u0647": "37828981835497620",
+    "\u067e\u062a\u0631\u0648\u062f\u0627\u0631\u06cc\u0648\u0634": "2019449432639594",
+    "\u067e\u062a\u0631\u0648\u0635\u0628\u0627": "30762816122316539",
     "\u067e\u062a\u0631\u0648\u0644": "69143674941561637",
+    "\u067e\u062a\u0631\u0648\u0645\u0627": "7670135462634715",
     "\u067e\u062e\u0634": "12638840758449459",
     "\u067e\u062f\u0631\u062e\u0634": "24079409192818584",
+    "\u067e\u0631\u062a\u0648": "48818952524587858",
     "\u067e\u0631\u062f\u0627\u062e\u062a": "59607545337891226",
     "\u067e\u0631\u062f\u06cc\u0633": "15039949673085566",
-    "\u067e\u0631\u0633\u067e\u0648\u0644\u06cc\u0633": "55289848471625247",
     "\u067e\u0633\u0647\u0646\u062f": "10120557300120078",
-    "\u067e\u0634\u0627\u0647\u0646": "44052047028305231",
-    "\u067e\u0644\u0627\u0633\u062a": "52593789542874668",
-    "\u067e\u0644\u0627\u0633\u062a\u062d": "18850167694315175",
     "\u067e\u0644\u0627\u0633\u06a9": "57722642338781674",
-    "\u067e\u0644\u0648\u0644\u0647": "29316948750916349",
+    "\u067e\u0648\u06cc\u0627": "48970598895465763",
     "\u067e\u06a9\u0631\u0645\u0627\u0646": "23214828924506640",
     "\u067e\u06a9\u0648\u06cc\u0631": "7235435095059069",
+    "\u067e\u06cc \u067e\u0627\u062f": "26316376625263940",
+    "\u067e\u06cc\u0631\u0648\u0632": "41746336706469006",
     "\u067e\u06cc\u0632\u062f": "32784604551756178",
     "\u0686\u0627\u0641\u0633\u062a": "23936607891892333",
     "\u0686\u062e\u0632\u0631": "41122066907413786",
     "\u0686\u062f\u0646": "12329519546621752",
     "\u0686\u0641\u06cc\u0628\u0631": "64358061873294912",
-    "\u0686\u0646\u0648\u067e\u0627": "43023243844297350",
     "\u0686\u06a9\u0627\u0631\u0646": "53113471126689455",
     "\u0686\u06a9\u0627\u0648\u0647": "24254843881948059",
     "\u0686\u06a9\u0627\u067e\u0627": "28957320033282870",
-    "\u06a9\u0627\u0628\u06af\u0646": "10654052153538617",
-    "\u06a9\u0627\u0630\u0631": "49353447565507376",
+    "\u06a9\u0627\u062c": "42670427020727409",
     "\u06a9\u0627\u0631\u0627": "71843282162462661",
-    "\u06a9\u0627\u0631\u06272": "10368700486623325",
     "\u06a9\u0627\u0631\u062f\u0627\u0646": "65023851436340574",
     "\u06a9\u0627\u0631\u06cc\u0633": "69067576215760005",
-    "\u06a9\u0627\u0631\u06cc\u0646": "16056283141617755",
-    "\u06a9\u0627\u0632\u0631\u0648": "16777570760181431",
     "\u06a9\u0627\u0633\u067e\u06cc\u0646": "28431095903407567",
     "\u06a9\u0627\u0644\u0627": "44549439964296944",
     "\u06a9\u0627\u0645\u0627": "4942127026063388",
     "\u06a9\u0627\u0645\u06cc\u0627\u0628": "16040900750729921",
     "\u06a9\u0627\u0648\u0647": "60350996279289099",
-    "\u06a9\u0627\u06cc\u062a\u0627": "45608932669358493",
-    "\u06a9\u0627\u06cc\u0632\u062f": "58810336532668771",
-    "\u06a9\u0628\u0627\u062f\u0647": "55979741213594029",
     "\u06a9\u0628\u0627\u0641\u0642": "43256212620530446",
     "\u06a9\u062a\u0631\u0627\u0645": "24085906177899789",
+    "\u06a9\u062a\u0648\u0633\u0639\u0647": "23374429962331387",
     "\u06a9\u062a\u0648\u06a9\u0627": "65671173927025645",
-    "\u06a9\u062a\u0648\u06a9\u0627\u062d": "6700951770411072",
     "\u06a9\u062d\u0627\u0641\u0638": "32257753560585502",
     "\u06a9\u062e\u0627\u06a9": "16405556680571453",
     "\u06a9\u062f\u0645\u0627": "3623921205367364",
     "\u06a9\u0631\u0627\u0632\u06cc": "57086055330734195",
     "\u06a9\u0631\u0645\u0627\u0634\u0627": "38437201078089290",
     "\u06a9\u0631\u0645\u0627\u0646": "50792786683910016",
+    "\u06a9\u0631\u0648\u0645\u06cc\u062a": "49632601495766480",
     "\u06a9\u0631\u0648\u06cc": "22787503301679573",
-    "\u06a9\u0632\u063a\u0627\u0644": "28291104595448527",
     "\u06a9\u0633\u0627\u0648\u0647": "25001509088465005",
     "\u06a9\u0633\u0627\u067e\u0627": "28325731560106431",
     "\u06a9\u0633\u0631\u0627": "4614779520007780",
     "\u06a9\u0633\u0631\u0627\u0645": "20560887114747719",
     "\u06a9\u0633\u0639\u062f\u06cc": "29122854902865456",
     "\u06a9\u0634\u0631\u0642": "42690477960659940",
-    "\u06a9\u0635\u062f\u0641": "42696242981550091",
     "\u06a9\u0637\u0628\u0633": "8977369674477111",
-    "\u06a9\u0641\u0631\u0622\u0648\u0631": "49627523909849331",
     "\u06a9\u0641\u0631\u0627": "23837844039713715",
-    "\u06a9\u0641\u067e\u0627\u0631\u0633": "19471788163911687",
-    "\u06a9\u0642\u0632\u0648\u06cc": "63499217872110599",
     "\u06a9\u0644\u0631": "1822787329898392",
     "\u06a9\u0644\u0648\u0646\u062f": "32678431934327184",
-    "\u06a9\u0645\u0627\u0633\u0647": "67690708346979840",
     "\u06a9\u0645\u0631\u062c\u0627\u0646": "50633804639547462",
-    "\u06a9\u0645\u0646\u062f2": "71516048161401340",
-    "\u06a9\u0645\u0646\u062f4": "55266031060966810",
     "\u06a9\u0645\u0646\u06af\u0646\u0632": "50341528161302545",
-    "\u06a9\u0645\u0646\u06af\u0646\u0632\u062d": "66630516232885208",
-    "\u06a9\u0645\u06cc\u0646\u0627": "54263829393913132",
     "\u06a9\u0646\u0648\u0631": "20411759370751096",
-    "\u06a9\u0647\u0631\u0627\u0645": "25631699615003698",
     "\u06a9\u0647\u0631\u0628\u0627": "25559236668122210",
-    "\u06a9\u0647\u0631\u0628\u06272": "44215112373339904",
     "\u06a9\u0647\u0645\u062f\u0627": "67206358287598044",
     "\u06a9\u0648\u062b\u0631": "22275596386264204",
-    "\u06a9\u0648\u0631\u0632": "42049553761321495",
     "\u06a9\u0648\u06cc\u0631": "43545527030854340",
     "\u06a9\u067e\u0627\u0631\u0633": "9698674686691945",
     "\u06a9\u067e\u0631\u0648\u0631": "22941065011246116",
     "\u06a9\u067e\u0634\u06cc\u0631": "57639364758870873",
     "\u06a9\u0686\u0627\u062f": "18027801615184692",
     "\u06a9\u06af\u0627\u0632": "62346804681275278",
     "\u06a9\u06af\u0644": "35700344742885862",
     "\u06a9\u06af\u0647\u0631": "30703140537034664",
     "\u06a9\u06cc \u0628\u06cc \u0633\u06cc": "62977319271289925",
-    "\u06a9\u06cc\u0627\u06462": "53254637903825194",
-    "\u06a9\u06cc\u0633\u0648\u0646": "49953653111442595",
-    "\u06a9\u06cc\u0645\u06cc\u0627": "27814844870305607",
+    "\u06a9\u06cc\u0645\u06cc\u0627": "14427168056799610",
     "\u06a9\u06cc\u0645\u06cc\u0627\u062a\u06a9": "39884565732277052",
+    "\u06af\u0627\u0631\u0627\u0646\u062a\u06cc": "971068957336171",
     "\u06af\u062f\u0646\u0627": "10114441830266109",
-    "\u06af\u0634\u0627\u0646": "70391097626818082",
-    "\u06af\u0646\u0628\u062f": "7670135462634715",
+    "\u06af\u0644\u062f\u06cc\u0631\u0627": "54715710303837090",
+    "\u06af\u0646\u062c": "58514988269776425",
+    "\u06af\u0646\u062c\u06cc\u0646": "57728534324022361",
     "\u06af\u0646\u062c\u06cc\u0646\u0647": "47101579271117172",
-    "\u06af\u0646\u062c\u06cc\u0646\u06472": "11273669187884551",
-    "\u06af\u0646\u06af\u06cc\u0646": "59470107928175959",
     "\u06af\u0648\u0647\u0631": "12390706505809150",
-    "\u06af\u0648\u0647\u06312": "35757908588761589",
     "\u06af\u0648\u0647\u0631\u0627\u0646": "65018804181564924",
-    "\u06af\u067e\u0627\u0631\u0633": "59848307608894801",
     "\u06af\u06a9\u0648\u062b\u0631": "66599109405217136",
-    "\u06af\u06a9\u06cc\u0634": "44665761767777759",
-    "\u06cc\u0627\u0631\u0627": "45284811973404357",
-    "\u06cc\u0627\u0642\u0648\u062a": "1438514795814416",
-    "\u06cc\u0627\u0642\u0648\u062a2": "29884261753438378"
+    "\u06cc\u0627\u0631\u0627": "45284811973404357"
 }
```

### Comparing `pytse_filter-1.33/src/pytse_filter.egg-info/PKG-INFO` & `pytse_filter-1.42/src/pytse_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytse_filter
-Version: 1.33
+Version: 1.42
 Summary: A user-friendly project to filter symbols of Tehran Stock Exchange
 Home-page: https://github.com/farhad-mohammadi/pytse_filter
 Author: Farhad Mohammadi
 Author-email: farhad.mohammadi60@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,15 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: tzdata==2024.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: jalali_core==1.0.0
 Requires-Dist: jdatetime==5.0.0
+Requires-Dist: lxml==5.2.1
 
 # pytse-filter: Tehran Stock Exchange Data Processing Library
 
 Welcome to the **pytse-filter** library, a Python package designed for processing and analyzing Tehran Stock Exchange (TSE) symbol data through user-defined text filters. This library simplifies the task of filtering TSE data based on various conditions, making it an essential tool for traders and analysts.
 
 ## Prerequisites
```

### Comparing `pytse_filter-1.33/src/pytse_filter.egg-info/SOURCES.txt` & `pytse_filter-1.42/src/pytse_filter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

